## Branches
<sub>Sammanställda riktlinjer för användning av branches i projektet.</sub>

* <sub>`master` branchen innehåller endast färdigställd funktionalitet.
* <sub>All utveckling av klienten sker i `client` branchen. All utveckling av servern sker i `server` branchen.</sub>
* <sub>Utveckling av specific funktionalitet eller features bryts ut i egna sub-branches. T.ex. uppsättningen av websocket görs i `server-ws` respektive `client-ws` branchen. Generellt arbetar endast en person åt gången i varje branch. När funktionaliteten anses vara färdigställd mergas den sedan in i `client` eller `server` branchen och testas där med hela servern/klienten för att säkerställa att allting fortfarande fungerar.</sub>
* <sub>När `client` eller `server` branchen anses vara färdigutvecklad för pågående iteration mergas denna in i `master` branchen.</sub>
* <sub>Vid slutet av varje iteration görs en release av `master` branchen och taggas med ett versionsnummer. Versionsnumret ska återspegla nuvarande iteration (iteration 2 -> v0.2). Finns det behov att göra flera releases under samma iteration bygger detta vidare på det ursprungliga versionsnumret (v0.2.1, v0.2.2 osv).</sub>


## Issues
<sub>Sammanställda riktlinjer för användning av issues i projektet.</sub>

* <sub>Nya issues ska kopplas till relevant Milestone och även tilldelas den/de personer som arbetar med issuet.</sub>
* <sub>Ett och samma issue kan sträcka sig över flera iterationer, och taggas då med respektive iterationslabel.</sub>
* <sub>Issues ska taggas med prioritet **High**, **Medium** eller **Low** och hanteras därefter. Varje issue rankas även i prioriteringsordning inom respektive kolumn om de har taggats med samma prioritetsgrad.</sub>
* <sub>Prioritetstaggar för ett issue kan uppdateras löpande, både under och mellan olika iterationer.</sub>
* <sub>När ett issue är avslutat så ska prioritetstaggen tas bort för att göra det enklare att kunna filtrera på till exempel brådskande, ej avslutade issues.</sub>
* <sub>Viktigt när man arbetar med ett issue är att man anger issue-numret i Toggl för att enkelt kunna koppla ihop ärende med arbetad tid.</sub>