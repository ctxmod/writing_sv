# Exempelkälla

En liten syntetisk källa som lagras under katalogen `sources/example/`
i exempelpaketet `source_example`. Den demonstrerar källstrukturen –
chunkar med deklarerade lokatorer och en översikt som refererar
chunkarna via implicita sökvägslokatorer – och är målet för de
live-citat som exempelpaketets egna innehållsdomäner bär.

Paketet runt omkring är den genomarbetade demonstrationen av en
väldifferentierad paketstruktur: en `package.yaml`-ingång,
innehållsdomäner (`rules/`, `reference/`) med modulens enda live-citat,
och denna katalogformiga källa som citaten skulle lösa upp mot.

Källan täcker inget externt material: varje chunk är syntetisk
undervisningsprosa skriven för denna modul, och `source.yaml`
deklarerar därför ingen `coverage:`. Dess citeringsnyckel är det
härledda kvalificerade namnet `writing_sv_core_source_example_example`
– modulnamn, profilsegment, exempelpaketssegment och källnamn
sammanfogade med understreck, med de strukturella katalognamnen
exkluderade från kedjan. Delat innehåll utanför detta paket bär inga
live-citat: citatsyntax undervisas i kodspann där, så detta paket är
den enda plats där ett live-citat av denna källa står.

## Lokatorer

- `chunks/01_malltext.md` deklarerar lokatorn `malltext`.
- `chunks/02_granskning.md` deklarerar lokatorn `granskning`.
- Varje fil bär också sin implicita sökvägslokator
  (`chunks/01_malltext.md`, `chunks/02_granskning.md`,
  `summary/oversikt.md`, `SOURCE.md`), så
  `[@writing_sv_core_source_example_example#chunks/01_malltext.md]`
  adresserar malltexten utan någon deklarerad lokator.
