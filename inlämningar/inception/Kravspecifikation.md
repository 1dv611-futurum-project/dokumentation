## Administrationspanel för hantering av support-ärenden via mail

<sub>Systemet erbjuder en administrationspanel för hantering av support-ärenden på webben. Systemet används av de ansvariga för support-ärenden hos Futurum Digital, och fungerar som en prototyp av företagets framtida support-hantering. Det är därför viktigt att systemet är riktat dels mot användaren men också programmeraren.</sub>

<sub>För mer information och status om de olika kraven, **besök de issues som är kopplade till kraven**. För att följa prioriteringen av kraven, kolla in de olika processerna.</sub>

### Specifikationer

#### Tekniska Begränsningar

|<sub>ID</sub>|<sub>Namn</sub>|<sub>Baskrav</sub>|<sub>Beroenden (ID)</sub>|
|----|-----|------------|-----|
|<sub>#1</sub>|<sub>Systemet ska använda Docker</sub>|<sub>--</sub>|<sub>--</sub>|
|<sub>#2</sub>|<sub>Systemet ska använda Node.js</sub>|<sub>nr.1</sub>|<sub>#1</sub>|
|<sub>#3</sub>|<sub>Systemet ska använda MongoDB</sub>|<sub>nr.1</sub>|<sub>#2</sub>|
|<sub>#4</sub>|<sub>Systemet ska använda ReactJS</sub>|<sub>nr.1</sub>|<sub>#2</sub>|
|<sub>#5</sub>|<sub>Systemet ska använda Websockets</sub>|<sub>nr.1</sub>|<sub>#2</sub>|

#### Kvalitetskrav ([Följ processen här](https://github.com/1dv611-futurum-project/futurum-project/projects/5))
|<sub>ID</sub>|<sub>Namn</sub>|<sub>Baskrav</sub>|<sub>Beroenden (ID)</sub>|
|----|-----|------------|-----|
|<sub>#6</sub>|<sub>[Systemet ska följa en utvecklingsprocess](https://github.com/1dv611-futurum-project/futurum-project/projects/3)</sub>|<sub>nr.2</sub>|<sub>--</sub>|
|<sub>#7</sub>|<sub>[Systemet ska vara användarvänligt](https://github.com/1dv611-futurum-project/futurum-project/issues/46)</sub>|<sub>nr.2</sub>|<sub>--</sub>|
|<sub>#8</sub>|<sub>[Systemet ska tillgodose hjälpsamma felmeddelanden](https://github.com/1dv611-futurum-project/futurum-project/issues/151)</sub>|<sub>nr.2</sub>|<sub>--</sub>|
|<sub>#9</sub>|<sub>[Systemet ska vara säkert](https://github.com/1dv611-futurum-project/futurum-project/issues/47)</sub>|<sub>nr.3</sub>|<sub>#13</sub>|
|<sub>#10</sub>|<sub>[Systemet ska följa webbstandarder](https://github.com/1dv611-futurum-project/futurum-project/issues/48)</sub>|<sub>nr.3-5</sub>|<sub>--</sub>|
|<sub>#11</sub>|<sub>[Systemet ska svara på ny data inom en acceptabel tidsram](https://github.com/1dv611-futurum-project/futurum-project/issues/49)</sub>|<sub>nr.2</sub>|<sub>--</sub>|
|<sub>#12</sub>|<sub>[Systemet ska erbjuda relevanta svar vid statusuppdatering](https://github.com/1dv611-futurum-project/futurum-project/issues/50)</sub>|<sub>nr.2</sub>|<sub>--</sub>|

#### Säkerhetskrav ([Följ processen här](https://github.com/1dv611-futurum-project/futurum-project/projects/4))
|<sub>ID</sub>|<sub>Namn</sub>|<sub>Baskrav</sub>|<sub>Beroenden (ID)</sub>|
|----|-----|------------|-----|
|<sub>#13</sub>|<sub>[Systemet ska ha skydd mot Cross-Site Scripting (XSS)](https://github.com/1dv611-futurum-project/futurum-project/issues/51)</sub>|<sub>nr.3-4</sub>|<sub>--</sub>|

#### Funktionella krav ([Följ processen här](https://github.com/1dv611-futurum-project/futurum-project/projects/2))

|<sub>ID</sub>|<sub>Namn</sub>|<sub>Baskrav</sub>|<sub>Beroenden (ID)</sub>|
|----|-----|------------|-----|
|<sub>#14</sub>|<sub>[Användare ska kunna se listade ärenden som inkommit via mail från registrerade mailadresser](https://github.com/1dv611-futurum-project/futurum-project/issues/15) </sub>|<sub>nr.3</sub>|<sub>#25</sub>|
|<sub>#15</sub>|<sub>[Användare ska få in helt nya mail "real-time" som ärenden från registrerade mailadresser](https://github.com/1dv611-futurum-project/futurum-project/issues/20) </sub>|<sub>nr.3</sub>|<sub>#25</sub>|
|<sub>#16</sub>|<sub>[Användare ska kunna ändra status på ärenden](https://github.com/1dv611-futurum-project/futurum-project/issues/17) </sub>|<sub>nr.4</sub>|<sub>#14, #25</sub>|
|<sub>#17</sub>|<sub>[Användare ska kunna se meddelande-historik av ärenden](https://github.com/1dv611-futurum-project/futurum-project/issues/24) </sub>|<sub>nr.2-4</sub>|<sub>#23, #25</sub>|
|<sub>#18</sub>|<sub>[Användare ska kunna lägga till mailadresser till en lista med registrerade mailadresser](https://github.com/1dv611-futurum-project/futurum-project/issues/16) </sub>|<sub>nr.4</sub>|<sub>#24</sub>|
|<sub>#19</sub>|<sub>[Användare ska kunna skicka meddelanden till ärendens avsändare via mail](https://github.com/1dv611-futurum-project/futurum-project/issues/19) </sub>|<sub>nr.4</sub>|<sub>#25</sub>|
|<sub>#20</sub>|<sub>[Användare ska kunna skicka statusuppdateringen till avsändaren](https://github.com/1dv611-futurum-project/futurum-project/issues/18) </sub>|<sub>nr.4</sub>|<sub>#18, #25</sub>|
|<sub>#21</sub>|<sub>[Mail från icke-registrerade avsändare ska vidarebefordras till annan mailadress](https://github.com/1dv611-futurum-project/futurum-project/issues/21) </sub>|<sub>nr.5</sub>|<sub>#18</sub>|
|<sub>#22</sub>|<sub>[Vid oväntade fel ska mail vidarebefordras till annan mailadress](https://github.com/1dv611-futurum-project/futurum-project/issues/22) </sub>|<sub>nr.5</sub>|<sub>--</sub>|
|<sub>#23</sub>|<sub>[Användare ska kunna få upp en vy med detaljerad information om ett ärende](https://github.com/1dv611-futurum-project/futurum-project/issues/148) </sub>|<sub>nr.4</sub>|<sub>#25</sub>|
|<sub>#24</sub>|<sub>[Användare ska kunna tilldela en ansvarig till ett ärende](https://github.com/1dv611-futurum-project/futurum-project/issues/149) </sub>|<sub>nr.4</sub>|<sub>#22, #25</sub>|
|<sub>#25</sub>|<sub>[Användare ska kunna autentisera sig mot Gmail via OAuth](https://github.com/1dv611-futurum-project/futurum-project/issues/150) </sub>|<sub>nr.3-4</sub>|<sub>--</sub>|

#### Användarfall
<sub>För utförligare förklaring av de funktionella kraven, [kolla in användarfallen här](https://github.com/1dv611-futurum-project/dokumentation/blob/master/inlämningar/inception/Anv%C3%A4ndarfall.md)</sub><br>

### Tester
<sub>För en lista över systemtester och testfall som testar kraven, se [Testspecifikationen](https://github.com/1dv611-futurum-project/dokumentation/blob/master/inlämningar/inception/Testspecifikation.md).</sub>
