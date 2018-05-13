<sub>Följ arbetet med milestones [här](https://github.com/1dv611-futurum-project/futurum-project/milestones)</sub>

#### MILESTONE 1. Project Approval - Inception (Design Approval, Requirements Review, Project Setup)
<sub>**Deadline: 1 April**</sub>

<sub>**Mål med milestone:** En gemensam fungerande utvecklingsmiljö finns. En struktur för hur vi arbetar med olika features finns. Vi är överens om utseendet på front-end av applikationen och har bekräftat med kunden. Vi har en gemensam vision för projektet som är bekräftad med kunden. </sub>

<sub>**Inom gruppen:**  </sub>  
<sub> * Sätt upp gemensam utvecklings-(och produktions-?)miljö med Docker</sub>  
<sub> * Färdigställ en arkitektur för hela systemet</sub>  
<sub> * Ha ett buildsystem som fungerar med React och Webpack</sub>  
<sub> * Ha identifierat vilka olika components och containers vi behöver</sub>  

<sub>**Mot kunden:**  </sub>  
<sub> * Färdigställ visionsdokument och få det bekräftat av kund</sub>  
<sub> * Gör en mockup för utseendet av react-appen och bekräfta med kund</sub>  
<sub> * Visa arkitektur-diagram över systemet, få bekräftat av kund</sub>  

#### MILESTONE 2. Project Approval - Inception (Big technical hurdles gone)
<sub>**Deadline: 8 April**</sub>

<sub>**Mål med milestone:** Mail tas emot på mailserver, vår server notifieras, klienten-skelett finns.</sub>

<sub>**Inom gruppen:**  </sub>   
<sub> * Sätta upp vår server med Imap-connection till futurum-mailen</sub>  
<sub> * Komma åt inkorgen på dev@futurumdigital.se från vår server</sub>  
<sub> * Bli notifierade på vår server när något händer i inkorgen på dev@futurumdigital.se</sub>  
<sub> * Skelett för React-klienten färdigt med en fungerande React-router och placeholders för relevanta sidor.</sub>  

<sub>**Mot kunden:**  </sub> 
<sub> - </sub>   

<sub>**Mot universitetet:**  </sub>   
<sub> * Skicka in material till referentgrupp</sub>  

#### MILESTONE 3. Project Phase - Elaboration (Skeleton) 
<sub>**Deadline: 18 april**</sub>

<sub>**Mål med milestone:** Klienten notifieras via websocket när mail inkommer.</sub>

<sub>**Inom gruppen:**  </sub>  
<sub> * Sätt upp en websocket-kontakt mellan React-appen och servern</sub>  
<sub> * Skicka meddelande genom Websocket när ett mail kommer in på servern</sub>  
<sub> * Uppdatera state i React-appen när ett websocketmeddelande kommer in</sub>  

<sub>**Mot kunden:**  </sub>  
<sub> * Del-leverans av systemet, bekräfta att vi är på rätt spår</sub>  

<sub>**Mot universitetet:**</sub>  
<sub> * Granska referentgrupps material</sub>  
<sub> * Förbered 10 minuters presentation av projektet</sub>  

#### MILESTONE 4. Project Phase - Elaboration (Expanded functionality)
<sub>**Deadline: 29 April**</sub>

<sub>**Mål med milstenen:** Ärenden kan filtreras på status på klienten. Status på ärenden kan ändras på klienten, uppdateras då på servern. Mail kan skickas mellan klient, via server, ut till kund.</sub>

<sub>**Inom gruppen:**  </sub>  
<sub> * Ha satt upp en MongoDB-databas med dokument för mail</sub>  
<sub> * Spara mail i databasen när de kommer in till servern (titel + body + kund + status + vem som har hand om ärendet)</sub>  
<sub> * Ha klientsidor som visar ärenden baserat på status</sub>  
<sub> * Server kan returnera ärenden baserat på status (genom websocket?)</sub>  
<sub> * Kunna skicka mail från vår server, från dev@futurumdigital.se, till andra mailaddresser, via Zoho API</sub>  
<sub> * Klientvy som visar ett enskilt ärende, där ansvarig för, och status på, ärendet kan ändras och en mailkonversation visas, samt mail kan skickas</sub>  
<sub> * System (websocket?) för att notifiera servern om att mail ska skickas och vart, med vilket innehåll.</sub>  
<sub> * Uppdatera databasen när status på ett ärende ändras</sub>  

<sub>**Mot kunden:**  </sub>  
<sub> * Del-leverans av systemet, bekräfta att vi är på rätt spår</sub> 

<sub>**Mot universitetet:**  </sub>   
<sub> * Skicka in material till referentgrupp</sub>  
<sub> * Granska referentgrupps material</sub>  
<sub> * Förbered 10 minuters presentation av projektet</sub>  

#### MILESTONE 5. Project Phase - Construction (Whitelist management)
<sub>**Deadline: 20 maj**</sub>

<sub>**Mål med milstenen:** Kundmail kan skötas via klienten och hanteras olika på servern beroende på om de finns i whitelist eller ej. Vilka mail som ligger på whitelist kan styras från klienten. Mail som inte ligger på whitelist vidarebefodras från servern till en annan mailaddress.</sub>  

<sub>**Inom gruppen:**  </sub>  
<sub> * Identifiera hur vi ska spara undan whitelisten. Också MongoDB?</sub>  
<sub> * Sätta upp databashantering för whitelisten</sub>  
<sub> * Sätta upp kommunikationsväg client-server för att lägga till och ta bort mail från whitelisten</sub>  
<sub> * React-gränssnitt för att lägga till och ta bort mailadresser från whitelist</sub>  
<sub> * Skicka meddelande till servern när whitelisten uppdateras på klienten</sub>  
<sub> * Enbart skicka mailet vidare från servern till klienten beroende på om avsändaradressen på inkommande mail från finns i whitelist</sub>  
<sub> * Vidarebefodra mail som inte finns i listan till en annan mailaddress</sub>  

<sub>**Mot kunden:**  </sub>  
<sub> * Del-leverans av systemet</sub>   
<sub> * Tillvägagångssätt samt datum för slutleverans överenskommet</sub> 

<sub>**Mot universitetet:**  </sub>   
<sub> * Skicka in material till referentgrupp</sub>  
<sub> * Granska referentgrupps material</sub>  
<sub> * Förbered 10 minuters presentation av projektet</sub>  

#### MILESTONE 6. Final Approval - Transition (Phase 1)
<sub>**Deadline: 30 maj**</sub>

<sub>**Mål med milstenen:** Slutleverans av sysstem till kund. Presentation hålls på universitetet.</sub> 

<sub>**Inom gruppen:**  </sub>     
<sub> * Städa upp i koden</sub>    
<sub> * Städa upp i dokumentation</sub>    

<sub>**Mot universitetet:**  </sub>       
<sub> * Förbered och håll slutpresentation</sub>    

<sub>**Mot kunden:**  </sub>   
<sub> * Slutleverans av systemet, sista feedback</sub>    

#### MILESTONE 7. Final Approval - Transition (Phase 2)
<sub>**Deadline: 12 juni**</sub>  

<sub>**Mål med milstenen:** All dokumentation klar, inlämnad, systemet överlämnat till kund.</sub> 

<sub>**Inom gruppen:**  </sub>   
<sub> * Skriv slutrapport</sub>    
<sub> * Städa upp i dokumentation för inlämning</sub>   
<sub> * Skriv personliga reflektioner</sub>    

<sub>**Mot kunden:**  </sub>   
<sub> * Ev. sista leverans av systemet om det fanns tidigare feedback</sub>     

<sub>**Mot universitetet:**  </sub>   
<sub> * Bekräfta inlämning</sub>    