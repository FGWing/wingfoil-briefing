# 🌊 Wingfoil-briefing Zandvoort–Wijk aan Zee
_01-11-2026 · Ochtendbriefing_

⚠️ **Technische kanttekening:** Windfinder is opgehaald via de Astro-JSON op de forecast-pagina (`FcTableWindpreviewContainer`/`ForecastSection` voor wind+golf+getij dag 1-2, `ForecastDataInit` voor dag 3-10 — in één fetch, dus de aparte Superforecast-pagina was niet nodig). Soarcast via de onderliggende grafiek-endpoints (`/sc/plotPerLocAndUnitReact.php?...&unit=m/s|deg`, station IJmond/133, dag vandaag/morgen/overmorgen). windwaarnemingen.nl (IJmuiden) via `database/vsp_vdg_wstats.php?st=IJmuiden1` (vandaag, incl. 10-minuten-actuals t/m 06:10) en `database/vsp_mrg_wstats.php?st=IJmuiden2` (morgen + overmorgen t/m 15:00, model-horizon bereikt).

**Netto beeld:** vandaag (zondag) blijft overal te zwak (Slecht). **Maandag** is een grensgeval-Optimaal-dag — wind bouwt op naar 13-14 kts met golf die pas vanaf de namiddag (±13:00) boven de 1,1m-drempel komt; de Harmonie-bronnen (Soarcast/windwaarnemingen) zien duidelijk meer wind/gust dan Windfinder/GFS, dus bij tegenvallend GFS-scenario blijft het beste venster beperkt tot de namiddag. **Dinsdag** blijft vrijwel identiek aan de inschatting van gisteren: Goed met een grensgeval-Optimaal-richting en periode, maar golf net te klein. In de outlook is **woensdag 4 november** het kansrijkst, al is dat fors naar beneden bijgesteld t.o.v. gisteren voor de dagen erna (vooral vrijdag 6 november is sterk afgezwakt in deze modelrun) — een duidelijk signaal om 4+ dagen vooruit niet te vertrouwen.

---

## ⚡ Snel overzicht
- **Zondag:** **Slecht** (te weinig wind, hele dag) — alle drie bronnen eens.
- **Maandag:** **Optimaal** (grensgeval, vooral vanaf de namiddag). Beste venster: **13:00-17:00**.
- **Dinsdag:** **Goed** (grensgeval met Optimaal — golf net te klein). Beste venster: **10:00-16:00**.
- **Beste dag in de 7 dagen erna:** woensdag 4 november (Matig, grensgeval met Goed(b))

---

## ⏰ Realitycheck vandaag
- Laatste actuele uren (04:00-06:10, windwaarnemingen.nl/IJmuiden): **gem. 3,0 kts (04:00) → 2,9 kts (05:00) → 5,6 kts (06:00-06:10)**, gust tot **7,0 kts**, richting draaiend van Zuid (165°) via ZW naar West/WNW (275-282°).
- Was voorspeld (windwaarnemingen.nl's eigen Harmonie-vsp voor dezelfde uren): 04:00 **3,1 kts / 6,2 kts gust, richting 174° (Zuid)**; 05:00 **3,1 kts / 5,1 kts, 222° (ZW)**; 06:00 **4,9 kts / 7,4 kts, 313° (NW)**.
- Conclusie: de wind **KLOPT ongeveer** qua kracht (binnen ~0,5 kt) en loopt bij het laatste uur zelfs licht **VOOR** (5,6 actueel vs. 4,9 kts voorspeld om 06:00). Richting draait zoals voorspeld van Zuid/ZW naar (W)NW. Rest-van-de-dag inschatting: **classificatie ongewijzigd (Slecht)** — zowel Windfinder als windwaarnemingen.nl zien voor de rest van de dag een piek van slechts ~8,0 kts/11,5 kts gust (rond 20:00), ruim onder de Slecht-drempel.

---

## 📅 Komende 72 uur

### Zondag — Slecht (te weinig wind, hele dag)
- Windfinder (GFS): 2,4-7,0 kts gem., gust 3,4-7,5 kts, richting sterk wisselend (24-356°, Oost/NO/Noord — side-shore t.o.v. Zandvoort maar irrelevant door windkracht) de hele dag. Golf 0,10-0,14m / 8,0-8,8s (ruim te klein om iets te doen).
- windwaarnemingen.nl (KNMI-Harmonie, vsp): 0,8-8,0 kts gem., gust 2,1-11,5 kts, richting zeer wisselend (7-360°, draaiend Z→ZW→NW/N→WNW→West gedurende de dag) — sterkste moment rond 20:00 (8,0 kts gem./11,5 kts gust).
- Soarcast (KNMI-Harmonie, IJmond, 07:00-18:00): 0,6-8,5 kts gem. (forecast), gust 5,1-11,5 kts — vergelijkbaar zwak, bevestigt de andere twee bronnen.
- **Alle drie bronnen eens: geen enkel uur komt boven de Slecht-drempel (gust <16 kts én gem. <14 kts) uit.**
- Pier-logica: niet van toepassing — golf (≤0,14m) ruim onder de 0,8m-drempel.
- Getij: laagwater 03:10 (0,39m), hoogwater 07:54 (1,77m), laagwater 15:37 (0,32m), hoogwater 20:12 (2,02m).

### Maandag — Optimaal (grensgeval, vooral vanaf de namiddag)
- Windfinder (GFS): 12,2-14,2 kts gem., gust 17,8-18,6 kts, richting NNO (14-42°, **side-shore** t.o.v. Zandvoort's kustlijn van 17,5°) de hele dag. Golf bouwt op van 0,42m (04:00) naar 0,95-1,18m vanaf 07:00, periode 4,9-6,9s (vanaf 07:00 steeds ≥5,7s).
- windwaarnemingen.nl (KNMI-Harmonie, vsp): 9,9-15,3 kts gem., gust 14,8-26,8 kts, richting NNO/NO (7-41°) — ziet duidelijk hogere gust-pieken (tot 26,8 kts) dan Windfinder/GFS.
- Soarcast (KNMI-Harmonie, IJmond): 15,2-20,9 kts gem., gust 21,5-27,5 kts, richting NNO (6-26°) — ziet nóg meer wind dan windwaarnemingen; bevestigt dat het Harmonie-model duidelijk meer wind/gust ziet dan GFS. **Deze modelafwijking (GFS vs. Harmonie, vooral in de gust) wordt expliciet vermeld i.p.v. gemiddeld.**
- Netto (klassering op het behoudende Windfinder/GFS-gemiddelde): wind zit net aan de 14kts-ondergrens, golf passeert de 1,1m-Optimaal-drempel pas vanaf de namiddag → **Optimaal, grensgeval** — de ochtend (07:00-10:00) is nog Goed(b)-grens (golf <1,0m), vanaf ±13:00 overtuigender Optimaal (golf 1,06-1,18m, periode ≥6,3s, side-shore). Komt het Harmonie-scenario (Soarcast/windwaarnemingen) uit, dan is het de hele dag overtuigend Optimaal.
- Pier-logica: niet van toepassing — richting is side-shore, niet aanlandig bij IJmuiden óf Wijk aan Zee.
- Getij: laagwater 04:18 (0,46m), hoogwater 09:12 (1,64m), laagwater 16:37 (0,35m), hoogwater 21:52 (1,96m).
- Beste venster (daglicht, zon ±07:45-17:10): **13:00-17:00** — wind 13,4-14,0 kts (Harmonie-bronnen 16-19+ kts), gust 17,8-24,9 kts (Harmonie-bronnen tot 22-27 kts), richting 14-25° (NNO, side-shore), golf 1,06-1,18m / 6,3-6,7s.

### Dinsdag — Goed (grensgeval met Optimaal — golf net te klein)
- Windfinder (GFS): 9,9-14,5 kts gem., gust 16,6-23,1 kts, richting NO/ONO (37-79°, **side-shore** vroeg → **licht aflandig** vanaf ±10:00 t.o.v. Zandvoort). Golf 0,56-1,11m met een gezonde periode van 6,5-7,1s de hele dag — golf neemt gedurende de dag geleidelijk af terwijl de wind oploopt.
- windwaarnemingen.nl (KNMI-Harmonie, vsp): 8,4-15,2 kts gem., gust 12,6-24,1 kts, richting NO/ONO (35-77°) — bouwt op in de middag, hogere gust dan Windfinder (tot 24,1 kts), richting sluit goed aan.
- Soarcast (KNMI-Harmonie, IJmond, 07:00-15:00, model-horizon bereikt): 12,9-18,1 kts gem., gust 17,7-24,6 kts, richting NO/ONO (44-80°) — ziet wederom meer wind dan Windfinder/GFS, zelfde patroon als de vorige twee dagen.
- Netto: richting en golfperiode zijn uitstekend (side-shore/licht aflandig, periode ≥6,5s de hele dag), maar de golfhoogte blijft tijdens daglicht net onder de 1,1m-Optimaal-drempel (0,56-0,93m) → **Goed, grensgeval met Optimaal** — vrijwel identiek aan de inschatting van gisteren voor deze dag.
- Pier-logica: niet van toepassing — richting is side-shore/licht aflandig, niet aanlandig.
- Getij: laagwater 05:55 (0,51m), hoogwater 10:24 (1,57m), laagwater 17:57 (0,38m), hoogwater 23:08 (1,97m).
- Beste venster (daglicht): **10:00-16:00** — wind 10,9-14,5 kts (Harmonie-bronnen hoger), gust 16,6-23,1 kts, richting 60-73° (NO/ONO), golf 0,67-0,83m / 6,9-7,1s.

---

## 🔭 Kans op mooie sessies daarna (dag 4-9)
Windfinder (GFS, enige bron zo ver vooruit) voor **woensdag 4 november t/m maandag 9 november**:

- **Woensdag 4 november — beste dag**: wind 11,8-14,9 kts gem. (gust 17,5-22,6 kts), richting ONO (65-77° tijdens daglicht, **licht aflandig** t.o.v. Zandvoort), golf klein (0,41-0,50m) met een periode die afneemt van 5,9s (ochtend) naar 4,6s (middag) → **Matig, grensgeval met Goed(b)** (golf te klein voor Goed(b); richting/wind verder prima). Meeste wind van de hele outlook-periode.
- **Donderdag 5 november**: wind 10,9-13,2 kts gem. (gust 16,0-20,3 kts), golf klein en kort (0,25-0,34m / 2,9-4,7s) → **Matig**.
- **Vrijdag 6 november**: fors naar beneden bijgesteld t.o.v. gisteren (destijds nog 13,4-14,7 kts) — deze run ziet slechts 6,9-9,7 kts gem. (gust 9,3-14,7 kts) → **Slecht**.
- **Zaterdag 7 november**: wind zwak (3,3-5,7 kts gem., gust 4,5-7,0 kts) → **Slecht**.
- **Zondag 8 november**: wind zeer zwak en wisselend van richting (2,0-3,8 kts gem.) → **Slecht**.
- **Maandag 9 november**: blijft overdag zwak (2,7-7,3 kts), bouwt pas na 16:00 op (9,2-10,9 kts, gust tot 21,1 kts) — mogelijk begin van een nieuw windvenster rond 10 november, maar binnen het daglicht van deze dag zelf nog **Slecht tot Matig-grensgeval**.

**Beste dag: woensdag 4 november** — de meeste wind van de outlook-periode, al blijft de golf klein/kort. Kans: **laag tot gemiddeld**.
⚠️ Onzeker op 4+ dagen — check dichter bij de tijd opnieuw. Let vooral op vrijdag 6 november: deze dag is in deze modelrun fors afgezwakt t.o.v. de inschatting van gisteren.

---
_Bronnen: Windfinder (GFS) · Soarcast (KNMI Harmonie, IJmond) · windwaarnemingen.nl (KNMI, IJmuiden)_
