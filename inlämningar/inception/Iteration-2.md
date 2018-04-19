# Iteration 2

## Föregående iteration

### Sammanfattning av föregående iteration
<sub>Vi har fått vår vision godkänd av kunden, samt designat en mockup för hur klientapplikationen ska se ut så att vi känner oss bekväma med att gå vidare. Vi har börjat titta på hur vi ska lösa de största tekniska riskerna. Vi har fått upp en gemensam utvecklingsmiljö med Docker, samt har satt upp en bare-bone boilerplate för både express-servern och React-klienten. Vi har ett system för hur vi delar upp uppgifter och använder branches för feature-utveckling. Detta betyder att vi har åstadkommit vad vi ville göra under iterationen och känner oss redo att gå vidare in i nästa iteration.</sub>

### Faktiskt arbetad tid under föregående iteration
<sub>[Toggle-rapport Iteration 1](reports/toggl_iteration_1.pdf)</sub>

### Totalt arbetad tid i projektet inför denna iteration

|<sub>Iteration</sub>|<sub>Miranda</sub>|<sub>Johan</sub>|<sub>Jesper</sub>|<sub>Molly</sub>|<sub>Totalt</sub>|
|----|----|-----|------------|----------|----|
|<sub>0</sub>|<sub>10.5</sub>|<sub>10.5</sub>|<sub>11</sub>|<sub>14.5</sub>|<sub>46.5</sub>|
|<sub>1</sub>|<sub>22</sub>|<sub>16.5</sub>|<sub>19.5</sub>|<sub>25</sub>|<sub>83</sub>|
|<sub>Total tid</sub>|<sub>32.5</sub>|<sub>27</sub>|<sub>30.5</sub>|<sub>39.5</sub>|<sub>129.5</sub>|

## Denna iteration

### Tidsuppskattad sprint backlog för denna iteration
<sub>[Tasks](https://github.com/1dv611-futurum-project/futurum-project/issues?utf8=%E2%9C%93&q=is%3Aissue+label%3A%22Iteration+2%22+) som planerats för denna iteration finns som issues.</sub>

<sub>Tid anges här som total tid spenderad av alla gruppmedlemmar - ett möte på en timme som alla deltagit på uppskattas alltså ta fyra timmar. Tiduppskattningen är mer generell än förra veckan eftersom den specifika tidsuppskattningen tar alldeles för lång tid i anspråk i ett gruppprojekt där vi inte vet exakt vem som kommer att utföra vilka uppgifter eller hur vi kommer att bryta ner de uppgifter som behöver utföras.</sub>
 
|<sub>Område</sub>|<sub>Requirement ID</sub>|<sub>Vi vill...</sub>|<sub>Så att...</sub>|<sub>Noteringar</sub>|<sub>Appr. Tid(h)</sub>|<sub>Ansvarig(h)</sub>|
|----|-----|------------|----------|-----|-----|-----|
|<sub>Möte</sub>|<sub>-</sub>|<sub>Handledarmöte</sub>|<sub>Vi bekräftar att vi är på rätt spår</sub>|<sub>-</sub>|<sub>4</sub>|<sub>Alla</sub>| 
|<sub>Möte</sub>|<sub>Alla</sub>|<sub>Gruppmöten</sub>|<sub>Vi kommer överens om hur vi ska jobba tillsammans</sub>|<sub>-</sub>|<sub>16</sub>|<sub>Alla</sub>| 
|<sub>Applikation</sub>|<sub>13, 19</sub>|<sub>Få upp React med React Router</sub>|<sub>Vi kan sköta navigering på klienten</sub>|<sub>-</sub>|<sub>10</sub>|<sub>Miranda + Jesper</sub>| 
|<sub>Applikation</sub>|<sub>13-20</sub>|<sub>Få upp ett skelett av React-sidorna</sub>|<sub>Vi kan visa upp en prototyp av systemet</sub>|<sub>-</sub>|<sub>15</sub>|<sub>Miranda + Jesper</sub>| 
|<sub>Applikation</sub>|<sub>16, 17, 20</sub>|<sub>Få igång serverns och databasens kommunikation</sub>|<sub>Vi kan spara undan mailärenden</sub>|<sub>-</sub>|<sub>12</sub>|<sub>Johan</sub>| 
|<sub>Applikation</sub>|<sub>13, 14, 18</sub>|<sub>Få igång Imap-integrationen</sub>|<sub>Vi kan spara undan mailärenden</sub>|<sub>-</sub>|<sub>12</sub>|<sub>Molly</sub>| 
|<sub>Dokumentation</sub>|<sub>6</sub>|<sub>Gå igenom dokumentation med avseende på detta dokument: [Referentgranskning](https://docs.google.com/document/d/17VSkMh0qtJXRLYmKUrHXy33qiVWww5ud1nT1suggTlk/edit)</sub>|<sub>Vi kan lämna in Inception-dokumentationen</sub>|<sub>-</sub>|<sub>10</sub>|<sub>Alla</sub>| 
|<sub>Dokumentation</sub>|<sub>6</sub>|<sub>Skriv iterationsplan för iteration 3</sub>|<sub>Vi följer utvecklingsprocessen</sub>|<sub>-</sub>|<sub>1.5</sub>|<sub>Molly</sub>| 
| | | | |<sub>Total tid i iterationen:</sub>| 80.5| |

### Mål med iterationen
<sub>Vi vill bli klara med Inceptionfasen genom att se till att vår dokumentation är uppdaterad och strukturen kring den fungerar bra. Vi vill vara säkra på hur vi arbetar med vår versionshantering och olika features, samt ha röjt undan de stora tekniska riskerna. Vi vill bli bekväma med Typescript.</sub>

#### Risker som ska hanteras 
<sub>R5. Dålig gruppkommunikation.   
R7. Problem med email-API:t. (risken har efter detta bytt namn till IMAP)<br> 
R8. Databasproblem.</sub>

#### Uppgifter för att hantera riskerna
* <sub>Ha flera gruppmöten där vi diskuterar vårt samarbete och hur vi fördelar uppgifterna.</sub>
* <sub>Få upp ett skelett till en fungerande klientapplikation.</sub>
* <sub>Få upp en integration mot email-servern.</sub>
* <sub>Få upp en integration med databasen.</sub>