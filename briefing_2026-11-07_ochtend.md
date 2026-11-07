# 🌊 Wingfoil-briefing Zandvoort–Wijk aan Zee
_07-11-2026 · Ochtendbriefing_

⚠️ **Technische kanttekening:** Windfinder opgehaald via de embedded Astro-JSON op de reguliere forecast-pagina (`FcTableWindpreviewContainer`, wind-only, 3-uurs stappen, dag 1-10) gecombineerd met `ForecastDataInit` (golf+getij) van zowel de forecast- als de weatherforecast-pagina. Opvallend: `ForecastDataInit` dekt op geen van beide pagina's vandaag (7 nov) — voor de golf/getij van vandaag is daarom eenmalig de gerenderde pagina (via Playwright) gebruikt i.p.v. de JSON-props. Soarcast via `/sc/plotPerLocAndUnitReact.php?json&jsonOnly&unit=m/s...` (snelheid/gust) plus `unit=deg` (richting, apart endpoint) voor vandaag/morgen/overmorgen, incl. eigen IJmond-sensor-actuals t/m nu. windwaarnemingen.nl via `database/vsp_vdg_wstats.php?st=IJmuiden1` (vandaag, incl. 10-min-actuals t/m 06:00) en `vsp_mrg_wstats.php?st=IJmuiden2` (morgen+overmorgen). Alle ruwe snelheden in m/s, hier omgerekend naar kts.

**Netto beeld:** **Zaterdag (vandaag)** is overtuigend **Slecht**: de wind loopt in de vroege ochtend wel duidelijk voor op alle drie modellen (+2 à +3kt), maar blijft ook dan nog ruim onder de 14kts-grens, en golf (0,1m) is en blijft de hele dag extreem plat. **Zondag** is een grensgeval tussen **Matig en Slecht** met een forse modelafwijking: GFS (Windfinder) blijft overtuigend onder de Slecht-drempel, maar Soarcast (Harmonie/IJmond) ziet een duidelijke ochtendpiek (±08:00-09:00, gust tot 20,4kts) die er net overheen gaat — netto-oordeel **Matig** omdat golf (0,23-0,38m) hoe dan ook ruim te klein blijft voor meer. **Maandag** is weer **Slecht**, ditmaal met slechts een kort en zwak afwijkend signaal van Soarcast rond 07:00-08:00. De outlook (dag 4-9) laat een duidelijke ommekeer zien t.o.v. eerdere runs: de wind trekt vanaf **donderdag 12 november** fors aan, met **vrijdag 13 november** als overtuigende uitschieter — licht aanlandige wind van 14,6-17,8kts gecombineerd met de hoogste golf van de hele periode (0,75-0,93m, periode 6,5-7,7s) levert bijna de hele dag een **Goed(a)**-klassering op, de beste papieren sinds lange tijd.

---

## ⚡ Snel overzicht
- **Zaterdag:** **Slecht** (windstil-achtig, golf 0,1m; wind loopt 's ochtends wel voor op de modellen — zie realitycheck, maar blijft te zwak).
- **Zondag:** **Matig** (grensgeval met Slecht — forse afwijking GFS vs. Soarcast/Harmonie op wind; golf hoe dan ook te klein). Beste venster: **08:00-09:00**.
- **Maandag:** **Slecht** (wind te zwak bij GFS en windwaarnemingen; Soarcast ziet een korte, zwakke piek rond 07:00-08:00).
- **Beste dag in de 7 dagen erna:** vrijdag 13 november (licht aanlandige wind 14,6-17,8kts + hoogste golf van de hele periode, 0,75-0,93m/~7s — Goed(a))

---

## ⏰ Realitycheck vandaag
- Laatste actuele uren (04:00-06:00, windwaarnemingen.nl/IJmuiden): **gem. 8,1-9,4 kts**, gust **10,6-11,2 kts**, richting **94,5-95,4°** (OOST). Soarcast's eigen IJmond-sensor zag over dezelfde late uren (05:40-06:00) vergelijkbaar: **gem. 7,8-8,4 kts**, gust **9,5-10,3 kts**, richting **108-120°**.
- Was voorspeld: windwaarnemingen's eigen Harmonie-vsp zag voor 04:00-06:00 slechts **5,4-7,0 kts / gust 9,3-10,7 kts, 93-105°**; Soarcast's eigen Harmonie-forecast zag voor dezelfde uren **7,0-8,7 kts / gust 11,1-12,1 kts, 98-113°**; Windfinder/GFS zag voor 01:00-07:00 **5,2-5,8 kts / gust 6,0-7,0 kts, 109-114°**.
- Conclusie: de wind loopt **licht tot duidelijk VOOR** op alle drie modellen (ongeveer **+2 à +3 kt** op het gemiddelde, **+1 à +2 kt** op de gust), richting vergelijkbaar en veilig (OOST, pal aflandig). Rest-van-de-dag inschatting: **classificatie Slecht blijft staan** — golf (0,1m) is sowieso de harde beperking, en alle modellen voorspellen voor de rest van de dag een verdere terugval naar 2-8 kts — maar met iets meer vertrouwen in de hogere kant van de bandbreedte voor het vroege ochtendvenster (07:00-09:00) dan de kale modellen suggereren.

---

## 📅 Komende 72 uur

### Zaterdag — Slecht
- Windfinder (GFS): 2,2-5,8 kts gem. tijdens daglicht, gust 2,7-7,0 kts, richting ONO/OZO (109-123°, **pal aflandig**). Golf vlak 0,1m, periode 6-7s.
- windwaarnemingen.nl (KNMI-Harmonie, vsp): 2,9-6,0 kts gem. tijdens daglicht, gust 6,8-11,3 kts, richting 75-155° (draait van OOST 's ochtends naar ZZO in de namiddag) — vergelijkbaar met GFS, allebei duidelijk lager dan wat vanochtend vroeg al gemeten wordt (zie realitycheck).
- Soarcast (KNMI-Harmonie, IJmond): 3,5-7,8 kts gem. tijdens daglicht, gust 8,7-13,0 kts, richting 75-148° — iets hoger dan windwaarnemingen, maar ook deze raming ligt ruim onder de actuele waarnemingen van vanochtend vroeg.
- Netto: alle drie de kale modellen zien zwakke wind (2,2-7,8 kts gem.) tijdens daglicht, ruim onder de 14kts-grens → **Slecht**, ondanks dat de vroege ochtend (zie realitycheck) iets harder waait dan voorspeld. Golf blijft het hele etmaal op 0,1m steken, ver onder de 1,1m-drempel → **Slecht** staat ook zonder twijfel vast op golf alleen.
- Pier-logica: niet van toepassing — richting is aflandig/side-shore, golf (0,1m) ruim onder de 0,8m-drempel.
- Getij: hoogwater 02:03 (2,1m), laagwater 10:25 (0,4m), hoogwater 14:20 (1,9m), laagwater 22:18 (0,3m).

### Zondag — Matig (grensgeval met Slecht — forse modelafwijking op wind)
- Windfinder (GFS, hourly): 8,4-10,8 kts gem. tijdens daglicht, gust 10,1-14,7 kts, richting 173-195° (**side-shore**, ZZW/ZUID). Golf groeit licht naar 0,23-0,38m, periode zakt van 6,2s naar 4,0s (onder de 5s-drempel vanaf ±09:00).
- windwaarnemingen.nl (KNMI-Harmonie, vsp): 7,8-10,1 kts gem. tijdens daglicht, gust 12,2-17,5 kts, richting 173-195° — tussen GFS en Soarcast in.
- Soarcast (KNMI-Harmonie, IJmond): 9,1-15,6 kts gem. tijdens daglicht, gust 15,4-20,4 kts, richting 181-194° — duidelijk hoger dan GFS, met een piek rond 06:00-09:00 (14,0-15,6 kts / 18,1-20,4 kts gust) die de Slecht-drempel (gust≥16 of gem≥14) doorbreekt. **Dit is een forse afwijking t.o.v. Windfinder/GFS en wordt expliciet vermeld i.p.v. gemiddeld.**
- Netto: richting is bij alle drie bronnen consistent side-shore (veilig, fijn om op te varen). GFS blijft overtuigend onder de Slecht-drempel; Soarcast ziet een duidelijke ochtendpiek erboven; windwaarnemingen zit ertussenin. Golf (0,23-0,38m) blijft in alle scenario's ruim te klein voor Goed(b)/Optimaal (drempel 1,1m), en de periode zakt al in de ochtend onder de 5s-drempel → zelfs in het beste scenario blijft het plafond **Matig**.
- Pier-logica: niet van toepassing — golf (0,23-0,38m) onder de 0,8m-drempel.
- Getij: hoogwater 02:44 (2,1m), laagwater 10:44 (0,5m), hoogwater 15:01 (2,0m), laagwater 18:59 (1,0m).
- Beste venster (daglicht): **08:00-09:00** — Soarcast ziet hier 14,0-15,6 kts / gust 18,1-20,4 kts (boven de Slecht-drempel), windwaarnemingen 8,2-9,7 kts / gust 14,2 kts, GFS lager (10,0-10,6 kts / gust 12,6-13,1 kts); richting 183-186° (ZUID, side-shore, veilig), golf 0,25-0,27m / 5,4-5,8s (beste periode van de ochtend, net boven de 5s-drempel).

### Maandag — Slecht (grensgeval — enkel Soarcast ziet een korte, zwakke escape)
- Windfinder (GFS, hourly): 6,1-10,3 kts gem. tijdens daglicht, gust 6,1-13,9 kts, richting 146-186° (**side-shore**/licht aflandig). Golf blijft klein (0,29-0,34m), periode daalt van 3,96s naar 3,46s (de hele dag onder de 5s-drempel).
- windwaarnemingen.nl (KNMI-Harmonie, vsp): 3,9-7,8 kts gem. tijdens daglicht, gust 9,7-14,4 kts, richting 166-205° — vergelijkbaar met GFS, blijft overal ruim onder de Slecht-drempel.
- Soarcast (KNMI-Harmonie, IJmond): 5,2-13,4 kts gem. tijdens daglicht, gust 9,7-20,2 kts, richting 170-200° — ziet net na zonsopkomst (±07:00-08:00) een korte piek die er net overheen gaat (gust 17,5-20,2 kts), maar zakt daarna snel terug naar hetzelfde zwakke niveau als de andere twee bronnen.
- Netto: GFS en windwaarnemingen zijn het eens — wind blijft de hele dag onder de Slecht-drempel (gust<16 én gem<14). Alleen Soarcast ziet een kort venster net na zonsopkomst dat erboven uitkomt — deze afwijking wordt hier expliciet vermeld. Golf (0,18-0,34m) en periode (<4s) blijven sowieso ruim onder de drempels, dus zelfs bij de Soarcast-piek is het plafond hooguit Matig voor dat ene korte venster → netto-oordeel voor de dag als geheel blijft **Slecht**.
- Pier-logica: niet van toepassing — side-shore/licht aflandig, golf (0,18-0,34m) onder de 0,8m-drempel.
- Getij: hoogwater 03:24 (2,1m), laagwater 11:17 (0,5m), hoogwater 15:38 (2,1m), laagwater 19:47 (1,0m).

---

## 🔭 Kans op mooie sessies daarna (dag 4-9)
Windfinder (GFS, enige bron zo ver vooruit) voor **dinsdag 10 november t/m maandag 16 november**:

- **Dinsdag 10 november**: wind zwak (2,9-8,5 kts, gust 2,9-13,5 kts), richting OOST/OZO (90-108°, pal aflandig). Golf blijft klein (0,15-0,17m), periode 3,9-6,0s → **Slecht**.
- **Woensdag 11 november**: wind bescheiden oplopend (6,4-10,2 kts, gust 8,7-14,2 kts), richting ONO/OOST (76-107°, licht/pal aflandig, veilig). Golf groeit licht naar 0,16-0,32m, met een sterk oplopende periode richting het einde van de dag (6,1-10,3s) → **Slecht/Matig-grens** (golf nog ruim te klein voor meer).
- **Donderdag 12 november**: wind trekt fors aan richting de avond — **11,2-19,2 kts gem., gust tot 22,0 kts**, richting draait van side-shore (OOST/NO) 's ochtends naar NNW (344-357°) in de middag/avond. Golf groeit naar 0,44-0,60m met een prima periode (6,3-7,7s) → **grensgeval**: sterke, bruikbare wind, maar golf nog niet bij de 1,1m-drempel en richting is side-shore i.p.v. aanlandig — valt buiten alle rijen van de tabel, het dichtst bij de Matig/Optimaal-grens.
- **Vrijdag 13 november — beste papieren van de hele periode**: wind blijft stevig, **14,6-17,8 kts gem., gust 17,7-21,1 kts**, richting draait naar NNW/NW (325-340°, **licht aanlandig** t.o.v. Zandvoort). Golf is hier het hoogst van de hele 9-daagse outlook: **0,75-0,93m met een uitstekende periode (6,5-7,7s)** — net onder de 1,1m-Optimaal-drempel, maar de combinatie van bruikbare wind + licht aanlandige richting + golf<1,1m levert vrijwel de hele dag (10:00-19:00) een **Goed(a)**-klassering op.
  - 🌊 Piervoorkeur: golf ≥0,8m én aanlandig bij Wijk aan Zee (eigen hoek 283,8° classificeert 325-340° als licht aanlandig; IJmuiden's pierzone-hoek 240° classificeert dezelfde richting als side-shore). Wind uit het NNW/NW valt in de 280°-360°-range van de pier-tabel → **IJmuiden (Zuidpier)** is hier de rustiger kant.
- **Zaterdag 14 november**: wind blijft hoog (8,4-15,9 kts), maar richting draait verder door naar WNW/W (292-332°, **pal aanlandig** vanaf de ochtend). Golf blijft net onder de drempel (0,81-0,92m), maar de combinatie van (net) te zwakke wind + pal aanlandige richting geeft tijdens het grootste deel van de daglichtperiode **Slecht** — alleen de vroege nacht haalt nog Goed(a).
- **Zondag 15 november**: wind neemt sterk af (1,4-8,1 kts), richting blijft (licht) aanlandig (274-330°). Golf daalt langzaam (0,73-0,79m) maar wind is te zwak → **Slecht**.
- **Maandag 16 november**: wind trekt weer aan richting de avond (9,2-16,3 kts gem., gust tot 26,5 kts!), richting pal aflandig (103-120°, veilig). Golf blijft rond 0,67-0,77m, nog net onder de drempel → grensgeval/Matig in de ochtend, met in de namiddag/avond een oplopende trend die wijst op mogelijk sterke papieren voor de week erná (buiten deze 9-daagse horizon).

**Beste dag: vrijdag 13 november** — de wind is hier voor het eerst in lange tijd echt bruikbaar (14,6-17,8 kts), de richting is licht aanlandig en veilig (met IJmuiden als beschutte kant achter de Zuidpier), en de golf is met 0,75-0,93m en een uitstekende periode (~7s) het hoogst van de hele outlook-periode — net niet genoeg voor Optimaal, maar ruimschoots voldoende voor **Goed(a)** gedurende vrijwel de hele dag. Kans: **gemiddeld**, met donderdag 12 en zaterdag 14 november als dichtstbijzijnde alternatieven als de golf iets anders uitpakt. ⚠️ Onzeker op 4+ dagen — check dichter bij de tijd opnieuw. Let vooral op of de golfhoogte op donderdag/vrijdag de 1,1m-drempel alsnog nadert, en of de wind-richting op vrijdag niet verder doordraait richting pal aanlandig (zoals op zaterdag 14 wel gebeurt).

---
_Bronnen: Windfinder (GFS) · Soarcast (KNMI Harmonie, IJmond) · windwaarnemingen.nl (KNMI, IJmuiden)_
