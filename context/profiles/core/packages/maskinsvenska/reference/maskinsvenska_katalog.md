# Katalog över maskinsvenska

Maskinsvenska är svensk text som läses som en mall eller som en
översättning från engelska, även när varje ord är rätt stavat. En
läsare som märker det kan dra slutsatsen att ingen skrev just till hen.
Skrivmodulens paket `machine_tells` (modulen `writing`, profilen
`core`) bär de språkoberoende markörerna och paketet `anti_patterns`
de strukturella, och båda gäller svensk text oförändrade. Katalogen
här bär de svenska formerna av dem och de markörer som bara finns i
svenskan.

Varje post är ett test med ett smalt undantag, enligt principen i
`tests_not_bans` (modulen `writing`, profilen `core`, paketet
`basics`). En människa kan skriva vilken som helst av markörerna, och
en språkmodell kan undvika dem alla, så katalogen säger ingenting om
vem som skrev en text. Den säger hur texten läses. Exemplen är
illustrativa och omskrivningarna skisser som inte lägger till några
fakta.

Underlaget är ojämnt, och varje post anger sitt. Där Isof,
Språkrådet eller Regeringskansliet har en regel bygger posten på den.
Någon lista från Isof över markörer för AI-skriven svenska har inte
hittats (2026-11-23), så flera poster vilar på iakttagelser från
praktiker. De är märkta som iakttagelser, och katalogen påstår ingenting
om hur vanliga markörerna är.

## Ordval och fraser

### 1. Trendinramningen

Test: texten förlorar ingen uppgift om den inledande inramningen
stryks. Fraser som "i dagens snabbrörliga värld", "i en alltmer
digitaliserad tid", "nu mer än någonsin" och "i takt med att AI
förändrar allt" klarar sällan testet.

Undvik (illustrativt):

> I dagens snabbrörliga värld är det viktigare än någonsin att ha koll på sina fakturor.

Bättre (illustrativt):

> Tjänsten matchar inkommande fakturor mot beställningar och flaggar avvikelser.

Undantag: förändringen är själv ämnet och anges med tid, plats eller
siffra ("Sedan 2024 tar kommunen bara emot ansökningar digitalt").

Underlag: iakttagelse från praktiker; samma mönster som
innehållsdeklarationen i skrivmodulens katalog (`catalogue`, post 10).

### 2. Tyngd utan tyngd

Test: meningen säger vad som är viktigt och för vem. Fraser som "det
är viktigt att notera att", "det är värt att nämna att", "det är
avgörande att" och "det är ingen hemlighet att" påstår en vikt som
meningen sedan inte visar, och de stryks så att uppgiften står ensam.

Undvik (illustrativt):

> Det är viktigt att notera att ansökan måste vara komplett.

Bättre (illustrativt):

> Vi kan bara pröva en komplett ansökan.

Undantag: *Observera att* i en instruktion, före en följd som läsaren
annars skulle missa, med följden utskriven i samma mening.

Underlag: den engelska formen står i `cut_padding` (modulen `writing`,
profilen `core`, paketet `basics`).

### 3. Ord-för-ord-lån

Test: en van svensk skribent som kände fakta skulle ha valt samma
uttryck. Ett översättningslån som bara följer den engelska frasen
skrivs om med det svenska uttrycket.

Undvik → bättre (illustrativt):

> vi tar fullt ägarskap för leveransen → vi ansvarar för hela leveransen · på daglig basis → dagligen · i slutet av dagen handlar det om kvalitet → till sist avgör kvaliteten · jag hoppas att detta mejl finner dig väl → (stryks) · tveka inte att höra av dig → hör gärna av dig · låt mig veta om tiden passar → säg till om tiden passar

Undantag: lån som Isof uttryckligen godtar står kvar. *Adressera* har
betydelsen 'väcka en fråga' och 'rikta fokus mot ett problem'
("adressera klimatproblemen"). *Spendera tid* passar in i svenskans
gamla mönster där tid behandlas som en tillgång och är inte säkert en
anglicism. *Göra en skillnad* är ett översättningslån från _make a
difference_ som Isof inte ser som ett problem, men som irriterar en
del läsare, och *göra skillnad* eller *göra nytta* undviker den
irritationen.

Underlag: Isofs Frågelåda om *adressera*, *spendera* och *göra
(en) skillnad*; regeln `svenska_fran_sakunderlaget` i paketet
`regler`. Vilka lån som stör är omstritt och skiftar med tiden, så
posten prövar läsningen och inte ordets ursprung. Exemplen som Isof inte har
besvarat är modulens omdömen.

### 4. Säljord och entusiasmord

Test: meningen konstaterar ett faktum som läsaren kan kontrollera.
"Fantastisk", "otroligt spännande", "banbrytande", "sömlös",
"skräddarsydd lösning", "vi är stolta över att kunna erbjuda" och
"brinner för" försöker flytta läsaren, och på svenska hörs de lätt som
reklam eller översättning.

Undvik (illustrativt):

> Vi är otroligt stolta över att kunna erbjuda en banbrytande och sömlös lösning för er fakturahantering.

Bättre (illustrativt):

> Tjänsten läser fakturor i de format era leverantörer redan skickar.

Undantag: en superlativ som är belagd och anger sitt belägg, och ett
citat som återges ordagrant.

Underlag: det konstaterande registret i `tone_and_register` (modulen
`writing`); det återhållsamma registret i paketet `mottagaren`, där
också osäkerheten i underlaget står; förbudet mot entusiasmord i
`svenska_ansokningar` (profilen `jobbansokan`).

### 5. Garderingsstaplar

Test: varje förbehåll motsvarar en verklig osäkerhet, och den står en
gång där den gäller. Staplade förbehåll som "kan potentiellt",
"skulle eventuellt kunna", "i viss mån" och "på sätt och vis" sänker ett
korrekt påstående utan att göra det sannare.

Undvik (illustrativt):

> Lösningen skulle potentiellt kunna bidra till att i viss mån minska den manuella hanteringen.

Bättre (illustrativt):

> I piloten minskade den manuella hanteringen med en fjärdedel.

Undantag: en osäkerhet som läsaren behöver känna till, sagd en gång
och med sin grund ("Siffran bygger på tre månaders data").

Underlag: kalibreringen i skrivmodulens paket `claims`; avsnittet om
gardering i `svenska_ansokningar` (profilen `jobbansokan`).

### 6. Den sammanfattande slutraden

Test: sista stycket tillför något som inte redan står i texten.
"Sammanfattningsvis …", "Allt som allt …", "I slutändan handlar det om …" och "Hoppas att detta
ger en bra överblick!" upprepar det läsaren just läst.

Undantag: en längre text som inleds med en sammanfattning, så som
_Myndigheternas skrivregler_ råder (avsnitt 1.5), och en rapport vars
slutsatser läses fristående.

Underlag: `redundancy` (modulen `writing`, profilen `core`, paketet
`basics`); [myndigheternas_skrivregler.md](../../regler/reference/myndigheternas_skrivregler.md).

## Mejlmallen och tilltalet

### 7. Mallhälsningen

Test: hälsning och avslutning passar relationen och meddelandet, och
varje rad före sakinnehållet säger något till just den här läsaren.
Mallen känns igen på staplade artighetsfraser ("Jag hoppas att allt är
bra med dig!", "Tack så mycket för ditt mejl!", "Hoppas att detta var
till hjälp!", "Tveka inte att höra av dig om du har några frågor"), på
ett *Kära* till någon skribenten inte känner, där engelskans _Dear_ har
förts över, och på en namnplats som står ofylld ("Hej [förnamn]!").

Undvik (illustrativt):

> Hej Anna!
>
> Jag hoppas att allt är bra med dig! Tack så mycket för ditt mejl. Mötet flyttas till torsdag kl. 10. Hoppas att detta var till hjälp, och tveka inte att höra av dig om du har några frågor!

Bättre (illustrativt):

> Hej Anna!
>
> Mötet flyttas till torsdag kl. 10, i samma lokal.

Isof ger inga strikta regler för hälsningen. Utropstecken efter
hälsningsordet, följt av stor bokstav, är det vanligaste, och en
hälsning utan skiljetecken är ett alternativ när utropstecknet känns
hurtigt. Kommatecken efter hälsningen har blivit vanligare under
påverkan från andra språk och följs då helst av liten bokstav, medan
komma följt av stor bokstav följer engelsk förebild. Skiljetecknet är
alltså ingen markör i sig, och skribentens stilpreferens avgör enligt
profilen `korrespondens`.

Undantag: innekretsregistret i profilen `korrespondens`, där en varm
första kontakt får utropstecken och en ledig avslutning.

Underlag: Isofs Frågelåda om hälsningsfraser; Isofs råd att hälsa och
tacka, i paketet `mottagaren`. Artighetsfraserna som mallmarkör är en
iakttagelse.

### 8. Versalt Du och Ni

Test: tilltalsordet skrivs med gemen. Isof avråder från versalt *Du*,
som vissa läsare uppfattar som insmickrande och andra som
avståndstagande.

Undantag: privata brev, där skribenten skriver som hen vill.

Underlag: Isofs Frågelåda om *du* och *ni*; paketet `mottagaren`.

### 9. Den avsändarlösa texten

Test: läsaren kan se vem som beslutar, gör och svarar. En text där
ingen avsändare syns, med passiv, *man* eller abstrakta subjekt där
organisationen eller skribenten handlar, läses som skriven av ingen.

Undvik (illustrativt):

> Ansökan kommer att behandlas och beslut kommer att fattas inom fyra veckor.

Bättre (illustrativt):

> Vi behandlar din ansökan och fattar beslut inom fyra veckor.

Undantag: aktören är okänd eller ovidkommande för läsaren, och avtal
där parterna har definierade benämningar enligt profilen
`affarsdokument`.

Underlag: Isofs råd om *vi* och *jag*; en kandidatuppsats (Lunds
universitet 2024) där vi-perspektivet saknades i de maskinella
omskrivningarna, ett litet underlag som redovisas i paketet
`mottagaren`.

## Form och typografi

### 10. Engelsk versalisering

Test: varje versal efter meningens första ord står i ett namn.
Rubriker skrivs med gemener, så en rubrik i engelsk titelform med
versal i varje ord är fel. Detsamma gäller versal på veckodagar,
månader, språk och nationaliteter.

Undvik → bättre (illustrativt):

> Så Bygger Vi En Hållbar Plattform → Så bygger vi en hållbar plattform · Måndag 3 Mars → måndag 3 mars · för Svenska kunder → för svenska kunder

Undantag: namn, och varumärken och myndigheter som stavar sitt namn på
eget sätt, enligt [versaler.md](../../regler/rules/versaler.md).

Underlag: _Myndigheternas skrivregler_ 3.5.2 och _Snabba skrivregler_
§2.2, digesterade i paketet `regler`.

### 11. Em-strecket och tankstrecksfrossan

Test: strecktestet i [skiljetecken.md](../../regler/rules/skiljetecken.md).
Det engelska em-strecket (—) är alltid fel tecken i svensk text, och
flera tankstreck i samma stycke betyder oftast att strecken står i
stället för meningsbyggnad.

Undantag: ett tankstreck som klarar strecktestet.

Underlag: _Snabba skrivregler_ §1.10 och kärnprofilens regel
`skiljetecken`.

### 12. Engelsk typografi

Test: siffror, datum, klockslag, citattecken och genitiv följer svensk
form. Engelska mönster som "Volvo's", decimalpunkt ("3.5"), "kl 14:30",
procent utan mellanslag ("10%"), olika citattecken i början och slutet
(“så här”) och kommatecken före *och* i en uppräkning hör inte hemma i
svensk löptext.

Undvik → bättre (illustrativt):

> Volvo's → Volvos · 3.5 % → 3,5 % · kl 14:30 → kl. 14.30 · 10% → 10 % · “så här” → ”så här” · mössa, vantar, och halsduk → mössa, vantar och halsduk

Undantag: maskinfält, kod och frontmatter, där ISO-former och
maskinläsbara format gäller.

Underlag: _Snabba skrivregler_ §1.6, §1.13, §1.14, §1.16 och §5.2;
paketet `former` och digesten i paketet `regler`.

### 13. Särskrivning och engelska sammansättningsmönster

Test: varje sammansättning skrivs ihop, och ett led som är en
förkortning, en siffra eller ett engelskt flerordsuttryck binds med
bindestreck. Ett engelskt substantivpar som förs över ord för ord
särskrivs ofta.

Undvik → bättre (illustrativt):

> kund resa → kundresa · AI baserad lösning → AI-baserad lösning · data driven styrning → datadriven styrning · real time data → realtidsdata

Undantag: fasta uttryck som skrivs isär (*i natt*, *i år*), och fall där
den isärskrivna formen bär den betydelse som avses.

Underlag: _Snabba skrivregler_ §3.1 och §3.3; kärnprofilens regel
[sammansattningar.md](../../regler/rules/sammansattningar.md).

## Meningsbyggnad och register

### 14. Kontrast för effekt

Test: läsaren tror faktiskt det som meningen förnekar. De svenska
formerna är "det handlar inte om X, utan om Y", "inte bara X, utan även
Y" och "X är inget tillägg. Det är grunden."

Undvik (illustrativt):

> Det handlar inte om teknik, utan om människor.

Bättre (illustrativt):

> Projektet börjar med intervjuer med dem som hanterar fakturorna i dag.

Undantag: en missuppfattning som läsaren verkligen har.

Underlag: skrivmodulens katalog (`catalogue`, post 4).

### 15. Annonseringen

Test: meningen säger saken i stället för att meddela att den kommer.
"Det som gör X intressant är …", "Här är grejen:", "Kort sagt:" och
"Spoiler:" annonserar ett påstående som kunde ha stått direkt.

Undvik (illustrativt):

> Det som gör lösningen unik är att den lär sig av varje faktura.

Bättre (illustrativt):

> Lösningen lär sig av varje faktura som en handläggare rättar.

Undantag: den svenska utbrytningen (*det var styrelsen som beslutade*)
är en vanlig fokuskonstruktion och ingen markör, eftersom den pekar ut
ett enskilt led i stället för att annonsera ett helt påstående.

Underlag: avsnittet om mallrösten i `tone_and_register` (modulen
`writing`); kolonregeln i kärnprofilens regel `skiljetecken`.

### 16. Subjektet först i varje mening

Test: i ett stycke där nästan varje mening börjar med subjektet prövas
om en tids-, plats- eller sambandsbestämning hellre står först, där den
knyter an till föregående mening. Svenskan låter ett annat led än
subjektet inleda meningen, och den möjligheten binder samman
meningarna.

Undvik (illustrativt):

> Vi lanserade tjänsten i mars. Vi fick in 200 ansökningar den första veckan. Vi behövde därför fler handläggare.

Bättre (illustrativt):

> Vi lanserade tjänsten i mars. Redan den första veckan kom 200 ansökningar in, och därför behövde vi fler handläggare.

Undantag: instruktioner och steglistor, där en fast form hjälper
läsaren.

Underlag: kärnprofilens regel [kommakedjor_och_rytm.md](../../regler/rules/kommakedjor_och_rytm.md);
subjektsinledd monotoni som markör för maskinsvenska är en iakttagelse
från praktiker, inte en undersökt frekvens.

### 17. Kanslisvenskan

Test: varje ord är det vanligaste som säger saken. Stela ord som
*erhålla*, *föreligga* och *nyttja*, och nominaliseringar som
"genomföra en utvärdering av", gör texten tyngre utan att göra den
exaktare. Maskinsvenskan pendlar ofta mellan den här stelheten och
säljtonen i post 4.

Undvik → bättre (illustrativt):

> erhålla → få · föreligga → finnas · nyttja → använda · vidta erforderliga åtgärder → vidta de åtgärder som behövs · genomföra en utvärdering av → utvärdera · Det kan konstateras att kostnaden ökade → Kostnaden ökade

Undantag: juridiska termer som måste stå kvar, och definierade termer i
avtal. Svarta listan betonar själv att den inte är en lista över
förbjudna ord.

Underlag: Regeringskansliets _Svarta listan_ (SB PM 2011:1, fjärde
upplagan), som föreslår *få* för *erhålla*, *finnas* för
*föreligga*, *använda* för *nyttja* och en omskrivning av *vidta
erforderliga åtgärder*; Isofs råd att en
myndighet inte behöver låta som en byråkratisk robot, i paketet
`mottagaren`.

### 18. Utropstecken och emojier i extern text

Test: tecknet bär en känsla som relationen och kanalen redan rymmer.
Utropstecken används sparsamt och aldrig flera i rad i jobbtext, och
emojier är inte självklara i externa mejl och mycket sällsynta i
myndighetstext.

Undantag: chatt, sociala medier och innekretsregistrets hälsning.

Underlag: _Snabba skrivregler_ §1.5; Isofs Frågelåda om emojier.

## Det katalogen inte fångar

En text kan klara alla poster och ändå inte vara avsändarens. Testet
för det är om avsändaren står för varje uppgift och varje mening, och
det står i paketet `mottagaren` och i skrivmodulens paket `integrity`.
Katalogen används för att skriva bättre till läsaren. Den är ingen
metod för att få en text att se mänskligt skriven ut.

## Källor

- https://frageladan.isof.se/faqs/29280 — Isofs Frågelåda: hur verbet *adressera* används; hämtad 2026-11-23.
- https://frageladan.isof.se/faqs/21783 — Isofs Frågelåda: *spendera* om tid; hämtad 2026-11-23.
- https://frageladan.isof.se/faqs/19851 — Isofs Frågelåda: *göra skillnad* och *göra en skillnad*, översättningslån från _make a difference_; hämtad 2026-11-23.
- https://frageladan.isof.se/faqs/21183 — Isofs Frågelåda: hur ett brev eller mejl inleds, skiljetecken efter hälsningsfrasen; hämtad 2026-11-23.
- https://frageladan.isof.se/faqs/21774 — Isofs Frågelåda: *du* med liten bokstav; hämtad 2026-11-23.
- https://frageladan.isof.se/faqs/30864 — Isofs Frågelåda: när emojier används; hämtad 2026-11-23.
- https://www.regeringen.se/rapporter/2011/10/pm-20111/ — Statsrådsberedningen, _Svarta listan – ord och fraser som kan ersättas i författningsspråk_, SB PM 2011:1 (fjärde upplagan, publicerad 1 oktober 2011, sidan uppdaterad 2 april 2015); hämtad 2026-11-23.
- https://www.isof.se/svenska-spraket/klarsprak/klarsprakshjalpen/skriv-klarsprak/tank-pa-dina-lasare/fordjupning-tank-pa-dina-lasare/anpassa-tonen-efter-sammanhanget — Isof, Anpassa tonen efter sammanhanget (uppdaterad 18 maj 2022); hämtad 2026-11-23.
- https://lup.lub.lu.se/student-papers/search/publication/9159126 — Zarah Lundberg, "Kan Chat GPT klarspråksanpassa text? Svaret är ja." (kandidatuppsats, Lunds universitet, 2024); hämtad 2026-11-23.
- https://erigo.se/sv/artiklar/skriver-din-kollega-eller-ar-det-chatgpt-och-spelar-det-nagon-roll — Katri Lindgren, "Skriver din kollega, eller är det ChatGPT" (Erigo, 27 april 2026, uppdaterad 15 november 2026); praktikers markörer för AI-skriven svenska utan egen empiri, underlag för iakttagelserna i post 2, 5, 6, 7, 11, 14 och 15; hämtad 2026-11-23.
- https://github.com/Trifocals7733/humanizer-svenska — humanizer-svenska (version 4.1.0, MIT), en öppen förteckning över mönster i AI-skriven svensk text utan forskningsunderlag; underlag för iakttagelserna i post 1, 3, 4, 9, 12, 16 och 17; hämtad 2026-11-23.
- _Snabba skrivregler_ (Isof 2024) och _Myndigheternas skrivregler_ (Språkrådet 2014) citeras med avsnittsnummer; bibliografin står i profilens `sources/` och digesterna i paketet `regler`.
