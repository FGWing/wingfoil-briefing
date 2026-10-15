# 🌊 Wingfoil-briefing Zandvoort–Wijk aan Zee
_15-10-2026 · Ochtendbriefing_

⚠️ **Technische kanttekening:** Soarcast blijft onbereikbaar deze run (pure JS/Vite-app, `/web/locationinfo?...` levert alleen een lege HTML-shell zonder onderliggende data — zelfde conclusie als alle voorgaande runs; meta-tag verwijst naar "weather2kite" maar er is geen bereikbaar API-adres gevonden). Windfinder is opgehaald via de onderliggende Astro-island props: de reguliere forecast-pagina gaf dag 1-2, en de `ForecastDataInit`-component op diezelfde pagina bevatte daarnaast al dag 3 t/m 10 (17-24 oktober) in 3-uurs stappen — dus geen aparte Superforecast-pagina nodig. windwaarnemingen.nl (IJmuiden) is opgehaald via `database/vsp_vdg_wstats.php?st=IJmuiden1` (vandaag: 10-minuten-actuals + ingebed KNMI-uurmodel) en `vsp_mrg_wstats.php?st=IJmuiden2` (morgen volledig + overmorgen t/m 16:00).

**Belangrijkste signaal deze run:** het patroon van de laatste dagen zet onverminderd door — GFS (Windfinder) voorspelt voor vanochtend vroeg 11,5-12,3 kts, maar de actuals bij IJmuiden liggen op 5,8-6,3 kts en liggen daarmee vrijwel exact op het KNMI-model (5,3-5,5 kts). Dit is niet een eenmalige afwijking maar een terugkerend beeld deze week, en het raakt niet alleen vandaag maar ook de KNMI-cijfers voor vrijdag en zaterdag (inclusief de eerder als "beste dag" aangewezen zaterdag) — zie Realitycheck en de dagsecties voor hoe dit is meegenomen.

---

## ⚡ Snel overzicht
- **Donderdag:** Grensgeval Goed/Optimaal volgens Windfinder (±11:00-17:00, piek 14:00, 14,9 kts side-shore, golf 0,84m), maar waarschijnlijk eerder **Matig** — het KNMI-model geeft voor dezelfde uren slechts ~6-8 kts, en de Realitycheck van vanochtend bevestigt dat de actuals tot nu toe KNMI volgen, niet GFS.
- **Vrijdag:** Slecht het grootste deel van de dag (4,6-9,9 kts). Windfinder ziet vanaf 17:00 een sprong naar noordelijke wind (15,6-17,6 kts, grensgeval Goed/Optimaal), maar KNMI (volledige dag beschikbaar) ziet deze avondopbouw niet en blijft de hele avond onder de 10 kts — lage betrouwbaarheid op dit venster.
- **Zaterdag:** Optimaal volgens Windfinder, een lang venster 08:00-20:00 (NNO side-shore, 14,4-17,2 kts, golf 1,0-1,4m/5,4-7,3s), maar KNMI (beschikbaar tot 16:00) voorspelt voor dezelfde uren maar 2-7 kts — een zeer groot verschil, in lijn met het GFS-overschattingspatroon van deze week. Behandel deze "beste dag" dus met nadrukkelijke onzekerheid.
- **Beste dag in de 7 dagen erna:** vrijdag 23 oktober
_(De eerste 3 regels zijn altijd de eerstvolgende 3 volle dagen vanaf het moment van versturen.)_

---

## ⏰ Realitycheck vandaag

- Laatste actuele uren (windwaarnemingen.nl, IJmuiden, 06:00-07:10): **wind 5,8-6,3 kts, gust 6,8-7,5 kts, richting 177-183° (ZUID)**.
- Was voorspeld voor dezelfde uren: het **ingebedde KNMI-uurmodel** gaf voor 06h/07h **186/179° (ZUID), 5,3-5,5 kts, gust 7,9-8,4 kts** — nagenoeg gelijk aan de actuals. **Windfinder/GFS** gaf voor de dichtstbijzijnde 3-uurspunten (05h/08h) **198-201°, 12,3 kts (beide punten), gust 20,1-21,6 kts** — ruim het dubbele van wat er werkelijk staat.
- Conclusie: de wind loopt **ACHTER op Windfinder/GFS**, maar **klopt vrijwel exact met windwaarnemingen.nl/KNMI**. Dit is al de tweede ochtend op rij met precies dit beeld. Rest-van-de-dag inschatting: **naar beneden bijgesteld** — het Windfinder-venster van vandaag (piek 14,9 kts om 14:00) krijgt beduidend minder vertrouwen; het KNMI-model zelf voorspelt voor de rest van vandaag een piek van slechts ~8 kts (gust ~11 kts) rond het middaguur, wat eerder op **Matig** uitkomt dan op het Windfinder-beeld "grensgeval Goed/Optimaal". Dit versterkt ook het voorbehoud bij vrijdag en zaterdag hieronder, waar hetzelfde GFS/KNMI-gat zich voordoet.

---

## 📅 Komende 72 uur

### Donderdag — Grensgeval Goed/Optimaal (Windfinder) / waarschijnlijk Matig (KNMI + Realitycheck)
- Bij **Zandvoort/Wijk aan Zee**: de hele dag side-shore richting (191-216°, zuid/ZZW), wind geleidelijk oplopend van 9-12 kts 's nachts naar een piek van **14,9 kts (gust 21,6 kts) om 14:00**, golf net onder de 1,1m-drempel (0,70-0,87m, periode 5,0-5,5s — periode zelf wel voldoende) → past bij geen tabelrij exact, dus **grensgeval Goed/Optimaal** volgens Windfinder alleen. Het KNMI-model (ingebed in windwaarnemingen.nl) voorspelt voor de hele dag echter maar 5,2-8,0 kts (gust max 11,3 kts, piek ook rond 12:00-14:00) → dat is ruim **Matig/Slecht**-niveau. Gezien de Realitycheck van vanochtend (actuals volgen KNMI, niet GFS) is **Matig de waarschijnlijkere uitkomst** voor de rest van de dag.
- Bij **IJmuiden** (pierzone-hoek): van ±05:00 tot 20:00 leest de richting hier als **licht aanlandig** (198-208°, 20:00) tot **pal aanlandig** (14:00-17:00 en 23:00, 211-216°) — minder gunstig dan Zandvoorts side-shore, en golf (0,74-0,87m) ligt boven de 0,8m-drempel voor pier-logica.
- 🌊 Piervoorkeur: **05:00-17:00** is de richting bij IJmuiden (licht/pal) aanlandig met golf ≥0,8m → **Wijk aan Zee (Noordpier)** is de rustiger keuze (de zuid/ZZW-golfslag komt uit de hoek die de Noordpier breekt).
- Golven (Windfinder, enige golfbron): 0,65-0,87m / 5,04-5,49s.
- Getij: laagwater 03:08 (0,34m), hoogwater 07:08 (1,97m), laagwater 15:21 (0,36m), hoogwater 19:21 (2,13m).
- Bronnen: Windfinder (GFS) en windwaarnemingen.nl (KNMI) zijn het **eens over de richting** (zuid/ZZW) maar wijken **fors af in windkracht** — GFS tot 14,9 kts tegenover KNMI maar tot 8,0 kts. De Realitycheck hierboven bevestigt dat de actuals tot nu toe de KNMI-lijn volgen. Soarcast niet bereikbaar.

### Vrijdag — Slecht (grootste deel van de dag), mogelijke avondopbouw (onzeker)
- Bij **Zandvoort/Wijk aan Zee**: **02:00-14:00** te weinig wind (4,6-9,9 kts, gust tot 11,3 kts) bij side-shore richting (186-220°, zuid/ZW) → **Slecht**. Windfinder ziet vanaf **17:00** een abrupte draai naar **noord** (335-358°, nog steeds side-shore qua classificatie) met een sprong naar **17,6 kts** (gust 20,7 kts), golf nog laag (0,81m/4,49s, periode net onder drempel) → grensgeval. Om **20:00**: 1°, 15,6 kts, golf 1,03m/5,03s en om **23:00**: 352°, 17,5 kts, golf 1,08m/5,37s — beide net onder de 1,1m-golfdrempel → **grensgeval Goed/Optimaal**, de opbouw richting het Optimaal-venster van zaterdag.
- **Belangrijk voorbehoud:** windwaarnemingen.nl/KNMI dekt deze dag nu volledig (00:00-23:00) en laat **geen enkele avondopbouw** zien — de wind blijft de hele avond onder de 10 kts (14:00 9,7 kts tot 23:00 8,2 kts, met een korte piek van 9,7 kts om 14:00). Dat staat in schril contrast met Windfinders 15,6-17,6 kts vanaf 17:00. Gezien het patroon dat GFS deze week systematisch te sterk zit (Realitycheck, en hetzelfde gat bij donderdag) is dit avondvenster met **grote onzekerheid** belast — mogelijk valt het net als vandaag fors terug naar het KNMI-beeld.
- Bij **IJmuiden/Wijk aan Zee** (pierzone-hoek): de noordelijke/zuidwestelijke richtingen vallen bij beide pierzones niet in de aanlandige hoek → geen piervoordeel van toepassing.
- Golven (Windfinder): 0,53-1,08m / 4,30-5,37s — laag overdag, oplopend in de avond (indien de wind er inderdaad komt).
- Getij: laagwater 03:29 (0,39m), hoogwater 07:40 (1,90m), laagwater 15:46 (0,36m), hoogwater 19:54 (2,07m).
- Bronnen: Windfinder (GFS) en windwaarnemingen.nl (KNMI) zijn het overdag **eens** (beide zwak), maar wijken 's avonds **extreem** af — alleen Windfinder ziet de noordelijke opbouw. Check dit venster dicht bij de tijd opnieuw. Soarcast niet bereikbaar.

### Zaterdag — Optimaal (Windfinder), maar met nadrukkelijke onzekerheid (KNMI wijkt sterk af)
- Bij **Zandvoort/Wijk aan Zee**: de richting draait verder naar **noord/NNO** (353-29°, side-shore t.o.v. de kust) bij wind die oploopt tot **14,4-17,2 kts** (gust 17,2-22,3 kts) en golf die mooi opbouwt tot **1,03-1,44m** met een lange periode (**5,4-7,3s**) → dit scoort **Optimaal** op vijf van de acht 3-uurspunten (08:00, 11:00, 14:00, 17:00, 20:00), het langste en sterkste venster van de komende 72 uur volgens Windfinder. Beste moment: **11:00-17:00** (golf piekt om 17:00 op 1,44m/6,74s).
- **Belangrijk voorbehoud:** windwaarnemingen.nl/KNMI is beschikbaar tot 16:00 en voorspelt voor **dezelfde uren slechts 2,2-6,9 kts** (gust wel pittig, 10-14 kts — wijst op buiige, instabiele lucht) — een verschil van bijna een factor 2-3 met Windfinder. Dit is de derde dag op rij met dit GFS/KNMI-gat, en de Realitycheck van vanochtend bevestigt dat de actuals tot nu toe steeds de (zwakkere) KNMI-lijn volgen. **Behandel de Optimaal-classificatie van zaterdag dus met nadrukkelijke onzekerheid** — dit was in eerdere briefings al de aangewezen "beste dag", maar dat beeld steunt vooral op GFS. Check dicht bij de tijd opnieuw, idealiter met een vers KNMI-uurmodel voor de middag/avond (nu nog niet beschikbaar).
- Bij **IJmuiden/Wijk aan Zee** (pierzone-hoek): bij enkele punten (11:00, 14:00, 23:00) leest de richting als **licht aflandig** t.o.v. de pierzone-hoek — geen pier-logica van toepassing (niet aanlandig).
- Golven (Windfinder, enige golfbron): 1,03-1,44m / 5,39-7,29s.
- Getij: laagwater 03:56 (0,44m), hoogwater 08:11 (1,83m), laagwater 16:17 (0,36m), hoogwater 20:28 (1,97m).
- Bronnen: Windfinder (GFS) enige bron met golfdata; windwaarnemingen.nl/KNMI dekt tot 16:00 en wijkt fors af in windkracht (zie voorbehoud). Soarcast niet bereikbaar.

---

## 🔭 Kans op mooie sessies daarna (dag 4-9)
Windfinder (GFS, enige bron zo ver vooruit, 3-uurs resolutie) voor **zondag 18 t/m vrijdag 23 oktober**:

- **Zondag 18 oktober**: richting draait naar (licht/pal) aflandig (50-89°, ONO/O), wind zwak (7,5-12,8 kts) → grotendeels **Slecht**, met een grensgeval richting Matig in de late avond (20:00-23:00, 10,5-12,8 kts, gust tot 21,8 kts) door toenemende gustiness.
- **Maandag 19 oktober**: de **hele dag pal aflandig** (76-85°, O/ONO) met stevige wind (13,2-15,9 kts) maar **extreme gust** (21,9-27,4 kts — zeer puffig) en weinig golf (0,47-0,64m, vlak water door de aflandige hoek) → **grensgeval Goed** de hele dag, met nadruk op de gustiness en de volledig aflandige hoek (lastiger terugkomen bij een gat in de wind).
- **Dinsdag 20 oktober**: vergelijkbaar maar nog puffiger — pal aflandig (85-96°), wind 12,3-16,3 kts, gust 19,7-26,3 kts (bijna het dubbele van het gemiddelde), golf zeer laag (0,26-0,33m) → **grensgeval Goed**, pittige vlakke sessie voor wie tegen de gustiness kan.
- **Woensdag 21 oktober**: verder verzwakkend, pal aflandig (89-109°), wind 10,9-15,2 kts, gust 16,4-21,8 kts, golf laag (0,16-0,22m) → **Matig/grensgeval Goed**.
- **Donderdag 22 oktober**: richting draait via aflandig naar side-shore (108-166°), wind zwak (6,4-11,0 kts) → **Slecht** het grootste deel van de dag, lichte verbetering richting **Matig** in de avond (20:00-23:00, 9,2-11,0 kts).
- **Vrijdag 23 oktober — beste dag**: richting draait naar zuid/ZW (side-shore) en vanaf de ochtend naar **licht aanlandig** (211-260°), wind pakt duidelijk aan tot **18,1-19,7 kts** (gust 23,2-28,8 kts), golf blijft bescheiden maar aanwezig (0,38-0,51m/5,9-6,6s) → scoort **Goed (a)** op meerdere punten (11:00, 14:00, 20:00), het meest overtuigende venster van de outlookperiode. Beste moment: **11:00-14:00** (18,1-19,1 kts, licht aanlandig).

**Beste dag: vrijdag 23 oktober**, met oplopende zuidwestelijke wind (18-20 kts) en een licht aanlandige hoek — het enige venster in deze outlookperiode dat een volledige categorie ("Goed (a)") haalt zonder te hoeven forceren. Kans: **gemiddeld** — dit ligt op dag 9 van de outlook en moet dichter bij de tijd opnieuw bevestigd worden, zeker gezien het GFS-overschattingspatroon dat deze week meerdere dagen zichtbaar was. Maandag 19 en dinsdag 20 oktober zijn interessante alternatieven voor wie van pittige, vlakke aflandige sessies houdt, maar de zeer hoge gust-factor en volledig aflandige hoek vragen om voorzichtigheid.
⚠️ Onzeker op 4+ dagen — check dichter bij de tijd opnieuw.

---
_Bronnen: Windfinder (GFS) · windwaarnemingen.nl (KNMI, IJmuiden) · Soarcast — deze run niet bereikbaar (JS-app, geen vindbaar/bereikbaar API-adres)_
