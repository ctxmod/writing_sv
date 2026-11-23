# Svenska säljutskick: gränser och exempel

Fördjupning till regeln [talspraksnara_utskick.md](../rules/talspraksnara_utskick.md).

Regeln lägger till det som gäller svenska säljutskick ovanpå säljprofilens filer, som gäller oförändrade, och ovanpå den svenska korrespondensen i [svensk_korrespondens.md](../../meddelanden/reference/svensk_korrespondens.md). Den svenska språkmekaniken, Isofs och Språkrådets skrivregler och säljregistertestet finns i paketet `regler` (modulen `writing_sv`, profilen `core`), och upprepas inte här.

## Talspråksnära svenska i utskicken

Skrivna säljutskick på svenska skrivs i en enkel, talspråksnära svenska: meningar som avsändaren skulle kunna säga i telefon med samma ord. Det gäller första kontakten, uppföljningen, introduktionsförfrågan och korta mejl som skrivs vid sidan av ett samtal. Varje utkast har en enda fråga eller begäran, inga marknadsföringsord, inga symmetriska eller balanserade konstruktioner som "både … och" eller par av satser byggda för rytmens skull, och inga punktlistor i mejlet. Ämnesraden är enkel och saklig, i stil med "Angående er AI-satsning", aldrig en ordlek; den säger vad utskicket vill ta upp, enligt den allmänna regeln om ämnesrader i `messages` (modulen `writing`, profilen `correspondence`, paketet `replies`).

Testet: läs utkastet högt. En mening som bara fungerar på papperet, eller som bär en bisatskedja som avsändaren aldrig skulle säga, skrivs om.

## En avvikelse från det bisatsdrivna registret

Regeln avviker medvetet från ett vårdat, bisatsdrivet register, som många skribenter har som sin svenska stilpreferens. För skrivna säljutskick gäller i stället det talspråksnära registret ovan. Avvikelsen gäller bara säljutskick. Offerter, projektbeskrivningar och avtal som ett utskick hänvisar till följer skrivmodulens profil `commercial_documents` (med profilen `affarsdokument` här) och skribentens stilpreferens som vanligt, och annan korrespondens följer korrespondensprofilen.

Det som inte ändras: det konstaterande registret (`tone_and_register` i modulen `writing`) gäller fullt ut – ett mejl får tilltala mottagaren direkt men inte ställa retoriska frågor, lova resultat eller förutsätta mottagarens problem. Tilltal, hälsningspar och tankstreck följer skribentens stilpreferens och den svenska mekaniken; en första kontakt via en gemensam bekant får använda innekretsregistrets hälsning med utropstecken, enligt [svensk_korrespondens.md](../../meddelanden/reference/svensk_korrespondens.md).

Kort och talspråksnära betyder inte hackigt. Fragment och staplade slagordsrader klarar fortfarande inte katalogens post 3 om stakiga och säljiga rader (`catalogue` (modulen `writing`, profilen `core`, paketet `anti_patterns`)); en mening i ett säljutskick är en hel mening, bara enkelt byggd.

Bisatsdrivet (undvik i ett säljutskick, illustrativt):

> Eftersom ni nu tar piloten för fakturamatchning vidare mot produktion, vilket brukar innebära att de många leverantörsformaten blir det som avgör om flödet håller, tänkte jag att det kunde vara värdefullt att höra av mig.

Talspråksnära (bättre, illustrativt):

> Jag såg att ni tar piloten för fakturamatchning vidare mot produktion. Där brukar leverantörsformaten bli det svåra när riktiga fakturor börjar komma in.

