# 🌊 Wingfoil-briefing Zandvoort–Wijk aan Zee
_08-11-2026 · Ochtendbriefing_

⚠️ **Technische kanttekening:** Windfinder opgehaald via de embedded Astro-JSON (`FcTableWindpreviewContainer` voor wind, `ForecastDataInit` voor golf+getij) op zowel de forecast- als de weatherforecast-pagina — samen dekken deze dag 1 t/m 9 (vandaag deels hourly via de weatherforecast-pagina, dag 4-9 3-uurs via de forecast-pagina). Soarcast via de `plotPerLocAndUnitReact.php`-JSON-endpoints (snelheid/gust + richting, los) voor vandaag/morgen/overmorgen, incl. eigen IJmond-sensor-actuals t/m nu. windwaarnemingen.nl via de `vsp_vdg_wstats.php`/`vsp_mrg_wstats.php`-endpoints (IJmuiden), incl. 10-minutenactuals t/m nu. Alle ruwe snelheden in m/s, hier omgerekend naar kts.

**Netto beeld:** **Zondag (vandaag)** is een grensgeval **Matig/Slecht** met een forse modelafwijking: Windfinder/GFS blijft de hele dag ruim onder de Slecht-drempel (6,9-9,5kts, golf 0,2-0,3m), maar Soarcast én windwaarnemingen (beide Harmonie) zien onafhankelijk van elkaar een duidelijke piek rond **09:00-10:00** (14-16kts, gust tot 19-21kts) — de realitycheck bevestigt dat de actuele wind dicht bij de Harmonie-kant van de bandbreedte zit, wat het vertrouwen in die piek verhoogt. Golf blijft hoe dan ook te klein voor meer dan Matig. **Maandag** is overtuigend **Slecht** — alle drie bronnen zijn het eens (zwakke wind, golf <0,35m). **Dinsdag** is weer een grensgeval **Matig/Slecht**: GFS blijft onder de drempel, maar beide Harmonie-bronnen zien een middagpiek (10:00-13:00, gust tot 17,1-17,7kts) die er net overheen gaat, al blijft golf (0,11-0,13m) ook hier de beperkende factor. De outlook (dag 4-9) bevestigt het beeld van vorige week: de wind trekt vanaf **donderdag 12 november** fors aan, met **vrijdag 13 november** als beste papieren — stevige wind (tot 15,9kts/19,5kts gust) uit een veilige side-shore hoek, gecombineerd met de hoogste golf van de hele periode (tot 1,01m/7,3-8,4s) — net onder de Optimaal-drempel, maar het dichtst erbij van de hele 9-daagse horizon.

---

## ⚡ Snel overzicht
- **Zondag:** **Matig** (grensgeval met Slecht — forse afwijking GFS vs. Harmonie-modellen; golf hoe dan ook te klein voor meer). Beste venster: **09:00-10:00**.
- **Maandag:** **Slecht** (alle drie bronnen eens: zwakke wind, kleine golf).
- **Dinsdag:** **Matig** (grensgeval met Slecht — GFS blijft onder de drempel, Harmonie-modellen zien een middagpiek). Beste venster: **11:00-12:00**.
- **Beste dag in de 7 dagen erna:** vrijdag 13 november (stevige side-shore wind tot 15,9kts + hoogste golf van de hele periode, tot 1,01m/~8s — grensgeval Goed/Optimaal)

---

## ⏰ Realitycheck vandaag
- Laatste actuele uren (03:00-06:10, windwaarnemingen.nl/IJmuiden): **gem. 5,4-7,4 kts**, gust **7,2-10,2 kts**, richting **103-127°** (OZO/ZO). Soarcast's eigen IJmond-sensor zag over dezelfde uren vergelijkbaar: **gem. 5,4-7,0 kts**, gust **~8,0-10,0 kts**, richting **~103-127°**.
- Was voorspeld: windwaarnemingen's eigen Harmonie-vsp zag voor 03:00-06:00 **5,6-7,8 kts / gust 8,7-12,8 kts, 103-155°**; Soarcast's eigen Harmonie-forecast zag voor dezelfde uren **5,4-7,8 kts / gust 8,2-12,1 kts, 109-160°**; Windfinder/GFS zag voor 01:00-07:00 slechts **2,2-4,7 kts / gust 2,4-6,8 kts, 147-208°**.
- Conclusie: de wind loopt **ongeveer CONFORM** de Harmonie-modellen (Soarcast/windwaarnemingen), maar duidelijk **VOOR** op Windfinder/GFS (+3 à +4 kt op het gemiddelde). Richting vergelijkbaar en veilig (OZO/ZO, pal aflandig voor Zandvoort). Rest-van-de-dag inschatting: **iets meer vertrouwen bijgesteld** richting de Harmonie-kant van de bandbreedte — inclusief de aangekondigde piek rond 09:00-10:00 (14-16kts/19-21kts gust) die Windfinder/GFS niet ziet; de classificatie **Matig blijft staan** als netto-oordeel voor de dag, maar de kans dat die piek zich daadwerkelijk voordoet wordt iets hoger ingeschat dan de kale modellen suggereren.

---

## 📅 Komende 72 uur

### Zondag — Matig (grensgeval met Slecht — forse modelafwijking op wind)
- Windfinder (GFS, 3-uurs, daglicht): 6,9-9,5 kts gem., gust 9,8-13,9 kts, richting 163-201° (**side-shore**, ZZO/ZUID). Golf 0,2-0,3m, periode 4-7s.
- windwaarnemingen.nl (KNMI-Harmonie, vsp, hourly): 7,4-14,0 kts gem., gust 10,9-19,4 kts, richting 157-209° — ziet een duidelijke piek om 09:00 (14,0kts/gust 19,4kts, 206°).
- Soarcast (KNMI-Harmonie, IJmond): 9,7-16,1 kts gem., gust 13,0-21,4 kts, richting 158-209° — ziet dezelfde piek rond 09:00-10:00 (16,1kts/gust 21,4 → 10,9kts/gust 21,0), onafhankelijk bevestigd door windwaarnemingen. **Dit is een forse afwijking t.o.v. Windfinder/GFS en wordt expliciet vermeld i.p.v. gemiddeld.**
- Netto: twee onafhankelijke Harmonie-bronnen zien een piek (gust>16, gem rond 14-16kts) die de Slecht-drempel ruimschoots doorbreekt en qua wind+richting (side-shore, veilig) bijna Optimaal-waardig is — maar golf (±0,25-0,3m) blijft ruim onder de 1,1m-drempel, wat het plafond hoe dan ook op **Matig** houdt. Windfinder/GFS ziet deze piek niet en blijft de hele dag onder de Slecht-drempel. De realitycheck (zie boven) ondersteunt de Harmonie-kant. Netto-oordeel: **Matig**, grensgeval met Slecht buiten het venster.
- Pier-logica: niet van toepassing — golf (0,2-0,3m) ruim onder de 0,8m-drempel.
- Getij: hoogwater 02:44 (2,1m), laagwater 10:44 (0,5m), hoogwater 15:01 (2,0m), laagwater 18:59 (1,0m).
- Beste venster: **09:00-10:00** — Soarcast/windwaarnemingen zien hier 14,0-16,1 kts / gust 19,4-21,4 kts, richting 206-209° (ZZW, side-shore, veilig); Windfinder blijft lager (9,5kts/gust 13,9kts). Golf 0,25-0,3m / ~6s.

### Maandag — Slecht
- Windfinder (GFS, hourly, daglicht): 6,7-8,8 kts gem., gust 8,4-13,5 kts, richting 142-173° (**side-shore/licht aflandig**, ZZO/ZO). Golf blijft klein (0,19-0,33m), periode 3,5-3,7s (de hele dag onder de 5s-drempel).
- windwaarnemingen.nl (KNMI-Harmonie, vsp): 4,7-8,9 kts gem., gust 7,6-13,8 kts, richting 119-158° — vergelijkbaar met GFS, blijft overal ruim onder de Slecht-drempel.
- Soarcast (KNMI-Harmonie, IJmond): 5,4-10,7 kts gem., gust 8,6-15,0 kts, richting 122-159° — iets hoger dan de andere twee, maar ook deze blijft ruim onder de Slecht-drempel (gust<16, gem<14).
- Netto: alle drie de bronnen zijn het eens — zwakke wind de hele dag, geen piek zoals zondag of dinsdag. Golf (0,19-0,33m) en periode (<4s) blijven ruim onder de drempels → **Slecht** staat zonder twijfel vast, ook op golf alleen.
- Pier-logica: niet van toepassing — golf (0,19-0,33m) ruim onder de 0,8m-drempel.
- Getij: hoogwater 03:24 (2,1m), laagwater 11:17 (0,5m), hoogwater 15:38 (2,1m), laagwater 19:47 (1,0m).

### Dinsdag — Matig (grensgeval met Slecht — middagpiek bij beide Harmonie-bronnen)
- Windfinder (GFS, hourly, daglicht): 5,5-8,2 kts gem., gust 9,3-13,9 kts, richting 82-130° (**pal aflandig**, OOST/OZO). Golf blijft extreem klein (0,11-0,13m), periode 6,6-9,0s (ruim boven de 5s-drempel, maar irrelevant door de kleine golf).
- windwaarnemingen.nl (KNMI-Harmonie, vsp): 7,2-10,7 kts gem., gust 10,7-17,1 kts, richting 87-116° — ziet een duidelijke middagpiek rond 11:00-13:00 (10,1-10,7kts/gust 16,7-17,1kts) die de Slecht-drempel (gust≥16) doorbreekt.
- Soarcast (KNMI-Harmonie, IJmond): 7,2-12,1 kts gem., gust 10,3-17,7 kts, richting 88-116° — bevestigt onafhankelijk dezelfde middagpiek (11:00-12:00: 12,1kts/gust 17,3-17,7kts). **Beide Harmonie-bronnen wijken hier af van Windfinder/GFS, wordt expliciet vermeld i.p.v. gemiddeld.**
- Netto: richting is bij alle drie bronnen consistent pal aflandig (veilig). GFS blijft de hele dag onder de Slecht-drempel; beide Harmonie-bronnen zien onafhankelijk een middagpiek die er net overheen gaat. Golf (0,11-0,13m) blijft in alle scenario's ver onder de 1,1m-drempel, dus zelfs in het beste scenario blijft het plafond **Matig** → netto-oordeel voor de dag als geheel: **Matig**, grensgeval met Slecht buiten het venster.
- Pier-logica: niet van toepassing — golf (0,11-0,13m) ruim onder de 0,8m-drempel.
- Getij: hoogwater 04:02 (2,1m), laagwater 11:57 (0,4m), hoogwater 16:14 (2,1m).
- Beste venster: **11:00-12:00** — Soarcast/windwaarnemingen zien hier 10,1-12,1 kts / gust 16,7-17,7 kts, richting 108-117° (OZO, pal aflandig, veilig); Windfinder blijft lager (7,2-7,3kts/gust 13,9kts). Golf 0,11m / ~8s (periode ruim boven drempel, maar golf te klein voor meer dan Matig).

---

## 🔭 Kans op mooie sessies daarna (dag 4-9)
Windfinder (GFS, enige bron zo ver vooruit) voor **woensdag 11 november t/m maandag 16 november**:

- **Woensdag 11 november**: wind zwak-bescheiden (7,2-8,7 kts, gust 10,3-13,3 kts), richting ONO/NO (29-86°, licht aflandig/side-shore, veilig). Golf klein (0,15-0,25m), periode goed (6,2-10,2s) → **Slecht** (wind en golf beide te laag).
- **Donderdag 12 november**: wind trekt fors aan (11,6-16,3 kts gem., gust 15,2-19,3 kts), richting draait naar N/NNW (344-358°, **side-shore** t.o.v. Zandvoort). Golf groeit snel naar 0,28-0,93m met prima periode (5,9-8,6s) → **grensgeval Goed/Optimaal**: wind en richting zijn al optimaal-waardig, golf (tot 0,93m) blijft net onder de 1,1m-drempel.
- **Vrijdag 13 november — beste papieren van de hele periode**: wind blijft stevig, **9,5-15,9 kts gem., gust 12,1-19,5 kts**, richting blijft N/NNW (344-358°, **side-shore**, veilig). Golf is hier het hoogst van de hele 9-daagse outlook: **tot 1,01m met een uitstekende periode (7,3-8,4s)** — net onder de 1,1m-Optimaal-drempel, maar het dichtst erbij van de hele periode. Netto: **grensgeval Goed/Optimaal**, de beste dag van de outlook.
- **Zaterdag 14 november**: wind valt sterk terug (1,5-7,1 kts), richting draait van N/NNW naar ZUID/ZZO (139-353°, wisselend). Golf blijft nog behoorlijk (0,59-0,81m) maar wind is te zwak → **Slecht**.
- **Zondag 15 november**: wind blijft zwak (7,3-9,1 kts, gust 9,7-16,1 kts), richting ZZO/ZO (137-162°, licht aflandig/side-shore, veilig). Golf daalt langzaam (0,43-0,55m) → **Slecht**, grensgeval met Matig aan het einde van de dag.
- **Maandag 16 november**: wind trekt weer hard aan (9,4-16,2 kts gem., **gust tot 30,7 kts** — zeer grillig, gust/gem-verhouding ongewoon hoog), richting OZO/ZO (104-150°, pal aflandig/licht aflandig, veilig). Golf groeit naar 0,50-1,04m, nog net onder de drempel → **Goed, met een expliciete gustiness-waarschuwing** (de gust is bijna dubbel het gemiddelde — comfortabeler qua consistentie is vrijdag 13).

**Beste dag: vrijdag 13 november** — stevige, bruikbare wind (9,5-15,9 kts) uit een veilige side-shore richting, met de hoogste golf van de hele outlook-periode (tot 1,01m, periode 7,3-8,4s) — net niet genoeg voor Optimaal, maar het dichtst bij de drempel van de hele 9 dagen. Kans: **gemiddeld**, met donderdag 12 en maandag 16 november (laatste met gustiness-voorbehoud) als dichtstbijzijnde alternatieven. ⚠️ Onzeker op 4+ dagen — check dichter bij de tijd opnieuw. Let vooral op of de golfhoogte op donderdag/vrijdag de 1,1m-drempel alsnog overschrijdt, en of maandag 16 november's extreme gustiness in latere runs bevestigd wordt.

---
_Bronnen: Windfinder (GFS) · Soarcast (KNMI Harmonie, IJmond) · windwaarnemingen.nl (KNMI, IJmuiden)_
