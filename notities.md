# 📓 Notities & logboek — wingfoil-briefing

Dit bestand is bedoeld om bij te houden waar de briefing goed zat en waar niet,
zodat `instructies.md` gericht bijgesteld kan worden. Voeg per sessie een
regel toe. Hoe concreter, hoe beter (welke drempel voelde verkeerd, niet
alleen "klopte niet").

## Hoe te gebruiken
1. Na een sessie op het water: voeg hieronder een nieuwe regel toe onder
   "Log".
2. Zodra een patroon zichtbaar wordt (bv. "golfperiode-drempel van 5s voelt
   vaak te streng aan"), zet dat om in een concrete aanpassing van
   `instructies.md` en noteer de wijziging onder "Doorgevoerde aanpassingen".

---

## Log

| Datum | Briefing zei | Werkelijkheid op het water | Vermoedelijke oorzaak | Actie nodig? |
|18-08-2026|Goed (grensgeval met optimaal)|Optimaal|Golfhoogte en tijd tussen golven was voldoende|Ja: Golfhoogte drempel omlaag naar 1m en tijd naar 4,5s|
| | | | | |
| | | | | |

---

## Doorgevoerde aanpassingen aan instructies.md

| Datum | Wijziging | Reden |
|---|---|---|
| _voorbeeld_ | — | — |
| | | |

---

## Open vragen / ideeën voor later
- [ ] Screenshot/grafiek van Windwaarnemingen of Soarcast meesturen naar Slack
      — voorlopig geparkeerd; alternatief: routine genereert zelf een
      grafiek (bv. met Python/matplotlib) op basis van de opgehaalde cijfers,
      met de eigen drempelwaarden als lijnen erin, en upload die naar Slack.
- [ ] Getij-informatie (eb/vloed) explicieter meenemen bij de pier-keuze
- [ ] Checken of de golfperiode-drempel (5s) en golfhoogte-drempel (1,1m)
      na een paar weken observatie nog kloppen
- [ ] Overwegen of een vierde categorie "Uitstekend" nuttig is voor de
      allerbeste omstandigheden (bv. wind >20kts + golf >1,3m + optimale hoek)
- [ ] **Sessie-tooling is niet altijd hetzelfde tussen runs, en dat raakt
      windwaarnemingen.nl direct.** `instructies.md` gaat ervan uit dat
      "get_page_text" een JS-uitvoerende (browser-gebaseerde) extractietool
      is: voor windwaarnemingen.nl moet eerst een change-event op de
      station-dropdown gesimuleerd worden (clientside JS) voordat de tabel
      met echte cijfers verschijnt. In de runs van 19 t/m 23-08 werkte dit
      prima (zie de Realitycheck-secties in die briefings). In de
      avondbriefing van 23-08 had de sessie echter alleen een platte
      `WebFetch`-tool (haalt kale HTML op, voert geen JavaScript uit) —
      daardoor kwam er voor windwaarnemingen.nl alleen het lege menu terug,
      geen tabeldata. Dit is dus geen inhoudelijke wijziging aan de bron,
      maar een verschil in beschikbare tooling tussen sessies.
      Actie: bij het begin van een run kort vaststellen of de sessie een
      browser-/JS-uitvoerende extractietool heeft; zo niet, dit expliciet
      vermelden in de briefing (zoals nu gebeurd) i.p.v. alleen te melden
      dat de bron "niet beschikbaar" was — het onderscheid tussen "bron is
      down" en "sessie mist de juiste tool" is voor de lezer nuttig.
      Zie ook: Windfinder dag-3/Superforecast-pagina's falen al langer
      structureel om dezelfde reden (dag-tabs vereisen een klik/JS), en
      Soarcast wisselt tussen runs (werkte 19-22/08 via een blijkbaar niet
      stabiel data-endpoint, faalde sindsdien).
