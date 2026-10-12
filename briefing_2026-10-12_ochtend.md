# 🌊 Wingfoil-briefing Zandvoort–Wijk aan Zee
_12-10-2026 · Ochtendbriefing_

⚠️ **Technische kanttekening:** Soarcast blijft onbereikbaar deze run (pure JS/Vite-app, geen server-rendered data, geen bruikbaar API-pad gevonden in de JS-bundle — net als alle voorgaande runs). Windfinder is via de onderliggende paginadata (Astro-island props, `ForecastSection`/`ForecastDataInit`/`FcTableWindpreviewContainer`) van de reguliere forecast-pagina opgehaald — deze ene pagina bevat al 3-uurs data t/m 21 oktober (dag 1 t/m 10), dus de Superforecast-pagina was niet nodig. windwaarnemingen.nl (IJmuiden) is via de onderliggende `database/vsp_vdg_wstats.php?st=IJmuiden1` (vandaag, 10-minuten-actuals + ingebed KNMI-uurmodel) en `vsp_mrg_wstats.php?st=IJmuiden2` (morgen + overmorgen t/m 16:00, KNMI-uurmodel) opgehaald.

---

## ⚡ Snel overzicht
- **Maandag:** Slecht (wind vrijwel de hele dag te zwak, 4,8-13 kts; kort randje bij IJmuiden/Wijk aan Zee rond 02:00-05:00 maar praktisch niet relevant door de zwakte)
- **Dinsdag:** Optimaal (14:00-17:00, piek ~17:00)
- **Woensdag:** Slecht (vroege ochtend 02:00-05:00 grensgeval Matig bij IJmuiden, daarna wind te zwak)
- **Beste dag in de 7 dagen erna:** zaterdag 17 oktober
_(De eerste 3 regels zijn altijd de eerstvolgende 3 volle dagen vanaf het moment van versturen.)_

---

## ⏰ Realitycheck vandaag

- Laatste actuele uren (windwaarnemingen.nl, IJmuiden, 05:00-07:10): **wind 7,6-9,2 kts (10-minutenwaarden), gust 8,5-11,3 kts**, richting vrij stabiel Zuid/ZZO (163-177°).
- Was voorspeld voor dezelfde uren: het ingebedde KNMI-uurmodel (windwaarnemingen.nl zelf) gaf voor 05h-07h **173-219°, 2,7-4,4 kts, gust 5,9-6,2 kts**; Windfinder (GFS) gaf voor de dichtstbijzijnde tijdstippen (05h/08h) **168-236°, 3,8-4,8 kts, gust 6,0-9,0 kts**.
- Conclusie: de wind loopt **licht VOOR** op beide modellen (7,6-9,2 kts actueel tegen 2,7-4,8 kts voorspeld — merkbaar sterker, al blijft het absolute niveau nog steeds zwak). Richting klopt goed bij het KNMI-model (zuid/zuidoost), maar Windfinder/GFS had de draai naar zuid nog niet goed te pakken (liet om 05:00 nog 235,7° WZW zien, terwijl het al 163-177° zuidelijk woei om diezelfde tijd — de draai kwam dus eerder dan GFS liet zien). Rest-van-de-dag inschatting: **ongewijzigd** — de iets hogere actuele snelheid verandert niets aan de kernconclusie dat vandaag een zwakke winddag is (ruim onder de 14 kts-drempel); het bevestigt vooral dat de richtingdraai naar zuid rond 03:30-04:00 al heeft plaatsgevonden, eerder dan beide modellen voor vanochtend lieten zien.

---

## 📅 Komende 72 uur

### Maandag — Slecht
- Bij **Zandvoort/Wijk aan Zee**: de wind is de **vrijwel hele dag te zwak** (4,8-13,0 kts) om serieus te varen. Richting draait van pal aanlandig (261,6° om 02:00) via side-shore (168-158°, 08:00-17:00) naar pal aflandig (135° om 20:00) en weer side-shore/licht aflandig (152,5° om 23:00) → **Slecht (te weinig wind)** het grootste deel van de dag. Om 23:00 piekt de gust tot 23,9 kts bij nog steeds een zwak gemiddelde (13,0 kts) — een **grensgeval richting Matig**, maar nog niet overtuigend genoeg om als venster te noemen.
- Bij **IJmuiden** (pierzone-hoek): **02:00** (261,6°) en **05:00** (235,7°) lezen hier als **pal aanlandig**, met golf 0,80-0,94m (≥0,8m) — ziet er zwaarder uit dan bij Zandvoort, maar de wind is op dat moment zo zwak (4,8-7,6 kts) dat dit praktisch niet relevant is.
- 🌊 Piervoorkeur: **02:00** valt de richting (261,6°) in de **neutrale pierzone (250-280°)** — geen duidelijk voordeel. **05:00** (235,7°, binnen 170-250°) zou **Wijk aan Zee (Noordpier)** rustiger maken, maar bij 4,8 kts wind is dit zonder praktisch belang.
- Golven (Windfinder, enige golfbron): 0,40-0,94m / 5,0-6,3s — de hele dag onder de 1,1m-drempel.
- Getij: laagwater ~00:56 (0,28 m), hoogwater ~05:20 (2,14 m), laagwater ~13:17 (0,49 m), hoogwater ~17:38 (2,13 m).
- Bronnen: Windfinder enige bron met golfdata. windwaarnemingen.nl (KNMI-model) bevestigt de zwakke wind, maar laat de wind al vanaf 04:00 naar zuid draaien terwijl Windfinder/GFS dat pas later in de ochtend laat zien → **wijkt af qua timing van de richtingdraai, eens over de zwakte**. Soarcast niet bereikbaar.

### Dinsdag — Optimaal
- Bij **Zandvoort/Wijk aan Zee**: **00:00-11:00** is de richting side-shore (167-201°, zuid/ZZW) maar de wind blijft net onder de 14 kts-drempel (12,4-14,3 kts) met golf nog onder de 1,1m-grens (0,67-0,91m) → **grensgeval Matig/Goed** — richting en golf verbeteren geleidelijk, wind net niet genoeg. **Vanaf 14:00** komt de golf over de drempel (1,11m/5,7s) bij wind 18,1 kts en nog steeds side-shore richting (214,7°) → **Optimaal**. Dit zet door tot **17:00** (19,7 kts, golf 1,35m/6,0s, richting 242,3° — nog net side-shore bij Zandvoort) — het beste venster van de dag. **Vanaf 20:00** draait de richting naar **pal aanlandig** (308,5° en 290,4° om 23:00) bij nog stevige golf (1,16-1,24m) → **Slecht/grensgeval Slecht bij Zandvoort en Wijk aan Zee** (forse branding, pal aanlandig) ondanks de op zichzelf prima windkracht (15,4-17,0 kts).
- Bij **IJmuiden** (pierzone-hoek): overdag (11:00-14:00, richting 200-215°) leest als **pal aanlandig/licht aanlandig** bij IJmuiden — iets minder gunstig dan Zandvoorts side-shore-lezing op dat moment. **Vanaf 20:00** (richting 308,5-290,4°) draait IJmuiden juist naar **side-shore** — precies tegenovergesteld aan Zandvoort/Wijk aan Zee op dat moment.
- 🌊 Piervoorkeur: **20:00-23:00** is de richting (290-309°, NW) bij Zandvoort/Wijk aan Zee pal aanlandig met golf 1,16-1,24m (≥0,8m, forse branding) → **IJmuiden (Zuidpier)** is dan duidelijk de rustigere/veiligere keuze — de richting valt in de 280-360°-zone waar de Zuidpier de NW-golfslag blokkeert, en IJmuiden leest hier toch al side-shore.
- Golven (Windfinder): 0,67-1,35m / 5,5-6,0s — ruim over de drempel vanaf de namiddag.
- Getij: laagwater ~01:43 (0,29 m), hoogwater ~05:57 (2,11 m), laagwater ~14:04 (0,43 m), hoogwater ~18:13 (2,17 m).
- Bronnen: Windfinder en windwaarnemingen.nl (KNMI-uurmodel) komen goed overeen in trend en richting (zuid → zuidwest → noordwest), met iets lagere piekwaarden bij het KNMI-model (22,0-22,6 kts rond 14:00-17:00 tegen Windfinders 18,1-19,7 kts is juist omgekeerd — KNMI zit hier hoger) → **wijkt licht af qua exacte snelheid, eens over richting en trend**. Soarcast niet bereikbaar.

### Woensdag — Slecht
- Bij **Zandvoort/Wijk aan Zee**: **02:00-05:00** is de richting pal aanlandig (302,7-308,6°) bij afnemende wind (17,0 → 14,9 kts) en stevige golf (1,12-1,15m/5,6s, ruim over de drempel) → **grensgeval Matig/Slecht bij Zandvoort** (de golf + pal aanlandige hoek pleiten voor Slecht, maar de wind is op zich nog net voldoende). **Vanaf 08:00** valt de wind snel terug (10,2 kts, verder dalend naar 7,3-9,3 kts de rest van de dag) → **Slecht (te weinig wind)** voor de rest van de dag, ondanks een geleidelijke draai naar gunstiger side-shore richting (235-197°) in de middag/avond.
- Bij **IJmuiden** (pierzone-hoek): **02:00-05:00** leest hier als **side-shore** (i.p.v. pal aanlandig bij Zandvoort) — een duidelijk gunstiger hoek op het moment dat daar nog bruikbare wind staat (14,9-17,0 kts).
- 🌊 Piervoorkeur: **02:00-05:00** valt de richting (302,7-308,6°, NW) bij Zandvoort/Wijk aan Zee pal aanlandig met golf ≥0,8m → **IJmuiden (Zuidpier)** is de rustigere/gunstigere keuze (zelfde logica als dinsdagavond: richting in de 280-360°-zone, en IJmuiden leest hier toch al side-shore). Dit is het enige moment vandaag waar de wind nog sterk genoeg is (14,9-17,0 kts) om dit verschil praktisch relevant te maken.
- Golven (Windfinder): 0,68-1,15m / 5,6-6,0s — hoog aan het begin van de dag, dalend naar de avond.
- Getij: laagwater ~02:31 (0,30 m), hoogwater ~06:34 (2,05 m), laagwater ~14:47 (0,38 m), hoogwater ~18:47 (2,17 m).
- Bronnen: Windfinder enige bron met golfdata tot deze diepte; windwaarnemingen.nl stopt om 16:00 voor deze dag. Beide bronnen laten dezelfde dalende windtrend zien → **eens over trend**. Check dicht bij de tijd opnieuw, vooral voor het vroege-ochtendvenster (02:00-05:00) dat nu nog op 2 dagen vooruit leunt. Soarcast niet bereikbaar.

---

## 🔭 Kans op mooie sessies daarna (dag 4-9)
Windfinder (GFS, enige bron zo ver vooruit, 3-uurs resolutie) voor **donderdag 15 t/m dinsdag 20 oktober**:

- **Donderdag 15 oktober**: wind blijft zwak (6,9-10,4 kts), richting side-shore/zuid (175-210°) — goede hoek, maar te weinig kracht → **Slecht**, geen bruikbaar venster.
- **Vrijdag 16 oktober**: overdag nog zwak (7,1-8,0 kts) en wisselvallig van richting, maar **vanaf 17:00** trekt de wind sterk aan (18,1 kts) bij noordelijke/side-shore richting (352°) en golf net over de drempel (1,02m/5,2s) → **grensgeval Optimaal**. **Om 23:00**: 17,0 kts, golf 1,13m/5,8s, richting 2,6° (side-shore) → **Optimaal**.
- **Zaterdag 17 oktober — beste dag**: de Optimaal-periode zet door vanaf vrijdagavond de **hele nacht en vroege ochtend** (02:00-08:00, richting 0-16° (noord), side-shore, wind 15,7-15,9 kts, golf 1,02-1,11m/6,0-6,1s). Rond 11:00 een korte dip naar Matig (14,4 kts, golf 0,97m), maar de rest van de dag (14:00-23:00) blijft het een **grensgeval Goed/Optimaal**: wind 15,4-17,8 kts, side-shore richting (3-12°), golf net onder de drempel (0,87-0,92m). Dit is in feite één lange, grotendeels aaneengesloten goede periode die al vrijdagavond begint en de hele zaterdag doorloopt (~24-30 uur).
- **Zondag 18 oktober**: sterke wind (17,7-21,5 kts) en goede side-shore hoek (346-9°) de hele ochtend, maar de golf blijft net onder de 1,1m-drempel (0,73-0,83m) → **grensgeval Goed/Optimaal** (alleen de golfhoogte ontbreekt voor een volwaardig Optimaal-oordeel). Vanaf de middag draait de richting naar (licht) aflandig (46-99°) bij afnemende golf → **Matig**, met een korte terugval richting Slecht in de late namiddag (wind 11,6 kts).
- **Maandag 19 oktober**: stevige wind (14,5-20,0 kts) bij licht aflandige/aflandige richting (70-84°) — een aflandige hoek geeft vlak water, maar de golf blijft laag (0,60-0,68m, period 6,3-6,8s) waardoor dit niet als volwaardig Optimaal classificeert → **grensgeval Goed**, met name 11:00-20:00 (wind 18-20 kts).
- **Dinsdag 20 oktober**: wind iets zwakker (12,4-15,3 kts) nog steeds aflandig (82-96°), golf 0,55-0,65m oplopend in periode (6,2-8,0s) → **Matig, grensgeval Goed**.

**Beste dag: zaterdag 17 oktober**, met een lange Optimaal/grensgeval-Optimaal-periode die al vrijdagavond begint en de volle zaterdag doorloopt — side-shore richting en wind rond 15-18 kts de hele dag, golf precies rond de drempelwaarde. Kans: **gemiddeld tot hoog** — een langere aaneengesloten periode met consistent signaal (noordelijke/side-shore wind) maakt dit robuuster dan een losse dag, maar op 5-6 dagen vooruit kan de exacte golfhoogte (die nu net rond de 1,1m-drempel schommelt) nog kantelen in beide richtingen.
⚠️ Onzeker op 4+ dagen — check dichter bij de tijd opnieuw.

---
_Bronnen: Windfinder (GFS) · windwaarnemingen.nl (KNMI, IJmuiden) · Soarcast — deze run niet bereikbaar (JS-app, geen vindbaar/bereikbaar API-adres)_
