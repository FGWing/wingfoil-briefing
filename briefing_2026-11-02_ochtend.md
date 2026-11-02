# 🌊 Wingfoil-briefing Zandvoort–Wijk aan Zee
_02-11-2026 · Ochtendbriefing_

⚠️ **Technische kanttekening:** Windfinder is opgehaald via de Astro-JSON op de forecast-pagina (`ForecastSection`/`FcTableWindpreviewContainer` voor dag 1-2 incl. wind+golf+getij, `ForecastDataInit` voor dag 3-11 — in één fetch, geen Superforecast-pagina nodig). Soarcast via de onderliggende grafiek-endpoints (`/sc/plotPerLocAndUnitReact.php?...&unit=m/s|deg`, station IJmond/133, dag vandaag/morgen/overmorgen). windwaarnemingen.nl (IJmuiden) via `database/vsp_vdg_wstats.php?st=IJmuiden1` (vandaag, incl. 10-minuten-actuals t/m 06:10) en `database/vsp_mrg_wstats.php?st=IJmuiden2` (morgen + overmorgen t/m 4 nov 15:00, model-horizon bereikt).

**Netto beeld:** **Maandag** (vandaag) is een stevige **Optimaal**-dag de hele daglichtperiode — en dat met meer vertrouwen dan een kale modellezing zou geven, want de actuals van vanochtend lopen al duidelijk vóór op zowel Windfinder/GFS als de eigen Harmonie-voorspelling. **Dinsdag** blijft nagenoeg identiek aan de inschatting van gisteren: Goed met uitstekende richting/periode, maar golf net te klein voor Optimaal. **Woensdag** is zwakker qua golf (klein en kort) ondanks prima wind/richting → Matig, grensgeval met Goed(b). In de outlook is het beeld somber: de meeste dagen (vrijdag t/m zondag) vallen vrijwel stil, en pas **dinsdag 10 november** komt er weer veel wind — maar dan met een kleine, korte golf en opvallend hoge/wisselende gust (mogelijk een actieve storing), dus met flinke onzekerheid.

---

## ⚡ Snel overzicht
- **Maandag:** **Optimaal** (hele daglichtperiode, bevestigd door de actuals). Beste venster: **10:00-17:00**.
- **Dinsdag:** **Goed** (grensgeval met Optimaal — golf net te klein). Beste venster: **07:00-13:00**.
- **Woensdag:** **Matig** (grensgeval met Goed(b) — golf te klein/kort ondanks prima wind/richting). Beste venster: **07:00-13:00**.
- **Beste dag in de 7 dagen erna:** dinsdag 10 november (onzeker — zie outlook)

---

## ⏰ Realitycheck vandaag
- Laatste actuele uren (04:00-06:10, windwaarnemingen.nl/IJmuiden): **gem. 16,8-19,2 kts** (piek 04:10, 19,2 kts), gust tot **23,6 kts**, richting **NNO (24-35°)**, geleidelijk draaiend iets meer naar NO.
- Was voorspeld: windwaarnemingen.nl's eigen Harmonie-vsp voor dezelfde uren zag **14,4-15,7 kts / 21,2-24,3 kts gust, 14-20° (NNO)**; Windfinder/GFS zag voor 04:00 **15,9 kts / 20,3 kts gust, 19° (NNO)**.
- Conclusie: de wind loopt duidelijk **VOOR** — zowel op het eigen Harmonie-model (+1,5 tot +3,5 kt gemiddeld) als op Windfinder/GFS. Richting draait zoals voorspeld, iets meer richting NO dan vooraf gedacht. Rest-van-de-dag inschatting: classificatie **Optimaal bevestigd, met méér vertrouwen** — de eerder als "grensgeval" te verwachten ochtend blijkt in de praktijk al ruim boven de 14kts-ondergrens te zitten.

---

## 📅 Komende 72 uur

### Maandag — Optimaal
- Windfinder (GFS): 13,7-16,7 kts gem. tijdens daglicht, gust 18,4-23,2 kts, richting NNO (13-33°, **side-shore** t.o.v. Zandvoort's kustlijn 17,5°) de hele dag. Golf bouwt op van 0,08m (nacht) naar 1,1-1,36m vanaf 07:00, periode 5,77-7,29s (ruim ≥5s zodra golf >1,1m is).
- Soarcast (KNMI-Harmonie, IJmond, 07:00-18:00): 15,2-22,5 kts gem., gust 21,0-29,5 kts, richting NNO (12-29°) — ziet duidelijk meer wind dan Windfinder/GFS, zelfde patroon als vorige dagen.
- windwaarnemingen.nl (KNMI-Harmonie, vsp): 11,7-17,5 kts gem. tijdens daglicht, gust 19,4-26,2 kts, richting NNO (10-30°) — tussen Windfinder en Soarcast in.
- **Actuals (zie Realitycheck) bevestigen dat de wind eerder aan de hoge kant van deze spreidng zit.**
- Netto: wind ruim binnen 14-25kts (met de actuals als onderbouwing), golf >1,1m vanaf 07:00 met gezonde periode, richting side-shore → **Optimaal, de hele daglichtperiode**, geen grensgeval meer zoals een kale GFS-lezing zou suggereren.
- Pier-logica: niet van toepassing — richting is side-shore, niet aanlandig bij IJmuiden óf Wijk aan Zee.
- Getij: laagwater 04:18 (0,46m), hoogwater 09:12 (1,64m), laagwater 16:37 (0,35m), hoogwater 21:52 (1,96m).
- Beste venster (daglicht, zon ±07:45-17:05): **10:00-17:00** — wind 13,7-15,2 kts (Harmonie-bronnen 15-22 kts), gust 18,8-19,8 kts (Harmonie-bronnen tot 24-29 kts), richting 13-24° (NNO, side-shore), golf 1,18-1,32m / 6,48-6,78s.

### Dinsdag — Goed (grensgeval met Optimaal — golf net te klein)
- Windfinder (GFS): 11,0-14,1 kts gem., gust 15,5-23,3 kts, richting NO/ONO (39-85°, **side-shore** vroeg → **licht/pal aflandig** vanaf ±10:00 t.o.v. Zandvoort). Golf 0,54-1,2m met gezonde periode van 6,33-7,34s de hele dag — golf neemt gedurende de dag geleidelijk af terwijl richting verder richting aflandig draait.
- Soarcast (KNMI-Harmonie, IJmond): 11,7-15,6 kts gem., gust 16,7-21,2 kts, richting NO/ONO (48-84°) — ziet iets meer wind dan Windfinder/GFS, zelfde patroon als voorgaande dagen.
- windwaarnemingen.nl (KNMI-Harmonie, vsp): 8,0-13,0 kts gem. tijdens daglicht, gust 13,8-20,4 kts, richting NO/ONO (47-83°) — iets lager dan Soarcast maar vergelijkbare richting.
- Netto: richting en golfperiode zijn uitstekend (side-shore → licht/pal aflandig, periode ≥6,3s de hele dag), maar de golfhoogte blijft tijdens daglicht net onder de 1,1m-Optimaal-drempel (0,6-0,94m) → **Goed, grensgeval met Optimaal** — vrijwel identiek aan de inschatting van gisteren voor deze dag.
- Pier-logica: niet van toepassing — richting is side-shore/aflandig, niet aanlandig.
- Getij: laagwater 05:55 (0,51m), hoogwater 10:24 (1,57m), laagwater 17:57 (0,38m), hoogwater 23:08 (1,97m).
- Beste venster (daglicht): **07:00-13:00** — wind 11,0-12,5 kts (Harmonie-bronnen hoger, tot 15,6 kts), gust 15,5-21,5 kts, richting 66-81° (NO/ONO, licht→pal aflandig), golf 0,73-0,94m / 6,86-7,23s (hoogste golf van de dag).

### Woensdag — Matig (grensgeval met Goed(b) — golf te klein/kort)
- Windfinder (GFS): 12,2-15,5 kts gem. tijdens daglicht, gust 18,4-24,2 kts, richting ONO/OOST (70-81°, **licht aflandig → pal aflandig** t.o.v. Zandvoort). Golf klein (0,42-0,48m) met een periode die schommelt tussen 4,22-6,16s (meermaals onder de 5s-drempel).
- Soarcast (KNMI-Harmonie, IJmond, 07:00-15:00, model-horizon bereikt): 11,9-15,6 kts gem., gust 16,3-21,4 kts, richting ONO (68-75°) — vergelijkbaar met Windfinder, bevestigt wind/richting.
- windwaarnemingen.nl (KNMI-Harmonie, vsp, t/m 15:00): 8,9-12,8 kts gem., gust 14,0-20,6 kts, richting ONO/OOST (69-86°) — ziet duidelijk MINDER wind dan Windfinder/Soarcast, een omgekeerd patroon t.o.v. de voorgaande dagen (waar Harmonie juist meer wind zag). **Deze afwijkende modelvergelijking wordt expliciet vermeld i.p.v. gemiddeld.**
- Netto: wind en richting zijn op zich gunstig (deels ≥14kts, mooi aflandig), maar de golf (0,42-0,48m, periode vaak <5s) blijft ver onder zowel de Optimaal- als de Goed(b)-drempel → **Matig, grensgeval met Goed(b)** — golf is hier de beperkende factor, niet wind of richting.
- Pier-logica: niet van toepassing — richting is aflandig, niet aanlandig.
- Getij: laagwater 07:36 (0,45m), hoogwater 11:37 (1,58m), laagwater 19:23 (0,32m).
- Beste venster (daglicht): **07:00-13:00** — wind 14,1-14,6 kts (hoogste van de dag), gust 18,4-24,2 kts, richting 70-75° (ONO, licht aflandig), golf 0,43-0,47m / 5,24-5,77s.

---

## 🔭 Kans op mooie sessies daarna (dag 4-9)
Windfinder (GFS, enige bron zo ver vooruit) voor **donderdag 5 november t/m dinsdag 10 november**:

- **Donderdag 5 november**: wind 10,2-12,9 kts gem. (gust 16,3-22,3 kts), richting ONO/OOST (77-85°, aflandig), golf klein (0,26-0,36m) met korte periode (2,58-4,31s) → **Matig, grensgeval met Goed(b)** (golf te klein/kort).
- **Vrijdag 6 november**: wind zwak (5,3-9,2 kts gem., gust 6,0-13,2 kts) → **Slecht**.
- **Zaterdag 7 november**: wind zeer zwak en sterk wisselend van richting (2,8-8,8 kts, draaiend van ZO naar Z/ZW — doortrekkend front) → **Slecht**.
- **Zondag 8 november**: wind zwak (8,0-10,1 kts gem., gust 10,3-13,1 kts), richting draait van side-shore naar (licht) aanlandig (218-266°) maar irrelevant door windkracht → **Slecht**.
- **Maandag 9 november**: overdag zwak (5,0-10,3 kts), bouwt pas na 19:00 (na zonsondergang) sterk op naar 13,0-15,8 kts/tot 28,7 kts gust uit pal aflandige hoek (111-113°) — binnen het daglicht van deze dag zelf nog **Slecht**, maar wel een signaal dat er iets aan het opbouwen is voor de dag erna.
- **Dinsdag 10 november**: duidelijk de windigste dag van de outlook-periode — wind 11,3-18,3 kts gem., gust **21,7-32,5 kts** (ongewoon hoog en wisselend, wijst op een actieve storing/front), richting draait van ZO via Z naar ZW (125-217°, grotendeels side-shore tot licht aflandig t.o.v. Zandvoort). Golf blijft echter klein (0,38-0,44m) met een periode net rond de 5s-drempel (5,0-5,6s) → wind/richting zouden op zichzelf Optimaal-niveau kunnen zijn, maar de golf blijft fors onder de drempel: **grensgeval, geen eenduidige categorie** — en de hoge, wisselende gust wijst op minder stabiele/mogelijk pittige omstandigheden dan de categorieën alleen laten zien.

**Beste dag: dinsdag 10 november** — de meeste wind van de hele outlook-periode en een bruikbare richting, maar de golf blijft klein en de gust is ongewoon hoog/wisselend. Kans: **laag tot gemiddeld**, en nadrukkelijk onzeker.
⚠️ Onzeker op 4+ dagen — check dichter bij de tijd opnieuw. Let vooral op de periode vrijdag 6 t/m zondag 8 november (vrijwel windstil) en op de aard van het systeem rond 9-10 november (mogelijk storing met pittige vlagen).

---
_Bronnen: Windfinder (GFS) · Soarcast (KNMI Harmonie, IJmond) · windwaarnemingen.nl (KNMI, IJmuiden)_
