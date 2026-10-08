# 🌊 Wingfoil-briefing Zandvoort–Wijk aan Zee
_08-10-2026 · Ochtendbriefing_

⚠️ **Technische kanttekening deze run:** Soarcast is (net als alle voorgaande runs) niet bereikbaar — pure JS-app (Vite-bundle onder `/web/assets/`), geen server-rendered data en geen vindbaar API-pad. Windfinder is via de onderliggende paginadata opgehaald — één bezoek aan de reguliere forecast-pagina leverde zowel de korte termijn (3-uurs, vandaag+morgen, component `ForecastSection`) als de 3-uurs data t/m 17 oktober (component `ForecastDataInit`) in dezelfde payload, dus geen apart bezoek aan de Superforecast-pagina nodig. windwaarnemingen.nl (IJmuiden) is via de onderliggende `vsp_vdg_wstats.php`-endpoint opgehaald: 10-minuten-actuals tot nu + het ingebedde KNMI-uurmodel (vsp) voor de rest van vandaag.

---

## ⚡ Snel overzicht
- **Donderdag:** Optimaal bij IJmuiden (02:00-23:00, side-shore) — Zandvoort/Wijk aan Zee ook Optimaal tot 17:00, draaien daarna pal aanlandig
- **Vrijdag:** Optimaal vroeg (05:00-08:00) ⚠️ extreme gust tot 31 kts, daarna grensgeval/Slecht
- **Zaterdag:** Slecht bij Zandvoort/Wijk aan Zee (pal aanlandig, grote golf) — Goed/grensgeval Optimaal bij IJmuiden (hele dag)
- **Beste dag in de 7 dagen erna:** zondag 11 oktober
_(De eerste 3 regels zijn altijd de eerstvolgende 3 volle dagen vanaf het moment van versturen.)_

---

## ⏰ Realitycheck vandaag

- Laatste actuele uren (windwaarnemingen.nl, IJmuiden, 05:00-07:10): **wind 13,2-15,4 kts gem, gust 16,5-18,3 kts**, richting noord/noordnoordwest (338-359°).
- Was voorspeld voor dezelfde uren: Windfinder (GFS, 3-uurs) 05h **333° 20/23 kts**, 08h **347° 22/25 kts**; KNMI-vsp (windwaarnemingen.nl, huidige modelrun) 05:00 **334° NNW 9,0/15,1 kts**, 06:00 **343° NNW 12,9/20,1 kts**, 07:00 **341° NNW 13,2/18,9 kts**.
- Conclusie: wind loopt **ACHTER** op Windfinder (actuele 13,2-15,4 kts duidelijk onder de 20-22 kts die Windfinder voor deze uren voorspelde), maar **conform tot licht VOOR** op KNMI-vsp (vsp bouwt van 9,0 naar 13,2 kts op, actueel ligt daar gelijk met of iets boven). Richting klopt bij alle drie goed (noord/NNW, 333-359°). Rest-van-de-dag inschatting: **licht bijgesteld** — de Optimaal-bij-IJmuiden-classificatie blijft staan (de 14-25 kts-drempel wordt al ruim gehaald en de side-shore richting is bevestigd), maar houd rekening met windsnelheden die dichter bij de onderkant van de Windfinder-range uitvallen dan bij de bovenkant.

---

## 📅 Komende 72 uur

### Donderdag — Optimaal bij IJmuiden
- Bij **IJmuiden** (pierzone-hoek 150°/330°): wind blijft de **hele dag side-shore** (richting 289-347°, N/NNW/WNW) → **Optimaal** de volle dag: wind 15-22 kts gem, gust 17-25 kts, golf 1,4-1,9 m / 7 s. Beste venster: **02:00-23:00**.
- Bij **Zandvoort/Wijk aan Zee**: zelfde richting leest hier tot ~14:00 ook nog side-shore/grensgeval-licht-aanlandig → **Optimaal**. Vanaf **17:00** (323°) grensgeval Optimaal/Goed (licht aanlandig, golf nog ruim over de drempel), en vanaf **20:00** (307°, 23:00 289°) **pal aanlandig** met golf 1,4-1,5 m → **Slecht** zonder pierbescherming.
- 🌊 Piervoorkeur: vanaf **20:00** (richting 289-307° = NW) is **IJmuiden** rustiger (Zuidpier breekt de NW-golfslag/-wind) — Wijk aan Zee ligt bij deze richting onbeschut, net als Zandvoort.
- Golven (Windfinder, enige golfbron): 1,4-1,9 m / 7 s — hele dag ruim over de 1,1 m/5 s-drempel.
- Getij: hoogwater ~02:44 (2,07 m), laagwater ~11:41 (0,34 m), hoogwater ~15:03 (1,78 m), laagwater ~22:51 (0,23 m).
- Bronnen: Windfinder enige bron met golfdata; windwaarnemingen.nl (KNMI-vsp + actuals) bevestigt richting goed, loopt qua kracht iets achter op Windfinder (zie Realitycheck) → **wijkt licht af qua snelheid, eens over richting**. Soarcast niet bereikbaar.

### Vrijdag — Optimaal vroeg, daarna grensgeval/Slecht ⚠️ zeer grillig
- Vroeg op de dag (**05:00-08:00**) een krachtig en goed venster: wind 19-21 kts gem, **gust pieken tot 31 kts** (!), richting 202-235° (zuid/zuidwest, side-shore bij Zandvoort en Wijk aan Zee) → **Optimaal**, golf 1,3-1,5 m / 6-7 s. Dit is stormachtig en met die gustpieken niet voor iedereen comfortabel.
- Vanaf **11:00 t/m 20:00** draait de wind naar 252-256° (west-zuidwest). Bij **Zandvoort** is dit nog net **licht aanlandig** (grensgeval met Optimaal, want golf 1,7-2,0 m/6-7 s blijft ruim over de drempel) → **Goed, grensgeval Optimaal**. Bij **IJmuiden en Wijk aan Zee** valt deze richting echter wél in hun eigen volle aanlandig-band → **Slecht** daar (grote golf, geen pierbescherming — zie piervoorkeur). Extreme gust blijft de hele periode: 30-32 kts.
- Om **23:00** draait de wind door naar 293° (NW) en wordt ook bij Zandvoort/Wijk aan Zee **pal aanlandig** → **Slecht**, maar IJmuiden krijgt dan weer pierbescherming (zie hieronder).
- 🌊 Piervoorkeur: **02:00-08:00** (richting 202-235° = zuid/zuidwest) is **Wijk aan Zee** beschut (Noordpier breekt de zuid(west)-golfslag). **11:00-20:00** (252-256°) valt in de **neutrale zone tussen de twee pierassen (250-280°)** — geen van beide pieren biedt hier voordeel, en juist in dit venster lezen IJmuiden/Wijk aan Zee door hun eigen hoek slechter (pal aanlandig) dan Zandvoort (nog licht aanlandig). Vanaf **23:00** (293° = NW) is **IJmuiden** weer beschut (Zuidpier).
- Golven (Windfinder): 1,3-2,0 m / 6-7 s — ruim boven de drempel de hele dag.
- Getij: hoogwater ~03:27 (2,14 m), laagwater ~12:58 (0,34 m), hoogwater ~15:46 (1,90 m), laagwater ~23:34 (0,23 m).
- Bronnen: alleen Windfinder (golfdata); windwaarnemingen.nl loopt voor deze dag niet ver genoeg door om te kunnen vergelijken. Soarcast niet bereikbaar. **Check dicht bij de tijd opnieuw** — de combinatie van extreme gust en een grillige richtingsdraai (bovendien iets anders dan de inschatting van gisteren) maakt dit een onzekere dag.

### Zaterdag — Slecht bij Zandvoort/Wijk aan Zee, Goed bij IJmuiden
- Bij **Zandvoort en Wijk aan Zee**: wind staat de **hele dag pal aanlandig** (richting 273-287°, WNW) met grote golf (1,8-2,0 m / 7 s) en voor het grootste deel van de dag (05:00-20:00, richting 273-276°) in de **neutrale pierzone (250-280°)** — geen pierbescherming → **Slecht** vrijwel de hele dag. Alleen rond 02:00 en 23:00 (287°) schuift de richting net naar de IJmuiden-kant.
- Bij **IJmuiden** (pierzone-hoek 150°/330°) leest dezelfde richting als **licht aanlandig** (273-276°, 05:00-20:00) tot **side-shore** (287° om 02:00 en 23:00) — dankzij de golf die ruim over de drempel blijft (1,8-2,0 m/7 s) is dit een grensgeval tussen Optimaal en Goed de hele dag, met echte **Optimaal**-momenten rond 02:00 en 23:00. Wind: 18,5-23,1 kts gem, gust 21,4-28,2 kts — stevig.
- 🌊 Piervoorkeur: vrijwel de hele dag (05:00-20:00) **neutrale zone (250-280°)** — IJmuidens voordeel komt hier puur door de eigen kustlijnhoek, niet door pierbescherming. Pas rond 02:00/23:00 (287°) krijgt **IJmuiden** ook echt Zuidpier-bescherming.
- Golven (Windfinder, enige golfbron): 1,77-2,02 m / 6,9-7,3 s.
- Getij: hoogwater ~04:05 (2,16 m), laagwater ~12:00 (0,49 m), hoogwater ~16:25 (1,99 m), laagwater ~00:14 (0,26 m, nacht naar zondag).
- Bronnen: alleen Windfinder (golfdata); richting/kracht intern consistent over de dag. windwaarnemingen.nl gaat niet zo ver door, Soarcast niet bereikbaar.

---

## 🔭 Kans op mooie sessies daarna (dag 4-9)
Windfinder (GFS, enige bron zo ver vooruit — in dezelfde payload als de korte termijn opgehaald, t/m 17 oktober) voor **zondag 11 t/m vrijdag 16 oktober**:

- **Zondag 11 oktober — beste dag**: wind staat de hele dag **pal aanlandig tot licht aanlandig bij Zandvoort/Wijk aan Zee** (270-308°, grotendeels in de **neutrale pierzone 250-280°** tot 14:00 → geen pierbescherming, en daar dus **Slecht** bij Zandvoort/Wijk aan Zee). Bij **IJmuiden** leest dezelfde richting gunstiger door de eigen hoek: licht aanlandig (grensgeval Optimaal/Goed, golf 1,7-2,1 m ruim over de drempel) tot 14:00, en vanaf **17:00-20:00** draait het naar 290-308° (NW) — dan **side-shore bij IJmuiden** mét Zuidpier-bescherming → **Optimaal**: wind 17,5-21,4 kts gem, gust 21,9-24,8 kts, golf 1,42-1,58 m / 7,1-7,2 s. Na 20:00 valt de wind snel terug (13,9 kts om 23:00) naar **Goed(b)**.
- **Maandag 12 oktober**: wind valt grotendeels weg (0,4-13,0 kts, wisselvallige richting) → **Slecht**.
- **Dinsdag 13 oktober**: matige, wisselvallige zuid/zuidzuidoostelijke wind (10-13 kts gem, gust tot 21 kts) maar golf blijft onder de 1,1 m-drempel (0,53-0,99 m) → **Matig**, net niet genoeg golf voor meer.
- **Woensdag 14 oktober**: vergelijkbaar, iets zwakker (zuid, 5-12,5 kts gem), golf 0,59-0,93 m → **Matig tot Slecht**.
- **Donderdag 15 oktober**: zwak en wisselvallig van richting (2-11,7 kts gem), golf 0,6-0,84 m → **Slecht**.
- **Vrijdag 16 oktober**: wind draait naar noord/noordnoordoost (344-22°) — dat is **side-shore bij Zandvoort** de vrijwel hele dag (05:00-23:00), wind 13-22 kts gem (gust tot 26 kts, met een piek van 22 kts gem rond 05:00), golf **net onder** de 1,1 m-drempel (0,9-1,08 m / 5,2-5,9 s) → **Goed, grensgeval Optimaal** voor een lang venster — qua richting en wind net zo kansrijk als zondag, alleen de golf blijft net iets te klein voor de volle Optimaal-classificatie.

**Beste dag: zondag 11 oktober**, met name **17:00-20:00 bij IJmuiden** (side-shore, Zuidpier-bescherming, krachtige langeperiode swell). Kans: **hoog** voor dat venster — het signaal is consistent over meerdere uren — al ligt de dag nog 3-4 dagen vooruit. **Vrijdag 16 oktober** is een goede tweede kans (langer venster, iets minder golf).
⚠️ Onzeker op 4+ dagen — check dichter bij de tijd opnieuw.

---
_Bronnen: Windfinder (GFS) · windwaarnemingen.nl (KNMI, IJmuiden) · Soarcast — deze run niet bereikbaar (JS-app, geen vindbaar/bereikbaar API-adres)_
