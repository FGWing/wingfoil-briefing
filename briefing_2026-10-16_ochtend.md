# 🌊 Wingfoil-briefing Zandvoort–Wijk aan Zee
_16-10-2026 · Ochtendbriefing_

⚠️ **Technische kanttekening:** Soarcast blijft onbereikbaar deze run (pure JS/Vite-app, `/web/locationinfo?...` levert alleen een lege HTML-shell zonder onderliggende data) — zelfde conclusie als alle voorgaande runs. Windfinder is opgehaald via de onderliggende Astro-island props op de reguliere forecast-pagina: één island (`ForecastSection`) bevatte dag 1-2 (16-17 okt) volledig, en een tweede island (`ForecastDataInit`) bevatte daarnaast al dag 3 t/m 10 (18-25 okt) in 3-uurs stappen — dus geen aparte Superforecast-pagina nodig. windwaarnemingen.nl (IJmuiden) is opgehaald via `database/vsp_vdg_wstats.php?st=IJmuiden1` (vandaag: 10-minuten-actuals + ingebed KNMI-uurmodel voor de hele dag) en `vsp_mrg_wstats.php?st=IJmuiden2` (morgen volledig + overmorgen t/m 16:00).

**Belangrijkste signaal deze run:** het GFS/KNMI-verschil van de afgelopen dagen zet onverminderd door, en wordt vandaag nog duidelijker. De actuals bij IJmuiden (06:00-07:10) liggen op 5,96-6,53 kts — dat is net iets hoger dan het KNMI-uurmodel voor diezelfde uren (5,0-5,3 kts), maar ruim onder Windfinder/GFS (8,3-9,1 kts voor de dichtstbijzijnde 3-uurspunten). Dit raakt niet alleen vandaag: voor zaterdag stemmen GFS en KNMI wél overeen over de windrichting (opbouwende noordelijke wind, de hele dag), maar GFS voorspelt 14-17 kts tegenover KNMI's 9-11 kts voor exact dezelfde uren — en voor zondag lopen zelfs de windrichtingen van de twee modellen volledig uit elkaar. Zie Realitycheck en de dagsecties hieronder voor hoe dit is verwerkt.

---

## ⚡ Snel overzicht
- **Vrijdag:** Windfinder ziet een opbouw naar **Optimaal in de avond** (20:00-23:00, 14,5-15,8 kts, side-shore noord, golf 1,14-1,16m/5,3-5,5s), maar het KNMI-model geeft voor diezelfde uren slechts ~9-11 kts — en de Realitycheck van vanochtend bevestigt dat de actuals tot nu toe dichter bij KNMI liggen dan bij GFS. Waarschijnlijker: **Matig, met kans op net Goed** in de avond.
- **Zaterdag:** **Grensgeval Goed/Optimaal**, het langste venster van de drie dagen — vrijwel de hele dag (02:00-20:00) side-shore noordelijke wind met mooie lange golfperiode (tot 7,9s). GFS en KNMI zijn het hier wel **eens over de richting**, maar GFS (14,2-17,1 kts) zit duidelijk hoger dan KNMI (9,3-11,2 kts). Beste moment: **11:00-20:00**, piek bij 17:00.
- **Zondag:** Windfinder ziet een ochtendopbouw naar **Optimaal om 08:00** (NO, 16,4 kts, golf 1,15m/7,9s), maar KNMI (beschikbaar t/m 16:00) ziet een compleet andere, veel zwakkere ochtend (2,5-6,8 kts) met een sterk afwijkende richting. Zeer **lage betrouwbaarheid** op dit venster — waarschijnlijk eerder Matig/Slecht. 's Middags draait de wind pal aflandig en valt verder weg.
- **Beste dag in de 7 dagen erna:** donderdag 22 oktober
_(De eerste 3 regels zijn altijd de eerstvolgende 3 volle dagen vanaf het moment van versturen.)_

---

## ⏰ Realitycheck vandaag

- Laatste actuele uren (windwaarnemingen.nl, IJmuiden, 06:00-07:10): **wind 5,96-6,53 kts, gust 6,55-7,42 kts, richting 187-194° (ZUID/ZZW)**.
- Was voorspeld voor dezelfde uren: het **ingebedde KNMI-uurmodel** gaf voor 06h/07h **192/197° (ZZW), 5,0-5,3 kts, gust 7,0-7,5 kts** — redelijk dicht bij de actuals, met de actuals zo'n 1-1,5 kts hoger. **Windfinder/GFS** gaf voor de dichtstbijzijnde 3-uurspunten (05h/08h) **197,9-204,4°, 8,3-9,1 kts, gust 14,7 kts** — bijna het dubbele van de werkelijke gust en duidelijk hoger qua gemiddelde.
- Conclusie: de wind loopt **ACHTER op Windfinder/GFS**, maar ligt **dicht bij (iets boven) windwaarnemingen.nl/KNMI**. Dit is al de derde/vierde ochtend op rij met dit beeld. Rest-van-de-dag inschatting: **naar beneden bijgesteld**. Het Windfinder-avondvenster (piek 15,8 kts om 20:00, classificatie Optimaal) krijgt beduidend minder vertrouwen; het KNMI-model zelf voorspelt voor vanavond (18:00-23:00) maar 8,8-11,1 kts (gust 13-17,5 kts). Met de ochtend-bias van +1 à 1,5 kts erbij komt de avond realistisch uit op **Matig, met een kans op net Goed** rond 20:00-21:00 — niet op het Optimaal-niveau dat GFS laat zien. Dit versterkt ook het voorbehoud bij zaterdag en vooral zondag hieronder, waar hetzelfde GFS/KNMI-gat (en bij zondag ook nog een richtingsverschil) zich voordoet.

---

## 📅 Komende 72 uur

### Vrijdag — Matig, met kans op net Goed in de avond (Windfinder zegt Optimaal)
- Bij **Zandvoort/Wijk aan Zee**: overdag (02:00-14:00) te weinig wind (7,7-10,5 kts, gust 11,5-18,5 kts) bij side-shore tot licht/pal aanlandige richting (198-281°) → **Slecht/Matig**. Vanaf **17:00** draait de wind naar **noord** (355-3°, side-shore) en loopt op naar **15,8 kts (gust 19,3 kts) om 20:00** en **14,5 kts om 23:00**, golf 0,94-1,16m/4,5-5,5s → dat scoort bij Windfinder **Optimaal** op de twee avondpunten. Het KNMI-model ziet dezelfde richtingsdraai (ook noord vanaf de avond) maar met veel minder kracht: 18:00-23:00 slechts **8,8-11,1 kts** (gust 13-17,5 kts). Gezien de Realitycheck hierboven (actuals dicht bij KNMI, niet GFS) is **Matig tot net Goed de waarschijnlijkere uitkomst** voor vanavond, niet Optimaal.
- Bij **IJmuiden/Wijk aan Zee** (pierzone-hoek): overdag kortstondig (licht) aanlandig bij lage golf (<0,8m) → geen piervoordeel van toepassing; 's avonds draait het naar side-shore, ook geen pier-logica relevant.
- Golven (Windfinder, enige golfbron): 0,59-1,16m / 4,44-5,54s.
- Getij: laagwater 03:29 (0,39m), hoogwater 07:40 (1,90m), laagwater 15:46 (0,36m), hoogwater 19:54 (2,07m).
- Bronnen: Windfinder (GFS) en windwaarnemingen.nl (KNMI) zijn het **eens over de richting** (zuid → noord gedurende de dag) maar wijken **fors af in windkracht** — GFS tot 15,8 kts tegenover KNMI maar tot 11,1 kts. De Realitycheck hierboven bevestigt dat de actuals tot nu toe de KNMI-lijn volgen (iets erboven). Soarcast niet bereikbaar.

### Zaterdag — Grensgeval Goed/Optimaal (langste venster van de drie dagen)
- Bij **Zandvoort/Wijk aan Zee**: vrijwel de **hele dag** (02:00-20:00) side-shore noordelijke richting (355-31°) met wind **14,2-17,1 kts** (gust 17,1-19,8 kts) en een opbouwende, lange golfperiode (**1,18-1,5m / 5,6-7,9s**) → dit scoort **Optimaal** op 6 van de 8 Windfinder-punten, het langste venster van de komende 72 uur. Beste moment: **17:00** (golf piekt op 1,46m/6,92s). Het KNMI-model stemt qua **richting goed overeen** (ook consequent noord, 342-32°) — dat geeft vertrouwen in de hoek — maar geeft voor dezelfde uren maar **9,3-11,2 kts** (gust 10,3-17,5 kts), duidelijk zwakker dan GFS. Met dat zwakkere windcijfer (maar wel de goede golf van Windfinder, enige golfbron) komt de dag op **Goed (b)** uit in plaats van Optimaal — vandaar het grensgeval. Gezien het GFS-overschattingspatroon van deze week is enige voorzichtigheid met de Optimaal-classificatie verstandig, maar dit is wel duidelijk de beste van de drie dagen.
- Bij **IJmuiden/Wijk aan Zee** (pierzone-hoek): de richting blijft de hele dag side-shore t.o.v. de pierzone-hoek (240°) → geen piervoordeel van toepassing (niet aanlandig).
- Golven (Windfinder, enige golfbron): 1,18-1,50m / 5,62-7,79s.
- Getij: laagwater 03:56 (0,44m), hoogwater 08:11 (1,83m), laagwater 16:17 (0,36m), hoogwater 20:28 (1,97m).
- Bronnen: Windfinder (GFS) en windwaarnemingen.nl (KNMI) zijn het **eens over de richting** (noord, de hele dag) maar wijken **fors af in windkracht** (GFS ~14-17 kts, KNMI ~9-11 kts) — zelfde patroon als de voorgaande dagen. Soarcast niet bereikbaar.

### Zondag — Onzeker: Windfinder ziet Optimaal-ochtend, KNMI een heel ander beeld
- Bij **Zandvoort/Wijk aan Zee**: Windfinder laat de wind 's ochtends (02:00-11:00) geleidelijk opbouwen uit **NO/NNO** (37-50°, side-shore t.o.v. de kust) naar **16,4 kts (gust 21,6 kts) om 08:00**, golf 1,15m met een lange periode van 7,9s → dat scoort **Optimaal** op dat punt. Het KNMI-model (beschikbaar t/m 16:00) ziet echter een **compleet andere ochtend**: richting draait snel van NNW naar oost/ONO, en de wind blijft de hele ochtend zwak (**2,5-6,8 kts**) — zowel richting als kracht wijken sterk af van Windfinder. Gezien dit grote verschil (en het aanhoudende GFS-overschattingspatroon van deze week) krijgt het Optimaal-venster van 08:00 **zeer lage betrouwbaarheid** — reken eerder op **Matig/Slecht**. 's Middags draait de wind bij Windfinder naar **pal aflandig** (73-92°) en valt terug naar 8,9-11,5 kts → **Slecht/Matig**, ongeacht welk model gelijk heeft.
- Bij **IJmuiden/Wijk aan Zee** (pierzone-hoek): de ochtendrichting leest bij IJmuiden als pal aflandig, 's middags eveneens pal/licht aflandig → geen piervoordeel van toepassing (niet aanlandig).
- Golven (Windfinder, enige golfbron): 0,64-1,35m / 7,28-7,97s (ochtend het hoogst/langst).
- Getij: laagwater 04:38 (0,49m), hoogwater 08:45 (1,73m), laagwater 16:58 (0,37m), hoogwater 21:11 (1,82m).
- Bronnen: Windfinder (GFS) en windwaarnemingen.nl (KNMI) wijken deze dag **zowel in richting als in windkracht extreem af** — het grootste verschil van de drie dagen. Check dit venster dicht bij de tijd opnieuw, idealiter met een vers KNMI-uurmodel voor de middag/avond (nu nog niet beschikbaar). Soarcast niet bereikbaar.

---

## 🔭 Kans op mooie sessies daarna (dag 4-9)
Windfinder (GFS, enige bron zo ver vooruit, 3-uurs resolutie) voor **maandag 19 t/m zaterdag 24 oktober**:

- **Maandag 19 oktober**: de **hele dag pal aflandig** (84-94°), wind 8,9-14,3 kts, golf laag (0,36-0,58m) → grotendeels **Slecht/Matig**, vlak water door de aflandige hoek.
- **Dinsdag 20 oktober**: nog steeds pal aflandig (87-130°), wind pakt duidelijk aan tot **12,1-17,4 kts** maar met **zeer forse gust** (19,1-27,9 kts — bijna het dubbele van het gemiddelde) en golf blijft zeer laag (0,25-0,29m) → **grensgeval Goed/Matig**, een pittige maar compleet vlakke sessie voor wie tegen de gustiness kan.
- **Woensdag 21 oktober**: richting draait via aflandig naar side-shore (162-215°), wind sterk oplopend (9,3-22,9 kts) maar golf blijft net onder de 1,1m-drempel (0,25-0,73m, oplopend) → meerdere punten **grensgeval Optimaal/Goed** (vooral 11:00-23:00): wind en richting zijn al goed, de golf moet nog iets opbouwen.
- **Donderdag 22 oktober — beste dag**: start **zeer winderig** (27-31 kts uit het WZW om 02:00-05:00 — bij >27 kts uit W/ZW/NW sluit de Reddingsbrigade IJmuiden normaliter de pieren voor wandelaars, een onafhankelijk signaal dat het die ochtend ruw is), rond het middaguur (08:00) al **Goed (a)** (19,4 kts, licht aanlandig, golf 0,98m) en vanaf **14:00-23:00** draait de richting naar **side-shore** met golf die mooi boven de 1,1m-drempel komt (1,14-1,26m/6,2-6,5s) bij **14,4-19,7 kts** → scoort **Optimaal** op vier punten (14:00, 17:00, 20:00, 23:00), het meest overtuigende en langste venster van de outlookperiode op comfortabele tijden. Beste moment: **14:00-20:00**.
- **Vrijdag 23 oktober**: blijft winderig en golfrijk (16,8-28 kts, golf 1,31-1,45m/6,3-6,55s, side-shore), maar op meerdere punten (08:00, 11:00, 14:00, 23:00) komt de wind **boven de 25 kts-Optimaal-grens** uit (tot 28 kts) → geweldige golf, maar voor ervaren foilers; de punten binnen de Optimaal-marge (02:00, 05:00, 17:00, 20:00) vallen helaas op minder praktische tijden dan donderdag.
- **Zaterdag 24 oktober**: 's ochtends (02:00-08:00) nog **Optimaal** (23,6-24,3 kts, golf 1,29-1,34m, side-shore), maar de wind blijft oplopen tot **32,8 kts** rond het middaguur en draait vanaf 17:00 **pal aanlandig** (263°) met golf van 1,4m → dat combineert tot **Slecht** (grote branding, pal aanlandig, geen pierbescherming bij Zandvoort/Bloemendaal) in de namiddag/avond.

**Beste dag: donderdag 22 oktober**, met een rustige, comfortabele Optimaal-middag/avond (14:00-20:00, 14-20 kts, side-shore, golfperiode ~6,5s) na een winderige, ruwe ochtend. Kans: **gemiddeld tot hoog** — dit is wel dag 7 van de outlook en moet dichter bij de tijd opnieuw bevestigd worden, zeker gezien het GFS-overschattingspatroon dat deze week meerdere dagen zichtbaar was (al gaat het hier om een periode met zoveel wind dat een correctie naar beneden nog steeds een prima sessie kan opleveren). Vrijdag 23 en zaterdag 24 oktober (ochtend) zijn stevige alternatieven voor wie van golfrijke, krachtige sessies houdt, maar vragen ervaring met wind rond en boven de 25 kts.
⚠️ Onzeker op 4+ dagen — check dichter bij de tijd opnieuw.

---
_Bronnen: Windfinder (GFS) · windwaarnemingen.nl (KNMI, IJmuiden) · Soarcast — deze run niet bereikbaar (JS-app, geen vindbaar/bereikbaar API-adres)_
