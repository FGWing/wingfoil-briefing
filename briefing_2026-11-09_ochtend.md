# 🌊 Wingfoil-briefing Zandvoort–Wijk aan Zee
_09-11-2026 · Ochtendbriefing_

⚠️ **Technische kanttekening:** Windfinder opgehaald via de embedded Astro-JSON (`FcTableWindpreviewContainer` voor wind, `ForecastDataInit` voor golf+getij) op zowel de weatherforecast-pagina (dag 1-3, hourly) als de forecast-pagina (dag 4-9, 3-uurs). **Data-gat:** Windfinder levert voor vandaag (maandag) geen golf-/getijvoorspelling — het getij voor vandaag is daarom overgenomen uit de briefing van gisteravond (astronomisch, dus onveranderd); golfdata voor vandaag ontbreekt simpelweg. Soarcast via de `plotPerLocAndUnitReact.php`-JSON-endpoints (losse calls voor snelheid/gust in m/s en richting in graden) voor vandaag/morgen/overmorgen, incl. eigen IJmond-sensor-actuals t/m nu. windwaarnemingen.nl via de `vsp_vdg_wstats.php`/`vsp_mrg_wstats.php`-endpoints (station IJmuiden), incl. 10-minutenactuals en de eigen vsp-voorspelling terugwerkend voor dezelfde uren. Alle ruwe snelheden in m/s, hier omgerekend naar kts.

**Netto beeld:** **Maandag (vandaag)** is overtuigend **Slecht** — de wind loopt wel merkbaar voor op Windfinder/GFS (die de hele dag onder 7,5kts blijft hangen), maar zelfs de hogere Harmonie-kant (Soarcast/windwaarnemingen, piek rond 05:00-06:00 met gem. 10,7-11,7kts/gust 14,2-15,7kts) komt niet boven de Slecht-drempel uit, en golfdata voor vandaag is bij Windfinder niet beschikbaar. **Dinsdag** is een duidelijke **Matig** met een scherpe modelafwijking: Windfinder/GFS ziet de hele dag maar 6-9,5kts, terwijl beide Harmonie-bronnen (Soarcast én windwaarnemingen, onafhankelijk van elkaar) in de avond oplopen tot 13,6-15,4kts/gust 15,9-20,6kts uit een veilige pal-aflandige hoek (OOST) — stevige, bruikbare wind, maar de golf (0,1-0,15m) is zo klein dat het plafond ondanks de sterke wind op Matig blijft staan. **Woensdag** is **Matig**: alle drie bronnen zien gematigde wind (6-11kts) uit een veilige side-shore/ONO-hoek, met windwaarnemingen structureel iets hoger dan Windfinder — golf (0,15-0,26m) blijft ruim te klein voor meer. De outlook (dag 4-9) bevestigt het beeld van de afgelopen dagen: vanaf **donderdag 12 november** trekt de wind fors aan, met **vrijdag 13 november** nog steeds als beste papieren (wind stevig in de Optimaal-band, golf tot 1,04m — het dichtst bij de 1,1m-drempel met de minste gustiness), maar nieuw deze run is dat **dinsdag 17 november** als eerste dag van de hele 9-daagse horizon de golfhoogte daadwerkelijk over de 1,1m-drempel laat gaan (tot 1,16m, periode 6,5-7,4s) — de wind blijft daar echter overwegend onder de 14kts-ondergrens en is zeer wisselvallig (gust bijna het dubbele van het gemiddelde).

---

## ⚡ Snel overzicht
- **Maandag:** **Slecht** (alle bronnen eens dat het onder de drempel blijft; Harmonie loopt wel voor op GFS).
- **Dinsdag:** **Matig** (forse modelafwijking — Harmonie-bronnen zien 's avonds stevige wind tot 15,4kts uit veilige hoek, maar golf te klein voor meer). Beste venster: **19:00-23:00**.
- **Woensdag:** **Matig** (alle bronnen eens over gematigde, veilige wind; golf te klein). Beste venster: **08:00-11:00**.
- **Beste dag in de 7 dagen erna:** vrijdag 13 november (wind stevig in de Optimaal-band, golf met 1,04m het dichtst bij de drempel van de hele periode, minste gustiness — dinsdag 17 november is een nieuw alternatief met golf boven de drempel, maar met te zwakke en zeer wisselvallige wind)

---

## ⏰ Realitycheck vandaag
- Laatste actuele uren (04:00-06:00, windwaarnemingen.nl/IJmuiden): **gem. 7,9-9,2 kts**, gust **10,3-12,2 kts**, richting **139-169°** (ZO/ZUID). Soarcast's eigen IJmond-sensor zag over dezelfde uren iets hoger: **gem. 8,6-10,9 kts**, gust **10,9-13,6 kts**, richting **161-199°** (ZO/ZUID/ZZW).
- Was voorspeld: windwaarnemingen's eigen Harmonie-vsp zag voor 04:00-06:00 **7,8-8,4 kts / gust 11,7-13,0 kts, 159-165°**; Soarcast's eigen Harmonie-forecast zag voor dezelfde uren juist iets hoger **10,7-11,7 kts / gust 14,2-15,7 kts, 164-169°**; Windfinder/GFS zag voor diezelfde uren slechts **6,7-7,0 kts / gust 10,7-12,2 kts, 158-169°**.
- Conclusie: de wind loopt **licht VOOR** op windwaarnemingen's eigen Harmonie-vsp en **duidelijk VOOR** op Windfinder/GFS, maar **iets ACHTER** op Soarcast's eigen (iets optimistischere) Harmonie-forecast — de twee Harmonie-bronnen spreiden dus zelf ook een beetje. Richting is bij alle bronnen consistent veilig (ZO-ZZW, aflandig/side-shore voor Zandvoort). Rest-van-de-dag inschatting: **licht meer vertrouwen** richting de Harmonie-kant van de bandbreedte, maar de classificatie **Slecht blijft ongewijzigd** — zelfs Soarcast's eigen (hoogste) forecast-piek voor vanochtend (gem. 11,7kts/gust 15,7kts rond 05:00-06:00) komt niet over de Slecht-drempel (gust≥16 of gem≥14) uit.

---

## 📅 Komende 72 uur

### Maandag — Slecht
- Windfinder (GFS, hourly, daglicht): 4,0-9,0 kts gem., gust 4,4-16,7 kts, richting 92-180° (**licht aflandig/side-shore**, ZZO/ZUID-ONO). Golfdata voor vandaag niet beschikbaar bij Windfinder (data-gat, zie technische kanttekening boven).
- windwaarnemingen.nl (KNMI-Harmonie, vsp, hourly): 2,5-8,4 kts gem., gust 3,9-13,0 kts, richting 88-173° — blijft de hele dag onder de Slecht-drempel.
- Soarcast (KNMI-Harmonie, IJmond): 3,7-11,7 kts gem., gust 6,2-15,7 kts, richting 100-173° — ziet een bescheiden piek rond 05:00-06:00 (11,5-11,7kts/gust 15,7kts), net niet genoeg om de Slecht-drempel te doorbreken.
- Netto: alle drie bronnen blijven de hele dag binnen de Slecht-drempel (gust<16 én gem<14) — zelfs de hoogste Harmonie-piek (Soarcast, 05:00-06:00) komt er net niet overheen. Richting is overal veilig (aflandig/side-shore), maar dat is hier niet de beperkende factor. **Slecht** staat zonder twijfel vast.
- Pier-logica: niet van toepassing — richting niet aanlandig.
- Getij _(overgenomen uit de briefing van gisteravond — astronomisch, dus onveranderd; Windfinder leverde vandaag geen eigen getijdata)_: hoogwater 03:24 (2,1m), laagwater 11:17 (0,5m), hoogwater 15:38 (2,1m), laagwater 19:47 (1,0m).

### Dinsdag — Matig (forse modelafwijking — Harmonie ziet 's avonds stevige wind, GFS niet)
- Windfinder (GFS, hourly, daglicht): 6,2-9,5 kts gem., gust 7,4-14,5 kts, richting 82-139° (**pal aflandig**, OOST/OZO). Golf extreem klein: 0,10-0,15m, periode 3,5-10,5s (wisselend, maar irrelevant door de kleine golf).
- windwaarnemingen.nl (KNMI-Harmonie, vsp, hourly): 2,1-11,7 kts gem., gust 2,9-18,1 kts, richting 61-161° — ziet een duidelijke avondpiek 19:00-23:00 (10,5-11,7kts/gust 15,9-18,1kts, 84-92°).
- Soarcast (KNMI-Harmonie, IJmond): 2,9-15,4 kts gem., gust 5,2-20,6 kts, richting 82-163° — bevestigt onafhankelijk dezelfde avondpiek, zelfs iets hoger (19:00-23:00: 13,6-15,4kts/gust 18,3-20,6kts, 85-93°). **Beide Harmonie-bronnen wijken hier fors af van Windfinder/GFS (dat max. 9,5kts/14,5kts ziet), dit wordt expliciet vermeld i.p.v. gemiddeld.**
- Netto: richting is bij alle drie bronnen consistent pal aflandig/OOST (veilig). De twee onafhankelijke Harmonie-bronnen zien 's avonds stevige, bruikbare wind (gem. 13,6-15,4kts, gust tot 20,6kts) die ruim boven de Slecht-drempel uitkomt en qua wind+richting al optimaal-waardig is — maar de golf (0,10-0,15m) is zo ver onder de 1,1m-drempel dat het plafond hoe dan ook op **Matig** blijft staan, ook al zou je bij dit windniveau normaal richting Optimaal/Goed kijken. Netto-oordeel: **Matig**, met een nadrukkelijke modelafwijking als kanttekening.
- Pier-logica: niet van toepassing — golf (0,10-0,15m) ruim onder de 0,8m-drempel.
- Getij: hoogwater 04:02 (2,1m), laagwater 11:57 (0,4m), hoogwater 16:14 (2,1m).
- Beste venster: **19:00-23:00** — Soarcast/windwaarnemingen zien hier 10,5-15,4 kts / gust 15,9-20,6 kts, richting 82-93° (OOST, pal aflandig, veilig); Windfinder blijft duidelijk lager (8,8-9,5kts/gust 13,6-14,5kts). Golf 0,14-0,15m / ~5-6s (veel te klein voor meer dan Matig, ondanks de stevige wind).

### Woensdag — Matig
- Windfinder (GFS, hourly, daglicht): 6,3-9,0 kts gem., gust 9,4-16,7 kts, richting 40-103° (**side-shore/licht aflandig**, NO-ONO-OZO). Golf 0,15-0,26m, periode 4,9-9,0s (periode prima, golf te klein).
- windwaarnemingen.nl (KNMI-Harmonie, vsp, hourly): 8,4-11,3 kts gem., gust 13,4-17,9 kts, richting 23-81° — structureel iets hoger dan Windfinder, met een piek in de vroege ochtend (00:00-04:00: 9,5-11,3kts/gust 16,1-17,9kts, 69-81°, ONO).
- Soarcast (KNMI-Harmonie, IJmond): tot 15:00 beschikbaar — 8,4-14,2 kts gem., gust 13,4-19,8 kts, richting 23-82° — bevestigt onafhankelijk hetzelfde beeld als windwaarnemingen (structureel hoger dan GFS), met de sterkste waarden rond middernacht/vroege ochtend.
- Netto: richting is bij alle bronnen consistent side-shore tot licht aflandig (NO/ONO/OOST) — veilig, dicht bij de kustlijnhoek. Beide Harmonie-bronnen zien iets meer wind dan GFS, maar zelfs hun bovenkant (tot ~11-14kts gem.) blijft onder de 15kts-grens, en de golf (0,15-0,26m) blijft ruim onder de 1,1m-drempel. Netto-oordeel: **Matig**, zonder noemenswaardige twijfel richting Slecht of Goed.
- Pier-logica: niet van toepassing — golf (0,15-0,26m) ruim onder de 0,8m-drempel.
- Getij: laagwater 00:24 (0,4m), hoogwater 04:39 (2,0m), laagwater 12:38 (0,4m), hoogwater 16:49 (2,2m).
- Beste venster: **08:00-11:00** — Windfinder ziet hier 8,4-8,8 kts / gust 12,6-16,7 kts, richting 51-58° (ONO, side-shore); windwaarnemingen ziet 8,4-10,1 kts / gust 13,8-15,0 kts, richting 28-45° (NNO/NO). Golf 0,19-0,23m / ~5,9-6,4s.

---

## 🔭 Kans op mooie sessies daarna (dag 4-9)
Windfinder (GFS, enige bron zo ver vooruit) voor **donderdag 12 t/m dinsdag 17 november**:

- **Donderdag 12 november**: wind trekt fors aan (14,6-18,0 kts gem., gust 17,0-21,4 kts), richting draait naar N/NNW (326-359°, **licht aanlandig/side-shore** t.o.v. Zandvoort, bij vlagen net over de grens maar nooit pal aanlandig). Golf groeit naar 0,31-0,92m met goede periode (6,3-8,2s) → **grensgeval Goed/Optimaal**: wind en richting zijn al optimaal-waardig, golf blijft net onder de 1,1m-drempel.
- **Vrijdag 13 november — nog steeds de beste papieren van de hele periode**: wind blijft stevig en overwegend binnen de Optimaal-band, **12,6-17,4 kts gem., gust 15,0-22,7 kts**, richting blijft rond N (356-14°, vrijwel exact **side-shore**, veilig). Golf is hier het hoogst van de hele 9-daagse outlook: **tot 1,04m met een uitstekende periode (7,8-8,6s)** — nog net onder de 1,1m-Optimaal-drempel, maar het dichtst erbij, met de minste gustiness van de sterke-winddagen. Netto: **grensgeval Goed/Optimaal**, de beste dag van de outlook.
- **Zaterdag 14 november**: wind valt sterk terug (3,2-10,8 kts), richting draait van N/NNW naar ZO/ZZO (21-145°, wisselend). Golf daalt (0,49-0,97m) maar wind is te zwak → **Slecht**.
- **Zondag 15 november**: wind blijft redelijk (11,4-15,6 kts gem.), maar zeer wisselvallig (gust 21,6-27,5 kts — bijna het dubbele van het gemiddelde), richting draait van pal aflandig naar side-shore (126-191°, veilig). Golf blijft klein (0,42-0,57m) → **Matig**, golf is hier duidelijk de beperkende factor, niet de wind.
- **Maandag 16 november**: wind vergelijkbaar met zondag (11,7-14,9 kts gem., gust 22,2-28,5 kts — opnieuw zeer wisselvallig), richting side-shore (156-187°, veilig). Golf groeit verder naar 0,57-0,86m, dichterbij de drempel maar er nog niet overheen → **grensgeval Matig/Goed, met een expliciete gustiness-waarschuwing**.
- **Dinsdag 17 november — nieuw dit keer, eerste dag met golf boven de drempel**: wind 11,2-15,0 kts gem. (grotendeels onder de 14kts-ondergrens voor Optimaal), gust 19,4-27,6 kts — opnieuw zeer wisselvallig (gust/gem-verhouding tot bijna 1,9), richting licht aflandig/side-shore (147-170°, veilig). Golf is hier voor het eerst in de hele 9-daagse horizon boven de Optimaal-drempel: **1,11-1,16m met een goede periode (6,5-7,4s)**. Netto: **grensgeval Matig/Goed(b)/Optimaal** — de golf is nu optimaal-waardig, maar de wind (anders dan bij vrijdag 13) is hier de beperkende factor, en de gustiness maakt de sessie minder consistent dan vrijdag.

**Beste dag: vrijdag 13 november** blijft de meest complete papieren — stevige, relatief consistente wind (12,6-17,4 kts) uit een vrijwel perfecte side-shore richting, met de hoogste golf van de hele outlook-periode (tot 1,04m, periode 7,8-8,6s). Kans: **gemiddeld**. **Dinsdag 17 november** is een interessant nieuw alternatief (eerste dag met golf écht boven de 1,1m-drempel) maar met te zwakke en te wisselvallige wind om vrijdag te overtreffen — donderdag 12 en maandag 16 november blijven de dichtstbijzijnde andere kanshebbers. ⚠️ Onzeker op 4+ dagen — check dichter bij de tijd opnieuw. Let vooral op of de golfhoogte op donderdag/vrijdag de 1,1m-drempel in latere runs alsnog overschrijdt, en of de wind op dinsdag 17 november in latere runs verder aantrekt richting de 14kts-Optimaal-ondergrens.

---
_Bronnen: Windfinder (GFS) · Soarcast (KNMI Harmonie, IJmond) · windwaarnemingen.nl (KNMI, IJmuiden)_
