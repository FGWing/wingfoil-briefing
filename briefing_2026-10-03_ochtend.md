# 🌊 Wingfoil-briefing Zandvoort–Wijk aan Zee
_03-10-2026 · Ochtendbriefing_

⚠️ **Technische kanttekening deze run:** Soarcast is (net als alle voorgaande runs) niet bereikbaar — een volledige JS-app zonder vindbaar/bereikbaar API-adres of statisch gerenderde data. Windfinder is via de onderliggende paginadata (astro-hydration props op de forecast-pagina) opgehaald — één bezoek leverde zowel de korte termijn (3-uurs) als de volledige 3-uurs data t/m 12 oktober in dezelfde payload (geen apart bezoek aan de Superforecast-pagina nodig). windwaarnemingen.nl (IJmuiden) is via de onderliggende vsp-JSON-endpoints opgehaald: 10-minuten-actuals + het ingebedde KNMI-uurmodel voor vandaag, en het KNMI-uurmodel voor morgen/overmorgen (tot 16:00).

---

## ⚡ Snel overzicht
- **Zaterdag:** Slecht
- **Zondag:** Slecht
- **Maandag:** Slecht (KNMI-vsp wijst op mogelijk iets meer wind in de middag dan Windfinder/GFS — zie toelichting; golf blijft hoe dan ook ruim onder de drempel)
- **Beste dag in de 7 dagen erna:** vrijdag 9 oktober

---

## ⏰ Realitycheck vandaag

- Laatste actuele uren (windwaarnemingen.nl, IJmuiden, 05:00-07:10): **wind 6,8-9,2 kts gem, gust 8,1-11,8 kts, richting vrij stabiel zuid tot zuidzuidoost (149-166°)**.
- Was voorspeld voor dezelfde uren (KNMI-vsp, huidige modelrun): **05:00 149° ZZO, 4,0/5,7 → 7,8/11,1 kts**; **06:00 154° ZZO, 3,8/5,8 → 7,4/11,3 kts**; **07:00 161° ZZO, 4,0/5,9 → 7,8/11,5 kts**. Windfinder (GFS, 3-uurs) zat voor hetzelfde blok op een vergelijkbare 6/8 kts.
- Conclusie: windkracht **klopt ongeveer, met een gemengd beeld** — om 05:00-06:00 lag de actuele gemiddelde wind ~1,5-1,8 kts boven de KNMI-vsp-voorspelling, maar om 07:00 juist duidelijk eronder (6,8 vs. 7,8 kts gem, en vooral de gust fors zwakker: 8,1 vs. 11,5 kts). Richting klopt goed overal (zuid/ZZO). Per saldo geen consistente over- of onderschatting aan te wijzen. Voor de rest van de dag: inschatting **ongewijzigd op Slecht** — zelfs met een optimistische opslag zoals om 05:00-06:00 (+~2 kts) blijft de modelpiek rond 12:00-13:00 (Windfinder 6 kts, KNMI-vsp 8,2/12,2 kts) ruim onder de Slecht-drempel, en de golf blijft de hele dag minimaal (0,2-0,3 m).

---

## 📅 Komende 72 uur

### Zaterdag — Slecht
- Windfinder (GFS, 3-uurs): hele dag zwak, 2-6 kts gem / 3-8 kts gust, richting draait van zuidzuidoost (164°) via zuidwest (248°) naar noordwest (309°) — nergens boven de Slecht-drempel.
- KNMI-vsp (uurmodel, dekt hele dag): bevestigt hetzelfde zwakke beeld, piek rond 12:00-13:00 van 8,2/12,2 kts (218-225°, ZW) — ook dit blijft ruim onder de Slecht-drempel. Beide bronnen zijn het dus eens.
- Golven (Windfinder, enige golfbron): 0,2-0,3 m / 4 s — ver onder de 1,1 m-drempel, geen Optimaal/Goed(b) mogelijk.
- 🌊 Piervoorkeur: niet van toepassing (golf <0,8 m).
- Getij: laagwater ~04:05 (0,3 m), hoogwater ~08:55 (1,8 m), laagwater ~16:43 (0,4 m), hoogwater ~21:14 (2,0 m).
- Bronnen: Windfinder en KNMI-vsp **eens** (Slecht), bevestigd door de Realitycheck hierboven. Soarcast niet bereikbaar.

### Zondag — Slecht
- Windfinder (GFS, 3-uurs): hele dag zeer zwak en onstabiel van richting — 2-6 kts gem / 3-6 kts gust, richting draait van noord (334°) via oost (94°, kort pal aflandig maar veel te zwak om relevant te zijn) naar west/zuidwest (257-283°) — nergens boven de Slecht-drempel.
- KNMI-vsp (uurmodel, dekt hele dag): ook hier een zwak en grillig beeld (wind vaak <3 kts, richting springt rond door de lichte windkracht) — consistent zwak met Windfinder, geen tegenstrijdig signaal van meer wind.
- Golven: 0,2-0,3 m / 4-5 s.
- 🌊 Piervoorkeur: niet van toepassing.
- Getij: laagwater ~05:02 (0,4 m), hoogwater ~10:13 (1,6 m), laagwater ~17:42 (0,4 m), hoogwater ~22:50 (1,8 m).
- Bronnen: Windfinder en KNMI-vsp **eens** — zwakke, windstille dag. Soarcast niet bereikbaar.

### Maandag — Slecht (grensgeval, zie model-divergentie)
- Windfinder (GFS, 3-uurs): 6,7-10,9 kts gem / 9,2-14,9 kts gust, richting zuidwest tot west-zuidwest (207-238°) — overal onder de Slecht-drempel (gust steeds <16 kts én gem <14 kts).
- KNMI-vsp (uurmodel, dekt tot 16:00): tekent een **duidelijk sterker beeld** voor de middag — 12:00 14,0/19,6 kts (230°, ZW), 13:00 13,6/19,6 kts (229°), 14:00 14,2/20,4 kts (232°) — dit ligt merkbaar boven Windfinder voor dezelfde uren. **Expliciete modeldivergentie, niet gemiddeld**: dit zou bij voldoende golf een grensgeval Matig/Goed(b) kunnen zijn, maar de golf (enige bron: Windfinder) blijft op dat moment maar 0,58 m / 4,3 s — ruim onder de 1,1 m-drempel, dus zelfs met de hogere KNMI-wind landt het hooguit op **Matig**, niet op Goed(b). Richting is side-shore bij Zandvoort (207-238°, >45° van pal aanlandig).
- Golven: 0,27-0,64 m / 4,3-4,8 s — ruim onder de drempel, ongeacht welk windmodel je volgt.
- 🌊 Piervoorkeur: niet van toepassing (golf <0,8 m).
- Getij: laagwater ~06:38 (0,5 m), hoogwater ~11:43 (1,5 m), laagwater ~19:02 (0,5 m), hoogwater ~00:26 volgende dag (1,9 m).
- Bronnen: Windfinder (GFS) en KNMI-vsp **wijken duidelijk af voor de middag** (±4-6 kts gem, ±5-6 kts gust) — vermeld expliciet i.p.v. gemiddeld; golfdata houdt de dag hoe dan ook op Slecht/hooguit Matig. Soarcast niet bereikbaar.

---

## 🔭 Kans op mooie sessies daarna (dag 4-9)
Windfinder (GFS, enige bron zo ver vooruit — in één keer t/m 12 oktober opgehaald) laat voor **dinsdag 6 t/m zondag 11 oktober** het volgende beeld zien:
- **Dinsdag 6 oktober**: zwak de hele dag, 3-9,7 kts gem (max gust 14,8 kts), richting draait van zuidzuidwest via west naar noord (206-349°) — overal **Slecht**. Golf 0,55-0,63 m.
- **Woensdag 7 oktober**: overwegend **Slecht** en zwak (5,4-6,4 kts) tot aan de avond, maar bouwt dan kort op — 20:00 al 17,0/19,0 kts (3°, noord, side-shore bij Zandvoort) — grensgeval Matig/Goed, golf blijft met 0,78 m/5,5 s net onder de Optimaal-drempel. Om 23:00 zakt het weer terug naar 11,3/15,3 kts (Slecht). Dit is vooral een signaal dat de wind richting donderdag aan het opbouwen is.
- **Donderdag 8 oktober**: bij **Zandvoort** komt de wind vrijwel de hele dag **pal aanlandig** te liggen (295-347°, WNW/NW) met golf die oploopt naar 1,0-1,5 m/5,7-7,3 s — dat is grote branding zonder pierbescherming, dus **Slecht bij Zandvoort**. Bij **IJmuiden** valt dezelfde richting dankzij de eigen pierzone-hoek (150°/330°) veel dichter bij side-shore, en de Zuidpier breekt de NW-golfslag: daar wisselen **Optimaal** (05:00 15,1/17,2 kts golf 1,16 m/5,7 s; 11:00 15,8/16,4 kts golf 1,43 m/6,4 s) en **Goed(b)** (08:00, 14:00, 17:00, telkens 12-14 kts met golf 1,3-1,5 m) elkaar af, tot de wind 's avonds wegvalt (20:00/23:00 Slecht). 🌊 **Piervoorkeur: IJmuiden rustiger** (NW-golfslag wordt door de Zuidpier gebroken).
- **Vrijdag 9 oktober — beste dag**: bij **Zandvoort** bouwt de wind overdag op van 8,9 naar 20,3 kts, richting zuid/zuidwest (194-239°) — dat is **side-shore** bij Zandvoort, en de golf loopt gelijk op naar 1,17-1,39 m / 6,5-7,2 s. Dit levert een breed, aaneengesloten **Optimaal-venster van ongeveer 11:00 tot 20:00** op (17,6-20,3 kts gem, gust 24,6-28,0 kts), zonder dat je afhankelijk bent van de pier — dit is de enige dag in de outlook met een stevig Optimaal-venster recht bij de hoofdspot Zandvoort zelf. Pas rond 23:00 draait de wind naar 262°, wat bij Zandvoort net pal aanlandig wordt (en bij IJmuiden in de neutrale zone tussen de twee pierassen valt, dus geen duidelijk piervoordeel) — dat late moment is minder interessant dan het middagvenster.
- **Zaterdag 10 oktober**: bij **Zandvoort** ligt de wind vrijwel de hele dag **pal aanlandig** (275-317°, W/WNW/NW) met golf 1,40-1,47 m/6,3-6,4 s — grote branding zonder pierbescherming, dus **Slecht bij Zandvoort**. Bij **IJmuiden** beschermt de Zuidpier tegen deze NW-golfslag en is de richting er licht aanlandig tot side-shore: **Optimaal/Goed(a)**, met zeer sterke wind (16,7-24,2 kts) die 's avonds fors aanwakkert (gust tot 29,4 kts om 20:00 — boven de 27 kts-drempel waarbij de Reddingsbrigade IJmuiden de pieren normaliter sluit voor wandelaars, een signaal dat het er ruig aan toe gaat). 🌊 Piervoorkeur: IJmuiden rustiger, maar met de kanttekening dat het laat op de dag pittig wordt.
- **Zondag 11 oktober**: vergelijkbaar met zaterdag maar nog krachtiger — bij **Zandvoort** weer pal/licht aanlandig (288-324°) met golf 1,45-1,59 m/6,5-7,3 s → **Slecht bij Zandvoort**. Bij **IJmuiden** is dezelfde richting dankzij de pierzone-hoek **side-shore**, en de Zuidpier beschermt: vrijwel de hele dag **Optimaal**, maar de wind is zeer fors (20,7-25,5 kts gem, gust 24,6-29,7 kts, meermaals boven de 27 kts-sluitingsdrempel van de Reddingsbrigade) — dit voelt eerder als een stormachtige/pittige dag dan een comfortabele sessie.

**Beste dag: vrijdag 9 oktober**, met name het venster **11:00-20:00 bij Zandvoort** — een breed Optimaal-venster (side-shore, wind 17,6-20,3 kts, golf >1,1 m met lange periode) recht bij de hoofdspot, zonder pier-afhankelijkheid en zonder extreme windkracht. Kans: **gemiddeld tot hoog** — het model laat al vanaf woensdagavond een consistente opbouw zien die logisch doorzet naar vrijdag, wat het vertrouwen vergroot. **Zaterdag 10 en zondag 11 oktober zijn sterkere maar pittigere IJmuiden-specifieke (pier-)alternatieven**, met gustpieken die mogelijk te ruig zijn voor een comfortabele sessie; **donderdag 8 oktober** is een mildere IJmuiden-optie met een wisselend Optimaal/Goed(b)-venster.
⚠️ Onzeker op 4+ dagen — check dichter bij de tijd opnieuw, met name de exacte windkracht en timing rond vrijdag 9 oktober en het verloop van het weekend erna.

---
_Bronnen: Windfinder (GFS) · windwaarnemingen.nl (KNMI, IJmuiden) · Soarcast — deze run niet bereikbaar (JS-app, geen vindbaar/bereikbaar API-adres)_
