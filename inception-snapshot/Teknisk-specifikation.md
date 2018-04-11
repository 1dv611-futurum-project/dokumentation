## Produktion
* NGIN-X, localhost
* Automatisk omstart?

## Språk

## Design

## Övergripande arkitektur

## Noteringar

Nodeserver som lyssnar på inkommande mail till support@futurum.digital. Vid nytt mail ska detta kollas mot en “white list”, som innehåller godkända e-postadresser. <br>

Om adressen är i white list ska servern lagra mailets innehåll, subject och avsändare i MongoDB, samt passa det vidare ner till en React-app via WebSockets.

Om adressen INTE är i whitelist ska mailet istället vidarebefordras till hi@futurum.digital.

Om ett meddelande av någon som helst orsak INTE sparas i MongoDB eller INTE kan skickas via WebSocket, ska ett meddelande gå till hi@futurum.digital med innehållet i det inskickade mailet.

Det är fritt fram att välja vilken miljö, t ex TypeScript eller ES7 osv som körs på servern. Det som önskas är tydliga designmönster och kod som ser likadan ut oavsett vem som skrivit. Här är linters till er hjälp.

Tänk noga igenom hur ni ska hantera WebSockets, och skapa en struktur för detta. Väldigt lätt att den blir en hemsk soppa annars. Tänk också på vad som ska hända vid uppkoppling, nedkoppling, saker som går snett osv (men bygg agilt - ni kommer stöta på saker förr eller senare ändå så planera inte tills ni blir gråhåriga). Vill ni inte använda rena WebSockets kan ni använda libs, så länge de är kompatibla med React. Vi har upplevt att bygga en egen liten abstraktion över native WebSocket ofta är lättare än att använda t ex Socket.io då den abstraherar bort väldigt mycket. Kravet för detta projekt är endast senaste Chrome som target.

Använd gärna väl etablerade npm packages för att ni ska slippa återuppfinna hjulet. Använd INTE alpha, beta eller saker som funnits mindre än 1 år, eller inte längre underhålls.