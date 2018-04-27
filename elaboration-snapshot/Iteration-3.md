# Iteration 3

## Föregående iteration

### Sammanfattning av föregående iteration
<sub>Vi har blivit klara med Inception-fasen genom att se till att vår dokumentation är uppdaterad och strukturen kring den fungerar bra. Vi har blivit säkra på hur vi arbetar med vår versionshantering och olika features, samt ha röjt undan de stora tekniska riskerna, vilket i detta fall betyder att vi fått Docker att fungera för samtliga gruppmedlemmar, har fått igång uppkopplingen mot kundens mail, och fått upp ett skelett till React-applikationen. Vi har blivit mer bekväma med Typescript. Vi har också kommit igång med tester och testrapporter. Johan har haft stora problem med Docker och köpt tre nya datorer, så av nödvändighet har han gjort färre timmar den här iteration medan Molly har gjort fler. Detta planeras att jämna ut sig under kommande iterationer.</sub>

### Faktiskt arbetad tid under föregående iteration
[Toggl-rapport Iteration 2](reports/toggl_iteration_2.pdf)</sub>

### Totalt arbetad tid i projektet inför nuvarande iteration

|<sub>Iteration</sub>|<sub>Miranda</sub>|<sub>Johan</sub>|<sub>Jesper</sub>|<sub>Molly</sub>|<sub>Totalt</sub>|
|----|----|-----|------------|----------|----|
|<sub>0</sub>|<sub>10.5</sub>|<sub>10.5</sub>|<sub>11</sub>|<sub>14.5</sub>|<sub>46.5</sub>|
|<sub>1</sub>|<sub>22</sub>|<sub>16.5</sub>|<sub>19.5</sub>|<sub>25</sub>|<sub>83</sub>|
|<sub>2</sub>|<sub>20.5</sub>|<sub>13.5</sub>|<sub>21.5</sub>|<sub>31.5</sub>|<sub>87</sub>|
|<sub>Total tid</sub>|<sub>53</sub>|<sub>40.5</sub>|<sub>52</sub>|<sub>71</sub>|<sub>216.5</sub>|

## Denna iteration

### Tidsuppskattad sprint backlog för denna iteration
<sub>[Tasks](https://github.com/1dv611-futurum-project/futurum-project/issues?utf8=%E2%9C%93&q=is%3Aissue+label%3A%22Iteration+3%22+) som planerats för denna iteration finns som issues.</sub>

<sub>Tid anges här som total tid spenderad av alla gruppmedlemmar - ett möte på en timme som alla deltagit på uppskattas alltså ta fyra timmar. Tidsuppskattningen fortsätter på förra veckans spår efter att ha bekräftat med handledaren att vara av det mer generella slaget, eftersom den specifika tidsuppskattningen tar alldeles för lång tid i anspråk i ett grupprojekt där vi inte vet exakt vem som kommer att utföra vilka uppgifter eller hur vi kommer att bryta ner de uppgifter som behöver utföras.</sub>
 
|<sub>Område</sub>|<sub>Requirement ID</sub>|<sub>Vi vill...</sub>|<sub>Så att...</sub>|<sub>Noteringar</sub>|<sub>Appr. Tid(h)</sub>|<sub>Ansvarig(h)</sub>|
|----|-----|------------|----------|-----|-----|-----|
|<sub>Möte</sub>|<sub>-</sub>|<sub>Handledarmöte</sub>|<sub>Vi bekräftar att vi är på rätt spår</sub>|<sub>-</sub>|<sub>4</sub>|<sub>Alla</sub>| 
|<sub>Möte</sub>|<sub>Alla</sub>|<sub>Gruppmöten</sub>|<sub>Vi kommer överens om hur vi ska jobba tillsammans</sub>|<sub>-</sub>|<sub>8</sub>|<sub>Alla</sub>| 
|<sub>Applikation</sub>|<sub>13-20</sub>|<sub>Få färdigt skelett-designen av React-sidorna</sub>|<sub>Vi kan visa upp en prototyp av systemet</sub>|<sub>-</sub>|<sub>10</sub>|<sub>Miranda + Jesper</sub>| 
|<sub>Applikation</sub>|<sub>13-20</sub>|<sub>Få upp en websocket-kontakt mellan klient och server</sub>|<sub>Klienten och servern kan kommunicera med varandra</sub>|<sub>-</sub>|<sub>32</sub>|<sub>Miranda + Jesper + Johan</sub>| 
|<sub>Applikation</sub>|<sub>16, 17, 20</sub>|<sub>Få igång serverns och databasens kommunikation</sub>|<sub>Vi kan spara undan mailärenden</sub>|<sub>-</sub>|<sub>12</sub>|<sub>Molly + Johan</sub>| 
|<sub>Applikation</sub>|<sub>8</sub>|<sub>Få upp en OAuth-autentisering för att autentisera användaren</sub>|<sub>Systemet bara är öppet för registrerade användare</sub>|<sub>-</sub>|<sub>8</sub>|<sub>Molly</sub>| </sub>|<sub>Vi kan lämna in Inception-dokumentationen</sub>|<sub>-</sub>|<sub>8</sub>|
|<sub>Dokumentation</sub>|<sub>6</sub>|<sub>Håll dokumentation uppdaterad</sub>|<sub>Vi följer utvecklingsprocessen</sub>|<sub>-</sub>|<sub>5</sub>|<sub>Alla</sub>| 
|<sub>Dokumentation</sub>|<sub>6</sub>|<sub>Skriv iterationsplan för iteration 3</sub>|<sub>Vi följer utvecklingsprocessen</sub>|<sub>-</sub>|<sub>1.5</sub>|<sub>Molly</sub>| 
|<sub>Dokumentation</sub>|<sub>6</sub>|<sub>Förbered 10 minuters presentation av Inception-fasen</sub>|<sub>Vi följer utvecklingsprocessen</sub>|<sub>-</sub>|<sub>2</sub>|<sub>Johan + Jesper</sub>|
|<sub>Dokumentation</sub>|<sub>6</sub>|<sub>Gå igenom annan grupps Inception-material och skriv rapport.</sub>|<sub>Vi följer utvecklingsprocessen.</sub>|<sub>-</sub>|<sub>4</sub>|<sub>Miranda + Molly</sub>|
| | | | |<sub>Total tid i iterationen:</sub>| 82.5| |

### Mål med iterationen
<sub>Målet med iterationen är att utforska de sista tekniska riskerna i form av databasen och Websocketen. Förhoppningen är att vi efter iterationen ska ha en färdig prototyp av systemet att produktionspaketera i Docker och delleverera till kunden. Resterande veckor under Elaboration kan då ägnas åt att lägga till saknade funktioner kring den teknik vi redan har, medan det tidigt satta målet att ha undanröjt de tekniska riskerna ger oss gott om tid att lösa eventuella problem som kan (kommer?) uppstå. Vi vill fortsätta med testning samt få upp vår OAuth-autentiering mot användaren så att kunden tydligt kan se att systemet kommer att vara säkert.</sub>

#### Risker som ska hanteras 
<sub>R2. Dåligt kundengagemang.  
R3. Tidsbrist.  
R5. Dålig gruppkommunikation.      
R8. Databasproblem.    
R9. Websocket.  </sub>   

#### Uppgifter för att hantera riskerna
* <sub>Ha flera gruppmöten där vi diskuterar vårt samarbete och hur vi fördelar uppgifterna.</sub>
* <sub>Få färdigt skelettet till en fungerande klientapplikation.</sub>
* <sub>Få upp en integration mellan klienten och servern genom en Websocket.</sub>
* <sub>Få upp en integration med databasen.</sub>
* <sub>Det tidigt satta målet att ha undanröjt de tekniska riskerna ger oss gott om tid att lösa eventuella problem som kan (kommer?) uppstå, vilket hjälper mot tidsbristen.</sub>
* <sub>Att sikta mot tidig delleverans mot kund är också bra för kundengagemanget.</sub>