# Adressera exempelkällan

Exempelpaketet bär modulens citation-undervisning. Denna referens
förklarar formerna den demonstrerar: hur källans citeringsnyckel
härleds, citatformerna, hur lokatorer adresserar platser inuti en
källa, och vad den renderade utmatningen gör med alltihop. Varje form
visas inuti en kodspann – inert enligt parserns immunitetsregel –
eftersom den enda platsen där ett live-citat hör hemma är den
genomarbetade filen bredvid denna.

## Citeringsnyckeln

Källans citeringsnyckel är dess härledda kvalificerade namn:
`writing_sv_core_source_example_example`. Kedjan vandrar
ägarvägen – modul `writing_sv`, profilsegment `core`,
exempelpaketssegment `source_example`, källnamn `example` – med de
strukturella katalognamnen (`profiles/`, `examples/`, `sources/`)
exkluderade, och sammanfogar segmenten med understreck. En
kvalificerad nyckel namnger exakt en entitet: namn valideras unika
över den aktiva kompositionen, så ett kvalificerat citat kan aldrig
tie.

Korta nycklar är bekvämformen: en nyckel som inte själv är ett
kvalificerat namn löses upp utåt efter första träff – den citerande
kroppens egna källor först, sedan dess ägarförfäder närmast först,
sist resten av den aktiva kompositionen. Denna modul övar ingen av
dessa: en källa, en nyckel, ingen tvetydighet att demonstrera.

## Citatformerna

De stödda pandoc-formerna, var och en med exempelnyckeln:

- Parentetisk: `[@writing_sv_core_source_example_example]`
- Narrativ: `@writing_sv_core_source_example_example`
- Suppress author: `[-@writing_sv_core_source_example_example]`
- Prefix: `[@se @writing_sv_core_source_example_example]`
- Suffix / lokator:
  `[@writing_sv_core_source_example_example, malltext]`
- Multipel: `[@writing_sv_core_source_example_example; @annan_källa]`
  – meningsfull med två olika nycklar, vilken denna
  enkällmodul inte har
- Måsviktad nyckel: `@{nyckel med mellanslag}` – måsvingrarna vinner;
  `#` och `/` är aldrig strukturella inuti dem
- Lokatormåsvingar:
  `[@writing_sv_core_source_example_example {…}]` – måsviktad
  suffixdata, buren oförändrad

## Lokatorer

Varje fil i en katalogformig källa bär en implicit sökvägslokator: sin
sökväg relativt källroten (`chunks/01_malltext.md`,
`summary/oversikt.md`, `SOURCE.md`). Deklarerade lokatorer lägger
mänskliga alias ovanpå – `<ctxmod_locator>`-markeringen i en
chunkkropp – och citatets suffixposition binder genom dem:
`[@writing_sv_core_source_example_example, malltext]` och
`[@writing_sv_core_source_example_example#chunks/01_malltext.md]`
adresserar samma fil. Matchning normaliserar med skiftlägesvikning och
mellanslagssammandragning, så `Malltext` och `malltext  ` binder
samma alias. Ett suffix som matchar ingen deklarerad lokator är inte
ett fel – det är prosa som förs vidare, pandoc-stil; bara `#`-sökvägsformen
valideras mot källträdet. Att deklarera en fils egen implicita sökväg
som alias är redundans och drar varningen CTX-REF018.

## Renderingsposturen

En citatförekomst renderas som en namngiven fotnotsmarkör vars namn
är det citerade målets kvalificerade namn, med lokatorn kvar inline på
platsen: `[@writing_sv_core_source_example_example, malltext]` blir
`[^writing_sv_core_source_example_example, malltext]` i den
renderade kroppen. En ensam namngiven markör utan suffix stavas
`[^writing_sv_core_source_example_example]` – markören är namnet,
så markör och listpost aligneras av konstruktion. Den renderade
`footnotes_list.yaml` är en ordnad mappning nycklad på kvalificerat
namn, med en post per unikt citerat mål, sorterad på kvalificerat
namn – ordningsvalet gjort för renderingsdifferensens stabilitet.
Postinnehåll för en källa är interimistiskt: `source.yaml`-metadata
rå serialiserad som inline-JSON, med `(inferred: <fields>)` tillagt
när inferensmarkeringar gäller; CSL/Hayagriva-pipelinen ersätter
den interimistiska formen på färdplanen. Lokatorer går aldrig in i
listan – de stannar inline på citatplatserna.

Exempelkällan själv deklarerar ingen `inferred:` – syntetiskt
material har inget overifierat – så `(inferred: …)`-noteringen
undervisas här i kodspann och syns i modulens renderade utmatning
först när en framtida lokal källa förtjänar den. Ärligheten är
regeln: ett fält listat i `inferred:` namnger ett värde författaren
inte verifierade, och noteringen hindrar den renderade bibliografin
från att presentera det som verifierat.

## Immunitet och det bokstavliga snabel-a

Inget inuti inline-kodspann eller kodblock tolkas som citat, länk
eller lokatormarkering; innehåll återkommer oförändrat genom båda
renderingspassen. Snedstrecksundantaget `\@` är inte en
citatkandidat, och undantagstecknet bevaras genom
tur-och-retur-resan, så ett bokstavligt `@` i triggerposition – ett
meningsinitialt handtag, ett fristående omnämnande – kräver en
kodspann eller ett undantag, och mitt-i-ord-adresser som
`namn@example.se` behöver inget eftersom föregående tecken är en
bokstav.
