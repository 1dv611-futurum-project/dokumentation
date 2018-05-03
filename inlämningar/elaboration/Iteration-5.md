# Iteration 5

## Föregående iteration

### Sammanfattning av föregående iteration
<sub>Vi har slutfört det grundläggande arbetet med de sista tekniska riskerna kring Websocket och IMAP. Vi har gjort en första leverans till kunden under veckan och fått bra feedback om att vi är på rätt väg. Vi lyckades till slut få upp en Websocket som fungerar bra mellan servern och klienten. Vi har också fortsatt med att få klart tester för de redan implementerade delarna av systemet, samt med förbättring av koden som redan finns på plats. Vi har enats om en databasdesign och har börjat jobba med modeller för den, och fått upp en grundläggande funktionalitet för att skicka, svara på och vidarebefordra mail från servern. Vi har också deltagit i en presentation av Inception-fasen samt granskat en annan grupp. </sub>

### Faktiskt arbetad tid under föregående iteration
<sub>[Toggl-rapport Iteration 4](reports/toggl_iteration_4.pdf)</sub>

### Totalt arbetad tid i projektet inför nuvarande iteration

|<sub>Iteration</sub>|<sub>Miranda</sub>|<sub>Johan</sub>|<sub>Jesper</sub>|<sub>Molly</sub>|<sub>Totalt</sub>|
|----|----|-----|------------|----------|----|
|<sub>0</sub>|<sub>10.5</sub>|<sub>10.5</sub>|<sub>11</sub>|<sub>14.5</sub>|<sub>46.5</sub>|
|<sub>1</sub>|<sub>22</sub>|<sub>16.5</sub>|<sub>19.5</sub>|<sub>25</sub>|<sub>83</sub>|
|<sub>2</sub>|<sub>20.5</sub>|<sub>13.5</sub>|<sub>21.5</sub>|<sub>31.5</sub>|<sub>87</sub>|
|<sub>3</sub>|<sub>19</sub>|<sub>17</sub>|<sub>19.5</sub>|<sub>20.5</sub>|<sub>76</sub>|
|<sub>4</sub>|<sub>20</sub>|<sub>22.5</sub>|<sub>20</sub>|<sub>20</sub>|<sub>82.5</sub>|
|<sub>Total tid</sub>|<sub>92</sub>|<sub>80</sub>|<sub>92.5</sub>|<sub>111.5</sub>|<sub>376</sub>|

## Denna iteration

### Tidsuppskattad sprint backlog för denna iteration
<sub>[Tasks](https://github.com/1dv611-futurum-project/futurum-project/issues?utf8=%E2%9C%93&q=is%3Aissue+label%3A%22Iteration+5%22+) som planerats för denna iteration finns som issues.</sub>

<sub>Tid anges här som total tid spenderad av alla gruppmedlemmar - ett möte på en timme som alla deltagit på uppskattas alltså ta fyra timmar. Tidsuppskattningen fortsätter på förra veckans spår efter att ha bekräftat med handledaren att vara av det mer generella slaget, eftersom den specifika tidsuppskattningen tar alldeles för lång tid i anspråk i ett grupprojekt där vi inte vet exakt vem som kommer att utföra vilka uppgifter eller hur vi kommer att bryta ner de uppgifter som behöver utföras.</sub>
 
|<sub>Område</sub>|<sub>Requirement ID</sub>|<sub>Vi vill...</sub>|<sub>Så att...</sub>|<sub>Noteringar</sub>|<sub>Appr. Tid(h)</sub>|<sub>Ansvarig</sub>|
|----|-----|------------|----------|-----|-----|-----|
|<sub>Möte</sub>|<sub>-</sub>|<sub>Handledarmöte</sub>|<sub>Vi bekräftar att vi är på rätt spår</sub>|<sub>-</sub>|<sub>4</sub>|<sub>Alla</sub>| 
|<sub>Möte</sub>|<sub>Alla</sub>|<sub>Gruppmöten</sub>|<sub>Vi kommer överens om hur vi ska jobba tillsammans</sub>|<sub>-</sub>|<sub>8</sub>|<sub>Alla</sub>| 
|<sub>Applikation</sub>|<sub>3, 16, 17, 18, 24</sub>|<sub>Göra databasmodeller</sub>|<sub>Vi kan spara undan mailärenden</sub>|<sub>-</sub>|<sub>3</sub>|<sub>Johan</sub>| 
|<sub>Applikation</sub>|<sub>3, 16, 17, 18, 24</sub>|<sub>Spara undan mail i databas när de kommer in på servern</sub>|<sub>Vi kan uppdatera status på dem.</sub>|<sub>-</sub>|<sub>4</sub>|<sub>Johan</sub>|
|<sub>Applikation</sub>|<sub>16</sub>|<sub>Uppdatera status på ärenden genom Websocket och spara undan i databasen</sub>|<sub>Vi kan kommunicera om statusen på ärenden till kund</sub>|<sub>-</sub>|<sub>3</sub>|<sub>Johan + Jesper</sub>|
|<sub>Applikation</sub>|<sub>24</sub>|<sub>Uppdatera tilldelning genom Websocket</sub>|<sub>Vi kan hålla reda på vem som har hand om ett ärende</sub>|<sub>-</sub>|<sub>3</sub>|<sub>Johan + Jesper</sub>|   
|<sub>Applikation</sub>|<sub>19, 20</sub>|<sub>Skicka mail till kund genom Websocket</sub>|<sub>Vi kan kommunicera med kund</sub>|<sub>-</sub>|<sub>3</sub>|<sub>Johan + Miranda</sub>|    
|<sub>Applikation</sub>|<sub>19, 20</sub>|<sub>Skicka mail till kund från server</sub>|<sub>Vi kan kommunicera med kund</sub>|<sub>-</sub>|<sub>5</sub>|<sub>Johan + Molly</sub>|    
|<sub>Applikation</sub>|<sub>17</sub>|<sub>Uppdatera klient när nytt mail kommer in i redan pågående konversation</sub>|<sub>Vi kan kommunicera med kund</sub>|<sub>-</sub>|<sub>10</sub>|<sub>Johan + Miranda  + Jesper</sub>|
|<sub>Applikation</sub>|<sub>14, 15, 17, 19-22</sub>|<sub>Felsök och felsäkra mailhanteringen</sub>|<sub>Vi kan kommunicera med kund</sub>|<sub>-</sub>|<sub>8</sub>|<sub>Molly</sub>|  
|<sub>Applikation</sub>|<sub>Alla</sub>|<sub>Tester</sub>|<sub>Tester skrivs för all kod som redan finns och all ny kod som skrivs.</sub>|<sub>-</sub>|<sub>12</sub>|<sub>Alla</sub>| 
|<sub>Dokumentation</sub>|<sub>6</sub>|<sub>Håll dokumentation uppdaterad</sub>|<sub>Vi följer utvecklingsprocessen</sub>|<sub>-</sub>|<sub>6</sub>|<sub>Alla</sub>| 
|<sub>Dokumentation</sub>|<sub>6</sub>|<sub>Skriv iterationsplan för iteration 6</sub>|<sub>Vi följer utvecklingsprocessen</sub>|<sub>-</sub>|<sub>1.5</sub>|<sub>Molly</sub>| 
|<sub>Dokumentation</sub>|<sub>6</sub>|<sub>Gå igenom dokumentation med [Elaborationgranskning](https://docs.google.com/document/d/1Y5wY5yaChtQz4VvmQoJ72TRmtN3wXmoDDyGGFxvdRys/edit) i bakhuvudet</sub>|<sub>Vi följer utvecklingsprocessen</sub>|<sub>-</sub>|<sub>6</sub>|<sub>Alla</sub>|
|<sub>Dokumentation</sub>|<sub>6</sub>|<sub>Färdigställ teknisk dokumentation.</sub>|<sub>Vi följer utvecklingsprocessen.</sub>|<sub>-</sub>|<sub>3</sub>|<sub>Johan</sub>|
| | | | |<sub>Total tid i iterationen:</sub>| 80.5| |

### Mål med iterationen
<sub>Målet med iterationen är att bli färdig med Elaboration-milstenen. Förutom att vår tekniska dokumentation ska vara klar, våra tekniska risker undanröjda och vår dokumentation inskickad till referentgruppen, så innebär det här för vår egen del att vi vill ha satt upp en databas där mail sparas undan när de kommer in från mail-servern, att ärenden ska kunna filtreras baserat på status på klienten, och att klienten och servern kan kommunicera genom Websocketen om statusändringar och att mail ska skickas till kund. Mail ska också faktiskt skickas ut till kunden. (se Milsten 4 [här](https://github.com/1dv611-futurum-project/futurum-project/wiki/Milstenar))</sub>

#### Risker som ska hanteras 
* <sub>R2. Tidsbrist.</sub>   
* <sub>R7. Databasproblem.</sub>       
* <sub>R8. Websocket.</sub>

#### Uppgifter för att hantera riskerna
* <sub>Kommunicera mellan klienten och servern genom en Websocket.</sub>
* <sub>Målet att ha undanröjt de tekniska riskerna ger oss gott om tid att lösa eventuella problem som kan (kommer?) uppstå, vilket hjälper mot tidsbristen.</sub>
* <sub>Databasen ska färdigställas och därmed identifieras eventuella databasproblem med många veckor kvar av projektet.</sub>