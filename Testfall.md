*Linnéuniversitetet*
*Iterativ mjukvaruutveckling*
*HT 2013*

Laboration 4: Testfall
Mattias Karlsson
mk222xa

#Barnens Uddevalla

#Testfall

Testfallet utgår från [*UC-05: Uppdatera information*](https://github.com/mk222xa/Uppgift-234/blob/master/Krav.md#information) som presenterades vid tidigare redovisning.

### UC-05: Uppdatera information <a name="information"></a>

**Nivå:** Underfunktion

**Huvudaktör:** Användare

**Sekundär aktör:** Administratör för Barnens Uddevalla

**Andra aktörer:** Besökande barn och föräldrar 

**Intressenter och deras områden:**

_Förening:_
Föreningen vill nå ut till nya kunder och sprida information om deras verksamhet.

_Administratör för Barnens Uddevalla:_
Administratören kontrollerar föreningens information och hjälper till med att skapa ett konto åt föreningen.

_Besökande barn och föräldrar:_
Denna aktör är målgruppen som ska surfa in på sidan och ta del av information och reklam på ett tydligt och enkelt sätt.

**Scenario**

 _Förening:_

1. Användare kontaktar Barnens Uddevalla för att skapa ett konto.

2. Systemet för in information och skapar ett konto åt föreningen.

_Administratör för Barnens Uddevalla:_

1. Systemet får en begäran om att skapa ett nytt konto.

2. Administratören kontrollerar samt godkänner eller nekar.

_Besökande barn och föräldrar:_

1. Användaren söker efter viss information i en sökruta

2. Systemet presenterar information (om tillgängligt) som länk(ar)

3. Användaren klickar på valfri presenterad länk

4. Användaren dirigeras till rätt sida

**Tillägg:**

***a. Fel vid ifyllande av kontaktformulär***

1. Felmeddelande visas

2. En automatisk felrapport sänds till administratör

3. Administratör administratör åtgärdar felet

4. Användaren fyller i informationen på nytt

***b. Sökruta fungerar ej***

1. Felmeddelande visas

2. En automatisk felrapport sänds till administratör

3. Administratör åtgärdar fel

***c. Inloggning fungerar ej för användare***

1. Lösenordsåterställning via hemsida

2. Systemet skickar nytt lösenord via email till användare

#Testfall UC-05

###TF1.1 Huvudscenario: Inloggning som administratör
1. Gå till inloggningssidan
2. Inloggningsruta presenteras
3. Användarnamn: admin, Lösenord: admintest
4. Inloggningen lyckades och administratörsrättigheter är aktiva

###TF 1.2 Huvudscenario: Inloggning som user
1. Gå till inloggningssidan
2. Inloggningsruta presenteras
3. Användarnamn: testuser, Lösenord: usertest
4. Inloggningen lyckades och rättigheter som user är aktiva

###TF 1.3 Alternativt scenario: Inloggningen misslyckades
1. Gå till inloggningssidan
2. Inloggningsruta presenteras
3. Användarnamn: userfail, Lösenord: userfail.
4. Inloggningen misslyckas och ett felmeddelande presenteras
5. Inloggningsruta presenteras med kvarstående felmeddelande samt länk till lösenordsåterställning

###TF2.1 Huvudscenario: User vill uppdatera information
1. Gå till inloggningssidan
2. Användarnamn:userupdate, Lösenord:userupdate
3. Gå till sidan för userinfo
4. Uppdatera Namn:Test User, Tel: 0522-73905, Email:testuser@barnensuddevalla.se
5. Informationen uppdateras och ett meddelande visas

### TF2.1 Efterkrav

Systemet skickar ett email till den nya emailadressen. Administratören måste även kontrollera de nya uppgifterna så att dessa stämmer samt ringa till det nya telefonnummret och se att det är en giltig förening.

###TF2.2 Alternativt scenario 1: Felaktigt format på information
1. Gå till inloggningssidan
2. Användarnamn:userupdate, Lösenord:userupdate
3. Gå till sidan för userinfo
4. Uppdatera Namn:T3st U53r, Tel: Nollfem22-73905, Email:Notavalidemail
5. Felaktigt formatterad information visas genom att rutorna lyser rött

###TF2.3 Alternativt scenario 2: Servern fungerar inte
1. Gå till inloggningssidan
2. Användarnamn:userupdate, Lösenord:userupdate
3. Felmeddelande visas

###TF3.1 Huvudscenario: Användare vill skapa ett konto
1. Gå till inloggningssidan
2. Välj "Skapa nytt konto"
3. Fyll i Användarnamn:newuser, Lösenord:newuser, Förening:Testförening
4. Administratör kontaktas av systemet och godkänner/nekar

###TF3.2 Alternativt scenario 1: Ogiltigt information vid registrering
1. Gå till inloggningssidan
2. Välj "Skapa nytt konto"
3. Fyll i Användarnamn:failed&/user, Lösenord:12, Förening:(blankt)
4. Felmeddelande visas och felaktigt ifyllda fält rödmarkeras

###TF3.3 Alternativt scenario 2: Systemet är ur funktion
1. Gå till inloggningssidan
2. Välj "Skapa nytt konto"
4. Felmeddelande visas 