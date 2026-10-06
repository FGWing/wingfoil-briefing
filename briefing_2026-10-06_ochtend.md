# 🌊 Wingfoil-briefing Zandvoort–Wijk aan Zee
_06-10-2026 · Ochtendbriefing_

⚠️ **Technische kanttekening deze run:** Soarcast is (net als alle voorgaande runs) niet bereikbaar — pure JS-app zonder vindbaar/bereikbaar API-adres (shell-HTML van 2,4KB, geen SSR-data in de gecompileerde bundle te vinden). Windfinder is via de onderliggende paginadata (astro-hydration props) opgehaald — één bezoek aan de reguliere forecast-pagina leverde zowel de korte termijn (3-uurs, vandaag+morgen) als de volledige 3-uurs data t/m 15 oktober in dezelfde payload (geen apart bezoek aan de Superforecast-pagina nodig). windwaarnemingen.nl (IJmuiden) is via de onderliggende vsp-PHP-endpoints opgehaald: 10-minuten-actuals + ingebed KNMI-uurmodel voor vandaag, en het KNMI-uurmodel voor morgen/overmorgen.

---

## ⚡ Snel overzicht
- **Dinsdag:** Slecht
- **Woensdag:** Slecht (late avond al eerste opbouw richting donderdag)
- **Donderdag:** Optimaal bij IJmuiden (Zandvoort pal aanlandig → Slecht) ⚠️ grote modelspreiding in kracht (08:00-20:00)
- **Beste dag in de 7 dagen erna:** zondag 11 oktober

---

## ⏰ Realitycheck vandaag

- Laatste actuele uren (windwaarnemingen.nl, IJmuiden, 05:00-07:30): **wind 3,6-7,1 kts gem, gust 5,0-10,0 kts**, richting draait van zuidwest/westzuidwest (201-258°) langzaam naar west (260-273°).
- Was voorspeld voor dezelfde uren: Windfinder (GFS, 3-uurs) 05h **247° 5,0/7,1 kts**, 08h **283° 5,6/7,7 kts**; KNMI-vsp (windwaarnemingen.nl, huidige modelrun) 06:00 **284° WNW 6,2/10,3 kts**, 07:00 **280° WEST 6,0/9,3 kts**.
- Conclusie: wind loopt ongeveer **CONFORM** verwachting. Windfinder voorspelde de richting bij 05h bijna exact (247° vs actueel 234-252°) en ook de kracht klopt goed; KNMI-vsp zit qua kracht (6,0-6,2kts) licht aan de hoge kant t.o.v. de actuele 3,6-7,1kts, en de richting draait in werkelijkheid iets trager door naar west dan KNMI's 280-284° al suggereerde. Rest-van-de-dag inschatting: **ongewijzigd** — dit blijft een zwakke dag, geen aanpassing nodig op basis van deze vroege uren.

---

## 📅 Komende 72 uur

### Dinsdag — Slecht
- Windfinder (GFS, 3-uurs): hele dag zwak, 3,0-7,0 kts gem / 3,1-10,1 kts gust, richting draait van zuidwest (220°) via west/WNW (267-291°) naar noord/oost (13-70°) in de loop van de avond/nacht.
- windwaarnemingen.nl (KNMI-vsp + actuals, IJmuiden): bevestigt het zwakke beeld — zie Realitycheck hierboven.
- Golven (Windfinder, enige golfbron): 0,39-0,62m / 3,7-7,3s — ruim onder de drempel.
- 🌊 Piervoorkeur: niet van toepassing (golf <0,8m).
- Getij: laagwater ~08:41 (0,5m), hoogwater ~13:04 (1,5m), laagwater ~20:38 (0,4m).
- Bronnen: Windfinder en KNMI-vsp **eens** (Slecht). Soarcast niet bereikbaar (zie technische kanttekening).

### Woensdag — Slecht
- Windfinder (GFS, 3-uurs): overwegend zwak en van richting oost/zuidoost (111-134°, bij Zandvoort pal aflandig — gunstige hoek, maar simpelweg te weinig wind: 1,4-9,4 kts gem). Draait laat op de avond naar noordwest/noord (303-336°) met de wind oplopend tot 15,8 kts gem/18,0 kts gust om 23:00 — de voorbode van de storm van donderdag.
- KNMI-vsp (uurmodel, windwaarnemingen.nl): bevestigt het zwakke oostelijke beeld overdag, maar laat de avondopbouw veel eerder en veel heftiger beginnen dan Windfinder: al vanaf 19:00 **16,7/25,7 kts**, oplopend naar **22,2/31,9 kts** om 23:00 — **grote afwijking met Windfinder** (15,8/18,0 kts) op exact hetzelfde moment. Dit is het eerste signaal van de grote modelspreiding die donderdag domineert (zie hieronder) — niet middelen, beide apart vermeld.
- Golven: 0,39-1,08m / 5,2-7,4s — pas laat op de avond (23:00) de 1,1m-drempel genaderd (1,08m).
- 🌊 Piervoorkeur: niet van toepassing (richting blijft overwegend side-shore/pal aflandig bij Zandvoort en IJmuiden, geen aanlandige component van betekenis).
- Getij: hoogwater ~01:46 (2,0m), laagwater ~10:15 (0,4m), hoogwater ~14:12 (1,6m), laagwater ~21:55 (0,3m).
- Bronnen: Windfinder en KNMI-vsp **eens** dat het overdag zwak blijft, maar wijken sterk af over tijdstip/kracht van de avondopbouw — zie hierboven. Soarcast niet bereikbaar.

### Donderdag — Optimaal bij IJmuiden ⚠️ grote modelspreiding
- Bij **Zandvoort**: wind grotendeels **pal aanlandig** (278-345°, NNW/NW) de hele dag → in combinatie met golf 1,55-1,84m en geen pierbescherming is dit **Slecht** (zware onbeschutte branding).
- Bij **IJmuiden** (pierzone-hoek 150°/330°): dezelfde richting leest als **side-shore tot licht aanlandig** → in combinatie met wind 15,3-20,8 kts (Windfinder) en golf 1,55-1,84m/7,0-7,3s is dit vrijwel de hele dag **Optimaal**.
- Beste venster (IJmuiden): **08:00-20:00** — Windfinder: wind 18,5-20,0 kts gem, gust 20,4-23,3 kts, richting 298-345° (NW/NNW).
- 🌊 Piervoorkeur: **IJmuiden** (Zuidpier breekt de noordwest-golfslag) de hele dag — Wijk aan Zee ligt bij deze richting juist net als Zandvoort onbeschut.
- Getij: hoogwater ~02:44 (2,1m), laagwater ~11:41 (0,3m), hoogwater ~15:03 (1,8m) — rond het middagvenster (11:00-15:00) dus van laag naar hoog water, shorebreak neemt richting hoogwater toe, ook aan de beschutte IJmuiden-kant.
- Bronnen: **grote afwijking, niet middelen.** Windfinder (GFS) houdt het op 15,3-20,8 kts gem / 18,1-23,5 kts gust — stevig maar beheersbaar, ruim onder de 27kts-sluitingsdrempel van de Reddingsbrigade. KNMI-vsp (windwaarnemingen.nl) voorspelt voor dezelfde uren een veel heftiger beeld: **20-27 kts gemiddeld**, met gust tot **36-39 kts** tussen 00:00-08:00 — als dat uitkomt, ligt dat ruim boven de sluitingsdrempel van de Reddingsbrigade en betekent dat veel grovere/gevaarlijkere condities dan Windfinders Optimaal-beeld. Soarcast was niet bereikbaar om als derde bron te arbitreren. **Check dit dicht bij de tijd opnieuw** — bij twijfel uitgaan van het zwaardere KNMI-scenario en voorzichtig zijn, zeker vroeg in de ochtend/nacht.

---

## 🔭 Kans op mooie sessies daarna (dag 4-9)
Windfinder (GFS, enige bron zo ver vooruit — in één keer t/m 15 oktober opgehaald) voor **vrijdag 9 t/m woensdag 14 oktober**, steeds beoordeeld op de IJmuiden-hoek (de richting is deze hele periode grotendeels noordwestelijk, waar IJmuiden door zijn kustlijnhoek structureel gunstiger ligt dan Zandvoort):

- **Vrijdag 9 oktober**: krachtig maar grillig. Bij IJmuiden overwegend pal aanlandig (dus Slecht/grensgeval) met twee korte Optimaal-vensters (rond 05:00 en 08:00-11:00) en extreme gust tot **32,4 kts** om 08:00 — stormachtig, waarschijnlijk niet comfortabel. 🌊 Piervoorkeur: wisselend, vaak neutrale zone (wad 267-279°).
- **Zaterdag 10 oktober**: bij IJmuiden grotendeels grensgeval (licht aanlandig, net niet side-shore genoeg voor een schone Optimaal-classificatie), wind 13,0-25,2 kts gem, gust 16,6-29,6 kts, golf 1,61-2,04m/6,6-7,4s. Bruikbaar, maar geen uitschieter. 🌊 Piervoorkeur: IJmuiden vanaf 05:00.
- **Zondag 11 oktober — beste dag**: bij IJmuiden vanaf 05:00 tot 23:00 vrijwel ononderbroken **Optimaal** — wind 14,2-25,3 kts gem, gust rustig afbouwend van 29,3 kts (vroege ochtend) naar 16,8-22,4 kts (middag/avond), golf 1,57-2,12m met lange periode (7,46-7,83s). Minder extreem/grillig dan vrijdag — een krachtige maar geleidelijk rustiger wordende dag. 🌊 Piervoorkeur: **IJmuiden** (Zuidpier) de hele dag.
- **Maandag 12 t/m woensdag 14 oktober**: de wind valt terug. Overwegend **Slecht** (3,1-13,4 kts gem), met alleen dinsdagavond (13 oktober, 13,4 kts gem/19,7 kts gust) een kort grensgeval Matig. Geen van deze dagen haalt de Optimaal- of Goed-drempel.

**Beste dag: zondag 11 oktober**, met name **05:00-23:00 bij IJmuiden** — krachtige, lange-periode swell die door de dag geleidelijk rustiger wordt, zonder de extreme piekstoten van vrijdag. Kans: **hoog** voor wind/richting — het signaal is op dit moment consistent over bijna de hele dag — al ligt de dag nog 5 dagen vooruit.
⚠️ Onzeker op 4+ dagen — check dichter bij de tijd opnieuw, met name of vrijdag/zaterdags zware wind de golfopbouw voor zondag beïnvloedt, en of donderdags modelspreiding (zie hierboven) ook voor dit deel van de week nog een rol speelt.

---
_Bronnen: Windfinder (GFS) · windwaarnemingen.nl (KNMI, IJmuiden) · Soarcast — deze run niet bereikbaar (JS-app, geen vindbaar/bereikbaar API-adres)_
