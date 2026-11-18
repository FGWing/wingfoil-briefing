# 🌊 Wingfoil-briefing Zandvoort–Wijk aan Zee
_18-11-2026 · Ochtendbriefing_

⚠️ **Technische kanttekening:** alle drie bronnen zijn deze run rechtstreeks via curl (geen browser) opgehaald. Windfinder: de embedded Astro-JSON (`FcTableWindpreviewContainer`/`ForecastSection`/`ForecastDataInit`) gedecodeerd — `ForecastSection` vult vandaag+morgen volledig (incl. golf/getij), `ForecastDataInit` vult dag 3 t/m 10. Soarcast: de pagina zelf is een lege JS-app, maar het onderliggende endpoint (`/sc/plotPerLocAndUnitReact.php?location=133&day=...&unit=m/s&forecastToShow=harmonie&json`) werkte deze run wél (in tegenstelling tot gisteren) en gaf uurlijkse wind/gust/richting voor vandaag t/m overmorgen. windwaarnemingen.nl via `database/vsp_vdg_wstats.php?st=IJmuiden1` (vandaag, 10-min-actuals + eigen uurlijkse Harmonie-vsp) en `vsp_mrg_wstats.php?st=IJmuiden2` (morgen+overmorgen).

**Netto beeld — grote, ongebruikelijke modelverdeeldheid vandaag die zich NIET in het voordeel van de storm heeft opgelost.** Windfinder (GFS) en Soarcast (Harmonie, IJmond) voorspelden voor vannacht/vanochtend een forse WZW-storm (27-31kts gem., gust tot 40-41kts). De realitycheck bij het IJmuiden-station laat echter zien dat de wind daar tot nu toe keurig de veel lagere eigen Harmonie-vsp van windwaarnemingen volgt (12-14kts gem., gust 17-20kts) — exact de helft van wat GFS/Soarcast beweerden. Voor de rest van vandaag volgen we daarom de bevestigde, lagere cijfers: na een kort **Goed(b)-grensgeval bij IJmuiden rond 07:00-08:00** (zwakke maar bruikbare wind, side-shore dankzij de pierzone-hoek, golf nog ruim boven de drempel dankzij de nog aanwezige deining) wordt de wind te zwak (gust<16, gem<14) en is de rest van de dag **Slecht** — in schril contrast met de storm die Windfinder/Soarcast voor vandaag lieten zien. **Donderdag** kent een vergelijkbare, nog onopgeloste modelverdeeldheid rond het middag-venster (Soarcast 18-20kts vs. windwaarnemingen 8kts) — gezien de uitkomst van vandaag is voorzichtigheid met de hogere cijfers op zijn plaats. **Vrijdag** is bij alle drie bronnen een zwakke, aflandige dag zonder bruikbaar venster. In de outlook springt **dinsdag 24 november** er het meest uit (zijdewind 19-21kts, golf net onder de drempel).

---

## ⚡ Snel overzicht
- **Woensdag:** **Risico/Slecht** het grootste deel van de dag (voorspelde GFS/Soarcast-storm bleek vanochtend niet te kloppen) — kort **Goed(b)-grensgeval bij IJmuiden ±07:00-08:00**.
- **Donderdag:** **Matig**, met een onopgeloste grote modelverdeeldheid rond **13:00-14:00** (Soarcast ziet daar 18-20kts/zijdewind, windwaarnemingen maar 8kts) — check dichter bij de tijd.
- **Vrijdag:** **Slecht-tot-Matig** — wind te zwak bij alle drie bronnen, bovendien aflandige richting.
- **Beste dag in de 7 dagen erna:** dinsdag 24 november — Goed-grensgeval, golf net onder de drempel.

---

## ⏰ Realitycheck vandaag
- Laatste actuele uren (04:00-06:10, windwaarnemingen.nl/IJmuiden, 10-min metingen): **gem. ≈13,7-14,2 kts** (04:00: 13,71 → 05:00: 14,14 → 06:00: 14,23 → 06:10: 14,06), gust **≈16,8-19,6 kts**, richting **≈254-267°** (WZW/WEST).
- Was voorspeld: windwaarnemingen's eigen Harmonie-vsp zag voor dezelfde uren **12,7-14,3 kts gem., gust 18,6-20,4 kts, richting 253-265°** (WZW/WEST) — vrijwel exacte match. Windfinder (GFS) en Soarcast (Harmonie, IJmond) zagen voor diezelfde uren echter een veel zwaardere storm: **27-30 kts gem., gust 35-41 kts**, richting 250-262° — ruim het dubbele van wat er werkelijk staat.
- Conclusie: de wind **KLOPT vrijwel exact** met windwaarnemingen's eigen (lagere) Harmonie-voorspelling voor het IJmuiden-station, maar loopt **FORS ACHTER** op de veel hogere stormvoorspelling van Windfinder/GFS en Soarcast/IJmond — richting komt bij alle drie overeen, alleen de windkracht wijkt massaal af. Rest-van-de-dag inschatting: **naar beneden bijgesteld** — voor de rest van vandaag volgen we de bevestigde, lagere windwaarnemingen-cijfers in plaats van de (tot nu toe onterechte) Windfinder/Soarcast-storm. Dat betekent een veel rustigere, en na de ochtend ook een te zwakke dag, in plaats van de stormachtige dag die GFS/Soarcast lieten zien.

---

## 📅 Komende 72 uur

### Woensdag — Risico/Slecht grootste deel van de dag, kort Goed(b)-grensgeval ±07:00-08:00 bij IJmuiden
- Windfinder (GFS, 3-uurs): voorspelt een WZW-storm 's nachts/vroege ochtend (23-27kts gem., gust tot 35kts, richting 250-257°), afbouwend door de ochtend naar 15-18kts (10:00-13:00, richting draait WNW 282-298°) en verder naar bijna windstil in de avond (3-6kts, 19:00-22:00). Golf blijft hoog en neemt de hele dag langzaam af: **1,6-2,1m**, periode 6,4-7,3s.
- Soarcast (Harmonie, IJmond, uurlijks — deze run wél beschikbaar): bevestigt dezelfde stormpiek qua schaal (23-31kts gem. 00:00-06:00, gust tot 40,6kts, richting 239-266°), afbouwend via 17-22kts (14:00-16:00) naar 4-10kts in de avond (20:00-23:00, richting draait via west/zuid naar 134-168°).
- windwaarnemingen.nl (eigen Harmonie-vsp + actuals, IJmuiden): ziet een veel kalmer beeld — vsp 11-15kts gem., gust 15,5-20,4kts de hele nacht/ochtend (richting 237-296°, vergelijkbaar qua draai), aflopend naar 2-5kts vanaf 17:00. **De actuals (zie Realitycheck) bevestigen deze lagere lijn vrijwel exact, niet de hogere Windfinder/Soarcast-storm.**
- Netto — grote, ongebruikelijke modelverdeeldheid (2x in windkracht) die vanochtend in het voordeel van de LAGERE cijfers is beslecht. Op basis daarvan: de nacht/vroege ochtend (voorbij) was met golf 1,9-2,1m en aanlandige richting feitelijk te ruw zonder piervoordeel; rond **07:00-08:00** draait de richting bij IJmuiden's pierzone-hoek naar licht aanlandig/side-shore (282-291°) terwijl de wind nog net voldoende is (11-12kts, gust 16-17,5kts) en de golf nog ruim boven de drempel staat (≈1,9m/7,1s) — een kort Goed(b)-grensgeval. Vanaf ±09:00 zakt de wind onder gust 16kts/gem 14kts (de Slecht-drempel) en blijft daar de rest van de dag, ook al staat er nog golf.
- Pier-logica: tussen ±07:00-16:00 is de richting (282-298°) bij **Wijk aan Zee** (eigen hoek, pal aanlandig 283,8°) juist **pal aanlandig zonder bescherming** (valt in de 280-360°-band die normaliter juist IJmuiden beschermt, niet Wijk aan Zee) — bij **IJmuiden** (pierzone-hoek, pal aanlandig 240°) is diezelfde richting **licht aanlandig/side-shore**, én profiteert van de Zuidpier. IJmuiden is dus duidelijk de voorkeursplek in dit venster, Wijk aan Zee vermijden.
- Getij: laagwater 05:03 (0,55m), hoogwater 09:31 (1,55m), laagwater 17:23 (0,36m), hoogwater 22:28 (1,8m) — bij vloed (vanaf ±13:00 oplopend naar 22:28) is de shorebreak zwaarder, ook aan de beschutte kant.
- Beste venster: **±07:00-08:00 bij IJmuiden** — wind 11-12 kts, gust 16-17,5 kts, richting 282-291° (licht aanlandig/side-shore bij IJmuiden's eigen hoek, Zuidpier-bescherming). Golf ≈1,9m/7,1s — ruim boven de drempel, maar de wind is mager; check de actuele gust vlak voor vertrek. Verder géén bruikbaar venster vandaag.

### Donderdag — Matig, grote modelverdeeldheid rond 13:00-14:00
- Windfinder (GFS, 3-uurs): zwakke, draaiende wind 's nachts/ochtend (11-13kts, richting van ZW via zuid naar pal aflandig 118-160°), bouwt op naar **20,0kts gem./27,5kts gust om 13:00** (richting 232,6°, side-shore/richting-SSW), zakt daarna weer naar 9-14kts met richting draaiend naar NNO (12-29°) in de avond. Golf blijft de hele dag onder de drempel: **0,75-1,1m**, periode 5,7-6,3s (rond 13:00 nog maar 0,86m).
- Soarcast (Harmonie, IJmond, uurlijks): ziet een forsere middagpiek dan Windfinder — **18,5-20,2kts gem., gust 22,9-28,2kts rond 01:00-02:00 en opnieuw 13:00-14:00** (richting 194-220°), en een tweede opleving 's avonds (15,6-16,1kts, 17:00-19:00, richting draait naar NNO 25-42°).
- windwaarnemingen.nl (eigen Harmonie-vsp, IJmuiden): ziet een veel zwakkere dag door — slechts **3-9kts gem.** vrijwel de hele dag, met een bescheiden piekje van 8,1kts/11,3kts gust om 13:00 (richting 208°, vergelijkbaar qua draai naar ZZW) en 6-6,9kts in de avond (richting NNO/NO).
- Netto — **opnieuw dezelfde modelverdeeldheid als vandaag, nog onopgelost.** Rond 13:00-14:00 zien Windfinder en Soarcast een bruikbaar venster (18-20kts, richting side-shore/ZZW, golf net onder de drempel — zou een Goed-grensgeval zijn), maar windwaarnemingen's eigen Harmonie-vsp ziet daar slechts ~8kts. Gezien de realitycheck van vandaag, waarin de lagere windwaarnemingen-lijn het gelijk kreeg, is terughoudendheid met de hogere cijfers verstandig — maar dit is nog geen garantie dat het morgen weer zo uitpakt. Classificatie voorlopig: **Matig**, met kans op opwaardering naar Goed als de hogere cijfers toch kloppen.
- Pier-logica: rond 13:00 is de richting (208-232°) bij **IJmuiden** (pierzone-hoek, pal aanlandig 240°) grensgeval pal aanlandig zónder Zuidpier-bescherming (valt in de 170-250°-band die juist Wijk aan Zee beschermt); bij **Wijk aan Zee** (eigen hoek) is diezelfde richting juist side-shore. Mocht het venster doorzetten, dan is Wijk aan Zee de voorkeursplek. Golf (0,85-0,86m) ligt rond de 0,8m-ondergrens voor piervermelding, dus marginaal relevant.
- Getij: laagwater 06:12 (0,56m), hoogwater 10:47 (1,53m), laagwater 18:35 (0,38m), avond oplopend naar hoogwater (1,52m+ om 22:00, exacte tijd niet in de data).
- Beste venster: **onzeker — 13:00-14:00 bij Wijk aan Zee** als de Soarcast/Windfinder-cijfers kloppen (wind 18-20kts, gust 23-28kts, richting 194-232° side-shore, golf 0,85-0,86m net onder de drempel); als windwaarnemingen gelijk krijgt (zoals vandaag) is de dag te zwak voor een goede sessie. Check dichter bij de tijd welke lijn het wint.

### Vrijdag — Slecht-tot-Matig, wind te zwak
- Windfinder (GFS, 3-uurs): wind zwak de hele dag (**3,4-9,2 kts gem.**, gust 5,4-15,1kts), richting pal aflandig/side-shore (46-108°). Golf laag: **0,52-0,67m**, periode 5,5-6,5s.
- Soarcast (Harmonie, IJmond): iets hoger maar nog steeds zwak (**7,0-12,1 kts gem.**, gust 11,3-16,7kts), richting vergelijkbaar aflandig/side-shore (68-133°).
- windwaarnemingen.nl (eigen Harmonie-vsp, IJmuiden): laagste van de drie (**2,5-5,0 kts gem.**, gust 4,6-8,0kts), richting ONO/OZO (67-133°), data beschikbaar t/m 15:00.
- Netto — **alle drie bronnen eens: te weinig wind voor een goede sessie**, en de golf blijft ruim onder de drempel (max 0,67m). Richting is bovendien pal- tot licht aflandig bij Zandvoort/Wijk aan Zee — extra voorzichtigheid geboden voor wie er met te weinig materiaal toch het water op gaat (wegwaaien van de kust). Classificatie: **Matig in het gunstigste geval (Soarcast), Slecht volgens windwaarnemingen.**
- Pier-logica: niet van toepassing (richting is aflandig, geen aanlandige component bij IJmuiden of Wijk aan Zee).
- Getij: hoogwater 23:35 (nacht ervoor, 1,88m), laagwater 07:40 (0,51m), hoogwater 11:59 (1,61m), laagwater 19:49 (0,33m).
- Beste venster: **geen bruikbaar venster.** Wind blijft bij alle bronnen te zwak voor een volwaardige sessie.

---

## 🔭 Kans op mooie sessies daarna (dag 4-9)
Windfinder (GFS, enige bron zo ver vooruit) voor **zaterdag 21 t/m donderdag 26 november**.

- **Zaterdag 21 november**: wind zwak (**4,0-10,6 kts gem.**, gust 5,9-13,4kts), richting NNW/N draaiend (322-358°), bij Zandvoort grotendeels licht aanlandig tot side-shore. Golf **0,67-0,80m**, net onder de drempel. Matig — geen uitschieter.
- **Zondag 22 november**: wind zeer zwak overdag (**2,5-4,4 kts**), bouwt licht op richting de avond (8,5-10,3kts, 16:00-19:00, richting N 18-26°, side-shore). Golf laag (0,57-0,63m). Slecht-tot-Matig.
- **Maandag 23 november**: wind bouwt op naar **12,5-14,4 kts gem.** rond 04:00-07:00 (gust 16,3-17,8kts), richting licht aanlandig/N (319-334°). Golf **0,65-0,73m**, net onder de drempel. Goed(a)-grensgeval in de vroege ochtend (wind net onder/op de 14kts-grens).
- **Dinsdag 24 november** (dag 7): wind de sterkste van de outlook-periode, oplopend naar **19,0-21,3 kts gem.** rond 10:00-13:00 (gust tot 30-34,5kts!), richting side-shore (154-157°, ZZO). Golf **0,85-0,86m** — net onder de 1,1m-drempel, verder zou dit een schone Optimaal-dag zijn. Goed-grensgeval, beste van de periode.
- **Woensdag 25 november** (dag 8): wisselvallige dag, wind 9,3-23,6kts met richting die alle kanten op draait (159-289°). Golf loopt op naar **0,89-1,04m** (net onder drempel). Rond 16:00 wordt de richting (289°) pal aanlandig bij Zandvoort/Wijk aan Zee zonder duidelijk piervoordeel — wissel tussen Matig en Risico, geen schoon venster.
- **Donderdag 26 november** (dag 9): forse wind rond 10:00-13:00 (**19,2-23,1 kts gem.**, gust 24-29,4kts) en opnieuw 's avonds (23,9kts/28,8kts om 22:00), maar richting (263-284°) is dan pal aanlandig bij zowel Zandvoort/Wijk aan Zee als IJmuiden's pierzone-hoek, en valt in de neutrale 250-280°-zone zonder piervoordeel. Golf 0,91-1,03m — net onder de drempel. Risico (sterke pal aanlandige wind zonder bescherming), geen bruikbaar venster.

**Beste dag: dinsdag 24 november** (±10:00-13:00) — de sterkste, meest bruikbare richting/wind-combinatie van de hele outlook-periode, alleen de golf blijft net onder de klassieke 1,1m-drempel. Kans: **laag-tot-gemiddeld** — geen dag in deze periode haalt een schone Optimaal-classificatie. ⚠️ Onzeker op 4+ dagen — check dichter bij de tijd opnieuw. Let in latere runs vooral op: (1) of dinsdag 24 november's golf de 1,1m-drempel alsnog haalt, en (2) hoe de grote modelverdeeldheid van vandaag/donderdag zich de komende dagen ontwikkelt — als Windfinder/Soarcast structureel te hoog blijven zitten t.o.v. windwaarnemingen, verdient die laatste meer gewicht in komende briefings.

---
_Bronnen: Windfinder (GFS) · Soarcast (KNMI Harmonie, IJmond) · windwaarnemingen.nl (KNMI, IJmuiden)_
