# Futurum

<sub>**Sannolikhet** * **Konsekvens** = **Prioritet**</sub>

<sub>Sannolikhet och konsekvens för riskerna värderas mellan 1 och 5, där 1 är lågt och 5 är högt. Prioriteten hos en risk räknas fram genom att gångra sannolikheten med konsekvensen. Den risk med högst värde på prioritet prioriteras högst.</sub>

|<sub>ID</sub>|<sub>Namn</sub>|<sub>Beskrivning</sub>|<sub>Status</sub>|<sub>Prio</sub>|<sub>[Krav](https://github.com/1dv611-futurum-project/dokumentation/blob/master/inlämningar/inception/Kravspecifikation.md)</sub>|
|----|-----------|-----------|-----------|--|--:|
|<sub>R1</sub>|<sub>Bristande kundengagemang</sub>|<sub>Kunden engagerar sig inte i projektet i form av feedback eller är svår att få tag i.</sub>|<sub>Hanteras löpande</sub>|<sub>6</sub>|<sub>Alla</sub>|
|<sub>R2</sub>|<sub>Tidsbrist</sub>|<sub>De timmar som tilldelats projektgruppen räcker inte till för att färdigställa produkten.</sub>|<sub>Hanteras löpande</sub>|<sub>4</sub>|<sub>Alla</sub>|
|<sub>R3</sub>|<sub>Sjukdom/närvarobrist</sub>|<sub>Minskad närvaro hos en eller flera medlemmar i gruppen, pga sjukdom, jobb, fritidsaktiviteter eller dylikt.</sub>|<sub>Hanteras löpande</sub>|<sub>9</sub>|<sub>Alla</sub>|
|<sub>R4</sub>|<sub>Dålig grupp-kommunikation</sub>|<sub>Kommunikationen inom gruppen är bristande eller otydlig och orsakar missförstånd.</sub>|<sub>Hanteras löpande</sub>|<sub>12</sub>|<sub>Alla</sub>|
|<sub>R5</sub>|<sub>Docker</sub>|<sub>Problem med Docker som utvecklingsplattform.</sub>|<sub>Hanterad</sub>|<sub>20</sub>|<sub>Alla</sub>|
|<sub>R6</sub>|<sub>IMAP</sub>|<sub>IMAP-modulen är svår att integrera mot.</sub>|<sub>Hanterad</sub>|<sub>20</sub>|<sub>13-14, 16, 18-21</sub>|
|<sub>R7</sub>|<sub>Databasproblem</sub>|<sub>Integrationen mot databasen via Docker blir problematisk eller fungerar inte.</sub>|<sub>Hanterad</sub>|<sub>10</sub>|<sub>13, 15, 17</sub>|
|<sub>R8</sub>|<sub>Websocket</sub>|<sub>Kommunikationen mellan klient och server via Websocket är problematisk eller svår att få fungerande.</sub>|<sub>Hanteras innan slutet av Elaboration-fasen</sub>|<sub>15</sub>|<sub>13-19</sub>|



***

## R1. Bristande kundengagemang
<sub>**Sannolikhet**: 2</sub> | <sub>**Konsekvens**: 3</sub> | <sub>**Prioritet**: 6</sub>

<sub>**Beskrivning**: Kunden engagerar sig inte i projektet i form av feedback eller är svår att få tag i.
<br/>**Bevakningsstrategi**: Kundansvarig ansvarar i första hand för kontakt med kunden. Märker denne av att kund verkar oengagerad/svår att få tag i, informeras resten av gruppen snarast.
<br/>**Konsekvensstrategi**: Försöka hålla regelbundna avstämningar med kund och på dessa ta upp allt oklart som uppkommit/vilken feedback som önskas. Samla så mycket som möjligt på en gång när man ändå har kunden på tråden.
<br/>**Sannolikhetsstrategi**: Stämma av med kund vilken typ av kontakt som föredras och ställa mer specifika frågor kring feedback för att öka engagemanget. Boka in kundmöten/avstämningar i god tid.</sub>

## R2. Tidsbrist
<sub>**Sannolikhet**: 2</sub> | <sub>**Konsekvens**: 2</sub> | <sub>**Prioritet**: 4</sub>

<sub>**Beskrivning**: De timmar som tilldelats projektgruppen räcker inte till för att färdigställa produkten.
<br/>**Bevakningsstrategi**: Alla i gruppen ansvarar för att i god tid vara med och försöka avgöra ifall tiden blir för knapp. Projektledaren har ett extra ansvar att hålla koll på de återstående timmarna för projektet genom sammanställning av tidsrapporter.
<br/>**Konsekvensstrategi**: Det är svårt att minska konsekvensen av risken, då projektet behöver färdigställas i så stor mån som möjligt innan slutleverans mot kund. Fokus bör dock i första hand ligga på att få ordning på grundfunktionaliteten som efterfrågats av kund för att göra denna leveransklar. Först efter det kan "onödig tid" läggas på extra funktionalitet och förfiningar.
<br/>**Sannolikhetsstrategi**: I god tid ta oss an de större uppgifter som vi tror kan vara tidskrävande och därmed minimera sannolikheten.</sub>

## R3. Sjukdom/närvarobrist
<sub>**Sannolikhet**: 3</sub> | <sub>**Konsekvens**: 3</sub> | <sub>**Prioritet**: 9</sub>

<sub>**Beskrivning**: Minskad närvaro hos en eller flera medlemmar i gruppen, pga sjukdom, jobb, fritidsaktiviteter eller dylikt.
<br/>**Bevakningsstrategi**: Ansvaret ligger hos hela gruppen att i god tid meddela eventuella aktiviteter, och så tidigt som möjligt gällande sjukdom.
<br/>**Konsekvensstrategi**: Ej tilldela för stora/isolerade ansvarsområden. Se till att alltid minst 1 till gruppmedlem har koll på/är insatt i ens eget arbete; vad som är gjort/ska göras/ej fungerat.
<br/>**Sannolikhetsstrategi**: Det är svårt att minska sannolikheten för risken då man omöjligt kan påverka sjukdomar och har svårt att påverka övriga åtaganden. Däremot är det varje enskild gruppmedlems ansvar att planera sin egen tid tillräckligt för att hinna arbeta den tid som ska läggas på projektet varje vecka.</sub>

## R4. Dålig gruppkommunikation
<sub>**Sannolikhet**: 3</sub> | <sub>**Konsekvens**: 4</sub> | <sub>**Prioritet**: 12</sub>

<sub>**Beskrivning**: Kommunikationen inom gruppen är bristande eller otydlig och orsakar missförstånd.
<br/>**Bevakningsstrategi**: Hela gruppen ansvarar för att försöka kommunicera regelbundet med varandra och vid oklarheter tidigt ställa frågor eller reda ut problem.
<br/>**Konsekvensstrategi**: Tydligt gå igenom det som ska göras/vem som ansvarar för vad och försäkra sig om att alla förstår och delar samma vision.
<br/>**Sannolikhetsstrategi**: Generellt vara noga med att dokumentera det som sagts på möten, beslut kring tekniker, och andra saker som bestämts internt.</sub>

## R5. Docker
<sub>**Sannolikhet**: 5</sub> | <sub>**Konsekvens**: 4</sub> | <sub>**Prioritet**: 20</sub>

<sub>**Beskrivning**: Docker är svårt/omöjligt att sätta upp som utvecklingsmiljö och få fungerande i alla operativsystem.
<br/>**Bevakningsstrategi**: De i gruppen som ansvarar för uppsättningen av Docker bevakar risken genom att kontinuerligt uppskatta svårighetsgraden under utvecklingens gång.
<br/>**Konsekvensstrategi**: Se till att eventuellt lägga fram ett andra alternativ eller en plan B kring utvecklingsmiljö ifall Docker inte går att få upp ordentligt.
<br/>**Sannolikhetsstrategi**: Med hjälp av tidig efterforskning kring vad som krävs för att sätta upp projektet i Docker och att ta sig an problemet i ett tidigt stadie av utvecklingen. Utförlig testning av Docker-miljön i alla operativsystem krävs också för att säkerhetställa att det är välfungerande.</sub>

## R6. IMAP
<sub>**Sannolikhet**: 4</sub> | <sub>**Konsekvens**: 5</sub> | <sub>**Prioritet**: 20</sub>

<sub>**Beskrivning**: IMAP-modulen som är nödvändig för att integrera mot kundens inkorg och hantera mail är svårhanterligt eller problematiskt.
<br/>**Bevakningsstrategi**: Alla i gruppen ansvarar för att basfunktionalitet implementeras i tid och är fungerande, de i gruppen som jobbar främst med servern har ett extra ansvar. Risken bevakas kontinuerligt under utvecklingens och integrationens gång.
<br/>**Konsekvensstrategi**: Tyvärr är det svårt att minska konsekvensen då hela applikationen förlitar sig på att kunna integrera mot kundens inkorg. Fungerar inte detta blir hela applikationen fallande. Så tidigt som möjligt bör en integrering påbörjas för att eventuellt hinna med att (om behovet finns) istället göra en skräddarsydd lösning.
<br/>**Sannolikhetsstrategi**: Genom att låta alla i gruppen engagera sig och försöka förstå hur integrationen mot IMAP fungerar ökar sannolikheten att eventuella problem som stöts på inte känns främmande utan istället blir hanterbara. Integrationen bör inte heller ligga på endast en specifik person.</sub>

## R7. Databasproblem
<sub>**Sannolikhet**: 2</sub> | <sub>**Konsekvens**: 5</sub> | <sub>**Prioritet**: 10</sub>

<sub>**Beskrivning**: Integrationen mot databasen via Docker blir problematisk eller fungerar inte.
<br/>**Bevakningsstrategi**: Alla i gruppen ansvarar för att bevaka risken kontinuerligt under utvecklingens tidiga stadier, de som främst arbetar med servern har ett extra ansvar. Vi sätter upp produktionsmiljön med Docker även som utvecklingsmiljö och testar tidigt.
<br/>**Konsekvensstrategi**: I nuläget är databasen uppsatt som en egen container i Docker. För att minska konsekvensen av eventuella integrationsproblem skulle vi istället kunna lägga databasen i samma container som servern.
<br/>**Sannolikhetsstrategi**: Se till att utvecklings- och produktionsmiljö via Docker är detsamma för att minimerar sannolikheten att stöta på eventuella problem vid produktionssättning. Kontinuerligt genomföra tester mot databasen och även testköra en produktionssättning tidigt.</sub>

## R8. Websocket
<sub>**Sannolikhet**: 3</sub> | <sub>**Konsekvens**: 5</sub> | <sub>**Prioritet**: 15</sub>

<sub>**Beskrivning**: Kommunikationen mellan klient och server via Websocket är problematisk eller svår att få fungerande.
<br/>**Bevakningsstrategi**: Alla i gruppen ansvarar för att i god tid sätta upp kommunikationen via Websocket både hos klient och server, vilket bör göras innan Elaboration-fasen är slut.
<br/>**Konsekvensstrategi**: Titta på olika alternativa Websocket-lösningar i god tid och därigenom ha en reservplan ifall förstahandsalternativet skulle misslyckas.
<br/>**Sannolikhetsstrategi**: Ta tag i problemet redan i en tidig utvecklingsfas och därigenom ge oss själva tid att prova olika lösningar. Alla bör vara involverade i processen, men erfarenhet inom gruppen sedan tidigare av Websockets hos olika gruppmedlemmar bör inte förbises.</sub>
