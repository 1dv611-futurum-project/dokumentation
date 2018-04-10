# UC1 Autentisera en användare och autentisera servern mot mailadressen som ska bevakas
## Huvudscenario
 <sub>1. Börjar när en användare vill komma åt applikationen</sub><br>
 <sub>2. Systemet frågar om användaren vill autentisera och tillåta applikationen åtkomst till mailen</sub><br>
 <sub>3. Systemet omdirigerar användaren till Googles OAuth-tjänst</sub><br>
 <sub>4. Googles inloggningstjänst ber om användarnamn och lösenord</sub><br>
 <sub>5. Google autentierar användaren och dirigerar tillbaka användaren till systemet</sub>

## Alternativa scenarion
<sub>2b. Användaren tillåter inte autentiering</sub><br>
* <sub>I. Google dirigerar tillbaka användaren till systemet</sub><br>
* <sub>II. Systemet visar ett felmeddelande om att autentiseringen inte tilläts</sub><br>
* <sub>III. Steg 2 i huvudscenario</sub>

<sub>5b. Användaren blir inte autentiserad</sub><br>
* <sub>I. Google dirigerar tillbaka användaren till systemet</sub><br>
* <sub>II. Systemet visar ett felmeddelande om att autentiseringen misslyckades</sub><br>
* <sub>III. Steg 2 i huvudscenario</sub>

## [Krav](https://github.com/1dv611-futurum-project/futurum-project/wiki/Kravspecifikation) som relaterar till detta scenario
* <sub> #7</sub>
* <sub> #8</sub>
* <sub> #13</sub>
* <sub> #14</sub>
* <sub> #15</sub>
* <sub> #16</sub>
* <sub> #17</sub>
* <sub> #18</sub>
* <sub> #19</sub>
* <sub> #20</sub>
* <sub> #21</sub>

# UC2 Lägga till registrerad avsändare
## Förutsättningar
<sub>Användaren är autentiserad ex. UC1</sub>

## Huvudscenario
 <sub>1. Börjar när en användare vill lägga till en registrerad avsändare</sub><br>
 <sub>2. Systemet frågar om mailadress och företagsnamn till avsändaren</sub><br>
 <sub>3. Användare förser mailadress och företagsnamn</sub><br>
 <sub>4. Systemet registrerar avsändaren och visar ett meddelande om att avsändaren sparats</sub>

## Alternativa scenarion
<sub>4a. Systemet kunde inte registrera avsändaren (adress finns redan, fel format på mailadress, fel format på företagsnamn)</sub><br>
* <sub>I. Systemet visar ett felmeddelande/sub><br>

## [Krav](https://github.com/1dv611-futurum-project/futurum-project/wiki/Kravspecifikation) som relaterar till detta scenario
* <sub> #17</sub>
* <sub> #18</sub>

# UC3 Ändra status på ärende
## Förutsättningar
<sub>Applikationen är tillåten åtkomst och användaren är autentiserad ex. UC1</sub><br>
<sub>Ärendet finns tillgängligt och har en registrerad avsändare ex. UC2</sub>

## Huvudscenario
 <sub>1. Börjar när en användare vill ändra status på ett ärende</sub><br>
 <sub>2. Systemet frågar om status på ärende/ärenden</sub><br>
 <sub>3. Användaren väljer att uppdatera status på ett ärende</sub><br>
 <sub>4. Systemet visar en popup-ruta och frågar om användaren vill skicka ärendeuppdateringen till avsändaren</sub><br>
 <sub>5. Användaren väljer att skicka statusuppdateringen till avsändaren</sub><br>
 <sub>6. Systemet stänger popup-rutan och visar ett meddelande om att statusuppdateringen skickats</sub><br>
 <sub>7. Systemet uppdaterar status på ärendet</sub>

## Alternativa scenarion
<sub>5a. Användaren väljer att inte skicka statusuppdateringen till avsändaren</sub><br>
* <sub>I. Systemet stänger popup-rutan</sub><br>
* <sub>II. Systemet uppdaterar status på ärendet</sub>

<sub>6a. Meddelandet kunde inte skickas</sub><br>
* <sub>I. Systemet stänger popup-rutan och visar ett felmeddelande</sub><br>
* <sub>II. Systemet uppdaterar inte status på ärendet</sub>

## [Krav](https://github.com/1dv611-futurum-project/futurum-project/wiki/Kravspecifikation) som relaterar till detta scenario
* <sub> #15</sub>
* <sub> #19</sub>

# UC4 Skicka meddelande till ärende
## Förutsättningar
<sub>Applikationen är tillåten åtkomst och användaren är autentiserad ex. UC1</sub><br>
<sub>Ärendet finns tillgängligt och har en registrerad avsändare ex. UC2</sub>

## Huvudscenario
 <sub>1. Börjar när en användare vill skicka ett meddelande till avsändaren av ett ärende</sub><br>
 <sub>2. Systemet frågar om meddelande</sub><br>
 <sub>3. Användaren förser ett meddelande</sub><br>
 <sub>4. Systemet skickar meddelandet och visar det skickade meddelandet i meddelandehistoriken</sub>

## Alternativa scenarion
<sub>4a. Meddelandet kunde inte skickas</sub><br>
* <sub>I. Systemet visar ett felmeddelande</sub>

## [Krav](https://github.com/1dv611-futurum-project/futurum-project/wiki/Kravspecifikation) som relaterar till detta scenario
* <sub> #16</sub>
* <sub> #18</sub>