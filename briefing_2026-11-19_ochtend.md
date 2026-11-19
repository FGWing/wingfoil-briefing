# 🌊 Wingfoil-briefing Zandvoort–Wijk aan Zee
_19-11-2026 · Ochtendbriefing_

⚠️ **Technische kanttekening:** alle drie bronnen zijn deze run rechtstreeks via curl (geen browser) opgehaald. Windfinder: de embedded Astro-JSON (`ForecastSection` voor vandaag+morgen incl. golf/getij, `ForecastDataInit` voor dag 3 t/m 10) gedecodeerd. Soarcast: de pagina zelf is een lege JS-app, maar het onderliggende endpoint bleek deze run `plotPerLocAndUnitReact.php?json&jsonOnly&location=133&day=...&windUnits=kts&forecastToShow=harm&duringDayOnly=true&runsToShow=lastOnly` (apart aangeroepen voor wind/gust en, met `unit=deg`, voor windrichting) — de eerder gebruikte `forecastToShow=harmonie`-variant gaf dit keer onbruikbare (veel te lage) cijfers; een losse screenshot van de pagina zelf bevestigde welke variant wél klopt. windwaarnemingen.nl via `database/vsp_vdg_wstats.php?st=IJmuiden1` (vandaag, 10-min-actuals + eigen uurlijkse Harmonie-vsp) en `vsp_mrg_wstats.php?st=IJmuiden2` (morgen+overmorgen).

**Netto beeld — opnieuw een grote modelverdeeldheid, en de ochtend-actuals bevestigen wederom de lagere lijn.** Voor vandaag voorspellen Windfinder (GFS) en Soarcast (Harmonie, IJmond) een duidelijke middagpiek (resp. 20-23kts/27-28kts gust rond 10:00-13:00, en zelfs 24,7kts/32kts gust om 11:00), maar windwaarnemingen's eigen Harmonie-vsp voor het IJmuiden-station ziet een veel bescheidener dag met slechts een kort piekje van ~12kts/17,5kts gust om 11:00. De actuals van de afgelopen 2-3 uur volgen duidelijk de lage lijn (3,4-4,9kts, dalend) en liggen ruim onder zowel Windfinder als Soarcast se voorspelling voor diezelfde uren. Op basis daarvan: **donderdag (vandaag)** grotendeels **Slecht**, met een kort **Matig-grensgeval rond 10:00-12:00 bij IJmuiden** als het bescheiden piekje van windwaarnemingen standhoudt — de veel hogere Windfinder/Soarcast-cijfers voor diezelfde uren verdienen gezien het trackrecord van de laatste dagen weinig vertrouwen. **Vrijdag** is bij alle drie bronnen eensgezind **Slecht** (wind nergens boven ~11kts). **Zaterdag** kent weer een forse modelverdeeldheid rond 12:00-13:00 (Soarcast tot 15,9kts/20,7kts gust, Windfinder en windwaarnemingen beduidend zwakker) — **Slecht-tot-Matig**. In de outlook springt geen enkele dag er sterk uit; **dinsdag 24 november** is de meest kansrijke (gusty, Matig-grensgeval), de rest van de week blijft overwegend te zwak.

---

## ⚡ Snel overzicht
- **Donderdag:** **Slecht**, met een kort **Matig-grensgeval ±10:00-12:00 bij IJmuiden** (grote modelverdeeldheid, lagere windwaarnemingen-lijn door de ochtend-actuals bevestigd).
- **Vrijdag:** **Slecht** — wind te zwak bij alle drie bronnen (nergens boven ~11kts).
- **Zaterdag:** **Slecht-tot-Matig**, met een onopgeloste modelverdeeldheid rond **12:00-13:00** (Soarcast ziet daar tot 15,9kts/20,7kts gust, Windfinder/windwaarnemingen beduidend zwakker).
- **Beste dag in de 7 dagen erna:** dinsdag 24 november — Matig-grensgeval, gustyste/sterkste dag van een verder zwakke outlook-week.

---

## ⏰ Realitycheck vandaag
- Laatste actuele uren (04:00-06:10, windwaarnemingen.nl/IJmuiden, 10-min metingen): **gem. ≈3,4-4,9 kts** (dalend: 04:00-blok ≈4,6kts → 05:00-blok ≈3,4kts → 06:00-blok ≈3,6kts), gust **≈5,0-7,0 kts**, richting draaiend van **≈161° (ZZO) naar ≈138° (ZO)**.
- Was voorspeld: windwaarnemingen's eigen Harmonie-vsp zag voor dezelfde uren **2,6-5,1 kts gem., gust 6,8-7,4 kts, richting 142-182°** (ZUID/ZO) — redelijk vergelijkbaar, de actuals liggen aan de zwakke kant hiervan. Windfinder (GFS) zag voor diezelfde uren echter **9,1-11,9 kts gem., gust 15,1-18,9 kts**, richting 135-175° — ruim het dubbele van de werkelijkheid. Soarcast levert voor deze vroege uren geen data (alleen overdag, vanaf 08:00).
- Conclusie: de wind **KLOPT ongeveer (iets aan de zwakke kant)** met windwaarnemingen's eigen (lagere) Harmonie-voorspelling, maar loopt **FORS ACHTER** op de hogere voorspelling van Windfinder/GFS — dezelfde patroon als de afgelopen dagen. Rest-van-de-dag inschatting: **naar beneden bijgesteld** — voor de rest van vandaag volgen we de lagere windwaarnemingen/Soarcast-ochtendlijn in plaats van de (nog onbevestigde) sterke Windfinder/Soarcast-middagpiek van 20-32kts.

---

## 📅 Komende 72 uur

### Donderdag — Slecht, kort Matig-grensgeval ±10:00-12:00 bij IJmuiden
- Windfinder (GFS, 3-uurs): bouwt op naar **20,2kts gem./27,5kts gust om 10:00** (richting 224°, side-shore) en **23,3kts/27,9kts gust om 13:00** (richting 273°, pal aanlandig bij Zandvoort), zakt in de avond terug naar 11,6-13,7kts. Golf blijft de hele dag net onder de drempel: **0,86-1,06m**, periode 5,5-6,5s (nooit boven 1,1m).
- Soarcast (Harmonie, IJmond, uurlijks, 08:00-17:00): ziet een scherpe, korte piek — **24,7kts gem./32,1kts gust om 11:00** (richting 329°, NW), daarna weer snel terug naar 6-11kts vanaf 13:00. Let op: dit is bijna het dubbele van windwaarnemingen's eigen lijn voor exact hetzelfde uur.
- windwaarnemingen.nl (eigen Harmonie-vsp, IJmuiden): ziet een veel bescheidener dag — grotendeels **2,6-7,2kts gem.**, met een kort piekje van **12,3kts gem./17,5kts gust om 11:00** (richting 324°, NW/licht aanlandig bij Zandvoort), erna weer snel terug naar 3-5kts. **De actuals (zie Realitycheck) bevestigen deze lagere lijn, niet de hogere Windfinder/Soarcast-cijfers.**
- Netto — derde dag op rij met een forse, nog onopgeloste modelverdeeldheid (2-2,5x in windkracht), ditmaal ook met een duidelijk richtingsverschil (Windfinder ziet rond het middaguur zuidwest/west, Soarcast en windwaarnemingen zien juist noordwest). Op basis van de ochtend-realitycheck volgen we de lagere, bevestigde lijn: vóór en na ±10:00-12:00 is de wind te zwak (gust<16, gem<14 → **Slecht**); rond **10:00-12:00** is er een kort **Matig-grensgeval** (≈9-12kts gem., gust tot 17,5kts, golf net onder de drempel op 1,0m/5,8s) — bruikbaar voor lichter materiaal, maar wie op de hogere Windfinder/Soarcast-cijfers rekent (20-32kts) loopt het risico op een tegenvaller, al kan een fors sterkere gust (richting Soarcast's 32kts) niet volledig worden uitgesloten.
- Pier-logica: rond 10:00-12:00 is de richting (NW, 320-340° volgens de bevestigde lijn) bij **IJmuiden** (pierzone-hoek, pal aanlandig 240°) licht aanlandig met Zuidpier-bescherming; bij **Wijk aan Zee** (eigen hoek, pal aanlandig 283,8°) valt dezelfde richting binnen de pal-aanlandige band zonder bescherming. IJmuiden is dus de voorkeursplek in dit venster. Golf (≈1,0m) zit net boven de 0,8m-drempel voor vermelding.
- Getij: laagwater 06:12 (0,56m), hoogwater 10:47 (1,53m), laagwater 18:35 (0,38m), hoogwater ±22:00 (1,52m) — rond het middagvenster is het tij net gekeerd naar eb, dus relatief rustig.
- Beste venster: **±10:00-12:00 bij IJmuiden** — wind ≈9-12 kts, gust tot ≈17,5 kts, richting ≈320-340° (licht aanlandig, Zuidpier-bescherming). Golf ≈1,0m/5,8s — net onder de drempel. Marginaal, check de actuele gust vlak voor vertrek; de veel hogere Windfinder/Soarcast-cijfers voor dit venster zijn (nog) niet bevestigd.

### Vrijdag — Slecht, wind te zwak bij alle drie bronnen
- Windfinder (GFS, 3-uurs): wind zwak de hele dag (**1,4-10,8 kts gem.**, gust 3,2-12,9kts), richting draait van oost/zuidoost (60-116°, aflandig) 's ochtends naar noordwest (299-328°, aanlandig-ish) in de avond. Golf laag en afnemend: **0,45-0,76m**, periode 5,7-6,2s.
- Soarcast (Harmonie, IJmond, 08:00-17:00): vergelijkbaar zwak (**3,3-8,9 kts gem.**, gust 6,8-12,4kts), richting draait van zuidoost (131-135°) via zuid/west (163-264°) naar noordwest (297-308°) in de late middag.
- windwaarnemingen.nl (eigen Harmonie-vsp, IJmuiden): de zwakste van de drie — **1,3-6,4 kts gem.** vrijwel de hele dag, gust 3,1-9,4kts, richting vergelijkbaar draaiend (86-346°, via zuid en west naar noordwest in de avond).
- Netto — **alle drie bronnen eens: veel te weinig wind voor een bruikbare sessie**, de hele dag door. Golf blijft ruim onder de drempel. Classificatie: **Slecht**, geen grensgeval.
- Pier-logica: niet van toepassing (golf blijft onder 0,8m en de wind is sowieso te zwak om relevant te zijn).
- Getij: hoogwater 23:35 (nacht ervoor, 1,88m), laagwater 07:40 (0,51m), hoogwater 11:59 (1,61m), laagwater 19:49 (0,33m).
- Beste venster: **geen bruikbaar venster.** Wind blijft bij alle bronnen de hele dag te zwak.

### Zaterdag — Slecht-tot-Matig, modelverdeeldheid rond 12:00-13:00
- Windfinder (GFS, 3-uurs): wind zwak-tot-matig de hele dag (**7,9-11,6 kts gem.**, gust 9,7-14,2kts), richting vrijwel de hele dag noordwest/west (273-328°, pal- tot licht aanlandig bij Zandvoort). Golf net onder de drempel en licht oplopend: **0,69-0,91m**, periode 6,3-6,9s.
- Soarcast (Harmonie, IJmond, 08:00-15:00): ziet een duidelijk sterkere middag dan Windfinder — **9,1-15,9 kts gem., gust tot 20,7kts rond 13:00** (richting 260-300°, west/pal aanlandig bij Zandvoort).
- windwaarnemingen.nl (eigen Harmonie-vsp, IJmuiden, tot 15:00): de zwakste van de drie — **4,2-7,4 kts gem.**, gust 6,8-10,7kts, richting vergelijkbaar west/noordwest (262-329°).
- Netto — **opnieuw modelverdeeldheid, dit keer op zowel wind als getallen van Windfinder onderling vergelijkbaar met windwaarnemingen, maar Soarcast duidelijk hoger.** Zelfs in het gunstigste geval (Soarcast, 12:00-13:00: 12,7-15,9kts gem./16,4-20,7kts gust) blijft de golf (≈0,87-0,91m) onder de 1,1m-drempel, en is de richting (260-271°) bij Zandvoort/Wijk aan Zee pal aanlandig — dat zou in het beste geval een grensgeval Matig/Risico zijn, geen schoon venster. Windfinder en windwaarnemingen wijzen beide op een zwakkere, minder uitgesproken dag. Classificatie: **Slecht-tot-Matig**, met een onzeker (en bij bevestiging nog altijd marginaal) venster rond 12:00-13:00.
- Pier-logica: rond 12:00-13:00 valt de richting (260-275°) in de **neutrale zone tussen de twee pierassen (250-280°)** — geen duidelijk piervoordeel bij IJmuiden of Wijk aan Zee. Golf (≈0,87-0,91m) zit boven de 0,8m-drempel voor vermelding, maar zonder bescherming aan een van beide kanten is dit voor beide plekken een kwetsbaar venster bij pal aanlandige wind.
- Getij: hoogwater 00:33 (1,99m), laagwater 08:54 (0,43m), hoogwater 12:57 (1,76m), laagwater 20:52 (0,28m) — bij het middagvenster staat het net op hoogwater, dus zwaardere shorebreak dan bij eb.
- Beste venster: **onzeker — ±12:00-13:00** als Soarcast's hogere cijfers kloppen (wind 12,7-15,9kts, gust 16,4-20,7kts, richting 260-271° pal aanlandig, golf net onder de drempel, geen piervoordeel); als Windfinder/windwaarnemingen gelijk krijgen is de dag te zwak voor een goede sessie. Check dichter bij de tijd welke lijn het wint.

---

## 🔭 Kans op mooie sessies daarna (dag 4-9)
Windfinder (GFS, enige bron zo ver vooruit) voor **zondag 22 t/m vrijdag 27 november**.

- **Zondag 22 november**: wind zwak de hele dag (**2,7-6,7 kts gem.**, gust 3,4-7,4kts), richting wisselend (oost/noord). Golf laag (**0,57-0,69m**), periode 6,5-7,1s. Slecht — geen uitschieter.
- **Maandag 23 november**: wind blijft zwak (**1,4-10,7 kts gem.**, gust 1,8-13,7kts), met een bescheiden piekje rond 07:00-13:00 (richting 272-306°, west/noordwest, pal- tot licht aanlandig). Golf **0,51-0,57m**, periode ~6,5-7s. Slecht — wind blijft onder de bruikbare drempel.
- **Dinsdag 24 november** (dag 7): de sterkste en meest gusty dag van de outlook-periode — **10,3-13,4 kts gem.**, gust oplopend tot **21,2-24,5kts** in de avond (19:00/22:00), richting zuidoost/zuidzuidoost (127-165°, pal- tot licht aflandig bij Zandvoort — geen piervermelding nodig). Golf blijft laag (**0,44-0,48m**), periode 5,3-6,6s. Grensgeval Matig (gemiddelde wind net onder 14-15kts, maar met ongewoon hoge gust-factor) — beste dag van de periode, al geen schone classificatie.
- **Woensdag 25 november** (dag 8): vergelijkbaar windniveau (**10,9-13,9 kts gem.**, gust 15,5-24,8kts), richting oost/oostzuidoost (94-127°, aflandig). Golfperiode zakt grotendeels onder de 5s-drempel (3,8-5,0s), golf **0,41-0,46m**. Matig — zelfde gusty patroon als dinsdag, iets zwakker gemiddeld.
- **Donderdag 26 november** (dag 9): wind zwakt af (**7,9-9,5 kts gem.**, gust 10,4-14,3kts), richting oost (73-99°, aflandig). Golf laag (**0,38-0,41m**). Slecht.
- **Vrijdag 27 november**: wind blijft zwak (**6,8-9,8 kts gem.**, gust 8,8-14,8kts), richting oost/oostzuidoost (91-121°, aflandig). Golf **0,39-0,56m**. Slecht.

**Beste dag: dinsdag 24 november** — de sterkste en meest gusty dag van de hele outlook-periode, maar met een gemiddelde wind die net onder de 14-15kts-drempel blijft en een golf die ruim onder de 1,1m-drempel zit. Kans: **laag** — geen enkele dag in deze periode haalt een schone Goed- of Optimaal-classificatie; de hele week oogt structureel zwak. ⚠️ Onzeker op 4+ dagen — check dichter bij de tijd opnieuw. Let in latere runs vooral op: (1) of de forse modelverdeeldheid van de afgelopen drie dagen (Windfinder/Soarcast structureel hoger dan windwaarnemingen, telkens in het nadeel van de hogere cijfers beslecht) blijft aanhouden — dat pleit voor meer gewicht aan windwaarnemingen in komende briefings, en (2) of dinsdag 24 en woensdag 25 november alsnog golf boven de 1,1m-drempel krijgen.

---
_Bronnen: Windfinder (GFS) · Soarcast (KNMI Harmonie, IJmond) · windwaarnemingen.nl (KNMI, IJmuiden)_
