# 🌊 Wingfoil-briefing Zandvoort–Wijk aan Zee
_11-10-2026 · Ochtendbriefing_

⚠️ **Technische kanttekening:** Soarcast blijft onbereikbaar deze run (pure JS/Vite-app, geen server-rendered data, geen bruikbaar API-pad gevonden — net als alle voorgaande runs). Windfinder is via de onderliggende paginadata (Astro-island props) opgehaald: de reguliere forecast-pagina + de Superforecast-pagina leveren samen uurdata voor vandaag t/m dinsdag en 3-uurs data t/m 20 oktober (dag 1 t/m 10). windwaarnemingen.nl (IJmuiden) is via de onderliggende `database/vsp_vdg_wstats.php` (vandaag, 10-minuten-actuals + ingebed KNMI-uurmodel) en `vsp_mrg_wstats.php` (morgen+overmorgen, KNMI-uurmodel) opgehaald.

---

## ⚡ Snel overzicht
- **Zondag:** Slecht bij Zandvoort/Wijk aan Zee (hele dag pal aanlandig, golf 1,1-2,2m) — Optimaal bij IJmuiden (08:00-16:00)
- **Maandag:** Slecht tot Matig bij alle plekken — wind vrijwel de hele dag te zwak (3,9-9,7 kts), iets beter 19:00-23:00 (Matig, grensgeval)
- **Dinsdag:** Goed, grensgeval Optimaal bij Zandvoort (11:00-20:00, piek ~17:00)
- **Beste dag in de 7 dagen erna:** zaterdag 17 oktober
_(De eerste 3 regels zijn altijd de eerstvolgende 3 volle dagen vanaf het moment van versturen.)_

---

## ⏰ Realitycheck vandaag

- Laatste actuele uren (windwaarnemingen.nl, IJmuiden, 05:00-07:10): **wind 12,6-13,7 kts gem (uurgemiddelden 13,7 / 13,2 / 12,6 kts), gust 15,6-18,4 kts**, richting West/WNW (263-304°, enigszins schommelend maar geen duidelijke drift).
- Was voorspeld voor dezelfde uren: het ingebedde KNMI-uurmodel (windwaarnemingen.nl zelf) gaf 05h-07h **277-320°, 10,3-13,1 kts, gust 17,8-20,3 kts**; Windfinder (GFS) gaf voor diezelfde uren **276-281°, 22,3-22,6 kts, gust 25,6-27,7 kts**.
- Conclusie: de wind loopt **conform tot licht VOOR** op het lokale KNMI-model (13-13,7 kts actueel tegen 10,3-13,1 kts voorspeld, al is de gust juist iets lager dan voorspeld), maar duidelijk **ACHTER** op Windfinder/GFS (12,6-13,7 kts actueel tegen 22-23 kts voorspeld — bijna de helft lager). Richting klopt bij beide bronnen goed (West/WNW). Rest-van-de-dag inschatting: **licht bijgesteld naar de voorzichtige kant** voor de wind-snelheid bij IJmuiden. De classificatie Optimaal (08:00-16:00) steunt vooral op de richting (side-shore) en de golf (1,6-2,1m, ruim boven de drempel) — die blijven overeind — maar houd er rekening mee dat de werkelijke gemiddelde windsnelheid dichter bij 13-16 kts kan liggen dan bij de 18-20 kts die Windfinder voor de ochtend/vroege middag laat zien. Richting het begin van de middag (als Windfinder nog altijd ruim boven de 14 kts-drempel blijft) is de marge het grootst, dus dat deel van het venster is het meest betrouwbaar.

---

## 📅 Komende 72 uur

### Zondag — Slecht bij Zandvoort/Wijk aan Zee, Optimaal bij IJmuiden
- Bij **Zandvoort/Wijk aan Zee** (hoek resp. 287,5°/283,8°): wind staat de **hele dag pal aanlandig** (richting 263-302°, West/WNW) met grote golf (1,1-2,2m / 6,5-7,9s, hoog aan het begin van de dag, afnemend naar de avond) → **Slecht** de volle dag — grote branding, geen pierbescherming. Vanaf **~17:00** valt de wind bovendien onder de 14 kts-drempel (13,0 kts dalend naar 10,0 kts om 23:00) → **Slecht (te weinig wind)** voor de rest van de avond.
- Bij **IJmuiden** (pierzone-hoek 150°/330°, pal aanlandig 240°): dezelfde richting leest hier anders. **00:00-07:00**: richting 271-281° is **licht aanlandig** bij IJmuiden, met wind 20,4-22,6 kts en golf ruim over de drempel (2,1-2,2m/7,6-7,9s) → **Goed, grensgeval Optimaal** (richting net niet ideaal, wind/golf ruim voldoende) — **let op: dit venster is al (grotendeels) voorbij en viel samen met de periode die in de Realitycheck duidelijk zwakker uitpakte dan voorspeld**. **08:00-16:00**: richting draait naar **286-302°** = **side-shore bij IJmuiden** → **Optimaal**: wind 14,5-20,2 kts (dalend), gust 15,9-24,9 kts, golf 1,6-2,1m/7,0-7,6s — zie Realitycheck voor een kanttekening bij de exacte windsnelheid, vooral in het eerste deel van dit venster. **Vanaf ~17:00** valt de wind te zwak (13,0 kts → 10,0 kts om 23:00) → **Slecht (te weinig wind)**.
- 🌊 Piervoorkeur: **00:00-07:00** valt de richting (271-281°) grotendeels in de **neutrale pierzone (250-280°)** — geen duidelijk pier-voordeel, IJmuidens betere klasse komt hier vooral door de eigen kustlijnhoek. **Vanaf 08:00** (richting 286-302°, boven 280°) krijgt **IJmuiden** een Zuidpier-voordeel — dit valt samen met de side-shore-lezing, dus een dubbel voordeel tijdens het beste venster.
- Golven (Windfinder, enige golfbron): 2,2m/7,9s dalend naar 1,1m/6,5s aan het einde van de dag.
- Getij: laagwater ~00:14 (0,26 m), hoogwater ~04:43 (2,16 m), laagwater ~12:34 (0,52 m), hoogwater ~17:02 (2,07 m).
- Bronnen: Windfinder enige bron met golfdata; windwaarnemingen.nl bevestigt richting goed, loopt qua windkracht duidelijk achter op Windfinder (zie Realitycheck) → **wijkt af qua snelheid, eens over richting**. Soarcast niet bereikbaar.

### Maandag — Slecht tot Matig bij alle plekken
- Bij **Zandvoort/Wijk aan Zee**: wind begint zwak en pal aanlandig (278-298°, 00:00-04:00, 3,9-8,5 kts) → Slecht. **05:00-18:00** draait de richting via licht aanlandig/zuid naar **side-shore** (172-190°), maar de wind blijft het grootste deel van de dag te zwak (5,2-9,5 kts) en de golf ruim onder de drempel (0,46-0,75m) → **Slecht**. Vanaf **19:00** trekt de wind iets aan (9,3-13,0 kts, gust 14,2-24,4 kts) bij licht aflandige/side-shore richting (144-153°) → **Matig**, met een grensgeval richting iets beters rond 22:00-23:00 (gust 22-24 kts) al blijft de gemiddelde windsnelheid net onder de 14 kts-grens.
- Bij **IJmuiden** (pierzone-hoek): vergelijkbaar patroon — vroeg zwak/pal aanlandig (Slecht), overdag side-shore maar te zwak (Slecht), 's avonds oplopend naar Matig bij dezelfde richting.
- 🌊 Piervoorkeur: kort relevant **00:00-03:00** (richting 291-298° is bij Wijk aan Zee pal aanlandig, golf 0,90-1,06m ≥0,8m) → IJmuiden (Zuidpier) zou dan rustiger zijn, maar de wind is op dat moment zo zwak (5,6-8,5 kts) dat dit praktisch niet relevant is. Verder op de dag geen pier-effect van betekenis (golf onder 0,8m of richting niet aanlandig).
- Golven (Windfinder): 0,46-1,06m / 5,0-6,5s — de hele dag onder de 1,1m-drempel.
- Getij: laagwater ~00:56 (0,28 m), hoogwater ~05:20 (2,14 m), laagwater ~13:17 (0,49 m), hoogwater ~17:38 (2,13 m).
- Bronnen: Windfinder + windwaarnemingen.nl (KNMI-uurmodel) voor richting/snelheid, komen goed overeen in trend (zwak, draaiend naar zuid). Soarcast niet bereikbaar. Check dicht bij de tijd opnieuw voor de exacte avondwaarden.

### Dinsdag — Goed, grensgeval Optimaal bij Zandvoort
- Bij **Zandvoort/Wijk aan Zee**: **00:00-10:00** side-shore (richting 150-190°, zuid), wind 11,7-13,9 kts, gust 18,8-25,5 kts, golf nog onder de drempel (0,56-0,77m) → **Matig, grensgeval naar Goed** (richting en wind bijna goed, golf nog te laag). **11:00-16:00**: wind blijft rond 12,4-13,9 kts (net onder de 14 kts-grens), golf loopt op naar 0,79-1,03m (nadert de drempel), richting nog side-shore (186-206°) → **grensgeval Matig/Goed** — wind net iets te zwak voor Goed(a)/Optimaal, golf net te laag voor Goed(b). **Om 17:00** komt de golf net over de drempel (1,10m/5,8s) bij wind 15,4 kts en nog side-shore richting (221°) → **Optimaal** (kort). **18:00-20:00**: richting draait naar **pal aanlandig** (264-311°) bij Zandvoort/Wijk aan Zee met golf net onder/op de grens (1,08-1,09m) → **grensgeval Slecht/Matig**. **Om 23:00**: wind valt terug naar 10,8 kts, golf 1,02m, richting 321° (licht aanlandig) → **Matig**.
- Bij **IJmuiden** (pierzone-hoek): overdag (11:00-16:00, richting 187-206°) leest als **licht aanlandig** bij IJmuiden — iets minder gunstig dan Zandvoorts side-shore-lezing in dezelfde periode. Vanaf 17:00-20:00 draait de richting (221-311°) bij IJmuiden juist naar side-shore.
- 🌊 Piervoorkeur: **13:00-16:00** is de richting bij IJmuiden licht aanlandig met golf 0,83-1,03m (≥0,8m) → **Wijk aan Zee (Noordpier)** zou dan rustiger zijn als keuze tussen die twee, maar **Zandvoort zelf blijft de betere optie** in dat venster (side-shore i.p.v. licht aanlandig). **Om 20:00** (richting 311°, NW) krijgt **IJmuiden (Zuidpier)** kort een voordeel, maar dat is laat op de avond.
- Golven (Windfinder): 0,56-1,10m / 5,2-5,8s — pas aan het einde van de middag over de 1,1m-drempel.
- Getij: laagwater ~01:43 (0,29 m), hoogwater ~05:57 (2,11 m), laagwater ~14:04 (0,43 m), hoogwater ~18:13 (2,17 m).
- Bronnen: alleen Windfinder gaat dit ver door met golfdata; windwaarnemingen.nl stopt na morgen. Dit venster leunt sterk op het model op 2 dagen vooruit — **check dicht bij de tijd opnieuw**, vooral of de golf inderdaad de 1,1m-drempel haalt in de namiddag.

---

## 🔭 Kans op mooie sessies daarna (dag 4-9)
Windfinder (GFS, enige bron zo ver vooruit, 3-uurs resolutie) voor **woensdag 14 t/m maandag 19 oktober**:

- **Woensdag 14 oktober**: wind zeer zwak (2,4-11,1 kts) en wisselvallig van richting (NW→WZW→zuid) → **Slecht**, geen bruikbaar venster.
- **Donderdag 15 oktober**: wind blijft zwak (7,4-9,7 kts), richting side-shore/zuid (153-176°) — goede hoek, maar te weinig kracht → **Slecht**.
- **Vrijdag 16 oktober**: ochtend zwak en wisselvallig (kort pal aanlandig, 317° om 11:00, 8,6 kts), maar **vanaf 14:00** trekt de wind sterk aan (18,7-20,8 kts) bij noordelijke/side-shore richting (339-358°) en golf over de drempel (1,14-1,28m/5,5-6,3s) → **Optimaal vanaf 14:00 tot einde dag**.
- **Zaterdag 17 oktober — beste dag**: de Optimaal-periode zet door de **hele ochtend en middag** (00:00-14:00, richting 1-17° (noord), side-shore, wind 15,0-18,4 kts, golf 1,03-1,23m/6,2-6,5s). Vanaf **17:00** zakt het naar een grensgeval en vanaf 20:00 naar **Matig** (wind 13,9-15,0 kts). Dit is in feite één lange aaneengesloten Optimaal-periode die al vrijdagmiddag begint en tot zaterdagmiddag/vroege avond doorloopt (~24 uur).
- **Zondag 18 oktober**: wind draait naar oost/aflandig (70-91°) en wordt zwak (5,5-10,7 kts) → **Slecht**, grensgeval Matig pas laat in de avond (23:00).
- **Maandag 19 oktober**: wind blijft zwak en wisselvallig (2,9-9,6 kts), richting draait van aflandig naar side-shore naar pal aanlandig → **Slecht**.

**Beste dag: zaterdag 17 oktober**, met een lange Optimaal-periode (00:00-14:00+) bij Zandvoort zelf — geen pier-afhankelijkheid nodig, en onderdeel van een nog langere window die al vrijdagmiddag begint. Kans: **gemiddeld tot hoog** — twee aaneensluitende dagen met consistent signaal (noordelijke wind, golf ruim over de drempel) maakt dit robuuster dan een losse dag, maar op 6 dagen vooruit kan de exacte timing nog verschuiven.
⚠️ Onzeker op 4+ dagen — check dichter bij de tijd opnieuw.

---
_Bronnen: Windfinder (GFS) · windwaarnemingen.nl (KNMI, IJmuiden) · Soarcast — deze run niet bereikbaar (JS-app, geen vindbaar/bereikbaar API-adres)_
