# Iteration 4

## Föregående iteration

### Sammanfattning av föregående iteration
<sub>Vi har börjat utforska de sista tekniska riskerna i form av databasen och Websocketen. Vi har ännu inte en helt färdig prototyp att visa för kunden, men vi har fått upp en integration med databasen och kommit igång med Websocketen. Vi hoppas på att slutföra arbetet med båda dessa saker nästa vecka. Vi har fortsatt med testning samt fått upp vår OAuth-autentiering mot användaren, samt har slutfört ett klient-skelett som väntar på att integreras med servern. Testningen har kommit igång med både manuella och automatiska tester, och vi har granskat en annan grupps Inception-inlämning och fått feedback på vår egen. Vi ligger i fas. </sub>

### Faktiskt arbetad tid under föregående iteration
<sub>[Toggl-rapport Iteration 3](reports/toggl_iteration_3.pdf)</sub>

### Totalt arbetad tid i projektet inför nuvarande iteration

|<sub>Iteration</sub>|<sub>Miranda</sub>|<sub>Johan</sub>|<sub>Jesper</sub>|<sub>Molly</sub>|<sub>Totalt</sub>|
|----|----|-----|------------|----------|----|
|<sub>0</sub>|<sub>10.5</sub>|<sub>10.5</sub>|<sub>11</sub>|<sub>14.5</sub>|<sub>46.5</sub>|
|<sub>1</sub>|<sub>22</sub>|<sub>16.5</sub>|<sub>19.5</sub>|<sub>25</sub>|<sub>83</sub>|
|<sub>2</sub>|<sub>20.5</sub>|<sub>13.5</sub>|<sub>21.5</sub>|<sub>31.5</sub>|<sub>87</sub>|
|<sub>3</sub>|<sub>19</sub>|<sub>17</sub>|<sub>19.5</sub>|<sub>20.5</sub>|<sub>76</sub>|
|<sub>Total tid</sub>|<sub>72</sub>|<sub>57.5</sub>|<sub>72.5</sub>|<sub>91.5</sub>|<sub>293.5</sub>|

## Denna iteration

### Tidsuppskattad sprint backlog för denna iteration
<sub>[Tasks](https://github.com/1dv611-futurum-project/futurum-project/issues?utf8=%E2%9C%93&q=is%3Aissue+label%3A%22Iteration+4%22+) som planerats för denna iteration finns som issues.</sub>

<sub>Tid anges här som total tid spenderad av alla gruppmedlemmar - ett möte på en timme som alla deltagit på uppskattas alltså ta fyra timmar. Tidsuppskattningen fortsätter på förra veckans spår efter att ha bekräftat med handledaren att vara av det mer generella slaget, eftersom den specifika tidsuppskattningen tar alldeles för lång tid i anspråk i ett grupprojekt där vi inte vet exakt vem som kommer att utföra vilka uppgifter eller hur vi kommer att bryta ner de uppgifter som behöver utföras.</sub>
 
|<sub>Område</sub>|<sub>Requirement ID</sub>|<sub>Vi vill...</sub>|<sub>Så att...</sub>|<sub>Noteringar</sub>|<sub>Appr. Tid(h)</sub>|<sub>Ansvarig</sub>|
|----|-----|------------|----------|-----|-----|-----|
|<sub>Möte</sub>|<sub>-</sub>|<sub>Handledarmöte</sub>|<sub>Vi bekräftar att vi är på rätt spår</sub>|<sub>-</sub>|<sub>4</sub>|<sub>Alla</sub>| 
|<sub>Möte</sub>|<sub>Alla</sub>|<sub>Gruppmöten</sub>|<sub>Vi kommer överens om hur vi ska jobba tillsammans</sub>|<sub>-</sub>|<sub>8</sub>|<sub>Alla</sub>| 
|<sub>Möte</sub>|<sub>Alla</sub>|<sub>Kundleverans</sub>|<sub>Vi bekräftar att vi är på rätt spår och får feedback.</sub>|<sub>-</sub>|<sub>4</sub>|<sub>Alla</sub>| 
|<sub>Applikation</sub>|<sub>13-20</sub>|<sub>Komponent för Websocket på klienten</sub>|<sub>Vi kan kommunicera mellan klient och server</sub>|<sub>-</sub>|<sub>15</sub>|<sub>Miranda + Jesper</sub>| 
|<sub>Applikation</sub>|<sub>13-20</sub>|<sub>Websocket-kontakt startad på servern</sub>|<sub>Klienten och servern kan kommunicera med varandra</sub>|<sub>-</sub>|<sub>15</sub>|<sub>Johan</sub>| 
|<sub>Applikation</sub>|<sub>13-20</sub>|<sub>Integrera Websocket på server och klient</sub>|<sub>Klienten och servern kan kommunicera med varandra</sub>|<sub>-</sub>|<sub>10</sub>|<sub>Miranda + Jesper + Johan</sub>| 
|<sub>Applikation</sub>|<sub>16, 17, 20</sub>|<sub>Göra databasmodeller</sub>|<sub>Vi kan spara undan mailärenden</sub>|<sub>-</sub>|<sub>3</sub>|<sub>Molly</sub>| 
|<sub>Applikation</sub>|<sub>Alla</sub>|<sub>Tester</sub>|<sub>Tester skrivs för all kod som redan finns och all ny kod som skrivs.</sub>|<sub>-</sub>|<sub>20</sub>|<sub>Alla</sub>| 
|<sub>Dokumentation</sub>|<sub>6</sub>|<sub>Håll dokumentation uppdaterad</sub>|<sub>Vi följer utvecklingsprocessen</sub>|<sub>-</sub>|<sub>6</sub>|<sub>Alla</sub>| 
|<sub>Dokumentation</sub>|<sub>6</sub>|<sub>Skriv iterationsplan för iteration 5</sub>|<sub>Vi följer utvecklingsprocessen</sub>|<sub>-</sub>|<sub>1.5</sub>|<sub>Molly</sub>| 
|<sub>Dokumentation</sub>|<sub>6</sub>|<sub>Håll 10 minuters presentation av Inception-fasen</sub>|<sub>Vi följer utvecklingsprocessen</sub>|<sub>-</sub>|<sub>0.5</sub>|<sub>Johan + Jesper</sub>|
|<sub>Dokumentation</sub>|<sub>6</sub>|<sub>Delta på annan grupps Inception-genomgång</sub>|<sub>Vi följer utvecklingsprocessen.</sub>|<sub>-</sub>|<sub>0.5</sub>|<sub>Miranda + Molly</sub>|
| | | | |<sub>Total tid i iterationen:</sub>| 87.5| |

### Mål med iterationen
<sub>Målet med iterationen är att slutföra det grundläggande arbetet med de sista tekniska riskerna kring Websocket och IMAP. Vi vill kunna göra en första leverans till kunden under veckan med all grundläggande funktionalitet på plats, och den sista stora del som behöver tas tag i då är att få upp en Websocket som fungerar bra mellan servern och klienten. Utöver detta vill vi fortsätta att få klart tester för de redan implementerade delarna av systemet, samt fortsätta med förbättring av koden som redan finns på plats. Baserat på vilken feedback vi får av kunden har vi sedan en vecka på oss att avrunda med de tekniska riskerna och få ihop vår basfunktionalitet stabilt med alla tester och refactoring av kod, innan Elaboration-inlämningen görs.</sub>

#### Risker som ska hanteras 
<sub>R2. Dåligt kundengagemang.  
R3. Tidsbrist.  
R5. Dålig gruppkommunikation.        
R9. Websocket.  </sub>   

#### Uppgifter för att hantera riskerna
* <sub>Ha flera gruppmöten där vi diskuterar vårt samarbete och hur vi fördelar uppgifterna.</sub>
* <sub>Få upp en integration mellan klienten och servern genom en Websocket.</sub>
* <sub>Det tidigt satta målet att ha undanröjt de tekniska riskerna ger oss gott om tid att lösa eventuella problem som kan (kommer?) uppstå, vilket hjälper mot tidsbristen.</sub>
* <sub>Tidig delleverans mot kund är bra för kundengagemanget.</sub>
* <sub>Tidig delleverans mot kund är också bra för tidig feedback, vilket motverkar tidsbrist senare i projektet.</sub>