# 🌊 Wingfoil-briefing Zandvoort–Wijk aan Zee
_22-11-2026 · Ochtendbriefing_

⚠️ **Technische kanttekening:** alle drie bronnen zijn deze run rechtstreeks via curl (geen browser) opgehaald. Windfinder: de embedded Astro-JSON op de forecast-pagina gedecodeerd — het `ForecastSection`-component met `fcData`/`layoutData` (ICON-EU/Superforecast, uurlijks, vandaag+morgen+deel van overmorgen) én het `fcSectionData`-blok (GFS, 3-uurs, dekt dag 3 t/m 9 incl. golf/getij — bij eerste extractie bleek het attribuut langer dan de initiële regex-match, waardoor dag 25/27/29 aanvankelijk leeg leken; na correctie volledig gedecodeerd). Soarcast: endpoint `sc/plotPerLocAndUnitReact.php?json&jsonOnly&location=133&day=...&windUnits=kts&forecastToShow=harm&duringDayOnly=true&runsToShow=lastOnly` (wind/gust in kts, richting in graden). windwaarnemingen.nl via `database/vsp_vdg_wstats.php?st=IJmuiden1` (vandaag, 10-min-actuals t/m 06:10 + eigen uurlijkse vsp) en `vsp_mrg_wstats.php?st=IJmuiden2` (morgen+overmorgen).

**Netto beeld — een matige zondag (vandaag), een zwakke maandag, en een grensgeval-dinsdag met een pittige gust-factor vanaf de middag; de outlook valt deze run fors terug t.o.v. gisteravond.** Vandaag blijft de wind bij alle drie bronnen onder de 14kts-drempel maar met voldoende gust voor Matig. Maandag is overal zwak (ongewoon goede overeenstemming tussen de bronnen). Dinsdag bouwt de gust gestaag op tot 25,5kts terwijl het gemiddelde onder de 12kts blijft — een "pittige-gust-Matig". In de outlook is woensdag 25 november de sterkste dag, maar het hele blok dinsdag t/m donderdag is deze run een stuk kalmer dan de vorige-run-outlook liet zien, en zondag 29/maandag 30 november vallen terug naar vrijwel windstil.

---

## ⚡ Snel overzicht
- **Zondag:** **Matig** (±12:00-17:00) — alle drie bronnen blijven onder de 14kts-drempel, gust komt vanaf de ochtend geregeld boven 16kts uit.
- **Maandag:** **Slecht** — wind zwak de hele dag, ongewoon grote overeenstemming tussen Windfinder/Soarcast/windwaarnemingen.
- **Dinsdag:** **Matig** (grensgeval, pittige gust) — gemiddelde blijft onder 14kts, maar gust loopt 's avonds op tot 25,5kts; golf en periode te laag voor Goed(b).
- **Beste dag in de 7 dagen erna:** woensdag 25 november — sterkste en meest consistente wind van de outlook-periode, maar pal-aflandige richting en korte golfperiode houden dit een grensgeval.

---

## ⏰ Realitycheck vandaag
- Laatste actuele uren (04:00-06:10, windwaarnemingen.nl/IJmuiden, 10-min metingen): **gem. ≈2,8-6,0 kts** (gemiddeld over dat venster ≈4,8kts), gust **≈4,7-7,6 kts**, richting wisselend tussen OZO en ZO (**97-126°**), opvallend schokkerig (10-min-waarden sprongen soms van 1 naar 9kts).
- Was voorspeld: windwaarnemingen's eigen vsp zag voor 04:00/05:00/06:00 **3,3 / 3,3 / 2,9 kts gem.** (gust 5,6 / 5,8 / 4,9 kts), richting 124° / 127° / 111°. Windfinder (Superforecast/ICON-EU) zag voor diezelfde uren **4,3 / 5,5 / 6,4 kts gem.** (gust 4,8 / 6,1 / 8,0 kts).
- Conclusie: **wisselend beeld, geen eenduidige bias** — om 04:00-05:00 liep de actuele wind duidelijk **VOOR** op windwaarnemingen's eigen (lage) vsp (ca. +60-70%) en ook iets voor op Windfinder, maar om 06:00 viel de wind juist terug tot **ONDER** beide voorspellingen (2,8kts actueel vs 2,9-6,4kts voorspeld). Rest-van-de-dag inschatting: **ongewijzigd** — de Matig-middagpiek blijft het waarschijnlijkste beeld, met een iets ruimere onzekerheidsmarge gezien de schokkerige vroege ochtend.

---

## 📅 Komende 72 uur

### Zondag — Matig
- Windfinder (Superforecast/ICON-EU, uurlijks): wind bouwt op van 1,6-4,3 kts 's nachts naar **9,2-11,5 kts gem.** tussen ±10:00-18:00 (piek 11,5kts om 13:00), gust oplopend tot **17,0-19,7 kts** (piek 19,7kts om 21:00). Richting draait van WNW/ZW 's nachts (134-225°) naar ONO/OOST overdag (**58-90°**, aflandig tot licht aflandig). Golf blijft **0,56-0,69m**, periode ruim boven 5s (6,7-7,7s).
- Soarcast (Harmonie, IJmond, 08:00-17:00): bevestigt het matige beeld — **6,3-13,6 kts gem., gust 9,2-18,3 kts**, richting 55-87° (vergelijkbaar, ONO). Piek iets later (17:00) en iets hoger dan Windfinder.
- windwaarnemingen.nl (eigen Harmonie-vsp, IJmuiden): iets zwakker dan Windfinder — **2,9-10,5 kts gem.** (piek 17:00), gust 4,9-16,5kts, richting vergelijkbaar maar wisselvalliger (39-352°). De realitycheck-actuals liggen tussen deze lijn en Windfinder in.
- Netto — alle drie bronnen blijven de hele dag onder de 14kts-gemiddelde-drempel, maar gust komt vanaf ±09:00 geregeld boven de 16kts-Slecht-grens uit (tot ~18-20kts in de namiddag/avond) — dus geen Slecht, maar golf blijft overal ruim onder 1,1m, dus ook geen Optimaal/Goed(b): dit blijft overal **Matig**.
- Pier-logica: niet van toepassing (richting aflandig/licht aflandig, golf <0,8m).
- Getij: hoogwater ±01:21 (2,10m), laagwater ±09:53 (0,38m), hoogwater ±13:43 (1,92m), laagwater ±21:49 (0,26m).
- Beste venster: **±12:00-17:00** — wind 9-11,5 kts, gust 15-19,7 kts, richting 60-82° (aflandig/licht aflandig).

### Maandag — Slecht
- Windfinder (Superforecast/ICON-EU, uurlijks): wind blijft de hele dag zwak, **1,6-7,8 kts gem.** (hoogste waarde pas 's avonds om 23:00), gust **1,9-13,9 kts**. Richting draait langzaam van ONO (78°, aflandig) 's nachts naar ZZW/ZW (192-216°, side-shore) overdag/'s avonds. Golf **0,42-0,60m**, periode 6,6-7,1s.
- Soarcast (Harmonie, IJmond, 08:00-17:00): bevestigt de zwakte — **2,2-8,6 kts gem., gust 4,1-12,0 kts**, richting draait sterk (74° 's ochtends naar 292° WNW 's avonds).
- windwaarnemingen.nl (eigen Harmonie-vsp, IJmuiden): opnieuw de zwakste lijn, **1,4-8,6 kts gem.**, gust 2,3-12,2kts, richting vergelijkbare draai (48°→330°).
- Netto — alle drie bronnen eens: gust blijft de hele dag onder 16kts én gemiddelde onder 14kts, dus **Slecht**. Ongewoon goede overeenstemming tussen de bronnen deze dag.
- Pier-logica: niet van toepassing.
- Getij: hoogwater ±02:06 (2,19m), laagwater ±10:42 (0,39m), hoogwater ±14:27 (2,06m), laagwater ±22:45 (0,28m).
- Beste venster: **geen bruikbaar venster.**

### Dinsdag — Matig (grensgeval)
- Windfinder (hourly t/m 19:00, aangevuld met 3-uurs GFS): wind bouwt gestaag op van ~8kts 's nachts naar **10,0-11,9 kts gem.** in de namiddag/avond, met vanaf ±12:00 een oplopende gust tot **19,1-25,5 kts** om 19:00 — het gemiddelde blijft echter de hele dag onder 14kts. Richting draait van side-shore (ZUID, ~190°) 's nachts naar licht aflandig/pal aflandig (**122-152°**, ZZO/ZO) overdag. Golf blijft laag: **0,37-0,42m**, periode daalt van 7,0s 's nachts naar 4,6-4,8s 's avonds (onder de 5s-drempel).
- Soarcast (Harmonie, IJmond, 08:00-15:00, partieel): **7,5-11,6 kts gem., gust 12,2-16,1 kts**, richting 125-167° (ZZO/ZO) — bevestigt het ochtendbeeld, met een lagere gust-piek dan Windfinder.
- windwaarnemingen.nl (eigen Harmonie-vsp, IJmuiden): toont 's nachts (02:00-05:00) een kortstondige extra pittige pols — **8,7-12,8 kts gem., gust tot 18,6 kts**, richting ZW/ZZW (197-231°) — die Windfinder niet laat zien; overdag (08:00-15:00) sluit windwaarnemingen met **5,8-9,1 kts** weer dichter aan bij de andere twee bronnen (iets lager).
- Netto — grensgeval: het gemiddelde blijft overal onder 14kts (dus geen Optimaal/Goed), maar de gust loopt vanaf de middag flink op (tot 25,5kts) terwijl golf (0,37-0,42m) en periode (vanaf de avond <5s) ruim onder de Goed(b)-drempel blijven. Dit past niet precies in één hokje: een pittige-gust-**Matig**, met 's nachts bovendien een onopgeloste modelverdeeldheid bij windwaarnemingen.
- Pier-logica: niet van toepassing (golf <0,8m).
- Getij: hoogwater ±02:50 (2,23m), laagwater ±11:21 (0,41m), hoogwater ±15:09 (2,18m).
- Beste venster: **±16:00-19:00** — wind 10-11,9 kts, gust 21-25,5 kts, richting 122-127° (pal aflandig). Let op: stevige/pittige gust-factor, check dichter bij de tijd.

---

## 🔭 Kans op mooie sessies daarna (dag 4-9)
Windfinder (GFS, enige bron zo ver vooruit) voor **woensdag 25 t/m maandag 30 november**. Opvallend deze run: het hele blok is fors kalmer dan de vorige-run-outlook voor dezelfde periode (die zag toen 14-19kts op bijna elke dag) — met name dinsdag t/m donderdag vallen nu een stuk terug, en het weekend (zondag 29/maandag 30) wordt bijna windstil.

- **Woensdag 25 november** (dag 4): sterkste dag van de outlook-periode — **11,1-16,5 kts gem.**, gust **17,1-26,3kts**, richting pal aflandig (**81-116°**, ONO/OOST). Golf laag (**0,31-0,38m**), periode kort (2,96-4,26s, onder 5s). **Goed, grensgeval** — het gemiddelde komt ruim in de 14-25kts-band, maar Optimaal/Goed(a) zijn niet toegesneden op pal-aflandige wind (die vragen side-shore/licht-aflandig resp. licht-aanlandig), en Goed(b) vraagt golf >1,1m wat hier ontbreekt.
- **Donderdag 26 november** (dag 5): **10,6-13,7 kts gem.**, gust **15,1-24,0kts**, richting pal aflandig (**83-100°**, ONO). Golf **0,24-0,33m**, periode kort (3,12-3,78s). **Matig-tot-Goed grensgeval** — gemiddelde hangt net onder de 14kts-drempel.
- **Vrijdag 27 november** (dag 6): **9,6-11,7 kts gem.**, gust **13,2-18,3kts**, richting pal aflandig (**93-115°**). Golf zeer laag (**0,18-0,29m**), periode kort (2,78-3,73s). **Matig** — ruim binnen de band, geen grensgeval deze keer.
- **Zaterdag 28 november** (dag 7): **7,9-10,1 kts gem.**, gust **11,9-17,0kts**, richting pal aflandig/licht aflandig (**109-129°**). Golf **0,30-0,34m**, periode 3,53-4,76s. **Matig**, aan de zwakke kant.
- **Zondag 29 november** (dag 8): wind zeer zwak en wisselend — **0,6-8,3 kts gem.(!)**, gust **0,6-12,7kts**, richting chaotisch (32-179°, vrijwel windstil rond 13:00). Golf **0,47-0,51m**. **Slecht**.
- **Maandag 30 november** (dag 9): **4,4-6,4 kts gem.**, gust **5,2-8,9kts**, richting NO/ONO (43-103°). Golf **0,56-0,62m** (hoogste van de outlook-periode, nog steeds ruim onder 1,1m). **Slecht**.

**Beste dag: woensdag 25 november** — duidelijk de sterkste en meest consistente dag van de hele outlook-periode, al blijven de pal-aflandige richting en de korte golfperiode een handicap voor een formele Optimaal-classificatie. Kans: **gemiddeld** — sterkste dag van de week, maar het hele blok is fors zwakker dan de vorige-run-outlook liet zien voor dezelfde periode, vooral dinsdag t/m donderdag. ⚠️ Onzeker op 4+ dagen — check dichter bij de tijd opnieuw.

---
_Bronnen: Windfinder (GFS / Superforecast ICON-EU) · Soarcast (KNMI Harmonie, IJmond) · windwaarnemingen.nl (KNMI, IJmuiden)_
