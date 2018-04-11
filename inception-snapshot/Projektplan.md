# Futurum

## Kund med kontaktuppgifter
<sub>Uppdragsgivare är *Futurum Digital*<br>
*Kontaktperson:* Anton K. Myrberg, anton@futurum.digital</sub>

## Uppdragstagare med kontaktuppgifter
<sub>Uppdragstagare är: </sub>
* <sub>Johan Söderlund js223zs@student.lnu.se</sub>
* <sub>Miranda Hammarstedt mirandahammarstedt@gmail.com</sub>
* <sub>Jesper Landmér Pedersen jp222vq@student.lnu.se</sub>
* <sub>Molly Arhammar mopooy@gmail.com</sub>

## Bakgrund till projektets uppkomst
<sub>Futurum Digital sköter idag sin kundkontakt genom flera olika kanaler, och det är svårt att hålla koll på status av varje enskilt projekt på ett överskådligt sätt. Futurum önskar sig en lösnig för att samla kundkommunikation och arbetsuppgifter på en plats.</sub>

## Syfte med projektet
<sub>Syftet med projektet är att samla Futurums kundkommunikation till en plats, och därmed förenkla strukturen för att hålla reda på vilket ärende som hanteras av vem, och var i processen varje ärende befinner sig. Detta skulle förenkla Futurums arbete då mindre tid skulle behöva läggas på administrativa uppgifter.</sub>

## Mål med projektet
<sub>Målet med applikationen är att </sub>
* <sub>Ha en nodejs-server som:</sub>
   * <sub>Reagerar på mail som skickas till en specifik Futurum-adress</sub>
   * <sub>Sparar dessa i en databas</sub>
   * <sub>Kommunicerar, via en websocket, med en React-app</sub>
* <sub>Ha en React-klient som</sub>
   * <sub>Visar Futurum inkomna ärenden så snart de kommer in</sub>
* <sub>Ett mail ska skickas tillbaka ut till kunden när statusen på något av de inkomna ärendena ändras.</sub>

## Begränsningar av projektet
<sub>Tekniker som ska användas:</sub>
* <sub>NodeJS</sub>
* <sub>React</sub>
* <sub>Websockets</sub>
* <sub>MongoDB</sub>

<sub>Den färdiga applikationen ska kunna deployas på kontorets Ubuntu 17.10 OS.</sub>

<sub>Övriga begränsningar är den tid som finns tillgänglig under resursplan, samt att baskrav ska uppfyllas.</sub>

## Resursplan
<sub>Projektets tidsresurs är **180** arbetstimmar per projektdeltagare, till en summa av totalt **720** timmar.
Timmarna ska spenderas som **20** timmar per vecka, per person, under projektets gång. </sub>

## Tidsplan för projektet
<sub>Projektet genomförs som en Scrum/OpenUP-process, i fyra cykler: *Inception*, *Elaboration*, *Construction* och *Transition*.</sub>

|<sub>Vecka</sub>|<sub>Milestones</sub> |<sub>Deliverables</sub> |
|----|-----------|--------------:|
| <sub>13</sub> |<sub>[MILESTONE 1. Project Approval - Inception (Design Approval, Requirements Review, Project Setup)](https://github.com/1dv611-futurum-project/futurum-project/wiki/Milestones)</sub>|<br> <sub>Tidrapporter</sub>|
| <sub>14</sub> | <sub>**(End Inception)** <br> [MILESTONE 2. Project Approval - Inception (Big technical hurdles gone)](https://github.com/1dv611-futurum-project/futurum-project/wiki/Milestones)</sub>| <sub>Vision Document, signerat av kund <br> Risklista <br> Kravspecifikation <br> Tidrapporter</sub> |
| <sub>15</sub> | <sub>Förbered Inception-presentation <br> Referentgranska en annan grupps Inception-inlämning</sub>|<sub><br> Tidrapporter</sub>|
| <sub>16</sub> |<sub>[MILESTONE 3. Project Phase - Elaboration (Skeleton)](https://github.com/1dv611-futurum-project/futurum-project/wiki/Milestones)</sub><br><sub>Presentation av Inception</sub><br><sub>Skicka material till kursledning för Inception</sub>   |<sub>Vision Document, signerat av kund <br> Risklista <br> Kravspecifikation <br> Tidrapporter</sub>|
| <sub>17</sub> | <sub>**(End Elaboration)** <br> [MILESTONE 4. Project Phase - Elaboration (Expanded functionality))](https://github.com/1dv611-futurum-project/futurum-project/wiki/Milestones)</sub> |  <sub>Testspecifikation <br> Arkitekturdokument och teknisk specifikation <br> Tidrapporter</sub>            |
| <sub>18</sub> |  <sub>Presentation Elaboration<br>Skicka material till kursledningen för Elaboration</sub>     |<sub>Testspecifikation <br> Arkitekturdokument och teknisk specifikation <br> Tidrapporter</sub>|
| <sub>19</sub> |   |               |<sub><br> Tidrapporter</sub>|
| <sub>20</sub> | <sub>**(End Construction)** <br>[MILESTONE 5. Project Phase - Construction (Whitelist management)](https://github.com/1dv611-futurum-project/futurum-project/wiki/Milestones)</sub>          |<sub>Source code <br> Kravspecifikation <br> Testspecifikation <br> Testrapporter <br> Risklista <br> Tidrapporter <br> Projektplan <br> Visionsdokument <br> Arkitektur och teknisk specifikation <br> Slutrapport <br></sub>|
| <sub>21</sub> |           |<sub><br> Tidrapporter</sub>|
| <sub>22</sub> |<sub>[MILESTONE 6. Final Approval - Transition (Phase 1)](https://github.com/1dv611-futurum-project/futurum-project/wiki/Milestones)<br>Slutpresentation av projekt</sub>|<sub>Färdig programvara till kund<br> Tidrapporter</sub>|
| <sub>23</sub> | <sub>**(End Transition)** <br>[MILESTONE 7. Final Approval - Transition (Phase 2)](https://github.com/1dv611-futurum-project/futurum-project/wiki/Milestones)</sub> |<sub>Färdig programvara <br> Kravspecifikation <br> Testspecifikation <br> Testrapporter <br> Risklista <br> Tidrapporter <br> Projektplan <br> Visionsdokument <br> Arkitektur och teknisk specifikation <br> Slutrapport <br></sub>|

## Kommunikationsplan
### Mot kund
#### Tid
<sub>Kunden är tillgänglig för att svara på frågor samma dag som han kontaktats, om problemet är litet. Större möten bör tidsbokas några dagar i förväg. Inga regelbundna möten är bestämda, men det är en målbild att bekräfta systemets status med kunden någon gång i veckan.</sub>

#### Plats
<sub>Kunden är öppen för kommunikation över mail, telefon, Asana eller Google Hangouts.</sub>

#### Orsak
<sub>Små problem och funderingar i relation till specifika krav tas över Asana, där man kan kommentera på kravet i fråga. Större möten med hela gruppen för del-leveranser av systemet tas över Google Hangouts. </sub>

### Inom utvecklingsgruppen
<sub>Gruppen kommunicerar med Slack som diskussionsverktyg och Github Projects som planeringsverktyg. På måndagar har gruppen ett handledarmöte och utvärderar förra veckans arbete, och i slutet av varje vecka försöker gruppen ha ett samtal över Slack där man utvärderar status på projektet och planerar nästa veckas arbete.</sub>

## Projektorganisation
### Ansvarsfördelning
<sub>Projektet har en *projektledare*, en *testansvarig*, en *implementationsansvarig* och en *kund- och kravansvarig*. Det är ansvarigs uppgift att strukturera arbetet kring sitt eget ansvarsområde och se till att det är gjort i tid, och allas uppgift att bidra till slutförandet av de arbetsuppgifter som uppstår under varje område.</sub>

<sub>**Kund- och kravansvarig:** Jesper, Miranda. </sub>   
<sub>**Implementationsansvarig:** Johan.  </sub>  
<sub>**Testansvarig:** Miranda.  </sub>  
<sub>**Projektledare:** Molly. </sub>     

<sub>Dokumentationsansvaret är delat i gruppen, med varje områdesansvarig som huvudansvarstagande för dokumentationen som faller under det området, enligt följande:</sub>

<sub>**Kundansvarig:** Ansvar för kravspecifikationen. </sub> <br>
<sub>**Implementationsansvarig:** Ansvar för arkitektur + teknisk dokumentation.</sub>  
<sub>**Testansvarig:** Ansvarig för testspecifikation.</sub>  
<sub>**Projektledare:** Ansvarig för projektplan + vision. </sub> 
  
<sub>**Alla:** Ansvariga för risklista + testrapporter.</sub>  