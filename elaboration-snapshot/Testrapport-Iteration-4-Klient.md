### Info
<sub>**Datum:** 20/4 -18</sub>  
<sub>**Version av systemet:** [v0.3]()</sub>  
<sub>**Testmiljö:**  Kubuntu 17.10</sub>

### Testfall och status
<sub>För en beskrivning av testfallen, se [här](https://github.com/1dv611-futurum-project/futurum-project/wiki/Testspecifikation).</sub>    

<sub>Denna testrapport berör:</sub>  

|<sub>Testfall</sub>|<sub>Namn</sub>|<sub>Status</sub>|
|----|--------|------------|
|<sub>T1.1-3</sub>|<sub>[Testfall 1 - Lägga till ny mailadress](https://github.com/1dv611-futurum-project/futurum-project/wiki/Testspecifikation#testfall-1---l%C3%A4gga-till-ny-mailadress)</sub>|<sub><img src="https://upload.wikimedia.org/wikipedia/commons/thumb/5/50/Yes_Check_Circle.svg/2000px-Yes_Check_Circle.svg.png" width="15"></sub>|
|<sub>T4.1-4</sub>|<sub>[Testfall 4 - Ändra status på ärende - flerkortsvy, uppdatering till kund](https://github.com/1dv611-futurum-project/futurum-project/wiki/Testspecifikation#testfall-4---%C3%84ndra-status-p%C3%A5-%C3%A4rende---flerkortsvy-uppdatering-till-kund)</sub>|<sub><img src="https://upload.wikimedia.org/wikipedia/commons/thumb/5/50/Yes_Check_Circle.svg/2000px-Yes_Check_Circle.svg.png" width="15"></sub>|
|<sub>T5.1-5</sub>|<sub>[Testfall 5 - Ändra status på ärende - enskild kortvy, utan uppdatering till kund](https://github.com/1dv611-futurum-project/futurum-project/wiki/Testspecifikation#testfall-5---%C3%84ndra-status-p%C3%A5-%C3%A4rende---enskild-kortvy-utan-uppdatering-till-kund)</sub>|<sub><img src="https://upload.wikimedia.org/wikipedia/commons/thumb/5/50/Yes_Check_Circle.svg/2000px-Yes_Check_Circle.svg.png" width="15"></sub>|
|<sub>T6.1-4</sub>|<sub>[Testfall 6 - Tilldela ärende](https://github.com/1dv611-futurum-project/futurum-project/wiki/Testspecifikation#testfall-6---tilldela-%C3%A4rende)</sub>|<sub><img src="https://upload.wikimedia.org/wikipedia/commons/thumb/5/50/Yes_Check_Circle.svg/2000px-Yes_Check_Circle.svg.png" width="15"></sub>|
|<sub>T8</sub>|<sub>[Testfall 8 - Svara på ett ärende](https://github.com/1dv611-futurum-project/futurum-project/wiki/Testspecifikation#testfall-8---svara-p%C3%A5-ett-%C3%A4rende)</sub>|<sub><img src="https://upload.wikimedia.org/wikipedia/commons/thumb/5/50/Yes_Check_Circle.svg/2000px-Yes_Check_Circle.svg.png" width="15"></sub>|

### Enhetstester
<sub>**Tekniker:**  Karma, chromium-browser, Mocha, Chai, Enzyme</sub>  
<sub>**Paket:**  Components</sub>

|<sub>Testfall</sub>|<sub>Krav</sub>|<sub>Status</sub>|
|----|--------|------------|
|<sub>[TicketOverview.unit.spec.tsx](https://github.com/1dv611-futurum-project/futurum-project/blob/client/services/client/test/components/TicketOverview/TicketOverview.unit.spec.tsx)</sub>|<sub>#23</sub>|<sub><img src="https://upload.wikimedia.org/wikipedia/commons/thumb/5/50/Yes_Check_Circle.svg/2000px-Yes_Check_Circle.svg.png" width="15"></sub>|
|<sub>[ClientInput.unit.spec.tsx](https://github.com/1dv611-futurum-project/futurum-project/blob/client/services/client/test/components/ClientInput/ClientInput.unit.spec.tsx)</sub>|<sub>#18</sub>|<sub><img src="https://upload.wikimedia.org/wikipedia/commons/thumb/5/50/Yes_Check_Circle.svg/2000px-Yes_Check_Circle.svg.png" width="15"></sub>|
|<sub>[DropDownSelect.unit.spec.tsx](https://github.com/1dv611-futurum-project/futurum-project/blob/client/services/client/test/components/DropDownSelect/DropDownSelect.unit.spec.tsx)</sub>|<sub>#16, #24</sub>|<sub><img src="https://upload.wikimedia.org/wikipedia/commons/thumb/5/50/Yes_Check_Circle.svg/2000px-Yes_Check_Circle.svg.png" width="15"></sub>|
|<sub>[Modal.unit.spec.tsx](https://github.com/1dv611-futurum-project/futurum-project/blob/client/services/client/test/components/Modal/Modal.unit.spec.tsx)</sub>|<sub>#20</sub>|<sub><img src="https://upload.wikimedia.org/wikipedia/commons/thumb/5/50/Yes_Check_Circle.svg/2000px-Yes_Check_Circle.svg.png" width="15"></sub>|
|<sub>[StatusSelect.unit.spec.tsx](https://github.com/1dv611-futurum-project/futurum-project/blob/client/services/client/test/components/StatusSelect/StatusSelect.unit.spec.tsx)</sub>|<sub>#16</sub>|<sub><img src="https://upload.wikimedia.org/wikipedia/commons/thumb/5/50/Yes_Check_Circle.svg/2000px-Yes_Check_Circle.svg.png" width="15"></sub>|

### Otestade delar av systemet
* <sub>Följande testfall: T1.4, T2-3, T4.5, T5.6, T6.5, T7, T9-10</sub> 
* <sub>Enhetstester för StatusColor.tsx, TicketAction.tsx</sub>  
* <sub>Postman eller manuella tester bör användas för att testa APIet.</sub>  

### Analys
<sub>Delar av testfallen har testats och kan inte testas fullt ut förrän integration med servern har implementerats. De delar av systemet som testats med enhetstester är de komponenterna som klienten erhåller. Den funktionalitet som finns på klienten fungerar som förväntat enligt testerna. Nästa steg är att utöka integrationen och kommunikationen mellan klient och server via Websocketen för att kunna testa resterande testfall som berör kundlistan och få fullständig funktionalitet kring tilldelning/statusuppdatering av ärenden.</sub>