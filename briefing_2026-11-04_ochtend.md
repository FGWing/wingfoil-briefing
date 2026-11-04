# 🌊 Wingfoil-briefing Zandvoort–Wijk aan Zee
_04-11-2026 · Ochtendbriefing_

⚠️ **Technische kanttekening:** Windfinder is opgehaald via de Astro-props op de forecast-pagina (`FcTableWindpreviewContainer`/HTML-tabel voor dag 1-2 incl. wind+golf+getij; `ForecastDataInit`-island voor dag 3-10, als JSON embedded in de pagina — in één fetch, geen losse Superforecast-pagina nodig). Soarcast via de onderliggende grafiek-endpoint (`/sc/plotPerLocAndUnitReact.php?json&jsonOnly&unit=m/s&windUnits=kts&location=133&day=...&forecastToShow=harm` voor wind/gust, `unit=deg` voor richting; station IJmond/133, dag vandaag/morgen/overmorgen — inclusief de eigen actuele sensordata voor vandaag t/m 06:00). windwaarnemingen.nl (IJmuiden) via `database/vsp_vdg_wstats.php?st=IJmuiden1` (vandaag, incl. 10-minuten-actuals t/m 06:10) en `database/vsp_mrg_wstats.php?st=IJmuiden2` (morgen + overmorgen t/m 6 nov 15:00, model-horizon bereikt).

**Netto beeld:** **Woensdag (vandaag)** en **donderdag** blijven beide **Matig** — golf is en blijft de beperkende factor (0,2-0,5m, ruim onder de 1,1m-drempel), ook al loopt de wind volgens de Harmonie-bronnen (Soarcast/windwaarnemingen) deels de 14-19kts-band binnen. **Vrijdag** is een lastig geval: Windfinder/GFS ziet nagenoeg windstil (Slecht), maar Soarcast en windwaarnemingen (beide Harmonie) zien 8-14kts — een forse modelafwijking die expliciet wordt vermeld in plaats van gemiddeld. De outlook (dag 4-9) is grotendeels zwak (zaterdag t/m maandag vrijwel windstil), met **dinsdag 10 nov** en vooral **donderdag 12 nov** als de kansrijkste dagen — en een grote waarschuwing: de eerder (03-11) verwachte stevige pal-aanlandige wind op **woensdag 11 nov** is in deze modelrun bijna volledig verdwenen (nu 4,7-9,4 kts in plaats van 17-22 kts), een duidelijk signaal om 4+ dagen vooruit niet te vertrouwen.

---

## ⚡ Snel overzicht
- **Woensdag:** **Matig** (grensgeval met Goed — golf ruim te klein, ondanks wind die bij de Harmonie-bronnen al in de 14-19kts-band komt). Beste venster: **13:00-16:00**.
- **Donderdag:** **Matig** (golf zeer klein en kort — periode slechts 3s, ongeacht welke windschatting je volgt). Beste venster: **10:00-13:00**.
- **Vrijdag:** **Slecht** (GFS) **tot hooguit Matig** (Harmonie-scenario) — golf te klein in beide gevallen; grote modelafwijking op wind.
- **Beste dag in de 7 dagen erna:** donderdag 12 november (golf dichtst bij de 1,1m-drempel van de hele outlook-periode)

---

## ⏰ Realitycheck vandaag
- Laatste actuele uren (04:00-06:10, windwaarnemingen.nl/IJmuiden): **gem. 12,3-15,0 kts**, gust **15,3-18,4 kts**, richting **75,9-87,1°** (ONO/OOST). Soarcast's eigen IJmond-sensor zag over dezelfde periode echter duidelijk méér: **gem. 11,5-18,3 kts**, gust tot **23,8 kts**, richting 57-92° — bij 06:00 bijvoorbeeld 18,3 kts/23,6 kts gust (Soarcast) tegenover 12,3 kts/15,3 kts gust (windwaarnemingen) voor vrijwel hetzelfde moment en dezelfde plek. **Deze twee "actuele" bronnen wijken dit keer zelf sterk van elkaar af** — dat wordt hier expliciet vermeld in plaats van gemiddeld.
- Was voorspeld: windwaarnemingen's eigen Harmonie-vsp zag voor 04:00-06:00 **10,9-11,8 kts / gust 18,4-20,9 kts, 77-80° (ONO/OOST)**; Windfinder/GFS zag voor 04:00-07:00 **12-14 kts / 22-23 kts gust, 70-76° (ONO)**.
- Conclusie: de wind loopt **VOOR** op zowel het GFS- als het eigen Harmonie-model van windwaarnemingen (gemiddeld +1 à +3 kt), en mogelijk nog sterker als Soarcast's eigen sensor representatief is. Rest-van-de-dag inschatting: **classificatie Matig/grensgeval Goed blijft staan, met meer vertrouwen richting de hogere kant van de bandbreedte (Harmonie-niveau, 15-19 kts in de namiddag)** — maar golf (0,4-0,5m) blijft de harde beperking, ongeacht welke windschatting uitkomt.

---

## 📅 Komende 72 uur

### Woensdag — Matig (grensgeval met Goed — golf ruim te klein)
- Windfinder (GFS): 11-14 kts gem. tijdens daglicht, gust 20-24 kts, richting ONO/OOST (72-88°, **licht aflandig → pal aflandig** t.o.v. Zandvoort). Golf blijft vlak 0,4-0,5m, periode 4-6s (≥5s t/m 16:00, zakt daarna naar 4s).
- windwaarnemingen.nl (KNMI-Harmonie, vsp): 10,7-16,3 kts gem. tijdens daglicht, gust 17,1-25,8 kts, richting 71-87° — duidelijk hoger dan Windfinder, vooral in de namiddag (14:00: 16,3 kts/25,8 kts gust).
- Soarcast (KNMI-Harmonie, IJmond): 13,8-19,6 kts gem. tijdens daglicht, gust 19,7-26,6 kts, richting 71-88° — ziet nóg meer wind dan windwaarnemingen, met een duidelijke piek rond 14:00-17:00 (18,7-19,6 kts). **Dit GFS-vs-Harmonie-verschil (net als de voorgaande dagen) wordt expliciet vermeld i.p.v. gemiddeld.**
- Netto: richting is prima (aflandig, veilig en schoon), en bij het Harmonie-scenario (bevestigd door de realitycheck van vanochtend) komt de wind ruim in de 14-25kts-band — maar de golf blijft het hele etmaal op 0,4-0,5m steken, ver onder de 1,1m-drempel → **Matig, grensgeval met Goed** — golf is zonder twijfel de beperkende factor, niet wind of richting.
- Pier-logica: niet van toepassing — richting is aflandig, golf (≤0,5m) ook ruim onder de 0,8m-drempel.
- Getij: laagwater 07:36 (0,5m), hoogwater 11:37 (1,6m), laagwater 19:23 (0,3m).
- Beste venster (daglicht): **13:00-16:00** — wind 13-14 kts (Harmonie-bronnen 17,5-19,6 kts), gust 22-26,6 kts, richting 71-80° (ONO, licht aflandig/pal aflandig-grens), golf 0,5m / 5s (periode hier nog net ≥5s, beste moment van de dag).

### Donderdag — Matig (golf zeer klein en kort)
- Windfinder (GFS): 9-15 kts gem. tijdens daglicht, gust 15-25 kts, richting OOST (82-92°, **pal aflandig**). Golf zeer klein (0,3m) met zeer korte periode (3s, ver onder de 5s-drempel) de hele dag.
- windwaarnemingen.nl (KNMI-Harmonie, vsp): 9,1-13,0 kts gem. tijdens daglicht, gust 16,1-21,0 kts, richting 76-95° — vergelijkbaar met Windfinder, soms zelfs iets lager.
- Soarcast (KNMI-Harmonie, IJmond): 12,3-15,8 kts gem. tijdens daglicht, gust 19,3-21,7 kts, richting 75-95° — ziet wederom iets meer wind dan de andere twee, maar het verschil is kleiner dan op voorgaande dagen.
- Netto: ongeacht welke windschatting je volgt (9-16 kts), de golf blijft het hele etmaal extreem klein en kort (0,3m/3s) → **Matig** — golf is hier zonder twijfel de beperkende factor; ook bij de hogere Soarcast-schatting blijft golf te slecht voor Goed(b) of Optimaal.
- Pier-logica: niet van toepassing — richting is aflandig, niet aanlandig.
- Getij: hoogwater 00:20 (2,0m), laagwater 08:48 (0,4m), hoogwater 12:43 (1,7m), laagwater 20:32 (0,2m).
- Beste venster (daglicht): **10:00-13:00** — wind 11-13 kts (Soarcast tot 15,2-15,8 kts), gust 16-22 kts, richting 90-92° (OOST, pal aflandig), golf 0,3m / 3s.

### Vrijdag — Slecht (GFS) tot hooguit Matig (Harmonie) — grote modelafwijking
- Windfinder (GFS): slechts 1,9-8,3 kts gem. de hele dag, gust 1,9-11,8 kts, richting OOST/ONO (79,5-104°, aflandig maar irrelevant door windkracht). Golf zeer klein (0,12-0,20m), periode 4,7-6,0s.
- windwaarnemingen.nl (KNMI-Harmonie, vsp, t/m 15:00): 8,4-11,1 kts gem., gust 13,2-17,7 kts, richting 75-100° — duidelijk méér wind dan Windfinder/GFS.
- Soarcast (KNMI-Harmonie, IJmond, t/m 15:00): 10,0-14,2 kts gem., gust 14,4-19,5 kts, richting 79-102° — ziet nóg meer wind, met een piek rond 09:00-11:00 (13,6-13,7 kts/18,9-19,1 kts gust). **Dit is een forse afwijking t.o.v. Windfinder/GFS (bijna windstil vs. bruikbare 10-14 kts) en wordt expliciet vermeld i.p.v. gemiddeld.**
- Netto: bij het GFS-scenario is het overduidelijk **Slecht** (gust <16 kts én gem. <14 kts, hele dag). Bij het Harmonie-scenario zou het rond 09:00-11:00 qua wind net in de Matig/grensgeval-Goed(b)-band kunnen komen — maar de golf (0,12-0,20m) is in beide scenario's veruit te klein voor Goed(b) of hoger, dus het plafond blijft **hooguit Matig**, zelfs in het optimistische geval.
- Pier-logica: niet van toepassing — richting is aflandig, golf ruim onder de 0,8m-drempel.
- Getij: hoogwater 01:17 (2,1m), laagwater 09:45 (0,4m), hoogwater 13:35 (1,8m), laagwater 17:43 (1,0m).

---

## 🔭 Kans op mooie sessies daarna (dag 4-9)
Windfinder (GFS, enige bron zo ver vooruit) voor **zaterdag 7 november t/m donderdag 12 november**:

- **Zaterdag 7 november**: wind zwak (2,2-8,0 kts gem., gust 2,2-11,1 kts), richting draait van Z (134°) via ZW naar W (258°) gedurende de dag → **Slecht**.
- **Zondag 8 november**: wind nog steeds zwak (5,6-10,7 kts, gust 8,0-13,4 kts), richting side-shore tot licht aanlandig (187,5-237,2°) tegen het einde van de dag, maar golf blijft klein (0,31-0,37m) → **Slecht**.
- **Maandag 9 november**: wind zwak (5,5-8,6 kts, gust 5,6-11,8 kts), richting side-shore/aflandig (114-175°) → **Slecht**.
- **Dinsdag 10 november**: wind bouwt gedurende de dag op naar 10,9-11,5 kts (avond), gust tot 19,2 kts, richting draait van pal aflandig (ONO/OOST, ~90-96°) overdag naar licht aflandig (67-77°) in de avond, golf groeit naar 0,42-0,50m met een gezonde periode (5,5-6,1s vanaf de namiddag) → **Matig** — beste venster rond 16:00-22:00.
- **Woensdag 11 november**: **grote bijstelling t.o.v. de briefing van gisteren** — destijds nog 17-22 kts WNW/pal aanlandig (Slecht geclassificeerd), nu slechts **4,7-9,4 kts** met wisselende, zwakke richting (46-85°, aflandig-achtig). Golf groeit wel door naar 0,50-0,80m met de beste periode van de hele outlook (6,0-6,9s), maar de wind is te zwak om daar iets mee te doen → **Matig op zijn best, en zeer onzeker** gezien de drastische wijziging t.o.v. gisteren.
- **Donderdag 12 november — beste papieren**: wind blijft bescheiden (4,7-13,4 kts, pieken tot 13,1-13,4 kts rond 04:00/13:00/16:00), gust tot 18,1 kts, richting side-shore (11,6-34,8° 's ochtends/middags, draaiend richting licht aflandig in de avond). Golf bouwt door naar **0,90-0,98m met periode 6,4-7,1s** — de golf komt hier het dichtst van de hele 9-daagse periode bij de 1,1m/Goed(b)-drempel, met een gunstige side-shore-richting. → **Matig, met de meeste kans om bij een iets hogere windschatting naar Goed(b) te kantelen.**

**Beste dag: donderdag 12 november** — de golf is hier veruit het best (0,90-0,98m, vlak onder de Goed(b)-drempel) met een prima richting; als de wind net iets hoger uitvalt dan nu voorspeld (>14 kts) kan dit een echte Goed(b)-dag worden. **Dinsdag 10 november** is het bescheiden maar stabielere alternatief. Kans: **laag tot gemiddeld**, en nadrukkelijk onzeker — zie de forse bijstelling op woensdag 11 nov als waarschuwing.
⚠️ Onzeker op 4+ dagen — check dichter bij de tijd opnieuw. Let vooral op zaterdag 7 t/m maandag 9 november (vrijwel windstil) en op hoe wind en richting rond 10-12 november zich verder ontwikkelen.

---
_Bronnen: Windfinder (GFS) · Soarcast (KNMI Harmonie, IJmond) · windwaarnemingen.nl (KNMI, IJmuiden)_
