  ### Produktion
<sub>Applikationen kommer isoleras i en [Docker](https://www.docker.com/)-miljö med fyra kontainrar. En vardera för Node-servern, React-klienten, en lokal MongDB databas och NGINX. Applikationen är då förberedd att produktionsättas lokalt hos Futurum Digital och exponeras genom [NGINX](https://www.nginx.com/resources/wiki/).</sub>

  ### Språk och tekniker
<sub>Vi använder Typescript genomgående på både server samt klient.</sub> 

<sub>I samarbete med Futurum Digital har vi valt att använda [NodeJS](https://nodejs.org/en/about/) som plattform till servern tillsammans med följande bibliotek: [Express](https://expressjs.com/) för hosting och routing, IMAP för att hantera mail-trafik in från servern, Gmails API för mail-trafik ut från servern, [SocketIo](https://www.npmjs.com/package/socket.io) för Websocketkommunikationen internt mellan klient och server, XOAuth2 för autentisering mot Gmail, [Mongoose](https://www.npmjs.com/package/mongoose) till dokumentdatabasen samt ett antal andra hjälpbibliotek (se package.json i `node` mappen).</sub>

<sub>Till att rendera och presentera data på klientsidan har vi valt att använda oss av [ReactJS](https://reactjs.org/) och [SASS](https://sass-lang.com/) till stilsättning. Vi använder även [Webpack](https://webpack.js.org/) för att bygga ihop alla filer och [Webpack-dev-server](https://github.com/webpack/webpack-dev-server) för att efterlikna kommande produktionsmiljö under utveckling och göra arbetet smidigare. I all CSS som skrivs i SASS-filerna följer vi också riktlinjerna för [BEM](http://getbem.com/introduction/).</sub>

#### Teknik-resurser
<sub>**[IMAP](https://en.wikipedia.org/wiki/Internet_Message_Access_Protocol)** - Förkortningen står för Internet Message Access Protocol, och är det standardprotokoll som används av mailklienter för att kommunicera med en mailserver över TCP/IP. I vårt fall är mailservern *Gmails* mailserver, och vi använder oss av en IMAP-klient-modul för NodeJS som en abstraktion över den rena IMAP-kommunikationen för att agera som en klient mot denna mailserver. Dokumentation för denna modul finns [här](https://github.com/mscdex/node-imap), och de enda förkunskaper som behövs för att ta den till sig är en viss förkunskap om [NodeJS](https://nodejs.org/en/docs/) och [Express](https://expressjs.com/).</sub>

<sub>**[OAuth](https://developers.google.com/gmail/imap/xoauth2-protocol) / [XOAuth2](https://developers.google.com/gmail/imap/xoauth2-protocol#the_sasl_xoauth2_mechanism)** - Autentieringen mot mailservern görs genom att en OAuth2 Access Token skickas till mailservern genom Googles implementation av en XOAuth2-mekanism (teorin bakom detta går att läsa mer om [här](https://developers.google.com/gmail/imap/xoauth2-protocol#the_sasl_xoauth2_mechanism)). Detta innebär att vi först måste införskaffa en Access Token för det mailkonto vi vill få tillgång till, vilket görs med hjälp av [Passports OAuth2-abstraktion för Google](https://github.com/jaredhanson/passport-google-oauth2). Detta steg fungerar också som en autentiering av att användaren har tillgång till mailadressen mot vilken de vill koppla upp vår applikation. Den Access och Refresh-token vi då får tillgång till transformeras med hjälp av en [OAuth2-XOAuth modul](https://github.com/andris9/xoauth2) för NodeJS, och skickas med den ovan nämnda IMAP-modulen. För att lära sig om detta krävs en viss förståelse kring vad ett [OAuth2-flöde är](http://www.bubblecode.net/en/2016/01/22/understanding-oauth2/), samt hur [Passport kan hjälpa till med det](http://www.passportjs.org/docs/oauth/). För att göra vår applikation till en klient i detta OAuth-flöde behöver den registreras som ett projekt i [Googles Developer Console](https://console.cloud.google.com/). Utöver detta räcker det med att läsa dokumentationen för de använda modulerna, samt [Googles OAuth2/XOAuth-dokumentation](https://developers.google.com/gmail/imap/xoauth2-protocol) om man vill få en förståelse för vad som händer under huven.</sub>

<sub>**[Gmail-API](https://developers.google.com/gmail/api/guides/)** - För att skicka mail från vår server å användarens vägnar kommunicerar vi direkt med Googles API. För att göra detta behöver Gmail-API:t aktiveras i vårt Google projekt som vi skapade ovan. Vi använder oss sedan av en NodeJS-modul som ett abstraktionslager över API:et. Dokumentation för denna modul finns [här](https://github.com/google/google-api-nodejs-client/). Mailen [base64](https://en.wikipedia.org/wiki/Base64)-enkodas och följer [RFC2822-standarden](https://tools.ietf.org/html/rfc2822#appendix-A.2). Det bästa sättet att lära sig mer om det här är att läsa Googles API-dokumentation, läsa modulens dokumentation, titta på RFC-standarden, och sedan prova sig fram.</sub>

  ### Design
<sub>**Databasdesign**</sub>

<sub>[MongoDB](https://www.mongodb.com/what-is-mongodb) är en dokumentdatabas som lämpar sig väl till mindre datamängder. Vi har skapat modeller som överensstämmer med dataflödena i applikationen, där uppdelningen är en "ticket"-modell, "customer"-modell och en "settings"-modell. En "ticket" skapas som ett eget objekt med kundinformation, datum, status, tilldelning till anställd och en lista med konversationen.</sub>

<sub>**Arkitekturella mönster**</sub>

<sub>På designnivå har vi strukturerat upp sockethanteringen i ett [factory pattern](https://en.wikipedia.org/wiki/Factory_(object-oriented_programming)) på både server- och klientsidan.</sub>

<sub>Klienten är strukturerad i enlighet med en klassisk Reactdesign bestående av kontainrar- och komponenter, som bygger upp en ["single-page-application"](https://en.wikipedia.org/wiki/Single-page_application).</sub>

<sub>Event emitters sköter dataleverans till `app.ts` som agerar likt ett nav eller en huvudkontroller för hela serverapplikationen. I emailhanteringen har detta implementerats genom [events-eventemitter](https://www.npmjs.com/package/EventEmitter) medan socketfactory-klassen levererar data genom typade kanaler med callback funktionalitet.</sub>

<sub>För att få så refaktorerbar kod som möjligt har vi hållit oss till att modellera stora delar av koden genom att skapa klasser som ärver av lämpliga och mestadels egenkonstruerade [interfaces](https://www.typescriptlang.org/docs/handbook/interfaces.html).</sub>

***

