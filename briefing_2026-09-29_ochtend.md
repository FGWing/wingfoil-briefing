# 🌊 Wingfoil-briefing Zandvoort–Wijk aan Zee
_29-09-2026 · Ochtendbriefing_

⚠️ **Technische kanttekening deze run:** Soarcast kon opnieuw niet geraadpleegd worden — nog altijd een volledige JS-app (React/Vite) zonder vindbaar/bereikbaar API-adres in de uitgeleverde bundle. Windfinder is dit keer wél via de onderliggende paginadata (in plaats van alleen de zichtbare tabel) opgehaald, inclusief golven/getij per 3 uur t/m 8 oktober in één keer — dus geen aparte Superforecast-pagina nodig voor de lange-termijn outlook. windwaarnemingen.nl (IJmuiden) is volledig gelukt via de directe KNMI-vsp/actuals-JSON.

---

## ⚡ Snel overzicht
- **Dinsdag:** Goed (grensgeval met Optimaal) — venster **05:00-08:00, loopt al tijdens het verzenden van deze briefing**
- **Woensdag:** Matig (02:00-08:00)
- **Donderdag:** Slecht (Windfinder) / Matig (KNMI-vsp) — modellen wijken sterk af, zie toelichting
- **Beste dag in de 7 dagen erna:** dinsdag 6 oktober (marginaal, nog ver vooruit)

---

## ⏰ Realitycheck vandaag

- Laatste actuele uren (windwaarnemingen.nl, IJmuiden, 05:00-07:10): **wind 17,0-19,4 kts, gust 19,7-25,9 kts, richting 84-92° (Oost)**
- Was voorspeld voor dezelfde uren: KNMI-vsp (windwaarnemingen.nl, huidige modelrun) gaf **12,4-12,8 kts gem / 19,2-20,2 kts gust, richting Oost (87-94°)**; Windfinder (GFS) gaf voor 05h **10,8 kts / 21,3 kts gust (84°)** en voor 08h **8,3 / 15,4 kts (76°)**.
- Conclusie: de wind **loopt fors VOOR** — het gemeten gemiddelde ligt bijna 2x hoger dan KNMI-vsp en ruim 1,5x hoger dan Windfinder; de gust zat dichter bij beide modellen maar bouwde daarna juist verder op (tot 25,9 kts) terwijl beide modellen een dalende gust voorspelden. Richting komt in alle drie bronnen goed overeen (Oost, 84-94°). Voor de rest van de dag: **vertrouwen naar boven bijgesteld voor het venster dat nu loopt** (grotendeels al gerealiseerd tegen verzendtijd), maar de classificatie voor ná 09:00 blijft **ongewijzigd Slecht** — beide modellen zijn het erover eens dat de wind daarna wegvalt, en het onderliggende mechanisme (nachtelijke regenband/instabiliteit, aanhoudende regen en ~100% bewolking in de Windfinder-data) is typisch een verschijnsel dat overdag verdwijnt.

---

## 📅 Komende 72 uur

### Dinsdag — Goed (grensgeval met Optimaal), venster loopt al
- **Beste venster: 05:00-08:00** (bij verzending van deze briefing grotendeels al bezig/voorbij). Actueel gemeten (windwaarnemingen.nl, zie Realitycheck): **wind 17-19 kts, gust 20-26 kts, richting ~84-92° (Oost = pal aflandig bij Zandvoort)** — fors sterker dan zowel Windfinder (10,8/21,3 kts) als KNMI-vsp (12,6-12,8/20 kts) voorspelden.
- **Grensgeval-classificatie:** het gemiddelde zit ruim in het Optimaal-bereik (14-25 kts) en de aflandige richting geeft vlak water, maar de criteria-tabel heeft geen exacte rij voor "sterke pal-aflandige wind" (Optimaal vraagt om side-shore/licht aflandig, Goed(a) om licht aanlandig) — vandaar Goed als dichtstbijzijnde categorie i.p.v. Matig/Optimaal geforceerd.
- **Na 08:00 stort het in naar Slecht.** Windfinder: 11h 8,6/12,4 kts (101°), 14h 6,5/8,6 kts (133°), 17h 7,3/11,4 kts (145°), 20h 7,8/12,3 kts (112°), 23h 9,7/18,5 kts (139°, kort grensgeval met Matig maar laat op de avond). KNMI-vsp bevestigt dezelfde afzwakking (8,2-11,1 kts gem / 8,6-18,9 kts gust) — beide bronnen eens over een rustige rest van de dag.
- Golven: 0,17-0,50 m / 4,3-5,8 s — de hele dag ruim onder de 1,1 m-drempel.
- 🌊 Piervoorkeur: niet van toepassing (golf blijft overal <0,8 m).
- Getij: laagwater ~01:37 (0,3 m), hoogwater ~05:59 (2,3 m), laagwater ~13:48 (0,5 m), hoogwater rond de vroege avond (niet exact bemonsterd), laagwater ~22:25 (0,8 m).
- Bronnen: Windfinder en KNMI-vsp **eens** over richting (Oost/OZO) en dagpatroon, maar de **actuele meting overtreft beide modellen fors** in gemiddelde wind — zie Realitycheck hierboven. Soarcast deze run niet bereikbaar.

### Woensdag — Matig
- **Beste venster: 02:00-08:00** — Windfinder: 02h 9,1/16,6 kts (143°, licht aflandig), 05h 9,7/17,6 kts (149°), 08h 9,3/17,4 kts (144°). Gemiddelde blijft net onder de 14 kts-ondergrens voor "Goed", vandaar Matig.
- KNMI-vsp bevestigt dit venster goed: 02h 9,7/14,0 kts (143°, ZO), 05h 10,9/15,7 kts (139°), 08h 11,5/16,9 kts (149°, ZZO) — vergelijkbare kracht én richting, **bronnen eens**.
- Na 08:00 valt het terug naar Slecht: 11h 9,3/15,0 kts (156°), 14h 8,3/12,2 kts (206°), daarna verder afzwakkend.
- **Let op avonddivergentie:** rond 17:00-20:00 wijken Windfinder en KNMI-vsp sterk af, zowel in kracht als richting — Windfinder geeft 17h 7,7/12,0 kts uit 249° (WZW), KNMI-vsp geeft 17h slechts 3,3/4,5 kts uit 153° (ZZO). Verandert niets aan de classificatie (beide ruim onder de Matig-drempel) maar toont dat de avondrichting onzeker is.
- Golven: 0,19-0,39 m / 2,8-4,7 s — ruim onder de 1,1 m-drempel de hele dag.
- 🌊 Piervoorkeur: niet van toepassing (golf blijft <0,8 m).
- Getij: laagwater ~02:08 (0,3 m), hoogwater ~06:37 (2,2 m), laagwater ~14:24 (0,5 m), hoogwater ~18:57 (2,2 m), laagwater ~23:24 (0,8 m).
- Bronnen: Windfinder en KNMI-vsp **eens** over de ochtend, **wijken duidelijk af** in de avond. Soarcast deze run niet bereikbaar.

### Donderdag — Slecht (Windfinder) / Matig (KNMI-vsp) — grote modeldivergentie
- **Windfinder (GFS) ziet de hele dag Slecht**: 02h 8,4/15,5 kts (185°), 05h 8,6/12,9 kts (282°, pal aanlandig), 08h 5,8/8,6 kts (257°), 11h 4,4/5,7 kts (294°), 14h 3,7/4,3 kts (329°) — nergens boven de 8,6 kts gemiddeld.
- **KNMI-vsp (windwaarnemingen.nl) ziet juist een opbouwende WZW/West-wind rond het middaguur**: 08h 12,1/16,3 kts (243°, WZW), 11h 13,4/18,3 kts (260°, West), 14h 11,1/18,5 kts (262°, West) — dit haalt "Matig" en zit met de richting (West/WZW) tegen pal aanlandig aan bij Zandvoort. Dekking van KNMI-vsp stopt na 14:00.
- **Dit is een aanzienlijke afwijking tussen de twee bronnen** — niet middelen: Windfinder ziet een vlakke, slappe dag, KNMI-vsp ziet een herkenbare middagpiek met andere windrichting (West i.p.v. Windfinders wisselende ONO/NW-achtige richtingen). Houd bij deze onzekerheid rekening met een kans op méér wind dan de hoofdbron (Windfinder) nu aangeeft, vooral rond 11:00-14:00.
- Golven (Windfinder, enige golfbron): 0,40-0,48 m / 3,9-5,0 s — ruim onder de 1,1 m-drempel, ook bij de KNMI-scenario's geen probleem voor piervoorkeur.
- 🌊 Piervoorkeur: niet van toepassing (golf blijft <0,8 m, ook al zou de KNMI-richting pal aanlandig zijn).
- Getij: laagwater ~02:42 (0,2 m), hoogwater ~07:19 (2,2 m), laagwater ~15:06 (0,4 m), hoogwater ~19:37 (2,2 m).
- Bronnen: Windfinder en KNMI-vsp **wijken sterk af** in kracht (KNMI ~2x hoger rond het middaguur) én richting. Soarcast deze run niet bereikbaar.

---

## 🔭 Kans op mooie sessies daarna (dag 4-9)
Windfinder (GFS, enige bron zo ver vooruit) laat voor **vrijdag 2 t/m woensdag 7 oktober** het volgende beeld zien:
- **Vrijdag 2 en zaterdag 3 oktober**: uitgesproken zwak, nergens boven 6,3 kts gemiddeld / 6,5 kts gust — Slecht.
- **Zondag 4 oktober**: bouwt licht op richting de avond (14h 8,8/10,0 kts, 241°) maar blijft onder elke bruikbare drempel — Slecht.
- **Maandag 5 oktober**: duidelijke opbouw in de middag/avond — 14h 12,1/16,1 kts (237°, side-shore), 17h 11,6/16,0 kts (229°), 23h 11,5/20,3 kts (214°, gusty) — Matig, met een grensgeval-gusty avond.
- **Dinsdag 6 oktober** springt er het meest uit: 08h 14,8/23,7 kts (223°, side-shore), **11h 17,2/24,6 kts (234°, side-shore)** — dit zit qua wind en richting tegen Optimaal aan, alleen de golf (~0,4 m) haalt de 1,1 m-drempel niet, dus een grensgeval Goed/Optimaal met opvallend hoge gust-factor (gust ~1,4x gemiddelde — wijst op een onstuimige/gusty periode, mogelijk een front). Na 14:00 draait de wind naar pal aanlandig en zakt de kracht terug naar Matig/Slecht.
- **Woensdag 7 oktober**: overwegend Slecht, met een korte Matig-piek om 08h (14,5/17,3 kts, 293°, pal aanlandig-achtig).

**Beste dag: dinsdag 6 oktober**, vooral het venster rond 08:00-11:00. Kans: **gemiddeld** — het signaal is consistent over meerdere 3-uurs-stappen (geen losse uitschieter), maar dit ligt nog 7 dagen vooruit.
⚠️ Onzeker op 4+ dagen — check dichter bij de tijd opnieuw, vooral de golfhoogte en de exacte timing van de richtingsdraai op dinsdag 6 oktober.

---
_Bronnen: Windfinder (GFS) · windwaarnemingen.nl (KNMI, IJmuiden) · Soarcast — deze run niet bereikbaar (JS-app, geen vindbaar/bereikbaar API-adres)_
