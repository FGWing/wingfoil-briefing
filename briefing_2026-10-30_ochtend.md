# 🌊 Wingfoil-briefing Zandvoort–Wijk aan Zee
_30-10-2026 · Ochtendbriefing_

⚠️ **Technische kanttekening:** Windfinder is opgehaald via de Astro-JSON op de forecast-pagina (`FcTableWindpreviewContainer`, wind 3-uurlijks voor alle 10 dagen) + de ingebedde `ForecastDataInit`-component voor golf-/getijdata (die component levert zelf alleen dag 3 t/m 10 — voor vandaag/morgen is daarom via een koppe-render de clientside tabel uitgelezen, die wél golfdata voor alle dagen toont). Soarcast via de onderliggende grafiek-endpoints (`plotPerLocAndUnitReact.php?...&unit=m/s|deg`, station IJmond/133). windwaarnemingen.nl (IJmuiden) via `vsp_vdg_wstats.php` (vandaag, incl. 10-minuten-actuals) en `vsp_mrg_wstats.php` (morgen+overmorgen).

**Netto beeld:** drie zwakke-winddagen op rij (vrijdag t/m zondag), bevestigd door alle drie bronnen — nergens komt de wind boven de Slecht-drempel uit. De outlook (dag 4-9) laat een opvallende bijstelling zien t.o.v. gisteren: **maandag 2 november** is gezakt van een duidelijke Optimaal-dag naar een zwak grensgeval, terwijl **dinsdag 3 november** nu als beste kans naar voren komt.

---

## ⚡ Snel overzicht
- **Vrijdag:** **Slecht** (te weinig wind, hele dag) — alle drie bronnen eens.
- **Zaterdag:** **Slecht** (te weinig wind, hele dag) — middag relatief sterkst, maar blijft onder de drempel.
- **Zondag:** **Slecht** (te weinig wind, hele dag) — zwakste en meest wisselende dag van de drie.
- **Beste dag in de 7 dagen erna:** dinsdag 3 november (Goed, grensgeval met Optimaal)

---

## ⏰ Realitycheck vandaag
- Laatste actuele uren (04:00-06:20, windwaarnemingen.nl/IJmuiden): **gem. 4,0 kts (2,3-5,9), gust gem. 5,4 kts (piek 7,4 kts), richting 92-108° (Oost/OZO)**.
- Was voorspeld voor dit venster: **windwaarnemingen.nl/KNMI-Harmonie (eigen vsp)** 3,5-4,7 kts gem., gust 6,4-7,0 kts, richting 102-131° (OZO/ZO). **Windfinder/GFS** 5,4-5,8 kts, gust 6,9-7,7 kts, richting 111-114° (OZO). **Soarcast/KNMI-Harmonie** (eerste beschikbare punt 07:00): 6,9 kts/9,1 kts/123°.
- Conclusie: de wind loopt licht **ACHTER** op alle drie modellen (vooral t.o.v. Windfinder en Soarcast; het eigen KNMI-Harmonie-model van windwaarnemingen.nl zat er het dichtst bij), richting komt redelijk overeen (Oost/OZO, actueel iets minder zuidelijk dan voorspeld). Rest-van-de-dag inschatting: **classificatie ongewijzigd (Slecht)** — de afwijking wijst zo nodig naar nóg minder wind, geen reden om naar boven bij te stellen.

---

## 📅 Komende 72 uur

### Vrijdag — Slecht (te weinig wind, hele dag)
- Windfinder (GFS): 5,0-7,2 kts gem., gust 6,1-12,6 kts, richting Oost/OZO (76-115°, licht tot pal aflandig t.o.v. Zandvoort) de hele dag. Golf 0,2-0,3m / 4-6s.
- windwaarnemingen.nl (KNMI-Harmonie, vsp): 3,5-10,1 kts gem., gust 5,4-15,7 kts, richting 74-131° (Oost/OZO/ZO) — sterkste punt rond 20:00-21:00, net onder de 16kts-gustdrempel.
- Soarcast (KNMI-Harmonie, IJmond, 07:00-18:00): 5,6-10,4 kts gem., gust 7,5-14,5 kts, richting 76-123°.
- **Alle drie bronnen eens: geen enkel uur komt boven de Slecht-drempel (gust <16 kts én gem. <14 kts) uit**, ook niet op het sterkste moment rond de vroege avond.
- Pier-logica: niet van toepassing — golf (0,2-0,3m) ruim onder de 0,8m-drempel.
- Getij: laagwater 01:28 (0,3m), hoogwater 06:04 (2,1m), laagwater 13:57 (0,4m), hoogwater 18:20 (2,3m).

### Zaterdag — Slecht (te weinig wind, hele dag)
- Windfinder (GFS): 4,4-7,2 kts gem., gust 6,3-11,6 kts, richting Oost/OZO (39-100°) overdag, draaiend naar side-shore/NO (39-55°) in de late middag/avond.
- windwaarnemingen.nl (KNMI-Harmonie, vsp): 2,1-9,3 kts gem., gust 5,4-15,7 kts, richting 19-122° (Oost/OZO overdag, NO/NNO in de avond) — piek rond 12:00-14:00 (gust tot 15,7 kts, net onder de drempel).
- Soarcast (KNMI-Harmonie, 07:00-18:00): 7,3-11,2 kts gem., gust 10,7-16,2 kts, richting 77-122° — iets hoger dan de andere twee; gust komt om 14:00 kortstondig net over 16 kts (16,2), maar het gemiddelde (11,2 kts) blijft ruim onder 14, dus de combinatie-eis voor Slecht blijft gelden.
- **Drie bronnen eens: blijft onder de Slecht-drempel.** Zaterdagmiddag (12:00-15:00) is het relatief sterkste, nog niet bruikbare moment.
- Pier-logica: niet van toepassing — golf (0,1-0,2m) zeer klein.
- Getij: laagwater 02:14 (0,3m), hoogwater 06:53 (1,9m), laagwater 14:45 (0,3m), hoogwater 19:08 (2,2m).

### Zondag — Slecht (te weinig wind, hele dag)
- Windfinder (GFS): 3,2-5,6 kts gem., gust 4,8-7,6 kts, richting sterk wisselend (4-81°, Noord/NNO/NO/ONO, side-shore tot licht aflandig).
- windwaarnemingen.nl (KNMI-Harmonie, vsp): 2,1-7,8 kts gem., gust 4,9-11,5 kts, richting 1-359° (Noord/NNO/NNW), geleidelijk draaiend.
- Soarcast (KNMI-Harmonie, 07:00-15:00): 3,9-9,4 kts gem., gust 5,7-12,2 kts, richting 0-30° (Noord/NNO) — sluit goed aan bij windwaarnemingen.nl.
- **Drie bronnen eens: zwakste en meest wisselende dag van de drie**, geen enkel uur in de buurt van een bruikbare drempel.
- Pier-logica: niet van toepassing — golf max. 0,19m.
- Getij: laagwater 03:10 (0,39m), hoogwater 07:54 (1,77m), laagwater 15:37 (0,32m), hoogwater 20:12 (2,02m).

---

## 🔭 Kans op mooie sessies daarna (dag 4-9)
Windfinder (GFS, enige bron zo ver vooruit) voor **maandag 2 november t/m zaterdag 7 november**:

- **Maandag 2 november**: wind bouwt op na een zwak begin tot **9,0-13,4 kts gem.** (gust 14,8-18,6 kts) overdag, richting Noord/NNO (14-48°, nagenoeg side-shore t.o.v. Zandvoort's kustlijn van 17,5°), golf stijgt rond het middaguur naar **0,76-1,04m / 6,7-7,5s** — net onder de 1,1m-Optimaal-drempel. Blijft overwegend **Matig/grensgeval met Goed(b)**, met zelfs een paar uren (13:00, 16:00, 22:00) die weer onder de Slecht-drempel zakken. ⚠️ Dit is een forse neerwaartse bijstelling t.o.v. gisteren, toen deze dag nog als duidelijke Optimaal-dag werd ingeschat — een goed voorbeeld van de onzekerheid op 4+ dagen vooruit.
- **Dinsdag 3 november — beste dag**: wind bouwt vanaf de ochtend op tot **13,4-16,0 kts gem.** (gust 18,2-25,8 kts) vanaf ongeveer 10:00, richting Oost/ONO (72-95°, licht tot pal aflandig t.o.v. Zandvoort — lekker schoon van het strand af), golf **0,54-0,83m met een gezonde periode van 6,3-7,6s**. Wind en richting voldoen aan de Optimaal-eisen, maar de golf blijft net onder de 1,1m-drempel → **Goed, grensgeval met Optimaal**. Breedste venster: ongeveer **10:00-22:00**.
- **Woensdag 4 november**: vergelijkbaar stevige wind (14,2-15,8 kts gem., gust 21,3-24,9 kts), richting Oost/OZO (71-86°, pal aflandig), maar de golf is kleiner en de periode zakt in de loop van de dag van 6,2s naar 3,7s (korter/choppy) → ook een grensgeval Goed/Matig, maar minder aantrekkelijk dan dinsdag door de kortere golfperiode.
- **Donderdag 5 november**: wind iets minder (11,5-13,7 kts gem., gust 17,6-23,3 kts), golf klein en kort (0,28-0,32m / 3,0-4,3s) → **Matig**.
- **Vrijdag 6 november**: wind zwak (6,4-10,2 kts, gust 8,5-15,4 kts) → **Slecht**.
- **Zaterdag 7 november**: wind zwak en zeer wisselend van richting (1,3-13,3 kts, gust 1,9-15,2 kts; draait van side-shore via kortstondig pal aanlandig rond het middaguur weer naar side-shore in de avond) → **Slecht**.

**Beste dag: dinsdag 3 november** — stevige, bouwende wind met een schone aflandige richting en een golf met gezonde periode, net onder de Optimaal-drempel qua hoogte. Woensdag 4 november is een goed alternatief (iets windiger, maar kortere/choppy golf). Kans: **gemiddeld tot hoog voor dinsdag**, maar gezien de forse bijstelling van maandag sinds gisteren extra onzeker.
⚠️ Onzeker op 4+ dagen — check dichter bij de tijd opnieuw.

---
_Bronnen: Windfinder (GFS) · Soarcast (KNMI Harmonie, IJmond) · windwaarnemingen.nl (KNMI, IJmuiden)_
