### Syfte och målsättning
<sub>Syftet med testningen är att kunna säkerställa kvalitén kontinuerligt under utvecklingens gång för den applikation som i slutskedet ska levereras till kund. Det slutgiltiga målet är i sin tur att få bekräftat att det som levereras har en fungerande grundfunktionalitet. Prioritering kommer främst att ligga på att leverera de [funktionella krav](https://github.com/1dv611-futurum-project/futurum-project/wiki/Kravspecifikation#funktionella-krav-f%C3%B6lj-processen-h%C3%A4r) som har efterfrågats av kund.  Testningen kommer också delvis att rikta sig mot de [kvalitetskrav](https://github.com/1dv611-futurum-project/futurum-project/wiki/Kravspecifikation#kvalitetskrav-f%C3%B6lj-processen-h%C3%A4r) som finns. Det här gäller endast kvalitetskraven gällande säkerhet, användarvänlighet, webbstandarder och svarstid. Testprocessen ska med andra ord se till så att systemet lever upp till de förväntade kraven.</sub>

### Verktyg
<sub>För att genomföra olika tester kommer vi att använda oss av följande verktyg:</sub>
* <sub>**Postman**, för att testa mot olika api-routes på servern. Förutsättningen för att det här ska fungera är att man har [Postman](https://www.getpostman.com/) installerat lokalt och även har importerat den Postman Collection som följer med systemet.</sub>
* <sub>**Mocha, Chai, Enzyme och Karma**, för att kunna testa specifika funktioner eller block av kod. För att kunna köra testerna behöver man gå in i en specifik Docker-container och där i köra `npm run test`.</sub>

### Strategi
<sub>Automatiska tester kommer att användas för att testa de funktionella kraven som beskrivs i kravspecifikationen. Dessa tester kan ses som enhetstester och kan testa både mindre, isolerade funktioner eller hela klasser. De automatiserade testerna bör köras varje gång server- eller klientapplikationen startas.</sub>

<sub>Manuella tester genomförs löpande under arbetets gång inom gruppen. Varje gång ny funktionalitet läggs till testas denna först manuellt kontinuerligt under utvecklingens gång innan den anses vara helt färdigställd. Flertalet manuella tester kommer även att behöva genomföras för att kunna simulera att mail inkommer till applikationen.</sub>

<sub>Även användargränssnitts-tester genomförs löpande under utveckling av klienten för att säkerställa att användargränssnittet är tydligt och användarvänligt i enlighet med de kvalitetskrav som har satts upp.</sub>

<sub>Ett begränsat antal explorativa användartester kommer att genomföras av kund för att få feedback av de tilltänkta slutanvändarna av systemet. Dessa användartester kommer endast att genomföras vid varje delleverans till kund, och genomförs i den mängd som kunden önskar och hinner med. Resultat från användartester bör prioriteras då de kommer direkt från slutanvändaren.</sub>

<sub>Explorativ testning genomförs också i slutet av varje iteration av alla i gruppen för både klient och server. På så sätt kan eventuella buggar som inte täcks in av övriga tester fångas upp och uppmärksammas. </sub>


### Ansvarsfördelning
<sub>Det övergripande ansvaret som innebär att hålla testspecifikationen uppdaterad, samt se till att testfall skrivs och resultaten rapporteras ligger hos testansvarig (Miranda). Testerna kommer i många fall vara uppdelade mellan klient/server, och därmed ligger också ansvaret för dessa tester hos respektive utvecklingsgrupp. Ansvariga för att skriva och köra tester på servern är i första hand Molly och Johan. Ansvariga för att skriva och köra testfall på klienten är i första hand Miranda och Jesper. Eventuella användartester som kommer behöva göras ansvarar gruppen gemensamt för att genomföra och strukturera upp.</sub>

<sub>Eventuella buggar som upptäcks under testprocessen ska inte pushas upp på Github utan försöka åtgärdas lokalt. Går det inte att åtgärda utan att ta hjälp av annan gruppmedlem som behöver tillgång till samma kod, ska det i så fall skapas en separat branch för att hantera buggen. Branchen får inte mergas in i master förrän buggen är fullständigt åtgärdad. Skulle en bugg mot förmodan hittas i den kod som redan ligger på Github, rapporteras det här i första hand till den som har producerat koden, och i andra hand till nästa medlem som är ansvarig inom området (klient/server). Alla kända buggar som upptäcks under testprocessen ska dokumenteras i de veckovisa testrapporterna och sammanställs dessutom som issues i ett [separat projekt](https://github.com/1dv611-futurum-project/futurum-project/projects/7) där de sedan kan tilldelas en ansvarig och hanteras löpande.</sub>

## Systemtester
### Systemtest 1: Säkerhet — Kvalitetskrav #9, Funktionellt krav #25
|<sub>Område</sub>|<sub>ID</sub>|<sub>Testfall</sub>|<sub>Testform</sub>|
|----|--------|------------|---------|
|<sub>Server</sub>|<sub>T1</sub>|<sub>[Autentisera servern mot mailadressen som ska bevakas - lyckad autentiering](https://github.com/1dv611-futurum-project/futurum-project/wiki/Testspecifikation#testfall-1---autentisera-servern-mot-mailadressen-som-ska-bevakas---lyckad-autentisering)</sub>|<sub>Manuellt</sub>|
|<sub>Server</sub>|<sub>T2</sub>|<sub>[Autentisera servern mot mailadressen som ska bevakas - autentiering behöver en upprepas](https://github.com/1dv611-futurum-project/futurum-project/wiki/Testspecifikation#testfall-2---autentisera-servern-mot-mailadressen-som-ska-bevakas---autentiering-behöver-ej-upprepas)</sub>|<sub>Manuellt</sub>|
|<sub>Server</sub>|<sub>T3</sub>|<sub>[Autentisera servern mot mailadressen som ska bevakas - autentiering upprepas om cookie tas bort](https://github.com/1dv611-futurum-project/futurum-project/wiki/Testspecifikation#testfall-3---autentisera-servern-mot-mailadressen-som-ska-bevakas---autentiering-upprepas-om-cookie-tas-bort)</sub>|<sub>Manuellt</sub>|
|<sub>Server</sub>|<sub>T4</sub>|<sub>[Autentisera servern mot mailadressen som ska bevakas - autentiering upprepas om server startas om](https://github.com/1dv611-futurum-project/futurum-project/wiki/Testspecifikation#testfall-4---autentisera-servern-mot-mailadressen-som-ska-bevakas---autentiering-upprepas-om-server-startas-om)</sub>|<sub>Manuellt</sub>|
|<sub>Server</sub>|<sub>T5</sub>|<sub>[Autentisera servern mot mailadressen som ska bevakas - misslyckad autentiering](https://github.com/1dv611-futurum-project/futurum-project/wiki/Testspecifikation#testfall-5---autentisera-servern-mot-mailadressen-som-ska-bevakas---misslyckad-autentisering)</sub>|<sub>Manuellt</sub>|
|<sub>Server</sub>|<sub>T6</sub>|<sub>[Autentisera servern mot mailadressen som ska bevakas - nekad autentiering](https://github.com/1dv611-futurum-project/futurum-project/wiki/Testspecifikation#testfall-6---autentisera-servern-mot-mailadressen-som-ska-bevakas---nekad-autentisering)</sub>|<sub>Manuellt</sub>|

### Systemtest 2: Visning av ärenden — Funktionellt krav #14, #17, #23
|<sub>Område</sub>|<sub>ID</sub>|<sub>Testfall</sub>|<sub>Testform</sub>|
|----|--------|------------|---------|
|<sub>Server</sub>|<sub>T1</sub>|<sub>[Autentisera servern mot mailadressen som ska bevakas - lyckad autentiering](https://github.com/1dv611-futurum-project/futurum-project/wiki/Testspecifikation#testfall-1---autentisera-servern-mot-mailadressen-som-ska-bevakas---lyckad-autentisering)</sub>|<sub>Manuellt</sub>|
|<sub>Server</sub>|<sub>T2</sub>|<sub>[Autentisera servern mot mailadressen som ska bevakas - autentiering behöver ej upprepas](https://github.com/1dv611-futurum-project/futurum-project/wiki/Testspecifikation#testfall-2---autentisera-servern-mot-mailadressen-som-ska-bevakas---autentiering-behöver-ej-upprepas)</sub>|<sub>Manuellt</sub>|
|<sub>Server</sub>|<sub>T3</sub>|<sub>[Autentisera servern mot mailadressen som ska bevakas - autentiering upprepas om cookie tas bort](https://github.com/1dv611-futurum-project/futurum-project/wiki/Testspecifikation#testfall-3---autentisera-servern-mot-mailadressen-som-ska-bevakas---autentiering-upprepas-om-cookie-tas-bort)</sub>|<sub>Manuellt</sub>|
|<sub>Server</sub>|<sub>T4</sub>|<sub>[Autentisera servern mot mailadressen som ska bevakas - autentiering upprepas om server startas om](https://github.com/1dv611-futurum-project/futurum-project/wiki/Testspecifikation#testfall-4---autentisera-servern-mot-mailadressen-som-ska-bevakas---autentiering-upprepas-om-server-startas-om)</sub>|<sub>Manuellt</sub>|

### Systemtest 3: Ärendehantering — Funktionellt krav #16, #19, #20, #24
|<sub>Område</sub>|<sub>ID</sub>|<sub>Testfall</sub>|<sub>Testform</sub>|
|----|--------|------------|---------|
|<sub>Server</sub>|<sub>T1</sub>|<sub>[Autentisera servern mot mailadressen som ska bevakas - lyckad autentiering](https://github.com/1dv611-futurum-project/futurum-project/wiki/Testspecifikation#testfall-1---autentisera-servern-mot-mailadressen-som-ska-bevakas---lyckad-autentisering)</sub>|<sub>Manuellt</sub>|
|<sub>Server</sub>|<sub>T2</sub>|<sub>[Autentisera servern mot mailadressen som ska bevakas - autentiering behöver ej upprepas](https://github.com/1dv611-futurum-project/futurum-project/wiki/Testspecifikation#testfall-2---autentisera-servern-mot-mailadressen-som-ska-bevakas---autentiering-behöver-ej-upprepas)</sub>|<sub>Manuellt</sub>|
|<sub>Server</sub>|<sub>T3</sub>|<sub>[Autentisera servern mot mailadressen som ska bevakas - autentiering upprepas om cookie tas bort](https://github.com/1dv611-futurum-project/futurum-project/wiki/Testspecifikation#testfall-3---autentisera-servern-mot-mailadressen-som-ska-bevakas---autentiering-upprepas-om-cookie-tas-bort)</sub>|<sub>Manuellt</sub>|
|<sub>Server</sub>|<sub>T4</sub>|<sub>[Autentisera servern mot mailadressen som ska bevakas - autentiering upprepas om server startas om](https://github.com/1dv611-futurum-project/futurum-project/wiki/Testspecifikation#testfall-4---autentisera-servern-mot-mailadressen-som-ska-bevakas---autentiering-upprepas-om-server-startas-om)</sub>|<sub>Manuellt</sub>|
|<sub>Klient</sub>|<sub>T4</sub>|<sub>[Ändra status på ärende - flerkortsvy, uppdatering till kund](https://github.com/1dv611-futurum-project/futurum-project/wiki/Testspecifikation#testfall-4---%C3%84ndra-status-p%C3%A5-%C3%A4rende---flerkortsvy-uppdatering-till-kund)</sub>|<sub>Manuellt</sub>|
|<sub>Klient</sub>|<sub>T5</sub>|<sub>[Ändra status på ärende - enskild kortvy, utan uppdatering till kund](https://github.com/1dv611-futurum-project/futurum-project/wiki/Testspecifikation#testfall-5---%C3%84ndra-status-p%C3%A5-%C3%A4rende---enskild-kortvy-utan-uppdatering-till-kund)</sub>|<sub>Manuellt</sub>|
|<sub>Klient</sub>|<sub>T6</sub>|<sub>[Tilldela ärende](https://github.com/1dv611-futurum-project/futurum-project/wiki/Testspecifikation#testfall-6---tilldela-%C3%A4rende)</sub>|<sub>Manuellt</sub>|
|<sub>Klient</sub>|<sub>T7</sub>|<sub>[Tilldela ärende - ta bort tilldelning](https://github.com/1dv611-futurum-project/futurum-project/wiki/Testspecifikation#testfall-7---tilldela-%C3%A4rende---ta-bort-tilldelning)</sub>|<sub>Manuellt</sub>|
|<sub>Klient</sub>|<sub>T8</sub>|<sub>[Svara på ett ärende](https://github.com/1dv611-futurum-project/futurum-project/wiki/Testspecifikation#testfall-8---svara-p%C3%A5-ett-%C3%A4rende)</sub>|<sub>Manuellt</sub>|
|<sub>Klient</sub>|<sub>T9</sub>|<sub>[Svara på ett ärende - med radbrytning](https://github.com/1dv611-futurum-project/futurum-project/wiki/Testspecifikation#testfall-9---svara-p%C3%A5-ett-%C3%A4rende---med-radbrytning)</sub>|<sub>Manuellt</sub>|
|<sub>Klient</sub>|<sub>T10</sub>|<sub>[Svara på ett ärende - med formatering](https://github.com/1dv611-futurum-project/futurum-project/wiki/Testspecifikation#testfall-10---svara-p%C3%A5-ett-%C3%A4rende---med-formatering)</sub>|<sub>Manuellt</sub>|


### Systemtest 4: Inkomna mail — Funktionellt krav #15, #21, #22
|<sub>Område</sub>|<sub>ID</sub>|<sub>Testfall</sub>|<sub>Testform</sub>|
|----|--------|------------|---------|
|<sub>Server</sub>|<sub>T1</sub>|<sub>[Autentisera servern mot mailadressen som ska bevakas - lyckad autentiering](https://github.com/1dv611-futurum-project/futurum-project/wiki/Testspecifikation#testfall-1---autentisera-servern-mot-mailadressen-som-ska-bevakas---lyckad-autentisering)</sub>|<sub>Manuellt</sub>|
|<sub>Server</sub>|<sub>T2</sub>|<sub>[Autentisera servern mot mailadressen som ska bevakas - autentiering behöver ej upprepas](https://github.com/1dv611-futurum-project/futurum-project/wiki/Testspecifikation#testfall-2---autentisera-servern-mot-mailadressen-som-ska-bevakas---autentiering-behöver-ej-upprepas)</sub>|<sub>Manuellt</sub>|
|<sub>Server</sub>|<sub>T3</sub>|<sub>[Autentisera servern mot mailadressen som ska bevakas - autentiering upprepas om cookie tas bort](https://github.com/1dv611-futurum-project/futurum-project/wiki/Testspecifikation#testfall-3---autentisera-servern-mot-mailadressen-som-ska-bevakas---autentiering-upprepas-om-cookie-tas-bort)</sub>|<sub>Manuellt</sub>|
|<sub>Server</sub>|<sub>T4</sub>|<sub>[Autentisera servern mot mailadressen som ska bevakas - autentiering upprepas om server startas om](https://github.com/1dv611-futurum-project/futurum-project/wiki/Testspecifikation#testfall-4---autentisera-servern-mot-mailadressen-som-ska-bevakas---autentiering-upprepas-om-server-startas-om)</sub>|<sub>Manuellt</sub>|
|<sub>Server</sub>|<sub>T7</sub>|<sub>[Ta emot mail som skickas till den autentierade mailadressen](https://github.com/1dv611-futurum-project/futurum-project/wiki/Testspecifikation#testfall-7---ta-emot-mail-som-skickas-till-den-autentierade-mailadressen)</sub>|<sub>Manuellt</sub>|

### Systemtest 5: Registrerade mailadresser — Funktionellt krav #18
|<sub>Område</sub>|<sub>ID</sub>|<sub>Testfall</sub>|<sub>Testform</sub>|
|----|--------|------------|---------|
|<sub>Klient</sub>|<sub>T1</sub>|<sub>[Lägga till ny mailadress](https://github.com/1dv611-futurum-project/futurum-project/wiki/Testspecifikation#testfall-1---l%C3%A4gga-till-ny-mailadress)</sub>|<sub>Manuellt</sub>|
|<sub>Klient</sub>|<sub>T2</sub>|<sub>[Lägga till ny mailadress - felaktig input](https://github.com/1dv611-futurum-project/futurum-project/wiki/Testspecifikation#testfall-2---l%C3%A4gga-till-ny-mailadress---felaktig-input)</sub>|<sub>Manuellt</sub>|
|<sub>Klient</sub>|<sub>T3</sub>|<sub>[Lägga till ny mailadress - redan registrerad mailadress](https://github.com/1dv611-futurum-project/futurum-project/wiki/Testspecifikation#testfall-3---l%C3%A4gga-till-ny-mailadress---redan-registrerad-mailadress)</sub>|<sub>Manuellt</sub>|


## Testfall - Server

#### Förkrav för testning på servern
<sub>En .env fil måste ha lagts i roten av `src`-mappen i node-containern. Filen måste innehålla följande variabler:
```
IMAP_USER=[mailadressen appen körs mot]
IMAP_FORWARDING_ADDRESS=[mailaddressen mail ska vidarebefodras till]
IMAP_REDIRECT_URL=[redirect-URL som stämmer överens med det registerarde projektet hos google]
IMAP_CLIENT_ID=[CLient ID från det registerade projektet hos google]
IMAP_CLIENT_SECRET=[Client secret från det registrerade projektet hos google]
```
</sub>

<sub>För de manuella testerna måste du även ha tillgång till lösenordet till den mail som uppges som IMAP_USER i .env-filen.</sub>

### Automatiska tester

#### Procedur
<sub>För att köra de automatiska testerna behöver man bygga projektet och se till att det är uppe och igång med `docker-compose up -d`. Testerna på servern körs sedan i node-containern med hjälp av `npm test`-kommandot och använder sig av mocha och chai. Det fullständiga kommandot för att köra testerna är med andra ord (efter att man har försäkrat sig om att Docker är igång som det ska) `docker exec -t -i futurumproject_node_1 npm run test`.</sub>  

<sub>Alla tester ska gå igenom för varje iteration. De automatiska testerna [hittar ni här](https://github.com/1dv611-futurum-project/futurum-project/tree/master/services/node/test). Utöver det här, kan också Postman-tester köras mot API:t. Större delen av kommunikationen mellan klient och server hanteras av Websocketen, och Postman-testerna testar därför endast av autentiseringen. Eftersom denna sker genom en dynamiskt skapad cookie som baseras på en OAuth-inloggning, testar Postman-testerna enbart att alla routes där en request görs utan korrekt cookie omdirigerar användaren till att logga in med OAuth hos Google. För att köra Postman-testerna, se till att systemet är uppe enligt ovan, navigera till `services/node/test/postman-test` i terminalen, och kör sedan kommandot: </sub>
<sub>
```
newman run Futurum.postman_collection.json -e Futurum.postman_collection_environment.json
```
</sub>

### Manuella tester
#### Procedur
<sub>För att köra de manuella testerna behöver man bygga projektet och se till att det är uppe och igång med `docker-compose up -d`.</sub>

#### Testfall 1 - Autentisera servern mot mailadressen som ska bevakas - lyckad autentisering
<sub>**Krav som testas**: #9, #14-#15, #17-#19, #21-#22</sub><br>
<sub>**Förkrav**: Förkrav enligt ovan. Rensa webbläsaren från cookies.</sub><br>
<sub>**Indata**: .env enligt ovan. Lösenord till den uppgivna testmailen.</sub><br>
<sub>**Utdata**: Redirect till /</sub><br>
<sub>**Kontroll av efterkrav**: En cookie som heter jwt har lagrats i webbläsaren.</sub><br>
<sub>**Genomförande**:</sub><br>
<sub>1. Placera .env-filen i node mappen, bredvid package.json.</sub><br>
<sub>2. Starta applikationen med `docker-compose up -d` och verifiera att den har gått igång utan problem.</sub><br>
<sub>3. Öppna adressen / i valfri webbläsare.</sub><br>
<sub>4. Bli redirectad till googles oauth-tjänst..</sub><br>
<sub>5. Välj mailen som uppgavs som IMAP_USER i `.env`-filen.</sub><br>
<sub>6. Uppge det korrekta lösenordet.</sub><br>
<sub>7. Tillåt applikationen åtkomst till mailadressen.</sub><br>
<sub>8. Kontrollera förväntat resultat enligt ovan.</sub><br>
<br>
#### Testfall 2 - Autentisera servern mot mailadressen som ska bevakas - autentiering behöver ej upprepas
<sub>**Krav som testas**: #9, #14-#15, #17-#19, #21-#22</sub><br>
<sub>**Förkrav**: Testfall 1 är utfört och passerar.</sub><br>
<sub>**Indata**: -</sub><br>
<sub>**Utdata**: React-applikationen visas.</sub><br>
<sub>**Kontroll av efterkrav**: En cookie som heter jwt har lagrats i webbläsaren.</sub><br>
<sub>**Genomförande**:</sub><br>
<sub>1. Testfall 1.</sub><br>
<sub>3. Ladda om sidan på path /.</sub><br>
<sub>4. Kontrollera förväntat resultat enligt ovan.</sub><br>
<br>
#### Testfall 3 - Autentisera servern mot mailadressen som ska bevakas - autentiering upprepas om cookie tas bort
<sub>**Krav som testas**: #9, #14-#15, #17-#19, #21-#22</sub><br>
<sub>**Förkrav**: Testfall 1 är utfört och passerar.</sub><br>
<sub>**Indata**: -</sub><br>
<sub>**Utdata**: Googles OAuth-tjänst visas.</sub><br>
<sub>**Kontroll av efterkrav**: En cookie som heter jwt har lagrats i webbläsaren.</sub><br>
<sub>**Genomförande**:</sub><br>
<sub>1. Testfall 1.</sub><br>
<sub>2. Rensa webbläsarens cookies.</sub><br>
<sub>3. Ladda om sidan på path /.</sub><br>
<sub>4. Kontrollera förväntat resultat enligt ovan.</sub><br>
<br>
#### Testfall 4 - Autentisera servern mot mailadressen som ska bevakas - autentiering upprepas om server startas om
<sub>**Krav som testas**: #9, #14-#15, #17-#19, #21-#22</sub><br>
<sub>**Förkrav**: Testfall 1 är utfört och passerar.</sub><br>
<sub>**Indata**: -</sub><br>
<sub>**Utdata**: Googles OAuth-tjänst visas.</sub><br>
<sub>**Kontroll av efterkrav**: En cookie som heter jwt har lagrats i webbläsaren.</sub><br>
<sub>**Genomförande**:</sub><br>
<sub>1. Testfall 1.</sub><br>
<sub>2. Starta om servern genom `docker-compose stop node` och `docker-compose up -d node`.</sub><br>
<sub>3. Ladda om sidan på path /.</sub><br>
<sub>4. Kontrollera förväntat resultat enligt ovan.</sub><br>
<br>
#### Testfall 5 - Autentisera servern mot mailadressen som ska bevakas - misslyckad autentisering
<sub>**Krav som testas**: #9</sub><br>
<sub>**Förkrav**: Förkrav enligt ovan. Rensa webbläsaren från cookies.</sub><br>
<sub>**Indata**: .env enligt ovan. Felaktigt lösenord till den uppgivna testmailen.</sub><br>
<sub>**Utdata**: Redirect till /node/auth/google/callback?error=access_denied#</sub><br>
<sub>**Kontroll av efterkrav**: -</sub><br>
<sub>**Genomförande**:</sub><br>
<sub>1. Placera .env-filen i node mappen, bredvid package.json.</sub><br>
<sub>2. Starta applikationen med `docker-compose up -d`.</sub><br>
<sub>3. Öppna adressen / i valfri webbläsare.</sub><br>
<sub>4. Välj mailen som är uppgiven i -env-filen som IMAP_USER.</sub><br>
<sub>5. Uppge ett inkorrekt lösenord.</sub><br>
<sub>6. Tillåt applikationen åtkomst till mailadressen.</sub><br>
<sub>7. Kontrollera förväntat resultat enligt ovan.</sub><br>
<br>
#### Testfall 6 - Autentisera servern mot mailadressen som ska bevakas - nekad autentisering
<sub>**Krav som testas**: #9</sub><br>
<sub>**Förkrav**: -</sub><br>
<sub>**Indata**: .env-fil med variablerna IMAP_CLIENT_ID, IMAP_CLIENT_SECRET och IMAP_USER, kopplade till mailadressen som applikationen kopplas upp mot.</sub><br>
<sub>**Utdata**: Redirect till /node/auth/google/callback?error=access_denied#</sub><br>
<sub>**Kontroll av efterkrav**: -</sub><br>
<sub>**Genomförande**:</sub><br>
<sub>1. Placera .env-filen i node mappen, bredvid package.json.</sub><br>
<sub>2. Starta applikationen med `docker-compose up -d`.</sub><br>
<sub>3. Öppna adressen / i valfri webbläsare.</sub><br>
<sub>4. Välj mailen som är uppgiven i .env-filen som IMAP_USER.</sub><br>
<sub>5. Tillåt inte applikationen åtkomst till mailadressen.</sub><br>
<sub>6. Kontrollera förväntat resultat enligt ovan.</sub><br>
<br>

#### Testfall 7 - Ta emot mail som skickas till den autentierade mailadressen
<sub>**Krav som testas**: #15</sub><br>
<sub>**Förkrav**: Server - T1</sub><br>
<sub>**Indata**: Rubrik: Test, Innehåll: Test, Mailadress: [samma som IMAP_USER i .env]</sub><br>
<sub>**Utdata**: Ett ärendekort med rubrik och innehåll enligt ovan visas på klienten.</sub><br>
<sub>**Kontroll av efterkrav**: Mailet har markerats som läst i den givna mailens inkorg.</sub><br>
<sub>**Genomförande**:</sub><br>
<sub>1. Genomför Server - Testfall 1.</sub><br>
<sub>2. Skriv ett mail från valfri mailadress till testmailen, enligt indata ovan.</sub><br>
<sub>3. Vänta upp till 60 sekunder.</sub><br>
<sub>4. Kontrollera utdata enligt ovan.</sub><br>
<br>


***


## Testfall - Klient
### Automatiska tester
#### Procedur
<sub>För att köra de automatiska testerna behöver man bygga projektet och se till att det är uppe och igång med `docker-compose up -d`. Gå sedan in i client-containern och kör `npm test`. Testerna körs med Karma i en "Chromium Headless Browser"-miljö, och använder enzyme, mocha och chai för att simulera klienten och exekvera testerna. Alla tester ska gå igenom för varje iteration. De automatiska testerna [hittar ni här](https://github.com/1dv611-futurum-project/futurum-project/tree/master/services/client/test).</sub>

### Manuella tester
#### Procedur
<sub>För att köra de manuella testerna behöver man bygga projektet och se till att det är uppe och igång med `docker-compose up -d`.</sub>

#### Testfall 1 - Lägga till ny mailadress
<sub>**Krav som testas**: #18</sub><br>
<sub>**Förkrav**: Applikationen är startad och användaren är autentierad.</sub><br>
<sub>**Indata**: Data för tilläggning av ny mailadress. Företag: Företaget AB. Mailadress: foretaget@foretaget.se</sub><br>
<sub>**Utdata**: Rutan för inmatning stängs och systemet bekräftar med — "**Kunden har lagts till i listan.**"</sub><br>
<sub>**Kontroll av efterkrav**: Den nya mailadressen med inmatad data har lagts till i kundlistan.</sub><br>
<sub>**Genomförande**:</sub><br>
<sub>1. Navigera till /clients eller Kundlista i menyn.</sub><br>
<sub>2. Tryck på knappen "Lägg till kund" för att öppna rutan för att lägga till en ny mailadress.</sub><br>
<sub>3. Fyll i företagsnamn och mailadress. Tryck "Spara".</sub><br>
<sub>4. Kontrollera förväntat resultat enligt ovan.</sub><br>
<br>

#### Testfall 2 - Lägga till ny mailadress - felaktig input
<sub>**Krav som testas**: #18</sub><br>
<sub>**Förkrav**: Applikationen är startad och användaren är autentierad.</sub><br>
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
<sub>**Krav som testas**: #18</sub><br>
<sub>**Förkrav**: Applikationen är startad och användaren är autentierad. Kund med mailadress kund@kunden.se finns redan registrerad.</sub><br>
<sub>**Indata**: Data för tilläggning av ny mailadress. Företag: Kunden AB. Mailadress: kund@kunden.se</sub><br>
<sub>**Utdata**: Datan är fortfarande ifylld och felmeddelande visas — "**Mailadressen finns redan registrerad.**"</sub><br>
<sub>**Kontroll av efterkrav**: Den nya mailadressen med inmatad data har *inte* lagts till i kundlistan.</sub><br>
<sub>**Genomförande**:</sub><br>
<sub>1. Navigera till /clients eller Kundlista i menyn.</sub><br>
<sub>2. Tryck på knappen "Lägg till kund" för att öppna rutan och lägga till en ny mailadress.</sub><br>
<sub>3. Fyll i företagsnamn och mailadress. Tryck "Spara".</sub><br>
<sub>4. Kontrollera förväntat resultat enligt ovan.</sub><br>
<br>

#### Testfall 4 - Ändra status på ärende - flerkortsvy, uppdatering till kund
<sub>**Krav som testas**: #12, #16, #20</sub><br>
<sub>**Förkrav**: Applikationen är startad och användaren är autentierad.</sub><br>
<sub>**Indata**: -</sub><br>
<sub>**Utdata**: Bekräftelse från systemet visas — "**Status för ärendet har uppdaterats och mail har skickats till kund.**"</sub><br>
<sub>**Kontroll av efterkrav**: Kortet för ärendet har uppdaterats med den nya statusen och statusfärgen. Kunden har fått ett mail om statusuppdateringen.</sub><br>
<sub>**Genomförande**:</sub><br>
<sub>1. Navigera till Alla ärenden i menyn.</sub><br>
<sub>2. Välj ett kort med status "Ej påbörjad" och röd statusfärg. Klicka på statustexten för att öppna en dropdown-meny.</sub><br>
<sub>3. Välj status "Påbörjad".</sub><br>
<sub>4. En pop-up ruta visas och frågar om statusuppdateringen ska skickas till kund. Välj "Ja".</sub><br>
<sub>6. Kontrollera förväntat resultat enligt ovan.</sub><br>
<br>

#### Testfall 5 - Ändra status på ärende - enskild kortvy, utan uppdatering till kund
<sub>**Krav som testas**: #12, #16, #20</sub><br>
<sub>**Förkrav**: Applikationen är startad och användaren är autentierad.</sub><br>
<sub>**Indata**: -</sub><br>
<sub>**Utdata**: Bekräftelse från systemet visas i pop-up rutan — "**Status för ärendet har uppdaterats.**"</sub><br>
<sub>**Kontroll av efterkrav**: Ärendet har uppdaterats med den nya statusen och statusfärgen. Kunden har *inte* fått något mail om statusuppdateringen.</sub><br>
<sub>**Genomförande**:</sub><br>
<sub>1. Navigera till Alla ärenden i menyn.</sub><br>
<sub>2. Välj ett kort med status "Ej påbörjad" och röd statusfärg. Klicka på ärenderubriken för att tas vidare till ärendets enskilda vy.</sub><br>
<sub>3. Vid "STATUS:", tryck på statustexten för att öppna en dropdown-meny.</sub><br>
<sub>4. Välj status "Påbörjad".</sub><br>
<sub>5. En pop-up ruta visas och frågar om statusuppdateringen ska skickas till kund. Välj "Nej".</sub><br>
<sub>6. Kontrollera förväntat resultat enligt ovan.</sub><br>
<br>

#### Testfall 6 - Tilldela ärende
<sub>**Krav som testas**: #24</sub><br>
<sub>**Förkrav**: Applikationen är startad och användaren är autentierad. Det finns ett ärende som ej har blivit tilldelat.</sub><br>
<sub>**Indata**: -</sub><br>
<sub>**Utdata**: Bekräftelse från systemet visas — "**Ärendet har tilldelats Sebastian Borgstedt.**"</sub><br>
<sub>**Kontroll av efterkrav**: Ärendet har uppdaterats med den nya tilldelningen.</sub><br>
<sub>**Genomförande**:</sub><br>
<sub>1. Navigera till Alla ärenden i menyn.</sub><br>
<sub>2. Välj ett kort med "—" där det står Tilldelad. Klicka på ärenderubriken för att tas vidare till ärendets enskilda vy.</sub><br>
<sub>3. Vid "TILLDELAD:", tryck i rutan för att öppna en dropdown-meny.</sub><br>
<sub>4. Välj "Sebastian Borgstedt".</sub><br>
<sub>5. Kontrollera förväntat resultat enligt ovan.</sub><br>
<br>

#### Testfall 7 - Tilldela ärende - ta bort tilldelning
<sub>**Krav som testas**: #24</sub><br>
<sub>**Förkrav**: Applikationen är startad och användaren är autentierad. Det finns ett ärende som har blivit tilldelat (testfall 6).</sub><br>
<sub>**Indata**: -</sub><br>
<sub>**Utdata**: -</sub><br>
<sub>**Kontroll av efterkrav**: Ärendet har uppdaterats och är inte längre tilldelad någon specifik ansvarig.</sub><br>
<sub>**Genomförande**:</sub><br>
<sub>1. Navigera till Alla ärenden i menyn.</sub><br>
<sub>2. Välj det kort som har tilldelats Sebastian Borgstedt. Klicka på ärenderubriken för att tas vidare till ärendets enskilda vy.</sub><br>
<sub>3. Vid "TILLDELAD:", tryck i rutan för att öppna en dropdown-meny.</sub><br>
<sub>4. Välj "-".</sub><br>
<sub>5. Kontrollera förväntat resultat enligt ovan.</sub><br>
<br>

#### Testfall 8 - Svara på ett ärende
<sub>**Krav som testas**: #19</sub><br>
<sub>**Förkrav**: Applikationen är startad och användaren är autentierad.</sub><br>
<sub>**Indata**: Meddelandetext: "Vi har tagit emot ditt ärende."</sub><br>
<sub>**Utdata**: -</sub><br>
<sub>**Kontroll av efterkrav**: Meddelandet dyker upp nedanför ärendeinformationen som en ny post överst i listan.</sub><br>
<sub>**Genomförande**:</sub><br>
<sub>1. Navigera till Alla ärenden i menyn.</sub><br>
<sub>2. Välj ett kort och klicka på ärenderubriken för att tas vidare till ärendets enskilda vy.</sub><br>
<sub>3. Tryck på den runda knappen intill texten "Skriv ett svar". </sub><br>
<sub>4. I rutan som öppnas, skriv indatan.</sub><br>
<sub>5. Tryck "Skicka".</sub><br>
<sub>6. Kontrollera förväntat resultat enligt ovan.</sub><br>
<br>

#### Testfall 9 - Svara på ett ärende - med radbrytning
<sub>**Krav som testas**: #19</sub><br>
<sub>**Förkrav**: Applikationen är startad och användaren är autentierad.</sub><br>
<sub>**Indata**: Meddelandetext: "Vi har tagit emot ditt ärende. \nMvh\nAnton Myrberg"</sub><br>
<sub>**Utdata**: -</sub><br>
<sub>**Kontroll av efterkrav**: Meddelandet dyker upp nedanför ärendeinformationen som en ny post överst i listan. Meddelandet visar korrekta radbrytningar.</sub><br>
<sub>**Genomförande**:</sub><br>
<sub>1. Navigera till Alla ärenden i menyn.</sub><br>
<sub>2. Välj ett kort och klicka på ärenderubriken för att tas vidare till ärendets enskilda vy.</sub><br>
<sub>3. Tryck på den runda knappen intill texten "Skriv ett svar". </sub><br>
<sub>4. I rutan som öppnas, skriv indatan.</sub><br>
<sub>5. Tryck "Skicka".</sub><br>
<sub>6. Kontrollera förväntat resultat enligt ovan.</sub><br>
<br>

#### Testfall 10 - Svara på ett ärende - med formatering
<sub>**Krav som testas**: #19</sub><br>
<sub>**Förkrav**: Applikationen är startad och användaren är autentierad.</sub><br>
<sub>**Indata**: Meddelandetext: "Vi har tagit emot ditt ärende. Detta skrivs i *kursiv* stil och så någonting i **fet** stil."</sub><br>
<sub>**Utdata**: -</sub><br>
<sub>**Kontroll av efterkrav**: Meddelandet dyker upp nedanför ärendeinformationen som en ny post överst i listan. Meddelandet visar korrekt formatering.</sub><br>
<sub>**Genomförande**:</sub><br>
<sub>1. Navigera till Alla ärenden i menyn.</sub><br>
<sub>2. Välj ett kort och klicka på ärenderubriken för att tas vidare till ärendets enskilda vy.</sub><br>
<sub>3. Tryck på den runda knappen intill texten "Skriv ett svar". </sub><br>
<sub>4. I rutan som öppnas, skriv indatan.</sub><br>
<sub>5. Tryck "Skicka".</sub><br>
<sub>6. Kontrollera förväntat resultat enligt ovan.</sub><br>
<br>
