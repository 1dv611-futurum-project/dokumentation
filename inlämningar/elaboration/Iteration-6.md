# Iteration 6

## Föregående iteration

### Sammanfattning av föregående iteration
<sub>Vi har lyckats med målet att bli färdiga med Elaboration-milstenen. Vår tekniska dokumentation är klar, våra tekniska risker är undanröjda i den mån att alla tekniska lösningar har testats och fungerar, och vår dokumentation inskickad till referentgrupp. Utöver detta har vi påbörjat implementationen av databasen med modeller och styrt upp Websocketkommunikationen mellan klient och server. Mailmodulen har också färdigställts så att mail också faktiskt kan skickas ut till kunden. Koden har städats upp både på servern och klienten, och tester har skrivits och exekverats för alla färdigställda delar av systemet. </sub>

### Faktiskt arbetad tid under föregående iteration  
<sub>[Toggl-rapport Iteration 5](reports/toggl_iteration_5.pdf)</sub>

### Totalt arbetad tid i projektet inför nuvarande iteration

|<sub>Iteration</sub>|<sub>Miranda</sub>|<sub>Johan</sub>|<sub>Jesper</sub>|<sub>Molly</sub>|<sub>Totalt</sub>|
|----|----|-----|------------|----------|----|
|<sub>0</sub>|<sub>10.5</sub>|<sub>10.5</sub>|<sub>11</sub>|<sub>14.5</sub>|<sub>46.5</sub>|
|<sub>1</sub>|<sub>22</sub>|<sub>16.5</sub>|<sub>19.5</sub>|<sub>25</sub>|<sub>83</sub>|
|<sub>2</sub>|<sub>20.5</sub>|<sub>13.5</sub>|<sub>21.5</sub>|<sub>31.5</sub>|<sub>87</sub>|
|<sub>3</sub>|<sub>19</sub>|<sub>17</sub>|<sub>19.5</sub>|<sub>20.5</sub>|<sub>76</sub>|
|<sub>4</sub>|<sub>20</sub>|<sub>22.5</sub>|<sub>20</sub>|<sub>20</sub>|<sub>82.5</sub>|
|<sub>5</sub>|<sub>20</sub>|<sub>18.5</sub>|<sub>21</sub>|<sub>27</sub>|<sub>86.5</sub>|
|<sub>Total tid</sub>|<sub>112</sub>|<sub>98.5</sub>|<sub>113.5</sub>|<sub>138.5</sub>|<sub>462.5</sub>|

## Denna iteration

### Resterande tid i projektet
<sub>Vi räknar med att vid iterationens början ha cirka 260 timmar kvar i projektet, att spendera över sex veckor. De sista tre veckorna ska spenderas på slutdokumentation, slutrapport, redovisningar och överlämningar av projektet till kund och eventuella problem som uppstår med detta, och där vill vi spara ungefär 20 timmar per gruppmedlem totalt, vilket ger oss 80 timmar över tre veckor att färdigställa projektet. Vi vill ha denna tid för att säkerställa att vi kan avrunda projektet på ett bra sätt. Det betyder i sin tur att vi har strax över 180 timmar kvar över de kommande tre veckorna, inkluderat denna Iteration 6, att färdigställa projektets funktionalitet. Det känns rimligt givet den plats vi är på i projektet - vi spenderar denna iteration med att slutföra integreringen av vår redan implementerade funktionalitet, nästa iteration med att lägga till de sista små extrafunktionerna som önskats av kund, och iterationen därpå med att felsöka, fixa buggar, göra code reviews och lösa problem. Den kvarvarande tiden ger oss mellan 60 och 70 timmar per iteration under dessa kommande iterationer, vilket också passar bra med de röda dagar som kommer att infalla. Projektet känns helt genomförbart under den tid som är kvar.</sub>

### Tidsuppskattad sprint backlog för denna iteration
<sub>[Tasks](https://github.com/1dv611-futurum-project/futurum-project/issues?utf8=%E2%9C%93&q=is%3Aissue+label%3A%22Iteration+6%22+) som planerats för denna iteration finns som issues.</sub>

<sub>Tid anges här som total tid spenderad av alla gruppmedlemmar - ett möte på en timme som alla deltagit på uppskattas alltså ta fyra timmar. Tidsuppskattningen fortsätter på förra veckans spår efter att ha bekräftat med handledaren att vara av det mer generella slaget, eftersom den specifika tidsuppskattningen tar alldeles för lång tid i anspråk i ett grupprojekt där vi inte vet exakt vem som kommer att utföra vilka uppgifter eller hur vi kommer att bryta ner de uppgifter som behöver utföras. Mollys totala timmar är lite lägre den här veckan för att kompensera för tidigare övertidsarbete, men timmar kommer att läggas till vid behov beroende på hur mycket arbete som behöver göras med mail-delen av applikationen under integrationsarbetet.</sub>

|<sub>Område</sub>|<sub>Requirement ID</sub>|<sub>Vi vill...</sub>|<sub>Så att...</sub>|<sub>Noteringar</sub>|<sub>Appr. Tid(h)</sub>|<sub>Ansvarig</sub>|
|----|-----|------------|----------|-----|-----|-----|
|<sub>Möte</sub>|<sub>-</sub>|<sub>Redovisning av elaboration</sub>|<sub>Vi följer utvecklingsprocessen</sub>|<sub>-</sub>|<sub>4</sub>|<sub>Alla</sub>|
|<sub>Möte</sub>|<sub>Alla</sub>|<sub>Gruppmöten</sub>|<sub>Vi kommer överens om hur vi ska jobba tillsammans</sub>|<sub>-</sub>|<sub>4</sub>|<sub>Alla</sub>|
|<sub>Möte</sub>|<sub>Alla</sub>|<sub>Kundmöte</sub>|<sub>Vi gör en delleverans av systemet.</sub>|<sub>-</sub>|<sub>4</sub>|<sub>Alla</sub>|
|<sub>Applikation</sub>|<sub>14, 16, 17, 18, 24</sub>|<sub>Färdigställa databas</sub>|<sub>Vi kan spara undan uppdateringar av information</sub>|<sub>-</sub>|<sub>7</sub>|<sub>Johan</sub>|
|<sub>Applikation</sub>|<sub>14, 16, 17, 18, 19, 20, 24</sub>|<sub>Databas - Websocketintegration på servern</sub>|<sub>Vi kan kommunicera mellan klient och databas och spara undan uppdateringar av information</sub>|<sub>-</sub>|<sub>1.5</sub>|<sub>Johan</sub>|
|<sub>Applikation</sub>|<sub>14, 16, 17, 18, 19, 20, 24</sub>|<sub>Mail - Websocketintegration på servern, socketdelen</sub>|<sub>Vi kan kommunicera med klienten över mail</sub>|<sub>-</sub>|<sub>1.5</sub>|<sub>Johan</sub>|  
|<sub>Applikation</sub>|<sub>14, 16, 17, 18, 19, 20, 24</sub>|<sub>Mail - Websocketintegration på servern, maildelen</sub>|<sub>Vi kan kommunicera med klienten över mail</sub>|<sub>Molly står i standby för eventuellt som behöver göras på mailsidan av den här integrationen - vi vet inte riktigt det förrän integrationen har börjat.</sub>|<sub>0-4</sub>|<sub>Molly</sub>|
|<sub>Applikation</sub>|<sub>15, 16, 17, 18, 19, 20, 24</sub>|<sub>Buggar på klienten - Websocketintegration och inloggningsrelaterade</sub>|<sub>Klientintegrationen med servern fungerar och inloggningsflödet fungerar</sub>|<sub></sub>|<sub>5</sub>|<sub>Johan</sub>|
|<sub>Applikation</sub>|<sub>14, 17, 19, 20, 23, 24</sub>|<sub>Buggar på klienten - ärendevisningsrelaterade</sub>|<sub>Klientintegrationen med servern fungerar och ärenden visas korrekt</sub>|<sub></sub>|<sub>5</sub>|<sub>Miranda</sub>|
|<sub>Applikation</sub>|<sub>Alla</sub>|<sub>Tester</sub>|<sub>Tester skrivs för all kod som redan finns och all ny kod som skrivs.</sub>|<sub>-</sub>|<sub>8</sub>|<sub>Alla</sub>|
|<sub>Dokumentation</sub>|<sub>6</sub>|<sub>Håll dokumentation uppdaterad</sub>|<sub>Vi följer utvecklingsprocessen</sub>|<sub>-</sub>|<sub>8</sub>|<sub>Alla</sub>|
|<sub>Dokumentation</sub>|<sub>6</sub>|<sub>Skriv iterationsplan för iteration 6</sub>|<sub>Vi följer utvecklingsprocessen</sub>|<sub>-</sub>|<sub>1.5</sub>|<sub>Molly</sub>|
|<sub>Dokumentation</sub>|<sub>6</sub>|<sub>Färdigställ presentation av Elaboration-fasen</sub>|<sub>Vi följer utvecklingsprocessen</sub>|<sub>-</sub>|<sub>6</sub>|<sub>Molly + Miranda</sub>|
|<sub>Dokumentation</sub>|<sub>6</sub>|<sub>Gå igenom referentgrupps dokumentation med [Elaborationgranskning](https://docs.google.com/document/d/1Y5wY5yaChtQz4VvmQoJ72TRmtN3wXmoDDyGGFxvdRys/edit) i bakhuvudet</sub>|<sub>Vi följer utvecklingsprocessen</sub>|<sub>-</sub>|<sub>6</sub>|<sub>Johan + Jesper</sub>|
| | | | |<sub>Total tid i iterationen:</sub>|70| |

### Mål med iterationen
<sub>Målet med kommande iteration är att färdigställa [Milsten 4](https://github.com/1dv611-futurum-project/futurum-project/wiki/Milstenar#milsten-4-project-phase---elaboration-ut%C3%B6kad-funktionalitet). Detta innebär att databasen ska färdigställas och integreras med Websocketen och mailmodulerna. I den bästa av världar går detta smidigt och får konsekvensen att mail sparas undan när de kommer in från mail-servern, ärenden kan filtreras baserat på status på klienten, och klienten och servern kan kommunicera genom Websocketen om statusändringar och att mail ska skickas till kund. Förmodligen kommer mindre problem uppstå i integrationen, men målet är att lösa dem under veckan. Alla tekniker och principer fungerar separat. Vi ska också ha ett kundmöte där funktionaliteten visas upp för kund.</sub>

#### Risker som ska hanteras  
* <sub> R1 - Bristande kundengagemang </sub>
* <sub> R2 - Tidsbrist </sub>
* <sub> R3 - Sjukdom/närvarobrist </sub>
* <sub> R6 - IMAP </sub>
* <sub> R7 - Databasproblem </sub>
* <sub> R8 - Websocket </sub>

#### Uppgifter för att hantera riskerna
* <sub> Kundengagemanget hanteras  som alltid genom ett kundmöte.</sub>
* <sub> Tidsbrist och närvarobrist hanteras genom att vi försöker färdigställa så mycket av funktionaliteten som möjligt nu över de sista tre aktiva veckorna.</sub>
* <sub> De resterande riskerna är egentligen så låga att de räknas som hanterade men kan ändå i någon mån sägas hanteras för sista gången i denna iteration. Genom att bygga ihop de tre sidorna av funktionaliteten bekräftar vi att riskerna är borta och färdighanterade.</sub>
