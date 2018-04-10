### Syfte och målsättning
<sub>Syftet med testningen är att kunna säkerställa kvalitén kontinuerligt under utvecklingens gång på den applikation som i slutskedet ska levereras till kund. Det slutgiltiga målet är i sin tur att få bekräftat att det som levereras har en fungerande grundfunktionalitet. Prioritering kommer främst att ligga på att leverera de [funktionella krav](https://github.com/1dv611-futurum-project/futurum-project/wiki/Kravspecifikation#funktionella-krav-f%C3%B6lj-processen-h%C3%A4r) som har efterfrågats av kund.  Testningen kommer också delvis att rikta sig mot de [kvalitetskrav](https://github.com/1dv611-futurum-project/futurum-project/wiki/Kravspecifikation#kvalitetskrav-f%C3%B6lj-processen-h%C3%A4r) som finns. Det här gäller endast kvalitetskraven gällande säkerhet, användarvänlighet, webbstandarder och svarstid. Testprocessen ska med andra ord se till så att systemet lever upp till de förväntade kraven.</sub>

### Verktyg
<sub>För att genomföra olika tester kommer vi att använda oss av följande verktyg:</sub>
* <sub>**Postman**, för att testa mot olika api-routes på servern. Förutsättningen för att det här ska fungera är att man har Postman installerat lokalt och även importerat den Postman Collection som följer med systemet.</sub>
* <sub>**Mocha, Chai och Karma**, för att kunna testa specifika funktioner eller block av kod. För att kunna köra testerna behöver man gå in i en specific Docker container och där i köra `npm run test`.</sub>

### Strategi
<sub>Automatiska tester kommer att användas för att testa de funktionella kraven som beskrivs i kravspecifikationen. Dessa tester kan ses som unit tests och kan testa både mindre, isolerade funktioner eller hela klasser. De automatiserade testerna bör köras varje gång server- eller klientapplikationen startas.</sub>

<sub>Manuella tester genomförs löpande under arbetets gång inom gruppen. Varje gång ny funktionalitet läggs till testas denna först manuellt kontinuerligt under utvecklingens gång innan den anses vara helt färdigställd. Flertalet manuella tester kommer även att behöva genomföras för att kunna simulera att mail inkommer till applikationen.</sub>

<sub>Även user interface tester genomförs löpande under utveckling av klienten för att säkerställa att användargränssnittet är tydligt och användarvänligt i enlighet med de kvalitetskrav som har satts upp.</sub>

<sub>Ett begränsat antal explorativa användartester kommer att genomföras av kund för att få feedback av de tilltänkta slutanvändarna av systemet. Dessa användartester kommer endast att genomföras vid varje delleverans till kund, och genomförs i den mängd som kunden önskar och hinner med. Resultat från användartester bör prioriteras då de kommer direkt från slutanvändaren.</sub>


### Ansvarsfördelning
<sub>Det övergripande ansvaret som innebär att hålla testspecifikationen uppdaterad, samt se till att testfall skrivs och resultaten rapporteras ligger hos testansvarig (Miranda). Testerna kommer i många fall vara uppdelade mellan klient/server, och därmed ligger också ansvaret för dessa tester hos respektive utvecklingsgrupp. Ansvariga för att skriva och köra tester på servern är i första hand Molly och Johan. Ansvariga för att skriva och köra testfall på klienten är i första hand Miranda och Jesper. Eventuella användartester som kommer behöva göras ansvarar gruppen gemensamt för att genomföra och strukturera upp.</sub>

<sub>Eventuella buggar som upptäcks under testprocessen ska inte pushas upp på Github utan försöka åtgärdas lokalt. Går det inte att åtgärda utan att ta hjälp av annan gruppmedlem som behöver tillgång till samma kod, ska det i så fall skapas en separat branch för att hantera buggen. Branchen får inte mergas in i master förrän buggen är fullständigt åtgärdad. Skulle en bugg mot förmodan hittas i den kod som redan ligger på Github, rapporteras det här i första hand till den som har producerat koden, och i andra hand till nästa medlem som är ansvarig inom området (klient/server). </sub>

## Systemtester
### Systemtest 1: Säkerhet — Kvalitetskrav #8
|<sub>Område</sub>|<sub>ID</sub>|<sub>Testfall</sub>|<sub>Testform</sub>|
|----|--------|------------|---------|
|<sub>Server</sub>|<sub>T1</sub>|<sub>[Autentisera servern mot mailadressen som ska bevakas - lyckad autentiering](https://github.com/1dv611-futurum-project/futurum-project/wiki/Testspecifikation#testfall-1---autentisera-servern-mot-mailadressen-som-ska-bevakas---lyckad-autentisering)</sub>|<sub>Manuellt</sub>|
|<sub>Server</sub>|<sub>T2</sub>|<sub>[Autentisera servern mot mailadressen som ska bevakas - misslyckad autentiering](https://github.com/1dv611-futurum-project/futurum-project/wiki/Testspecifikation#testfall-2---autentisera-servern-mot-mailadressen-som-ska-bevakas---misslyckad-autentisering)</sub>|<sub>Manuellt</sub>|
|<sub>Server</sub>|<sub>T3</sub>|<sub>[Autentisera servern mot mailadressen som ska bevakas - nekad autentiering](https://github.com/1dv611-futurum-project/futurum-project/wiki/Testspecifikation#testfall-3---autentisera-servern-mot-mailadressen-som-ska-bevakas---nekad-autentisering)</sub>|<sub>Manuellt</sub>|

### Systemtest 2: Visning av ärenden — Funktionellt krav #13, #16
|<sub>Område</sub>|<sub>ID</sub>|<sub>Testfall</sub>|<sub>Testform</sub>|
|----|--------|------------|---------|
|<sub>Server</sub>|<sub>T1</sub>|<sub>[Autentisera servern mot mailadressen som ska bevakas - lyckad autentiering](https://github.com/1dv611-futurum-project/futurum-project/wiki/Testspecifikation#testfall-1---autentisera-servern-mot-mailadressen-som-ska-bevakas---lyckad-autentisering)</sub>|<sub>Manuellt</sub>|
|<sub>Server</sub>|<sub>T2</sub>|<sub>[Autentisera servern mot mailadressen som ska bevakas - misslyckad autentiering](https://github.com/1dv611-futurum-project/futurum-project/wiki/Testspecifikation#testfall-2---autentisera-servern-mot-mailadressen-som-ska-bevakas---misslyckad-autentisering)</sub>|<sub>Manuellt</sub>|
|<sub>Server</sub>|<sub>T3</sub>|<sub>[Autentisera servern mot mailadressen som ska bevakas - nekad autentiering](https://github.com/1dv611-futurum-project/futurum-project/wiki/Testspecifikation#testfall-3---autentisera-servern-mot-mailadressen-som-ska-bevakas---nekad-autentisering)</sub>|<sub>Manuellt</sub>|

### Systemtest 3: Ärendehantering — Funktionellt krav #15, #18, #19
|<sub>Område</sub>|<sub>ID</sub>|<sub>Testfall</sub>|<sub>Testform</sub>|
|----|--------|------------|---------|
|<sub>Server</sub>|<sub>T1</sub>|<sub>[Autentisera servern mot mailadressen som ska bevakas - lyckad autentiering](https://github.com/1dv611-futurum-project/futurum-project/wiki/Testspecifikation#testfall-1---autentisera-servern-mot-mailadressen-som-ska-bevakas---lyckad-autentisering)</sub>|<sub>Manuellt</sub>|
|<sub>Server</sub>|<sub>T2</sub>|<sub>[Autentisera servern mot mailadressen som ska bevakas - misslyckad autentiering](https://github.com/1dv611-futurum-project/futurum-project/wiki/Testspecifikation#testfall-2---autentisera-servern-mot-mailadressen-som-ska-bevakas---misslyckad-autentisering)</sub>|<sub>Manuellt</sub>|
|<sub>Server</sub>|<sub>T3</sub>|<sub>[Autentisera servern mot mailadressen som ska bevakas - nekad autentiering](https://github.com/1dv611-futurum-project/futurum-project/wiki/Testspecifikation#testfall-3---autentisera-servern-mot-mailadressen-som-ska-bevakas---nekad-autentisering)</sub>|<sub>Manuellt</sub>|
|<sub>Klient</sub>|<sub>T4</sub>|<sub>[Ändra status på ärende - flerkortsvy, uppdatering till kund](https://github.com/1dv611-futurum-project/futurum-project/wiki/Testspecifikation#testfall-4---%C3%84ndra-status-p%C3%A5-%C3%A4rende---flerkortsvy-uppdatering-till-kund)</sub>|<sub>Manuellt</sub>|
|<sub>Klient</sub>|<sub>T5</sub>|<sub>[Ändra status på ärende - enskild kortvy, utan uppdatering till kund](https://github.com/1dv611-futurum-project/futurum-project/wiki/Testspecifikation#testfall-5---%C3%84ndra-status-p%C3%A5-%C3%A4rende---enskild-kortvy-utan-uppdatering-till-kund)</sub>|<sub>Manuellt</sub>|

### Systemtest 4: Inkomna mail — Funktionellt krav #14, #20, #21
|<sub>Område</sub>|<sub>ID</sub>|<sub>Testfall</sub>|<sub>Testform</sub>|
|----|--------|------------|---------|
|<sub>Server</sub>|<sub>T1</sub>|<sub>[Autentisera servern mot mailadressen som ska bevakas - lyckad autentiering](https://github.com/1dv611-futurum-project/futurum-project/wiki/Testspecifikation#testfall-1---autentisera-servern-mot-mailadressen-som-ska-bevakas---lyckad-autentisering)</sub>|<sub>Manuellt</sub>|
|<sub>Server</sub>|<sub>T2</sub>|<sub>[Autentisera servern mot mailadressen som ska bevakas - misslyckad autentiering](https://github.com/1dv611-futurum-project/futurum-project/wiki/Testspecifikation#testfall-2---autentisera-servern-mot-mailadressen-som-ska-bevakas---misslyckad-autentisering)</sub>|<sub>Manuellt</sub>|
|<sub>Server</sub>|<sub>T3</sub>|<sub>[Autentisera servern mot mailadressen som ska bevakas - nekad autentiering](https://github.com/1dv611-futurum-project/futurum-project/wiki/Testspecifikation#testfall-3---autentisera-servern-mot-mailadressen-som-ska-bevakas---nekad-autentisering)</sub>|<sub>Manuellt</sub>|

### Systemtest 5: Registrerade mailadresser — Funktionellt krav #17
|<sub>Område</sub>|<sub>ID</sub>|<sub>Testfall</sub>|<sub>Testform</sub>|
|----|--------|------------|---------|
|<sub>Server</sub>|<sub>T1</sub>|<sub>[Autentisera servern mot mailadressen som ska bevakas - lyckad autentiering](https://github.com/1dv611-futurum-project/futurum-project/wiki/Testspecifikation#testfall-1---autentisera-servern-mot-mailadressen-som-ska-bevakas---lyckad-autentisering)</sub>|<sub>Manuellt</sub>|
|<sub>Server</sub>|<sub>T2</sub>|<sub>[Autentisera servern mot mailadressen som ska bevakas - misslyckad autentiering](https://github.com/1dv611-futurum-project/futurum-project/wiki/Testspecifikation#testfall-2---autentisera-servern-mot-mailadressen-som-ska-bevakas---misslyckad-autentisering)</sub>|<sub>Manuellt</sub>|
|<sub>Server</sub>|<sub>T3</sub>|<sub>[Autentisera servern mot mailadressen som ska bevakas - nekad autentiering](https://github.com/1dv611-futurum-project/futurum-project/wiki/Testspecifikation#testfall-3---autentisera-servern-mot-mailadressen-som-ska-bevakas---nekad-autentisering)</sub>|<sub>Manuellt</sub>|
|<sub>Klient</sub>|<sub>T1</sub>|<sub>[Lägga till ny mailadress](https://github.com/1dv611-futurum-project/futurum-project/wiki/Testspecifikation#testfall-1---l%C3%A4gga-till-ny-mailadress)</sub>|<sub>Manuellt</sub>|
|<sub>Klient</sub>|<sub>T2</sub>|<sub>[Lägga till ny mailadress - felaktig input](https://github.com/1dv611-futurum-project/futurum-project/wiki/Testspecifikation#testfall-2---l%C3%A4gga-till-ny-mailadress---felaktig-input)</sub>|<sub>Manuellt</sub>|
|<sub>Klient</sub>|<sub>T3</sub>|<sub>[Lägga till ny mailadress - redan registrerad mailadress](https://github.com/1dv611-futurum-project/futurum-project/wiki/Testspecifikation#testfall-3---l%C3%A4gga-till-ny-mailadress---redan-registrerad-mailadress)</sub>|<sub>Manuellt</sub>|


## Testfall - Server

### Manuella tester
#### Testfall 1 - Autentisera servern mot mailadressen som ska bevakas - lyckad autentisering
<sub>**Krav som testas**: #8, #13-#21</sub><br>
<sub>**Förkrav**: -</sub><br>
<sub>**Indata**: .env-fil med variablerna IMAP_CLIENT_ID, IMAP_CLIENT_SECRET och IMAP_USER, kopplade till mailadressen som applikationen kopplas upp mot.</sub><br>
<sub>**Utdata**: Redirect till /</sub><br>
<sub>**Kontroll av efterkrav**: -</sub><br>
<sub>**Genomförande**:</sub><br>
<sub>1. Starta applikationen med docker-compose.</sub><br>
<sub>2. Placera .env-filen i node mappen, bredvid package.json.</sub><br>
<sub>3. Öppna adressen /node/auth/google i valfri webbläsare.</sub><br>
<sub>4. Välj mailen dev@futurumdigital.se.</sub><br>
<sub>5. Uppge det korrekta lösenordet.</sub><br>
<sub>6. Tillåt applikationen åtkomst till mailadressen.</sub><br>
<sub>7. Kontrollera förväntat resultat enligt ovan.</sub><br>
<br>
#### Testfall 2 - Autentisera servern mot mailadressen som ska bevakas - misslyckad autentisering
<sub>**Krav som testas**: #8, #13-#21</sub><br>
<sub>**Förkrav**: -</sub><br>
<sub>**Indata**: .env-fil med variablerna IMAP_CLIENT_ID, IMAP_CLIENT_SECRET och IMAP_USER, kopplade till mailadressen som applikationen kopplas upp mot.</sub><br>
<sub>**Utdata**: Redirect till /node/auth/google/callback?error=access_denied#</sub><br>
<sub>**Kontroll av efterkrav**: -</sub><br>
<sub>**Genomförande**:</sub><br>
<sub>1. Starta applikationen med docker-compose.</sub><br>
<sub>2. Placera .env-filen i node mappen, bredvid package.json.</sub><br>
<sub>3. Öppna adressen /node/auth/google i valfri webbläsare.</sub><br>
<sub>4. Välj mailen dev@futurumdigital.se.</sub><br>
<sub>5. Uppge ett inkorrekt lösenord.</sub><br>
<sub>6. Tillåt applikationen åtkomst till mailadressen.</sub><br>
<sub>7. Kontrollera förväntat resultat enligt ovan.</sub><br>
<br>
#### Testfall 3 - Autentisera servern mot mailadressen som ska bevakas - nekad autentisering
<sub>**Krav som testas**: #8, #13-#21</sub><br>
<sub>**Förkrav**: -</sub><br>
<sub>**Indata**: .env-fil med variablerna IMAP_CLIENT_ID, IMAP_CLIENT_SECRET och IMAP_USER, kopplade till mailadressen som applikationen kopplas upp mot.</sub><br>
<sub>**Utdata**: Redirect till /node/auth/google/callback?error=access_denied#</sub><br>
<sub>**Kontroll av efterkrav**: -</sub><br>
<sub>**Genomförande**:</sub><br>
<sub>1. Starta applikationen med docker-compose.</sub><br>
<sub>2. Placera .env-filen i node mappen, bredvid package.json.</sub><br>
<sub>3. Öppna adressen /node/auth/google i valfri webbläsare.</sub><br>
<sub>4. Välj mailen dev@futurumdigital.se.</sub><br>
<sub>5. Tillåt inte applikationen åtkomst till mailadressen.</sub><br>
<sub>6. Kontrollera förväntat resultat enligt ovan.</sub><br>
<br>


## Testfall - Klient

### Manuella tester
#### Testfall 1 - Lägga till ny mailadress
<sub>**Krav som testas**: #17</sub><br>
<sub>**Förkrav**: Applikationen är startad och användaren är autentiserad.</sub><br>
<sub>**Indata**: Data för tilläggning av ny mailadress. Företag: Företaget AB. Mailadress: foretaget@foretaget.se</sub><br>
<sub>**Utdata**: Rutan för inmatning stängs och systemet bekräftar med — "**Mailadressen har lagts till i listan.**"</sub><br>
<sub>**Kontroll av efterkrav**: Den nya mailadressen med inmatad data har lagts till i kundlistan.</sub><br>
<sub>**Genomförande**:</sub><br>
<sub>1. Navigera till /clients eller Kundlista i menyn.</sub><br>
<sub>2. Tryck på knappen "Lägg till kund" för att öppna rutan för att lägga till en ny mailadress.</sub><br>
<sub>3. Fyll i företagsnamn och mailadress. Tryck "Spara".</sub><br>
<sub>4. Kontrollera förväntat resultat enligt ovan.</sub><br>
<br>

#### Testfall 2 - Lägga till ny mailadress - felaktig input
<sub>**Krav som testas**: #17</sub><br>
<sub>**Förkrav**: Applikationen är startad och användaren är autentiserad.</sub><br>
<sub>**Indata**: Data för tilläggning av ny mailadress. Företag: Företaget AB. Mailadress: abc</sub><br>
<sub>**Utdata**: Datan är fortfarande ifylld och felmeddelande visas — "**Felaktigt format på mailadressen.**"</sub><br>
<sub>**Kontroll av efterkrav**: Den nya mailadressen med inmatad data har *inte* lagts till i kundlistan.</sub><br>
<sub>**Genomförande**:</sub><br>
<sub>1. Navigera till /clients eller Kundlista i menyn.</sub><br>
<sub>2. Tryck på knappen "Lägg till kund" för att öppna rutan för att lägga till en ny mailadress.</sub><br>
<sub>3. Fyll i företagsnamn och mailadress. Tryck "Spara".</sub><br>
<sub>4. Kontrollera förväntat resultat enligt ovan.</sub><br>
<br>

#### Testfall 3 - Lägga till ny mailadress - redan registrerad mailadress
<sub>**Krav som testas**: #17</sub><br>
<sub>**Förkrav**: Applikationen är startad och användaren är autentiserad. Kund med mailadress kund@kunden.se finns redan registrerad.</sub><br>
<sub>**Indata**: Data för tilläggning av ny mailadress. Företag: Kunden AB. Mailadress: kund@kunden.se</sub><br>
<sub>**Utdata**: Datan är fortfarande ifylld och felmeddelande visas — "**Mailadressen finns redan registrerad.**"</sub><br>
<sub>**Kontroll av efterkrav**: Den nya mailadressen med inmatad data har *inte* lagts till i kundlistan.</sub><br>
<sub>**Genomförande**:</sub><br>
<sub>1. Navigera till /clients eller Kundlista i menyn.</sub><br>
<sub>2. Tryck på knappen "Lägg till kund" för att öppna rutan för att lägga till en ny mailadress.</sub><br>
<sub>3. Fyll i företagsnamn och mailadress. Tryck "Spara".</sub><br>
<sub>4. Kontrollera förväntat resultat enligt ovan.</sub><br>
<br>

#### Testfall 4 - Ändra status på ärende - flerkortsvy, uppdatering till kund
<sub>**Krav som testas**: #11, #15, #19</sub><br>
<sub>**Förkrav**: Applikationen är startad och användaren är autentiserad.</sub><br>
<sub>**Indata**: -</sub><br>
<sub>**Utdata**: Bekräftelse från systemet visas i pop-up rutan — "**Status för ärendet har blivit uppdaterad och vidarebefodrat till kund.**"</sub><br>
<sub>**Kontroll av efterkrav**: Kortet för ärendet har uppdaterats med den nya statusen och statusfärgen. Kunden har fått ett mail om statusuppdateringen.</sub><br>
<sub>**Genomförande**:</sub><br>
<sub>1. Navigera till Alla ärenden i menyn.</sub><br>
<sub>2. Välj ett kort med status "Ej påbörjad" och röd statusfärg. Klicka på statustexten för att öppna en dropdown-meny.</sub><br>
<sub>3. Välj status "Påbörjad".</sub><br>
<sub>4. En pop-up ruta visas och frågar om statusuppdateringen ska skickas till kund. Välj "Ja".</sub><br>
<sub>6. Kontrollera förväntat resultat enligt ovan.</sub><br>
<br>

#### Testfall 5 - Ändra status på ärende - enskild kortvy, utan uppdatering till kund
<sub>**Krav som testas**: #11, #15, #19</sub><br>
<sub>**Förkrav**: Applikationen är startad och användaren är autentiserad.</sub><br>
<sub>**Indata**: -</sub><br>
<sub>**Utdata**: Bekräftelse från systemet visas i pop-up rutan — "**Status för ärendet har blivit uppdaterad.**"</sub><br>
<sub>**Kontroll av efterkrav**: Ärendet har uppdaterats med den nya statusen och statusfärgen. Kunden har *inte* fått något mail om statusuppdateringen.</sub><br>
<sub>**Genomförande**:</sub><br>
<sub>1. Navigera till Alla ärenden i menyn.</sub><br>
<sub>2. Välj ett kort med status "Ej påbörjad" och röd statusfärg. Klicka på ärendetiteln för att tas vidare till ärendets enskilda vy.</sub><br>
<sub>3. Vid "STATUS:", tryck på statustexten för att öppna en dropdown-meny.</sub><br>
<sub>4. Välj status "Påbörjad".</sub><br>
<sub>5. En pop-up ruta visas och frågar om statusuppdateringen ska skickas till kund. Välj "Nej".</sub><br>
<sub>6. Kontrollera förväntat resultat enligt ovan.</sub><br>
<br>

### Användartester