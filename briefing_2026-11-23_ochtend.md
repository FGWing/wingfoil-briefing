# 🌊 Wingfoil-briefing Zandvoort–Wijk aan Zee
_23-11-2026 · Ochtendbriefing_

⚠️ **Technische kanttekening:** alle drie bronnen zijn deze run rechtstreeks via curl (geen browser) opgehaald. Windfinder: de embedded Astro-JSON gedecodeerd — `ForecastSection`/`ForecastDataInit` op zowel de forecast- als de Superforecast-pagina (hourly ICON-EU-achtige data voor vandaag t/m woensdag, GFS 3-uurs voor donderdag t/m dinsdag 1 dec, incl. golf/getij). Soarcast: endpoint `plotPerLocAndUnitReact.php` met `unit=deg` (richting) en `unit=m/s&windUnits=kts` (wind/gust, kts). windwaarnemingen.nl via `vsp_vdg_wstats.php?st=IJmuiden1` (vandaag, 10-min-actuals t/m 06:10 + eigen uurlijkse vsp) en `vsp_mrg_wstats.php?st=IJmuiden2` (morgen+overmorgen).

**Netto beeld — een windstille maandag (vandaag), een pittige-gust-grensgeval-dinsdag, en een stevige, consistente woensdag die de beste dag van de hele 72-uursperiode is.** Vandaag blijft de wind bij alle bronnen de hele dag onder de Slecht-drempel, en de vroege-ochtend-actuals vallen zelfs nog onder de toch al zwakke voorspelling. Dinsdag bouwt de wind pas laat op naar 14kts gemiddeld, met een fors oplopende gust (tot 29kts) die niet in één hokje past. Woensdag is de uitschieter: 14-18kts gemiddeld vrijwel de hele dag bij alle drie bronnen, maar de zuiver aflandige hoek en korte golfperiode houden dit een "Goed, grensgeval" in plaats van Optimaal. In de outlook is donderdag 26 november de beste dag van het blok dag 4-9, waarna het weekend en begin volgende week terugvallen naar (bijna) windstil.

---

## ⚡ Snel overzicht
- **Maandag:** **Slecht** — wind blijft de hele dag onder de 14kts/16kts-gust-drempel, ochtend-actuals bevestigen dit.
- **Dinsdag:** **Matig** (grensgeval, pittige gust) — gemiddelde haalt pas rond 20:00-22:00 kort 14kts, maar de gust loopt dan al op tot 28-29kts.
- **Woensdag:** **Goed** (grensgeval) — stevige, consistente 14-18kts vrijwel de hele dag, maar pal-aflandige richting en korte golfperiode passen niet bij Optimaal.
- **Beste dag in de 7 dagen erna:** donderdag 26 november — sterkste dag van de outlook-periode, al blijft het door de aflandige richting en korte golfperiode een grensgeval.

---

## ⏰ Realitycheck vandaag
- Laatste actuele uren (04:00-06:10, windwaarnemingen.nl/IJmuiden, 10-min metingen): **gem. ≈0,8-2,2 kts** (gemiddeld over dat venster ≈1,5kts), gust **≈1,2-3,0 kts**, richting wisselend tussen NNO en OOST (**18-90°**).
- Was voorspeld: windwaarnemingen's eigen vsp zag voor 04:00/05:00/06:00 **5,2 / 1,7 / 1,7 kts gem.** (gust 8,2 / 7,8 / 3,1 kts), richting 46° / 91° / 51°. Windfinder (Superforecast, hourly) zag voor diezelfde uren **4,6 / 5,2 / 6,9 kts gem.** (gust 6,1 / 7,3 / 12,3 kts), richting 50° / 36° / 35°.
- Conclusie: de wind loopt duidelijk **ACHTER** op beide voorspellingen — de actuals (0,8-2,2kts) liggen onder zowel windwaarnemingen's eigen (al lage) vsp als onder Windfinder's iets hogere voorspelling. Rest-van-de-dag inschatting: **ongewijzigd/licht bevestigd** — maandag was al overal als Slecht geclassificeerd (gust blijft de hele dag onder de 16kts-grens bij alle bronnen), en deze zwakke ochtend-actuals maken een opleving later vandaag eerder minder dan meer waarschijnlijk.

---

## 📅 Komende 72 uur

### Maandag — Slecht
- Windfinder (Superforecast, hourly): wind blijft de hele dag zwak, **3,6-8,1 kts gem.** (hoogste waarden rond middernacht, nu al gepasseerd), gust **3,6-15,9 kts** (piek net voor/na middernacht; overdag max ~12,3kts om 06:00). Richting erg wisselend: draait van ONO/OOST 's nachts (35-106°, aflandig) naar ZZO/ZZW/WZW overdag/'s avonds (143-227°, richting side-shore/licht aanlandig). Golf **0,39-0,57m**, periode 6,5-7,1s (ruim boven 5s, maar golf te laag voor Optimaal/Goed(b)).
- Soarcast (Harmonie, IJmond, 08:00-17:00): ziet een duidelijkere middagpiek dan Windfinder — **3,7-9,8 kts gem., gust 6,2-13,4 kts** (Windfinder zelfde uren: 3,6-5,7kts gem., gust 3,6-6,5kts) — expliciete afwijking tussen de modellen, Soarcast ligt in de middag een stuk hoger. Richting 187-257° (ZUID/WZW), ~20-30° westelijker dan Windfinder in dezelfde uren.
- Netto — ondanks de afwijking tussen Windfinder en Soarcast blijft de gust bij beide ruim onder de 16kts-Slecht-grens en het gemiddelde onder 14kts: overal **Slecht**, de hele dag. De realitycheck (zie boven) bevestigt dit beeld eerder dan dat hij het tegenspreekt.
- Pier-logica: niet van toepassing (richting niet aanlandig, en golf blijft onder 0,8m).
- Getij: hoogwater ±02:06 (2,19m), laagwater ±10:42 (0,39m), hoogwater ±14:27 (2,06m), laagwater ±22:45 (0,28m).
- Beste venster: **geen bruikbaar venster.** (windwaarnemingen's eigen vsp laat 's avonds laat, rond 23:00-24:00, een kleine gust-piek tot 16,5-17,5kts zien die Windfinder niet in dezelfde mate bevestigt — te laat en te onzeker om als venster te tellen.)

### Dinsdag — Matig (grensgeval, pittige gust)
- Windfinder (Superforecast, hourly): wind bouwt gestaag op van ~8kts 's nachts naar **12,4-14,3 kts gem.** in de avond (piek ±20:00-21:00), terwijl de gust al vanaf ±07:00 de 16kts-grens doorbreekt en 's avonds oploopt tot **28,1-29,0 kts**. Richting draait van side-shore/ZZW 's nachts (186-206°) naar pal aflandig (OZO/OOST, **105-123°**) overdag/'s avonds. Golf blijft laag: **0,34-0,38m**, periode kort en dalend (3,3-7,0s, onder 5s vanaf de namiddag).
- Soarcast (Harmonie, IJmond, 08:00-17:00): bevestigt de opbouw — **8,8-16,6 kts gem., gust 12,1-22,9 kts**, richting 109-153° (~15-30° oostelijker/zuidelijker dan Windfinder, maar dezelfde trend).
- windwaarnemingen.nl (eigen Harmonie-vsp, IJmuiden): iets lagere gust dan Windfinder — **6,0-13,0 kts gem., gust 9,7-21,2 kts**, richting vergelijkbaar (96-206°).
- Netto — grensgeval: het gemiddelde haalt pas kort (±20:00-22:00) de 14kts-grens, maar de gust is dan al fors hoger (28-29kts) dan de Matig/Goed(b)-drempel van 19kts, terwijl golf/periode te laag blijven voor Optimaal/Goed(b) en de richting (pal aflandig) niet past bij Goed(a)'s "licht aanlandig". Dit is dezelfde pittige-gust-situatie als in de vorige-run-outlook voor deze dag: een **Matig**-grensgeval met een stevige, mogelijk onveilige gust-factor — check dichter bij de tijd.
- Pier-logica: niet van toepassing (richting aflandig/side-shore, niet aanlandig).
- Getij: hoogwater ±02:50 (2,23m), laagwater ±11:21 (0,41m), hoogwater ±15:09 (2,18m); rond 19:00-20:00 een zwak secundair signaal (mogelijk dubbelhoogwater-effect, ±0,97-0,99m).
- Beste venster: **±19:00-22:00** — wind 12,4-14,3 kts, gust 28,1-28,9 kts, richting 105-121° (pal aflandig). Let op: zeer pittige gust-factor, houd een stevige veiligheidsmarge aan.

### Woensdag — Goed (grensgeval)
- Windfinder (Superforecast, hourly t/m 19:00): stevige, consistente wind: **13,7-17,7 kts gem.**, gust **22,0-30,6 kts**, richting vrijwel de hele dag pal aflandig (OOST/ONO, **85-117°**). Golf laag: **0,32-0,39m**, periode kort (2,64-3,33s, ruim onder 5s).
- Soarcast (Harmonie, IJmond, 08:00-15:00, partieel): duidelijk hoger gemiddelde dan Windfinder — **18,0-21,9 kts gem., gust 24,8-30,1 kts** (Windfinder zelfde uren: 15,0-16,4kts gem.) — expliciete afwijking, Soarcast ziet deze dag nog pittiger. Richting 73-86° (ONO), iets noordelijker dan Windfinder.
- windwaarnemingen.nl (eigen Harmonie-vsp, IJmuiden, 00:00-15:00): **13,2-18,1 kts gem., gust 20,2-29,0 kts**, richting 74-96° — ligt tussen Windfinder en Soarcast in, bevestigt de algemene sterkte van de dag.
- Netto — het gemiddelde zit bij alle drie bronnen solide in de 14-25kts-band, maar de richting is overal pal aflandig (binnen ~30° van Zandvoort's pal-aflandige hoek 107,5°) — dit past niet bij Optimaal (vraagt side-shore/licht aflandig) of Goed(a) (vraagt licht aanlandig). Golf blijft laag en periode kort, wat ook Goed(b) uitsluit (vraagt golf >1,1m). Netto dus een **Goed, grensgeval**: de windkracht zelf is prima wingfoilbaar en zeer consistent tussen de bronnen, maar de formele classificatie wringt door de zuivere aflandige hoek en de korte, platte golfslag.
- Pier-logica: niet van toepassing (richting aflandig, niet aanlandig).
- Getij: laagwater ±23:40 (0,31m, nacht van dinsdag op woensdag), hoogwater ±03:34 (2,22m), laagwater ±11:50 (0,41m), hoogwater ±15:53 (2,26m).
- Beste venster: **±09:00-14:00** — wind 15,0-17,7 kts (Soarcast zelfs 18-21,9 kts), gust 22,0-30,6 kts, richting 89-93° (pal aflandig, OOST). Stevige dag; houd rekening met de forse gust.

---

## 🔭 Kans op mooie sessies daarna (dag 4-9)
Windfinder (GFS, enige bron zo ver vooruit) voor **donderdag 26 november t/m dinsdag 1 december**.

- **Donderdag 26 november** (dag 4): **12,1-15,4 kts gem.**, gust **19,0-24,6 kts**, richting licht aflandig/pal aflandig (**78-97°**, ONO/OOST). Golf laag (**0,18-0,32m**), periode kort (2,67-4,06s). **Matig-tot-Goed grensgeval** — het gemiddelde kruist af en toe kort de 14kts-grens, maar blijft meestal net onder.
- **Vrijdag 27 november** (dag 5): **7,7-10,7 kts gem.**, gust **11,6-17,3 kts**, richting pal aflandig (**97-122°**). Golf zeer laag (**0,15-0,20m**), periode kort (3,28-4,38s). **Matig**, aan de zwakke kant.
- **Zaterdag 28 november** (dag 6): **9,6-13,6 kts gem.**, gust **14,4-23,5 kts**, richting licht aflandig (**128-147°**, draaiend richting side-shore). Golf **0,19-0,35m**, periode 3,94-5,54s (kruist rond de middag kort de 5s-drempel, maar golf blijft ruim onder 1,1m). **Matig**, 's avonds de sterkste van deze dag.
- **Zondag 29 november** (dag 7): wind stort in de loop van de dag in — **1,5-12,9 kts gem.(!)**, gust **1,5-22,0 kts**, richting draait van ZZO (152°) naar bijna stil en terug naar ZZW. Golf **0,38-0,51m**. **Slecht** (met een korte pittige-gust-episode 's nachts).
- **Maandag 30 november** (dag 8): **2,6-9,5 kts gem.**, gust **3,3-13,0 kts**, richting wisselend (290-356°, NW/N). Golf **0,53-0,65m** (hoogste van de outlook-periode, nog steeds ruim onder 1,1m). **Slecht**.
- **Dinsdag 1 december** (dag 9): **5,0-8,0 kts gem.**, gust **6,9-11,5 kts**, richting WZW/ZW (236-268°). Golf **0,57-0,61m**. **Slecht**.

**Beste dag: donderdag 26 november** — duidelijk de sterkste en meest bruikbare dag van het blok dag 4-9, al blijft de licht-aflandige/pal-aflandige richting en de korte golfperiode een grensgeval-handicap voor een formele Goed-classificatie. Kans: **gemiddeld** — de rest van de week (vrijdag t/m dinsdag) is duidelijk zwakker, met name het weekend en begin volgende week vallen terug naar (bijna) windstil. ⚠️ Onzeker op 4+ dagen — check dichter bij de tijd opnieuw.

---
_Bronnen: Windfinder (GFS / Superforecast ICON-EU) · Soarcast (KNMI Harmonie, IJmond) · windwaarnemingen.nl (KNMI, IJmuiden)_
