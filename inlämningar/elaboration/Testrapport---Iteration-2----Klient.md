### Info
<sub>**Datum:** 5/4 -18</sub>  
<sub>**Version av systemet:** [v0.2](https://github.com/1dv611-futurum-project/futurum-project/releases/tag/0.2)</sub>  
<sub>**Testmiljö:**  Kubuntu 17.10, Chrome 65 x64</sub>

### Testfall och status
<sub>För en beskrivning av testfallen, se [här](https://github.com/1dv611-futurum-project/dokumentation/blob/master/inlämningar/inception/Testspecifikation.md).</sub>    

<sub>Denna testrapport berör:</sub>  

|<sub>Testfall</sub>|<sub>Namn</sub>|<sub>Status</sub>|
|----|--------|------------|
|<sub>T4.1-3</sub>|<sub>[Testfall 4 - Ändra status på ärende - flerkortsvy, uppdatering till kund](https://github.com/1dv611-futurum-project/dokumentation/blob/master/inlämningar/inception/Testspecifikation.md)</sub>|<sub><img src="https://upload.wikimedia.org/wikipedia/commons/thumb/5/50/Yes_Check_Circle.svg/2000px-Yes_Check_Circle.svg.png" width="15"></sub>|
|<sub>T5.1-4</sub>|<sub>[Testfall 5 - Ändra status på ärende - enskild kortvy, utan uppdatering till kund](https://github.com/1dv611-futurum-project/dokumentation/blob/master/inlämningar/inception/Testspecifikation.md)</sub>|<sub><img src="https://upload.wikimedia.org/wikipedia/commons/thumb/5/50/Yes_Check_Circle.svg/2000px-Yes_Check_Circle.svg.png" width="15"></sub>|

### Enhetstester
<sub>**Tekniker:**  Karma, PhantomJS, Mocha, Chai, Enzyme</sub>  
<sub>**Paket:**  Components</sub>

|<sub>Testfall</sub>|<sub>Krav</sub>|<sub>Status</sub>|
|----|--------|------------|
|<sub>[Header.unit.spec.tsx](https://github.com/1dv611-futurum-project/futurum-project/blob/client/services/client/test/components/Header/Header.unit.spec.tsx)</sub>|<sub>#7</sub>|<sub><img src="https://upload.wikimedia.org/wikipedia/commons/thumb/5/50/Yes_Check_Circle.svg/2000px-Yes_Check_Circle.svg.png" width="15"></sub>|
|<sub>[Ticket.unit.spec.tsx](https://github.com/1dv611-futurum-project/futurum-project/tree/client/services/client/test/components/Ticket)</sub>|<sub>#14</sub>|<sub><img src="https://upload.wikimedia.org/wikipedia/commons/thumb/5/50/Yes_Check_Circle.svg/2000px-Yes_Check_Circle.svg.png" width="15"></sub>|
|<sub>[StatusSelect.unit.spec.tsx](https://github.com/1dv611-futurum-project/futurum-project/tree/client/services/client/test/components/StatusSelect)</sub>|<sub>#16</sub>|<sub><img src="https://upload.wikimedia.org/wikipedia/commons/thumb/5/50/Yes_Check_Circle.svg/2000px-Yes_Check_Circle.svg.png" width="15"></sub>|

### Otestade delar av systemet
* <sub>Testfall 1-3 & hela Testfall 4-5</sub>
* <sub>Enhetstester för Addbutton.tsx, ClientList.tsx, Message.tsx, MessageInput.tsx, Modal.tsx, TicketOverview.tsx, TicketsList.tsx</sub>  
* <sub>Postman eller manuella tester bör användas för att testa APIet.</sub>  

### Analys
<sub>Delar av testfallen har testats och kan inte testas fullt ut förrän integration med servern har implementerats. De delar av systemet som testats med enhetstester är de komponenterna som klienten erhåller. Enhetstesterna är till för att skapa en ram och grundstomme för fortsatt utveckling.</sub>
