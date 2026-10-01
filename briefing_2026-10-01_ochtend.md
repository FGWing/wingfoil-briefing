# 🌊 Wingfoil-briefing Zandvoort–Wijk aan Zee
_01-10-2026 · Ochtendbriefing_

⚠️ **Technische kanttekening deze run:** Soarcast is (net als alle voorgaande runs) niet bereikbaar — een volledige JS-app (React/Vite) zonder vindbaar/bereikbaar API-adres in de uitgeleverde bundle. Windfinder is via de onderliggende paginadata opgehaald (astro-hydration props), inclusief wind + golven + getij per 3 uur t/m 10 oktober in één keer — dus ook de lange-termijn outlook zonder apart bezoek aan de Superforecast-pagina nodig te hebben. windwaarnemingen.nl (IJmuiden) is rechtstreeks via de KNMI-vsp/actuals-JSON-endpoints opgehaald (10-minutenwaarden voor vandaag inclusief lopende modelvoorspelling, plus het uurmodel voor morgen/overmorgen).

---

## ⚡ Snel overzicht
- **Donderdag:** Matig — venster **11:00-14:00** (mogelijk tot 17:00, zie toelichting)
- **Vrijdag:** Slecht
- **Zaterdag:** Slecht
- **Beste dag in de 7 dagen erna:** donderdag 8 oktober

---

## ⏰ Realitycheck vandaag

- Laatste actuele uren (windwaarnemingen.nl, IJmuiden, 05:00-07:10): **wind 8,7-13,2 kts, gust 11,2-15,9 kts, richting draait van 154° (ZZO) via 185° (ZUID) naar 276° (WEST) — met een sprongsgewijze draai in de laatste 10 minuten (07:10)**.
- Was voorspeld voor dezelfde uren: KNMI-vsp (huidige modelrun) gaf **05:00 165° ZZO, 8,5/14,0 kts**; **06:00 204° ZZW, 8,0/12,4 kts**; **07:00 227° ZW, 7,6/12,2 kts**. Windfinder (GFS, 3-uurs resolutie) gaf voor 05h **179° (ZZO), 8,7/15,4 kts** en voor 08h **235°, 7,5/11,8 kts**.
- Conclusie: windkracht **klopt ongeveer** (actuele gusts rond 06:00-07:00 liggen zelfs iets boven KNMI-vsp, consistent met Windfinder), maar de **richting draait sneller door dan beide modellen voorspelden** — om 07:10 al op West (276°) gemeten, terwijl KNMI-vsp voor precies dat uur nog 227° (ZW) gaf en Windfinder pas rond 08:00 richting WZW (235°) bewoog. Voor de rest van de dag: classificatie **ongewijzigd Matig**, maar met **iets meer vertrouwen bijgesteld** richting het KNMI-scenario van een eerder/sterker westelijk middagvenster (zie Donderdag hieronder) — de richtingsdraai en windkracht van vanochtend ondersteunen dat scenario beter dan Windfinders eigen tabel.

---

## 📅 Komende 72 uur

### Donderdag — Matig
- **Windfinder (GFS)**: 02h 10,3/20,5 kts (158°, side-shore, 's nachts), 05h 8,7/15,4 kts (179°, side-shore) — Slecht; 08h 7,5/11,8 kts (235°, side-shore) — Slecht; **11h 10,2/17,3 kts (233°, side-shore) — Matig**; **14h 12,7/16,5 kts (261°, pal aanlandig bij Zandvoort) — Matig**; 17h 10,4/13,4 kts (257°, licht aanlandig) — terug naar Slecht; 20h/23h verder wegvallend (6,2-7,7 kts).
- **KNMI-vsp (windwaarnemingen.nl) ziet de middag duidelijk sterker en langer**: 12:00 9,7/13,6 kts (238°), **13:00 14,2/19,4 kts (270°)**, **14:00 13,4/20,0 kts (274°)**, 15:00 12,6/18,5 kts (272°), **17:00 12,6/18,5 kts (259°, WZW)** — dit rekt het bruikbare venster op tot in elk geval 17:00, met rond 13:00-14:00 een gust-piek die tegen de grens van Goed(b) aan zit (avg bijna 14 kts, gust net onder/rond 19-20 kts).
- **Dit is een merkbare afwijking tussen de modellen** — niet middelen. **Zie Realitycheck**: de actuele richting draait dit moment (07:10) al snel door naar West, sneller dan beide modellen voor dit uur voorspelden, en de windkracht loopt niet achter — dit geeft het KNMI-scenario van een eerder/sterker westelijk middagvenster iets meer geloofwaardigheid dan Windfinders eigen terugval-na-14:00-beeld.
- Golven (Windfinder, enige golfbron): 0,41-0,58 m / 3,9-5,0 s — ruim onder de 1,1 m-drempel de hele dag.
- 🌊 Piervoorkeur: niet van toepassing (golf blijft <0,8 m).
- Getij: laagwater ~02:42 (0,24 m), hoogwater ~07:19 (2,15 m), laagwater ~15:06 (0,42 m), hoogwater ~19:37 (2,2 m).
- Bronnen: Windfinder en KNMI-vsp **wijken merkbaar af** in de middag (Windfinder: terugval na 14:00; KNMI-vsp: aanhoudend venster tot 17:00) — zie toelichting. Soarcast niet bereikbaar (JS-app, geen vindbaar API-adres).

### Vrijdag — Slecht
- Windfinder: hele dag zwak — 4,5-8,0 kts gem / 4,7-9,4 kts gust, richting 188-237° (zuid tot zuidwest) — nergens boven de Matig-drempel.
- KNMI-vsp bevestigt een zwakke dag: 3,3-7,0 kts gem / 4,3-12,4 kts gust — consistent met Windfinder, geen divergentie.
- Golven: 0,19-0,43 m / 3,5-4,3 s.
- 🌊 Piervoorkeur: niet van toepassing.
- Getij: laagwater ~03:20 (0,25 m), hoogwater ~08:03 (2,02 m), laagwater ~15:52 (0,39 m), hoogwater ~20:21 (2,14 m).
- Bronnen: Windfinder en KNMI-vsp **eens** — zwakke dag. Soarcast niet bereikbaar.

### Zaterdag — Slecht
- Windfinder: hele dag zwak — 4,2-6,2 kts gem / 5,0-8,0 kts gust, richting 181-277° (zuid draaiend naar west gedurende de dag) — nergens boven de Matig-drempel; de avondlijke draai naar pal aanlandig (264-277°) heeft bij deze lage kracht geen praktisch effect.
- KNMI-vsp (via de "morgen"-tabel, dekt tot 16:00) bevestigt eenzelfde zwak beeld.
- Golven: 0,16-0,27 m / 3,5-4,5 s.
- 🌊 Piervoorkeur: niet van toepassing.
- Getij: laagwater ~04:05 (0,30 m), hoogwater ~08:55 (1,84 m), laagwater ~16:43 (0,40 m), hoogwater ~21:14 (2,0 m).
- Bronnen: Windfinder en KNMI-vsp **eens** — zwakke dag. Soarcast niet bereikbaar.

---

## 🔭 Kans op mooie sessies daarna (dag 4-9)
Windfinder (GFS, enige bron zo ver vooruit) laat voor **zondag 4 t/m vrijdag 9 oktober** het volgende beeld zien:
- **Zondag 4 oktober**: zwak de hele dag, nergens boven 9,8 kts gemiddeld — Slecht.
- **Maandag 5 oktober**: bouwt overdag op naar Matig — 11h-14h 12,0-12,3/16,3 kts (241-245°, side-shore/licht aanlandig bij Zandvoort) — daarna 's avonds weer terugval naar Slecht.
- **Dinsdag 6 oktober**: Slecht, hele dag zwak-matig (5,9-9,2 kts gem), golf loopt op naar 0,57-0,66 m maar wind blijft te zwak om dat te benutten.
- **Woensdag 7 oktober**: overwegend Slecht overdag, maar bouwt 's avonds snel op — 23:00 al 17,0/18,1 kts (334°, side-shore bij Zandvoort), grensgeval Optimaal/Goed. Golf loopt op naar 1,08 m / 6,0 s en passeert de 0,8 m-pierdrempel rond het begin van de avond, terwijl de wind dan nog overwegend pal aanlandig is bij Zandvoort (288-317°, NW) maar bij **IJmuiden dankzij de eigen pierzone-hoek (150°/330°) al side-shore** is. 🌊 **Piervoorkeur: IJmuiden rustiger** vanaf ~17:00-23:00 (wind uit 280-335° → Zuidpier breekt de golfslag).
- **Donderdag 8 oktober — beste dag, breed en stevig venster**: 05h 15,3/16,9 kts (326°) grensgeval, **08h 18,9/21,0 kts (323°) al Optimaal bij IJmuiden** (side-shore dankzij pierzone-hoek)/grensgeval bij Zandvoort, en vanaf **11h t/m 20h Optimaal bij Zandvoort**: 11h 18,2/21,0 kts (333°, side-shore), 14h 17,0/19,9 kts (329°), 17h 16,6/19,7 kts (341°), 20h 18,6/21,3 kts (334°) — golf 1,18-1,35 m / 6,5-7,1 s, ruim boven de Optimaal-drempel (>1,1 m én periode ≥5 s). Richting blijft overwegend side-shore bij Zandvoort, dus geen pier-overweging nodig daar; bij IJmuiden eveneens side-shore de hele dag. 23h zakt terug naar Goed(b) (13,7/17,0 kts).
- **Vrijdag 9 oktober**: wind blijft stevig tot sterk en bouwt verder op (10,4 → 21,1 kts gem gedurende de dag, gust tot 28 kts 's middags/avonds — pittig), maar de richting draait naar West/ZW (220-266°), wat bij Zandvoort overdag pal aanlandig wordt (grensgeval Optimaal/Goed, maar minder comfortabel dan donderdag door de hogere gust-pieken en minder gunstige hoek). Golf 0,90-1,26 m. 🌊 **Piervoorkeur: Wijk aan Zee rustiger** (wind 214-250° valt in de zuid(west)-band waar de Noordpier de golfslag breekt), met name van 11:00 tot 23:00.

**Beste dag: donderdag 8 oktober**, met name het venster **11:00-20:00** — breed en overwegend Optimaal bij Zandvoort, en zelfs al vanaf 05:00-08:00 Optimaal bij IJmuiden dankzij de pierzone-hoek. Kans: **gemiddeld tot hoog** (het signaal is deze run consistent over meerdere opeenvolgende 3-uurs-stappen en bij zowel Zandvoort als IJmuiden — een duidelijk breder en rustiger venster dan de smalle piek-vóór-storm die in eerdere runs voor deze periode naar voren kwam). **Vrijdag 9 oktober is een stevig maar guster alternatief**, met als extra aandachtspunt de Wijk aan Zee-piervoorkeur.
⚠️ Onzeker op 4+ dagen — check dichter bij de tijd opnieuw, met name de exacte timing en intensiteit rond donderdag 8 / vrijdag 9 oktober.

---
_Bronnen: Windfinder (GFS) · windwaarnemingen.nl (KNMI, IJmuiden) · Soarcast — deze run niet bereikbaar (JS-app, geen vindbaar/bereikbaar API-adres)_
