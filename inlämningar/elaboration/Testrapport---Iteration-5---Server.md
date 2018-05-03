### Info
<sub>**Datum:** 27/4 -18</sub>  
<sub>**Version av systemet:** [v0.5](https://github.com/1dv611-futurum-project/futurum-project/releases/tag/0.4)</sub>  
<sub>**Testmiljö:**  Kubuntu 17.10, Chrome 65 x64</sub>  
<sub>**Systemtest:** Regression: 1-4, Nya tester: 1-4. Se [här](https://github.com/1dv611-futurum-project/dokumentation/blob/master/inlämningar/inception/Testspecifikation.md).</sub>  

### Manuella testfall och status
<sub>För en beskrivning av testfallen, se [här](https://github.com/1dv611-futurum-project/dokumentation/blob/master/inlämningar/inception/Testspecifikation.md).</sub>    

<sub>Denna testrapport berör:</sub>

#### Regressionstest  

|<sub>Testfall</sub>|<sub>Namn</sub>|<sub>Status</sub>|
|----|--------|------------|
|<sub>T1</sub>|<sub>[Autentisera servern mot mailadressen som ska bevakas - lyckad autentiering](https://github.com/1dv611-futurum-project/dokumentation/blob/master/inlämningar/inception/Testspecifikation.md)</sub>|<sub><img src="https://upload.wikimedia.org/wikipedia/commons/thumb/5/50/Yes_Check_Circle.svg/2000px-Yes_Check_Circle.svg.png" width="15"></sub>|
|<sub>T2</sub>|<sub>[Autentisera servern mot mailadressen som ska bevakas - misslyckad autentiering](https://github.com/1dv611-futurum-project/dokumentation/blob/master/inlämningar/inception/Testspecifikation.md)</sub>|<sub><img src="https://upload.wikimedia.org/wikipedia/commons/thumb/5/50/Yes_Check_Circle.svg/2000px-Yes_Check_Circle.svg.png" width="15"></sub>|
|<sub>T3</sub>|<sub>[Autentisera servern mot mailadressen som ska bevakas - misslyckad autentiering](https://github.com/1dv611-futurum-project/dokumentation/blob/master/inlämningar/inception/Testspecifikation.md)</sub>|<sub><img src="https://upload.wikimedia.org/wikipedia/commons/thumb/5/50/Yes_Check_Circle.svg/2000px-Yes_Check_Circle.svg.png" width="15"></sub>|
|<sub>T4</sub>|<sub>[Autentisera servern mot mailadressen som ska bevakas - misslyckad autentiering](https://github.com/1dv611-futurum-project/dokumentation/blob/master/inlämningar/inception/Testspecifikation.md)</sub>|<sub><img src="https://upload.wikimedia.org/wikipedia/commons/thumb/5/50/Yes_Check_Circle.svg/2000px-Yes_Check_Circle.svg.png" width="15"></sub>|
|<sub>T5</sub>|<sub>[Autentisera servern mot mailadressen som ska bevakas - misslyckad autentiering](https://github.com/1dv611-futurum-project/dokumentation/blob/master/inlämningar/inception/Testspecifikation.md)</sub>|<sub><img src="https://upload.wikimedia.org/wikipedia/commons/thumb/5/50/Yes_Check_Circle.svg/2000px-Yes_Check_Circle.svg.png" width="15"></sub>|
|<sub>T6</sub>|<sub>[Autentisera servern mot mailadressen som ska bevakas - nekad autentiering](https://github.com/1dv611-futurum-project/dokumentation/blob/master/inlämningar/inception/Testspecifikation.md)</sub>|<sub><img src="https://upload.wikimedia.org/wikipedia/commons/thumb/5/50/Yes_Check_Circle.svg/2000px-Yes_Check_Circle.svg.png" width="15"></sub>|
|<sub>T7</sub>|<sub>[Ta emot mail som skickas till den autentierade mailadressen](https://github.com/1dv611-futurum-project/dokumentation/blob/master/inlämningar/inception/Testspecifikation.md)</sub>|<sub><img src="https://upload.wikimedia.org/wikipedia/commons/thumb/5/50/Yes_Check_Circle.svg/2000px-Yes_Check_Circle.svg.png" width="15"></sub>|

#### Nya test
|<sub>Testfall</sub>|<sub>Namn</sub>|<sub>Status</sub>|
|----|--------|------------|

### Enhetstester och status
<sub>**Tekniker:** Mocha, Chai </sub>  

<sub>Denna testrapport berör:</sub>

#### Regressionstest

|<sub>Testfall</sub>|<sub>Krav</sub>|<sub>Status</sub>|
|----|--------|------------|
|<sub>[mongoose-models-test-suite.ts](https://github.com/1dv611-futurum-project/futurum-project/blob/server/services/node/test/db-tests/mongoose-models-test-suite.ts)</sub>|<sub>#3, #15-#17</sub>|<sub><img src="https://upload.wikimedia.org/wikipedia/commons/thumb/5/50/Yes_Check_Circle.svg/2000px-Yes_Check_Circle.svg.png" width="15"></sub>|
|<sub>[db-handler-test-suite.ts](https://github.com/1dv611-futurum-project/futurum-project/blob/server/services/node/test/db-tests/db-handler-test-suite.ts)</sub>|<sub>#3, #15-#17</sub>|<sub><img src="https://upload.wikimedia.org/wikipedia/commons/thumb/5/50/Yes_Check_Circle.svg/2000px-Yes_Check_Circle.svg.png" width="15"></sub>|
|<sub>[db-connection-test-suite.ts](https://github.com/1dv611-futurum-project/futurum-project/blob/server/services/node/test/db-tests/db-connection-test-suite.ts)</sub>|<sub>#3, #15-#17</sub>|<sub><img src="https://upload.wikimedia.org/wikipedia/commons/thumb/5/50/Yes_Check_Circle.svg/2000px-Yes_Check_Circle.svg.png" width="15"></sub>|
|<sub>[email-handler-test-suite.ts](https://github.com/1dv611-futurum-project/futurum-project/blob/server/services/node/test/email-tests/email-handler-test-suite.ts)</sub>|<sub>#14, #18</sub>|<sub><img src="https://upload.wikimedia.org/wikipedia/commons/thumb/5/50/Yes_Check_Circle.svg/2000px-Yes_Check_Circle.svg.png" width="15"></sub>|

#### Nya test
|<sub>Testfall</sub>|<sub>Krav</sub>|<sub>Status</sub>|
|----|--------|------------|
|<sub>[xoauth-generator-test-suite.ts](https://github.com/1dv611-futurum-project/futurum-project/blob/server/services/node/test/email-tests/xoauth-generator-test-suite.ts)</sub>|<sub>#14, #15, #19</sub>|<sub><img src="https://upload.wikimedia.org/wikipedia/commons/thumb/5/50/Yes_Check_Circle.svg/2000px-Yes_Check_Circle.svg.png" width="15"></sub>|
|<sub>[imap-connection-test-suite.ts](https://github.com/1dv611-futurum-project/futurum-project/blob/server/services/node/test/email-tests/imap-connection-test-suite.ts)</sub>|<sub>#14, #15, #19</sub>|<sub><img src="https://upload.wikimedia.org/wikipedia/commons/thumb/5/50/Yes_Check_Circle.svg/2000px-Yes_Check_Circle.svg.png" width="15"></sub>|
|<sub>[imap-handler-test-suite.ts](https://github.com/1dv611-futurum-project/futurum-project/blob/server/services/node/test/email-tests/imap-handler-test-suite.ts)</sub>|<sub>#14, #15, #19</sub>|<sub><img src="https://upload.wikimedia.org/wikipedia/commons/thumb/5/50/Yes_Check_Circle.svg/2000px-Yes_Check_Circle.svg.png" width="15"></sub>|
|<sub>[mail-sender-test-suite.ts](https://github.com/1dv611-futurum-project/futurum-project/blob/server/services/node/test/email-tests/mail-sender-test-suite.ts)</sub>|<sub>#14, #15, #19</sub>|<sub><img src="https://upload.wikimedia.org/wikipedia/commons/thumb/5/50/Yes_Check_Circle.svg/2000px-Yes_Check_Circle.svg.png" width="15"></sub>|

#### Postman

<sub>Utöver detta kan Postman-tester köras mot API:t. Största delen av den kommunikativa funktionaliteten i programmet ligger i Websocketen, och Postmantesterna testar därför endast autentieringen. Eftersom autentieringen sker genom en dynamiskt skapad cookie baserat på OAuth-inloggning, testar Postmantesterna enbart att alla routes där ett anrop görs utan korrekt cookie omdirigerar användaren till att logga in med OAuth via Google. För att köra Postmantesterna, se till att systemet är uppe enligt ovan, stå i `services/node/test/postman-test`, och kör kommandot `newman run Futurum.postman_collection.json -e Futurum.postman_collection_environment.json`.</sub>

|<sub>Testfall</sub>|<sub>Krav</sub>|<sub>Status</sub>|
|----|--------|------------|
|<sub>[Futurum.postman_collection.json](https://github.com/1dv611-futurum-project/futurum-project/blob/server/services/node/test/postman-tests/Futurum.postman_collection.json)</sub>|<sub>#9</sub>|<sub><img src="https://upload.wikimedia.org/wikipedia/commons/thumb/5/50/Yes_Check_Circle.svg/2000px-Yes_Check_Circle.svg.png" width="15"></sub>|

### Status på buggar
#### Funna genom planerad testning
|<sub>Testfall</sub>|<sub>Beskrivning av bugg</sub>|<sub>Löst</sub>|
|----|--------|------------|
|<sub>[imap-handler-test-suite.ts](https://github.com/1dv611-futurum-project/futurum-project/blob/server/services/node/test/email-tests/imap-handler-test-suite.ts)</sub>|<sub>Error-eventet genererade inte ett eget fel att skicka vidare.</sub>|<sub><img src="https://upload.wikimedia.org/wikipedia/commons/thumb/5/50/Yes_Check_Circle.svg/2000px-Yes_Check_Circle.svg.png" width="15"></sub>|
|<sub>[imap-handler-test-suite.ts](https://github.com/1dv611-futurum-project/futurum-project/blob/server/services/node/test/email-tests/imap-handler-test-suite.ts)</sub>|<sub>References-headern i inkomna mail orsakade fel om den inte kom in som array.</sub>|<sub><img src="https://upload.wikimedia.org/wikipedia/commons/thumb/5/50/Yes_Check_Circle.svg/2000px-Yes_Check_Circle.svg.png" width="15"></sub>|

#### Funna genom explorativ manuell testning
|<sub>Beskrivning av bugg</sub>|<sub>Löst</sub>|
|--------|------------|
|<sub>Om mail tas bort på mail-servern medan vår server är uppkopplad så genereras ett fel som inte hanteras på vår server.</sub>|<sub><img src="https://upload.wikimedia.org/wikipedia/commons/thumb/5/50/Yes_Check_Circle.svg/2000px-Yes_Check_Circle.svg.png" width="15"></sub>|
|<sub>Mail med rubriker som innnehåller å ä eller ö kodades fel.</sub>|<sub><img src="https://upload.wikimedia.org/wikipedia/commons/thumb/5/50/Yes_Check_Circle.svg/2000px-Yes_Check_Circle.svg.png" width="15"></sub>|

#### Kända buggar som går vidare in i nästa iteration
|<sub>Beskrivning av bugg</sub>|<sub>Ansvar för att lösa</sub>|
|--------|------------|

### Otestade delar av systemet
* <sub>Fler automatiska tester behöver skrivas för integreringen mot databasen allteftersom den utvecklas.</sub>  
* <sub>Integrationstester saknas, främst relevant för servern i den mån att bristen på integration gör det omöjligt att testa hela emailfunktionaliteten utan att ändra i källkoden.</sub>

### Analys
<sub>Testfallen och testinstruktionerna har uppdaterats för manuella och automatiska testfall på klienten. Automatiska tester har skrivits färdigt för Email-hanteringen på servern. Regressionstester görs och systemet fungerar fortfarande. De delar av systemet som finns känns stabila. Fler manuella tester behöver skrivas för mailhanteringen för att testa att skicka, vidarebefordra och svara på mail allteftersom funktionaliteten utvecklas, men i nuläget är mailhanteringen testad till den nivå som är möjlig med automatiska tester när ingen integration finns mot klienten. Delarna är testade med en hybrid av automatiska och manuella tester som inte gör sig väl i skrift. Fler manuella tester för mailhantering kommer att skrivas när integreringen mot klienten är klar. Det viktigaste att komma igång med nu är att att hålla databastestningen uppdaterad. Snart behöver vi börja skriva end-to-end tester för hela systemet. En del buggar hittades och åtgärdades under veckans testning vad gäller mailhanteringen, men inga större kända buggar löper vidare in i nästa vecka.</sub>
