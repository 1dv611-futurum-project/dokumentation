### Info
<sub>**Datum:** 27/4 -18</sub>  
<sub>**Version av systemet:** [v0.5]()</sub>  
<sub>**Testmiljö:**  Kubuntu 17.10</sub>

### Testfall och status
<sub>För en beskrivning av testfallen, se [här](https://github.com/1dv611-futurum-project/dokumentation/blob/master/inlämningar/inception/Testspecifikation.md).</sub>    

<sub>Denna testrapport berör:</sub>  

#### Regressionstest

|<sub>Testfall</sub>|<sub>Namn</sub>|<sub>Status</sub>|
|----|--------|------------|
|<sub>T1</sub>|<sub>[Testfall 1 - Lägga till ny mailadress](https://github.com/1dv611-futurum-project/dokumentation/blob/master/inlämningar/inception/Testspecifikation.md)</sub>|<sub><img src="https://upload.wikimedia.org/wikipedia/commons/thumb/5/50/Yes_Check_Circle.svg/2000px-Yes_Check_Circle.svg.png" width="15"></sub>|
|<sub>T4</sub>|<sub>[Testfall 4 - Ändra status på ärende - flerkortsvy, uppdatering till kund](https://github.com/1dv611-futurum-project/dokumentation/blob/master/inlämningar/inception/Testspecifikation.md)</sub>|<sub><img src="https://upload.wikimedia.org/wikipedia/commons/thumb/5/50/Yes_Check_Circle.svg/2000px-Yes_Check_Circle.svg.png" width="15"></sub>|
|<sub>T5</sub>|<sub>[Testfall 5 - Ändra status på ärende - enskild kortvy, utan uppdatering till kund](https://github.com/1dv611-futurum-project/dokumentation/blob/master/inlämningar/inception/Testspecifikation.md)</sub>|<sub><img src="https://upload.wikimedia.org/wikipedia/commons/thumb/5/50/Yes_Check_Circle.svg/2000px-Yes_Check_Circle.svg.png" width="15"></sub>|
|<sub>T6</sub>|<sub>[Testfall 6 - Tilldela ärende](https://github.com/1dv611-futurum-project/dokumentation/blob/master/inlämningar/inception/Testspecifikation.md)</sub>|<sub><img src="https://upload.wikimedia.org/wikipedia/commons/thumb/5/50/Yes_Check_Circle.svg/2000px-Yes_Check_Circle.svg.png" width="15"></sub>|
|<sub>T8</sub>|<sub>[Testfall 8 - Svara på ett ärende](https://github.com/1dv611-futurum-project/dokumentation/blob/master/inlämningar/inception/Testspecifikation.md)</sub>|<sub><img src="https://upload.wikimedia.org/wikipedia/commons/thumb/5/50/Yes_Check_Circle.svg/2000px-Yes_Check_Circle.svg.png" width="15"></sub>|

#### Nya test
|<sub>Testfall</sub>|<sub>Namn</sub>|<sub>Status</sub>|
|----|--------|------------|
|<sub>T2</sub>|<sub>[Testfall 2 - Lägga till ny mailadress - felaktig input](https://github.com/1dv611-futurum-project/dokumentation/blob/master/inlämningar/inception/Testspecifikation.md)</sub>|<sub><img src="https://upload.wikimedia.org/wikipedia/commons/thumb/5/50/Yes_Check_Circle.svg/2000px-Yes_Check_Circle.svg.png" width="15"></sub>|

### Enhetstester
<sub>**Tekniker:**  Karma, chromium-browser, Mocha, Chai, Enzyme</sub>  
<sub>**Paket:**  Components</sub>

#### Regressionstest

|<sub>Testfall</sub>|<sub>Krav</sub>|<sub>Status</sub>|
|----|--------|------------|
|<sub>[Header.unit.spec.tsx](https://github.com/1dv611-futurum-project/futurum-project/blob/client/services/client/test/components/Header/Header.unit.spec.tsx)</sub>|<sub>#7</sub>|<sub><img src="https://upload.wikimedia.org/wikipedia/commons/thumb/5/50/Yes_Check_Circle.svg/2000px-Yes_Check_Circle.svg.png" width="15"></sub>|
|<sub>[Ticket.unit.spec.tsx](https://github.com/1dv611-futurum-project/futurum-project/tree/client/services/client/test/components/Ticket)</sub>|<sub>#14</sub>|<sub><img src="https://upload.wikimedia.org/wikipedia/commons/thumb/5/50/Yes_Check_Circle.svg/2000px-Yes_Check_Circle.svg.png" width="15"></sub>|
|<sub>[AddButton.unit.spec.tsx](https://github.com/1dv611-futurum-project/futurum-project/blob/client/services/client/test/components/AddButton/AddButton.unit.spec.tsx)</sub>|<sub>#18 - 19</sub>|<sub><img src="https://upload.wikimedia.org/wikipedia/commons/thumb/5/50/Yes_Check_Circle.svg/2000px-Yes_Check_Circle.svg.png" width="15"></sub>|
|<sub>[ClientList.unit.spec.tsx](https://github.com/1dv611-futurum-project/futurum-project/blob/client/services/client/test/components/ClientList/ClientList.unit.spec.tsx)</sub>|<sub>#18</sub>|<sub><img src="https://upload.wikimedia.org/wikipedia/commons/thumb/5/50/Yes_Check_Circle.svg/2000px-Yes_Check_Circle.svg.png" width="15"></sub>|
|<sub>[Message.unit.spec.tsx](https://github.com/1dv611-futurum-project/futurum-project/blob/client/services/client/test/components/Message/Message.unit.spec.tsx)</sub>|<sub>#19</sub>|<sub><img src="https://upload.wikimedia.org/wikipedia/commons/thumb/5/50/Yes_Check_Circle.svg/2000px-Yes_Check_Circle.svg.png" width="15"></sub>|
|<sub>[MessageInput.unit.spec.tsx](https://github.com/1dv611-futurum-project/futurum-project/blob/client/services/client/test/components/MessageInput/MessageInput.unit.spec.tsx)</sub>|<sub>#19</sub>|<sub><img src="https://upload.wikimedia.org/wikipedia/commons/thumb/5/50/Yes_Check_Circle.svg/2000px-Yes_Check_Circle.svg.png" width="15"></sub>|
|<sub>[TicketOverview.unit.spec.tsx](https://github.com/1dv611-futurum-project/futurum-project/blob/client/services/client/test/components/TicketOverview/TicketOverview.unit.spec.tsx)</sub>|<sub>#23</sub>|<sub><img src="https://upload.wikimedia.org/wikipedia/commons/thumb/5/50/Yes_Check_Circle.svg/2000px-Yes_Check_Circle.svg.png" width="15"></sub>|
|<sub>[ClientInput.unit.spec.tsx](https://github.com/1dv611-futurum-project/futurum-project/blob/client/services/client/test/components/ClientInput/ClientInput.unit.spec.tsx)</sub>|<sub>#18</sub>|<sub><img src="https://upload.wikimedia.org/wikipedia/commons/thumb/5/50/Yes_Check_Circle.svg/2000px-Yes_Check_Circle.svg.png" width="15"></sub>|
|<sub>[DropDownSelect.unit.spec.tsx](https://github.com/1dv611-futurum-project/futurum-project/blob/client/services/client/test/components/DropDownSelect/DropDownSelect.unit.spec.tsx)</sub>|<sub>#16, #24</sub>|<sub><img src="https://upload.wikimedia.org/wikipedia/commons/thumb/5/50/Yes_Check_Circle.svg/2000px-Yes_Check_Circle.svg.png" width="15"></sub>|
|<sub>[Modal.unit.spec.tsx](https://github.com/1dv611-futurum-project/futurum-project/blob/client/services/client/test/components/Modal/Modal.unit.spec.tsx)</sub>|<sub>#20</sub>|<sub><img src="https://upload.wikimedia.org/wikipedia/commons/thumb/5/50/Yes_Check_Circle.svg/2000px-Yes_Check_Circle.svg.png" width="15"></sub>|
|<sub>[StatusSelect.unit.spec.tsx](https://github.com/1dv611-futurum-project/futurum-project/blob/client/services/client/test/components/StatusSelect/StatusSelect.unit.spec.tsx)</sub>|<sub>#16</sub>|<sub><img src="https://upload.wikimedia.org/wikipedia/commons/thumb/5/50/Yes_Check_Circle.svg/2000px-Yes_Check_Circle.svg.png" width="15"></sub>|

#### Nya test
|<sub>Testfall</sub>|<sub>Namn</sub>|<sub>Status</sub>|
|----|--------|------------|
|<sub>[SnackbarNotice.unit.spec.tsx](https://github.com/1dv611-futurum-project/futurum-project/blob/client/services/client/test/components/SnackbarNotice/SnackbarNotice.unit.spec.tsx)</sub>|<sub>#16</sub>|<sub><img src="http://4.bp.blogspot.com/-3COrhYW7glE/UkxdoBarJfI/AAAAAAAAAwc/lgigiGxjObc/s1600/x_mark_red_circle.png" width="15"></sub>|

### Status på buggar
#### Funna genom planerad testning
|<sub>Testfall</sub>|<sub>Beskrivning av bugg</sub>|<sub>Löst</sub>|
|----|--------|------------|

#### Funna genom explorativ manuell testning
|<sub>Beskrivning av bugg</sub>|<sub>Löst</sub>|
|--------|------------|
|<sub>[När man har skickat ett meddelande i ärendevyn och ändrar tilldelad](https://github.com/1dv611-futurum-project/futurum-project/issues/182)</sub>|<sub><img src="http://4.bp.blogspot.com/-3COrhYW7glE/UkxdoBarJfI/AAAAAAAAAwc/lgigiGxjObc/s1600/x_mark_red_circle.png" width="15"></sub>|

#### Kända buggar som går vidare in i nästa iteration
|<sub>Beskrivning av bugg</sub>|<sub>Ansvar för att lösa</sub>|
|--------|------------|
|<sub>[När man har skickat ett meddelande i ärendevyn och ändrar tilldelad](https://github.com/1dv611-futurum-project/futurum-project/issues/182)</sub>|<sub>Miranda + Jesper</sub>|

### Otestade delar av systemet
* <sub>Följande testfall: T3, T7, T9-10</sub>
* <sub>Enhetstester för StatusColor.tsx, TicketAction.tsx</sub>  
* <sub>Postman eller manuella tester bör användas för att testa APIet.</sub>  

### Analys
<sub>Delar av testfallen har testats och kan inte testas fullt ut förrän integration med servern har implementerats. De delar av systemet som testats med enhetstester är de komponenterna som klienten erhåller. Under den här iterationen var det några av regressionstesterna som tidigare gått igenom som inte längre gjorde det. Det här var till följd av den omfattande omskrivning av kod som har skedde i samband med implementeringen av Websocket på klienten, vilket gjorde att vissa props inte längre överensstämde med tidigare uppsättning som beskrevs i testerna. Med andra ord fungerade komponenterna fortfarande som de skulle men hade ändrat grundstruktur, vilket även testerna behövde uppdateras till att efterfölja. Det nya enhetstestet för SnackbarNotice har inte till fullo implementerats ännu och går därför inte igenom. Det här beräknas dock åtgärdas under nästkommande iteration.</sub>

<sub>Tack vare den explorativa manuella testningen upptäcktes även en annan bugg på klienten som har dokumenterats och satts upp som ett issue för att kunna behandlas under någon av de tre kommande iterationerna.</sub>
