<sub>_Märk väl, för vedertagna mjukvarutermer använder vi engelska._</sub>

### <sub>Arkitekturellt signifikanta krav</sub>
* <sub>Klient-server arkitektur</sub>
   * <sub>Komponent pattern - klientsida</sub>
   * <sub>Lagerarkitektur - serversida</sub>
   * <sub>Dependency injection av websocket middleware</sub>
* <sub>Depedency injection av betydelsefulla middleware</sub>
* <sub>Kommunikationsdesign patterns</sub>
   * <sub>Eventemitter pattern</sub>
   * <sub>Callback pattern</sub>
* <sub>Modellering med interface arvsstruktur</sub>
* <sub>Factory designpattern för lämpliga middleware</sub>

<sub>**Futurum Support är en webbapplikation strukturerad i en layered arkitektur och byggd i NodeJS med Express och React genom Typescript, där det arkitekturella mottot är "separation of concern".**</sub>

<sub>_Val av arkitektur och designmönster grundar sig först och främst i kundens önskan att få ett system som liknar organisationens befintliga system i tekniker liksom utseendet. Kunden kan då enklare följa utvecklingsprocessen och får därmed en möjlighet till kontinuerligt inflytande. Det förenklar även framtida vidareutveckling och integration av systemet._</sub>

<sub>En layered arkitektur strukturerad i MVC lämpar sig väl för att skapa en webbapplikation för ärendehantering och gör undersystemens och komponenternas ansvar enkla att separera och utveckla parallelt. För att minimera utvecklingsrisker i gruppen har vi valt att isolera server och klient ifrån varandra i separata docker-containrar, där klienten har fullt ansvar för det grafiska gränssnittet medan servern sköter autentisering, hantering av inkomna mail och datapersistens. Kommunikationen mellan dessa två undersystemen sker genom en Websocket vilket gör det möjligt att i realtid kunna leverera inkomna mail till klienten för snabb administration. </sub>

<sub>För att hedra kundens önskan om att få ett system som är enkelt att underhålla har vi även valt att använda TSlint för genomgående stylistisk/syntaktisk kvalitet.</sub>

***<sub>Övergripande subsystem</sub>***
* <sub>React-klient</sub>
   * <sub>SPA med browser history</sub>
   * <sub>Admin-gränssnitt för ärendehantering</sub>
   * <sub>Eventemitter/receiver genom Websocket till servern</sub>
* <sub>NodeJS-server</sub>
   * <sub>Authentisering genom OAuth2 via Google mail</sub>
   * <sub>IMAP events Google mail</sub>
   * <sub>Databashantering till och från lokal MongoDB</sub>
   * <sub>Eventemitter/receiver genom Websocket till klienten</sub>


### <sub>Övergripande arkitektur</sub>
<sub>_Observera att klassdiagram och skisser till viss del kan skilja sig från nuvarande implementation (se datum). Vid slutleverans av systemet kommer samtliga modeller uppdateras och stämma överens med faktisk implementation._</sub><br>
![Mockup architecture](https://go.gliffy.com/go/share/image/safym22fpbukh9ljeobv.png?utm_medium=live-embed&utm_source=custom "Mockup")
<sub>[***Kommentera***](https://go.gliffy.com/go/share/s88e9hjfbh306wqcfuva) _senast ändrad i iteration 2._</sub>
<br>

![Mockup](https://go.gliffy.com/go/share/image/sr6iclkcbyywsisdyw0a.png?utm_medium=live-embed&utm_source=custom)
<sub>[***Kommentera***](https://go.gliffy.com/go/share/slhwa5vns09dme78nupu) _senast ändrad i iteration 2._</sub>
<br>

### <sub>Klassdiagram</sub>
**<sub>Server</sub>**
![Server](https://go.gliffy.com/go/share/image/s12bghk6ug6ravy6316x.png?utm_medium=live-embed&utm_source=custom)
<sub>_Senast ändrad i iteration 4._</sub>
<br><br><br>
**<sub>Klient</sub>**
![Klient](https://go.gliffy.com/go/share/image/sdo18fasym3ps8o2mj30.png?utm_medium=live-embed&utm_source=custom)
<sub>[***Kommentera***](https://go.gliffy.com/go/share/shaxllsik5dip9p0eiw0) _senast ändrad i iteration 4._</sub>
<br>

