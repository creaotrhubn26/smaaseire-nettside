# SmåSeire – offentlig nettside

Statisk produkt-, støtte- og personvernside for SmåSeire fra Creatorhub AS. Ingen brukerdatabase, analyseverktøy eller appkildekode.

## Sentral styring av julemodus

Administrator med skrivetilgang til dette GitHub-repoet åpner Actions → **Nettside og julemodus** → **Run workflow**, velger **På** eller **Av** og en fremtidig utløpsdato. Vent til publiseringen er grønn. Endringen gjelder neste appversjon med sesongstøtte; versjon 1.1 (3) har ikke denne funksjonen.

Ingen nøkkel eller administratortilgang legges i appen. Den leser bare offentlig `app-config.json` over HTTPS. Endringer registreres i Git-historikken. Appen sjekker ved oppstart, når den blir aktiv og inntil hvert femte minutt mens den er åpen. GitHub Pages kan mellomlagre responsen, så endringen er ikke øyeblikkelig. Uten nett beholdes sist gyldige innstilling i maks 24 timer; deretter skjules juleinnholdet. Utløpsdato er en ekstra automatisk stopp. Listene slettes ikke.

Julemodus er **av** ved første publisering. Ønsker, besøksplan og private gaveplaner lagres lokalt, aldri i denne nettsiden eller konfigurasjonsfilen. Ikke legg persondata i repoet.
