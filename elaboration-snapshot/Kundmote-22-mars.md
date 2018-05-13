## Johans anteckningar

* Ärende system
* support@futum digital
* nuvarande mail soho mail
* Nästa möte onsdag kl 14:00.

### Admingränssnitt
* Mail.body (content)
* Vidarebefordra
* Status
* (Eventuell auth i ett senare skede på admingränssnittet)

* Node server lyssnar på inkommande mail
* Spara i databas
* Websocket middleware
* Reactapp – ärendehantering
* Ett kort per ärende (material design card)
* Felhantering

### Logik
* Vem har rättigheter att skicka mail till servern?
* vem skickade
* Statushantering
  * 0 - Ej påbörjad
  * 1 - Påbörjad
  * 2 - Avslutad, genomförd
  * 3 - Avslutad, kommer inte ändras
* Redirect beroende vem ärendet gäller

### Tekniker
* Node.js
* React
* tslint eller prettify
* TypeScript

### Mina funderingar
* Lägger vi upp en egen smtp i node.js?
* Vi måste fundera på hur mongodb schema ska se ut så tidigt som möjligt.
   1. Förenkla mot react eller mailet?
   2. Ligger all ticket logik i react?
* Var börjar vi utvecka, server eller client? Måste ha en aning om vilken data vi jobbar med från servern innan vi börjar med clienten.

### Projektstruktur
* Sätta egna milestones, utgå från de Anton lägger upp på Asana