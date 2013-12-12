*Linnéuniversitetet*
*Iterativ mjukvaruutveckling*
*HT 2013*

Laboration 3: Krav
Mattias Karlsson
mk222xa

#Krav

##Introduktion

[Barnens Uddevalla](https://github.com/mk222xa/Uppgift-234/blob/master/Vision.md) är en webbportal som riktar sig mot barn och deras föräldrar. Tanken med sidan är att information om aktiviteter, events och lokala föreningar ska vara samlat och lätt att ta del av oavsett ålder eller datorvana. 

##Användningsområden(User Cases)

Följande användningsområden fokuserar på Barnens Uddevalla.

### UC-01: Besökare letar information om events

Kort sammanfattning: Använderen besöker Barnens Uddevalla för att få information om events i Uddevalla under de kommande två veckorna. Events kommer att ligga på startsidan med närmsta eventet överst och användaren kan läsa en kortfattad beskrivning om eventet, var/när/hur och även en länk till organisatörens hemsida om det finns en lämplig sida att länka till. Varje event kommer även att finnas i ett utskriftsvänligt format så att besökaren kan skriva ut och ta med sig informationen. 

### UC-02: Organisatörer annonserar

Kort sammanfattning: När en organisatör ordnar ett event som riktar sig mot barn i åldrarna 4-15 så är Barnens Uddevalla tänkt att vara en självklar sida att annonsera på. Kraven på organisatören är att eventet är lämpligt för barn eller barn tillsammans med deras föräldrar. Varje event måste godkännas av Barnens Uddevalla och uppfylla rimliga krav om att inte sprida några hatiska, antidemokratiska eller rasistiska budskap. Organisatören måste ha tydlig information om vad en besökare kan förvänta sig och vilken åldersgrupp som avses (en lägsta ålder om någon sådan är lämplig). 

### UC-03: Lokala annonsörer vill nå ut till användare

Kort sammanfattning: När lokala annonsörer vill nå ut till potentiella kunder så är en annons på Barnens Uddevalla ett bra alternativ. Beroende på vilken typ av vara eller tjänst som annonsen avser så placeras annonsen på lämpligt ställe på Barnens Uddevalla i samråd med administratör. En kostnad kommer att tas ut baserad på hur länge annonsen skall finnas och var på sidan den ligger. 

### UC-04: Google AdWords annonsering

Kort sammanfattning: Google AdWords kommer användas och placeringen är väldigt viktig då annonserna inte får ta fokus från själva innehållet eller på något sätt påverka navigationen. En väl strukturerad HTML5 och CSS kod är oerhört viktigt här! 

### UC-05: Lokala föreningar vill nå ut med information

**Nivå:** Underfunktion

**Huvudaktör:** Förening

**Sekundär aktör:** Administratör för Barnens Uddevalla

**Andra aktörer:** Besökande barn och föräldrar 

**Intressenter och deras områden:**

_Förening:_
Föreningen vill nå ut till nya kunder och sprida information om deras verksamhet.

_Administratör för Barnens Uddevalla:_
Administratören kontrollerar föreningens information och hjälper till med att skapa ett konto åt föreningen.

_Besökande barn och föräldrar:_
Denna aktör är målgruppen som ska surfa in på sidan och ta del av information och reklam på ett tydligt och enkelt sätt.

**Huvudmålet**

 _Förening:_

1. Föreningen kontaktar Barnens Uddevalla via email eller telefon.

2. Administratör för Barnens Uddevalla för in information och skapar ett konto åt föreningen.

3. Föreningen för in egen information och uppdateringar.

_Administratör för Barnens Uddevalla:_

1. Administratören tar emot information från föreningen och verifierar att den stämmer.

2. Administratören skapar ett konto föreningen

_Besökande barn och föräldrar:_

1. Besökaren går in på sidan och möts av en tilltalande design och ett eller flera event listade på startsidans nyhetsflöde.

2. Besökaren klickar på ett event för att få mer information.

3. Besökaren "surfar runt" på sidan och tar del av olika föreningars information

4. Besökaren klickar på tilltalande reklam

**Tillägg:**

***a. Administratör för Barnens Uddevalla är inte tillgänglig***

1. Automatiskt mailsvar med information

2. Telefonsvarare där ett meddelande kan lämnas

3. Administratör återkommer snarast möjligt till förening

4. Föreningens konto blir upprättat och föreningen kan i fortsättningen uppdatera sin information utan att kontakta administratör

***b. Informationen som förening lämnar överensstämmer inte med verkligheten***

1. Förening underrättas omgående av administratör

2. Informationen uppdateras för att återspegla verkligheten

***c. Inloggning och/eller uppdatering av information fungerar ej för förening***

1. Lösenordsåterställning via hemsida

2. Kvarstår problemet kontaktas administratören.

3. Administratör åtgärdar felet på lämpligt sätt

### UC-06: Besökaren vill skriva ut information

Kort sammanfattning: Det är viktigt att informationen på Barnens Uddevalla finns i ett bra utskriftsformat. Det ska vara möjligt att få upp varje enskilt event i ett separat utskriftsfönster där användaren kan skriva ut informationen på ett bra sätt. Föreningars information ska vara utskiftsvänligt, det ska vara möjligt att välja om du vill skriva ut med eventuella bilder eller bara text. 

### UC-07: Sammankoppling med sociala medier

Kort sammanfattning: Barnens Uddevalla kommer att finnas på Twitter, Facebook, Google+ och Instagram. Det är viktigt att administratören är aktiv och uppdaterar nyhetsflödet på dessa medier samtidigt som dessa uppdateringar länkas in på den egna hemsidan i ett nyhetsflöde där besökaren kan klicka på en nyhet och komma till det sociala media som är aktuellt. Uppdateringarna på dessa sociala medier måste vara aktuella men korta och en mer utförlig uppdatering ska finnas på Barnens Uddevallas hemsida för att locka dit besökare. Här är det arbete med respektive medies API som gäller, det ska finnas en "Gilla" knapp för varja medie på hemsidan. 

### UC-08: Mobil anpassning av sidan

Kort sammanfattning: Det är viktigt att sidan har en responsiv design då väldigt många surfar från mobil. Telefonnummer till olika events och föreningar ska vara införda på ett sådant sätt att besökaren som surfar på mobilen kan klicka på det telefonnummer som är listat för det som eftersöks och då få upp alternativet att ringa direkt från telefonen eller Skype i de fall där Skype är installerat på mobiltelefonen. En välskriven HTML5-kod får det här att fungera.

### UC-09: En besökare vill tipsa vänner och bekanta

Kort sammanfattning: När en besökare hittar något som är intressant t. ex. ett event som vore aktuellt att dela med sig av till vänner och bekanta så ska det finnas en ikon för att dela. Om besökaren trycker på ikonen för att dela så ska en "popup" dyka upp med alternativen för Facebook, Google+ eller direkt till kompisens email(här är det möjligt att skriva in flera emailadresser). 

### UC-10: En aktör vill rapportera om ett fel på sidan eller i informationen

Kort sammanfattning: På undersidan "Kontakta Barnens Uddevalla" ska ett kontaktformulär finnas med en dropdown lista över olika alternativ. Här kan den som vill kontakta markera vad det gäller och även skriva ett meddelande. När formuläret skickas så sorteras det efter vad ärendet gäller på servern och skickas sedan vidare till administratör för Barnens Uddevalla. En kopia på meddelandet kommer även att skickas till den som kontaktade Barnens Uddevalla. Vid förfrågningar kontaktar administratör den som kontaktade Barnens Uddevalla antingen via email eller telefon efter önskemål. Vid felanmälan så åtgärdas felet snarast möjligt, information uppdateras och buggar åtgärdas.

