### Info
<sub>**Datum:** 13/4 -18</sub>  
<sub>**Version av systemet:** [v0.2](https://github.com/1dv611-futurum-project/futurum-project/releases/tag/0.2)</sub>  
<sub>**Testmiljö:**  Kubuntu 17.10, Chrome 65 x64</sub>  
<sub>**Systemtest:** 1-4 Se [här](https://github.com/1dv611-futurum-project/dokumentation/blob/master/inlämningar/elaboration/Testspecifikation.md).</sub>  

### Manuella testfall och status
<sub>För en beskrivning av testfallen, se [här](https://github.com/1dv611-futurum-project/dokumentation/blob/master/inlämningar/elaboration/Testspecifikation.md).</sub>    

<sub>Denna testrapport berör:</sub>  

|<sub>Testfall</sub>|<sub>Namn</sub>|<sub>Status</sub>|
|----|--------|------------|
|<sub>T1</sub>|<sub>[Autentisera servern mot mailadressen som ska bevakas - lyckad autentiering](https://github.com/1dv611-futurum-project/dokumentation/blob/master/inlämningar/elaboration/Testspecifikation.md)</sub>|<sub><img src="https://upload.wikimedia.org/wikipedia/commons/thumb/5/50/Yes_Check_Circle.svg/2000px-Yes_Check_Circle.svg.png" width="15"></sub>|
|<sub>T2</sub>|<sub>[Autentisera servern mot mailadressen som ska bevakas - misslyckad autentiering](https://github.com/1dv611-futurum-project/dokumentation/blob/master/inlämningar/elaboration/Testspecifikation.md)</sub>|<sub><img src="https://upload.wikimedia.org/wikipedia/commons/thumb/5/50/Yes_Check_Circle.svg/2000px-Yes_Check_Circle.svg.png" width="15"></sub>|
|<sub>T3</sub>|<sub>[Autentisera servern mot mailadressen som ska bevakas - misslyckad autentiering](https://github.com/1dv611-futurum-project/dokumentation/blob/master/inlämningar/elaboration/Testspecifikation.md)</sub>|<sub><img src="https://upload.wikimedia.org/wikipedia/commons/thumb/5/50/Yes_Check_Circle.svg/2000px-Yes_Check_Circle.svg.png" width="15"></sub>|
|<sub>T4</sub>|<sub>[Autentisera servern mot mailadressen som ska bevakas - misslyckad autentiering](https://github.com/1dv611-futurum-project/dokumentation/blob/master/inlämningar/elaboration/Testspecifikation.md)</sub>|<sub><img src="https://upload.wikimedia.org/wikipedia/commons/thumb/5/50/Yes_Check_Circle.svg/2000px-Yes_Check_Circle.svg.png" width="15"></sub>|
|<sub>T5</sub>|<sub>[Autentisera servern mot mailadressen som ska bevakas - misslyckad autentiering](https://github.com/1dv611-futurum-project/dokumentation/blob/master/inlämningar/elaboration/Testspecifikation.md)</sub>|<sub><img src="https://upload.wikimedia.org/wikipedia/commons/thumb/5/50/Yes_Check_Circle.svg/2000px-Yes_Check_Circle.svg.png" width="15"></sub>|
|<sub>T6</sub>|<sub>[Autentisera servern mot mailadressen som ska bevakas - nekad autentiering](https://github.com/1dv611-futurum-project/dokumentation/blob/master/inlämningar/elaboration/Testspecifikation.md)</sub>|<sub><img src="https://upload.wikimedia.org/wikipedia/commons/thumb/5/50/Yes_Check_Circle.svg/2000px-Yes_Check_Circle.svg.png" width="15"></sub>|

### Enhetstester och status
<sub>**Tekniker:** Mocha, Chai </sub>  

<sub>Denna testrapport berör:</sub>  

|<sub>Testfall</sub>|<sub>Krav</sub>|<sub>Status</sub>|
|----|--------|------------|
|<sub>[mongoose-models-test-suite.ts](https://github.com/1dv611-futurum-project/futurum-project/blob/server/services/node/test/db-tests/mongoose-models-test-suite.ts)</sub>|<sub>#3, #15-#17</sub>|<sub><img src="https://upload.wikimedia.org/wikipedia/commons/thumb/5/50/Yes_Check_Circle.svg/2000px-Yes_Check_Circle.svg.png" width="15"></sub>|
|<sub>[db-handler-test-suite.ts](https://github.com/1dv611-futurum-project/futurum-project/blob/server/services/node/test/db-tests/db-handler-test-suite.ts)</sub>|<sub>#3, #15-#17</sub>|<sub><img src="https://upload.wikimedia.org/wikipedia/commons/thumb/5/50/Yes_Check_Circle.svg/2000px-Yes_Check_Circle.svg.png" width="15"></sub>|
|<sub>[db-connection-test-suite.ts](https://github.com/1dv611-futurum-project/futurum-project/blob/server/services/node/test/db-tests/db-connection-test-suite.ts)</sub>|<sub>#3, #15-#17</sub>|<sub><img src="https://upload.wikimedia.org/wikipedia/commons/thumb/5/50/Yes_Check_Circle.svg/2000px-Yes_Check_Circle.svg.png" width="15"></sub>|

### Otestade delar av systemet
* <sub>Automatiska tester behöver skrivas för IMAPHandler.</sub>  
* <sub>Fler automatiska tester behöver skrivas för integreringen mot databasen allteftersom den utvecklas.</sub>  
* <sub>Postman eller manuella tester bör användas för att testa de routes som finns.</sub>  

### Analys
<sub>Autentieringen av servern och autentieringen av användaren sker nu i ett enda steg mot Googles OAuth-tjänst, så testfallen har skrivits om och förtydligats. Automatiska tester har skrivit för databashanteringen på servern, vilket betyder att hela servern utom IMAP-hanteringen nu testas antingen automatiskt eller manuellt. De delar av systemet som finns känns stabila. Det viktigaste att komma igång med nu är integrationstestning mellan servern och klienten, samt automatiska tester för IMAP och rester av mailhanteringen.</sub>
