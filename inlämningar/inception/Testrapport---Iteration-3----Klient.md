### Info
<sub>**Datum:** 13/4 -18</sub>  
<sub>**Version av systemet:** [v0.3]()</sub>  
<sub>**Testmiljö:**  Kubuntu 17.10</sub>

### Testfall och status
<sub>För en beskrivning av testfallen, se [här](https://github.com/1dv611-futurum-project/dokumentation/blob/master/inlämningar/inception/Testspecifikation).</sub>    

<sub>Denna testrapport berör:</sub>  

|<sub>Testfall</sub>|<sub>Namn</sub>|<sub>Status</sub>|
|----|--------|------------|
|<sub>TSX</sub>|<sub>[--](https://github.com/1dv611-futurum-project/dokumentation/blob/master/inlämningar/inception/Testspecifikation.md)</sub>|<sub><img src="http://4.bp.blogspot.com/-3COrhYW7glE/UkxdoBarJfI/AAAAAAAAAwc/lgigiGxjObc/s1600/x_mark_red_circle.png" width="15"></sub>|

### Enhetstester
<sub>**Tekniker:**  Karma, chromium-browser, Mocha, Chai, Enzyme</sub>  
<sub>**Paket:**  Components</sub>

|<sub>Testfall</sub>|<sub>Krav</sub>|<sub>Status</sub>|
|----|--------|------------|
|<sub>[AddButton.unit.spec.tsx](https://github.com/1dv611-futurum-project/futurum-project/blob/client/services/client/test/components/AddButton/AddButton.unit.spec.tsx)</sub>|<sub>#17 - 18</sub>|<sub><img src="https://upload.wikimedia.org/wikipedia/commons/thumb/5/50/Yes_Check_Circle.svg/2000px-Yes_Check_Circle.svg.png" width="15"></sub>|
|<sub>[ClientList.unit.spec.tsx](https://github.com/1dv611-futurum-project/futurum-project/blob/client/services/client/test/components/ClientList/ClientList.unit.spec.tsx)</sub>|<sub>#17</sub>|<sub><img src="https://upload.wikimedia.org/wikipedia/commons/thumb/5/50/Yes_Check_Circle.svg/2000px-Yes_Check_Circle.svg.png" width="15"></sub>|
|<sub>[Message.unit.spec.tsx](https://github.com/1dv611-futurum-project/futurum-project/blob/client/services/client/test/components/Message/Message.unit.spec.tsx)</sub>|<sub>#18</sub>|<sub><img src="https://upload.wikimedia.org/wikipedia/commons/thumb/5/50/Yes_Check_Circle.svg/2000px-Yes_Check_Circle.svg.png" width="15"></sub>|
|<sub>[MessageInput.unit.spec.tsx](https://github.com/1dv611-futurum-project/futurum-project/blob/client/services/client/test/components/MessageInput/MessageInput.unit.spec.tsx)</sub>|<sub>#18</sub>|<sub><img src="https://upload.wikimedia.org/wikipedia/commons/thumb/5/50/Yes_Check_Circle.svg/2000px-Yes_Check_Circle.svg.png" width="15"></sub>|
|<sub>[TicketOverview.unit.spec.tsx](https://github.com/1dv611-futurum-project/futurum-project/blob/client/services/client/test/components/TicketOverview/TicketOverview.unit.spec.tsx)</sub>|<sub>#13</sub>|<sub><img src="https://upload.wikimedia.org/wikipedia/commons/thumb/5/50/Yes_Check_Circle.svg/2000px-Yes_Check_Circle.svg.png" width="15"></sub>|

### Otestade delar av systemet
* <sub>Testfall 1-5</sub> 
* <sub>Enhetstester för Modal.tsx, TicketsList.tsx</sub>  
* <sub>Postman eller manuella tester bör användas för att testa APIet.</sub>  

### Analys
<sub>Delar av testfallen har testats och kan inte testas fullt ut förrän integration med servern har implementerats. De delar av systemet som testats med enhetstester är de komponenterna som klienten erhåller.</sub>
