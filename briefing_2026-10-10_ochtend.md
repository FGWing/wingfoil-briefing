# 🌊 Wingfoil-briefing Zandvoort–Wijk aan Zee
_10-10-2026 · Ochtendbriefing_

⚠️ **Technische kanttekening:** Soarcast blijft onbereikbaar deze run (pure JS/Vite-app, geen server-rendered data, geen bruikbaar API-pad gevonden in de gebundelde JS). Windfinder is via de onderliggende paginadata opgehaald: de reguliere forecast-pagina embedt in een Astro-island-payload 3-uurs data tot en met 19 oktober (dag 1 t/m 9), de Superforecast-pagina gaf aanvullend uurdata voor vandaag. windwaarnemingen.nl (IJmuiden) is via het onderliggende `database/vsp_vdg_wstats.php`-endpoint opgehaald (10-minuten-actuals + ingebed KNMI-uurmodel).

---

## ⚡ Snel overzicht
- **Zaterdag:** Slecht bij Zandvoort/Wijk aan Zee (hele dag pal aanlandig, golf 1,8-2,3m) — Goed, grensgeval Optimaal tot Optimaal bij IJmuiden vrijwel de hele dag (07:00-23:00)
- **Zondag:** Slecht bij Zandvoort/Wijk aan Zee (hele dag) — Optimaal bij IJmuiden 05:00-11:00, Goed/grensgeval Optimaal 02:00 en 14:00, vanaf ~15:00 te weinig wind
- **Maandag:** Matig tot Slecht bij alle plekken — wind te zwak (7-12 kts) het grootste deel van de dag, iets meer richting Matig in de avond (20:00-23:00) bij zuidelijke wind
- **Beste dag in de 7 dagen erna:** dinsdag 13 oktober
_(De eerste 3 regels zijn altijd de eerstvolgende 3 volle dagen vanaf het moment van versturen.)_

---

## ⏰ Realitycheck vandaag

- Laatste actuele uren (windwaarnemingen.nl, IJmuiden, 05:00-07:10): **wind 12,4-15,4 kts gem (uurgemiddelden 13,0-14,6 kts), gust 14,7-17,6 kts**, richting WNW→WEST (266°→288°, geleidelijk draaiend naar west).
- Was voorspeld voor dezelfde uren: ingebedde KNMI-uurmodel (windwaarnemingen.nl zelf) gaf 05h-07h **272-278°, 10,5-12,1 kts, gust 15,3-16,4 kts**; Windfinder (GFS) gaf voor 05h **277,7° 20/24 kts** en voor de ochtend-superforecast (07h) **280,8° 18/23 kts**.
- Conclusie: de wind loopt **licht VOOR** op het lokale KNMI-model (13-14,6 kts actueel tegen 10,5-12,1 kts voorspeld, gust vergelijkbaar), maar duidelijk **ACHTER** op Windfinder/GFS (13-14,6 kts actueel tegen 18-20 kts voorspeld, gust 15-18 kts tegen 23-24 kts voorspeld). Richting klopt bij alle bronnen goed (drift van WNW naar West). Rest-van-de-dag inschatting: **licht bijgesteld naar de voorzichtige kant** voor de wind-snelheid — de Goed/grensgeval Optimaal-classificatie bij IJmuiden blijft overeind (direction/golf-criteria zijn hier bepalend, niet de exacte kts-waarde), maar houd rekening met gemiddelde windsnelheden dichter bij 14-18 kts dan bij de 18-25 kts die Windfinder voor de rest van de dag laat zien, zeker in de vroege uren. Richting de avond (als Windfinder een verdere toename naar 23-25 kts gust 28 kts laat zien) is de marge weer groter, dus dat deel van de dag kan alsnog kloppen.

---

## 📅 Komende 72 uur

### Zaterdag — Slecht bij Zandvoort/Wijk aan Zee, Goed/grensgeval Optimaal tot Optimaal bij IJmuiden
- Bij **Zandvoort/Wijk aan Zee** (hoek resp. 287,5°/283,8°): wind staat de **hele dag pal aanlandig** (richting 272-287°, WNW/West) met grote golf (1,8-2,3m / 7-8s, oplopend gedurende de dag) → **Slecht** de volle dag, geen bruikbaar venster (grote branding, geen pierbescherming).
- Bij **IJmuiden** (pierzone-hoek 150°/330°, pal aanlandig 240°): dezelfde richting (272-287°) leest hier als **licht aanlandig** → wind 18-25 kts + golf ruim over de drempel (>1,1m/≥5s) geeft **Goed, grensgeval Optimaal** vrijwel de hele dag. Rond **00:00** en **16:00** draait de richting net door naar **side-shore** (285-287°) → kort **Optimaal**. Wind blijft stevig: 18-25 kts gem, gust 22-28 kts (zie Realitycheck — houd in de ochtend rekening met iets zwakkere waarden).
- 🌊 Piervoorkeur: richting schommelt rond de grens van de **neutrale pierzone (250-280°)**; rond **00:00, 13:00 en 16:00-18:00/23:00** komt de richting net boven 280° (NW) en krijgt **IJmuiden** een licht Zuidpier-voordeel. De rest van de dag (272-280°) is IJmuidens betere klasse vooral te danken aan de **eigen kustlijnhoek** (licht aanlandig i.p.v. pal aanlandig bij Zandvoort/WaZ), niet aan pierbescherming.
- Golven (Windfinder, enige golfbron): 1,8-2,3m / 7-8s — ruim boven de drempel de hele dag.
- Getij: hoogwater ~04:05 (2,16 m), laagwater ~12:00 (0,49 m), hoogwater ~16:25 (1,99 m), laagwater ~00:14 (0,26 m, nacht naar zondag).
- Bronnen: Windfinder enige bron met golfdata; windwaarnemingen.nl bevestigt richting goed, loopt qua windkracht iets achter op Windfinder (zie Realitycheck) → **wijkt af qua snelheid, eens over richting**. Soarcast niet bereikbaar.

### Zondag — Slecht bij Zandvoort/Wijk aan Zee, Optimaal bij IJmuiden tot ~11:00
- Bij **Zandvoort/Wijk aan Zee**: wind staat tot in de namiddag **pal aanlandig** (richting 268-293°) met golf nog 1,1-2,3m → **Slecht**. Vanaf **~17:00** valt de wind onder de 14 kts-drempel (13 kts dalend naar 8 kts om 23:00) → **Slecht (te weinig wind)** voor de rest van de dag/avond.
- Bij **IJmuiden**: **02:00** licht aanlandig (281°) → Goed, grensgeval Optimaal. **05:00-11:00** richting draait naar **285-293°** = **side-shore bij IJmuiden** → **Optimaal**: wind 17-23 kts, gust 20-27 kts, golf 2,0-2,3m/8s. **14:00** terug naar licht aanlandig (283°) → Goed, grensgeval Optimaal (wind 15 kts, golf 1,7m/7s). **Vanaf ~17:00** valt de wind te zwak (13 kts → 8 kts om 23:00) → **Slecht (te weinig wind)**.
- 🌊 Piervoorkeur: **05:00-11:00** (richting 285-293°, NW) is **IJmuiden** duidelijk beschut door de Zuidpier — dit valt samen met de side-shore-lezing, dus een dubbel voordeel. Op de andere momenten (268-283°) grotendeels neutrale zone of eigen kustlijnhoek-voordeel, geen sterk pier-effect.
- Golven (Windfinder): 1,1-2,3m / 7-8s in de ochtend/middag, afnemend naar 1,1m/7s in de avond.
- Getij: hoogwater ~04:43 (2,16 m), laagwater ~12:34 (0,52 m), hoogwater ~17:02 (2,07 m), laagwater ~00:56 (0,28 m, nacht naar maandag).
- Bronnen: alleen Windfinder (golfdata + enige bron die zo ver doorgaat); windwaarnemingen.nl en Soarcast gaan niet zo ver door/niet bereikbaar. **Check dicht bij de tijd opnieuw** — het middaguur waarop de wind wegvalt is in dit soort GFS-runs nog onzeker.

### Maandag — Matig tot Slecht bij alle plekken
- Bij **Zandvoort/Wijk aan Zee**: wind begint zwak en pal aanlandig (267° om 02:00, golf 0,93m) → Slecht. Vanaf **05:00** draait de richting via zuidwest naar zuid (231°→154°) = **side-shore**, maar de wind blijft het grootste deel van de dag te zwak (6,9-11 kts) en de golf te klein (0,72-0,9m, onder de drempel) → **Slecht/Matig** grensgeval. Vanaf **20:00** trekt de wind iets aan (9,9-12 kts, gust 16,8-21,4 kts) bij zuidelijke (154-161°) side-shore richting → **Matig**, met een grensgeval naar Goed(b) rond 23:00 als de gust-waarden kloppen.
- Bij **IJmuiden** (pierzone-hoek): zelfde patroon — vroeg pal/licht aanlandig bij te zwakke wind (Slecht), overdag side-shore maar te zwak (Slecht/Matig), 's avonds oplopend naar Matig.
- 🌊 Piervoorkeur: niet vermeld — richting is overdag side-shore/aflandig-achtig (geen aanlandige situatie van betekenis) en golf blijft het grootste deel van de dag onder de 0,8m-drempel; geen relevant pier-effect.
- Golven (Windfinder): 0,72-0,93m / 5,2-6,5s — onder de 1,1m-drempel de hele dag.
- Getij: hoogwater ~05:20 (2,14 m), laagwater ~13:17 (0,49 m), hoogwater ~17:38 (2,13 m).
- Bronnen: alleen Windfinder; windwaarnemingen.nl en Soarcast gaan niet zo ver door/niet bereikbaar. Zwakke-windsignaal is op 2 dagen vooruit redelijk betrouwbaar, maar check dicht bij de tijd opnieuw voor de exacte avondwaarden.

---

## 🔭 Kans op mooie sessies daarna (dag 4-9)
Windfinder (GFS, enige bron zo ver vooruit, 3-uurs resolutie) voor **dinsdag 13 t/m zondag 18 oktober**:

- **Dinsdag 13 oktober — beste dag**: wind draait zuid/zuidzuidwest (174-237°) en blijft de **vrijwel hele dag side-shore bij Zandvoort**, met golf die rond de middag over de drempel komt (1,07-1,32m/6,2-6,4s vanaf 08:00) → **Optimaal 11:00-20:00**: wind 15-20,6 kts gem, gust 24,9-31,0 kts. Vanaf 23:00 draait de richting naar NW/pal aanlandig → Matig/Slecht daar.
- **Woensdag 14 oktober**: wind valt grotendeels weg en wordt pal aanlandig bij Zandvoort (richting 242-312°, kracht 5,7-14,4 kts), golf net onder de drempel (0,78-0,97m) → **Slecht**, geen goed venster.
- **Donderdag 15 oktober**: zuidelijke wind (171-202°) de hele dag, side-shore bij Zandvoort, maar wind (9,5-12,1 kts) en golf (0,78-1,1m) blijven overwegend onder de Optimaal-drempel → **Matig** als beste classificatie (iets zwakker dan gisteren ingeschat — de modelrun is naar beneden bijgesteld).
- **Vrijdag 16 oktober**: wind draait van WNW (283°, 's ochtends, pal aanlandig) naar **noord/NNO (353-8°)** vanaf 08:00 — dat leest bij Zandvoort als **side-shore**, met golf net over de drempel (1,05-1,16m/5,6-6,2s) → **Optimaal 11:00-23:00**: wind 14,5-17,5 kts, gust 17,5-20,1 kts. **Let op: dit is een duidelijke wijziging t.o.v. de vorige modelrun**, die voor deze dag nog westelijke/pal aanlandige wind liet zien — op 6 dagen vooruit kan dit nog kantelen.
- **Zaterdag 17 oktober**: wind uit noord/NNO (14-34°) maar te zwak (5,4-12,1 kts) → **Slecht tot Matig**, kort Goed(b)-grensgeval rond 02:00.
- **Zondag 18 oktober**: wind zeer zwak en wisselvallig van richting (0,8-6,5 kts) → **Slecht**.

**Beste dag: dinsdag 13 oktober**, met een lang Optimaal-venster (11:00-20:00) bij Zandvoort zelf — geen pier-afhankelijkheid nodig. Kans: **gemiddeld tot hoog** — het signaal is consistent met de vorige modelrun (zelfde dag kwam er gisteren ook al als beste uit), maar de golfhoogte ligt net over de drempel en kan nog kantelen. **Vrijdag 16 oktober** is een nieuwe, nog onzekere tweede kans (grote modelwijziging t.o.v. gisteren) — dichter bij de tijd opnieuw checken.
⚠️ Onzeker op 4+ dagen — check dichter bij de tijd opnieuw.

---
_Bronnen: Windfinder (GFS) · windwaarnemingen.nl (KNMI, IJmuiden) · Soarcast — deze run niet bereikbaar (JS-app, geen vindbaar/bereikbaar API-adres)_
