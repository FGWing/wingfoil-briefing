# 🌊 Wingfoil-briefing Zandvoort–Wijk aan Zee
_21-11-2026 · Ochtendbriefing_

⚠️ **Technische kanttekening:** alle drie bronnen zijn deze run rechtstreeks via curl (geen browser) opgehaald. Windfinder: de embedded Astro-JSON gedecodeerd — op de forecast-pagina (`/forecast/...`) staat het `ForecastSection`-component met ingebouwde `fcData` voor vandaag+morgen (uurlijks via het hogere-resolutie Superforecast/ICON-EU-model, ook te vinden op de Superforecast-pagina zelf) én een apart `fcSectionData`-blok (GFS, 3-uurs) dat de hele 10-daagse reeks bevat; voor dag 1-3 is bewust de fijnere Superforecast/ICON-EU-laag gebruikt, voor dag 4-9 de GFS-laag (enige bron die zo ver komt). Soarcast: endpoint `sc/plotPerLocAndUnitReact.php?json&jsonOnly&location=133&day=...&windUnits=kts&forecastToShow=harm&duringDayOnly=true&runsToShow=lastOnly&unit=m/s` (wind/gust) en `&unit=deg` (richting). windwaarnemingen.nl via `database/vsp_vdg_wstats.php?st=IJmuiden1` (vandaag, 10-min-actuals t/m 06:10 + eigen uurlijkse vsp) en `vsp_mrg_wstats.php?st=IJmuiden2` (morgen+overmorgen).

**Netto beeld — een zwakke zaterdag, een grensgeval-zondag met flinke modelspreiding, een rustige maandag, en in de verre outlook een opvallend winderig blok (dinsdag 24 t/m zondag 29 november) waarbij golfhoogte steeds de beperkende factor blijft.** Vandaag (zaterdag) blijft de wind bij alle drie bronnen te zwak om boven Slecht uit te komen; de ochtend-realitycheck bevestigt dat Windfinder's hogere cijfers niet worden gehaald. Zondag is een grensgeval-Matig met een opvallend grote spreiding tussen de drie bronnen (Windfinder ziet een pittige middag, Soarcast en windwaarnemingen fors minder). Maandag is opnieuw zwak. In de outlook valt op dat vrijwel elke dag van dinsdag t/m zondag sterke, gestaag aflandige wind laat zien (vaak 14-19kts, gust tot 32kts!) — maar de golfhoogte blijft de hele week onder de 0,6m, ruim onder de 1,1m-drempel, waardoor geen enkele dag de formele Optimaal/Goed(b)-lat haalt. Zondag 29 november springt er het sterkst uit (17-19kts de hele dag, als enige dag met golfperiode structureel ≥5s).

---

## ⚡ Snel overzicht
- **Zaterdag:** **Slecht** — wind blijft bij alle drie bronnen te zwak (nergens gelijktijdig gust≥16/gem≥14); realitycheck bevestigt dat Windfinder's hogere cijfers niet gehaald worden.
- **Zondag:** **Matig** (grensgeval richting Goed rond 10:00-14:00) — grote modelspreiding: Windfinder ziet 10-13,5kts/tot 20kts gust, Soarcast en windwaarnemingen fors minder.
- **Maandag:** **Slecht** — wind zwak en wisselend de hele dag bij alle bronnen.
- **Beste dag in de 7 dagen erna:** zondag 29 november — sterkste en meest consistente wind van de hele outlook-periode (17-19kts, gust tot 32kts), maar golf blijft met 0,46-0,54m ruim onder de 1,1m-drempel.

---

## ⏰ Realitycheck vandaag
- Laatste actuele uren (04:00-06:10, windwaarnemingen.nl/IJmuiden, 10-min metingen): **gem. ≈3,7-9,5 kts** (gemiddeld ≈5,2kts), gust **≈4,9-11,4 kts** (gemiddeld ≈6,9kts), richting draaiend van **NW (≈353°) naar WEST (≈272°)**.
- Was voorspeld: windwaarnemingen's eigen Harmonie-vsp zag voor dezelfde uren (04:00-06:00) **4,4-4,9 kts gem., gust 6,8-7,6 kts, richting 294-302°** (WNW) — de actuals liggen hier dicht bij, iets variabeler door de draaiende richting. Windfinder (Superforecast/ICON-EU) zag voor diezelfde uren juist **8,0-8,7 kts gem., gust 12,0-12,8 kts** — bijna het dubbele van de werkelijke gust.
- Conclusie: windwaarnemingen's eigen (lage) voorspelling **KLOPT ongeveer**, maar Windfinder's hogere lijn **loopt FORS ACHTER** op de realiteit. Rest-van-de-dag inschatting: **bijgesteld naar de lagere/bevestigde lijn** — dit versterkt het Slecht-oordeel voor vandaag eerder dan het te ondermijnen (Windfinder's cijfers waren al te zwak voor meer dan Slecht, en nu blijkt zelfs die lijn nog optimistisch).

---

## 📅 Komende 72 uur

### Zaterdag — Slecht
- Windfinder (Superforecast/ICON-EU, uurlijks): wind blijft de hele dag **5,3-12,3 kts gem.** (piek 12,3kts om 13:00), gust **7,2-12,8 kts**, richting overwegend **pal aanlandig voor Zandvoort, 263-350°** (WNW/NW, draaiend). Golf **0,63-0,88m**, periode 4,3-6,8s (grotendeels ≥5s vanaf de ochtend).
- Soarcast (Harmonie, IJmond, 08:00-17:00): bevestigt een vergelijkbaar zwak beeld — **5,1-12,6 kts gem., gust 11,1-18,2 kts**, richting 270-312° (WNW/NW). Iets hogere gust-piek dan Windfinder rond 13:00, maar per saldo hetzelfde zwakke verhaal.
- windwaarnemingen.nl (eigen Harmonie-vsp, IJmuiden): de hele dag zwak, **1,9-6,4 kts gem.**, gust 3,6-9,2kts, richting vergelijkbaar WNW/NW (120-316°, met uitschieter OZO laat op de dag). **De realitycheck-actuals bevestigen deze lagere lijn.**
- Netto — alle drie bronnen zijn het eens: de hele dag blijft gust<16kts én gem<14kts, dus **Slecht**. Zelfs Windfinder's eigen hoogste uur (13:00, 12,3/12,6kts) komt niet in de buurt van de drempel.
- Pier-logica: richting is het grootste deel van de dag pal aanlandig bij Zandvoort/Wijk aan Zee (260-320°) en golf bereikt 0,8-0,88m tussen ±08:00-16:00 (dus net over de 0,8m-drempel) — golfrichting clustert rond 344-350° (NW/N), wat **IJmuiden (Zuidpier)** een licht voordeel geeft. Gezien de zwakke wind is dit vooral theoretisch relevant.
- Getij: hoogwater ±00:33 (1,99m), laagwater ±08:54 (0,43m), hoogwater ±12:57 (1,76m), laagwater ±20:52 (0,28m).
- Beste venster: **geen bruikbaar venster.**

### Zondag — Matig
- Windfinder (Superforecast/ICON-EU, uurlijks): wind bouwt op van ≈4-5kts 's nachts naar **10,4-13,5 kts gem.** tussen 10:00-14:00 (piek 13,5kts om 12:00), gust oplopend tot **17,8-20,1 kts**, richting **70-113°** (aflandig/licht aflandig, ONO). Golf blijft laag: **0,56-0,68m**, periode 6,7-7,6s (ruim boven 5s).
- Soarcast (Harmonie, IJmond, 08:00-17:00): ziet een duidelijk zwakkere middag — **6,5-9,1 kts gem., gust 8,6-13,4 kts**, richting vergelijkbaar (54-91°, ONO). Bevestigt de richting, niet de kracht van Windfinder.
- windwaarnemingen.nl (eigen Harmonie-vsp, IJmuiden): opnieuw de zwakste van de drie — **1,7-5,4 kts gem.**, gust 2,2-8,3kts, richting vergelijkbaar (39-155°). Derde bron op rij die fors onder Windfinder blijft.
- Netto — grote modelspreiding: op basis van Windfinder's piek (10:00-14:00) wordt de 14kts-drempel net niet gehaald (max 13,5kts gem.) en blijft golf (0,56-0,58m) ruim onder 1,1m, dus geen Optimaal/Goed(b); dit zou een schoon **grensgeval Matig-naar-Goed(a)** zijn. Maar Soarcast én windwaarnemingen bevestigen die piek niet — bij voorzichtige lezing blijft het een rustige **Matig**-middag. Richting is aflandig, dus schoon water.
- Pier-logica: niet van toepassing (golf blijft onder 0,8m, richting aflandig).
- Getij: hoogwater ±01:21 (2,10m), laagwater ±09:53 (0,38m), hoogwater ±13:43 (1,92m), laagwater ±21:49 (0,26m).
- Beste venster: **±10:00-14:00** — wind 10-13,5 kts (Windfinder) / 7-9 kts (Soarcast/windwaarnemingen fors lager), gust 13-20 kts, richting 70-77° (aflandig, ONO). Check dichter bij de tijd welke lijn gelijk krijgt.

### Maandag — Slecht
- Windfinder (Superforecast/ICON-EU, uurlijks, t/m 19:00): wind blijft de hele dag zwak en wisselend, **3,5-7,8 kts gem.**, gust **3,6-18,4 kts** (enige uitschieter: 00:00-01:00 nog een gusty restant van zondagavond, daarna snel wegvallend). Richting draait sterk: van **76-115°** (aflandig, OZO/ONO) 's nachts naar **182-216°** (side-shore, vrijwel exact evenwijdig aan de kust) vanaf de middag. Golf blijft laag: **0,44-0,58m**, periode 6,5-7,5s.
- Soarcast (Harmonie, IJmond, 08:00-15:00): bevestigt de zwakte — **1,0-6,0 kts gem., gust 4,5-10,4 kts**, richting erg wisselend/onbetrouwbaar bij deze lage windsterktes (0-360°, bijna stilstand).
- windwaarnemingen.nl (eigen Harmonie-vsp, IJmuiden): opnieuw de zwakste lijn, **0,3-4,4 kts gem.**, gust 1,1-6,6kts, richting eveneens wisselend (1-329°).
- Netto — alle drie bronnen eens: wind blijft de hele dag ruim onder de Slecht-drempel (gust<16kts, gem<14kts), dus **Slecht**. De draai naar side-shore (180-216°) rond het middaguur is op zich gunstig qua schoon water, maar irrelevant zolang de wind zo zwak blijft.
- Pier-logica: niet van toepassing (golf blijft onder 0,8m).
- Getij: hoogwater ±02:06 (2,19m), laagwater ±10:42 (0,39m), hoogwater ±14:27 (2,06m).
- Beste venster: **geen bruikbaar venster.**

---

## 🔭 Kans op mooie sessies daarna (dag 4-9)
Windfinder (GFS, enige bron zo ver vooruit) voor **dinsdag 24 t/m zondag 29 november**. Opvallend deze run: vrijwel de hele week laat sterke, gestaag aflandige wind zien — maar de golfhoogte blijft steeds (ver) onder de 1,1m-drempel, waardoor geen dag formeel Optimaal of Goed(b) haalt. De categorieën "Optimaal"/"Goed(a)" zijn bovendien niet helemaal toegesneden op pal-aflandige wind (ze noemen side-shore/licht-aflandig resp. licht-aanlandig); waar dat speelt is dit als grensgeval benoemd.

- **Dinsdag 24 november** (dag 4): sterk en consistent de hele dag — **14,2-15,6 kts gem.**, gust **20,6-27,4kts**, richting pal aflandig (**122-137°**, OZO). Golf blijft echter laag (**0,35-0,40m**), periode wisselend (4,0-7,2s, 's ochtends beter). **Goed, grensgeval richting Optimaal** — wind ruim voldoende en schoon aflandig water, alleen golfhoogte ontbreekt. Dit is een forse opwaardering t.o.v. de vorige run (die zag 13,5-16,0kts voor deze dag, nu dus sterker en nog consistenter).
- **Woensdag 25 november** (dag 5): net onder de 14kts-drempel — **11,7-14,4 kts gem.**, gust **20,3-24,3kts**, richting pal aflandig (**80-112°**, ONO/OOST). Golf laag (**0,30-0,34m**), periode merendeels onder 5s (2,9-4,0s). **Matig-tot-Goed grensgeval** — wind hangt net rond de drempel, golf en periode blijven tekort.
- **Donderdag 26 november** (dag 6): sterk, met de laagste golf van de hele periode — **13,4-15,3 kts gem.**, gust **20,4-26,2kts**, richting pal aflandig (**67-92°**, ONO/OOST). Golf zeer laag (**0,20-0,26m**), periode onder 5s (3,4-3,9s). **Goed, grensgeval richting Optimaal**, net als dinsdag — sterke, schone aflandige wind maar vlak water. Forse opwaardering t.o.v. de vorige run (die zag slechts 8,2-10,0kts/Slecht voor deze dag).
- **Vrijdag 27 november** (dag 7): iets wisselvalliger — **10,6-13,0 kts gem.**, gust **18,7-24,2kts**, richting pal aflandig (**84-107°**, ONO). Golf **0,20-0,34m**, periode onder 5s (2,6-4,2s). **Matig**, met pittige gust-factor (gust vaak ruim boven de Matig-drempel van 19kts terwijl het gemiddelde eronder blijft — grensgeval).
- **Zaterdag 28 november** (dag 8): bouwt gestaag op tot een stevige avond — **11,4-17,7 kts gem.**, gust tot **31,9kts(!)** tegen de avond, richting pal aflandig (**81-178°**, draaiend van ONO 's ochtends richting side-shore in de avond). Golf blijft laag maar loopt wel op (**0,37-0,49m**), periode nadert 5s laat op de dag (3,6-5,1s). **Goed, grensgeval richting Optimaal** in de namiddag/avond — fors andere uitkomst dan de vorige run (die zag 13,5-14,4kts aanlandig met golf net onder 1,1m voor deze dag; nu een compleet ander windregime met veel hogere gust en aflandige richting — op 8 dagen vooruit dus met de nodige onzekerheid).
- **Zondag 29 november** (dag 9): de sterkste en meest consistente dag van de hele periode — **17,1-19,2 kts gem.** de hele dag, gust **26,5-32,1kts**, richting pal aflandig (**86-99°**, ONO). Golf **0,46-0,54m** — nog steeds ruim onder 1,1m, maar als enige dag met periode structureel **≥5s (5,3-5,8s)**. **Goed, grensgeval richting Optimaal** — sterkste wind van de week, enige die ook op periode voldoet, maar golfhoogte blijft de beperkende factor. Ook dit is een forse wijziging t.o.v. de vorige run (die zag een side-shore Goed(b)-match met golf juist wél over de drempel, 1,08-1,21m) — op 9 dagen vooruit een stevige modelwijziging.

**Beste dag: zondag 29 november** — sterkste en meest consistente wind van de hele outlook-periode, en de enige dag met voldoende golfperiode; golfhoogte blijft echter het hele blok (dinsdag t/m zondag) de beperkende factor. Kans: **gemiddeld tot hoog** — zes dagen op rij met stevige, schone aflandige wind is een duidelijke verbetering t.o.v. de structureel zwakke afgelopen weken, maar vrijwel elke dag is op golfhoogte een grensgeval en de cijfers zijn sinds de vorige run (vooral voor zaterdag 28 en zondag 29) al flink verschoven. ⚠️ Onzeker op 4+ dagen — check dichter bij de tijd opnieuw.

---
_Bronnen: Windfinder (GFS / Superforecast ICON-EU) · Soarcast (KNMI Harmonie, IJmond) · windwaarnemingen.nl (KNMI, IJmuiden)_
