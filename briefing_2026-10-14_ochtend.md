# 🌊 Wingfoil-briefing Zandvoort–Wijk aan Zee
_14-10-2026 · Ochtendbriefing_

⚠️ **Technische kanttekening:** Soarcast blijft onbereikbaar deze run (pure JS/Vite-app, `/web/locationinfo?...` levert alleen een lege HTML-shell zonder onderliggende data — zelfde conclusie als alle voorgaande runs). Windfinder is opgehaald via de onderliggende Astro-island props op de reguliere forecast-pagina: deze bevatten per dag volledige data (wind, golven, getij) en dekken dag 1 t/m 10 (14-23 oktober) in 3-uurs stappen, dus geen aparte Superforecast-pagina nodig. windwaarnemingen.nl (IJmuiden) is opgehaald via `database/vsp_vdg_wstats.php?st=IJmuiden1` (vandaag: 10-minuten-actuals + ingebed KNMI-uurmodel) en `vsp_mrg_wstats.php?st=IJmuiden2` (morgen + overmorgen t/m 16:00). **Opvallend deze run:** voor donderdag wijken Windfinder (GFS) en windwaarnemingen.nl (KNMI) weer fors af in windkracht (GFS 11,5-15,1 kts vs KNMI maar 4,7-7,9 kts voor dezelfde uren) terwijl de richting tussen beide wel overeenkomt — zie Realitycheck voor hoe dit is meegenomen.

---

## ⚡ Snel overzicht
- **Woensdag:** Slecht — de hele dag te weinig wind, bevestigd door de Realitycheck (geen bruikbaar venster).
- **Donderdag:** Grensgeval Goed/Optimaal volgens Windfinder (±11:00-17:00, piek 14:00, ~15 kts side-shore), maar KNMI voorspelt voor dezelfde uren maar ~5-8 kts (Matig-niveau) — zie Realitycheck voor welke kant waarschijnlijker is.
- **Vrijdag:** Slecht het grootste deel van de dag; vanaf 20:00 bouwt een noordelijke wind op naar Optimaal om 23:00 (16,3 kts, golf 1,16m) — alleen door Windfinder gezien, KNMI dekt dit venster niet (data stopt om 16:00).
- **Beste dag in de 7 dagen erna:** zaterdag 17 oktober
_(De eerste 3 regels zijn altijd de eerstvolgende 3 volle dagen vanaf het moment van versturen.)_

---

## ⏰ Realitycheck vandaag

- Laatste actuele uren (windwaarnemingen.nl, IJmuiden, 06:00-07:10): **wind 5,9-7,3 kts, gust 7,6-8,9 kts, richting 293-310° (WNW/NW)**.
- Was voorspeld voor dezelfde uren: het **ingebedde KNMI-uurmodel** gaf voor 06h/07h **298-308°, 6,0-6,4 kts, gust 8,8-10,1 kts** — nagenoeg gelijk aan de actuals (zelfs licht zwakker dan gemeten). **Windfinder/GFS** gaf voor de dichtstbijzijnde 3-uurspunten (05h/08h) **303-309°, 7,0-12,0 kts, gust 9,2-15,9 kts** — met name het 05h-punt (12,0 kts) ruim boven wat er daadwerkelijk stond.
- Conclusie: de wind loopt **ACHTER op Windfinder/GFS** (vooral de vroege ochtend), maar **klopt vrijwel exact met windwaarnemingen.nl/KNMI**. Richting komt bij beide modellen overeen (WNW/NW). Rest-van-de-dag inschatting: **bevestigd/licht naar beneden bijgesteld** — vandaag was het Windfinder-venster toch al zwak (piek ~10-11 kts rond 14:00-17:00), dus blijft **Slecht**. Belangrijker: dit bevestigt opnieuw het patroon dat GFS deze week systematisch te sterk voorspelt, wat het vertrouwen in **donderdags** Windfinder-venster (11,5-15,1 kts) verder verlaagt nu KNMI daar slechts 4,7-7,9 kts voor voorspelt — zie de dagsectie hieronder.

---

## 📅 Komende 72 uur

### Woensdag — Slecht
- De hele dag (vanaf nu) te weinig wind: 6,6-11,3 kts (gust tot 17,8 kts) bij side-shore tot licht/pal aanlandige richting (211-241°) tot aan de vroege avond. Enige uitzondering is een marginaal moment om 23:00 (10,1 kts, side-shore 185°) → **grensgeval Matig**, maar dat ligt buiten een praktisch sessievenster.
- Golven (Windfinder): 0,76-1,29m / 5,1-6,8s — ruim voldoende hoogte/periode, maar de wind ontbreekt.
- Getij: laagwater 02:31 (0,30 m), hoogwater 06:34 (2,05 m), laagwater 14:47 (0,38 m), hoogwater 18:47 (2,17 m).
- Bronnen: windwaarnemingen.nl/KNMI bevestigt vanochtend al dat Windfinder/GFS te sterk zit (zie Realitycheck); voor de rest van de dag is GFS's eigen voorspelling al zwak, dus het beeld "Slecht" staat vast. Soarcast niet bereikbaar.

### Donderdag — Grensgeval Goed/Optimaal (Windfinder) / Matig (KNMI) — zie toelichting
- Bij **Zandvoort/Wijk aan Zee**: de hele dag is de richting **side-shore** (197-213°, zuid/ZZW) bij geleidelijk oplopende wind (11,5→15,1 kts, gust 20,7-23,0 kts — fors gustig) en golf net onder de 1,1m-drempel (0,78-0,89m, periode 5,2-5,6s, periode zelf wel voldoende). Dit past bij geen van de tabelrijen exact (wind+richting zitten in de Optimaal-band vanaf ~14:00, de golf ontbreekt net) → **grensgeval Goed/Optimaal**, beste moment rond **14:00** (15,1 kts, golf 0,89m). Vanaf 20:00 valt de wind terug (9,1-10,0 kts) → **Matig**.
- Bij **IJmuiden** (pierzone-hoek): vanaf ±05:00 leest de richting hier als **licht aanlandig** (197-203°) tot **pal aanlandig** (14:00-17:00, 211-213°) — minder gunstig dan Zandvoorts side-shore.
- 🌊 Piervoorkeur: **05:00-17:00** is de richting bij IJmuiden (licht/pal) aanlandig met golf ≥0,8m (vanaf 08:00) → **Wijk aan Zee (Noordpier)** is de rustiger keuze, al blijft het effect met golf net rond 0,85-0,89m mild.
- Golven (Windfinder, enige golfbron): 0,68-0,89m / 5,2-5,6s.
- Getij: laagwater 03:08 (0,34 m), hoogwater 07:08 (1,97 m), laagwater 15:21 (0,36 m), hoogwater 19:21 (2,13 m).
- Bronnen: Windfinder (GFS) en windwaarnemingen.nl (KNMI) zijn het **eens over de richting** (zuid/ZZW) maar wijken **extreem sterk af in windkracht** — GFS 11,5-15,1 kts tegenover KNMI maar 4,7-7,9 kts, een verschil van bijna een factor 2. Gezien de Realitycheck van vanochtend (actuals volgen KNMI, niet GFS) is het **aannemelijker dat donderdag dichter bij Matig uitkomt dan bij het Windfinder-geschetste grensgeval Optimaal** — behandel dit venster met nadruk als onzeker en check dicht bij de tijd opnieuw. Soarcast niet bereikbaar.

### Vrijdag — Slecht (grootste deel van de dag), bouwend naar Optimaal vanaf de avond
- Bij **Zandvoort/Wijk aan Zee**: **02:00-14:00** is de wind te zwak (7,4-8,9 kts, gust tot 16,1 kts) bij side-shore richting (186-230°, zuid/ZW) → **Slecht**. Vanaf **17:00** draait de richting abrupt naar **noord** (3°, nog steeds side-shore qua classificatie) bij een sprong naar **20,8 kts** (gust 25,4 kts), maar golf/periode (0,89m/4,7s) hebben de omdraai nog niet bijgebeend → **grensgeval Goed/Optimaal**. Om **20:00**: 357°, 14,4 kts, golf 1,05m/5,2s → **Matig** (golf net onder drempel). Om **23:00**: 340°, 16,3 kts, golf 1,16m/5,7s → **Optimaal** — en dit zet door tot in zaterdag (zie outlook).
- Bij **IJmuiden/Wijk aan Zee** (pierzone-hoek): de noordelijke richting vanaf 17:00 valt bij beide pierzones niet in de aanlandige hoek (side-shore/aflandig voor hun eigen assen) → geen piervoordeel van toepassing deze avond.
- Golven (Windfinder): 0,57-1,16m / 4,4-5,7s — laag overdag, fors oplopend in de avond.
- Getij: laagwater 03:29 (0,39 m), hoogwater 07:40 (1,90 m), laagwater 15:46 (0,36 m), hoogwater 19:54 (2,07 m).
- Bronnen: windwaarnemingen.nl/KNMI dekt deze dag alleen tot 16:00 en laat tot dan een veel rustiger beeld zien (geleidelijke veer zuid→ZW→WZW→NW, 7,2-9,3 kts) zonder de avondsprong — **de krachtige avond-/nachtwind vanaf 17:00 is dus alleen door Windfinder gezien en niet kruisgevalideerd**. Check dit venster dicht bij de tijd opnieuw. Soarcast niet bereikbaar.

---

## 🔭 Kans op mooie sessies daarna (dag 4-9)
Windfinder (GFS, enige bron zo ver vooruit, 3-uurs resolutie) voor **zaterdag 17 t/m donderdag 22 oktober**:

- **Zaterdag 17 oktober — beste dag**: de Optimaal-periode die vrijdagavond begint loopt vrijwel ononderbroken door tot de late middag. **02:00-17:00**: richting noord/NNO (358-24°, side-shore), wind **16,1-18,7 kts** (gust 18,8-23,8 kts), golf **1,19-1,42m / 5,8-7,0s** → **Optimaal**, zes opeenvolgende meetpunten lang (~15 uur). Vanaf **20:00** zwakt de wind af (11,9 kts, golf nog 1,31m) → **Goed (b)**, om **23:00** verder naar een grensgeval Matig/Goed (b) bij afnemende wind (11,5 kts) maar oplopende gust (20,5 kts).
- **Zondag 18 oktober**: ochtend nog redelijk — **02:00**: NO (46°, side-shore), 10,9 kts, golf 1,14m/7,6s → **Goed (b)**. Daarna geleidelijk verzwakkend (golf en wind beide afnemend) via **Matig** (08:00-11:00, 11,2-12,2 kts, golf 0,84-0,92m) naar **Slecht** vanaf 14:00 (7,7-11,9 kts, golf <0,8m).
- **Maandag 19 oktober**: grootste deel van de dag te zwak (6,6-12,1 kts) → **Slecht**. Vanaf **17:00** draait de richting naar licht/pal aflandig (63-87°, ONO/O) bij oplopende wind (13,8-15,5 kts) en zeer pittige gust (tot 29,1 kts) maar weinig golf (0,63-0,65m, vlak water door de aflandige hoek) → **grensgeval Goed** (sterke, vlakke, maar puffige aflandige wind).
- **Dinsdag 20 oktober**: de hele dag **pal aflandig** (80-91°, OZO/O) met stevige wind (14,4-16,6 kts) maar zeer extreme gust (21,4-29,6 kts, bijna het dubbele van het gemiddelde — puffig/buiig) en vlak water (golf 0,46-0,58m) → **grensgeval Goed**, met nadruk op de gustiness en de volledig aflandige hoek (lastiger terugkomen bij een gat in de wind).
- **Woensdag 21 oktober**: vergelijkbaar maar zwakker — pal aflandig (88-99°), wind 12,4-14,7 kts, gust nog steeds pittig (18,4-27,0 kts), golf laag (0,34-0,40m) → **Matig/grensgeval Goed**.
- **Donderdag 22 oktober**: verder verzwakkend, pal aflandig (92-112°). **Matig** in de ochtend (08:00-11:00, 10,0-10,9 kts) → **Slecht** vanaf de middag (5,9-7,8 kts).

**Beste dag: zaterdag 17 oktober**, met een lange, vrijwel ononderbroken Optimaal-periode van ~15 uur (noordelijke/NNO side-shore wind 16-19 kts, golf 1,2-1,4m/6-7s) die al vrijdagavond begint. Kans: **gemiddeld tot hoog** — dit is dezelfde periode die ook in eerdere briefings al als beste venster naar voren kwam (consistent signaal over meerdere modelruns heen). Dinsdag 20 oktober is een interessant alternatief voor wie van pittige, vlakke aflandige sessies houdt, maar de zeer hoge gust-factor en volledig aflandige hoek vragen om voorzichtigheid.
⚠️ Onzeker op 4+ dagen — check dichter bij de tijd opnieuw.

---
_Bronnen: Windfinder (GFS) · windwaarnemingen.nl (KNMI, IJmuiden) · Soarcast — deze run niet bereikbaar (JS-app, geen vindbaar/bereikbaar API-adres)_
