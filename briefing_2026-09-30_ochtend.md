# 🌊 Wingfoil-briefing Zandvoort–Wijk aan Zee
_30-09-2026 · Ochtendbriefing_

⚠️ **Technische kanttekening deze run:** Soarcast is (net als de vorige runs) niet bereikbaar — nog altijd een volledige JS-app (React/Vite) zonder vindbaar/bereikbaar API-adres in de uitgeleverde bundle. Windfinder is deze keer volledig via de onderliggende paginadata opgehaald (astro-hydration props, geen screenshots nodig), inclusief wind + golven + getij per 3 uur t/m 9 oktober in één keer. windwaarnemingen.nl (IJmuiden) is rechtstreeks via de KNMI-vsp/actuals-JSON-endpoints opgehaald (10-minutenwaarden voor vandaag inclusief lopende modelvoorspelling, plus het uurmodel voor morgen/overmorgen).

---

## ⚡ Snel overzicht
- **Woensdag:** Matig (grensgeval met Goed) — venster **05:00-11:00**
- **Donderdag:** Slecht (Windfinder) / mogelijk Matig **11:00-19:00** (KNMI-vsp) — modellen wijken sterk af, zie toelichting
- **Vrijdag:** Slecht
- **Beste dag in de 7 dagen erna:** donderdag 8 oktober (kort maar krachtig venster rond 08:00, vlak vóór een snel opbouwende storm — zie kanttekening in de outlook; woensdag 7 oktober is het veiligere alternatief)

---

## ⏰ Realitycheck vandaag

- Laatste actuele uren (windwaarnemingen.nl, IJmuiden, 05:00-07:10): **wind 9,4-11,2 kts, gust 13,0-16,6 kts, richting 129-135° (ZO)**
- Was voorspeld voor dezelfde uren: KNMI-vsp (windwaarnemingen.nl, huidige modelrun) gaf **9,5-10,3 kts gem / 14,8-15,6 kts gust, richting ZO (135-140°)**; Windfinder (GFS) gaf voor 05h **9,9/19,2 kts (151°)** en voor 08h **9,7/16,9 kts (140°)**.
- Conclusie: de wind **klopt vrijwel exact met KNMI-vsp** (verschil <1 kt in zowel gemiddelde als gust), maar **loopt iets ACHTER op Windfinders eigen gust-voorspelling** — die gaf 19,2 kts gust voor 05h, terwijl er nu 13-16,6 kts gemeten wordt. Richting komt in alle drie bronnen goed overeen (ZO, 129-151°). Voor de rest van de dag: classificatie **ongewijzigd Matig** (het onderliggende windbeeld/patroon klopt goed), maar het vertrouwen in Windfinders relatief hoge gust-cijfers voor de rest van de ochtend is **iets naar beneden bijgesteld** — reken op iets rustigere pieken dan de Windfinder-tabel hieronder suggereert.

---

## 📅 Komende 72 uur

### Woensdag — Matig (grensgeval met Goed)
- **Beste venster: 05:00-11:00** — Windfinder: 05h 9,9/19,2 kts (151°, licht aflandig), 08h 9,7/16,9 kts (140°), 11h 10,9/19,1 kts (165°, side-shore). Het gemiddelde (10-11 kts) blijft net onder de 14 kts-ondergrens voor Optimaal/Goed(a), en de hoge gust-cijfers (19,1-19,2) zetten dit net over de Matig-grens (die gust <19 vraagt) — vandaar grensgeval. **Zie Realitycheck**: de actuele metingen en KNMI-vsp liggen dichter bij een nette Matig-classificatie (gust ~15-17,7 kts), dus in de praktijk voelt dit venster waarschijnlijk als een rustige, prima-vlakke Matig-sessie i.p.v. net-Goed.
- Na 14:00 zakt het verder terug: 14h 9,6/16,6 kts (182°), **17h duikt naar Slecht** (6,1/10,3 kts, 198°), 20h en 23h herstellen licht naar Matig (7,4-8,4/16,2-17,5 kts, 172-192°, side-shore).
- Golven: 0,17-0,45 m / 3,0-5,2 s — de hele dag ruim onder de 1,1 m-drempel.
- 🌊 Piervoorkeur: niet van toepassing (golf blijft overal <0,8 m).
- Getij: laagwater ~02:08 (0,25 m), hoogwater ~06:37 (2,23 m), laagwater ~14:24 (0,46 m), hoogwater ~18:57 (2,2 m), laagwater ~23:24 (0,84 m).
- Bronnen: Windfinder en KNMI-vsp **eens** over het patroon (zwak-matig in de ochtend, wegvallend na 14:00). De **actuele meting bevestigt KNMI-vsp nauwkeurig**; Windfinders gust-voorspelling liep er dit keer merkbaar bovenuit — zie Realitycheck. Soarcast niet bereikbaar.

### Donderdag — Slecht (Windfinder) / Matig mogelijk 11:00-19:00 (KNMI-vsp) — grote modeldivergentie
- **Windfinder (GFS) ziet de hele dag Slecht**: 02h 7,8/14,4 kts (182°), 05h 8,2/13,2 kts (217°), 08h 5,6/7,6 kts (229°), 11h 5,9/8,7 kts (256°, licht aanlandig), 14h 6,4/10,0 kts (214°), 17h 9,2/13,5 kts (269°, pal aanlandig), 20h 7,2/10,5 kts (265°), 23h 6,1/8,3 kts (266°) — nergens boven de 9,2 kts gemiddeld of 16 kts gust.
- **KNMI-vsp (windwaarnemingen.nl) ziet juist een opbouwende West/WZW-bries rond het middaguur**: 12:00 12,2/17,3 kts (259°, WEST), 14:00 12,1/16,7 kts (252°, WZW), 17:00 12,2/16,7 kts (247°, WZW) — dit haalt net de Matig-drempel (gem <15, gust <19) i.p.v. Windfinders Slecht.
- **Dit is een aanzienlijke afwijking** — niet middelen. Vanochtend verifieerde KNMI-vsp bij IJmuiden zeer nauwkeurig tegen de actuals (zie Realitycheck), wat dit KNMI-scenario voor morgenmiddag iets meer vertrouwen geeft dan gebruikelijk, maar het blijft een divergentie van bijna een factor 2 in gemiddelde wind. Richting is in beide bronnen vergelijkbaar (West/WZW-achtig na het middaguur).
- Golven (Windfinder, enige golfbron): 0,39-0,50 m / 3,9-5,2 s — ruim onder de 1,1 m-drempel, ook in het KNMI-scenario geen probleem.
- 🌊 Piervoorkeur: niet van toepassing (golf blijft <0,8 m).
- Getij: laagwater ~02:42 (0,24 m), hoogwater ~07:19 (2,15 m), laagwater ~15:06 (0,42 m), hoogwater ~19:37 (2,2 m).
- Bronnen: Windfinder en KNMI-vsp **wijken sterk af** in kracht, komen overeen in richting. Soarcast niet bereikbaar.

### Vrijdag — Slecht
- **Windfinder ziet de hele dag zwak**: 02h 4,7/5,2 kts (217°), 05h 5,7/6,7 kts (190°), 08h 6,4/8,0 kts (187°), 11h 8,6/10,7 kts (200°), 14h 9,8/10,6 kts (225°), 17h 7,7/8,6 kts (233°), 20h 5,5/7,3 kts (235°), 23h 4,4/5,8 kts (177°) — nergens boven de 9,8 kts gemiddeld.
- KNMI-vsp bevestigt een zwakke dag, met een fractioneel sterkere middag (13:00-16:00: 8,4-10,7 kts gem / 14,2-15,4 kts gust, ZW/WZW) — blijft echter ruim binnen de Slecht-drempel, geen materiële divergentie.
- Golven: 0,26-0,43 m / 3,7-4,2 s — ruim onder de 1,1 m-drempel.
- 🌊 Piervoorkeur: niet van toepassing (golf blijft <0,8 m).
- Getij: laagwater ~03:20 (0,25 m), hoogwater ~08:03 (2,02 m), laagwater ~15:52 (0,39 m), hoogwater ~20:21 (2,14 m).
- Bronnen: Windfinder en KNMI-vsp **eens** — zwakke dag. Soarcast niet bereikbaar.

---

## 🔭 Kans op mooie sessies daarna (dag 4-9)
Windfinder (GFS, enige bron zo ver vooruit) laat voor **zaterdag 3 t/m donderdag 8 oktober** het volgende beeld zien:
- **Zaterdag 3 en zondag 4 oktober**: zeer zwak, nergens boven 6,2 kts gemiddeld / 9,1 kts gust — Slecht.
- **Maandag 5 oktober**: bouwt op in de middag/avond — 11h 11,3/17,2 kts (228°, side-shore), 14h 12,6/17,8 kts (244°, licht aanlandig), 17h 12,8/18,8 kts (234°) — Matig, met een gusty avond (20h 12,0/20,7 kts, 23h 13,2/22,6 kts) die net over de Matig-drempel piekt.
- **Dinsdag 6 oktober**: wisselvallig — 's nachts/vroege ochtend grensgeval Matig/Goed (12,7-13,0/20,0-21,2 kts, 236-253°), overdag terugval naar Matig/Slecht met een richtingsdraai naar pal aanlandig (267-313°), 's avonds weer Matig tot grensgeval Goed (20h 12,7/16,9 kts, 23h 15,2/19,3 kts, 301°). Golf loopt op naar 0,74 m — nog onder de 0,8 m pierdrempel.
- **Woensdag 7 oktober — sterkste kandidaat voor een volle dag**: de hele dag gestage 14-20 kts (gust tot 22,9 kts) uit WNW (287-303°). Bij **Zandvoort** is dit pal aanlandig (past niet in de Optimaal/Goed(a)-tabelrijen → overal "grensgeval Goed"), maar bij **IJmuiden valt exact dezelfde windrichting dankzij de eigen pierzone-kusthoek (150°/330°) als side-shore** — daar dus het hele etmaal "grensgeval Optimaal/Goed(a)". Golf loopt op van 0,80 m 's nachts naar 1,03 m 's avonds (periode steeds 5,8-6,5 s, ruim voldoende) — net onder de 1,1 m Optimaal-drempel. 🌊 **Piervoorkeur: IJmuiden rustiger** (wind uit 280-360° → Zuidpier breekt de golfslag) — vrijwel de hele dag van toepassing zodra de golf de 0,8 m passeert (rond het middaguur).
- **Donderdag 8 oktober**: kort maar krachtig venster — 05h Goed(a) (16,3/20,5 kts, 243°), **08h zelfs kortstondig Optimaal bij Zandvoort** (22,9/31,1 kts, 239°, side-shore, golf 1,15 m/6,7 s). Direct daarna schiet de wind door naar stormkracht: 11h 31,5/42,3 kts, 14h 32,4/43,6 kts — ruim boven de Optimaal-bovengrens (25 kts), golf tot 1,25 m. Bij >27 kts uit W/ZW/NW sluit de Reddingsbrigade IJmuiden normaliter de pieren — een onafhankelijk signaal dat dit na de ochtend een pittige/gevaarlijke dag wordt, alleen voor gevorderde riders met klein materiaal en uitsluitend in het korte venster vóór de piek.

**Beste dag: donderdag 8 oktober**, specifiek het venster rond **08:00** (hoogste score, Optimaal), maar dit is een smal venster vlak voor een snel opbouwende storm waarvan de exacte timing op 8 dagen vooruit nog goed kan verschuiven. Kans: **gemiddeld** (het signaal — een korte Optimaal-piek net voor stormopbouw — is fysisch plausibel en consistent tussen 3-uurs-stappen, maar timing en golfhoogte zijn nog onzeker). **Woensdag 7 oktober is het veiligere alternatief**: een volle dag gestage 14-20 kts, met name aantrekkelijk bij IJmuiden dankzij het piervoordeel.
⚠️ Onzeker op 4+ dagen — check dichter bij de tijd opnieuw, met name de exacte timing en intensiteit van de storm op donderdag 8 oktober.

---
_Bronnen: Windfinder (GFS) · windwaarnemingen.nl (KNMI, IJmuiden) · Soarcast — deze run niet bereikbaar (JS-app, geen vindbaar/bereikbaar API-adres)_
