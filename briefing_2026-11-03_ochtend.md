# 🌊 Wingfoil-briefing Zandvoort–Wijk aan Zee
_03-11-2026 · Ochtendbriefing_

⚠️ **Technische kanttekening:** Windfinder is opgehaald via de Astro-props op de forecast-pagina (`ForecastSection` voor dag 1-2 incl. wind+golf+getij, `ForecastDataInit` voor dag 3-10 — in één fetch, geen Superforecast-pagina nodig; modelrun init 03-11 05:37 UTC). Soarcast via de onderliggende grafiek-endpoints (`/sc/plotPerLocAndUnitReact.php?...&unit=m/s|deg`, station IJmond/133, dag today/tomorrow/dayaftertomorrow — inclusief de eigen actuele sensordata voor vandaag). windwaarnemingen.nl (IJmuiden) via `database/vsp_vdg_wstats.php?st=IJmuiden1` (vandaag, incl. 10-minuten-actuals t/m 06:10) en `database/vsp_mrg_wstats.php?st=IJmuiden2` (morgen + overmorgen t/m 5 nov 15:00, model-horizon bereikt).

**Netto beeld:** **Vandaag (dinsdag)** en **morgen (woensdag)** zijn allebei **Matig, grensgeval met Goed(b)** — wind en richting zijn oké tot prima (aflandig/side-shore), maar de golf blijft met 0,4-0,9m ruim onder de 1,1m-drempel. **Donderdag** zakt verder naar gewoon **Matig** — golf wordt extreem klein en kort. De outlook is grotendeels windstil (vrijdag t/m maandag vrijwel **Slecht**), met **dinsdag 10 november** als beste (zwakke) dag en **woensdag 11 november** als de dag met veruit de meeste energie — maar dan met pal aanlandige wind voor Zandvoort, dus voorlopig **Slecht** geclassificeerd ondanks 17-22kts.

---

## ⚡ Snel overzicht
- **Dinsdag:** **Matig** (grensgeval met Goed(b) — golf net te klein). Beste venster: **07:00-10:00**.
- **Woensdag:** **Matig** (grensgeval met Goed(b) — golf te klein, periode zakt later onder 5s). Beste venster: **10:00-13:00**.
- **Donderdag:** **Matig** (golf zeer klein en kort, ongeacht welke windschatting je volgt). Beste venster: **10:00-13:00**.
- **Beste dag in de 7 dagen erna:** dinsdag 10 november (zwak maar bruikbaar — zie outlook voor de onzekere "grote" dag erna)

---

## ⏰ Realitycheck vandaag
- Laatste actuele uren (04:00-06:10, windwaarnemingen.nl/IJmuiden, bevestigd door Soarcast's eigen IJmond-sensor): **gem. 12,9-15,6 kts** (gem. ~13,9 kts), gust **17,3-22,4 kts**, richting **40-65°** (NO/ONO).
- Was voorspeld: windwaarnemingen's eigen Harmonie-vsp zag voor 04:00-06:00 **10,3-11,9 kts / gust 17,9 kts, 44-52° (NO)**; Windfinder/GFS zag voor 04:00 **14,2 kts / 19,0 kts gust, 42° (NO)**.
- Conclusie: de wind loopt duidelijk **VOOR** op het eigen Harmonie-model van windwaarnemingen.nl (+2 tot +3,5 kt gemiddeld), maar komt goed overeen met Windfinder/GFS en Soarcast. Rest-van-de-dag inschatting: classificatie **Matig/grensgeval Goed(b) blijft staan, met iets meer vertrouwen richting de hogere kant (13-15kt) van de bandbreedte** — golf blijft de beperkende factor vandaag, niet wind.

---

## 📅 Komende 72 uur

### Dinsdag — Matig (grensgeval met Goed(b) — golf net te klein)
- Windfinder (GFS): 12,3-14,2 kts gem. tijdens daglicht, gust 15,9-23,8 kts, richting NO/ONO (48-81°, **side-shore → licht/pal aflandig** t.o.v. Zandvoort). Golf daalt gestaag van 0,94m (07:00) naar 0,56m (22:00), periode gezond (6,28-7,24s, ruim ≥5s) maar golf blijft de hele dag onder de 1,1m-drempel.
- Soarcast (KNMI-Harmonie, IJmond): 11,7-14,4 kts gem. tijdens daglicht, gust 16,3-20,4 kts, richting 52-81° — vergelijkbaar met Windfinder. De eigen actuele sensor meet nu al 12,4-16,1 kts, hoger dan beide modellen voor dit tijdstip (zie Realitycheck).
- windwaarnemingen.nl (KNMI-Harmonie, vsp): 9,1-12,2 kts gem. tijdens daglicht, gust 14,2-19,2 kts, richting 44-83° — duidelijk lager dan Windfinder/Soarcast én lager dan de actuals bevestigen → deze modelrun wordt vandaag met minder vertrouwen gebruikt.
- Netto: wind blijft overwegend onder 15kt, golf daalt tijdens daglicht ruim onder de 1,1m-drempel ondanks gezonde periode → **Matig, grensgeval met Goed(b)** — golf is hier de beperkende factor, niet wind of richting.
- Pier-logica: niet van toepassing — richting is side-shore/aflandig, niet aanlandig.
- Getij: laagwater 05:55 (0,51m), hoogwater 10:24 (1,57m), laagwater 17:57 (0,38m), hoogwater 23:08 (1,97m).
- Beste venster (daglicht, zon 07:40-17:09): **07:00-10:00** — wind 11,6-12,3 kts (actuals/Soarcast tot 14-16kt), gust 17,9-18,2 kts, richting 48-71° (NO/ONO, side-shore→licht aflandig), golf 0,82-0,94m / 6,85-7,04s (hoogste golf van de dag, net onder de 1,1m-drempel).

### Woensdag — Matig (grensgeval met Goed(b) — golf te klein/kort ondanks prima wind/richting)
- Windfinder (GFS): 13,7-15,5 kts gem. tijdens daglicht, gust 20,6-23,6 kts, richting ONO/OOST (70-84°, **licht aflandig → pal aflandig**). Golf klein (0,41-0,45m), periode 5,28-5,55s 's ochtends maar zakt naar 4,49-4,71s in de namiddag/avond (onder de 5s-drempel).
- Soarcast (KNMI-Harmonie, IJmond): 11,5-18,3 kts gem., gust 15,9-25,1 kts, richting 69-88° — ziet rond het middaguur (12:00-14:00) duidelijk meer wind dan Windfinder (17-18kt vs 14-15kt). **Deze afwijking wordt expliciet vermeld i.p.v. gemiddeld.**
- windwaarnemingen.nl (KNMI-Harmonie, vsp): 8,4-15,4 kts gem. tijdens daglicht, gust 13,4-24,5 kts, richting 71-90° — middags vergelijkbaar met Windfinder, 's avonds weer hoger richting Soarcast's niveau.
- Netto: wind en richting zouden op zichzelf richting Optimaal-niveau kunnen gaan (14-25kt band, aflandige hoek), maar de golf blijft met 0,41-0,45m ver onder de 1,1m-drempel en de periode zakt 's middags/avonds onder 5s → **Matig, grensgeval met Goed(b)** — golf is wederom de beperkende factor.
- Pier-logica: niet van toepassing — richting is aflandig, niet aanlandig.
- Getij: laagwater 07:36 (0,45m), hoogwater 11:37 (1,58m), laagwater 19:23 (0,32m).
- Beste venster (daglicht): **10:00-13:00** — wind 14,0-15,3 kts (Soarcast hoger, tot 18,3 kts), gust 20,6-23,6 kts, richting 73-81° (ONO/OOST, licht→pal aflandig), golf 0,42-0,44m / 5,28-5,5s (periode hier nog net ≥5s, beste moment van de dag).

### Donderdag — Matig (golf zeer klein en kort, ongeacht de windschatting)
- Windfinder (GFS): 12,5-14,3 kts gem. tijdens daglicht, gust 19,0-23,5 kts, richting OOST (77-84°, **pal aflandig**). Golf zeer klein (0,29-0,35m) met zeer korte periode (2,58-2,69s, ver onder de 5s-drempel).
- Soarcast (KNMI-Harmonie, IJmond): 13,0-17,9 kts gem., gust 16,3-24,7 kts, richting 83-101° — ziet duidelijk meer wind dan Windfinder (tot 17,9 kts rond 11:00-12:00). **Expliciet afwijkend vermeld.**
- windwaarnemingen.nl (KNMI-Harmonie, vsp, t/m 15:00): 9,7-15,0 kts gem., gust 16,3-23,9 kts, richting 83-100° — tussen Windfinder en Soarcast in, bevestigt de hogere kant rond het middaguur.
- Netto: ongeacht welke windschatting je volgt (12-18kt), de golf blijft het hele etmaal extreem klein en kort → **Matig** — golf is hier zonder twijfel de beperkende factor; ook bij de hogere Soarcast-schatting blijft golf te slecht voor Goed(b) of Optimaal.
- Pier-logica: niet van toepassing — richting is aflandig, niet aanlandig.
- Getij: hoogwater 00:20 (2,02m), laagwater 08:48 (0,37m), hoogwater 12:43 (1,67m), laagwater 20:32 (0,23m).
- Beste venster (daglicht): **10:00-13:00** — wind 13,6-14,2 kts (Soarcast/windwaarnemingen tot 15-17kt), gust 19,0-23,5 kts, richting 80° (OOST, pal aflandig), golf 0,33-0,35m / 2,58-2,69s.

---

## 🔭 Kans op mooie sessies daarna (dag 4-9)
Windfinder (GFS, enige bron zo ver vooruit) voor **vrijdag 6 november t/m woensdag 11 november**:

- **Vrijdag 6 november**: wind zwak (5,5-8,6 kts gem., gust 6,3-12,2 kts), richting ONO/OOST (71-96°, aflandig) → **Slecht**.
- **Zaterdag 7 november**: wind zeer zwak (1,9-4,7 kts), richting draaiend van OZO naar Z/ZZW (101-197°, doortrekkend front) → **Slecht**.
- **Zondag 8 november**: wind zwak (5,4-7,0 kts, gust 4,7-9,5 kts), richting ZZO/Z (125-168°) → **Slecht**.
- **Maandag 9 november**: 's ochtends nog zwak-matig (7,2-9,7 kts, gust kort tot 16,5 kts rond 10:00), richting OZO/ZO (105-131°), neemt in de middag/avond verder af → **Slecht**.
- **Dinsdag 10 november**: wind bouwt gedurende de dag op van 4,9 kts (nacht) naar 12,1 kts (16:00), gust tot 18,5 kts, richting draait van ONO (78°) 's ochtends naar NNO/N (20-37°) 's avonds, golf klein (0,38-0,48m) → **Matig** — de beste dag van deze rustige periode, al blijft het bescheiden.
- **Woensdag 11 november**: duidelijk de windigste dag van de outlook-periode — wind 17,1-22,3 kts gem., gust **19,5-25,1 kts**, richting WNW/W (275-294°) = **pal aanlandig** t.o.v. Zandvoort. Golf bouwt op naar 0,59-0,79m (net onder de 0,8m-pier-drempel) met gezonde periode (6,4-7,0s). Ondanks de stevige wind valt deze dag voor het open strand (Zandvoort) in de categorie **Slecht** vanwege de pal aanlandige richting (verwachte chop/shorebreak zonder piervoordeel). De golf groeit de dag erna nog iets verder door (tot 0,81m op 12 nov) — mogelijk biedt de Zuidpier bij IJmuiden dan enige bescherming, maar dat moet dichter bij de tijd opnieuw gecheckt worden, en als de richting nog iets verder zuidwest/side-shore draait zou dit alsnog een topdag kunnen worden.

**Beste dag: dinsdag 10 november** — bescheiden maar de enige dag in deze periode die boven Slecht uitkomt. **Woensdag 11 november** is de dag om extra te volgen: veruit de meeste energie, maar momenteel de verkeerde (onshore) hoek voor Zandvoort. Kans: **laag tot gemiddeld**, en nadrukkelijk onzeker.
⚠️ Onzeker op 4+ dagen — check dichter bij de tijd opnieuw. Let vooral op vrijdag 6 t/m maandag 9 november (vrijwel windstil) en op hoe de richting rond 10-11 november zich verder ontwikkelt.

---
_Bronnen: Windfinder (GFS) · Soarcast (KNMI Harmonie, IJmond) · windwaarnemingen.nl (KNMI, IJmuiden)_
