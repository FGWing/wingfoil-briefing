# 🌊 Wingfoil-briefing Zandvoort–Wijk aan Zee
_27-11-2026 · Ochtendbriefing_

⚠️ **Technische kanttekening:** alle drie bronnen rechtstreeks via curl/API opgehaald (geen interactieve browser nodig). Windfinder: zowel de reguliere forecast- als de Superforecast-pagina zijn Astro-sites die de volledige uurlijkse data (incl. golf/getij) server-side meesturen in een verborgen `astro-island`-attribuut; rechtstreeks gedecodeerd. Gebleken: de Superforecast-pagina levert zelf maar ±3 dagen (vandaag t/m zondag), ondanks de eigen paginatekst die anders suggereert — voor de dag 4-9 outlook is daarom teruggevallen op de reguliere forecast-pagina (GFS), die tot en met 6 december volledige uurlijkse data (incl. golf) meestuurt. Soarcast: endpoint `sc/plotPerLocAndUnitReact.php?json&jsonOnly&unit=...&location=133&day=0/1/2&forecastToShow=harm` (wind/gust in m/s, richting in graden). windwaarnemingen.nl: `database/vsp_vdg_wstats.php?st=IJmuiden1` (vandaag, actuals+vsp) en `vsp_mrg_wstats.php?st=IJmuiden2` (morgen+overmorgen vsp) — windsnelheid/gust in m/s, omgerekend naar knopen.

**Netto beeld — een zwakke maar opvallend vlagerige vrijdag (vandaag), een zaterdag die gedurende de dag flink opbouwt naar een sterke avond, en een zondag die sterkst is in de vroege uren en daarna afzwakt (met een duidelijke Soarcast-afwijking in de middag). In de outlook springt woensdag 2 december eruit als de sterkste dag van het hele dag 4-9-blok, met een aanlandige zwenking 's avonds die de IJmuiden-pier in beeld brengt.** De Realitycheck van vanochtend laat zien dat de wind iets achterblijft bij de voorspelling, vooral in de gust, maar rond 06:00 weer aansluit.

---

## ⚡ Snel overzicht
- **Vrijdag:** **Matig** (grensgeval, vlagerig) (21:00-23:00)
- **Zaterdag:** **Goed** (grensgeval) (17:00-23:00)
- **Zondag:** **Matig-tot-Goed** (grensgeval) (00:00-07:00)
- **Beste dag in de 7 dagen erna:** woensdag 2 december — duidelijk de sterkste en meest kansrijke dag van het hele dag 4-9-blok.

---

## ⏰ Realitycheck vandaag
- Laatste actuele uren (04:00-06:10, windwaarnemingen.nl/IJmuiden, omgerekend m/s→kts): **gem. 7,0-8,8 kts**, gust **8,4-13,5 kts**, richting **92-97° (OOST)**.
- Was voorspeld: windwaarnemingen's eigen uurlijkse vsp voor 04:00/05:00/06:00 zag **7,4 / 8,6 / 8,6 kts gem.** (gust 12,2 / 13,8 / 13,2 kts), richting **113 / 104 / 97° (OZO/OOST)**.
- Conclusie: de wind loopt licht **ACHTER** — het gemeten gemiddelde lag om 04:00-05:00 0,2-1,6kts onder de eigen vsp-voorspelling, en de gust bleef duidelijk achter (actueel 9-9,4kts tegen voorspeld 12-14kts). Tegen 06:00 trekt het gemeten beeld (8,8/13,5kts) weer vrijwel gelijk met de voorspelling (8,6/13,2kts). Richting klopt goed (OOST, pal aflandig). Rest-van-de-dag inschatting: **licht naar onder bijgesteld** — de classificatie (Matig, grensgeval) blijft staan, maar houd rekening met gust aan de onderkant van de voorspelde bandbreedte in plaats van bij Soarcast's hogere cijfers.

---

## 📅 Komende 72 uur

### Vrijdag — Matig (grensgeval, vlagerig)
- Windfinder (Superforecast, hourly ICON-EU): wind **7,6-11,3 kts gem.**, gust **14,5-21,3 kts**, richting **105-126° (OOST, pal aflandig)**. Golf laag en kort: **0,11-0,16m**, periode **1,89-4,57s**.
- Soarcast (Harmonie, IJmond): hoger — **10,7-14,4 kts gem., gust 15,7-19,8 kts**, richting 101-136° (vergelijkbaar).
- windwaarnemingen.nl (eigen Harmonie-vsp, IJmuiden): laagste van de drie — **7,4-10,9 kts gem., gust 12,2-16,7 kts**, richting 97-136°.
- Netto — alle drie bronnen zijn het eens over de pal aflandige richting (binnen ~20° van Zandvoort's 107,5°) en de lage/korte golf, maar het gemiddelde loopt uiteen van zwak (Windfinder/windwaarnemingen, 7-11kts) tot gematigd (Soarcast tot 14,4kts). Opvallend: de gust loopt op tot 19-21kts terwijl het gemiddelde nooit boven de 14-15kts-grens komt — een duidelijk vlagerige dag die niet netjes in de "Matig"-voorwaarde (gust<19) past. Golf sluit Optimaal/Goed(b) hoe dan ook uit. Netto **Matig, grensgeval (vlagerig)**.
- Pier-logica: niet van toepassing (golf blijft onder 0,8m, max 0,16m).
- Getij: laagwater ±01:11 (0,36m), hoogwater ±05:07 (2,1m), laagwater ±13:06 (0,32m), hoogwater ±17:22 (2,3m).
- Beste venster: **±21:00-23:00** — wind 10,5-10,8 kts (Soarcast 14,2-14,4 kts), gust 19,3-19,8 kts, richting 120-130° (pal aflandig). Bovenkant van de dag; de Realitycheck wijst op mogelijk iets minder dan de hogere Soarcast-cijfers.

### Zaterdag — Goed (grensgeval)
- Windfinder (Superforecast, hourly ICON-EU): wind **9,3-15,3 kts gem.** (stijgend gedurende de dag), gust **18,2-28,0 kts**, richting draait van **128° (pal aflandig)** 's nachts naar **163° (side-shore, richting zuid)** in de avond. Golf bouwt op van **0,14m/2,79s** 's nachts naar **0,63m/5,4s** aan het eind van de avond.
- Soarcast (Harmonie, IJmond): hoger, vooral in de avond — **14,0-20,8 kts gem., gust 19,2-28,8 kts**, richting 121-163° (vergelijkbaar patroon).
- windwaarnemingen.nl (eigen Harmonie-vsp, IJmuiden): tussen de twee andere bronnen in — **9,3-16,5 kts gem., gust 15,2-26,0 kts**, richting 117-160°.
- Netto — alle drie bronnen bevestigen de opbouw door de dag en de draai van aflandig naar side-shore. De avond (17:00-23:00) komt bij alle bronnen ruim in de 14-25kts-band (Soarcast tot 20,8kts) met een gunstige side-shore richting, maar de golfhoogte blijft net onder de 1,1m-Optimaal-grens (max 0,63m) ondanks een oplopende periode (tot 5,4s). Netto **Goed, grensgeval** — had Optimaal kunnen zijn met iets meer golfhoogte.
- Pier-logica: niet van toepassing (golf blijft onder 0,8m, max 0,63m).
- Getij: laagwater ±01:46 (0,38m), hoogwater ±05:57 (2,0m), laagwater ±13:51 (0,26m), hoogwater ±18:11 (2,26m).
- Beste venster: **±17:00-23:00** — wind 14,1-15,3 kts (Soarcast tot 18,9-20,8 kts), gust 24,9-28,0 kts, richting 139-163° (licht aflandig tot side-shore). Stevige gusts; check de avond voor de sterkste combinatie.

### Zondag — Matig-tot-Goed (grensgeval)
- Windfinder (Superforecast, hourly ICON-EU): wind **5,8-14,8 kts gem.** (sterkst 's nachts/vroege ochtend, neemt daarna geleidelijk af), gust **10,3-27,8 kts**, richting **165-195° (side-shore, draaiend richting zuid/ZZW)**. Golf **0,59-0,75m**, periode **4,88-6,29s** (ruim boven 5s de hele dag, hoogte blijft onder 1,1m).
- Soarcast (Harmonie, IJmond, tot 15:00): **11,5-20,0 kts gem., gust 16,1-27,8 kts**, richting 163-204° — ander patroon: daalt eerst net als Windfinder, maar stijgt na 10:00 weer naar 15,9kts om 15:00 — duidelijke modeldivergentie in de middag.
- windwaarnemingen.nl (eigen Harmonie-vsp, IJmuiden, tot 15:00): **8,5-15,9 kts gem., gust 13,4-24,9 kts**, richting 161-194° — ligt dicht bij Windfinder en bevestigt de dalende lijn.
- Netto — 2 van de 3 bronnen (Windfinder, windwaarnemingen) zijn het eens over een dalende lijn gedurende de dag, met het sterkste venster 's nachts/vroege ochtend (14-15kts, side-shore, periode>5s maar hoogte nog net onder 1,1m — Goed(b) qua wind/richting maar net niet qua golf). Soarcast wijkt in de middag af met een hernieuwde stijging — expliciet vermeld i.p.v. gemiddeld. Netto **Matig-tot-Goed, grensgeval**, sterkst in de nacht/vroege ochtend.
- Pier-logica: niet van toepassing (golf blijft onder 0,8m, max 0,75m).
- Getij: laagwater ±02:27 (0,39m), hoogwater ±06:50 (1,89m), laagwater ±14:38 (0,21m), hoogwater ±19:05 (2,18m).
- Beste venster: **±00:00-07:00** — wind 12,2-14,8 kts (Soarcast 17,1-20,0 kts), gust 19,0-27,8 kts, richting 165-182° (side-shore). Check dichter bij de tijd of Soarcast's middagstijging bewaarheid wordt.

---

## 🔭 Kans op mooie sessies daarna (dag 4-9)
Windfinder (GFS, enige bron zo ver vooruit) voor **maandag 30 november t/m zaterdag 5 december**.

- **Maandag 30 november** (dag 4): **5,7-10,3 kts gem.**, gust **6,5-17,3 kts**, richting **side-shore tot licht aanlandig (178-209°)**. Golf **0,55-0,68m**, periode **4,43-5,16s**. **Matig**, zwak — sterkste moment 's avonds (19:00-22:00, 9,7-10,3kts).
- **Dinsdag 1 december** (dag 5): **10,6-15,6 kts gem.** (stijgend), gust **18,2-29,3 kts**, richting **side-shore (179-187°)**. Golf **0,69-0,79m**, periode consistent **≥5,2s**. 's Avonds (19:00-22:00) 15,4-15,6kts in de Optimaal-band met ideale side-shore richting, maar golfhoogte nog net onder 1,1m. **Goed, grensgeval** — dicht bij Optimaal.
- **Woensdag 2 december** (dag 6): **11,6-18,9 kts gem.** (piek 13:00, 18,9kts) — hoogste van de hele outlook, gust **16,6-33,7 kts**, richting overdag side-shore (180-203°), zwenkt 's avonds naar **313-324° (NW, licht aanlandig)**. Golf **0,82-0,87m** — hoogste golf van de week, periode **5,7-6,0s**. Overdag **Goed, grensgeval** (golf nog net <1,1m); 's avonds (19:00: 18,6kts, gust 22,3kts, dir 324°, golf 0,84m) past de classificatie letterlijk op **Goed(a)**. Pier-logica van toepassing: richting NW + golf ≥0,8m → **IJmuiden (Zuidpier) rustiger**.
- **Donderdag 3 december** (dag 7): **6,5-13,2 kts gem.**, gust **8,6-18,2 kts**, richting **aanlandig, NW/N (287-331°)** — vervolg van de zwenking van dinsdagavond. Golf **0,80-0,96m**, periode **5,6-6,9s**. Wind te zwak voor Goed/Optimaal: **Matig**. Pier-logica van toepassing: pal aanlandig (dicht bij Zandvoort's 287,5°) + golf tot 0,96m → **IJmuiden (Zuidpier) rustiger**, Wijk aan Zee ligt hier juist bloot.
- **Vrijdag 4 december** (dag 8): **2,4-5,3 kts gem.**, gust **3,1-5,6 kts** — duidelijke windstille lul-dag. **Slecht**.
- **Zaterdag 5 december** (dag 9): **6,6-9,1 kts gem.**, gust **7,2-12,7 kts** — nog te zwak, ondanks een opvallend lange golfperiode (6,3-7,1s) blijft de golfhoogte te laag (0,47-0,52m) om iets te betekenen. **Slecht**.

**Beste dag: woensdag 2 december** — duidelijk de sterkste wind van de hele dag 4-9-periode (tot 18,9kts), de hoogste golf van de week (tot 0,87m) en een avondzwenking naar een aanlandige, pier-beschutte richting bij IJmuiden. Kans: **gemiddeld-tot-hoog**. Donderdag 3 december is een alternatief dankzij aanhoudende golf en pierbescherming, maar met zwakkere wind. ⚠️ Onzeker op 4+ dagen — check dichter bij de tijd opnieuw.

---
_Bronnen: Windfinder (GFS / Superforecast ICON-EU) · Soarcast (KNMI Harmonie, IJmond) · windwaarnemingen.nl (KNMI, IJmuiden)_
