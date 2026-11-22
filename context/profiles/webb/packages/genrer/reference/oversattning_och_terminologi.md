# Översättning mellan svenska och engelska

Båda riktningarna skrivs från sakunderlaget, inte från den översatta
strukturen. En text som följer källspråkets bygge hörs som
översättning, och varje mening som ryms i källans rytm bär källans
val – även där målspråket skulle välja annorlunda. Skriv om från
ämnet: säg vad innehållet säger, i målspråkets ordning.

Engelska ramar i svensk text översätts bort: *säkerhetsfirst*,
*gated bakom*, *end-to-end-ansvar*, *setup* är importformer som
svenskan har ord för. Fällorna sitter ofta i formerna, inte iorden:
tal- och datummönster, citattecken och sammansättningsregler skiljer
sig mellan språken, och kärnpaketets mekanikregler gäller även
översatt text.

## Terminologin som bro

Terminologin är parallellspråkighetens bro: en term per begrepp på
båda språken, och termvalen dokumenterade så att nästa text inte
börjar om. En domän kan förlora precision i översättning; termer som
saknar svensk motsvarighet behålls, och deras plats i texten
förklaras vid första användningen.

## Engelska ramar i svensk text

Skrivmodulens profil `translation` bär genreprinciperna för båda
riktningarna; här står den svenska tillämpningen. Svensk text som
översätts från engelska, eller skrivs med engelska förlagor i
bakhuvudet, behåller de tekniska begreppen men släpper den engelska
inramningen. Testet och de bearbetade exemplen står i kärnprofilens
regel `svenska_fran_sakunderlaget`: styrsystem för _control plane_,
konfiguration för _setup_, helhetsansvar för _end-to-end-ansvar_,
kundsystem för klientsystem och "Jag träffar er gärna" för en
välkommen konversation. Ett ord som saknar fast ersättning, som
"säkerhetsfirst", skrivs om från fakta. Fler termpar finns i
profilens regel [facktermer.md](../../principer/rules/facktermer.md).

En engelsk konstruktion som fått stå kvar i svensk text prövas som en
engelsk term: saknar svenskan en bra motsvarighet? Finns en sådan
används den svenska, och meningen byggs om kring den.

## Originalet först

Där en publikation finns på svenska och engelska och svenska är
originalspråket skrivs och fastställs den svenska texten först, och
den engelska versionen översätts därefter och skrivs från
sakunderlaget. En ändring i sak görs i originalet och förs över till
versionen. Hur en viss publikation publicerar sina språkversioner är
publikationens egen regel.

## Terminologi och parallellspråkighet

Hur svenska och engelska termer hanteras i samma text, varför den
svenska termen väljs där den finns, var man hittar den och vilka
skrivregler som skiljer språken åt står i digesten
`terminologi_och_parallellsprak` (profilen `parallellsprak`, paketet
`sprakbruk`), ur Isofs _Parallella fackspråk_ och _Snabba skrivregler_.
