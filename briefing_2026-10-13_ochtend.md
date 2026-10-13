# 🌊 Wingfoil-briefing Zandvoort–Wijk aan Zee
_13-10-2026 · Ochtendbriefing_

⚠️ **Technische kanttekening:** Soarcast blijft onbereikbaar deze run (pure JS/Vite-app, `/web/locationinfo?...` levert alleen een lege HTML-shell; ook de onderliggende JS-bundle doorzocht op een API-endpoint — niets bruikbaars gevonden, zelfde conclusie als alle voorgaande runs). Windfinder is opgehaald via de onderliggende Astro-island props op de reguliere forecast-pagina: de `ForecastSection`-componenten bevatten per dag volledige data inclusief golven/getij en dekken samen dag 1 t/m 10 (13-22 oktober) in 3-uurs stappen, dus de Superforecast-pagina was niet nodig. windwaarnemingen.nl (IJmuiden) is opgehaald via `database/vsp_vdg_wstats.php?st=IJmuiden1` (vandaag: 10-minuten-actuals + ingebed KNMI-uurmodel) en `vsp_mrg_wstats.php?st=IJmuiden2` (morgen + overmorgen t/m 16:00, KNMI-uurmodel). **Opvallend deze run:** Windfinder (GFS) en windwaarnemingen.nl (KNMI-Harmonie) wijken voor dinsdag/woensdag fors af in windkracht (GFS vaak 40-100% hoger dan KNMI) terwijl de richting tussen beide modellen juist goed overeenkomt — zie Realitycheck en de dagsecties hieronder voor hoe dit is meegenomen.

---

## ⚡ Snel overzicht
- **Dinsdag:** Optimaal volgens Windfinder/GFS (14:00-16:00, ~20 kts), maar grote modelonzekerheid — KNMI voorspelt voor dezelfde uren maar ~12 kts (Matig-niveau); zie Realitycheck. Vanaf 17:00 draait de wind pal aanlandig met forse branding (1,2-1,4m) → Slecht/grensgeval.
- **Woensdag:** Slecht (grootste deel van de dag te zwak, 5,9-9,7 kts vanaf 08:00); vroege ochtend 02:00-05:00 grensgeval Optimaal/Goed bij **IJmuiden** dankzij pierbeschutting (zie piervoorkeur), terwijl Zandvoort/Wijk aan Zee op dat moment pal aanlandig met forse branding zien.
- **Donderdag:** Grensgeval Matig/Goed de hele dag (side-shore, wind geleidelijk oplopend naar 14,5 kts rond 14:00, golf net onder de 1,1m-drempel: 0,71-0,87m).
- **Beste dag in de 7 dagen erna:** zaterdag 17 oktober
_(De eerste 3 regels zijn altijd de eerstvolgende 3 volle dagen vanaf het moment van versturen.)_

---

## ⏰ Realitycheck vandaag

- Laatste actuele uren (windwaarnemingen.nl, IJmuiden, 06:00-07:10, 10-minutenwaarden): **wind 5,9-6,5 kts, gust 7,9-9,1 kts, richting 161-169° (zuid/ZZO)**.
- Was voorspeld voor dezelfde uren: het **ingebedde KNMI-uurmodel** (windwaarnemingen.nl zelf) gaf voor 06h/07h **175-180°, 6,1-6,3 kts, gust 9,1 kts** — nagenoeg gelijk aan de actuals (actueel zelfs licht zwakker). **Windfinder/GFS** gaf voor de dichtstbijzijnde 3-uurspunten (05h/08h) **179-189°, 12,3-13,5 kts, gust 19,9-26,6 kts** — ruim het dubbele van wat er nu daadwerkelijk staat.
- Conclusie: de wind loopt **fors ACHTER op Windfinder/GFS**, maar **klopt vrijwel exact met windwaarnemingen.nl/KNMI** (zelfs nog iets zwakker dan dat model zelf voorspelde). Richting komt bij beide modellen wel overeen (zuid/ZZO → geleidelijke draai naar ZW gedurende de dag). Rest-van-de-dag inschatting: **naar beneden bijgesteld** — het "Optimaal"-venster van vanmiddag (14:00-17:00, 20 kts volgens GFS) steunt vrijwel volledig op het model dat vanochtend al duidelijk te sterk bleek; KNMI's eigen voorspelling voor diezelfde namiddag-uren (~12 kts, Matig-niveau) is gezien de ochtendcijfers aannemelijker. Houd rekening met een reëel scenario tussen Matig en Goed in plaats van het door GFS gesuggereerde Optimaal, en check dit dicht bij de tijd opnieuw.

---

## 📅 Komende 72 uur

### Dinsdag — Optimaal (Windfinder) / grensgeval Matig-Goed (KNMI) — zie toelichting
- Bij **Zandvoort/Wijk aan Zee**: **02:00-08:00** is de richting side-shore (173-189°, zuid/ZZW) bij geleidelijk oplopende wind (11,8→13,5 kts, gust tot 26,6 kts) en nog zwakke golf (0,56-0,75m) → **grensgeval Matig** (wind net onder de drempel, golf nog te laag). **11:00**: wind 15,8 kts (gust 25,3), golf 1,04m/5,86s, richting 210,8° (side-shore) → **grensgeval Goed/Optimaal**. **14:00**: volgens Windfinder/GFS 20,2 kts (gust 30,6), golf 1,30m/6,01s, richting 222,4° (side-shore) → **Optimaal** — maar zie Realitycheck: KNMI voorspelt voor dit moment maar ~12 kts, dus behandel dit venster als **onzeker, mogelijk eerder Matig/Goed**. **Vanaf 17:00** draait de richting **pal aanlandig** (259,5° → 291-301,5° in de avond) bij nog altijd stevige wind (12,8-19,7 kts) en zware golf (1,11-1,44m) → **Slecht/grensgeval Slecht** (forse branding, pal aanlandig) ondanks de op zichzelf prima windkracht.
- Bij **IJmuiden** (pierzone-hoek): **11:00-23:00** leest de richting (210,8-291°) hier grotendeels als **pal aanlandig** (211-260°) tot **side-shore** (291°) — op de momenten dat Zandvoort juist aanlandig krijgt (17:00, 259,5°) is ook IJmuiden pal aanlandig, geen voordeel.
- 🌊 Piervoorkeur: **17:00** (259,5°, tussen de twee pierassen) → **neutrale zone (250-280°)**, geen van beide pieren biedt hier voordeel — zowel IJmuiden als Wijk aan Zee pal aanlandig met golf 1,44m, dus bij beide stevige branding. **20:00-23:00** (291-301,5°, NW) → **IJmuiden (Zuidpier)** rustiger: bij Zandvoort/Wijk aan Zee pal aanlandig met golf 1,0-1,2m, bij IJmuiden leest de hoek hier al side-shore.
- Golven (Windfinder, enige golfbron): 0,56-1,44m / 5,3-6,2s — oplopend gedurende de dag, piek rond 17:00.
- Getij: laagwater ~01:43 (0,29 m), hoogwater ~05:57 (2,11 m), laagwater ~14:04 (0,43 m), hoogwater ~18:13 (2,17 m).
- Bronnen: Windfinder (GFS) en windwaarnemingen.nl (KNMI-uurmodel) **wijken sterk af in windkracht** (GFS 40-100% hoger) maar **zijn eens over de richting** (zuid → ZW → WZW/NW-draai in de avond) → vermeld beide, niet gemiddeld; zie Realitycheck voor welke kant de ochtendcijfers op wijzen. Soarcast niet bereikbaar.

### Woensdag — Slecht (grootste deel van de dag), grensgeval Optimaal/Goed bij IJmuiden in de vroege ochtend
- Bij **Zandvoort/Wijk aan Zee**: **02:00-05:00** is de richting pal aanlandig (298,7-309,4°) bij nog stevige wind (12,5-15,1 kts) en zware golf (1,15-1,19m/5,6-5,7s, ruim over de drempel) → **Slecht/grensgeval** (forse branding, pal aanlandig, ondanks op zich bruikbare windkracht). **Vanaf 08:00** valt de wind snel terug (6,9 kts, verder dalend tot 5,9-9,7 kts de rest van de dag) → **Slecht (te weinig wind)** voor de rest van de dag, met een geleidelijke draai naar side-shore/licht aflandig (251°→198°) in de middag/avond die niets meer uitmaakt door de zwakte.
- Bij **IJmuiden** (pierzone-hoek): **02:00-05:00** leest de richting hier als **side-shore** (i.p.v. pal aanlandig bij Zandvoort/Wijk aan Zee) — een duidelijk gunstiger hoek op het enige moment vandaag dat de wind nog bruikbaar is. Om 02:00: wind 15,1 kts, golf 1,15m/5,58s, side-shore → komt uit op **Optimaal**. Om 05:00: wind 12,5 kts, golf 1,19m/5,7s, side-shore (niet pal aanlandig) → **Goed (b)**.
- 🌊 Piervoorkeur: **02:00-05:00** valt de richting (299-309°, NW) bij Zandvoort/Wijk aan Zee pal aanlandig met golf ≥0,8m → **IJmuiden (Zuidpier)** is de duidelijk gunstigere keuze (richting in de 280-360°-zone, Zuidpier blokkeert de NW-golfslag, en IJmuiden leest hier toch al side-shore). Dit is het enige bruikbare venster van de dag — vlak bij de pier dus, niet op het open strand.
- Golven (Windfinder): 0,70-1,19m / 5,56-6,28s — hoog aan het begin van de dag, dalend naar de avond.
- Getij: laagwater ~02:31 (0,30 m), hoogwater ~06:34 (2,05 m), laagwater ~14:47 (0,38 m), hoogwater ~18:47 (2,17 m).
- Bronnen: Windfinder en windwaarnemingen.nl/KNMI zijn het **eens over de richting** (NW vroeg, draaiend naar zuid/zuidwest later) en over de **dalende trend**, maar Windfinder zit opnieuw structureel hoger in windkracht (bv. 02:00: 15,1 vs 10,7 kts KNMI; 14:00: 8,8 vs 4,9 kts KNMI) — gezien de Realitycheck van vanochtend is het aannemelijk dat KNMI dichter bij de werkelijkheid zal liggen, wat het IJmuiden-venster om 02:00 mogelijk dichter bij Goed(b) dan bij Optimaal brengt. Soarcast niet bereikbaar.

### Donderdag — grensgeval Matig/Goed
- Bij **Zandvoort/Wijk aan Zee**: de hele dag is de richting **side-shore** (192,9-220,9°, zuid/ZZW), met de wind geleidelijk oplopend van 8,4 kts (02:00/23:00) naar een piek van **14,5 kts rond 14:00** (gust 15,2-20,9 kts de hele dag). De golf blijft de hele dag net onder de 1,1m-drempel (0,71-0,87m, periode 5,2-5,5s) → dit past bij geen van de tabelrijen exact (wind+richting zitten in de Optimaal-band, alleen de golf ontbreekt) → **grensgeval Matig/Goed**, met het beste moment rond **14:00** (14,5 kts, side-shore, golf 0,87m — net te weinig voor Optimaal).
- Bij **IJmuiden** (pierzone-hoek): **vanaf 14:00** leest de richting hier als **licht aanlandig** (209°) tot **pal aanlandig** (17:00, 220,9°) — iets minder gunstig dan Zandvoorts side-shore op dat moment.
- 🌊 Piervoorkeur: **14:00-17:00** is de richting bij IJmuiden licht/pal aanlandig met golf 0,86-0,87m (≥0,8m) → **Wijk aan Zee (Noordpier)** zou dan de rustigere keuze zijn, al is het effect met golf net onder 0,9m mild.
- Golven (Windfinder): 0,71-0,87m / 5,24-5,50s — de hele dag onder de 1,1m-drempel, maar dicht erbij.
- Getij: laagwater ~03:08 (0,34 m), hoogwater ~07:08 (1,97 m), laagwater ~15:21 (0,36 m), hoogwater ~19:21 (2,13 m).
- Bronnen: windwaarnemingen.nl dekt deze dag alleen tot 16:00 (KNMI-model); voor het beschikbare deel van de dag komen beide bronnen qua **richting en de geleidelijk oplopende trend goed overeen**, Windfinder iets hoger in snelheid. Check het middagvenster (14:00) dicht bij de tijd opnieuw, zowel voor de exacte windkracht als voor de golfhoogte die nu net onder de drempel zit. Soarcast niet bereikbaar.

---

## 🔭 Kans op mooie sessies daarna (dag 4-9)
Windfinder (GFS, enige bron zo ver vooruit, 3-uurs resolutie) voor **vrijdag 16 t/m woensdag 21 oktober**:

- **Vrijdag 16 oktober**: ochtend/vroege middag nog zwak en side-shore (8,5-10,2 kts) → Slecht. Om **14:00** draait de richting naar licht aanlandig (320°, NNW) bij 14,1 kts en golf 1,01m/4,97s (periode <5s) → **Goed (a)**. **Vanaf 17:00** draait de richting verder naar **side-shore/noord** (348-357°) bij 15,7-17,7 kts en golf oplopend tot 1,16-1,19m (periode ≥5s) → **Optimaal**, en dit zet door de hele avond/nacht door.
- **Zaterdag 17 oktober — beste dag**: de Optimaal-periode die vrijdagavond begint loopt door tot diep in de ochtend (**02:00-05:00**, richting 2-6° (noord), side-shore, wind 15,3-15,7 kts, golf 1,11-1,16m/6,0-6,1s) → **Optimaal**. Van **08:00 tot 20:00** blijft de richting side-shore/NNO (10-25°) met stevige wind (13,4-17,4 kts, gust 19,3-21,8 kts), maar de golf zakt net onder de 1,1m-drempel (0,92-1,06m) → **grensgeval Goed/Optimaal** de hele dag — in de praktijk één lange, grotendeels aaneengesloten goede periode van ruim 24 uur (vrijdagavond t/m zaterdagavond).
- **Zondag 18 oktober**: wind valt terug (6,0-11,0 kts) en de richting draait via side-shore (02:00, 35°) naar licht aflandig/pal aflandig vanaf de middag (65-94°) bij lage golf (0,65-0,84m) → **Matig, grensgeval Slecht** door de zwakte, met aflandige (vlakke) condities als enige pluspunt.
- **Maandag 19 oktober**: wind blijft zwak tot matig (6,3-12,6 kts), richting pal/licht aflandig (69-96°) — vlak water door de aflandige hoek, maar te weinig kracht voor een volwaardige sessie → **Slecht, grensgeval Matig** (vooral 's avonds, 23:00: 12,6 kts).
- **Dinsdag 20 oktober**: **02:00-08:00** licht/pal aflandig (66-73°) met wind net onder de 14kts-drempel (11,9-13,4 kts) maar pittige gust (19,4-21,5 kts) en lage golf (0,49-0,55m) → **grensgeval Matig/Goed** (vlak water, gustiger dan gemiddeld). **11:00**: pal aflandig, 13,1 kts, golf 0,50m → **Matig**. Rest van de dag te zwak → **Slecht**.
- **Woensdag 21 oktober**: overwegend zwak en wisselvallig aflandig (5,9-10,0 kts) → **Slecht**, met een lichte verbetering richting de avond (20:00-23:00: 9,9-10,0 kts, gust 17,8-18,5 kts, golf 0,62-0,64m) → **grensgeval Matig**.

**Beste dag: zaterdag 17 oktober**, met een lange Optimaal/grensgeval-Optimaal-periode die al vrijdagavond begint en de volle zaterdag doorloopt — noordelijke/side-shore wind rond 13-18 kts de hele periode, golf net rond de drempelwaarde. Kans: **gemiddeld tot hoog** — dit is dezelfde periode die ook in eerdere briefings al als beste venster naar voren kwam (consistent signaal over meerdere modelruns heen), maar op 4-5 dagen vooruit kan de golfhoogte (die nu net rond de 1,0-1,1m-drempel schommelt) nog kantelen in beide richtingen.
⚠️ Onzeker op 4+ dagen — check dichter bij de tijd opnieuw.

---
_Bronnen: Windfinder (GFS) · windwaarnemingen.nl (KNMI, IJmuiden) · Soarcast — deze run niet bereikbaar (JS-app, geen vindbaar/bereikbaar API-adres)_
