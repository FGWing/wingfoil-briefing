# 🌊 Wingfoil-briefing Zandvoort–Wijk aan Zee
_10-11-2026 · Ochtendbriefing_

⚠️ **Technische kanttekening:** Windfinder opgehaald via Playwright + de embedded Astro-JSON (`FcTableWindpreviewContainer` voor wind, `ForecastDataInit` voor wind+golf+getij gecombineerd) op zowel de forecast-pagina (dag 1-10, 3-uurs) als de weatherforecast/Superforecast-pagina (dag 1-3, hourly). **Data-gat:** net als voorgaande dagen levert Windfinder voor vandaag (dinsdag) geen golf-/getijvoorspelling — getij voor vandaag is daarom overgenomen uit de briefing van gisteravond (astronomisch, dus onveranderd). Soarcast via de `plotPerLocAndUnitReact.php`-JSON-endpoints (wind in kts, richting in graden, alleen daglichturen). windwaarnemingen.nl via de `vsp_vdg_wstats.php`/`vsp_mrg_wstats.php`-endpoints (station IJmuiden), met 10-minuten-actuals en de eigen vsp-voorspelling (hourly) voor dezelfde uren. Alle ruwe snelheden in m/s, hier omgerekend naar kts (×1,94384).

**Netto beeld:** **Dinsdag (vandaag)** is overtuigend **Slecht** — alle drie bronnen blijven vrijwel de hele dag diep onder de drempel (Windfinder/GFS max. 9,1kts, Soarcast max. 9,5kts); alleen windwaarnemingen's eigen Harmonie-vsp laat een eenzijdige avondpiek zien (20:00-24:00, gust tot 16,9kts) die niet door Soarcast bevestigd kan worden (geen data na 17:00). **Woensdag** is **Matig**: de twee Harmonie-bronnen (Soarcast, windwaarnemingen) zien structureel meer wind dan Windfinder/GFS, met windwaarnemingen zelfs een forse nachtelijke piek (gust tot 19,6kts), maar de golf (0,18-0,27m) blijft de hele dag te klein voor meer dan Matig. **Donderdag is het grote nieuws van deze run**: alle drie bronnen bevestigen onafhankelijk een forse wind- en golfopbouw vanaf de ochtend (NNW, side-shore, veilig) — wind komt ruim boven de 14kts-Optimaal-drempel (tot 19,5-20,8kts) en de golf schiet vanaf ±13:00 over de 1,1m-drempel (tot 1,53m, periode tot 8,3s). **Donderdag is daarmee overtuigend Optimaal vanaf de vroege/midden-middag** — een forse opwaardering t.o.v. eerdere runs. De outlook (dag 4-9) bevestigt dit beeld: **vrijdag 13 november** heeft de grootste golf van de hele 9-daagse horizon (tot 1,76m) gecombineerd met stevige wind, maar de richting draait overdag naar (licht) aanlandig bij die enorme golf — een veiligheidskanttekening. Vanaf **maandag 16 t/m woensdag 18 november** laat de outlook zeer zware, stormachtige windsnelheden zien (gust tot 50kts) die ondanks een hoog gemiddelde waarschijnlijk te extreem zijn om te wingfoilen.

---

## ⚡ Snel overzicht
- **Dinsdag:** **Slecht** (alle bronnen eens; windwaarnemingen's eigen Harmonie-vsp ziet wel een eenzijdige avondpiek die net over de Matig-grens gaat, niet bevestigd door Soarcast).
- **Woensdag:** **Matig** (Harmonie-bronnen zien meer wind dan GFS, maar golf blijft de hele dag te klein). Beste venster: **07:00-09:00**.
- **Donderdag:** **Optimaal** (alle drie bronnen eens — forse NNW-wind + opbouwende golf boven de drempel, veilige side-shore richting). Beste venster: **13:00 tot (minstens) 22:00**.
- **Beste dag in de 7 dagen erna:** vrijdag 13 november (grootste golf van de hele outlook, tot 1,76m, gecombineerd met stevige wind — maar met een richting/veiligheidskanttekening overdag bij die enorme golf)

---

## ⏰ Realitycheck vandaag
- Laatste actuele uren (04:00-06:10, windwaarnemingen.nl/IJmuiden): **gem. 6,6-7,1 kts**, gust **7,7-8,5 kts**, richting **118-162°** (ZO/ZZO/OZO).
- Was voorspeld: windwaarnemingen's eigen Harmonie-vsp zag voor diezelfde uren (04:00-06:00) slechts **4,1-4,9 kts / gust 6,0-6,6 kts, 148-176°** (ZUID/ZZO); Windfinder/GFS zag voor dezelfde uren nog veel minder: **3,6-4,0 kts / gust 3,6-4,0 kts, 90-121°**.
- Conclusie: de wind loopt **duidelijk VOOR** op zowel windwaarnemingen's eigen Harmonie-vsp (+2 à 2,6kts gem., +1,5 à 2,3kts gust) als — nog veel sterker — op Windfinder/GFS. De richting waait iets oostelijker (meer ZO/OZO) dan voorspeld (meer ZUID/ZZO), maar blijft in beide gevallen veilig aflandig voor Zandvoort. Rest-van-de-dag inschatting: **licht meer vertrouwen** in de hogere kant van de bandbreedte, met name voor de avondpiek die windwaarnemingen's eigen Harmonie-vsp al liet zien (20:00-24:00, gust tot 16,9kts) — die zou gezien de ochtend-overperformance weleens iets hoger kunnen uitvallen dan voorspeld. De classificatie **Slecht blijft voor het grootste deel van de dag staan**; alleen in de late avond is een grensgeval met Matig niet uit te sluiten (eenzijdig signaal, Soarcast heeft geen avonddata om dit te bevestigen).

---

## 📅 Komende 72 uur

### Dinsdag — Slecht
- Windfinder (GFS, hourly): 3,6-9,1 kts gem., gust 3,6-14,9 kts, richting 85-128° (**pal aflandig**, OZO/OOST, zeer veilig).
- Soarcast (KNMI-Harmonie, IJmond, daglicht 07:00-17:00): 3,5-9,5 kts gem., gust 6,1-13,0 kts, richting 83-140° — bevestigt hetzelfde beeld.
- windwaarnemingen.nl (KNMI-Harmonie, vsp, hourly hele dag): 3,7-11,1 kts gem., gust 4,7-16,9 kts, richting 80-174° — ziet een avondpiek **20:00-24:00** (10,1-11,1kts/gust **15,7-16,9kts**) die Windfinder niet laat zien.
- Netto: Windfinder en Soarcast blijven de hele dag ruim onder de Slecht-drempel (gust<16 én gem<14). windwaarnemingen's eigen Harmonie-vsp ziet als enige bron een late-avondpiek die net over de gust-16-grens gaat — een eenzijdig signaal (geen Soarcast-data na 17:00 om te bevestigen), dus met voorbehoud. Richting is de hele dag veilig pal aflandig, dat is hier niet de beperkende factor. **Slecht** staat voor het grootste deel van de dag vast, met alleen in de late avond een mogelijk grensgeval naar Matig.
- Pier-logica: niet van toepassing — richting pal aflandig.
- Getij _(overgenomen uit de briefing van gisteravond — astronomisch, dus onveranderd; Windfinder leverde vandaag geen eigen getijdata)_: hoogwater 04:02 (2,1m), laagwater 11:57 (0,4m), hoogwater 16:14 (2,1m).

### Woensdag — Matig (modelspreiding — Harmonie ziet meer wind dan GFS, golf overal te klein)
- Windfinder (GFS, hourly, Superforecast): 2,5-9,9 kts gem., gust 4,7-17,1 kts, richting 45-83° (**side-shore/licht aflandig**, NO/ONO). Golf 0,18-0,27m, periode 4,0-9,4s (periode prima vanaf de middag, golf de hele dag te klein).
- Soarcast (KNMI-Harmonie, IJmond, daglicht 07:00-17:00): 7,1-11,7 kts gem., gust 10,5-17,3 kts, richting 42-68° — structureel hoger dan Windfinder, met het sterkst in de vroege ochtend.
- windwaarnemingen.nl (KNMI-Harmonie, vsp, hourly): 4,1-12,4 kts gem., gust 7,2-19,6 kts, richting 25-88° — ziet de hoogste piek van alle drie bronnen, vooral 's nachts/vroege ochtend (00:00-04:00: 10,9-12,4kts/gust **16,7-19,6kts**).
- Netto: richting is bij alle bronnen consistent veilig (licht aflandig tot side-shore, NO/ONO). Beide Harmonie-bronnen zien merkbaar meer wind dan Windfinder/GFS — dit wordt expliciet vermeld i.p.v. gemiddeld, met windwaarnemingen als sterkste (deels nachtelijke, moeilijk haalbare) uitschieter. De golf blijft echter de hele dag klein (0,18-0,27m), waardoor het plafond ook bij de Harmonie-kant van de bandbreedte op **Matig** blijft staan.
- Pier-logica: niet van toepassing — golf (0,18-0,27m) ruim onder de 0,8m-drempel.
- Getij: laagwater 00:24 (0,4m), hoogwater 04:39 (2,0m), laagwater 12:38 (0,4m), hoogwater 16:49 (2,2m).
- Beste venster: **07:00-09:00** — Soarcast ziet hier de sterkste daguren (11,4-11,7kts/gust 16,4-17,3kts, 67-68°, ONO); Windfinder blijft duidelijk lager (8,2-8,6kts/gust 10,4-10,8kts). Golf 0,19-0,20m/4,3-4,8s — te klein voor meer dan Matig, ondanks de bruikbare wind bij Soarcast.

### Donderdag — Optimaal (grote opwaardering t.o.v. eerdere runs — alle drie bronnen eens)
- Windfinder (GFS, hourly tot 15:00 + 3-uurs erna): wind bouwt op van ~2-5 kts 's nachts naar **14,0-19,5 kts gem.** vanaf 13:00 (gust tot 22,9kts); richting draait van ZW (213°) 's nachts naar **NNW (328-357°)** vanaf de ochtend — stevig en veilig side-shore. Golf groeit gestaag van 0,28m naar **1,53m** (22:00), periode daalt eerst naar 5,6s rond het middaguur en loopt daarna weer op naar 8,3s in de avond.
- Soarcast (KNMI-Harmonie, IJmond, daglicht 07:00-15:00): bevestigt onafhankelijk hetzelfde beeld, zelfs iets hoger — **15,0-20,8 kts gem., gust 20,1-26,7 kts**, richting 325-349° (NNW).
- windwaarnemingen.nl (KNMI-Harmonie, vsp, hourly tot 15:00): bevestigt het een **derde keer** onafhankelijk — wind trekt al vanaf 06:00 fors aan: **12,8-18,5 kts gem., gust 20,2-26,4 kts**, richting 326-347° (NNW). Alle drie bronnen zijn het hier nagenoeg roerend eens.
- Netto: een stevige, veilige (side-shore/NNW) winddag die vanaf ±13:00 ruim boven de 14kts-Optimaal-ondergrens komt én blijft (14-19,5kts gem., gust tot 22,9-26,7kts), terwijl de golf vanaf diezelfde tijd ook over de 1,1m-Optimaal-drempel gaat met een prima periode (6,0-8,3s). Van ±10:00-13:00 is het nog een grensgeval Goed/Optimaal (golf net onder 1,1m, wind al wel in de band); vanaf ±13:00 is het zonder twijfel **Optimaal**.
- Pier-logica: niet van toepassing — richting side-shore (335-357°), niet aanlandig.
- Getij: laagwater 01:04 (0,4m), hoogwater 05:15 (2,0m), laagwater 13:16 (0,3m), hoogwater 17:24 (2,2m).
- Beste venster: **13:00 tot (minstens) 22:00** — wind 14,0-19,5 kts / gust 20,0-22,9 kts, richting 343-356° (NNW, side-shore, veilig). Golf 1,13-1,53m / periode 6,0-8,3s — ruim boven de Optimaal-drempel en bij het einde van de avond nog groeiend.

---

## 🔭 Kans op mooie sessies daarna (dag 4-9)
Windfinder (GFS, enige bron zo ver vooruit) voor **vrijdag 13 t/m woensdag 18 november**:

- **Vrijdag 13 november**: wind blijft stevig de hele dag (**13,3-19,9 kts gem., gust 15,2-24,4 kts**), richting draait van NNW (340°) 's nachts via NNW/NW (317-333°) geleidelijk richting (licht) aanlandig WNW later op de dag. Golf is enorm voor deze periode — **1,35-1,76m met een uitstekende periode (8,4-9,2s), de grootste golf van de hele 9-daagse outlook**. 's Nachts/vroege ochtend (01:00-04:00, nog side-shore) is dit zuiver **Optimaal**; vanaf ±07:00 draait de richting naar licht aanlandig (en rond 22:00 zelfs bijna pal aanlandig) terwijl de golf enorm blijft — een combinatie die niet goed in de tabel past (Optimaal vereist side-shore/licht aflandig; Goed(a) veronderstelt een kleine golf) en die in de praktijk een waarschuwing verdient voor forse, aanlandige branding. **Pier-logica van toepassing** (richting 280-360°, golf ≥0,8m): **IJmuiden (Zuidpier)** is hier de rustigere/veiligere kant t.o.v. Wijk aan Zee.
- **Zaterdag 14 november**: wind valt sterk terug (**6,5-9,8 kts gem., gust 7,7-12,8 kts**) → **Slecht**. Golf zakt geleidelijk mee (0,60-1,21m), maar wind is hier de beperkende factor.
- **Zondag 15 november**: wind blijft laag-matig (7,9-12,2 kts gem.) maar zeer wisselvallig — gust loopt 's avonds (19:00-22:00) op tot **22,0-24,0 kts**, bijna het dubbele van het gemiddelde. Richting 139-173° (ZO/ZZO, veilig aflandig/side-shore). Golf blijft klein (0,50-0,68m) → **Matig**, met een nadrukkelijke gustiness-waarschuwing in de avond.
- **Maandag 16 november**: wind trekt fors aan (**8,5-23,4 kts gem.**) maar met extreme gustiness (gust **18,5-41,9 kts** — soms bijna het dubbele van het gemiddelde). Richting overwegend side-shore (162-248°, draaiend ZZO→ZW). Golf komt vanaf de vroege middag over de 1,1m-drempel (tot 1,26m, periode 6,6-7,1s). Cijfermatig grotendeels **Optimaal** (wind 18-23kts, golf>1,1m, side-shore), maar de gustwaarden (tot 42kts, windkracht 9) wijzen op stormachtige, zeer onregelmatige omstandigheden die in de praktijk waarschijnlijk te ruw/onveilig zijn — dit nadrukkelijk als waarschuwing vermelden, niet als kans.
- **Dinsdag 17 november**: wind nog verder omhoog (**20,5-29,2 kts gem., gust tot 50,1 kts** — volle stormkracht). Richting wisselend ZZW-ZW-ZO. Golf 1,30-1,61m, periode ~6,7-6,9s. Dit zijn stormforce-windsnelheden (Bft 9-10 in de pieken), ver voorbij wat normaal nog veilig te wingfoilen is; bij WZW/ZW-richting (bv. 16:00, 233°, 28,2kts) geldt bovendien het officiële pierensluiting-signaal van de Reddingsbrigade IJmuiden (windkracht 6+ uit W/ZW/NW). Puur als weerswaarschuwing vermelden, niet als kans.
- **Woensdag 18 november**: wind blijft stormachtig (**21,1-31,4 kts gem., gust 27,7-42,7 kts**), richting WZW/W/ZW (232-269°) — valt bij meerdere uren binnen het Reddingsbrigade-sluitingscriterium (windkracht 6+ uit W/ZW/NW). Golf 1,18-1,32m. Wederom een stormwaarschuwing, geen wingfoil-kans in de praktijk.

**Beste dag: vrijdag 13 november** blijft de beste papieren van de hele outlook — veruit de grootste golf (tot 1,76m) gecombineerd met stevige wind (tot 19,9kts). Let wel goed op de richting die overdag naar (licht) aanlandig draait bij zo'n enorme golf: de vroege ochtend (voor zonsopgang, nog side-shore) is zuiver Optimaal, overdag eerder een grensgeval met een veiligheidskanttekening — IJmuiden (lij van de Zuidpier) is dan relatief rustiger dan Wijk aan Zee of het open strand. Kans: **hoog** qua wind+golf-cijfers, maar met een duidelijk richting/veiligheidsvoorbehoud. ⚠️ Onzeker op 4+ dagen — check dichter bij de tijd opnieuw. Let in latere runs vooral op: (1) of vrijdag 13 november overdag alsnog meer side-shore blijft i.p.v. verder aanlandig draait, en (2) of de zeer zware windsnelheden van maandag 16 t/m woensdag 18 november (gust tot 50kts) in latere runs afzwakken — en check dan ook of de Reddingsbrigade-pieren op die dagen daadwerkelijk gesloten zijn.

---
_Bronnen: Windfinder (GFS) · Soarcast (KNMI Harmonie, IJmond) · windwaarnemingen.nl (KNMI, IJmuiden)_
