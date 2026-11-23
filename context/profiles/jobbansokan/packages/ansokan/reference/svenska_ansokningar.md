# Svenska jobbansökningar

Filen lägger till det som gäller svenska personliga brev och arbetslivsbeskrivningar ovanpå genreprinciperna i `claims_in_applications` (modulen `writing`, profilen `job_application`, paketet `letters`), `cover_letter` (modulen `writing`, profilen `job_application`, paketet `letters`) och `cv_entries` (modulen `writing`, profilen `job_application`, paketet `cv`). Den svenska språkmekaniken och Isofs och Språkrådets skrivregler finns i den här modulens kärnprofil (`core`) och upprepas inte här. Brevets fyra stycken står i [personligt_brev_struktur.md](personligt_brev_struktur.md).

## Motivationen bär brevet

Ett personligt brev, en intressetext, ett "varför söker du"-fält eller ett meddelande till en arbetsgivare bärs av verkliga skäl att vilja vara där — organisationen eller produkten, ett område sökanden vill växa i, ett arbete sökanden särskilt tycker om och som utgör en stor del av rollen, valet av den sortens organisation — aldrig av en cv-återberättelse av varför sökanden är kvalificerad ("rollen beskriver det jag redan gör"). Motivationen är sann: den är förankrad i sökandens faktiska karriärriktning och i kontrollerbara fakta om arbetsgivaren, och ett skäl utan källa föreslås för bekräftelse. Det första stycket är motivationen; huvudexemplet följer och stöder den.

Att bevisa lämplighet genom att återberätta CV:t är aldrig textens centrum eller inledning. Inledningar av följande slag är förbjudna (illustrativt):

> Rollen beskriver det jag redan gör.

> Jag har relevant erfarenhet av …, vilket gör mig till en bra match för tjänsten.

Bättre (illustrativt):

> Jag söker mig till ett produktbolag, och ert verktyg för schemaläggning är en produkt jag gärna vill vara med och utveckla. Annonsen nämner integrationsarbete, och det är den sortens arbete jag tycker mest om.

En kort, övergripande hänvisning till bakgrunden är tillåten i stödjande roll, men aldrig som skälet till att söka. Testet är att stryka varje mening vars uppgift är att visa att sökanden kvalificerar sig. Det som återstår ska fortfarande säga varför sökanden vill ha just den här rollen här. Engagemang visas genom konkreta skäl och aldrig genom entusiasmord som "brinner för", "passionerad" eller "drömjobb".

### Ett område är inget skäl

Att nämna ett område är inget skäl. "Plattformar och informationsflöden är det jag vill fördjupa mig i" pekar ut en domän men säger inte varför. Texten ska säga vad i området som är intressant eller stimulerande för sökanden personligen, kopplat till erfarenheter och personlig strävan. Testet är om läsaren efter meningen kan svara på "varför spelar det roll för sökanden?" utifrån texten. Kan läsaren inte det behöver meningen det personliga skälet, som hämtas ur sakunderlaget om sökanden och följer samma ärlighetskrav som all motivation.

Svagt (illustrativt):

> Plattformar och informationsflöden är delar av utvecklingsarbetet som jag gärna vill fördjupa mig i.

Starkare (illustrativt, och skälet måste finnas i sakunderlaget):

> Jag tycker om att förstå hur ett helt system hänger ihop, från data in till det som användarna ser. En plattform som flera team bygger på är ett ställe där den förståelsen gör skillnad.

### Ödmjukhet mot rollen

Annonsen ger en riktning, och arbetsuppgifterna i den är exempel. Arbetet förändras över tid, och sökanden kan inte veta av annonstexten vad rollen faktiskt kommer att innehålla eller hur organisationen runt den ser ut. Därför återger texten inte annonsens uppgifter och upplägg som fakta om rollen, och den påstår ingenting om organisationen eller rollen som sökanden inte kan veta eller kontrollera. Konstaterande meningar av typen "X är Y" om arbetsgivaren eller arbetet undviks. Texten skrivs utifrån sökandens egna önskemål, nyfikenhet och erfarenheter och får vara trevande där den rör arbetsgivaren ("jag föreställer mig", "jag skulle gärna vilja förstå").

Förbjudna mönster (illustrativt):

> I den här rollen står plattformen mellan Data Scientists, en lösningsarkitekt och IT.

> Rollen är till stor del det arbetet.

Bättre (illustrativt):

> Jag skulle gärna vilja förstå hur en AI-tjänst går från idé till drift hos en organisation där så många är beroende av datan.

Kontrollerbara offentliga fakta om organisationen får användas sparsamt och bara där de bär motivationen. Ett faktum som bara visar att sökanden har läst annonsen eller webbplatsen stryks.

### Precision och proportion i hänvisningar till bakgrunden

En hänvisning till bakgrunden ska säga något som läsaren begriper och som betyder något i sammanhanget, annars stryks den. Vaga omfångsfraser blandade med detaljer som inte spelar roll är förbjudna, till exempel verktygsuppräkningar och fraser som "från Terraform till övervakning". En konkret mening räcker, och i en kort motivationstext nämns bakgrunden högst en gång.

Svagt (illustrativt):

> Vid sidan av anställningen har jag byggt och driftar en egen AI-tjänst i molnet från Terraform till övervakning.

Starkare (illustrativt, och faktat måste finnas i sakunderlaget):

> Mycket av arbetet med en tjänst börjar först när den är lanserad. Det har jag sett i de AI-assistenter som jag ofta bygger och driftar.

Hänvisningar till bakgrunden hålls proportionerliga. Ett enskilt sidoprojekt eller en demo lyfts aldrig upp till en fristående prestation som bär stycket, och inramningar som "på egen hand" eller "vid sidan av anställningen" är förbjudna där de blåser upp omfånget. Det som sökanden gör ofta beskrivs som vardag, kort och allmänt. Ett visningsprojekt hör hemma i CV:t, där dess teknikstack är relevant, och inte i motivationstexten.

## Rubrik och ram

Rubriken på ett personligt brev är rollkopplad — "Ansökan – <roll>" — och en generisk hälsningsfras som rubrik klarar inte rollkopplingen. Brevet ramas in av "Hej [förnamn]" och "Vänliga hälsningar" enligt svensk språkmekanik.

## Stoltheten som ankare

Ett kort ansökningsmejl får inleda med det bygge sökanden är mest stolt över ("Det system jag är mest stolt över är …", illustrativt), enligt `cover_letter` (modulen `writing`, profilen `job_application`, paketet `letters`). Meningen står kvar och ersätts inte av en neutral platshållare som "ett relevant exempel". Ankaret är en insats och ingen kvalifikationsuppräkning, så det följs av varför den sortens arbete drar sökanden till rollen och aldrig av en lista över hur det matchar annonsen.

## Tempus och rubriker i CV:t

Preteritum för avslutade roller, presens för den nuvarande. En rubrik över ansvarsområden heter "Huvudansvar" eller "Huvudsakliga ansvarsområden"; "Nyckelansvarsområden" är en kalk på engelskans "Key Responsibilities" och används inte, jämför rubrikregeln i `cv_entries` (modulen `writing`, profilen `job_application`, paketet `cv`).

## Teknikstödlista

En teknikstack får stå som en stödlista i anslutning till posten den hör till, till exempel "Teknik: Go, TypeScript, PostgreSQL." Listan är det genuint listlika innehåll som katalogens post 1 tillåter, och den presenteras av en mening eller av det sammanhang den står i.

## Gardering och överföring

Garderingsmedel stryks i stället för att behållas: staplade "skulle nog / verkar"-markörer och mynt som "erfarenhetsbank" sänker ett korrekt påstående utan att göra det sannare, enligt kalibreringsregeln i den allmänna anspråksdoktrinen. En överföring till tjänstens krav namnger de specifika överförbara arbetsmomenten; en garderad likvärdighet ("i stort sett liknande arbete") är för vid, per `claims_in_applications` (modulen `writing`, profilen `job_application`, paketet `letters`).

## Relevansövergångar

Slutkontrollen stryker varje "det är precis det ni söker"-mening. Faller resonemanget samman när meningen är borta ligger felet i exemplet eller i anspråkets omfattning, och det är där rättelsen görs, enligt borttagningstestet i `claims_in_applications` (modulen `writing`, profilen `job_application`, paketet `letters`).

## Maskinsvenska och det återhållsamma registret

Ett personligt brev läses som sökandens egen röst, och en rekryterare som känner igen mallen läser resten av brevet med den misstanken. Brevet prövas därför mot katalogen i paketet `maskinsvenska` (modulen `writing_sv`, profilen `core`) före kvalitetsporten, särskilt posterna 3 om ord-för-ord-lån, 4 om säljord och 5 om garderingar. Det återhållsamma svenska registret, och hur omstritt underlaget för det är, står i paketet `mottagaren` i samma profil. För brevet räcker att engagemang visas med konkreta skäl, som avsnittet om motivationen ovan redan kräver.

Ett brev som en språkmodell har hjälpt till med blir sökandens eget när varje mening är en som sökanden kan säga och förklara i en intervju och varje uppgift går att belägga enligt [claims_med_stod.md](../rules/claims_med_stod.md). Ramen "Hej [förnamn]" gäller när namnet är känt, och en namnplats som står ofylld är en mallmarkör (post 7). När namnet saknas följer brevet råden om okänd mottagare i profilen `korrespondens`.

## Språkval

Brevet skrivs på svenska när svenska är naturligt och rollen kräver det; annars på engelska, som väljs hellre än maskinöversatt svenska. Valet görs en gång per brev och hela brevet följer det.


## Påståenden och kvalitetsporten

Fördjupning till regeln [claims_med_stod.md](../rules/claims_med_stod.md). Svensk ansökningstext går igenom skrivmodulens kvalitetsport (`quality_gate` i modulen `writing`, profilen `core`, paketet `process`).

Ett exempel har ett huvudjobb: problemet, ditt beslut, resultatet. Detaljer och resultat väljs efter belagd förmåga, och mekanismen beskrivs före kvalitetsbeskrivningen – *hur* är kontrollerbart, *kvalitativ* är bara ett ord. Det stabila sakunderlaget är grunden varje text väljer ur; en text väljer, men omtolkar den aldrig.

Kvalitetsporten är den stående engångsporten för utåtriktad prosa. Den kan bära en stopplista med de påståendeformer som aldrig får stå, som examensmeriter som inte är avlagda, påhittade kvantifieringar, tidsinflation och ostödda universalpåståenden. Utöver stopplistan bär den en samling principutlösare som pekar tillbaka på påståendereglerna. En ren körning av en lista rensar aldrig en omdömesregel: stopplistan fångar de mekaniska felen, men omdömet – är påståendet faktiskt, relevant och sägbart? – är granskarens. Bevisbördan ligger på den som vill ändra något, och ändamålsbarren står kvar tills något konkret tränger undan dem. Det färdiga utkastet läses om mot porten och mot borttagningstestet i `claims_in_applications`. Varje fynd åtgärdas eller erkänns innan texten släpps.
