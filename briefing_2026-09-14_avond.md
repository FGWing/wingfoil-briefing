# 🌊 Wingfoil-briefing Zandvoort–Wijk aan Zee
_14-09-2026 · Avondbriefing_

---

## ⚡ Snel overzicht
- **Dinsdag:** Goed (grensgeval Matig — Windfinder zelf lager dan de andere bronnen) (08:00-17:00)
- **Woensdag:** Matig (09:00-14:00)
- **Donderdag:** Optimaal (11:00-17:00)
- **Beste dag in de 7 dagen erna:** zaterdag 19 september

---

## 📅 Komende 72 uur

### Dinsdag — Goed (grensgeval Matig)
- Beste venster: **08:00-17:00** — wind 11,0-13,5 kts, gust 19,1-20,7 kts, richting 203-234° (**side-shore** bij Zandvoort)
- Golven: 0,73-0,84 m / 4,88-4,95 s — periode blijft de hele dag net onder de 5s-Optimaal-drempel
- Bronnen: Windfinder 11,0-13,5 kts · Soarcast 13,6-17,7 kts · windwaarnemingen.nl 12,4-14,6 kts → **wijkt af**: Soarcast en windwaarnemingen.nl tonen duidelijk meer wind (tot 17,7 kts) dan Windfinder; richting is bij alle drie vrijwel gelijk (203-252°, side-shore). Zelfs als de hogere cijfers kloppen, houdt de korte golfperiode (<5s) dit venster op Goed in plaats van Optimaal. Vanaf 20:00 draait de wind naar 312-315° (**pal aanlandig**) en zakt de gemiddelde wind — avond niet interessant.

### Woensdag — Matig
- Beste venster: **09:00-14:00** — wind 13,1-14,0 kts, gust 15,5-16,2 kts, richting 284-292° (**pal aanlandig** bij Zandvoort)
- Golven: 0,95-1,16 m / 5,13-5,64 s — golf is prima, maar de combinatie van beperkte wind en pal aanlandige richting houdt dit op Matig
- 🌊 Piervoorkeur: richting (284-292°, NW) + golf ≥0,8m → pier-logica van toepassing. Valt in de "280°-360°"-band → **IJmuiden** (Zuidpier) is de rustigere kant; Wijk aan Zee ligt hier vol in de aanlandige golfslag
- Buiten dit venster (vóór 09:00 en na 14:00) zakt de wind onder de Slecht-drempel (gust <16 kts ÉN gem <14 kts) — geen bruikbare uren
- Bronnen: Windfinder 13,1-14,0 kts (204-292°) · Soarcast 12,6-13,7 kts · windwaarnemingen.nl 11,3-12,2 kts → **eens** (kleine onderlinge afwijking, alle drie rond de 12-14 kts)

### Donderdag — Optimaal
- Beste venster: **11:00-17:00** — wind 15,9-19,4 kts, gust 19,7-24,8 kts, richting 231-238° (**side-shore** bij Zandvoort)
- Golven: 1,11-1,34 m / 5,78-6,04 s — ruim boven de Optimaal-drempel (>1,1m én ≥5s)
- Geen pier-logica van toepassing in dit venster (richting is side-shore, niet aanlandig)
- Bronnen: Windfinder 15,9-19,4 kts. Soarcast en windwaarnemingen.nl reiken deze run niet ver genoeg vooruit om de namiddag te dekken → **niet vergelijkbaar** voor dit venster. Let op: voor 08:00 's ochtends laten Soarcast (29,5 kts gust) en windwaarnemingen.nl (31,5 kts gust) een veel scherpere uitschieter zien dan Windfinder (20,0 kts) — wijst mogelijk op een kortstondig pittig randje/frontje vroeg in de ochtend, buiten het hoofdvenster. Het middagvenster zelf oogt in Windfinder consistent en stevig.

---

## 🔭 Kans op mooie sessies daarna (dag 4-9)
Naast donderdag (zie hierboven, Optimaal) springt **zaterdag 19 september** er duidelijk uit: wind 15,6-16,6 kts, gust 22,0-23,0 kts, richting 211-218° (side-shore bij Zandvoort), golf 1,15-1,23 m / 5,52-5,73 s tussen ongeveer 11:00-17:00 — voldoet ruim aan Optimaal. Vrijdag 18 sept heeft prima golf (1,12-1,27 m / 5,5-5,8 s) maar te weinig wind (13,1-13,4 kts) uit een pal aanlandige hoek (272-292°) → Matig, lage kans. Zondag 20 t/m dinsdag 22 sept valt de wind terug naar 1-8 kts → Slecht, lage kans.
Kans: **hoog voor donderdag 17 en zaterdag 19 september**, laag voor de rest van de periode.
⚠️ Onzeker op 4+ dagen — check dichter bij de tijd opnieuw.

---
_Bronnen: Windfinder (GFS) · Soarcast (KNMI Harmonie) · windwaarnemingen.nl (KNMI, IJmuiden)_
_Let op: Windfinder-data is gehaald uit de ingebedde paginadata (Astro-serialisatie in de `props`-attributen: `ForecastSection` (ssr) voor dinsdag/woensdag, `ForecastDataInit` voor donderdag t/m dag 9) van de forecast-pagina. Soarcast is opgehaald via `/sc/scapi.php?table=mv_forecast_location_markers` (location_id 133 = IJmond/KNMI). windwaarnemingen.nl via `database/vsp_mrg_wstats.php?st=IJmuiden2`. Ruwe waarden in m/s zijn omgerekend naar knopen (×1,94384)._
