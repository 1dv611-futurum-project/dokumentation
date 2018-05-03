## Administrationspanel för hantering av supportärenden via mail

<sub>Systemet erbjuder en administrationspanel för hantering av supportärenden på webben. Systemet används av de ansvariga för supportärenden hos Futurum Digital, och fungerar som en prototyp av företagets framtida supporthantering. Det är därför viktigt att systemet är riktat dels mot användaren men också programmeraren.</sub>

<sub>Varje krav är länkat till ett issue som hanteras löpande under utvecklingsprocessen. Det går att följa status för ett krav både genom tabellen nedan och issuet i realtid. Alla krav prioriteras med nivån Hög, Mellan eller Låg (taggarna för issues använder motsvarande High, Medium, Low). Prioriteringen mellan krav som har samma prioritetsnivå framgår tydligare i visningen av issues då varje kolumn sorteras i prioritetsordning.</sub>

<sub>_Krav märkta med * innehåller mer information i sitt specifika issue. Det här kan vara en kort beskrivning eller punkter för att göra kravet mätbart (gäller kvalitetskraven)._</sub>

### Specifikationer

#### Tekniska Begränsningar

|<sub>ID</sub>|<sub>Namn</sub>|<sub>Baskrav</sub>|<sub>Beroenden (ID)</sub>|<sub>Prioritet</sub>|<sub>Status</sub>|
|----|-----|------------|-----|-----|-----|
|<sub>#1</sub>|<sub>Systemet ska använda Docker</sub>|<sub>--</sub>|<sub>--</sub>|<sub>Hög</sub>|<sub>Implementerat</sub>|
|<sub>#2</sub>|<sub>Systemet ska använda NodeJS</sub>|<sub>nr.1</sub>|<sub>#1</sub>|<sub>Hög</sub>|<sub>Implementerat</sub>|
|<sub>#3</sub>|<sub>Systemet ska använda MongoDB</sub>|<sub>nr.1</sub>|<sub>#2</sub>|<sub>Hög</sub>|<sub>Implementerat</sub>|
|<sub>#4</sub>|<sub>Systemet ska använda ReactJS</sub>|<sub>nr.1</sub>|<sub>#2</sub>|<sub>Hög</sub>|<sub>Implementerat</sub>|
|<sub>#5</sub>|<sub>Systemet ska använda Websockets</sub>|<sub>nr.1</sub>|<sub>#2</sub>|<sub>Hög</sub>|<sub>Implementerat</sub>|

#### Kvalitetskrav ([Följ processen här](https://github.com/1dv611-futurum-project/futurum-project/projects/5))
|<sub>ID</sub>|<sub>Namn</sub>|<sub>Baskrav</sub>|<sub>Beroenden (ID)</sub>|<sub>Prioritet</sub>|<sub>Status</sub>|
|----|-----|------------|-----|-----|-----|
|<sub>#6</sub>|<sub>[Systemet ska följa en utvecklingsprocess](https://github.com/1dv611-futurum-project/futurum-project/projects/3) (separat process med issues)</sub>|<sub>nr.2</sub>|<sub>--</sub>|<sub>Hög</sub>|<sub>Pågående</sub>|
|<sub>#7</sub>|<sub>[Systemet ska vara användarvänligt*](https://github.com/1dv611-futurum-project/futurum-project/issues/46)</sub>|<sub>nr.2</sub>|<sub>--</sub>|<sub>Hög</sub>|<sub>Pågående</sub>|
|<sub>#8</sub>|<sub>[Systemet ska tillgodose hjälpsamma felmeddelanden*](https://github.com/1dv611-futurum-project/futurum-project/issues/151)</sub>|<sub>nr.2</sub>|<sub>--</sub>|<sub>Låg</sub>|<sub>Pågående</sub>|
|<sub>#9</sub>|<sub>[Systemet ska vara säkert*](https://github.com/1dv611-futurum-project/futurum-project/issues/47)</sub>|<sub>nr.3</sub>|<sub>#13</sub>|<sub>Låg</sub>|<sub>Pågående</sub>|
|<sub>#10</sub>|<sub>[Systemet ska följa webbstandarder*](https://github.com/1dv611-futurum-project/futurum-project/issues/48)</sub>|<sub>nr.3-5</sub>|<sub>--</sub>|<sub>Mellan</sub>|<sub>Pågående</sub>|
|<sub>#11</sub>|<sub>[Systemet ska svara på ny data inom en acceptabel tidsram*](https://github.com/1dv611-futurum-project/futurum-project/issues/49)</sub>|<sub>nr.2</sub>|<sub>--</sub>|<sub>Mellan</sub>|<sub>Ej påbörjat</sub>|
|<sub>#12</sub>|<sub>[Systemet ska erbjuda relevanta svar vid statusuppdatering*](https://github.com/1dv611-futurum-project/futurum-project/issues/50)</sub>|<sub>nr.2</sub>|<sub>--</sub>|<sub>Mellan</sub>|<sub>Pågående</sub>|

#### Säkerhetskrav ([Följ processen här](https://github.com/1dv611-futurum-project/futurum-project/projects/4))
|<sub>ID</sub>|<sub>Namn</sub>|<sub>Baskrav</sub>|<sub>Beroenden (ID)</sub>|<sub>Prioritet</sub>|<sub>Status</sub>|
|----|-----|------------|-----|-----|-----|
|<sub>#13</sub>|<sub>[Systemet ska ha skydd mot Cross-Site Scripting (XSS)*](https://github.com/1dv611-futurum-project/futurum-project/issues/51)</sub>|<sub>nr.3-4</sub>|<sub>--</sub>|<sub>Mellan</sub>|<sub>Pågående</sub>|

#### Funktionella krav ([Följ processen här](https://github.com/1dv611-futurum-project/futurum-project/projects/2))

|<sub>ID</sub>|<sub>Namn</sub>|<sub>Baskrav</sub>|<sub>Beroenden (ID)</sub>|<sub>Prioritet</sub>|<sub>Status</sub>|
|----|-----|------------|-----|-----|-----|
|<sub>#14</sub>|<sub>[Användare ska kunna se listade ärenden som inkommit via mail från registrerade mailadresser](https://github.com/1dv611-futurum-project/futurum-project/issues/15) </sub>|<sub>nr.3</sub>|<sub>#25</sub>|<sub>Hög</sub>|<sub>Pågående</sub>|
|<sub>#15</sub>|<sub>[Användare ska få in helt nya mail "real-time" som ärenden från registrerade mailadresser](https://github.com/1dv611-futurum-project/futurum-project/issues/20) </sub>|<sub>nr.3</sub>|<sub>#25</sub>|<sub>Hög</sub>|<sub>Implementerat</sub>|
|<sub>#16</sub>|<sub>[Användare ska kunna ändra status på ärenden*](https://github.com/1dv611-futurum-project/futurum-project/issues/17) </sub>|<sub>nr.4</sub>|<sub>#14, #25</sub>|<sub>Hög</sub>|<sub>Implementerat</sub>|
|<sub>#17</sub>|<sub>[Användare ska kunna se meddelande-historik av ärenden](https://github.com/1dv611-futurum-project/futurum-project/issues/24) </sub>|<sub>nr.2-4</sub>|<sub>#23, #25</sub>|<sub>Mellan</sub>|<sub>Pågående</sub>|
|<sub>#18</sub>|<sub>[Användare ska kunna lägga till mailadresser till en lista med registrerade mailadresser](https://github.com/1dv611-futurum-project/futurum-project/issues/16) </sub>|<sub>nr.4</sub>|<sub>#24</sub>|<sub>Hög</sub>|<sub>Pågående</sub>|
|<sub>#19</sub>|<sub>[Användare ska kunna skicka meddelanden till ärendens avsändare via mail](https://github.com/1dv611-futurum-project/futurum-project/issues/19) </sub>|<sub>nr.4</sub>|<sub>#25</sub>|<sub>Hög</sub>|<sub>Pågående</sub>|
|<sub>#20</sub>|<sub>[Användare ska kunna skicka statusuppdateringen till avsändaren](https://github.com/1dv611-futurum-project/futurum-project/issues/18) </sub>|<sub>nr.4</sub>|<sub>#18, #25</sub>|<sub>Mellan</sub>|<sub>Pågående</sub>|
|<sub>#21</sub>|<sub>[Mail från icke-registrerade avsändare ska vidarebefordras till annan mailadress*](https://github.com/1dv611-futurum-project/futurum-project/issues/21) </sub>|<sub>nr.5</sub>|<sub>#18</sub>|<sub>Hög</sub>|<sub>Ej påbörjat</sub>|
|<sub>#22</sub>|<sub>[Vid oväntade fel ska mail vidarebefordras till annan mailadress](https://github.com/1dv611-futurum-project/futurum-project/issues/22) </sub>|<sub>nr.5</sub>|<sub>--</sub>|<sub>Hög</sub>|<sub>Pågående</sub>|
|<sub>#23</sub>|<sub>[Användare ska kunna få upp en vy med detaljerad information om ett ärende*](https://github.com/1dv611-futurum-project/futurum-project/issues/148) </sub>|<sub>nr.4</sub>|<sub>#25</sub>|<sub>Mellan</sub>|<sub>Implementerat</sub>|
|<sub>#24</sub>|<sub>[Användare ska kunna tilldela en ansvarig till ett ärende](https://github.com/1dv611-futurum-project/futurum-project/issues/149) </sub>|<sub>nr.4</sub>|<sub>#22, #25</sub>|<sub>Mellan</sub>|<sub>Pågående</sub>|
|<sub>#25</sub>|<sub>[Användare ska kunna autentisera sig mot Gmail via OAuth*](https://github.com/1dv611-futurum-project/futurum-project/issues/150) </sub>|<sub>nr.3-4</sub>|<sub>--</sub>|<sub>Hög</sub>|<sub>Implementerat</sub>|

#### Användarfall
<sub>För en utförligare förklaring av de funktionella kraven, [läs mer i användarfallen](https://github.com/1dv611-futurum-project/dokumentation/blob/master/inlämningar/elaboration/Användarfall.md).</sub><br>

### Tester
<sub>För en lista över systemtester och testfall som testar kraven, se [Testspecifikationen](https://github.com/1dv611-futurum-project/dokumentation/blob/master/inlämningar/elaboration/Testspecifikation.md).</sub>
