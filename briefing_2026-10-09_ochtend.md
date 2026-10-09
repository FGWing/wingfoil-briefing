# 🌊 Wingfoil-briefing Zandvoort–Wijk aan Zee
_09-10-2026 · Ochtendbriefing_

⚠️ **Technische kanttekening:** Soarcast blijft onbereikbaar (pure JS/Vite-app onder `/web/assets/`, geen server-rendered data, geen vindbaar API-pad in de gebundelde JS — opnieuw gecontroleerd deze run). Windfinder is via de onderliggende paginadata opgehaald: de reguliere forecast-pagina bevat in dezelfde payload zowel 3-uurs data tot en met 18 oktober (dag 1 t/m 9) als — op de Superforecast-pagina — uurdata voor de eerste 72 uur. windwaarnemingen.nl (IJmuiden) is via het onderliggende `vsp_vdg_wstats.php`-endpoint opgehaald (10-minuten-actuals + ingebed KNMI-uurmodel).

---

## ⚡ Snel overzicht
- **Vrijdag:** Optimaal bij Zandvoort/Wijk aan Zee (05:00-10:00, side-shore) — rest van de dag grotendeels Slecht (pal aanlandig, grote golf); bij IJmuiden Optimaal vanaf 21:00
- **Zaterdag:** Slecht bij Zandvoort/Wijk aan Zee (hele dag pal aanlandig, golf 1,9-2,3m) — Goed, grensgeval Optimaal bij IJmuiden vrijwel de hele dag
- **Zondag:** Slecht bij Zandvoort/Wijk aan Zee — Goed, grensgeval Optimaal bij IJmuiden tot ~14:00, daarna valt de wind geleidelijk weg
- **Beste dag in de 7 dagen erna:** dinsdag 13 oktober
_(De eerste 3 regels zijn altijd de eerstvolgende 3 volle dagen vanaf het moment van versturen.)_

---

## ⏰ Realitycheck vandaag

- Laatste actuele uren (windwaarnemingen.nl, IJmuiden, 06:00-07:10): **wind 12,4-17,6 kts gem (dip rond 06:30), gust 15,4-20,3 kts**, richting ZW→ZZW (228°→195°).
- Was voorspeld voor dezelfde uren: Windfinder (GFS, uurdata) 06h **227° 19,8/27,2 kts**, 07h **201° 18,6/28,8 kts**; KNMI-vsp (windwaarnemingen.nl, ingebedde modelrun) 06h **227° 13,9/19,4 kts**, 07h **192° 9,9/19,5 kts**.
- Conclusie: wind loopt **ACHTER** op Windfinder — vooral de gust blijft duidelijk onder de voorspelling (15-20 kts actueel tegen 27-29 kts voorspeld), het gemiddelde ook een paar knopen lager. Tegenover het lokale KNMI-model (windwaarnemingen.nl) loopt de wind juist **licht VOOR tot conform** (gemiddelde iets hoger dan de 9,9-13,9 kts die dat model gaf, gust vergelijkbaar). Richting klopt bij alle bronnen goed. Rest-van-de-dag inschatting: **licht bijgesteld naar de voorzichtige kant** — het 05:00-10:00-venster blijft Optimaal (de 14-25 kts-ondergrens wordt gehaald en de side-shore richting is bevestigd), maar houd rekening met gemiddelde windsnelheden dichter bij 14-18 kts dan bij de 18-21 kts die Windfinder laat zien, en met gust-pieken die waarschijnlijk duidelijk lager uitvallen dan de voorspelde 28-34 kts.

---

## 📅 Komende 72 uur

### Vrijdag — Optimaal bij Zandvoort/Wijk aan Zee (05:00-10:00), daarna Slecht
- Bij **Zandvoort/Wijk aan Zee** (hoek resp. 287,5°/283,8°): **00:00-02:00** nog pal/licht aanlandig met matige wind (13-14 kts) en golf 1,4-1,5m → grensgeval Matig/Slecht. **03:00-04:00** licht aanlandig, golf voldoet ruim → Goed, grensgeval Optimaal. **05:00-10:00**: richting draait naar 196-240° (ZW/ZZW) = **side-shore** → **Optimaal**: wind 18,3-20,7 kts gem, gust 23,7-34,2 kts (zie Realitycheck — gust waarschijnlijk zachter), golf 1,45-1,69m/5,4-6,5s. **11:00** terug naar licht aanlandig (grensgeval Optimaal). **12:00-18:00**: richting 255-268° = **pal aanlandig** met golf tot 2,1m → **Slecht** (geen pierbescherming, open strand). **19:00** kort grensgeval Optimaal (licht aanlandig). **20:00-23:00**: pal aanlandig (258-300°), golf 1,9-2,1m → **Slecht**.
- Bij **IJmuiden** (pierzone-hoek 150°/330°, pal aanlandig 240°): **01:00-06:00** pal aanlandig → Slecht. **07:00-09:00** licht aanlandig (196-202°), golf ruim over drempel → Goed, grensgeval Optimaal. **10:00-20:00** pal aanlandig (bij IJmuiden valt deze richting ongunstiger dan bij Zandvoort) → Slecht. **21:00-23:00**: richting 294-300° = **side-shore bij IJmuiden** → **Optimaal**: wind 19,3-23,8 kts, gust 26,6-33,4 kts, golf 1,9-2,0m/7,2s. Dit venster loopt door in de nacht naar zaterdag (zie onder).
- 🌊 Piervoorkeur: **12:00-20:00** valt de richting (255-268°) in de **neutrale pierzone (250-280°)** — geen van beide pieren biedt hier voordeel, vandaar Slecht bij zowel Zandvoort/WaZ als IJmuiden. Vanaf **21:00** (294-300° = NW) is **IJmuiden** beschut (Zuidpier breekt de NW-golfslag) — Zandvoort/WaZ blijven hier onbeschut.
- Golven (Windfinder, enige golfbron): 1,4-2,1m / 5,4-7,3s — ruim boven de 1,1m/5s-drempel vanaf 03:00.
- Getij: hoogwater ~03:27 (2,14 m), laagwater ~12:58 (0,34 m), hoogwater ~15:46 (1,90 m), laagwater ~23:34 (0,23 m).
- Bronnen: Windfinder enige bron met golfdata; windwaarnemingen.nl bevestigt richting goed voor de ochtenduren, loopt qua kracht iets achter (zie Realitycheck) → **wijkt licht af qua snelheid, eens over richting**. Soarcast niet bereikbaar.

### Zaterdag — Slecht bij Zandvoort/Wijk aan Zee, Goed/grensgeval Optimaal bij IJmuiden
- Bij **Zandvoort/Wijk aan Zee**: wind staat de **hele dag pal aanlandig** (richting 268-298°, WNW/W) met grote golf (1,86-2,33m / 7,0-7,9s, oplopend gedurende de dag) → **Slecht** de volle dag, geen bruikbaar venster.
- Bij **IJmuiden** (pierzone-hoek 150°/330°): **00:00-03:00** side-shore (288-298°, doorlopend vanaf vrijdagnacht) → **Optimaal**. **04:00-08:00** licht aanlandig (273-280°) maar golf ruim over drempel → Goed, grensgeval Optimaal. **09:00-11:00** pal aanlandig (268-269°) → Slecht. **12:00-21:00** licht aanlandig (270-286°) met golf 2,0-2,3m/7,2-7,8s → Goed, grensgeval Optimaal vrijwel de hele middag/avond. **22:00** side-shore (286°) → Optimaal. Wind blijft de hele dag stevig: 17,5-24,4 kts gem, gust 22,9-28,8 kts.
- 🌊 Piervoorkeur: **00:00-08:00 en 18:00-23:00** (richting >280°, NW) is **IJmuiden** beschut (Zuidpier). **09:00-17:00** (268-277°) valt in de **neutrale zone (250-280°)** — IJmuidens relatief betere lezing hier komt puur door de eigen kustlijnhoek (licht aanlandig i.p.v. pal aanlandig bij Zandvoort/WaZ), niet door pierbescherming.
- Golven (Windfinder, enige golfbron): 1,86-2,33m / 7,0-7,9s — fors, hele dag ruim over de drempel.
- Getij: hoogwater ~04:05 (2,16 m), laagwater ~12:00 (0,49 m), hoogwater ~16:25 (1,99 m), laagwater ~00:14 (0,26 m, nacht naar zondag).
- Bronnen: alleen Windfinder (golfdata); windwaarnemingen.nl gaat niet zo ver door om te vergelijken. Soarcast niet bereikbaar. Check dicht bij de tijd opnieuw voor IJmuiden — het is een lang grensgeval-venster dat met een kleine richtingsverschuiving kan kantelen.

### Zondag — Slecht bij Zandvoort/Wijk aan Zee, Goed/grensgeval Optimaal bij IJmuiden tot ~14:00
- Bij **Zandvoort/Wijk aan Zee**: wind staat tot ~14:00 **pal aanlandig** (richting 272-286°) met golf nog 1,7-2,3m → **Slecht**. Vanaf **15:00** valt de wind onder de 14 kts-drempel (13,1 kts dalend naar 7-8 kts) → **Slecht (te weinig wind)** voor de rest van de dag.
- Bij **IJmuiden**: **00:00** licht aanlandig (280°) → Goed, grensgeval Optimaal. **01:00** side-shore (285°) → Optimaal. **02:00-07:00** licht aanlandig (272-284°) → Goed, grensgeval Optimaal. **08:00** side-shore (286°) → Optimaal. **09:00-14:00** licht aanlandig (272-277°), wind zakt geleidelijk van 18,6 naar 15,7 kts maar blijft net binnen de 14-25 kts-band → Goed, grensgeval Optimaal. **Vanaf 15:00** valt de wind te zwak (13,1 kts → 7-8 kts om 17:00-20:00) → **Slecht (te weinig wind)**.
- 🌊 Piervoorkeur: richting schommelt rond de grens van de **neutrale zone (250-280°)**, met korte pieken net over 280° (01:00, 05:00, 07:00-08:00) waarbij **IJmuiden** kort Zuidpier-voordeel krijgt; de rest van de ochtend is het vooral de eigen kustlijnhoek die IJmuiden gunstiger laat uitlezen dan Zandvoort/WaZ.
- Golven (Windfinder): 1,75-2,32m/7,1-8,0s in de ochtend, geleidelijk afnemend naar 1,2-1,6m/6,8-7,0s in de namiddag.
- Getij: hoogwater ~04:43 (2,16 m), laagwater ~12:34 (0,52 m), hoogwater ~17:02 (2,07 m), laagwater ~00:56 (0,28 m, nacht naar maandag).
- Bronnen: alleen Windfinder; windwaarnemingen.nl en Soarcast gaan niet zo ver door/niet bereikbaar. **Check dicht bij de tijd opnieuw** — het middaguur waarop de wind wegvalt is in dit soort GFS-runs nog onzeker.

---

## 🔭 Kans op mooie sessies daarna (dag 4-9)
Windfinder (GFS, enige bron zo ver vooruit, 3-uurs resolutie) voor **maandag 12 t/m zaterdag 17 oktober**:

- **Maandag 12 oktober**: zwakke, zuid/zuidzuidoostelijke wind (6,9-14,1 kts) en kleine golf (0,68-0,93m, onder de drempel) → **Slecht tot Matig**, met een kort beter moment rond 11:00-17:00 (Matig, wind ~11-14 kts) maar golf blijft te klein.
- **Dinsdag 13 oktober — beste dag**: wind draait zuid/zuidzuidwest/zuidwest (151-242°) en blijft de **vrijwel hele dag side-shore bij Zandvoort**, met golf die net over de drempel komt (1,11-1,36m/6,0-6,5s vanaf 05:00) → **Optimaal 05:00-17:00**: wind 14,1-15,3 kts gem, gust 22,7-26,1 kts. Vanaf 20:00 draait de richting naar NW/pal aanlandig → Slecht.
- **Woensdag 14 oktober**: wind valt grotendeels weg of is wisselvallig (1,7-12,7 kts), golf net onder de drempel (0,86-1,08m) → **Slecht tot Matig**, geen goed venster.
- **Donderdag 15 oktober**: 's ochtends (02:00-11:00) zuidwestelijke wind (218-226°), side-shore bij Zandvoort, golf 1,11-1,32m/5,9-6,0s → **Optimaal**: wind 14,7-18,4 kts, gust 23,5-27,2 kts. Vanaf 14:00 draait de wind naar NW/pal aanlandig bij Zandvoort → Slecht daar, maar bij **IJmuiden** juist side-shore vanaf 14:00 (301-302°) → Optimaal (wind 18,6-18,8 kts, gust 22,2-23,1 kts).
- **Vrijdag 16 oktober**: wind blijft westelijk (275-311°) — pal aanlandig bij Zandvoort (golf 1,12-1,19m, net over de drempel) → **Slecht**. Bij **IJmuiden** leest dezelfde richting als licht aanlandig/side-shore → **Goed, grensgeval Optimaal** vrijwel de hele dag (02:00-17:00), wind 14,2-15,8 kts, gust 14,8-18,5 kts (rustiger dan de dagen ervoor).
- **Zaterdag 17 oktober**: wind te zwak en wisselvallig van richting (6,7-10,8 kts) → **Slecht**.

**Beste dag: dinsdag 13 oktober**, met een lang Optimaal-venster (05:00-17:00) bij Zandvoort zelf — geen pier-afhankelijkheid nodig. Kans: **gemiddeld tot hoog** — het signaal is consistent over 12+ uur, maar de golfhoogte ligt net over de drempel (1,1-1,4m) en het gemiddelde windcijfer aan de onderkant van de Optimaal-band, dus een kleine modelbijstelling kan het naar Goed(a) laten kantelen. **Donderdag 15 oktober** (ochtend bij Zandvoort, middag bij IJmuiden) is een goede tweede kans.
⚠️ Onzeker op 4+ dagen — check dichter bij de tijd opnieuw.

---
_Bronnen: Windfinder (GFS) · windwaarnemingen.nl (KNMI, IJmuiden) · Soarcast — deze run niet bereikbaar (JS-app, geen vindbaar/bereikbaar API-adres)_
