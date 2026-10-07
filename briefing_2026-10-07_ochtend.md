# 🌊 Wingfoil-briefing Zandvoort–Wijk aan Zee
_07-10-2026 · Ochtendbriefing_

⚠️ **Technische kanttekening deze run:** Soarcast is (net als alle voorgaande runs) niet bereikbaar — pure JS-app (Vite-bundle), geen SSR-data en geen vindbaar API-pad in de gecompileerde bundle. Windfinder is via de onderliggende paginadata (astro-hydration props) opgehaald — één bezoek aan de reguliere forecast-pagina leverde zowel de korte termijn (3-uurs, vandaag+morgen, component `ForecastSection`) als de volledige 3-uurs data t/m 16 oktober (component `ForecastDataInit`) in dezelfde payload — geen apart bezoek aan de Superforecast-pagina nodig. windwaarnemingen.nl (IJmuiden) is via de onderliggende `vsp_vdg_wstats.php`/`vsp_mrg_wstats.php`-endpoints opgehaald: 10-minuten-actuals + ingebed KNMI-uurmodel voor vandaag, en het KNMI-uurmodel t/m morgenmiddag 16:00.

---

## ⚡ Snel overzicht
- **Woensdag:** Slecht (late avond al eerste opbouw richting donderdag)
- **Donderdag:** Optimaal bij IJmuiden (02:00-20:00) — Zandvoort/Wijk aan Zee draaien vanaf de avond pal aanlandig
- **Vrijdag:** Grensgeval/Slecht — kort Optimaal-venster 05:00-08:00, daarna overwegend Slecht met extreme gust
- **Beste dag in de 7 dagen erna:** zondag 11 oktober

---

## ⏰ Realitycheck vandaag

- Laatste actuele uren (windwaarnemingen.nl, IJmuiden, 05:40-07:10): **wind 1,8-2,8 kts gem, gust 2,5-3,8 kts**, richting oost/oostzuidoost (95-109°).
- Was voorspeld voor dezelfde uren: Windfinder (GFS, 3-uurs) 05h **105° 5,5/7,6 kts**, 08h **101° 5,4/7,2 kts**; KNMI-vsp (windwaarnemingen.nl, huidige modelrun) 05:00 **124° ZO 3,4/5,1 kts**, 06:00 **116° OZO 3,4/5,1 kts**, 07:00 **122° OZO 2,8/4,9 kts**.
- Conclusie: wind loopt **ACHTER** op de verwachting — de actuele 1,8-2,8 kts ligt duidelijk onder zowel Windfinder (5,4-5,5 kts) als KNMI-vsp (2,8-3,4 kts) voor dezelfde uren. Richting klopt wel goed (oost/oostzuidoost, 95-109° vs voorspelde 101-124°). Rest-van-de-dag inschatting: **ongewijzigd** — dit blijft hoe dan ook een zwakke dag tot de avond; de verwachte windopbouw rond 23:00 (richting donderdag) is een apart synoptisch signaal dat niet wordt beïnvloed door deze lichte ochtend-onderschatting.

---

## 📅 Komende 72 uur

### Woensdag — Slecht
- Windfinder (GFS, 3-uurs): hele dag zwak en overwegend aflandig/side-shore bij Zandvoort, 0,5-9,6 kts gem / 1,8-11,3 kts gust, richting draait van oost (101-116°) via noord (12-333°) in de loop van de middag/avond. Pas om **23:00** trekt het aan: **19,2 kts gem / 21,6 kts gust, richting 347° (NNW, side-shore)** — golf dan ook net over de drempel (1,11m/5,12s) → **Optimaal**, maar dit is de allereerste aanzet van de stormfase die donderdag domineert, geen volwaardig middag/avondvenster.
- windwaarnemingen.nl (KNMI-vsp + actuals, IJmuiden): bevestigt het zwakke beeld — zie Realitycheck hierboven.
- Golven (Windfinder, enige golfbron): 0,36-1,11m / 5,1-7,4s — pas om 23:00 over de 1,1m-drempel.
- 🌊 Piervoorkeur: niet van toepassing (geen enkel moment vandaag tegelijk aanlandig én golf ≥0,8m bij IJmuiden/Wijk aan Zee).
- Getij: hoogwater ~01:46 (2,0m), laagwater ~10:15 (0,4m), hoogwater ~14:12 (1,65m), laagwater ~21:55 (0,3m).
- Bronnen: Windfinder en KNMI-vsp **eens** dat het overdag zwak blijft. Soarcast niet bereikbaar (zie technische kanttekening).

### Donderdag — Optimaal bij IJmuiden
- Bij **IJmuiden** (pierzone-hoek 150°/330°): wind blijft de **hele dag side-shore** (richting 314-351°, NW/NNW) → vrijwel continu **Optimaal**: wind 17,0-21,7 kts gem, gust 20,0-26,0 kts, golf 1,55-2,01m / 6,4-7,8s. Beste venster: **02:00-20:00**.
- Bij **Zandvoort/Wijk aan Zee**: zelfde richting leest hier grensgeval-tot-pal-aanlandig. Overdag (02:00-17:00) nog grensgeval (licht aanlandig, golf ruim over de drempel), maar vanaf **20:00-23:00** draait het bij Zandvoort naar **pal aanlandig** (314° en 280°) met golf 1,57-1,68m en geen pierbescherming → **Slecht** vanaf de avond. Wijk aan Zee volgt dezelfde verslechtering iets vertraagd (grensgeval → pal aanlandig om 23:00).
- 🌊 Piervoorkeur: **IJmuiden** (Zuidpier breekt de noordwest-golfslag/-wind, 280-360° range) de hele dag — Wijk aan Zee ligt bij deze NW-richting juist onbeschut, net als Zandvoort.
- Getij: hoogwater ~02:44 (2,1m), laagwater ~11:41 (0,3m), hoogwater ~15:03 (1,8m), laagwater ~22:51 (0,2m).
- Bronnen: Windfinder enige bron met golfdata; richting/kracht intern consistent over de dag. Soarcast niet bereikbaar.

### Vrijdag — Grensgeval/Slecht ⚠️ zeer grillig
- Vroeg op de dag (**05:00-08:00**) nog een kort goed venster: wind 20,4-21,7 kts gem, **gust pieken tot 32,3 kts** (!), richting 197-239° (zuid/zuidwest, side-shore bij Zandvoort en Wijk aan Zee) → **Optimaal**, golf 1,36-1,54m/5,7-6,6s. Dit is stormachtig en met die gustpieken niet voor iedereen comfortabel.
- Vanaf **11:00** draait de wind verder door naar west/zuidwest (252-285°) en leest bij Zandvoort en Wijk aan Zee vrijwel de hele rest van de dag **pal aanlandig**, met golf blijvend groot (1,76-2,02m) → **Slecht** (grote onbeschutte branding) van 11:00 tot in de avond.
- 🌊 Piervoorkeur: vroeg op de dag (02:00-08:00, richting 197-251° = zuid/zuidwest) is **Wijk aan Zee** beschut (Noordpier breekt de zuid(west)-golfslag). Vanaf 11:00 valt de richting (252-285°) echter grotendeels in de **neutrale zone tussen de twee pierassen (250-280°)** — geen van beide pieren biedt dan nog duidelijk voordeel, wat samenvalt met het grote onbeschutte deel van de dag.
- Getij: hoogwater ~03:27 (2,1m), laagwater ~12:58 (0,3m), hoogwater ~15:46 (1,9m), laagwater ~23:34 (0,2m).
- Bronnen: alleen Windfinder (golfdata); KNMI-vsp (windwaarnemingen.nl) loopt voor deze dag tot 16:00 door en bevestigt de forse wind qua orde van grootte voor de ochtend. Soarcast niet bereikbaar. **Check dicht bij de tijd opnieuw** — de combinatie van extreme gust en een grillige richtingsdraai maakt dit een onzekere dag.

---

## 🔭 Kans op mooie sessies daarna (dag 4-9)
Windfinder (GFS, enige bron zo ver vooruit — in dezelfde payload als de korte termijn opgehaald, t/m 16 oktober) voor **zaterdag 10 t/m donderdag 15 oktober**:

- **Zaterdag 10 oktober**: stevige wind (19,2-24,2 kts gem, gust 22,5-30,0 kts) maar richting (266-281°, west/WNW) valt bij zowel Zandvoort/Wijk aan Zee (pal aanlandig) als IJmuiden grotendeels in de **neutrale pierzone (250-280°)** → vrijwel de hele dag **Slecht**, groot onbeschut zwell (1,78-2,17m). Alleen de late uren (281° om 23:00) kantelen net richting IJmuiden-voordeel.
- **Zondag 11 oktober — beste dag**: bij **IJmuiden** van **02:00 tot 14:00** vrijwel ononderbroken **Optimaal** — wind 16,5-22,0 kts gem (geleidelijk afbouwend), gust 19,4-26,0 kts, golf 1,78-2,14m met lange periode (7,3-7,6s), richting 280-349° (WNW/NW, side-shore bij IJmuiden → Zuidpier beschermt). Na 14:00 valt de wind snel terug (<14 kts) en wordt de rest van de dag **Slecht** (te zwak).
- **Maandag 12 oktober**: wind valt grotendeels weg (1,0-9,3 kts, wisselvallige richting) → **Slecht**.
- **Dinsdag 13 oktober**: zwakke zuid/zuidzuidoostelijke wind (7,5-9,9 kts gem, gust 9,7-13,2 kts) → **Slecht**, simpelweg te weinig kracht.
- **Woensdag 14 oktober**: nog zwakker en wisselvallig van richting (3,5-8,8 kts gem) → **Slecht**.
- **Donderdag 15 oktober**: overdag nog zwak (5,7-8,8 kts), maar 's avonds (20:00-23:00) een korte opleving naar **Matig** (9,2-9,8 kts gem, gust 16,5-18,7 kts) — golf net onder de 1,1m-drempel. Mogelijk voorbode van meer wind ná dag 9, buiten dit outlook-bereik.

**Beste dag: zondag 11 oktober**, met name **02:00-14:00 bij IJmuiden** — krachtige, langeperiode swell uit het noordwesten die geleidelijk afbouwt, met duidelijk pierbeschutting. Kans: **hoog** voor wind/richting in het ochtendvenster — het signaal is consistent over meerdere uren — al ligt de dag nog 4 dagen vooruit.
⚠️ Onzeker op 4+ dagen — check dichter bij de tijd opnieuw, met name of de krachtige/grillige wind van donderdag-vrijdag (zie boven) de golfopbouw voor zaterdag/zondag beïnvloedt.

---
_Bronnen: Windfinder (GFS) · windwaarnemingen.nl (KNMI, IJmuiden) · Soarcast — deze run niet bereikbaar (JS-app, geen vindbaar/bereikbaar API-adres)_
