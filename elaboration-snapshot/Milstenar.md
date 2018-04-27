<sub>Följ arbetet med milstenar [här](https://github.com/1dv611-futurum-project/futurum-project/milestones).</sub>

#### [MILSTEN 1. Project Approval - Inception (Godkännande av design, Kravgranskning, Projektstruktur)](https://github.com/1dv611-futurum-project/futurum-project/milestone/1)
<sub>**Deadline: 1 April 2018**</sub>

<sub>**Mål med milstenen:** En gemensam fungerande utvecklingsmiljö finns. En struktur för hur vi arbetar med olika features finns. Vi är överens om utseendet på front-end av applikationen och har bekräftat med kund. Vi har en gemensam vision för projektet som är bekräftad av kund. </sub>

<sub>**Inom gruppen:**  </sub>  
<sub> * Sätt upp gemensam utvecklings-miljö med Docker</sub>  
<sub> * Färdigställ en arkitektur för hela systemet</sub>  
<sub> * Ha ett buildsystem som fungerar med React och Webpack</sub>  
<sub> * Ha identifierat vilka olika komponenter och containrar vi behöver för en komponentbaserad arkitektur på klienten</sub>  

<sub>**Mot kunden:**  </sub>  
<sub> * Färdigställ visionsdokument och få det bekräftat av kund</sub>  
<sub> * Gör en mock-up för utseendet av React-applikationen och bekräfta med kund</sub>  
<sub> * Visa arkitektur-diagram över systemet, få bekräftat av kund</sub>  

#### [MILSTEN 2. Project Approval - Inception (Stora tekniska hinder borttagna)](https://github.com/1dv611-futurum-project/futurum-project/milestone/2)
<sub>**Deadline: 8 April 2018**</sub>

<sub>**Mål med milstenen:** Mail tas emot på mail-server, vår server notifieras, klient-skelett finns.</sub>

<sub>**Inom gruppen:**  </sub>   
<sub> * Sätta upp vår server med IMAP-förbindelse till Futurum Digitals supportmail</sub>  
<sub> * Komma åt inkorgen på dev@futurumdigital.se från vår server</sub>  
<sub> * Bli notifierade på vår server när något händer i inkorgen på dev@futurumdigital.se</sub>  
<sub> * Skelett för React-klienten färdigt med en fungerande React-router och platshållare för relevanta sidor.</sub>  

<sub>**Mot kunden:**  </sub> 
<sub> - </sub>   

<sub>**Mot universitetet:**  </sub>   
<sub> * Skicka in material till referentgrupp</sub>  

#### [MILSTEN 3. Project Phase - Elaboration (Skelett)](https://github.com/1dv611-futurum-project/futurum-project/milestone/3)
<sub>**Deadline: 18 april 2018**</sub>

<sub>**Mål med milstenen:** Klienten notifieras via Websocket när mail inkommer.</sub>

<sub>**Inom gruppen:**  </sub>  
<sub> * Sätt upp en Websocket-kontakt mellan React-appen och servern</sub>  
<sub> * Skicka meddelande genom Websocket när ett mail kommer in på servern</sub>  
<sub> * Uppdatera "state" i React-appen när ett Websocket-meddelande kommer in</sub>  

<sub>**Mot kunden:**  </sub>  
<sub> * Delleverans av systemet, bekräfta att vi är på rätt spår</sub>  

<sub>**Mot universitetet:**</sub>  
<sub> * Granska referentgruppens material för Inception-fasen</sub>  
<sub> * Förbered 10 minuters presentation av Inception-fasen</sub>  

#### [MILSTEN 4. Project Phase - Elaboration (Utökad funktionalitet)](https://github.com/1dv611-futurum-project/futurum-project/milestone/4)
<sub>**Deadline: 2 Maj 2018**</sub>

<sub>**Mål med milstenen:** Ärenden kan filtreras på status på klienten. Status på ärenden kan ändras på klienten och uppdateras då på servern. Mail kan skickas mellan klient, via server, ut till kund.</sub>

<sub>**Inom gruppen:**  </sub>  
<sub> * Ha satt upp en MongoDB-databas med dokument för mail</sub>  
<sub> * Spara mail i databasen när de kommer in till servern (titel + body + kund + status + vem som har hand om ärendet)</sub>  
<sub> * Ha klientsidor som visar ärenden baserat på status</sub>  
<sub> * Server kan returnera ärenden baserat på status (genom websocket?)</sub>  
<sub> * Kunna skicka mail från vår server, från dev@futurumdigital.se, till andra mailaddresser</sub>  
<sub> * Klientvy som visar ett enskilt ärende, där ansvarig för, och status på, ärendet kan ändras och en mailkonversation visas, samt mail kan skickas</sub>  
<sub> * Websocket-förbindelse för att notifiera servern om att mail ska skickas och vart, med vilket innehåll</sub>  
<sub> * Uppdatera databasen när status på ett ärende ändras</sub>  

<sub>**Mot kunden:**  </sub>  
<sub> * Delleverans av systemet, bekräfta att vi är på rätt spår</sub> 

<sub>**Mot universitetet:**  </sub>   
<sub> * Skicka in material till referentgrupp</sub>  
<sub> * Granska referentgrupps material</sub>  
<sub> * Förbered 10 minuters presentation av Elaboration-fasen</sub>  

#### [MILSTEN 5. Project Phase - Construction (Felhantering & hantering av oregistrerade kunder)](https://github.com/1dv611-futurum-project/futurum-project/milestone/5)
<sub>**Deadline: 20 maj**</sub>

<sub>**Mål med milstenen:** Inkomna mail/ärenden till Futurum Digitals supportmail kan skötas via klienten och hanteras olika på servern beroende på om de finns i vitlistan av registrerade kunder eller ej. Vilka registrerade kunder som finns på vitlistan kan styras från klienten. Mail som inte ligger på vitlistan vidarebefordras från servern till en extern mailadress. Mail skickas även till den externa mailadressen vid fel i systemet under hantering av inkommande mail/ärenden.</sub>  

<sub>**Inom gruppen:**  </sub>  
<sub> * Identifiera hur vi ska spara undan vitlistan (MongoDB?)</sub>  
<sub> * Sätta upp databashantering för vitlistan</sub>  
<sub> * Sätta upp kommunikationsväg klient-server för att lägga till och ta bort mail från vitlistan</sub>  
<sub> * React-gränssnitt för att lägga till och ta bort mailadresser från vitlistan</sub>  
<sub> * Skicka meddelande till servern när vitlistan uppdateras på klienten</sub>  
<sub> * Enbart skicka inkomna mail vidare från servern till klienten om avsändaradressen för mailet finns med i vitlistan</sub>  
<sub> * Vidarebefodra mail som inte finns i listan till en extern mailadress</sub>  
<sub> * Meddela extern mailadress vid fel i systemet under hantering av ärenden</sub>  

<sub>**Mot kunden:**  </sub>  
<sub> * Delleverans av systemet</sub>   
<sub> * Tillvägagångssätt samt datum för slutleverans överenskommet</sub> 

<sub>**Mot universitetet:**  </sub>   
<sub> * Skicka in material till referentgrupp</sub>  
<sub> * Granska referentgruppens material för Construction-fasen</sub>  

#### [MILSTEN 6. Final Approval - Transition (Fas 1)](https://github.com/1dv611-futurum-project/futurum-project/milestone/6)
<sub>**Deadline: 30 maj 2018**</sub>

<sub>**Mål med milstenen:** Slutleverans av systemet till kund. Presentation hålls på universitetet.</sub> 

<sub>**Inom gruppen:**  </sub>     
<sub> * Städa upp i koden</sub>    
<sub> * Städa upp i dokumentationen</sub>    

<sub>**Mot universitetet:**  </sub>       
<sub> * Förbered och håll slutpresentation</sub>    

<sub>**Mot kunden:**  </sub>   
<sub> * Slutleverans av systemet, sista feedback</sub>    

#### [MILSTEN 7. Final Approval - Transition (Fas 2)](https://github.com/1dv611-futurum-project/futurum-project/milestone/7)
<sub>**Deadline: 12 juni 2018**</sub>  

<sub>**Mål med milstenen:** All dokumentation är klar och inlämnad, systemet är överlämnat till kund.</sub> 

<sub>**Inom gruppen:**  </sub>   
<sub> * Skriv slutrapport</sub>    
<sub> * Städa upp i dokumentationen inför inlämning</sub>   
<sub> * Skriv personliga reflektioner</sub>    

<sub>**Mot kunden:**  </sub>   
<sub> * Ev. sista leverans av systemet om det fanns tidigare feedback</sub>     

<sub>**Mot universitetet:**  </sub>   
<sub> * Bekräfta inlämning</sub>    