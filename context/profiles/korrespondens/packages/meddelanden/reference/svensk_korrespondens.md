# Svensk korrespondens

Filen lägger till det som gäller svenska mejl, meddelanden, brev och svar ovanpå genreprinciperna i `message_doctrine` (modulen `writing`, profilen `correspondence`, paketet `message_doctrine`), `messages` (modulen `writing`, profilen `correspondence`, paketet `replies`) och `answer_at_asked_length` (modulen `writing`, profilen `correspondence`, paketet `application_answers`), som gäller oförändrade. Den svenska språkmekaniken, Isofs och Språkrådets skrivregler och säljregistertestet finns i den svenska profilen, `package` (modulen `writing_sv`, profilen `core`, paketet `regler`), och upprepas inte här.

## Inledningen ger poängen

Testet är detsamma som i `message_doctrine` (modulen `writing`, profilen `correspondence`, paketet `message_doctrine`) §2: ger första meningen syftet, svaret eller det viktigaste beskedet? Typiska svenska inledningar som inte klarar testet är "Jag skriver för att …", "Härmed önskar jag meddela …" och varje allmän upprepning av ämnet. De är exempel, inte en uttömmande förteckning; en uppvärmning som inte står här faller på samma sätt.

Alltför ceremoniellt (undvik):

> Härmed önskar jag meddela att projektet har slutförts.

Bättre:

> Projektet är nu klart, och nästa steg är att vi går igenom resultatet tillsammans.

Alltför trevande (undvik, illustrativt):

> Jag skriver för att höra om ni möjligen skulle kunna tänkas vara intresserade.

Bättre (illustrativt):

> Jag hör av mig om uppdraget som backendutvecklare, eftersom er schemaläggningsprodukt är en jag gärna vill vara med och bygga.

Ämnesraden säger vad avsändaren vill, till exempel "Intresse för en utvecklarroll hos er", och aldrig bara vilket område meddelandet rör. Gäller meddelandet en viss roll eller ett visst uppdrag framgår vilket; säger brödtexten bara "rollen" bär ämnesraden namnet. Regeln står i `messages` (modulen `writing`, profilen `correspondence`, paketet `replies`).

Kort mejl som leder med poängen (illustrativt):

> Hej Anna,
>
> Jag har gått igenom underlaget och ser två vägar framåt. Vill ni komma vidare snabbt rekommenderar jag alternativ 1, eftersom det kräver minst förändring i ert nuvarande flöde. Jag sammanställer gärna ett konkret förslag till torsdag.
>
> Vänliga hälsningar,
> Daniel

## Konkreta tider

När ett möte önskas föreslår meddelandet konkreta tider. Ett vagt spann lämnar planeringen till mottagaren.

Vagt (undvik):

> Jag är ganska ledig onsdag och torsdag, vad passar dig?

Konkret (bättre):

> Jag är ledig i dag kl. 15 eller 16 och i morgon eftermiddag, vad passar dig?

## Säg bara det som gagnar meddelandet

Proven i `messages` (modulen `writing`, profilen `correspondence`, paketet `replies`) gäller oförändrade. De svenska paren nedan är illustrativa; namn och företag är påhittade.

Utfylld med återgivning (undvik):

> Hej Sam, det låter bra alltihop, lönen, hybridupplägget och att få träffa teamledaren efter vårt samtal. Tar gärna det vidare. Jag är ledig i dag kl. 16.30 och i morgon eftermiddag, vad passar dig?

Nedskuren till bekräftelse och logistik (bättre):

> Hej Sam, det låter bra alltihop, tar gärna det vidare. Jag är ledig i dag kl. 16.30 och i morgon eftermiddag, vad passar dig?

Interna detaljer till en rekryterare man nyss träffat (undvik):

> Jag har jobbat deltid och planen var att gå upp till heltid, men avtalet skrevs aldrig under och ett par kunder drogs in.

Neutralt och sakligt (bättre):

> Ett par kunduppdrag drogs in och företaget kan behöva dra ner, så jag tittar på andra möjligheter.

Mottagarens pitch upprepad (undvik):

> Northwind låter genuint intressant, att bygga riktiga produktionssystem ovanpå röriga operativa flöden ligger nära det jag gör.

Bekräftar och går vidare (bättre):

> Northwind låter genuint intressant, och både AI-spåret och plattformsspåret ser ut att passa.

Ett beslut som försvarar sig (undvik):

> Jag vill helst inte sprida ut mig, så låt oss leda med A och återkomma till B om det inte blir något.

Sagt rakt (bättre):

> Låt oss fokusera på A och återkomma till B om det inte blir något.

Nästa omgång frågor påklistrad på ett riktningssättande meddelande (undvik):

> Jag tror vi kan parkera C. För A, kan du säga lönespannet och hur nästa steg ser ut? Tar gärna en teknisk intervju när det passar dem.

Meddelandet gör sitt enda jobb (bättre):

> Jag tror vi kan parkera C.

Matchningen uppräknad och det egna arbetet påtalat över ett bifogat CV (undvik):

> Tack för samtalet och informationen. Företaget ser ut som en bra match, rollen ligger nära det jag gör: bygga produktionssatta LLM- och RAG-system praktiskt, plus strategirådgivningen och affärssidan. Mitt CV är bifogat, anpassat för rollen. Tar gärna det vidare till ett samtal med de två rekryterande cheferna när det passar.

En lätt rad som låter CV:t bära innehållet (bättre):

> Tack för samtalet och för att du skickade detaljerna. Ser ut som en bra match och ligger nära det jag är ute efter. Mitt CV är bifogat; säg till om du hellre vill ha det på engelska.

## Hälsningar och register

Hälsning och avslutning följer skribentens egen stilpreferens där en sådan finns (ett personligt lager eller en husstil); annars ett neutralt par som "Hej …" och "Vänliga hälsningar". Ett meddelande till en personlig kontakt eller en kontakt via en gemensam bekant använder det par relationen faktiskt har, enligt `messages` (modulen `writing`, profilen `correspondence`, paketet `replies`). Hur ett svenskt säljutskick formuleras, inklusive dess talspråksnära register, står i skrivmodulens profil `sales_outbound` och i profilen `korrespondens`, paketet `saljutskick`.

I en varm notis eller en första kontakt via en gemensam bekant gäller innekretsregistret i `messages` (modulen `writing`, profilen `correspondence`, paketet `replies`). På svenska ser det ut så här:

- Den gemensamma kontakten nämns som kretsen nämner hen, med smeknamn där kretsen använder ett.
- Hälsningen får ha utropstecken ("Hej Maria!") och avslutningen är ledig ("Mvh" eller bara förnamnet). Det avviker från skribentens standardpar och gäller varma och referensbaserade första kontakter.
- Nedtonande ramar ("Några initiala frågor bara:") och naturliga verbval används hellre än stelare: "rekryterar ni" hellre än "söker ni", "brukar ni vara" hellre än "är ni".
- Erfarenhet i vardagsregister avrundas nedåt, aldrig uppåt: "sedan 2018" får bli "sedan ca 2018" (illustrativt). Den uppenbara aritmetiken får mötas av en enda bisats ("eftersom jag också har pluggat parallellt").
- Frågorna står som nakna rader, två eller tre, med mjuka habitualisformuleringar. En första notis frågar inte hur processen eller nästa steg ser ut, och företagsresearchen får en lätt rad ("Jag kikade lite på er hemsida och … låter spännande").

## Mallton och okänd mottagare

Ett svenskt mejl som inleds med staplade artighetsfraser och avslutas med "Tveka inte att höra av dig" läses som en mall. Prövningen står i katalogen i paketet `maskinsvenska` (modulen `writing_sv`, profilen `core`), i posterna 2, 3, 7 och 9, och Isofs råd att hälsa och tacka med en mening var står i paketet `mottagaren` i samma profil. Skiljetecknet efter hälsningen är ingen markör i sig. Isof beskriver utropstecken som det vanligaste valet, hälsning utan skiljetecken som ett alternativ när utropstecknet känns hurtigt och kommatecken som ett lån från andra språk som har blivit vanligt, och skribentens stilpreferens avgör enligt avsnittet ovan.

När mottagarens namn inte är känt överförs inte engelskans _To whom it may concern_ som "Till den det berör". Isof råder att i stället ringa in vem texten ska nå, med en funktion ("Till personalchefen", "Till säljansvarig") eller en rubrik som säger vad saken gäller, så att ingen behöver läsa hela texten för att avgöra vem den angår.

## Svar på en ställd fråga

Reglerna i `answer_at_asked_length` (modulen `writing`, profilen `correspondence`, paketet `application_answers`) gäller oförändrade för svar på svenska: svara på den fråga som ställdes, i den längd den ställdes i, och sluta där. Upprepa inte frågan, inled inte och sammanfatta inte. En verklig brist medges en gång, i det fält som frågar om den; samma brist medgiven igen i intilliggande fält är en ansökan som argumenterar mot sig själv. Korthet ger aldrig utrymme för överdrift: där ett kortare svar inte går att skriva sant skrivs det ärliga längre. Ett formulärsvar läses snabbt av någon som bara avgör om det ska bli ett samtal, och ett kort och konkret svar lämnar resonemanget till samtalet.

Överförklarat (undvik, illustrativt):

> Jag har arbetat med de här systemen sedan 2021, först i prototypform och sedan alltmer i produktion, även om den exakta gränsen beror något på vad som räknas som produktion.

En rad (bättre, illustrativt):

> Fem år, i produktion sedan 2021.

Fält om en viss teknik, besvarat med föregripande medgivande (undvik, illustrativt):

> Jag har byggt retrieval-pipelines i Python och TypeScript, men jag ska säga direkt att jag inte arbetat med just er vektordatabas, så det skulle krävas en viss upplärning.

Svarar på den fråga som ställdes (bättre, illustrativt):

> Jag har byggt produktionssatta retrieval-pipelines i Python och TypeScript.

Upprepar, inleder och sammanfattar (undvik, illustrativt):

> Vad gäller frågan om varför jag är intresserad av rollen: det som drar är kombinationen av reglerad data och tillämpad AI, ett område jag arbetat inom i flera år, och jag tror att den kombinationen är huvudskälet till att rollen lockar.

Börjar med svaret och slutar där (bättre, illustrativt):

> Tillämpad AI på reglerad data är det område jag helst vill växa inom, och er produkt för kliniskt beslutsstöd är där det arbetet görs på riktigt.

Ett fält som frågar varför sökanden är intresserad, varför hen söker eller vad som lockar med organisationen är en motivationsfråga och besvaras med motivation. Det kan vara organisationen, produkten eller uppdraget, uppskattat för något konkret, ett område sökanden vill växa i, en sorts arbete sökanden särskilt tycker om och som annonsen pekar mot, eller valet av just den sortens organisation. Att återberätta CV:t ("rollen matchar det jag redan gör", "jag har relevant erfarenhet av …") svarar på en annan fråga. Det är förbjudet som svarets centrum eller inledning och får bara förekomma som en kort stödjande bisats. Motivationen är sann och förankrad, och ett områdesnamn är inget skäl, enligt `svenska_ansokningar` (modulen `writing_sv`, profilen `jobbansokan`, paketet `ansokan`). Svaret påstår ingenting om organisationen eller rollen som sökanden inte kan veta eller kontrollera, och verktygslistor och omfångsfraser stryks.

## Källor

- https://frageladan.isof.se/faqs/21183 — Isofs Frågelåda: hur ett brev eller mejl inleds, skiljetecken efter hälsningsfrasen; hämtad 2026-11-23.
- https://frageladan.isof.se/faqs/24960 — Isofs Frågelåda: engelskans _to whom it may concern_ och att ringa in mottagaren; hämtad 2026-11-23.
