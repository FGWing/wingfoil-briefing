# 🌊 Wingfoil-briefing Zandvoort–Wijk aan Zee
_06-11-2026 · Ochtendbriefing_

⚠️ **Technische kanttekening:** Windfinder opgehaald via de embedded Astro-JSON op de reguliere forecast-pagina: `FcTableWindpreviewContainer` (wind-only, 3-uurs stappen, dag 1-10 in één keer) gecombineerd met de `ForecastDataInit`-islands van zowel de forecast- als de weatherforecast-pagina voor golf+getij (hourly voor dag 2-3, 3-uurs voor dag 3-10 — ruwe data in m/s, hier omgerekend naar kts). Soarcast via `/sc/plotPerLocAndUnitReact.php?json&jsonOnly&unit=m/s...&location=133&day=...` (vandaag/morgen/overmorgen, incl. eigen IJmond-sensor-actuals t/m nu). windwaarnemingen.nl via `database/vsp_vdg_wstats.php?st=IJmuiden1` (vandaag, incl. 10-min-actuals t/m 06:10, ruwe data in m/s) en `vsp_mrg_wstats.php?st=IJmuiden2` (morgen+overmorgen t/m 8 nov 15:00, model-horizon bereikt).

**Netto beeld:** **Vrijdag (vandaag)** is een grensgeval: de kale modellen (GFS én Harmonie) voorspelden voor de vroege ochtend maar 7,5-9 kts, maar de realitycheck laat zien dat het al 13-17 kts waait — een forse positieve afwijking die de inschatting voor het ochtendvenster flink optrekt, al blijft golf (0,1m) hard de beperkende factor → **Matig**. **Zaterdag** is overtuigend **Slecht**: alle drie bronnen zijn het eens dat het nagenoeg windstil blijft. **Zondag** is opnieuw **Matig**, met een duidelijke GFS-vs-Harmonie-kloof (6-9 kts vs. 8-15 kts) die expliciet vermeld wordt. De outlook (dag 4-9) blijft grotendeels zwak — maandag en dinsdag vrijwel windstil — met een geleidelijk opbouwende golf (periode tot ~8s) richting het eind van de week; **vrijdag 13 november** springt eruit als beste dag (golf en periode het dichtst bij de 1,1m/5s-drempel van de hele periode), met zaterdag 14 november als sterke opvolger door de verder oplopende wind.

---

## ⚡ Snel overzicht
- **Vrijdag:** **Matig** (golf ruim te klein; wind loopt 's ochtends fors voor op alle modellen — zie realitycheck). Beste venster: **07:00-10:00**.
- **Zaterdag:** **Slecht** (vrijwel windstil, golf te klein — alle drie bronnen eens).
- **Zondag:** **Matig** (golf nog klein; forse modelafwijking GFS vs. Harmonie op wind). Beste venster: **07:00-10:00**.
- **Beste dag in de 7 dagen erna:** vrijdag 13 november (golf 0,6-0,7m met de beste periode van de hele outlook-periode, ~8s, bij een veilige aflandige richting)

---

## ⏰ Realitycheck vandaag
- Laatste actuele uren (04:00-06:10, windwaarnemingen.nl/IJmuiden): **gem. 13,4-14,9 kts**, gust **16,2-17,8 kts**, richting **87-93°** (OOST). Soarcast's eigen IJmond-sensor zag over dezelfde periode vergelijkbaar: **gem. 13,7-16,7 kts**, gust **16,4-19,2 kts**, richting **90-108°** — dit keer liggen de twee "actuele" bronnen redelijk dicht bij elkaar (in tegenstelling tot eerdere ochtenden waar ze sterk uiteenliepen).
- Was voorspeld: windwaarnemingen's eigen Harmonie-vsp zag voor 04:00-06:00 slechts **7,6-8,6 kts / gust 12,2-13,0 kts, 83-93°**; Soarcast's eigen Harmonie-forecast zag voor dezelfde uren **10,0-11,3 kts / gust 15,0-15,4 kts, 90-98°**; Windfinder/GFS zag voor 01:00-07:00 **8,5-9,0 kts / gust 11,5-13,2 kts, 87-93°**.
- Conclusie: de wind loopt **fors VOOR** op alle drie modellen (ongeveer **+5 à +7 kt** op het gemiddelde, **+4 à +6 kt** op de gust) — een grotere afwijking dan gebruikelijk. Rest-van-de-dag inschatting: **classificatie Matig blijft staan (golf 0,1m is en blijft de harde beperking, los van wind), maar met merkbaar meer vertrouwen in de hogere kant van de bandbreedte voor het ochtendvenster (07:00-10:00)** dan de kale modellen (6-9 kts) suggereren — reëel scenario is dat het rond 12-17 kts blijft steken vóór de door alle modellen voorspelde terugval richting het middaguur.

---

## 📅 Komende 72 uur

### Vrijdag — Matig (grensgeval — golf ruim te klein, wind loopt voor op de modellen)
- Windfinder (GFS): 6,0-9,0 kts gem. tijdens daglicht, gust 8,7-13,2 kts, richting ONO/OOST (92-104°, **pal aflandig**). Golf vlak 0,1m, periode 5-6s.
- windwaarnemingen.nl (KNMI-Harmonie, vsp): 5,8-8,7 kts gem. tijdens daglicht, gust 10,5-13,4 kts, richting 74-92° — vergelijkbaar met GFS, allebei duidelijk lager dan wat vanochtend al gemeten wordt (zie realitycheck).
- Soarcast (KNMI-Harmonie, IJmond): 7,1-11,7 kts gem. tijdens daglicht, gust 11,0-15,8 kts, richting 82-95° — iets hoger dan windwaarnemingen, maar ook deze raming ligt ruim onder de actuele waarnemingen van vanochtend.
- Netto: alle drie de kale modellen zien zwakke wind (6-12 kts) die zonder de realitycheck richting Slecht/laag-Matig zou wijzen, maar de actuele metingen liggen 5-7 kt hoger — reëel is dat de ochtend eerder in de 12-17kts-band blijft hangen dan in de voorspelde 6-9 kts. Richting is in alle gevallen prima (pal aflandig, veilig en schoon). Golf blijft echter het hele etmaal op 0,1m steken, ver onder de 1,1m-drempel → **Matig**, golf is zonder twijfel de beperkende factor, ongeacht welke windschatting je volgt.
- Pier-logica: niet van toepassing — richting is aflandig, golf (0,1m) ruim onder de 0,8m-drempel.
- Getij: hoogwater 01:17 (2,1m), laagwater 09:45 (0,4m), hoogwater 13:35 (1,8m), laagwater 21:29 (0,2m).
- Beste venster (daglicht): **07:00-10:00** — kale modellen zien hier 8-12 kts/gust 12-16 kts, maar gezien de realitycheck is een reëel scenario 12-17 kts/gust 16-19 kts, richting 82-100° (OOST, pal aflandig), golf 0,1m / 5-6s — vóór de door alle modellen verwachte terugval richting het middaguur.

### Zaterdag — Slecht (vrijwel windstil, golf te klein)
- Windfinder (GFS): 5,0-7,3 kts gem. tijdens daglicht, gust 6,5-11,0 kts, richting draait van OZO (114°) 's ochtends via ZO naar ZZO (163°) in de namiddag. Golf zeer klein (0,12-0,15m), periode 5,4-6,2s.
- windwaarnemingen.nl (KNMI-Harmonie, vsp): 4,3-8,7 kts gem. tijdens daglicht, gust 8,9-13,6 kts, richting 80-137° — vergelijkbaar met GFS.
- Soarcast (KNMI-Harmonie, IJmond): 5,1-10,6 kts gem. tijdens daglicht, gust 9,5-15,0 kts, richting 81-137° — iets hoger dan de andere twee, maar het verschil is klein en verandert niets aan de conclusie.
- Netto: alle drie bronnen zijn het eens — gust blijft overal onder de 16 kts én het gemiddelde onder de 14 kts, de hele dag → **Slecht** (voldoet overduidelijk aan de Slecht-conditie, geen afwijkende modellen deze keer). Golf is met 0,1-0,15m ook ver te klein, dus zelfs als de wind zou meevallen was golf alsnog limiterend.
- Pier-logica: niet van toepassing — golf (0,1-0,15m) ruim onder de 0,8m-drempel.
- Getij: hoogwater 02:03 (2,1m), laagwater 10:25 (0,4m), hoogwater 14:20 (1,9m), laagwater 22:18 (0,3m).

### Zondag — Matig (golf nog klein, forse modelafwijking op wind)
- Windfinder (GFS): 5,8-8,8 kts gem. tijdens daglicht, gust 7,7-12,5 kts, richting 163-188° (**side-shore**, ZZO/ZUID). Golf groeit licht naar 0,30-0,35m, periode zakt van 5,4s naar 4,2s (onder de 5s-drempel vanaf de namiddag).
- windwaarnemingen.nl (KNMI-Harmonie, vsp, t/m 15:00): 7,6-10,9 kts gem., gust 12,8-17,9 kts, richting 168-188° — duidelijk hoger dan GFS.
- Soarcast (KNMI-Harmonie, IJmond, t/m 15:00): 10,0-14,9 kts gem., gust 15,7-21,6 kts, richting 174-192° — nóg hoger, met een piek rond 07:00-09:00 (14,1-14,9 kts / 19,3-21,6 kts gust). **Dit is een forse afwijking t.o.v. Windfinder/GFS (bijna 2x zoveel wind bij Soarcast) en wordt expliciet vermeld i.p.v. gemiddeld.**
- Netto: richting is bij alle drie bronnen consistent side-shore (veilig, fijn om op te varen). Bij het GFS-scenario blijft het qua wind rond Matig/Slecht-grens; bij het Harmonie-scenario (vooral Soarcast) komt de ochtend dicht bij de 14-25kts-band. Golf (0,30-0,35m) is in beide scenario's ruim te klein voor Goed(b) of hoger, en de periode zakt in de loop van de dag onder de 5s → plafond blijft **Matig**, ongeacht welke windschatting uitkomt.
- Pier-logica: niet van toepassing — golf (0,30-0,35m) onder de 0,8m-drempel.
- Getij: hoogwater 02:44 (2,1m), laagwater 10:44 (0,5m), hoogwater 15:01 (2,0m).
- Beste venster (daglicht): **07:00-10:00** — wind 6-9 kts (GFS) tot 10-15 kts (Harmonie-bronnen), gust 10-21,6 kts, richting 174-188° (ZZO/ZUID, side-shore), golf 0,30-0,33m / 5,2-5,4s (beste periode van de dag, nog net rond de drempel).

---

## 🔭 Kans op mooie sessies daarna (dag 4-9)
Windfinder (GFS, enige bron zo ver vooruit) voor **maandag 9 november t/m zaterdag 14 november**:

- **Maandag 9 november**: wind zwak en afnemend (1,6-9,7 kts, gust 2,6-14,4 kts), richting draait van side-shore (175°) via ZZW naar bijna stil → **Slecht**.
- **Dinsdag 10 november**: wind nog steeds zeer zwak (1,2-7,5 kts, gust 2,5-11,5 kts), richting OZO/ZO (101-165°, aflandig-achtig), golf blijft klein (0,14-0,21m) → **Slecht**.
- **Woensdag 11 november**: wind trekt duidelijk aan richting de middag — piek rond 13:00 van **14,1 kts gem. / 21,0 kts gust**, richting ONO (71-96°, **licht aflandig/pal aflandig**, veilig). Golf groeit naar 0,22-0,43m met een prima periode (7,2-8,3s, ruim boven de 5s-drempel) → **Matig, met een sterke piek rond het middaguur die tegen Goed aan schurkt** (wind net in de band, maar golf nog te klein voor Goed(b)).
- **Donderdag 12 november**: wind bescheiden (6,7-10,7 kts, gust 10,9-17,3 kts), richting ENO/ONO (52-78°, licht aflandig). Golf blijft opbouwen: **0,42-0,67m met periode 7,5-8,9s** — ruim boven de 5s-drempel, maar nog altijd onder de 1,1m-hoogtedrempel → **Matig**.
- **Vrijdag 13 november — beste papieren**: wind bouwt door naar **9,6-13,3 kts, gust tot 17,3-22,9 kts**, richting ONO/OOST (78-89°, pal aflandig, veilig). Golf is hier het hoogst van de hele 9-daagse periode: **0,62-0,74m met periode 7,8-8,1s** — de golf komt het dichtst bij de 1,1m/Goed(b)-drempel van de hele outlook, met een uitstekende periode gedurende vrijwel de hele dag (niet maar één piekuur). → **Matig, met de meeste kans om bij een iets hogere windschatting naar Goed(b) te kantelen.**
- **Zaterdag 14 november**: wind loopt verder op tot **11,1-13,9 kts, gust tot 17,1-23,4 kts** — de hoogste wind van de hele outlook-periode, richting ENO (57-73°, licht aflandig). Golf blijft stevig (0,55-0,60m, periode 6,7-7,5s) maar iets lager dan vrijdag → **Matig**, met een oplopende windtrend die erop wijst dat de dagen ná deze 9-daagse horizon mogelijk nog interessanter worden.

**Beste dag: vrijdag 13 november** — golf en periode zijn hier het best van de hele periode (0,62-0,74m / ~8s), met een veilige aflandige richting en bruikbare wind (9,6-13,3 kts, pittige gusts tot 23 kts). **Zaterdag 14 november** is de sterke opvolger door de nog hogere wind. Kans: **laag tot gemiddeld**, en nadrukkelijk onzeker op deze afstand. ⚠️ Onzeker op 4+ dagen — check dichter bij de tijd opnieuw. Let vooral op hoe de oplopende windtrend van woensdag t/m zaterdag zich verder ontwikkelt, en of de golfhoogte op vrijdag/zaterdag de 1,1m-drempel alsnog weet te naderen of te doorbreken.

---
_Bronnen: Windfinder (GFS) · Soarcast (KNMI Harmonie, IJmond) · windwaarnemingen.nl (KNMI, IJmuiden)_
