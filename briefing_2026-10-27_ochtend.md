# 🌊 Wingfoil-briefing Zandvoort–Wijk aan Zee
_27-10-2026 · Ochtendbriefing_

⚠️ **Technische kanttekening:** Alle drie bronnen waren deze run volledig bereikbaar — voor het eerst sinds het begin van deze briefingreeks ook **Soarcast**. Windfinder is opgehaald via de onderliggende Astro-JSON op de reguliere forecast-pagina (die zelf al 9 dagen aan data bevat: dag 1-2 in het hoofd-component, dag 3-10 in een preload-component — de losse Superforecast-pagina was dus niet nodig). windwaarnemingen.nl (IJmuiden) is opgehaald via de vsp-database-endpoints (`vsp_vdg_wstats.php` voor vandaag incl. 10-minuten-actuals, `vsp_mrg_wstats.php` voor morgen+overmorgen tot 15:00u). **Soarcast** is deze keer bereikt via de directe grafiek-eindpunten (`plotPerLocAndUnitReact.php`, locatie 133 = IJmond KNMI) — met één technisch addendum: het `windUnits=kts`-parameter wordt door de API genegeerd, de teruggegeven wind/gust-waarden stonden gewoon in km/u (bevestigd doordat de richtingsdata vrijwel identiek was aan windwaarnemingen.nl, maar de snelheid pas na /1,852 overeenkwam) — hieronder al naar kts omgerekend.

🚨 **Belangrijkste signaal: aanhoudend groot verschil tussen Windfinder/GFS en de twee KNMI-bronnen (windwaarnemingen.nl én nu ook Soarcast), en dit keer een heel zwakke-wind periode.** De Realitycheck bevestigt opnieuw dat de praktijk de KNMI-lijn volgt, niet GFS. Nieuw en belangrijk: Soarcast bevestigt onafhankelijk de KNMI-cijfers (nagenoeg identieke richting, vergelijkbare windkracht) — dat verhoogt het vertrouwen in de KNMI-lijn flink. Netto beeld voor de komende 72 uur: **drie opeenvolgende Slecht-dagen wegens te weinig wind**, en ook de outlook dag 4-9 is zwak, met een forse neerwaartse bijstelling t.o.v. de vorige run (25 oktober).

---

## ⚡ Snel overzicht
- **Dinsdag:** **Slecht** (te weinig wind, hele dag) — KNMI én Soarcast stemmen overeen, Windfinder/GFS loopt fors voor op windkracht (zie Realitycheck).
- **Woensdag:** **Slecht** (te weinig wind, hele dag) — KNMI/Soarcast ~5-9 kts; GFS iets hoger (~9-14 kts) maar blijft in dezelfde categorie.
- **Donderdag:** **Slecht** (te weinig wind, hele dag) — voor het eerst deze week stemmen KNMI én GFS overeen: wind valt vrijwel helemaal weg.
- **Beste dag in de 7 dagen erna:** dinsdag 3 november (hoogstens Matig)

---

## ⏰ Realitycheck vandaag
- Laatste actuele uren (windwaarnemingen.nl, IJmuiden, 04:00-06:10): **wind gem. ~10,4 kts, gust gem. ~12,8 kts (piek 14,5 kts), richting ~175-194° (Zuid/ZZW)**.
- Was voorspeld voor dezelfde uren: **windwaarnemingen.nl/KNMI** gaf gem. **~9,6 kts, gust ~14,4 kts, richting ~187°** — dicht bij de praktijk. **Windfinder/GFS** gaf voor dit venster **~18,7-20 kts gem., gust ~30-32 kts** — bijna het dubbele, bij vergelijkbare richting.
- Conclusie: de wind loopt **licht VOOR op KNMI** qua gemiddelde (+~0,8 kt), de gust juist **licht ACHTER** (-~1,6 kt) — per saldo **conform verwachting**. **Windfinder/GFS overschat opnieuw drastisch** (~+90-100%), net als de afgelopen dagen. Nieuw deze run: **Soarcast (KNMI Harmonie) bevestigt onafhankelijk** de KNMI-lijn voor de rest van de ochtend/middag (9-13 kts, gust 13-17 kts, vrijwel identieke richting) — dit verhoogt het vertrouwen in KNMI als leidende bron aanzienlijk. Rest-van-de-dag inschatting: **ongewijzigd, Slecht (te weinig wind) blijft staan**, nu met hoger vertrouwen dankzij de onafhankelijke Soarcast-bevestiging. Windfinder/GFS-cijfers worden voor de rest van de 72 uur expliciet apart getoond, niet gemiddeld.

---

## 📅 Komende 72 uur

### Dinsdag — Slecht (te weinig wind, hele dag)
- Bij **Zandvoort/Wijk aan Zee**: **KNMI** (windwaarnemingen.nl) voorspelt de hele dag maar **6,4-10,3 kts gemiddeld, gust 10,8-15,3 kts** — ruim onder de 14kts-ondergrens voor Goed/Optimaal en nagenoeg de hele dag binnen de Slecht-drempel (gust <16 én gem <14). **Soarcast** bevestigt dit onafhankelijk voor de daglichturen (9-12,9 kts, gust 13,2-16,8 kts, richting 179-233° — vrijwel identiek aan KNMI). Richting draait van zuid/ZZW (180-204°, side-shore t.o.v. Zandvoorts kustlijn 197,5°) in de ochtend naar west (257-282°, pal aanlandig) in de avond — maar dat maakt niets uit zolang de wind te zwak blijft. **Windfinder/GFS** tekent voor de ochtend een heel ander beeld (18,2-20,1 kts gem., gust 29,8-32,6 kts — dat zou met deze golf en hoek Optimaal betekenen), maar de Realitycheck laat zien dat dit een drastische overschatting is; de praktijk volgt duidelijk de KNMI/Soarcast-lijn.
- 🌊 Piervoorkeur: in de late avond (20:00-24:00) draait de wind pal aanlandig (257-282°) voor Zandvoort/Wijk aan Zee met golf nog ~1,0-1,1m (Windfinder/GFS, enige golfbron) — net binnen de pier-logica-drempel (≥0,8m). Richting valt grotendeels in de **250°-280°-neutrale zone** tussen de twee pierassen → geen duidelijk piervoordeel, en bij deze zwakke windkracht sowieso niet relevant voor een sessie.
- Golven (Windfinder/GFS, enige bron): 1,09-1,52m / 5,7-7,3s, geleidelijk afbouwend door de dag.
- Getij: hoogwater 03:55 (2,3m), laagwater 12:08 (0,49m), hoogwater 16:15 (2,24m), laagwater 20:12 (0,91m, opnieuw verhoogd), kleine secundaire piek 21:18 (0,99m).
- Bronnen: **KNMI en Soarcast stemmen vrijwel exact overeen** op windkracht én richting → hoog vertrouwen. Windfinder/GFS wijkt fors af op windkracht (zie Realitycheck) → expliciet vermeld, niet gemiddeld.

### Woensdag — Slecht (te weinig wind, hele dag)
- Bij **Zandvoort/Wijk aan Zee**: **KNMI** voorspelt **5,3-7,9 kts gemiddeld, gust 6,7-10,9 kts** — de hele dag ruim onder de Slecht-drempel. **Soarcast** bevestigt dit voor de daglichturen (7,1-9,2 kts, gust 9,8-11,6 kts, richting 235-277°). **Windfinder/GFS** geeft iets hogere cijfers (8,7-14,0 kts gem., gust 13,3-16,5 kts) maar blijft daarmee ook in de Matig/Slecht-categorie — voor het eerst deze week is het modelverschil klein genoeg om de classificatie niet te laten kantelen. Richting: westelijk (233-280°) de hele dag, voor Zandvoort pal- tot licht aanlandig.
- 🌊 Piervoorkeur: 's ochtends (00:00-09:00, richting 263-277°, golf nog 1,02-1,16m volgens Windfinder/GFS) is de hoek pal aanlandig voor IJmuiden/Wijk aan Zee, maar de richting valt in de **250°-280°-neutrale zone** → geen duidelijk piervoordeel. Bij deze windkracht sowieso geen bruikbare sessie.
- Golven: 0,86-1,16m / 5,4-5,8s, geleidelijk afbouwend.
- Getij: laagwater 00:20 (0,32m), hoogwater 04:36 (2,28m), laagwater 12:32 (0,47m), hoogwater 16:55 (2,29m), laagwater 21:03 (0,94m, opnieuw verhoogd).
- Bronnen: **KNMI en Soarcast eens over zwakke wind** (hoog vertrouwen); Windfinder/GFS iets hoger maar leidt tot dezelfde praktische conclusie.

### Donderdag — Slecht (te weinig wind, hele dag)
- Bij **Zandvoort/Wijk aan Zee**: zowel **KNMI** (beschikbaar tot 15:00) als **Windfinder/GFS** voorspellen deze keer vrijwel hetzelfde: wind valt verder terug naar **1,1-7,2 kts gemiddeld**, met gust tot hoogstens **9,7-13,5 kts** — overtuigend Slecht (te weinig wind), zonder het gebruikelijke modelverschil. **Soarcast** (daglichturen) bevestigt dit nog sterker: slechts 1,1-3,3 kts, gust 2,2-4,4 kts. Richting draait van zuid/west (200-272°) 's ochtends naar oost/ONO (aflandig, ~107-133° in de outlook-data) richting de avond.
- Pier-logica: niet van toepassing — windrichting is op geen moment pal- of licht aanlandig voor IJmuiden/Wijk aan Zee.
- Golven: 0,14-0,74m / 4,5-5,3s — de zware swell van afgelopen weekend (zondag 25 okt: 2,3-3,25m) is nu volledig uitgedempt.
- Getij: laagwater 00:50 (0,33m), hoogwater 05:19 (2,2m), laagwater 13:12 (0,42m), hoogwater 17:36 (2,3m).
- Bronnen: **KNMI, Soarcast en Windfinder/GFS stemmen voor het eerst deze week alle drie overeen** → hoog vertrouwen dat dit een echt windstille dag wordt.

---

## 🔭 Kans op mooie sessies daarna (dag 4-9)
Windfinder (GFS, enige bron zo ver vooruit — let op: dit model heeft de afgelopen dagen structureel te hoge windsnelheden gegeven, dus lees onderstaande cijfers met extra terughoudendheid) voor **vrijdag 30 oktober t/m woensdag 4 november**:

- **Vrijdag 30 oktober t/m zondag 1 november (overdag)**: wind blijft zwak (3,7-9,0 kts), richting ONO/O (aflandig voor Zandvoort) → **Slecht**, geen bruikbaar venster. Dit is een forse neerwaartse bijstelling t.o.v. de vorige run (briefing 25 oktober), die voor zaterdag nog een opbouw naar 21 kts voorspelde — een duidelijk voorbeeld van hoe onzeker 4+ dagen vooruit is.
- **Zondag 1 november (avond)**: wind trekt aan naar 11,4-12,2 kts met gust tot 17,8-19,1 kts, richting draait naar west (256-266°, licht aanlandig) — een grensgeval tussen Matig en Goed(b), maar golf blijft heel klein (0,29-0,33m, ruim onder de 1,1m-drempel) → blijft **Matig/grensgeval**.
- **Maandag 2 november**: wind 8,2-10,5 kts (gust tot 16,9 kts), richting NNO (17-38°) — vlak bij de kustlijnhoek, dus side-shore. Golf blijft klein (0,41-0,49m) → **Matig**.
- **Dinsdag 3 november — beste dag**: vergelijkbaar beeld, wind 7,4-11,2 kts (piekgust 17,1 kts rond 19:00), side-shore richting (20-38°), golf nog steeds klein (0,29-0,43m) → **Matig**, met het breedste venster van bruikbare wind van de hele periode, vooral **13:00-22:00**.
- **Woensdag 4 november**: wind valt terug naar 5,7-7,6 kts → **Slecht**, geen bruikbaar venster.

**Beste dag: dinsdag 3 november**, met de nadruk dat dit hoogstens **Matig** is — geen van de zes outlook-dagen in deze (uitsluitend op GFS gebaseerde) run haalt de 14kts-ondergrens voor Goed/Optimaal. Kans: **laag** (zelfs de beste dag is een bescheiden side-shore-windje zonder golf, en gezien hoe drastisch deze outlook al is herzien t.o.v. de vorige run is er weinig vertrouwen in de exacte cijfers).
⚠️ Onzeker op 4+ dagen — check dichter bij de tijd opnieuw.

---
_Bronnen: Windfinder (GFS) · Soarcast (KNMI Harmonie) · windwaarnemingen.nl (KNMI, IJmuiden)_
