# Bokstavligt snabel-a

Snabel-a (`@`) är citatutlösare i modulens värdformat. Mitt i ordet,
som i `namn@example.com`, är tecknet vanlig prosa: det som står före
`@` är en bokstav, och ingen citatkandidat startar. I triggerposition –
ett handtag i början av en mening eller ett fristående omnämnande –
tolkas ett bart `@` som början på en citeringsnyckel, och en nyckel
som inte kan lösas upp stoppar renderingen med CTX-REF013.

## Motivering

Falska träffar kommer just från handtag och adresser, som vanlig text
naturligt innehåller. Två säkra stavningar finns, och båda går igenom
renderingen oförändrade: kodspannen och det omvända snedstrecket
framför tecknet, `\@`. Välj kodspann när token är ett namn eller en
adress (`@ctxmod`, `tips@example.se`) eller när citatsyntax visas;
välj snedstrecket när snabel-a sitter inbäddat i löptext där
backticks skulle vilseleda om formateringen. Kodspann och kodblock är
immuna zoner: inget mellan backticks tolkas som citat, länk eller
lokatormarkering. Granskningen före publicering är en sökning efter
varje `@` i dokumentet; varje träff ska vara mitt i ett ord, inuti en
kodspann eller försedd med undantagstecknet `\@`.
