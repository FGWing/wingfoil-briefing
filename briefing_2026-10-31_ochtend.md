# 🌊 Wingfoil-briefing Zandvoort–Wijk aan Zee
_31-10-2026 · Ochtendbriefing_

⚠️ **Technische kanttekening:** Windfinder is opgehaald via de Astro-JSON op de forecast-pagina (`FcTableWindpreviewContainer` voor wind 3-uurlijks dag 1-10, plus de server-gerenderde HTML-tabel voor golf-/getijdata dag 1-2) en de `ForecastDataInit`-component (golf-/getij-/winddata dag 3-10). Soarcast via de onderliggende grafiek-endpoints (`/sc/plotPerLocAndUnitReact.php?...&unit=m/s|deg`, station IJmond/133, inclusief actuals voor vandaag). windwaarnemingen.nl (IJmuiden) via `database/vsp_vdg_wstats.php?st=IJmuiden1` (vandaag, incl. 10-minuten-actuals) en `database/vsp_mrg_wstats.php?st=IJmuiden2` (morgen+overmorgen).

**Netto beeld:** vandaag en morgen blijven te zwak (Slecht), maar **maandag 2 november** is een duidelijke Optimaal-dag — de wind bouwt al vanaf de vroege ochtend op tot 12-15 kts gem. (gust 17-24 kts, Soarcast ziet zelfs tot 22 kts/28 kts) uit een nette side-shore hoek (NNO), met golven die vanaf 04:00 boven de 1,1m-drempel komen met een gezonde periode van 6-7,4s. Dit bevestigt de inschatting van gisteren voor **dinsdag 3 november** als beste dag in de outlook (dag 4-9) — vrijwel ongewijzigd t.o.v. gisteren, een geruststellende stabiele voorspelling na de forse bijstelling van eerder deze week.

---

## ⚡ Snel overzicht
- **Zaterdag:** **Slecht** (te weinig wind, hele dag) — alle drie bronnen eens.
- **Zondag:** **Slecht** (te weinig wind, vrijwel hele dag — kort Matig-grensvenster rond 15:00-18:00).
- **Maandag:** **Optimaal** — wind, golf en richting voldoen vanaf de ochtend. Beste venster: **08:00-17:00**.
- **Beste dag in de 7 dagen erna:** dinsdag 3 november (Goed, grensgeval met Optimaal)

---

## ⏰ Realitycheck vandaag
- Laatste actuele uren (04:00-06:10, windwaarnemingen.nl/IJmuiden): **gem. 6,3 kts (4,3-8,0), gust gem. 8,7 kts (piek 11,1 kts), richting 84-129° (Oost/OZO)**.
- Was voorspeld voor dit venster: **windwaarnemingen.nl/KNMI-Harmonie (eigen vsp)** 7,0-7,6 kts gem., gust 11,5-12,1 kts, richting 88-93° (Oost). **Soarcast/KNMI-Harmonie**: laatste uur (05:00-06:00) gem. ca. 5,8 kts/gust 8,5 kts gemeten vs. ca. 8,4-9,1 kts/12-13 kts voorspeld voor diezelfde uren. **Windfinder/GFS** (3-uurs blokken 01h/04h/07h): 7 kts gem., gust 10-12 kts, richting 92-103°.
- Conclusie: de wind loopt licht **ACHTER** op zowel windwaarnemingen.nl's eigen Harmonie-model als Soarcast; Windfinder/GFS zat er deze ochtend het dichtst bij (7 kts voorspeld vs. 6,3 kts actueel). Richting komt goed overeen (Oost/OZO bij alle bronnen). Rest-van-de-dag inschatting: **classificatie ongewijzigd (Slecht)** — de lichte onderschrijding geeft geen aanleiding om naar boven bij te stellen, eerder het tegenovergestelde.

---

## 📅 Komende 72 uur

### Zaterdag — Slecht (te weinig wind, hele dag)
- Windfinder (GFS): 5-7 kts gem., gust 7-12 kts, richting Oost/OZO (63-115°, pal aflandig t.o.v. Zandvoort — mooie richting, maar te weinig wind om iets te doen) de hele dag. Golf 0,1-0,2m / 9-11s.
- windwaarnemingen.nl (KNMI-Harmonie, vsp): 1,6-9,5 kts gem., gust 2,9-14,4 kts, richting 79-167° (Oost/OZO/ZO, draaiend naar ZZO in de avond) — sterkste punt rond 07:00-13:00 (gust 11-13 kts), nergens boven de drempel.
- Soarcast (KNMI-Harmonie, IJmond, hele dag): 3,7-11,5 kts gem. (forecast), gust 5,8-15,4 kts — iets hoger dan de andere twee, maar ook hier blijft de gust ruim onder de 16kts-drempel.
- **Alle drie bronnen eens: geen enkel uur komt boven de Slecht-drempel (gust <16 kts én gem. <14 kts) uit.** Relatief sterkste moment: rond 11:00-14:00 (gust ~12-13 kts), nog niet bruikbaar.
- Pier-logica: niet van toepassing — golf (0,1-0,2m) ruim onder de 0,8m-drempel.
- Getij: laagwater 02:14 (0,3m), hoogwater 06:53 (1,9m), laagwater 14:45 (0,3m), hoogwater 19:08 (2,2m).

### Zondag — Slecht (te weinig wind, vrijwel hele dag)
- Windfinder (GFS): 2-7 kts gem., gust 2-10 kts, richting sterk wisselend (8-341°, Oost/NO vroeg, draaiend via ZZO/ZW naar NNW in de middag/avond). Golf 0,1-0,6m / 5-9s.
- windwaarnemingen.nl (KNMI-Harmonie, vsp): 1,0-12,2 kts gem., gust 3,7-18,5 kts, richting 30-355° (Oost/NO vroeg, draaiend naar NNW/NW vanaf de middag) — **duidelijke piek rond 16:00-17:00** (12,2 kts gem. / 17,3-18,5 kts gust), richting dan NW (310-318°).
- Soarcast (KNMI-Harmonie, IJmond): bevestigt dezelfde piek — 15,2 kts gem. / 18,9 kts gust om 16:00, richting NW (310-328°).
- **Opvallende modelafwijking:** Windfinder/GFS ziet deze piek rond 16:00-17:00 veel zwakker (slechts 5-7 kts/7-10 kts gust) dan de twee Harmonie-bronnen (windwaarnemingen.nl én Soarcast), die onafhankelijk van elkaar wél een duidelijke piek naar 17-19 kts gust tonen — dit wordt expliciet vermeld i.p.v. gemiddeld. Bij de Harmonie-piek is de richting (NW, 310-318°) **pal aanlandig** t.o.v. Zandvoort (287,5°), maar de golf blijft klein (circa 0,2-0,4m geïnterpoleerd), dus geen brandingsgevaar.
- Netto: als de Harmonie-piek uitkomt is 15:00-18:00 een kort **Matig-grensvenster** (wind <15 kts, gust <19 kts, golf klein); de rest van de dag blijft ruim onder de Slecht-drempel. Geen bruikbaar venster voor een volwaardige sessie.
- Pier-logica: niet van toepassing — golf tijdens de piek naar schatting <0,8m.
- Getij: laagwater 03:10 (0,4m), hoogwater 07:54 (1,8m), laagwater 15:37 (0,3m), hoogwater 20:12 (2,0m).

### Maandag — Optimaal
- Windfinder (GFS): 12,4-15,0 kts gem., gust 16,3-21,1 kts, richting NNO (13-35°, **side-shore** t.o.v. Zandvoort's kustlijn van 17,5°) de hele dag. Golf bouwt op van 0,89m (01:00) naar 1,10-1,32m vanaf 04:00, met een gezonde periode van 5,8-7,4s.
- windwaarnemingen.nl (KNMI-Harmonie, vsp): 11,3-15,6 kts gem., gust 17,3-24,1 kts, richting NNO (8-25°) — bouwt al vanaf 02:00 op, sterkste punt rond 15:00 (gust 24,1 kts).
- Soarcast (KNMI-Harmonie, IJmond): 14,6-22,2 kts gem., gust 18,7-28,2 kts, richting NNO (12-24°) — **ziet duidelijk méér wind dan de andere twee bronnen**, vooral in de middag (15:00: 22,2 kts gem./28,2 kts gust). Richting sluit wel goed aan bij Windfinder en windwaarnemingen.nl. Deze afwijking in kracht wordt expliciet vermeld i.p.v. gemiddeld — ga voor de klassering uit van het behoudende gemiddelde van Windfinder/windwaarnemingen.nl, met Soarcast als signaal dat het ook flink hoger kan uitpakken.
- **Alle drie bronnen eens over de kwalificatie Optimaal**: wind in het 14-25kts-bereik (of net erboven volgens Soarcast), golf >1,1m met gezonde periode (≥5s) vanaf de ochtend, richting side-shore — ruim voldaan.
- Pier-logica: niet van toepassing — richting is side-shore, niet (licht) aanlandig.
- Getij: laagwater 04:18 (0,46m), hoogwater 09:12 (1,64m), laagwater 16:37 (0,35m), hoogwater 21:52 (1,96m).
- Beste venster (daglicht): **08:00-17:00** — wind 12-15 kts (Soarcast tot 19-22 kts), gust 17-25 kts, richting 13-25° (NNO, side-shore), golf 1,1-1,3m / 6,4-7,2s.

---

## 🔭 Kans op mooie sessies daarna (dag 4-9)
Windfinder (GFS, enige bron zo ver vooruit) voor **dinsdag 3 november t/m zondag 8 november**:

- **Dinsdag 3 november — beste dag, bevestigt gisteren**: wind 11,6-15,0 kts gem. (gust 16,3-22,4 kts), richting ONO/OZO (23-78°, side-shore vroeg op de dag, draaiend naar licht/pal aflandig in de middag t.o.v. Zandvoort), golf 0,57-1,20m met een gezonde periode van 6,5-7,5s — alleen vroeg in de ochtend (rond 01:00) nog net boven de 1,1m-Optimaal-drempel, overdag net eronder. **Goed, grensgeval met Optimaal** — vrijwel ongewijzigd t.o.v. de inschatting van gisteren. Breedste venster: ongeveer 08:00-18:00.
- **Woensdag 4 november**: vergelijkbaar stevige wind (13,4-14,7 kts gem., gust 17,7-22,9 kts), richting ONO (66-82°, licht tot pal aflandig), maar golf klein en de periode zakt in de loop van de dag van 6,3s naar 4,5s (korter/choppy) → grensgeval **Goed(b)/Matig**, minder aantrekkelijk dan dinsdag.
- **Donderdag 5 november**: wind iets minder (10,6-12,5 kts gem., gust 16,7-21,6 kts), golf klein en kort (0,32-0,38m / 2,9-4,3s) → **Matig**.
- **Vrijdag 6 november**: wind zwak (7,5-9,6 kts gem., gust 12,3-15,4 kts) → **Slecht**.
- **Zaterdag 7 november**: wind zwak (4,9-6,8 kts gem., gust 7,0-10,1 kts) → **Slecht**.
- **Zondag 8 november**: wind zwak en wisselend (3,8-6,8 kts gem., gust 6,2-9,6 kts) → **Slecht**.

**Beste dag: dinsdag 3 november** — stevige, bouwende wind met een schone richting en een golf met gezonde periode, net onder/rond de Optimaal-drempel qua hoogte. Deze inschatting is vandaag vrijwel identiek aan gisteren — een stabiele bevestiging in plaats van een bijstelling. Kans: **gemiddeld tot hoog**.
⚠️ Onzeker op 4+ dagen — check dichter bij de tijd opnieuw.

---
_Bronnen: Windfinder (GFS) · Soarcast (KNMI Harmonie, IJmond) · windwaarnemingen.nl (KNMI, IJmuiden)_
