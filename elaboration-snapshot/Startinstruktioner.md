## Översikt
<sub>Följande behövs för att kunna köra applikationen lokalt:</sub>
* <sub>Ett projekt hos Google.</sub>
* <sub>En .env fil med korrekta variabler inlagda.</sub>
* <sub>Docker installerat.</sub>
* <sub>En nedklonad kopia av projektet.</sub>

<sub>För att starta upp projektet, gör följande:</sub>
* <sub>Klona ned [projektet](https://github.com/1dv611-futurum-project/futurum-project) från `master` med kommandot `git clone https://github.com/1dv611-futurum-project/futurum-project`.</sub>
* <sub>[Sätt upp ett projekt hos google](https://github.com/1dv611-futurum-project/futurum-project/wiki/Startinstruktioner#s%C3%A4tt-upp-ett-projekt-hos-google).</sub>
* <sub>[Initiera .env-filen](https://github.com/1dv611-futurum-project/futurum-project/wiki/Startinstruktioner#initiera--env-filen) och placera den i foldern `/services/node`, bredvid `package.json`.</sub>
* <sub>[Installera Docker](https://github.com/1dv611-futurum-project/futurum-project/blob/master/README.md).</sub>
* <sub>[Starta](https://github.com/1dv611-futurum-project/futurum-project/blob/master/README.md) projektet med `docker-compose`, stående i projektets rot-folder.</sub>

## För utveckling
<sub>För att komma igång med utveckling av applikationen, följ instruktionerna för uppstart av projektet enligt ovan. Öppna källkoden i valfri utvecklingsmiljö. Följ sedan processen som beskriven under [arbetsprocessen](https://github.com/1dv611-futurum-project/futurum-project/wiki/Arbetsprocessen), samt använd dig av relevanta [docker-kommandon](https://github.com/1dv611-futurum-project/futurum-project). För utveckling på klienten kan det vara värt att notera att startkommandot i Dockerfilen på client-branchen är anpassat för utveckling, och startar applikationen från `react-dev-server` med hot-reload aktiverat.</sub>

## Sätt upp ett projekt hos Google
<sub> Logga först in på valfritt Google-konto och navigera till [Google Cloud Platform (https://console.cloud.google.com/). Följ sedan följande instruktioner: </sub>

<sub> 1. Acceptera Terms of Service:</sub>

[![TermsOfService](https://github.com/1dv611-futurum-project/futurum-project/wiki/images/tos.jpg)](https://github.com/1dv611-futurum-project/futurum-project/wiki/images/tos.jpg)

<sub> 2. Välj "Select a project":</sub>

[![Projekt1](https://github.com/1dv611-futurum-project/futurum-project/wiki/images/proj1.jpg)](https://github.com/1dv611-futurum-project/futurum-project/wiki/images/proj1.jpg)

<sub> 3. Tryck på plusset för att skapa ett nytt projekt:</sub>

[![Projekt2](https://github.com/1dv611-futurum-project/futurum-project/wiki/images/proj2.jpg)](https://github.com/1dv611-futurum-project/futurum-project/wiki/images/proj2.jpg)

<sub> 4. Dör projektet till varlfritt namn och välj "Create":</sub>

[![Projekt3](https://github.com/1dv611-futurum-project/futurum-project/wiki/images/proj3.jpg)](https://github.com/1dv611-futurum-project/futurum-project/wiki/images/proj3.jpg)

<sub>Aktivera Google+ och Gmail APIerna genom att gå till projektets Dashboard, välja 'Enable APIs and Services', söka upp Gmail och Google+ och aktivera dem:</sub>

<sub>5. Gå till projektets Dashboard:</sub>

[![API1](https://github.com/1dv611-futurum-project/futurum-project/wiki/images/api1.jpg)](https://github.com/1dv611-futurum-project/futurum-project/wiki/images/api1.jpg)

<sub> 6. Välj ditt projekt:</sub>

[![API2](https://github.com/1dv611-futurum-project/futurum-project/wiki/images/api2.jpg)](https://github.com/1dv611-futurum-project/futurum-project/wiki/images/api2.jpg)

<sub> 7. Välj 'Enable APIs and Services':</sub>

[![API3](https://github.com/1dv611-futurum-project/futurum-project/wiki/images/api3.jpg)](https://github.com/1dv611-futurum-project/futurum-project/wiki/images/api3.jpg)

<sub> 8. Sök upp Gmail och välj "Enable" för att aktivera:</sub>

[![API4](https://github.com/1dv611-futurum-project/futurum-project/wiki/images/api4.jpg)](https://github.com/1dv611-futurum-project/futurum-project/wiki/images/api4.jpg)

<sub> 9. Upprepa steg 8 för att aktivera även Google+.</sub>

<sub> 10. Tryck på nyckeln för att skapa credentials för projektet och välj "Create credentials":</sub>

[![Cred1](https://github.com/1dv611-futurum-project/futurum-project/wiki/images/cred1.jpg)](https://github.com/1dv611-futurum-project/futurum-project/wiki/images/cred1.jpg)

<sub> 11. Välj "Help me choose":</sub>

[![Cred2](https://github.com/1dv611-futurum-project/futurum-project/wiki/images/cred2.jpg)](https://github.com/1dv611-futurum-project/futurum-project/wiki/images/cred2.jpg)

<sub> 12. Fyll i alternativ som nedan och välj "What credentials do I need?":</sub>

[![Cred3](https://github.com/1dv611-futurum-project/futurum-project/wiki/images/cred3.jpg)](https://github.com/1dv611-futurum-project/futurum-project/wiki/images/cred3.jpg)

<sub>13. Fyll i `http://127.0.0.1:8080/node/auth/google/callback` som Authorized redirect URIs och välj Create ClientID:</sub>

[![Cred4](https://github.com/1dv611-futurum-project/futurum-project/wiki/images/cred4.jpg)](https://github.com/1dv611-futurum-project/futurum-project/wiki/images/cred4.jpg)

<sub>14. Fyll i valfri mailadress och namn här:</sub>

[![Cred5](https://github.com/1dv611-futurum-project/futurum-project/wiki/images/cred5.jpg)](https://github.com/1dv611-futurum-project/futurum-project/wiki/images/cred5.jpg)

<sub>15. Välj "I'll do this later" på frågan om du vill ladda ner credentials:</sub>

[![Cred6](https://github.com/1dv611-futurum-project/futurum-project/wiki/images/cred6.jpg)](https://github.com/1dv611-futurum-project/futurum-project/wiki/images/cred6.jpg)

<sub>16. Välj istället namnet på dina credentials:</sub>

[![Cred7](https://github.com/1dv611-futurum-project/futurum-project/wiki/images/cred7.jpg)](https://github.com/1dv611-futurum-project/futurum-project/wiki/images/cred7.jpg)

<sub>17. Och notera "Client ID" och "Client secret" härifrån:</sub>

[![Cred8](https://github.com/1dv611-futurum-project/futurum-project/wiki/images/cred8.jpg)](https://github.com/1dv611-futurum-project/futurum-project/wiki/images/cred8.jpg)

## Initiera .env-filen
* <sub>Gå till mappen `/services/node` i projektet.</sub>
* <sub>Skapa en fil som heter `.env` (notera punkten).</sub>
* <sub>Spara filen med följande variabler inlagda:</sub>
```
IMAP_USER=[Den mailadress du vill koppla upp applikationen mot för att ta emot mail.]
IMAP_FORWARDING_ADDRESS=[Den mailaddress du vill ha mail vidarebefodrade till, när sådan funktionalitet är påkallad.]
IMAP_REDIRECT_URL=http://127.0.0.1:8080/node/auth/google/callback
IMAP_CLIENT_ID=[Ditt noterade Client ID från Google-projektet ovan.]
IMAP_CLIENT_SECRET=[Din noterade Client secret från Google-projektet ovan.]

```