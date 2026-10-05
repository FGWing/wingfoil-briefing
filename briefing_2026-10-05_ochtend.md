# 🌊 Wingfoil-briefing Zandvoort–Wijk aan Zee
_05-10-2026 · Ochtendbriefing_

⚠️ **Technische kanttekening deze run:** Soarcast is (net als alle voorgaande runs) niet bereikbaar — pure JS-app zonder vindbaar/bereikbaar API-adres of statisch gerenderde data (shell-HTML is 2,4KB, geen SSR-data in de bundle te vinden). Windfinder is via de onderliggende paginadata (astro-hydration props) opgehaald — één bezoek aan de reguliere forecast-pagina leverde zowel de korte termijn (3-uurs, vandaag+morgen) als de volledige 3-uurs data t/m 14 oktober in dezelfde payload (geen apart bezoek aan de Superforecast-pagina nodig). windwaarnemingen.nl (IJmuiden) is via de onderliggende vsp-JSON-endpoints opgehaald: 10-minuten-actuals + het ingebedde KNMI-uurmodel voor vandaag, en het KNMI-uurmodel voor morgen/overmorgen.

---

## ⚡ Snel overzicht
- **Maandag:** Goed (a) — grensgeval met Optimaal qua richting (12:00-17:00)
- **Dinsdag:** Slecht
- **Woensdag:** Slecht
- **Beste dag in de 7 dagen erna:** donderdag 8 oktober

---

## ⏰ Realitycheck vandaag

- Laatste actuele uren (windwaarnemingen.nl, IJmuiden, 05:00-07:10): **wind 12,1-15,3 kts gem, gust 15,1-17,3 kts, richting zuidwest (221-227°)**.
- Was voorspeld voor dezelfde uren (KNMI-vsp, huidige modelrun): **05:00 182° ZUID, 8,6/12,1 kts; 06:00 183° ZUID, 8,7/12,2 kts; 07:00 197° ZZW, 8,6/12,4 kts**. Windfinder (GFS, 3-uurs) zat voor 05h op een vergelijkbare 8,1/12,3 kts, richting 226° (wél al de juiste richting).
- Conclusie: windkracht loopt duidelijk **VOOR** — de actuele gemiddelde wind ligt ~4-7 kts boven wat beide modellen voor deze uren voorspelden, en ook de richting is al verder naar zuidwest gedraaid dan het KNMI-model aangaf (dat zat nog op zuid/ZZW). Opvallend: de huidige actuals (15,3 kts om 07:00) liggen al dicht bij wat het KNMI-model pas voor ±11:00-12:00 voorspelde (13,2 kts) — de opbouw lijkt dus 4-5 uur eerder te gaan dan gemodelleerd. Voor de rest van de dag: inschatting **bijgesteld** — het middagvenster wordt met iets meer vertrouwen ingeschat, mogelijk al vanaf 12:00-13:00 bruikbaar (i.p.v. pas na 15:00) en mogelijk net iets sterker dan de gemodelleerde piek van 14,6-15,2 kts. De golfhoogte (uitsluitend Windfinder, landstations meten geen golven) blijft hoe dan ook laag (max ~0,7m), dus dit verandert de classificatie niet voorbij Goed(a)/grensgeval-Optimaal.

---

## 📅 Komende 72 uur

### Maandag — Goed (a) — grensgeval met Optimaal
- Beste venster: **12:00-17:00** (mogelijk al vanaf 12:00 bruikbaar, zie Realitycheck) — wind 11-15 kts gem (Windfinder 3-uurs-punten), KNMI-vsp-piek 14,6-15,2 kts rond 15:00-16:00, gust 14-21 kts, richting 240-255° (WZW) — dit ligt bij Zandvoort op de grens tussen "licht aanlandig" en "side-shore" (de actuele wind van vanochtend was al dichter bij side-shore dan het model nu voorspelt).
- Golven: 0,5-0,7m / 4-5s — te laag voor Optimaal, vormt het plafond van de dag.
- 🌊 Piervoorkeur: niet van toepassing (golf <0,8m).
- Getij: laagwater ~06:38 (0,5m), hoogwater ~11:43 (1,5m), laagwater ~19:02 (0,5m), hoogwater ~00:26 volgende dag (1,9m).
- Bronnen: Windfinder (GFS) en KNMI-vsp **eens** over het patroon (opbouw ochtend → piek middag → afname avond), maar beide modellen **onderschatten de ochtendwind fors** (zie Realitycheck) — neem de piektijd en -kracht daardoor met een lichte plus. Soarcast niet bereikbaar.

### Dinsdag — Slecht
- Windfinder (GFS, 3-uurs): hele dag zwak en instabiel van richting — 1,8-7,3 kts gem / 2,3-10,8 kts gust, richting draait van zuidwest (225°) via noordwest/noord (294-343°) naar oost (61°) — overal ruim onder de Slecht-drempel.
- KNMI-vsp (uurmodel, dekt hele dag): bevestigt het zwakke beeld — zelfs de "piek" om 00:00 is maar 10,5/14,6 kts, de middag zakt terug naar 1-4 kts. Beide bronnen zijn het eens: een vrijwel windstille dag.
- Golven (Windfinder, enige golfbron): 0,4-0,6m / 3,9-6,6s — ruim onder de drempel.
- 🌊 Piervoorkeur: niet van toepassing (golf <0,8m).
- Getij: laagwater ~08:41 (0,5m), hoogwater ~13:04 (1,5m), laagwater ~20:38 (0,4m).
- Bronnen: Windfinder en KNMI-vsp **eens** (Slecht). Soarcast niet bereikbaar.

### Woensdag — Slecht
- Windfinder (GFS, 3-uurs): overwegend zwak en nu uit oost/oostzuidoost (88-100°, bij Zandvoort pal aflandig — gunstige richting, maar met 4,1-6,6 kts gem simpelweg te weinig wind). Pas laat op de avond (23:00) draait het naar noordwest (298°, pal aanlandig) met wind nog steeds zwak (7,5 kts) maar golf oplopend naar 0,96m.
- KNMI-vsp (uurmodel, dekt t/m 16:00): bevestigt het zwakke oostelijke beeld (4,5-6,4 kts, richting OZO/OOST) — geen tegenstrijdig signaal.
- Golven: 0,4-1,0m / 5,6-7,3s — de avondwaarde (0,96m) nadert de pierdrempel (0,8m), maar de wind (7,5 kts) is zo zwak dat dit irrelevant is voor de classificatie.
- 🌊 Piervoorkeur: niet van toepassing (wind te zwak om relevant te zijn, ondanks golf > 0,8m laat op de avond).
- Getij: hoogwater ~01:46 (2,0m), laagwater ~10:15 (0,4m), hoogwater ~14:12 (1,7m), laagwater ~21:55 (0,3m).
- Bronnen: Windfinder en KNMI-vsp **eens** (Slecht). Soarcast niet bereikbaar.

---

## 🔭 Kans op mooie sessies daarna (dag 4-9)
Windfinder (GFS, enige bron zo ver vooruit — in één keer t/m 14 oktober opgehaald) laat voor **donderdag 8 t/m dinsdag 13 oktober** het volgende beeld zien. Deze periode wordt gedomineerd door een stevig NW/W-windveld waarbij **IJmuiden** door zijn eigen kustlijnhoek (150°/330°) de hele periode veel gunstiger ligt dan **Zandvoort** (waar dezelfde richting grotendeels pal aanlandig is):

- **Donderdag 8 oktober — beste dag**: bij **IJmuiden** staat de wind vrijwel de **hele dag side-shore tot licht aflandig** (309-347°, NW/NNW) met wind gestaag 17,7-21,5 kts gem, gust 21,1-25,0 kts, en golf 1,39-1,88m / 6,3-7,6s — dat is de **hele dag Optimaal**, met de meest consistente en minst extreme windstoten van de hele outlookperiode (geen enkel moment boven de 27kts-sluitingsdrempel van de Reddingsbrigade). Bij **Zandvoort** is vooral de vroege ochtend (02:00-08:00) ook al side-shore/Optimaal, maar draait het richting de avond (17:00, 23:00) naar pal aanlandig — daar dus minder gunstig. 🌊 **Piervoorkeur: IJmuiden** (Zuidpier breekt de NW-golfslag) vrijwel de hele dag. Venster: ruim overdag (08:00-18:00) ruim binnen Optimaal.
- **Vrijdag 9 oktober**: nog krachtiger maar grilliger. Bij **IJmuiden** 's nachts (02:00) Optimaal, dan kort **Slecht** (05:00-08:00, wind draait daar tijdelijk pal aanlandig), om 11:00 weer Optimaal (18,4/28,0 kts — gust al boven de Reddingsbrigade-drempel), en van 14:00-20:00 een grensgeval Optimaal/Goed(a) met **extreme windstoten tot 32,5 kts** (277°, in de neutrale zone tussen de pierassen — geen piervoordeel op dat moment) — dit is stormachtig en waarschijnlijk niet comfortabel. Bij **Zandvoort** is het vrijwel de hele dag pal aanlandig → Slecht. 🌊 Piervoorkeur: kort **Wijk aan Zee** (08:00/11:00, wind dan uit het zuiden), daarna vooral neutraal/te extreem om nog relevant te zijn.
- **Zaterdag 10 oktober**: bij **IJmuiden** opnieuw Optimaal/grensgeval-Optimaal vrijwel de hele dag — 16,6-21,9 kts gem, gust 19,5-26,0 kts (sterk, iets minder extreem dan vrijdag), golf 1,58-1,73m / 6,65-6,95s. Bij **Zandvoort** de hele dag pal aanlandig (280-297°) → Slecht/zware branding zonder beschutting. 🌊 Piervoorkeur: **IJmuiden**, vrijwel de hele dag.
- **Zondag 11 oktober**: vergelijkbaar met zaterdag — bij **IJmuiden** Optimaal/grensgeval-Optimaal, 18,0-22,7 kts gem, gust 22,7-26,8 kts, golf 1,23-1,54m / 6,55-6,89s. Bij **Zandvoort** weer pal aanlandig (275-316°) → Slecht. 🌊 Piervoorkeur: **IJmuiden**.
- **Maandag 12 oktober**: de wind valt terug. Bij **IJmuiden** 's ochtends (02:00-08:00) nog Optimaal (15,6-17,9 kts, gust 18,7-21,8 kts, golf 1,16-1,24m), maar na 11:00 al **Slecht** (<13 kts) en de richting draait via noord naar oost. Bij **Zandvoort** is 08:00 nog kort side-shore Optimaal (15,6 kts, golf 1,16m/6,3s) — het laatste redelijke moment daar. 🌊 Piervoorkeur: **IJmuiden**, maar alleen tot ±08:00-11:00.
- **Dinsdag 13 oktober**: overwegend **Slecht** — zwak (6-12 kts) en pal aflandig bij Zandvoort (gunstige richting, maar te weinig wind). Alleen 's avonds (20:00/23:00) komt de gust boven 16 kts (16,1-20,2 kts) — grensgeval Matig, maar het gemiddelde blijft te laag.

**Beste dag: donderdag 8 oktober**, met name het venster **08:00-18:00 bij IJmuiden** — een vrijwel ononderbroken Optimaal-dag (18-21 kts gem, golf 1,4-1,9m met lange periode), zonder de extreme windstoten die vrijdag t/m zondag kenmerken. Kans: **hoog** — het signaal is sterk en over de hele dag consistent, al ligt de dag nog 3+ dagen vooruit. **Vrijdag 9 t/m zondag 11 oktober zijn sterkere maar pittigere/stormachtige IJmuiden-alternatieven**, met gustpieken die herhaaldelijk boven de 27kts-sluitingsdrempel van de Reddingsbrigade komen — indrukwekkend maar niet voor iedereen comfortabel.
⚠️ Onzeker op 4+ dagen — check dichter bij de tijd opnieuw, met name de exacte kracht en timing rond donderdag 8 oktober en of de windstoten vrijdag-zondag werkelijk zo extreem uitpakken.

---
_Bronnen: Windfinder (GFS) · windwaarnemingen.nl (KNMI, IJmuiden) · Soarcast — deze run niet bereikbaar (JS-app, geen vindbaar/bereikbaar API-adres)_
