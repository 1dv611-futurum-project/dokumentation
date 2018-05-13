### Info
<sub>**Datum:** 5/4 -18</sub>  
<sub>**Version av systemet:** [v0.2]()</sub>  
<sub>**Testmiljö:**  Kubuntu 17.10, Chrome 65 x64</sub>  
<sub>**Systemtest:** Eftersom detta är ett test av grundläggande funktionalitet är testfallen en del av flera systemtest: 1, 2, 3 ,4 och 5. Se [här](https://github.com/1dv611-futurum-project/futurum-project/wiki/Testspecifikation).</sub>  

### Testfall och status
<sub>För en beskrivning av testfallen, se [här](https://github.com/1dv611-futurum-project/futurum-project/wiki/Testspecifikation).</sub>    

<sub>Denna testrapport berör:</sub>  

|<sub>Testfall</sub>|<sub>Namn</sub>|<sub>Status</sub>|
|----|--------|------------|
|<sub>T1</sub>|<sub>[Autentisera servern mot mailadressen som ska bevakas - lyckad autentiering](https://github.com/1dv611-futurum-project/futurum-project/wiki/Testspecifikation#testfall-1---autentisera-servern-mot-mailadressen-som-ska-bevakas---lyckad-autentisering)</sub>|<sub><img src="https://upload.wikimedia.org/wikipedia/commons/thumb/5/50/Yes_Check_Circle.svg/2000px-Yes_Check_Circle.svg.png" width="15"></sub>|
|<sub>T2</sub>|<sub>[Autentisera servern mot mailadressen som ska bevakas - misslyckad autentiering](https://github.com/1dv611-futurum-project/futurum-project/wiki/Testspecifikation#testfall-2---autentisera-servern-mot-mailadressen-som-ska-bevakas---misslyckad-autentisering)</sub>|<sub><img src="https://upload.wikimedia.org/wikipedia/commons/thumb/5/50/Yes_Check_Circle.svg/2000px-Yes_Check_Circle.svg.png" width="15"></sub>|
|<sub>T3</sub>|<sub>[Autentisera servern mot mailadressen som ska bevakas - nekad autentiering](https://github.com/1dv611-futurum-project/futurum-project/wiki/Testspecifikation#testfall-3---autentisera-servern-mot-mailadressen-som-ska-bevakas---nekad-autentisering)</sub>|<sub><img src="https://upload.wikimedia.org/wikipedia/commons/thumb/5/50/Yes_Check_Circle.svg/2000px-Yes_Check_Circle.svg.png" width="15"></sub>|

### Otestade delar av systemet
* <sub>Automatiska tester behöver skrivas för IMAPHandler.</sub>  
* <sub>Postman eller manuella tester bör användas för att testa de routes som finns.</sub>  

### Analys
<sub>De delar av systemet som finns känns stabila och passerar de manuella testerna. Implementationen är lite halvfärdig eftersom den inte har integrerats med klienten, och utfallen av testen som testar en medveten "misslyckad" inloggning kan därför inte presentera några vettiga felmeddelanden, utan en koll mot webläsarens adressfält får göras istället. Testfallen kommer behöva uppdateras. Det är svårt att testa delar av systemet på något annat sätt än manuellt eftersom integreringen som finns än så längre är nästan enbart mot externa APIer och verktyg som inte kan mockas i ett test.</sub>