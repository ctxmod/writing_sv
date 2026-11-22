# Myndigheternas skrivregler: digest av avsnitt 1.5 och 3.5

Ett urval ur Språkrådets _Myndigheternas skrivregler_: de två avsnitt som handlar om att göra en längre text överskådlig, med sammanfattning, rubriker och röd tråd. Boken skrevs för myndigheter, kommuner och annan offentlig verksamhet, men råden om sammanfattningar och rubriker gäller all längre sakprosa. Basprofilens modell och [snabba_skrivregler_digest.md](snabba_skrivregler_digest.md) gäller vid sidan av digesten. Hur råden förhåller sig till skrivmodulens katalog står i avsnittet [Förhållande till skrivmodulens katalog](#förhållande-till-skrivmodulens-katalog) sist i filen.

## Källa

- Titel: _Myndigheternas skrivregler_, åttonde upplagan. Utgivare: Språkrådet och Norstedts Juridik AB/Fritzes, 2014. ISBN 978-91-38-32625-1.
- Upplaga: den åttonde, från 2014, är den upplaga som Isofs vägledningssida länkar som gratis-pdf (sidan uppdaterad 26 januari 2026), och pdf:ens egen tryckort anger "8 upplagan". En nionde upplaga (2023) kunde inte beläggas: varken Isofs sida eller sökningen 2026-10-17 visade någon, så digesten bygger på den åttonde.
- Isofs sida: <https://www.isof.se/utforska/vagledningar/myndigheternas-skrivregler>.
- Källfil: <https://sprakochfolkminnen.diva-portal.org/smash/get/diva2:1136028/FULLTEXT02.pdf>. DiVA svarade inte från värden, så filen hämtades 2026-10-17 via Wayback Machine-kopian `https://web.archive.org/web/20260224152843id_/https://sprakochfolkminnen.diva-portal.org/smash/get/diva2:1136028/FULLTEXT02.pdf`, med SHA-256 `92cd871dcb7b8d2c0f3cde798b8866fc285c1857ce135ec2b0e555ee11d23141`.
- Kontroll: texten i avsnitt 1.5 och 3.5 lästes med två oberoende extraktioner av samma fil, och de stämde överens.
- Villkor: tryckorten säger "© 2014 Språkrådet och Norstedts Juridik AB/Fritzes" och förbjuder mångfaldigande utan medgivande från förlaget. Därför återger digesten råden med egna ord och citerar bara korta formuleringar. Boken finns inte i fulltext någonstans i modulen; bibliografin står i profilens källa `myndigheternas_skrivregler` (`sources/myndigheternas_skrivregler.yaml` i profilen `core`).

Hänvisningarna nedan, till exempel (1.5.3), avser bokens avsnittsnummer; sidnumren är de tryckta.

## Avsnitt 1.5: Gör texten överskådlig (s. 25–27)

Avsnittet utgår från att en text ofta har flera läsargrupper och att inte alla behöver läsa allt. Läsaren ska därför snabbt kunna få överblick och hitta det hon behöver. Informativa rubriker hjälper, och i längre texter även en innehållsförteckning. Huvudbudskapet kan lyftas fram redan i rubriken eller placeras i början av texten (1.5).

I texter som är längre än några sidor behöver läsaren, enligt boken, anvisningar om hur texten är uppbyggd och vad den innehåller i stort. Boken föreslår uttryck som "i nästa avsnitt", "i bilaga 1" och "avslutningsvis", och varnar för vaga hänvisningar som "nedan", "som presenterats ovan" och "i det följande" (1.5). Hur rådet förhåller sig till katalogens poster om metapåståenden står sist i filen.

Den grafiska formen påverkar hur lätt texten är att ta till sig: tillräckliga marginaler, luft på sidan, radavstånd, radlängd, typsnitt och teckenstorlek, och stycken av lagom längd. Bilder, punktuppställningar och figurer skapar också luft (1.5.1).

Rubrikerna ska sammanfatta vad som står i textens olika delar, väcka intresse och visa hur texten är disponerad. Med talande rubriker bildar rubrikerna tillsammans en sammanfattning av texten. Ämnesord som "Historik", "Metod" och "Undersökning" räknar boken som föga informativa; en informativ rubrik berättar vad som sägs eller händer i texten, och innehåller därför gärna ett verb. Bokens exempel ställer ämnesordet mot rubriken som bär budskapet: "Vargjakt" mot "Naturvårdsverket ger klartecken för vargjakt i vinter" (1.5.2).

### 1.5.3 Sammanfatta det viktigaste

En längre text bör alltid ha en sammanfattning. Enligt boken ska en bra sammanfattning "stå först, innehålla det viktigaste och vara kort". Eftersom många kanske bara läser sammanfattningen ska den också kunna läsas oberoende av huvudtexten. Utöver en sammanfattning av hela texten kan innehållet i kapitel och avsnitt sammanfattas var för sig, så som boken själv gör i början av varje kapitel (1.5.3).

Rådet stöder skrivmodulens helhet-till-detalj-modell (`whole_to_detail` i modulen `writing`): det viktigaste kommer först, och sammanfattningen ger läsaren ramen innan detaljerna. Modellen citerar avsnittet bland sina källor i `whole_to_detail` (modulen `writing`, profilen `core`, paketet `whole_to_detail`). Kravet att sammanfattningen ska kunna läsas för sig motsvarar granskningstestets fråga på dokumentnivå i `review_test` (modulen `writing`, profilen `core`, paketet `whole_to_detail`).

### Punktuppställningar och röd tråd

Punktuppställningar och faktarutor delar upp texten grafiskt och framhäver viktig information. Boken föreslår en punktuppställning när viss information ska framhävas, eller när en mening blir lång för att den innehåller flera villkor eller uppräkningar (1.5.4). När innehållet alls hör hemma i en lista avgörs av skrivmodulens antimönsterkatalog, post 1, i `catalogue` (modulen `writing`, profilen `core`, paketet `anti_patterns`).

Den röda tråden byggs genom att huvudtanken anges och ämnet avgränsas tidigt, "gärna allra först", och genom en logisk disposition med ett genomgående tema. Sambandsord visar hur meningar och stycken hänger ihop, och boken grupperar dem efter funktion: tillägg (också, dessutom), tid (sedan, därefter), motsats (men, däremot, trots att), villkor (om, ifall), följd (så att, alltså, följaktligen) och avsikt (för att, i syfte att). Det som hör ihop samlas i samma stycke, som gärna inleds med en sammanfattande mening som lyfter fram det viktiga med ett nyckelord. Nyckelordet kan sedan upprepas exakt eller i ändrad form. Samband skapas också med ord som hör ihop (tabeller och diagram blir figurer), med pronomen och med adverb som syftar tillbaka (1.5.5).

Rådet om huvudtanken först ligger nära modellens "huvudtanke före utveckling". Ämnesmeningens plats i stycket får variera, så länge läsaren har ramen innan detaljerna kommer, enligt modellens förfiningar i `whole_to_detail` (modulen `writing`, profilen `core`).

## Avsnitt 3.5: Rubriker ger struktur åt innehållet (s. 38–40)

Rubriker har två funktioner: de upplyser om innehållet och visar hur texten är disponerad, så att läsaren får överblick (3.5).

### Rubriknivåer och utseende

En text på två sidor eller mer behöver i regel både huvudrubrik och mellanrubriker, och ibland underrubriker. Numrerade rubriker hålls till högst tre nivåer; ett par onumrerade nivåer kan läggas till, men de tas i regel inte med i innehållsförteckningen (3.5.1).

En rubrik ska skilja sig tydligt från löptexten. En lång rubrik delas hellre på två rader än sträcks över hela sidans bredd. Rubriker skrivs med gemener och avstavas inte. En rubrik avslutas aldrig med punkt eller kolon, utom att en punktuppställning kan ha kolon i sin rubrik. Efter en frågerubrik sätter boken frågetecken, och utropstecken i förekommande fall. Rubriker är inte understrukna. Boken ger teckengrader per nivå, från 20–24 punkter för huvudrubriken ned till löptextens storlek på fjärde nivån (3.5.2). Hur frågerubriker förhåller sig till skrivmodulens katalog står sist i filen.

### Huvudrubriken och ärendemeningen

Huvudrubriken talar om vad texten handlar om och är helst kort och kärnfull. En tvåledad rubrik kan ange huvudtiteln på den övre raden och beskriva innehållet på den undre. När rubriken delas i huvudrubrik och underrubrik kan ett tankstreck stå mellan dem, och står underrubriken på egen rad flyttas tankstrecket dit, som i "Köpta relationer – om korruption i det kommunala Sverige" (3.5.3). Det stämmer med tankstrecksformen i [skiljetecken.md](../rules/skiljetecken.md).

I förvaltningsbeslut och andra formella brev heter huvudrubriken ärendemening. Den inleds aldrig med "angående", "beträffande" eller liknande, utan går rakt på sak: "Din begäran att få ta del av uppgifter i belastningsregistret". En lång ärendemening kan delas i två led med tankstreck (3.5.4).

### Mellan- och underrubriker

Mellan- och underrubriker ska vara informativa och beskriva innehållet i styckena som följer. De berättar vad som sägs eller händer i texten, använder nyckelord ur texten och innehåller gärna verb, som i "Anpassa översättningen språkligt och innehållsligt". En underrubrik står närmast det stycke den hör till. Den första meningen efter en rubrik får inte vara en fortsättning på rubriken (3.5.5); samma regel står hos Isof (51).

I rapporter, kataloger och handböcker kan kapitelrubriken upprepas i sidhuvudet eller sidfoten som kolumntitel (3.5.6).

Rådet om informativa rubriker med verb stöder katalogens post 9, där rubriken bär sitt budskap, och modellens krav på en ram före detaljerna.

## Det som digesten inte täcker

Digesten täcker avsnitt 1.5 (med 1.5.1–1.5.5) och 3.5 (med 3.5.1–3.5.6). Bokens övriga kapitel är inte digesterade: klarspråk i övrigt (1.1–1.4, 1.6), webben (2), text och form utanför 3.5, avstavning, stavning, böjning, ordbildning, ordval, stor och liten bokstav, hop- och särskrivning, förkortningar, sifferuttryck, skiljetecken, källhänvisningar och korrekturtecken (4–14). De låg utanför uppdraget. För de flesta av dem täcker [snabba_skrivregler_digest.md](snabba_skrivregler_digest.md) motsvarande regler ur _Snabba skrivregler_.

## Förhållande till skrivmodulens katalog

- Frågetecken sätts efter en frågerubrik (3.5.2), vilket förutsätter att frågerubriker används. Skrivmodulens antimönsterkatalog (post 9) gör frågerubriker sällsynta; där de ändå används behåller de frågetecknet.
- Läsanvisningar om hur en text längre än några sidor är uppbyggd och vad den innehåller i stort, med uttryck som "i nästa avsnitt" och "avslutningsvis" (1.5), är tillåtna sparsamt i långa texter. De ryms i undantaget i katalogens post 5 (metapåståenden, med undantag för korta läsanvisningar och en navigerande hänvisning till var uppskjuten detalj finns) och fäller inte post 10 (öppningar som bara deklarerar innehållet), så länge de orienterar läsaren i ämnet.
