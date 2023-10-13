# navngivning av datoer på norsk

> [!INFO]+ Obs!
> Navngivning av notater er kanskje et annet tema?

Som et utgangspunkt

Takk til Oyvind, og Ekornfisk som gikk opp stien før meg.

Når notatene dine sorteres alfabetisk så vil det sette noen begrensninger på notater som inneholder notater, [[daily notes]] f. eks. Som standard får de bare navnet på dagens dato. Nøyaktig hvordan datoen skal skrives kan du påvirke i innstillingene.

Men dersom du tar den norske tilnærminga og skriver f. eks 21.01.2023, så vil den lista sortere etter det første tallet i stigende rekkefølge. Det vil si at det neste notatet på lista kan være 22.07.2023, fordi det er det første tallet som gjelder.

Du kan absolutt sortere notatene på andre måter (som dato opprettet, eller dato endret), som for all del vil fikse det problemet på her på en enklere måte. Samtidig foretrekker jeg å sortere notatene mine alfabetisk, og da måtte jeg finne en vei rundt det.

Jeg ville altså formatere mine daglige notater på denne måten "2023-01-21 - Lørdag". Jeg syns det er lettere å huske hva som har skjedd når, om jeg har ukedagen tilknytta til en rekke hendelser. Ved å starte med årstallet vil alle notatene fra 2023 komme etter hverandre, og det neste tallet som sorteres etter da blir månedene, og deretter dagene. Sånn sett får du både alfabetisk *og* kronologisk rekkefølge.

Om du vil lese mer formatering av datoer finner du en [oversikt her](https://momentjs.com/docs/#/displaying/format/). Bare for å gi deg litt kontekst så det eventuelt blir lettere å forstå: 2023-01-21 er det samme som `YYYY-MM-DD`. For å legge til ukedagen på slutten så blir det `YYYY-MM-DD - dddd`.

Du kan endre språket på brukergrensesnittet i Obsidian, hvis du vil at alt skal stå på norsk. Om du, som meg, riktignok foretrekker å ha brukergrensesnittet på engelsk, men datoen på norsk, så må du installere en plugin som heter Calendar. Der kan du overstyre måten datoer vises.

- [ ] Vis et skjermbilde av innstillingene på Calendar-pluginen
- [ ] Vis et skjermbilde av språkinnstillingene i Obsidian (about-seksjonen)

##  Kilder

---
- Oyvind hadde tidligere etterspurt det samme på Discord
	- https://discord.com/channels/686053708261228577/694233507500916796/931470798680633354
- Ekornfisk tok det et steg videre med å [lage stor forbokstav på ukedagene](https://forum.obsidian.md/t/uppercase-capital-letter-on-weekdays-in-mother-language/36044) på norsk
	- Svaret som kom ut fra det var fra en som kaller seg Angel, som anbefalte å legge inn følgende kode i templaten for daily notes:
	- <div class="Capitalize"><% tp.file.creation_date("dddd DD.MM.YY") %></div>
	- div.Capitalize { text-transform: capitalize; }