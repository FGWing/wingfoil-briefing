# 🌊 Wingfoil-briefing Zandvoort–Wijk aan Zee
_28-10-2026 · Ochtendbriefing_

⚠️ **Technische kanttekening:** Soarcast kon deze run niet opgehaald worden — de pagina (`/web/locationinfo?...`) is een pure client-side React-app die zonder JavaScript-executie leeg blijft (geen server-rendered data), en de achterliggende API (`/sc/scapi.php`, `/sc/latest-spot-harm-all`) is niet bedoeld voor directe geautomatiseerde aanroepen zonder een browsersessie. Kruisvalidatie dit keer dus alleen tussen Windfinder (GFS) en windwaarnemingen.nl (KNMI). Windfinder is opgehaald via de onderliggende Astro-JSON (forecast-pagina geeft vandaag+morgen in detail, de preload-component erin geeft dag 3 t/m 10). windwaarnemingen.nl is opgehaald via de vsp-database-endpoints (`vsp_vdg_wstats.php`/`vsp_mrg_wstats.php`, station IJmuiden).

**Netto beeld:** vandaag (woensdag) een bruikbaar **Goed**-venster in de middag, maar donderdag en vrijdag vallen de wind helemaal weg (**Slecht**, te weinig wind). De Realitycheck laat zien dat de wind vanochtend iets harder waait dan beide modellen voorspelden — dat geeft iets meer vertrouwen in het middagvenster van vandaag. De outlook (dag 4-9) laat een kansrijke periode zien rond maandag 2 november.

---

## ⚡ Snel overzicht
- **Woensdag:** **Goed (a)** (12:00-16:00) — wind 13-15,6 kts, licht aanlandig, golf net onder de 1,1m-drempel.
- **Donderdag:** **Slecht** (te weinig wind, hele dag) — Windfinder en KNMI stemmen overeen.
- **Vrijdag:** **Slecht** (te weinig wind, hele dag) — wind komt pas in de avond iets op, blijft ruim onder de 15kts-drempel.
- **Beste dag in de 7 dagen erna:** maandag 2 november (grensgeval Optimaal/Goed)

---

## ⏰ Realitycheck vandaag
- Laatste actuele uren (windwaarnemingen.nl, IJmuiden, 04:00-06:10): **wind gem. ~14,8 kts, gust gem. ~17,3 kts (piek 19,8 kts), richting 254-268° (WZW/West)**.
- Was voorspeld voor dezelfde uren: **windwaarnemingen.nl/KNMI** gaf voor 04:00-06:00 gem. **~12,1 kts, gust ~17,6 kts, richting 254-262°**. **Windfinder/GFS** gaf voor dit venster **~11,4-11,5 kts gem., gust ~15,2-15,3 kts** — beide modellen iets lager dan de praktijk.
- Conclusie: de wind loopt **licht VOOR op beide modellen** qua gemiddelde (+~2,7 kt t.o.v. KNMI, +~3,3 kt t.o.v. Windfinder/GFS); de gust is **conform verwachting** (KNMI) tot iets hoger. Rest-van-de-dag inschatting: **licht naar boven bijgesteld** — het Goed(a)-venster in de middag (zie hieronder) wordt aannemelijker, en gezien windwaarnemingen.nl voor het middagblok zelf al hogere cijfers geeft dan Windfinder, is een iets stevigere sessie dan de kale Windfinder-tabel suggereert niet uitgesloten.

---

## 📅 Komende 72 uur

### Woensdag — Goed (a)
- Beste venster: **12:00-16:00** — wind 13-15,6 kts, gust 16-21,6 kts, richting 234-253° ([licht aanlandig, overgang naar side-shore richting het einde van het venster] t.o.v. Zandvoorts kustlijn 197,5°/17,5°)
- Golven: 0,96-0,98m / 5,3-5,6s — net onder de 1,1m-drempel voor Optimaal, vandaar Goed(a) i.p.v. Optimaal.
- 🌊 Piervoorkeur: windrichting (234-253°, zuid/zuidwest-component) + golf ~1,0m ≥0,8m-drempel → **Wijk aan Zee rustiger** — de Noordpier breekt de zuid(west)-golfslag; bij IJmuiden staat de wind hier vrijwel pal aanlandig (pierzone-hoek 240°) tegen de onbeschutte zijde.
- Getij: laagwater 00:20 (0,32m), hoogwater 04:36 (2,28m), laagwater 12:32 (0,47m), hoogwater 16:55 (2,29m), laagwater 21:03 (0,94m). Rond het venster (12:00-16:00) loopt het van laag- naar hoogwater — shorebreak neemt richting 16:00 geleidelijk toe.
- Bronnen: Windfinder 13-14 kts / gust 16-18 kts · Soarcast niet beschikbaar deze run · windwaarnemingen.nl (KNMI) 13,6-15,6 kts / gust 18,7-21,6 kts → **wijkt af, KNMI geeft duidelijk hogere gusts**; zie Realitycheck voor waarom KNMI hier iets meer vertrouwen krijgt.

### Donderdag — Slecht (te weinig wind, hele dag)
- Windfinder: wind daalt de hele dag van ~7,8 naar 0,3 kts (gust max 11,4 kts), richting draait van west (240-268°) via zuid (190-227°) naar noord/oost (315-349°, 90-128° in de avond) — ruim binnen de Slecht-drempel (gust <16 én gem <14) de gehele dag.
- windwaarnemingen.nl (KNMI): bevestigt dit vrijwel exact — 1,6-10,7 kts gem., gust 4,1-14,8 kts, richting eveneens sterk wisselend (190-354°, later 12-103°). Geen enkel uur komt boven de Slecht-drempel uit.
- Pier-logica: niet van toepassing — wind is op geen moment bruikbaar sterk, en golf blijft klein (0,29-0,83m, onder de 0,8m pierdrempel voor het grootste deel van de dag).
- Golven (Windfinder, enige golfbron): 0,29-0,83m / 4,0-5,4s, afbouwend door de dag.
- Getij: laagwater 00:50 (0,33m), hoogwater 05:19 (2,2m), laagwater 13:12 (0,42m), hoogwater 17:36 (2,3m).
- Bronnen: **Windfinder en KNMI stemmen vrijwel volledig overeen** → hoog vertrouwen dat dit een windstille dag wordt. Soarcast niet beschikbaar deze run.

### Vrijdag — Slecht (te weinig wind, hele dag)
- windwaarnemingen.nl (KNMI, beschikbaar tot 15:00): wind blijft de hele ochtend/middag zwak, 3,3-8,4 kts gem., gust 4,5-13,2 kts, richting oost/zuidoost (85-161°, aflandig t.o.v. Zandvoort) — ruim binnen de Slecht-drempel.
- Windfinder bevestigt dit beeld voor de hele dag en loopt door tot de avond: 4,6-7,2 kts gem. overdag, in de avond een lichte opleving naar 6,4-6,7 kts gem. met gust tot 10,3-11,3 kts (richting 81-89°, pal aflandig) — blijft ruim onder de 15kts/16kts-drempel voor Matig/Goed.
- Pier-logica: niet van toepassing — windrichting is de hele dag pal- tot licht aflandig voor IJmuiden/Wijk aan Zee, en windkracht is sowieso te laag voor een bruikbare sessie.
- Golven (Windfinder, enige golfbron): 0,19-0,27m / 4,9-6,1s — zeer klein, de kleine swell van eerder deze week is volledig uitgedempt.
- Getij: laagwater 01:28 (0,33m), hoogwater 06:04 (2,08m), laagwater 13:57 (0,36m), hoogwater 18:20 (2,26m).
- Bronnen: **Windfinder en KNMI stemmen overeen** op een windstille dag → hoog vertrouwen. Soarcast niet beschikbaar deze run.

---

## 🔭 Kans op mooie sessies daarna (dag 4-9)
Windfinder (GFS, enige bron zo ver vooruit) voor **zaterdag 31 oktober t/m donderdag 5 november**:

- **Zaterdag 31 oktober**: wind blijft zwak (3,5-7,1 kts), richting oost (78-105°, aflandig) → **Slecht**, geen bruikbaar venster.
- **Zondag 1 november**: overdag nog zwak en wisselend (1,5-9,0 kts), maar in de avond trekt de wind duidelijk aan: 19:00 al 9,0 kts/gust 15,4 kts, 22:00 **14,5 kts gem./gust 20,8 kts**, richting draait naar noord/NNO (6-23°, side-shore) — een **grensgeval tussen Optimaal en Goed**: wind en richting zijn ideaal, maar de golf blijft klein (0,38-0,47m, ruim onder de 1,1m-drempel) waardoor het net geen Optimaal wordt.
- **Maandag 2 november — beste dag**: deze opbouw zet zich de hele dag door: wind 10,3-17,2 kts gem. (piekgust tot 23,9 kts rond het middaguur), richting vrijwel de hele dag 11-38° (NNO, nagenoeg exact side-shore t.o.v. Zandvoorts kustlijn), en de golf loopt op tot **0,81-0,90m met periode 5,6-6,4s** — ook hier **grensgeval Optimaal/Goed(a)**: wind, richting en periode zitten op Optimaal-niveau, alleen de golfhoogte blijft net (~0,2m) onder de 1,1m-drempel. Breedste venster van bruikbare wind: **ongeveer 04:00-19:00**.
- **Dinsdag 3 november**: wind valt terug naar 3,8-9,2 kts, golf ook kleiner (0,45-0,67m) → **Matig**, geen sterk venster.
- **Woensdag 4 november**: wind bouwt tegen de avond weer op (8,7 kts → 13,7 kts gem., gust tot 18,2 kts rond 22:00), richting noord (345-358°, side-shore), golf nog klein (0,41-0,5m) → **Matig**, met een oplevend venster richting de avond dat aansluit op...
- **Donderdag 5 november**: ...een dag die de hele dag door stevig blijft: 11,7-14,6 kts gem., gust 13,8-19,8 kts, richting noord (347-6°), golf 0,5-0,55m → opnieuw **Matig/grensgeval met Goed(b)**, wind en richting goed maar golf te klein.

**Beste dag: maandag 2 november**, met de kanttekening dat dit een grensgeval Optimaal/Goed(a) is (golf net onder de drempel) — en dat zondagavond 1 november en donderdag 5 november ook kansrijk zijn. Kans: **gemiddeld tot hoog** (deze periode laat voor het eerst in weken een aaneengesloten reeks dagen met bruikbare wind zien, maar het is nog 5+ dagen vooruit).
⚠️ Onzeker op 4+ dagen — check dichter bij de tijd opnieuw.

---
_Bronnen: Windfinder (GFS) · Soarcast (KNMI Harmonie, niet beschikbaar deze run) · windwaarnemingen.nl (KNMI, IJmuiden)_
