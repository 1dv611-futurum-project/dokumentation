# Versionshantering
<sub>Projektets kodbas finns i ett repositorie på Github och därigenom sköts även all versionshantering. Dokumentation, backlog och övriga tekniska specifikationer finns tillgängliga i den tillhörande wikin.</sub>

<sub>All utveckling utgår från `master` branchen där även all färdigställd eller levererad funktionalitet ligger. Utöver det här finns en `client` samt `server` branch för utveckling inom respektive område. [Generella riktlinjer för utveckling i branches har sammanställts nedan](https://github.com/1dv611-futurum-project/dokumentation/inlämningar/inception/Arbetsprocessen#branches).</sub>

## Utvecklingssteg
<sub>Följande definierade steg beskriver hur en normal utvecklingsprocess i projektet för ny funktionalitet kan se ut.</sub>

<sub>1. Börja med att dra ner projektet lokalt till din dator. </sub>
```
$ git clone https://github.com/1dv611-futurum-project/futurum-project.git
```
<sub>2. Byt till den branch som du planerar att utveckla i (**client** för klienten, eller **server** för servern), och dra ner de senaste ändringarna.</sub> 
```
$ git checkout [branch]
$ git pull
```
<sub>3. Navigera till roten av mappen i din terminal och starta Docker (för fler användbara Docker-kommandon, se [Readme-filen](https://github.com/1dv611-futurum-project/futurum-project/blob/master/README.md) i master-branchen).</sub>
```
$ docker-compose up -d --build
```
<sub>4. Klienten körs nu på `localhost:8080`, och servern på `localhost:8080/node`. Båda två startas/byggs automatiskt om vid ändringar i källkoden.</sub>  
<sub>5. Skapa en ny, separat branch för den funktionalitet som du planerar att utveckla.</sub>
```
$ git checkout -b [branchName]
```
<sub>6. Lägg till och committa dina ändringar i branchen.</sub>
```
$ git add . && git commit -m "Commit message"
```
<sub>7. Pusha upp ändringarna i den branch du precis skapat.</sub>
```
$ git push origin [branchName]
```
<sub>8. När funktionaliteten i sub-branchen är färdigutvecklad, gör en merge mellan sub-branchen och `server` eller `client`, beroende på om det är server eller client funktionalitet.</sub>
```
$ git checkout [server/client] && git merge [branchname]
```
<sub>9. Inför leverande och/eller release sammanställs all färdig funktionalitet från server och client-brancherna i master-branchen med hjälp av en merge eller en pull-request direkt på Github.</sub>
```
$ git checkout master && git merge [server/client]
```

## Projekthantering med issues
<sub>För att hantera krav från backloggen och de olika iterationerna under projektets gång används [Projects](https://github.com/1dv611-futurum-project/futurum-project/projects) och [Issues](https://github.com/1dv611-futurum-project/futurum-project/issues) på Github. De fyra första projekten hanterar de olika typerna av krav som har definierats i [kravspecifikationen](https://github.com/1dv611-futurum-project/dokumentation/inlämningar/inception/Kravspecifikation). Det femte projektet hanterar istället uppgifter för de olika iterationerna. [Generella riktlinjer för användning av issues har sammanställts nedan](https://github.com/1dv611-futurum-project/dokumentation/inlämningar/inception//Arbetsprocessen#issues).</sub>

<sub>En normal arbetsprocess för att skapa ett nytt issue kan se ut som följande:</sub>

<sub>1. Skapa ett nytt issue (`New issue`).</sub>  
<sub>2. Sätt en lämplig rubrik, kategoriserad under antingen Dokumentation, Applikation, Kundhantering eller Handledning (ex. `Dokumentation - Färdigställ projektplan`).</sub>  
<sub>3. Tilldela issuet till personen/personerna det berör.</sub>  
<sub>4. Lägg till korrekt Milestone och projekt för issuet (Iterationshantering).</sub>  
<sub>5. Tagga issuet med relevanta taggar för iterationsnummer och prioritering.</sub>  
<sub>6. Gå över till [Iterationshanteringen](https://github.com/1dv611-futurum-project/futurum-project/projects/1). Det nya issuet kommer nu att ligga i `To Do`-kolumnen längst till vänster. När korrekt iteration behandlas, dra över issuet till kolumnen `Selected for iteration`. När kortet är under utveckling/hanteras, dra istället över det till kolumnen `In progress`.</sub>  
<sub>7. När ett issue är färdigt, stäng issuet så det automatiskt förflyttas till kolumnen `Done`.</sub>


# Riktlinjer

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
