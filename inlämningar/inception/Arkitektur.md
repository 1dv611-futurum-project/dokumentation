## Arkitektur
<sub>**Futurum Support Application är en webbapplikation strukturerad i en layered arkitektur och byggd i Node Express och React genom typescript. Där det arkitekturella mottot är "separation of concern".**</sub>

<sub>_Val av arkitektur och designmönster grundar sig först och främst i kundens önskan att få ett system som liknar organisationens befintliga system i tekniker liksom utseende. Kunden får det då enkelt att följa utvecklingsprocessen och därmed en möjlighet till kontinuerligt inflytande. Det förenklar även framtida vidareutveckling och integration av systemet._</sub>

<sub>En layered arkitektur strukturerad i MVC lämpar sig väl för att skapa en webbapplikation för ärendehantering och gör subsystemens och komponenternas ansvar enkla att separera och utveckla parallelt. För att minimera utvecklingsrisker i teamet har vi valt att isolera server från klient i separata dockerkontainrar, där klienten har fullt ansvar för det grafiska gränssnittet medans servern sköter autentisering, hantering av inkomna mail och datapersistens. Samverkan mellan dessa två subsystemen sker genom websocket vilket möjliggör att i realtid leverera nyinkomna mail upp till klienten för snabb administration. </sub>

<sub>För att hedra kundens önskan om att få ett system som är enkelt att underhålla har vi valt att använda tslint för genomgående stylistisk/syntaktisk kvalitet.</sub>

![Mockup architecture](https://go.gliffy.com/go/share/image/safym22fpbukh9ljeobv.png?utm_medium=live-embed&utm_source=custom "Mockup")
<sub>[***Kommentera***](https://go.gliffy.com/go/share/s88e9hjfbh306wqcfuva)</sub>

## Klassdiagram

![Klass mockup](https://go.gliffy.com/go/share/image/sr6iclkcbyywsisdyw0a.png?utm_medium=live-embed&utm_source=custom)
<sub>[***Kommentera***](https://go.gliffy.com/go/share/slhwa5vns09dme78nupu)</sub>

### Node
![Klassdiagram node](https://go.gliffy.com/go/share/image/s12bghk6ug6ravy6316x.png?utm_medium=live-embed&utm_source=custom)


* <sub>React</sub>
   * <sub>SPA med hashrouting</sub>
   * <sub>Admins gränssnitt för ärendehantering</sub>
   * <sub>Eventemitter/reciever genom websocket till serverappen.</sub>
* <sub>Node</sub>
   * <sub>Authentisering genom OAuth2 Google mail.</sub>
   * <sub>IMAP events google mail.</sub>
   * <sub>Databashantering till och från lokal MongoDB.</sub>
   * <sub>Eventemitter/reciever genom websocket till klientappen.</sub>
