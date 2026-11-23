# Mottagaranpassning

Skrivmodulens paket `reader` (modulen `writing`, profilen `core`) bär
principen att varje text skrivs för en bestämd läsare, och paketet
`integrity` bär principen att texten är avsändarens egen. Båda gäller
svensk text oförändrade. Filen lägger till det som är svenskt: Isofs
råd om läsaren och tonen, de svenska tilltalsorden, det återhållsamma
registret och avsändarens ansvar när en språkmodell har varit med i
arbetet. Markörerna som får svensk text att läsas som maskinsvenska
står i paketet `maskinsvenska`, och klarspråkskravet i språklagen står
i [standardsvenska.md](../../regler/reference/standardsvenska.md).

## Läsarens frågor först

Isofs Klarspråkshjälpen börjar med syftet och läsaren. Skribenten
frågar sig vem som läser, i vilken situation, med vilken oro eller
nyfikenhet och med vilka förkunskaper, och väljer först därefter
innehåll, ton och ord. Isof råder också att svara på läsarens frågor
först i stället för att följa avsändarens ordning, vilket är samma
ordning som skrivmodulens `answer_first` och `reader_order` kräver.

Testet är frågan Isof ställer: vad skulle jag vilja veta först om jag
var läsaren? Inleds texten med avsändarens bakgrund, regelverket eller
en allmän upptakt flyttas svaret upp.

## Artig utan utfyllnad

Isof råder att hälsa och tacka och påpekar att en text som är för kort
kan uppfattas som ovänlig. Rådet ger inget utrymme för utfyllnad. En
hälsning och ett tack tar en mening var, och båda riktar sig till den
här läsaren i den här situationen. Det som därefter står före
sakinnehållet prövas mot katalogen i paketet `maskinsvenska`.

För kort (undvik, illustrativt):

> Bilaga 4 saknas. Komplettera.

Utfyllt (undvik, illustrativt):

> Hej! Vi hoppas att allt är bra med dig. Vi vill börja med att tacka dig så mycket för din ansökan, som vi har tagit emot och läst med stort intresse. Vi vill dock uppmärksamma dig på att bilaga 4 tyvärr saknas.

Bättre (illustrativt):

> Hej! Tack för din ansökan. Bilaga 4 saknas, och vi kan pröva ansökan först när den har kommit in. Skicka den gärna senast den 15 december.

## Tilltalet

Isof rekommenderar *du* med gemen som det normala tilltalet till
enskilda, också när en text till många tilltalar var och en
personligt, och *ni* med gemen till flera personer och till juridiska
personer som företag. Den läsare som tilltalas direkt får sitt eget
pronomen: "din redogörelse" i stället för "den sökandes redogörelse".
Versalt *Du* är tänkt som ett mellanting mellan du och ni, men Isof
påpekar att vissa läsare uppfattar det som insmickrande och andra som
avståndstagande, så det används inte. Åsikterna om *ni* varierar på
samma sätt, där en del hör det som artigt och andra som distanserat,
och sammanhanget avgör.

Ett affärsdokument till en organisation tilltalar den med *ni*, enligt
profilen `affarsdokument`.

## En synlig avsändare

Läsaren ska kunna se vem som beslutar, gör och svarar. Isof råder att
organisationen nämns vid namn en gång och att texten därefter skriver
*vi*, att samma text inte blandar olika *vi* (myndigheten, en
projektgrupp och ett allmänt vi som betyder *man*), och att den som
skriver ensam, till exempel i ett mejl, skriver *jag*.

Maskinellt omskriven svensk text kan tappa avsändaren. I en
kandidatuppsats från Lunds universitet (2024) följde tre omskrivningar
gjorda med en språkmodell och tre gjorda av människor samma
klarspråksråd lika väl, och den enda skillnad som gällde hela gruppen
var att vi-perspektivet saknades i de maskinella texterna. Underlaget
är litet, så resultatet är en indikation och inget belagt mönster.
Markören står som post 9 i katalogen i paketet `maskinsvenska`.

## Tonen följer avsändare, texttyp och kanal

Isof råder att tonen anpassas efter avsändaren, texttypen och kanalen.
En organisation kan vilja låta mänsklig, vänlig och hjälpsam, och en
myndighet behöver enligt Isof inte låta som en byråkratisk robot ens
när beskedet är tråkigt. Ett beslut ska vara korrekt och juridiskt
hållbart, men det behöver inte vara krångligt. En webbtext kan ofta
vara lättare, och i sociala medier kan humor fungera. Den allmänna
regeln om ett register per text står i `tone_and_register` (modulen
`writing`, profilen `core`, paketet `basics`).

## Det återhållsamma registret

Svensk offentlig kommunikation har beskrivits med ideal som lugn,
måttfullhet, kompromiss, *lagom* och att inte framstå som mer än andra
(Allwood, i en engelsk översättning från 1999 av en text från 1982).
Beskrivningen är generaliserande och äldre, och nyare forskning om
svenska komplimangsvar läser normen som balans och uppriktighet snarare
än som förnekelse av egna förtjänster. Saken är alltså omstridd som
beskrivning av hur svenskar faktiskt skriver.

För skrivandet räcker en försiktigare slutsats. Det konstaterande
registret i `tone_and_register` gäller redan, och på svenska hörs en
engelsk säljton i form av superlativ, entusiasmord och löften om
utfall lätt som reklam eller som översättning. Engagemang och värde
visas därför med konkreta skäl och fakta. Återhållsamhet är ändå ingen
gardering, så ett belagt påstående står utan förbehåll enligt
skrivmodulens paket `claims`. Markörerna står som post 4 och post 5 i
katalogen i paketet `maskinsvenska`.

## Text som sammanfattas av en maskin

Isof råder att skriva så att den som låter en AI-tjänst sammanfatta
texten får med huvudbudskapet. Det kräver en tydlig sammanfattning,
informativa mellanrubriker och det viktigaste först, vilket är samma
råd som _Myndigheternas skrivregler_ ger om sammanfattning och
rubriker (se
[myndigheternas_skrivregler.md](../../regler/reference/myndigheternas_skrivregler.md)).
En text som en människa kan skumma är också en text som en maskin
sammanfattar rätt.

## Avsändaren står för texten

Isof slår fast att den som tar hjälp av AI själv ansvarar för texten
och måste kontrollera resultatet. Fakta och resonemang kontrolleras,
och skribenten prövar att det som lyfts fram verkligen är det
viktigaste för läsarna. Isof råder också skribenten att ge den färdiga
texten sin egen karaktär.

Kontrollen gäller också betydelsen. I ett test som
Isofs bulletin _Klarspråk_ publicerade 2023 gjorde en språkmodell en
flytande och i övrigt bra omskrivning, men den ändrade "studier runt om
i världen" till "globala studier" och påstod därmed något om studierna
som originalet inte sa. En sådan ändring syns inte i en språkgranskning
och fångas bara av den som jämför med sakunderlaget.

Testet för varje mening i en text som en språkmodell har skrivit eller
bearbetat är om avsändaren kan stå för den. Uppgiften ska stämma med
sakunderlaget, och meningen ska vara en som avsändaren skulle kunna
säga till läsaren och förklara om hen fick frågan. Principen och dess
språkoberoende test står i skrivmodulens paket `integrity`. Att rensa
bort markörerna ur en text som avsändaren inte står för gör den inte
till avsändarens egen, och katalogen i `maskinsvenska` är därför ett
redigeringsstöd och ingen metod att dölja ursprunget.

## Hur svenska läsare tar emot maskinskrivet material

Underlaget om svenska läsare är tunt. Ingen svensk studie av hur läsare
uppfattar maskinskriven svensk sakprosa har hittats (2026-11-23). Två
uppgifter pekar ändå åt samma håll som den internationella forskning
som skrivmodulens paket `reader` redovisar.

- Enligt en Novusundersökning från juni 2025 (1 095 intervjuer) är
  svenskar fortfarande mest negativa till AI-genererat material i
  marknadsföring och kommunikation, och de negativa svaren om
  myndigheters kommunikation har ökat. I de fria svaren beskrivs sådant
  material bland annat som fejk, vilseledande, själlöst och slarvigt,
  medan en växande grupp godtar det med villkor som märkning och mänsklig
  kvalitetskontroll. Frågorna gällde material i allmänhet och inte text
  särskilt.
- En studie med japanska deltagare (Nakano m.fl., 2026) fann att
  uppgiften om att en text var AI-skriven sänkte läsarnas bedömning av
  författarens trovärdighet, omtanke och sympati, och att sänkningen
  var störst i mellanmänskliga texter som meddelanden. Resultatet gäller
  inte nödvändigtvis svenska läsare.

Slutsatsen för skrivandet vilar på principen, och siffrorna stöder den.
En text som läsaren uppfattar som skriven av ingen säger att läsaren
inte var värd avsändarens tid, och det gäller i synnerhet personliga
meddelanden.

## Källor

- https://www.isof.se/svenska-spraket/klarsprak/klarsprakshjalpen/skriv-klarsprak/tank-pa-dina-lasare — Isof, Klarspråkshjälpen: Tänk på dina läsare (publicerad 19 april 2022, uppdaterad 11 september 2026); hämtad 2026-11-23.
- https://www.isof.se/svenska-spraket/klarsprak/klarsprakshjalpen/skriv-klarsprak/tank-pa-dina-lasare/fordjupning-tank-pa-dina-lasare/anpassa-tonen-efter-sammanhanget — Isof, Anpassa tonen efter sammanhanget (publicerad 19 april 2022, uppdaterad 18 maj 2022); hämtad 2026-11-23.
- https://www.isof.se/svenska-spraket/klarsprak/klarsprakshjalpen/skriv-klarsprak/tank-pa-dina-lasare/fordjupning-tank-pa-dina-lasare/du-eller-ni-myndigheten-eller-vi — Isof, Du eller ni? Myndigheten eller vi? (publicerad 19 april 2022, uppdaterad 18 maj 2022); hämtad 2026-11-23.
- https://frageladan.isof.se/faqs/21774 — Isofs Frågelåda: du med liten bokstav, versalt Du uppfattas som insmickrande eller avståndstagande; hämtad 2026-11-23.
- https://frageladan.isof.se/faqs/25179 — Isofs Frågelåda: du och ni till enskilda, flera och juridiska personer; hämtad 2026-11-23.
- https://www.isof.se/svenska-spraket/klarsprak/klarsprakshjalpen/skriv-klarsprak/ta-hjalp-av-ai — Isof, Klarspråkshjälpen: Ta hjälp av AI (publicerad 22 april 2025, uppdaterad 11 september 2026); ansvaret för texten, kontroll av fakta, text som sammanfattas av AI; hämtad 2026-11-23.
- https://www.isof.se/svenska-spraket/klarsprak/bulletinen-klarsprak/artiklar-klarsprak/2023-12-06-skrivradet-ai-som-klarsprakskollega — Ulrika Gotthardsson, "Skrivrådet: AI som klarspråkskollega", _Klarspråk_ 4/2023 (6 december 2023); betydelseändringen "runt om i världen" → "globala"; hämtad 2026-11-23.
- https://lup.lub.lu.se/student-papers/search/publication/9159126 — Zarah Lundberg, "Kan Chat GPT klarspråksanpassa text? Svaret är ja." (kandidatuppsats, Lunds universitet, 2024); vi-perspektivet saknades i de maskinella texterna; hämtad 2026-11-23.
- https://gup.ub.gu.se/file/120719 — Jens Allwood, "Are There Swedish Patterns of Communication?", i H. Tamura (red.), _Cultural Acceptance of CSCW in Japan & Nordic Countries_, Kyoto Institute of Technology 1999, s. 90–120 (översättning av en text från 1982); hämtad 2026-11-23.
- https://www.frontiersin.org/journals/communication/articles/10.3389/fcomm.2026.1836869/full — Dehghani och Huang, "Compliment responses in Persian and Swedish", _Frontiers in Communication_ 11 (19 maj 2026); jantelagen och lagom som balans och uppriktighet; hämtad 2026-11-23.
- https://novus.se/egnaundersokningar-arkiv/syn-pa-ai-genererat-innehall/ — Novus, "Svenskarnas syn på AI-genererat innehåll: Försiktig normalisering" (fältperiod vecka 25 2025, n = 1 095); hämtad 2026-11-23.
- https://arxiv.org/abs/2510.24011 — Nakano, Takezawa, Matulic, Yang och Yatani, "Understanding Reader Perception Shifts upon Disclosure of AI Authorship" (v2, 22 januari 2026, IUI '26; japanska deltagare); hämtad 2026-11-23.
