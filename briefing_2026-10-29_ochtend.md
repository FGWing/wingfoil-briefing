# 🌊 Wingfoil-briefing Zandvoort–Wijk aan Zee
_29-10-2026 · Ochtendbriefing_

⚠️ **Technische kanttekening:** Alle drie bronnen waren deze run bereikbaar, **inclusief Soarcast** (de client-side React-pagina zelf blijft leeg zonder browser-sessie, maar de onderliggende grafiek-endpoint `/sc/plotPerLocAndUnitReact.php?location=133&forecastToShow=harm&runsToShow=lastOnly&unit=m/s` (en `unit=deg` voor richting) levert wél bruikbare JSON op — zowel de KNMI-Harmonie-voorspelling als de 10-minuten-actuals bij meetstation IJmond). Windfinder is opgehaald via de Astro-JSON op de forecast-pagina (deze bevatte in één keer alle 10 dagen 3-uurlijks, inclusief golfdata — de losse Superforecast-pagina was niet nodig). windwaarnemingen.nl (IJmuiden) via de vsp-database-endpoints (`vsp_vdg_wstats.php` voor vandaag incl. 10-minuten-actuals, `vsp_mrg_wstats.php` voor morgen+overmorgen tot 15:00u).

**Netto beeld:** drie opeenvolgende **Slecht**-dagen (donderdag t/m zaterdag), bevestigd door alle drie bronnen — windkracht komt op geen moment van de drie dagen boven de Slecht-drempel uit. De Realitycheck laat wel een opvallende **richtingsafwijking** zien: de actuele wind staat vanochtend duidelijk zuidelijker (ZZW/Zuid) dan alle drie modellen voorspelden (WZW/West) — de windkracht zelf loopt uiteen per meetstation. De outlook (dag 4-9) is wél bemoedigend: **maandag 2 november** tekent zich af als een duidelijke **Optimaal**-dag.

---

## ⚡ Snel overzicht
- **Donderdag:** **Slecht** (te weinig wind, hele dag) — alle drie bronnen eens.
- **Vrijdag:** **Slecht** (te weinig wind, hele dag) — windrichting aflandig (oost/zuidoost), maar irrelevant door windkracht.
- **Zaterdag:** **Slecht** (te weinig wind, hele dag) — lichte verbetering rond het middaguur volgens windwaarnemingen.nl, maar blijft ruim onder de drempel.
- **Beste dag in de 7 dagen erna:** maandag 2 november (Optimaal)

---

## ⏰ Realitycheck vandaag
- Laatste actuele uren (04:00-06:10): **windwaarnemingen.nl/IJmuiden: gem. 9,1 kts, gust gem. 11,0 kts (piek 12,3 kts), richting 178-208° (Zuid/ZZW)**. **Soarcast/IJmond (nog geen 2 km verderop): gem. 6,2 kts, gust gem. 7,9 kts (piek 9,1 kts), richting 198-227° (ZZW/ZW)**.
- Was voorspeld voor dit venster: **Windfinder/GFS** ~5,4-5,8 kts gem., gust 7,0-8,2 kts, richting 248-256° (WZW). **windwaarnemingen.nl/KNMI-Harmonie (vsp)** 7,6-8,4 kts gem., gust 10,3-11,5 kts, richting 262-274° (West). **Soarcast/KNMI-Harmonie** 8,4-8,9 kts gem., gust 10,5-11,5 kts, richting 258-271° (West).
- Conclusie: de **windkracht** loopt uiteen per station — windwaarnemingen.nl meet zelf iets **harder dan zijn eigen modelvoorspelling** (+1,2 kt), Soarcast juist **zwakker dan zijn eigen modelvoorspelling** (-2,4 kt). Belangrijker is de **richting**: beide meetstations zitten dit venster 60-90° zuidelijker (Zuid/ZZW/ZW) dan alle drie modellen voorspelden (WZW/West) — een duidelijke en consistente afwijking. Rest-van-de-dag inschatting: **windkracht-classificatie ongewijzigd (Slecht, te weinig wind)** — de bias is niet groot genoeg om de dag bruikbaar te maken — maar houd er rekening mee dat de wind vandaag mogelijk **meer side-shore/zuidelijk** staat dan de modeltabellen hieronder suggereren, met name als de huidige zuidelijke component aanhoudt.

---

## 📅 Komende 72 uur

### Donderdag — Slecht (te weinig wind, hele dag)
- Windfinder (GFS): wind daalt van 5,8 kts 's nachts naar 2,5 kts in de namiddag (gust 8,2→2,5 kts), trekt 's avonds weer iets aan tot 4,4 kts. Richting zeer wisselend door de dag: WZW/West (~248-256°) 's nachts, draait via ZW (217-229°) in de ochtend naar WNW/NW/Noord (322-331°) in de namiddag en NO/OZO (42-102°) in de avond — typisch beeld bij een zwakke-wind-dag zonder dominant drukpatroon.
- windwaarnemingen.nl (KNMI-Harmonie, vsp): bevestigt zwakke wind, 1,6-9,1 kts gem., gust 4,5-12,2 kts; richting overdag grotendeels West/ZW (204-292°), draaiend naar Noord/Oost (353-134°) in de avond.
- Soarcast (KNMI-Harmonie, locatie IJmond): sluit hierbij aan — 1,2-10,7 kts gem., gust 3,3-12,8 kts, richting eveneens sterk wisselend (10-327°, zelfde patroon als de andere twee bronnen).
- **Alle drie bronnen eens: geen enkel uur komt boven de Slecht-drempel (gust <16 kts én gem. <14 kts) uit.** De vroege ochtend (tot ~07:00) is relatief het sterkst van de dag, zie Realitycheck.
- Pier-logica: feitelijk niet van toepassing — golf (Windfinder, enige golfbron) is 0,32-0,86m/4,2-5,4s en komt alleen rond middernacht/01:00 net over de 0,8m-pierdrempel (richting dan ~248°, net pal aanlandig voor IJmuiden) — maar zonder bruikbare windkracht heeft dat geen praktische betekenis.
- Getij: laagwater 00:50 (0,33m), hoogwater 05:19 (2,2m), laagwater 13:12 (0,42m), hoogwater 17:36 (2,3m).

### Vrijdag — Slecht (te weinig wind, hele dag)
- Windfinder (GFS): 4,0-6,5 kts gem., gust 4,5-10,1 kts, richting Oost/ZO (84-130°, aflandig t.o.v. Zandvoort) de hele dag, met een lichte piek rond 19:00-22:00.
- windwaarnemingen.nl (KNMI-Harmonie, vsp): 2,1-8,2 kts gem., gust 5,4-13,4 kts, richting eveneens Oost/ONO/ZO (67-144°) — iets hoger dan Windfinder maar zelfde patroon.
- Soarcast (KNMI-Harmonie): 2,1-10,5 kts gem., gust 5,2-14,2 kts, richting 66-145° — sluit nauw aan bij windwaarnemingen.nl (logisch, zelfde onderliggende model).
- **Drie bronnen eens op een windstille dag** → hoog vertrouwen. Hoogste waarden (gust tot ~14 kts) rond 15:00-21:00, nog steeds ruim onder de Goed/Matig-drempel.
- Pier-logica: niet van toepassing — golf (Windfinder) blijft klein, 0,18-0,29m, ruim onder de 0,8m-pierdrempel.
- Getij: laagwater 01:28 (0,33m), hoogwater 06:04 (2,08m), laagwater 13:57 (0,36m), hoogwater 18:20 (2,26m).

### Zaterdag — Slecht (te weinig wind, hele dag)
- Windfinder (GFS): 3,4-6,5 kts gem., gust 3,7-10,2 kts, richting Oost/OZO (68-107°, licht aflandig tot pal aflandig). Golven zeer klein maar met ongewoon lange periode: 0,14-0,16m / 7,0-10,9s — een uitgedempte restswell zonder noemenswaardige energie.
- windwaarnemingen.nl (KNMI-Harmonie, vsp, beschikbaar t/m 14:00): 4,9-8,7 kts gem., gust 7,2-14,6 kts, richting Oost/OZO (69-116°) — iets hoger dan Windfinder, met een voorzichtige piek rond het middaguur (gust 14,4-14,6 kts).
- Soarcast (KNMI-Harmonie, t/m 14:00): 6,2-10,7 kts gem., gust 8,7-15,0 kts, richting 77-117° — bevestigt dezelfde lichte middagpiek, nog iets hoger dan windwaarnemingen.nl.
- **Drie bronnen eens: blijft onder de Slecht-drempel**, maar de twee KNMI-bronnen laten wel zien dat zaterdagmiddag het minst slechte moment van de drie dagen is (gust net onder 15-16 kts). Geen bruikbaar venster te verwachten.
- Pier-logica: niet van toepassing — golf te klein (max 0,16m), wind te zwak.
- Getij: laagwater 02:14 (0,35m), hoogwater 06:53 (1,93m), laagwater 14:45 (0,32m), hoogwater 19:08 (2,17m).

---

## 🔭 Kans op mooie sessies daarna (dag 4-9)
Windfinder (GFS, enige bron zo ver vooruit) voor **zondag 1 november t/m vrijdag 6 november**:

- **Zondag 1 november**: overdag zwak en wisselend (1,0-9,8 kts), maar vanaf de avond trekt de wind duidelijk aan: 19:00 **16,8 kts gem./21,2 kts gust**, 22:00 16,4/21,9 kts, richting 14-17° (Noord, nagenoeg exact side-shore t.o.v. Zandvoort) — een **grensgeval tussen Optimaal en Goed(a)**: wind en richting zijn ideaal, maar de golf is met 0,59-0,89m (periode 4,8-5,2s) nog net onder de 1,1m-drempel.
- **Maandag 2 november — beste dag, duidelijk Optimaal**: wind blijft vrijwel de hele dag stevig, **15,7-20,3 kts gem.** (piekgust tot **27,7 kts** rond 16:00), richting 2,5-39° (Noord/NNO/NO, side-shore t.o.v. Zandvoort), én de golf bouwt op tot **1,11-1,54m met periode 5,9-7,6s**. Dit voldoet van ~04:00 tot in de avond ruim aan alle drie Optimaal-criteria (wind 14-25 kts, golf >1,1m én periode ≥5s, side-shore) — de duidelijkste "pure" Optimaal-dag in weken, een stuk beter dan de vorige inschatting van gisteren (toen nog een grensgeval). Breedste venster: **ongeveer 04:00-22:00**.
- **Dinsdag 3 november**: wind zakt naar 10,5-14,4 kts (gust 17,2-23,0 kts), richting 45-77° (NO/ONO, licht aflandig tot aflandig), golf 0,64-0,95m/6,0-7,0s → grensgeval Matig/Goed(b).
- **Woensdag 4 november**: wind verder terug naar 9,1-11,6 kts (gust 15,8-19,1 kts), richting 60-76° (ONO), golf 0,59-0,69m/5,8-6,1s → **Matig**.
- **Donderdag 5 november**: zwak, 5,8-10,4 kts (gust 8,4-16,0 kts), richting 37-77°, golf 0,66-0,77m/6,1-6,4s → **Matig/Slecht grensgeval**.
- **Vrijdag 6 november**: 7,5-10,4 kts (gust 11,8-14,5 kts), richting 25-77° (NO/ONO), golf 0,67-0,80m/6,5-6,6s → **Matig**.

**Beste dag: maandag 2 november** — een duidelijke Optimaal-dag met wind, richting, golfhoogte én golfperiode allemaal in de juiste range, en een breed venster van zo'n 18 uur. Zondagavond 1 november is een kansrijke opwarmer (grensgeval Optimaal/Goed). Kans: **hoog voor maandag specifiek**, maar met de gebruikelijke onzekerheid op 4+ dagen vooruit.
⚠️ Onzeker op 4+ dagen — check dichter bij de tijd opnieuw.

---
_Bronnen: Windfinder (GFS) · Soarcast (KNMI Harmonie, IJmond) · windwaarnemingen.nl (KNMI, IJmuiden)_
