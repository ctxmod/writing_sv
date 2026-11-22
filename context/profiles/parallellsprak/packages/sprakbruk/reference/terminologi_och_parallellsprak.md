# Terminologi och parallellspråkighet: digest för sv↔en

Digesten är ett urval ur två Isof-publikationer, valt för det som spelar roll när en skribent eller en agent skriver svensk fackprosa, väljer mellan svenska och engelska termer eller översätter mellan språken. Den första är _Parallella fackspråk. Studentperspektiv på språk i högre utbildning_ (Malmström, Karlsson och Warnby, Rapporter från Språkrådet 23, Isof 2025), här kallad PF. Den andra är _Snabba skrivregler_ (Isof 2024), här kallad SR, för de regler som skiljer svenska från engelska.

Hänvisningarna anger rapportens avsnitt med rubrik och tryckta sidor (PF) respektive skrivreglernas avsnittsnummer (SR §1.6 och så vidare). Bibliografi och hämtningsuppgifter står i kärnprofilens källor `parallellsprak` och `skrivregler` (`sources/` i profilen `core`). Publikationerna är upphovsrättsskyddade (© Isof) och finns inte i fulltext i modulen; digesten citerar bara korta formuleringar.

PF är en enkätrapport om språk i högre utbildning. Det som följer är rapportens begrepp och slutsatser omsatta i skrivpraxis. Rapportens egna siffror och rekommendationer gäller lärosäten och citeras inte som regler för annan text. Det grundläggande hantverket, att båda riktningarna skrivs från sakunderlaget, står i `translation_principles` (modulen `writing`, profilen `translation`, paketet `principles`).

## Begrepp

Rapportens termlista (PF, avsnittet ”Termlista”, s. 4–5) ger definitionerna att använda:

| Term                       | Definition (PF, avsnittet ”Termlista”, s. 4–5)                                                                |
| -------------------------- | --------------------------------------------------------------------------------- |
| fackspråk                  | språkform som används för kommunikation inom ett särskilt ämnesområde             |
| term                       | benämning för ett begrepp som tillhör ett fackområde                              |
| terminologi                | uppsättning benämningar som hör till ett fackområde                               |
| parallellspråkighet        | samtidig användning av flera språk i ett visst sammanhang                         |
| språkpolicy / språkpolitik | riktlinjer för språkförhållanden / offentlig verksamhet som rör språkförhållanden |

Med parallellspråkighet menar rapporten en "klok", medveten och planerad användning av två eller flera språk inom samma område (PF, avsnittet ”Svenska, engelska och parallellspråkighet inom svensk högre utbildning”, s. 6–8, PF, avsnittet ”Mot en fungerande parallellspråkighet och svensk terminologi i praktiken”, s. 21–24); begreppet kräver ingen exakt 50–50-fördelning mellan språken, vilket det ofta tas för. Det gäller i princip alla språk, även om det i praktiken nästan alltid handlar om svenska och engelska (PF, avsnittet ”Svenska, engelska och parallellspråkighet inom svensk högre utbildning”, s. 6–8).

## Varför svenska termer väljs

Språklagen gör svenska till huvudspråk. Det allmänna ska se till att svenskan "används och utvecklas" (6 §), och myndigheter ska se till att svensk terminologi inom deras fackområden "finns tillgänglig, används och utvecklas" (12 §). Språkrådet tolkar det så att svenskan ska finnas kvar inom fackområden där engelskan dominerar (PF, avsnittet ”Språklagen och lärosätenas ansvar för svenska och svenskt fackspråk”, s. 8–9).

Debatten gäller risken att svenskan förlorar mark till engelskan inom vissa domäner, särskilt teknik och naturvetenskap (PF, avsnittet ”Svenska, engelska och parallellspråkighet inom svensk högre utbildning”, s. 6–8, PF, avsnittet ”Svenskt fackspråk är viktigt för både studier och arbete”, s. 16–19, PF, avsnittet ”Studenter värderar svenskt fackspråk högre än deras lärare gör”, s. 19–21). Rapporten använder inte ordet domänförlust, men det är just den risken den beskriver.

En fungerande terminologi gör det möjligt att delta i ett specialiserat samtal och att förstå, sortera och strukturera ny kunskap (PF, avsnittet ”Svenska, engelska och parallellspråkighet inom svensk högre utbildning”, s. 6–8). En svensk term som läsaren saknar blir därför en lucka i läsarens tänkande lika väl som i texten.

Engelskan är starkast inom teknik och naturvetenskap, men även där föredrar de flesta studenter svenska (PF, avsnittet ”Studenter föredrar och värnar om svenska – Studenter vill studera på svenska”, s. 12–16, PF, avsnittet ”Svenskt fackspråk är viktigt för både studier och arbete”, s. 16–19). Att en text handlar om teknik är alltså inget skäl att utgå från att läsaren vill ha engelska termer.

I praktiken gäller regeln `facktermer` i profilen `webb`: den etablerade svenska termen väljs där en sådan finns, och engelskan behålls bara där svenskan saknar en bra motsvarighet (RAG, LLM, API). Undantaget för externt förankrad terminologi gäller fortfarande.

## Parallell termhantering i text

PF, avsnittet ”Mot en fungerande parallellspråkighet och svensk terminologi i praktiken”, s. 21–24 föreslår att centrala termer presenteras på båda språken, att man gör termlistor och att man reflekterar över ämnets termer. Överfört till skrift blir det fem regler.

1. En central term införs på båda språken när läsaren kan möta den engelska formen. Den svenska termen skrivs först och den engelska inom parentes vid första förekomsten, "styrsystem (control plane)", och därefter används bara den svenska.
2. Ett begrepp får en benämning genom hela texten. Den svenska och den engelska termen växlar inte i samma text; de allmänna reglerna om ordval och redundans står i basens `prefer_plain_words` (modulen `writing`, profilen `core`, paketet `basics`) och `cut_padding` (modulen `writing`, profilen `core`, paketet `basics`).
3. Fackspråk skiljs från allmänspråk efter läsaren. Att veta vad som är professionens fackspråk och vad som är allmänspråkliga ord kan vara avgörande för kommunikationen med en lekman (PF, avsnittet ”Studenter värderar svenskt fackspråk högre än deras lärare gör”, s. 19–21). Konsulttext och essäer riktar sig ofta till läsare utanför fackområdet, och där förklaras termen eller ersätts med det allmänspråkliga ordet.
4. En text med många termer får en ordlista, så att löptexten slipper förklara varje term (PF, avsnittet ”Mot en fungerande parallellspråkighet och svensk terminologi i praktiken”, s. 21–24 punkt ii; SR §4.2 om förkortningar).
5. Språkvalet planeras medvetet. PF, avsnittet ”Mot en fungerande parallellspråkighet och svensk terminologi i praktiken”, s. 21–24 varnar för enkelriktad parallellspråkighet, där engelska glider in i svensk text medan svenska aldrig kommer in i engelsk. Testet för en engelsk term i svensk text är att valet kan motiveras; en term som står där av bekvämlighet klarar inte testet.

## Var man hittar termen

Fem källor täcker det mesta. Rikstermbanken (rikstermbanken.se) och uppslagsverk ger facktermer som saknas i ordböcker (SR §8.3). Isofs lista Engelska ord på svenska (isof.se/engelska-ord) ger svenska förslag på engelska ord, och svensk-engelska lexikon finns hos NE och Folkets lexikon (folkets-lexikon.csc.kth.se), engelska ordböcker via onelook.com (SR §8.3). Svenska datatermer (it-ord.computersweden.se) ger it-termer och nämns redan i mekaniken. SS-ISO 704 _Terminologiarbete_ beskriver hur termer och begrepp etableras (PF, avsnittet ”Mot en fungerande parallellspråkighet och svensk terminologi i praktiken”, s. 21–24).

Förslag från maskinöversättning och chattbottar granskas kritiskt (SR §8.1), och det gäller också agentens egna översättningsutkast.

## Skrivregler som skiljer svenska från engelska

Texten skrivs efter målspråkets konventioner; en konvention som följer med från källtexten är ett mekaniskt fel. Detaljerna står i [snabba_skrivregler_digest.md](../../../../core/packages/regler/reference/snabba_skrivregler_digest.md), och tabellen samlar de punkter där språken skiljer sig:

| Område                                     | Svenska                                                         | Engelska                              | Källa |
| ------------------------------------------ | --------------------------------------------------------------- | ------------------------------------- | ----- |
| Sammansättningar                           | skrivs ihop: kaffepaus, systemarkitektur                        | ofta isär: coffee break               | SR §3.1 |
| Blandade led                               | bindestreck före sista ledet: all inclusive-resa                | —                                     | SR §3.3 |
| Veckodagar, månader, nationalitetsadjektiv | liten bokstav: torsdag, mars, svensk                            | stor: Thursday, March, Swedish        | SR §2.2 |
| Titlar och namn med flera ord              | bara första ordet versalt: _Det sjunde inseglet_                | title case: _The Old Man and the Sea_ | SR §2.5 |
| Genitiv                                    | ingen apostrof: Annas, Lars cykel                               | apostrof: Anna's, the girls'          | SR §1.14 |
| Citattecken                                | ”…” (lika i början och slutet), även kring citat på andra språk | “…”                                   | SR §1.13 |
| Tal                                        | 3 400; 3,14                                                     | 3,400; 3.14                           | SR §5.2 |
| Förkortningar av vanliga ord               | gemener: vd, aids                                               | ofta versaler: CEO, AIDS              | SR §4.3 |
| Böjning av förkortningar                   | kolon: EU:s, API:t, AI:n                                        | apostrof eller ingen ändelse          | SR §4.4 |

## Förhållande till andra regler

Regeln om den svenska termen först, punkt 1 ovan, följer mekaniken och gäller inte en text som medvetet följer en extern källas termer; undantaget i regeln `facktermer` i profilen `webb` står kvar.

Inga regler här ställer krav som krockar med en vanlig husstil eller personlig stilpreferens. PF:s budskap om att svenskan ska vara närvarande stöder de befintliga principerna och ger dem inga nya krav.

