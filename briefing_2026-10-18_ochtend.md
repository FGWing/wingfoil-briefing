# 🌊 Wingfoil-briefing Zandvoort–Wijk aan Zee
_18-10-2026 · Ochtendbriefing_

⚠️ **Technische kanttekening:** Soarcast blijft onbereikbaar deze run (pure JS/Vite-app, `/web/locationinfo?...` levert alleen een lege HTML-shell zonder onderliggende data, en ook de JS-bundel bevat geen vindbaar API-adres) — zelfde conclusie als alle voorgaande runs. Windfinder is opgehaald via de onderliggende Astro-island props op de reguliere forecast-pagina: het `ForecastSection`-island bevatte vandaag+morgen (18-19 okt, 3-uurs resolutie) en het `ForecastDataInit`-island daarnaast al overmorgen t/m dag 10 (20-27 okt, ook 3-uurs) — dus geen aparte Superforecast-pagina nodig. windwaarnemingen.nl (IJmuiden) is opgehaald via `database/vsp_vdg_wstats.php?st=IJmuiden1` (vandaag: 10-minuten-actuals t/m 07:10 + ingebed KNMI-uurmodel voor de hele dag) en `vsp_mrg_wstats.php?st=IJmuiden2` (morgen volledig + overmorgen t/m 16:00).

**Belangrijkste signaal deze run:** het GFS/KNMI-verschil zet onverminderd door, nu al voor de derde ochtend/dag op rij in deze reeks briefings, en is vrijwel even extreem als gisteren. Windfinder/GFS laat voor **vandaag** vroeg in de ochtend nog 10,5-14,1 kts zien, maar de actuals bij IJmuiden (05:00-07:10) liggen op slechts 5,0-6,33 kts en het ingebedde KNMI-uurmodel voorspelt voor de **hele dag** nooit meer dan ~8,1 kts. De Realitycheck hieronder bevestigt dat de actuals dicht bij KNMI liggen, niet bij GFS — en datzelfde gat (GFS ongeveer het dubbele van KNMI) komt vrijwel identiek terug op maandag en dinsdag. Hierdoor wordt de hele 72-uursperiode als **Slecht tot hoogstens een laag-vertrouwen grensgeval** ingeschat. Positief nieuws zit verderop in de outlook: **zaterdag 24 oktober** springt er dit keer uit als beste dag, met donderdag 22 oktober (al meermaals genoemd in eerdere briefings) als sterk alternatief.

---

## ⚡ Snel overzicht
- **Zondag:** Windfinder/GFS claimde vroeg in de ochtend nog 10,5-14,1 kts (side-shore), maar de Realitycheck van vanochtend en het KNMI-uurmodel laten voor de hele dag nooit meer dan ~8,1 kts zien. **Slecht** de hele dag, met een klein, onzeker grensgeval rond het middaguur.
- **Maandag:** richting blijft pal aflandig (OOST, 85-93°); GFS (12,0-16,2 kts) en KNMI (4,9-8,6 kts) wijken opnieuw extreem af, en golf is vlak (0,40-0,58m, ruim onder de 1,1m-drempel). **Slecht** de hele dag.
- **Dinsdag:** tot 16:00 bevestigt KNMI hetzelfde gat met GFS (GFS 14,0-15,6 kts vs KNMI 6,6-9,0 kts, pal aflandig, golf vlak 0,34-0,38m). Na 16:00 (buiten KNMI-bereik) claimt GFS een opleving naar side-shore met 14,2-16,2 kts, maar golf blijft zwak en is onbevestigd. **Slecht/Matig**, met een laag-vertrouwen grensgeval rond 20:00-23:00.
- **Beste dag in de 7 dagen erna:** zaterdag 24 oktober
_(De eerste 3 regels zijn altijd de eerstvolgende 3 volle dagen vanaf het moment van versturen.)_

---

## ⏰ Realitycheck vandaag

- Laatste actuele uren (windwaarnemingen.nl, IJmuiden, 05:00-07:10): **wind 5,0-6,33 kts (laatste punt 07:10: 6,33 kts), gust 5,94-8,64 kts, richting 27,6-69,6° (NNO draaiend via NO naar ONO)**.
- Was voorspeld voor dezelfde uren: het **ingebedde KNMI-uurmodel** gaf voor 05h/06h/07h **40°/5,3 kts/gust 7,9 · 40°/5,0 kts/gust 8,0 · 63°/6,3 kts/gust 9,7** — nauwelijks afwijkend van de actuals, zowel qua kracht als richting. **Windfinder/GFS** gaf voor de vergelijkbare 3-uurspunten (05:00/08:00) **48°/10,5 kts/gust 18,7** en **46°/12,4 kts/gust 20,6** — ruim het dubbele van de actuele wind.
- Conclusie: de wind loopt **ACHTER op Windfinder/GFS**, maar ligt **dicht bij windwaarnemingen.nl/KNMI**. Dit is al de derde dag op rij met dit beeld in deze briefingreeks. Rest-van-de-dag inschatting: **fors naar beneden bijgesteld**. Het KNMI-uurmodel (dat vanochtend goed bleek te kloppen) voorspelt voor de rest van de dag nooit meer dan **~8,1 kts** (12:00, gust 13,1) — dat is het reële beeld, niet de 10-14 kts die GFS voor de ochtend liet zien. Dit versterkt ook het voorbehoud bij maandag en dinsdag hieronder, waar hetzelfde GFS/KNMI-gat terugkomt.

---

## 📅 Komende 72 uur

### Zondag — Slecht (GFS-cijfers niet bevestigd door KNMI/actuals)
- Bij **Zandvoort/Wijk aan Zee**: Windfinder/GFS liet vroeg vanochtend (02:00) nog 14,1 kts/gust 21,8 zien (side-shore, golf 1,29m/7,9s — dat moment is al voorbij), en zakt daarna zelf ook af (05:00-11:00: 10,5-12,8 kts, golf 0,99-1,14m). Het KNMI-uurmodel en de actuals van vanochtend (zie Realitycheck) liggen voor de hele dag nog veel lager: nooit meer dan **~8,1 kts** (12:00, gust 13,1), ruim onder de Matig-drempel (gust<16 én gem<14 kts → Slecht). Richting draait van side-shore ('s ochtends) naar licht/pal aflandig (vanaf 14:00, 65-87°). Realistisch: **Slecht** de hele dag, met een kleine kans op een kortstondig grensgeval rond het middaguur.
- Bij **IJmuiden/Wijk aan Zee** (pierzone-hoek): richting leest de hele dag als (licht) aflandig t.o.v. de pierzone-hoek (240°) → geen piervoordeel van toepassing (niet aanlandig).
- Golven (Windfinder, enige golfbron): 0,65-1,29m / 7,12-7,98s, afbouwend door de dag — let op: dezelfde GFS-bron die de wind vanochtend fors overschatte, dus ook hier enige voorzichtigheid.
- Getij: laagwater 04:38 (0,49m), hoogwater 08:45 (1,73m), laagwater 16:58 (0,37m), hoogwater 21:11 (1,82m).
- Bronnen: Windfinder (GFS) en windwaarnemingen.nl (KNMI) zijn het **eens over de richting** (side-shore → aflandig) maar wijken **fors af in windkracht** (GFS ruim het dubbele) — bevestigd door de Realitycheck hierboven. Soarcast niet bereikbaar.

### Maandag — Slecht (aanhoudend GFS/KNMI-gat, vlak water)
- Bij **Zandvoort/Wijk aan Zee**: richting blijft de hele dag **pal aflandig** (85-93°, OOST). Windfinder/GFS geeft **12,0-16,2 kts** (gust 17,7-25,2) maar het KNMI-uurmodel geeft voor exact dezelfde uren slechts **4,9-8,6 kts** (gust 8,2-14,1) — hetzelfde aanhoudende verschil als vandaag zet onverminderd door. Golf is bovendien flink onder de 1,1m-drempel (**0,40-0,58m**). Gezien de Realitycheck van vanochtend (actuals dicht bij KNMI, niet bij GFS) is **Slecht** de realistische inschatting voor de hele dag.
- Bij **IJmuiden/Wijk aan Zee** (pierzone-hoek): richting leest ook hier als (licht/pal) aflandig → geen piervoordeel van toepassing.
- Golven (Windfinder, enige golfbron): 0,40-0,58m / 4,68-9,19s — vlak water, ongeacht welk windmodel gelijk heeft.
- Getij: laagwater 05:30 (0,55m), hoogwater 09:37 (1,57m), laagwater 17:49 (0,41m), hoogwater 22:56 (1,67m).
- Bronnen: Windfinder (GFS) en windwaarnemingen.nl (KNMI) eens over de richting (pal aflandig, OOST), windkracht wijkt weer fors af (GFS ±2x KNMI). Soarcast niet bereikbaar.

### Dinsdag — Slecht/Matig (grensgeval laat op de dag, laag vertrouwen)
- Bij **Zandvoort/Wijk aan Zee**: tot 16:00 bevestigt het KNMI-uurmodel (beschikbaar t/m 16:00) hetzelfde GFS/KNMI-gat: GFS **14,0-15,6 kts** vs KNMI **6,6-9,0 kts**, beide pal aflandig (OOST/OZO, 88-103°), golf vlak (0,34-0,38m). Na 16:00 (buiten KNMI-bereik) laat GFS de richting draaien naar **side-shore** (159-190°) met **14,2-16,2 kts** (gust 23,2-24,9) — dat zou een grensgeval Matig/Goed opleveren, maar de golf blijft zwak (0,28-0,32m/2,7-3,0s, niet de >1,1m/≥5s die voor Optimaal nodig is) en is, gezien het patroon van de afgelopen dagen, niet vertrouwd zonder KNMI-bevestiging. Realistisch: **Slecht** tot 16:00, daarna op zijn best een laag-vertrouwen grensgeval **Matig** rond 20:00-23:00.
- Bij **IJmuiden/Wijk aan Zee** (pierzone-hoek): richting leest de hele dag als (licht/pal) aflandig of side-shore → geen piervoordeel van toepassing (niet aanlandig).
- Golven (Windfinder, enige golfbron): 0,28-0,38m / 2,69-3,54s — vlak, kortperiodiek lokaal windzeetje.
- Getij: laagwater 06:31 (0,59m), hoogwater 11:12 (1,43m), laagwater 18:50 (0,45m).
- Bronnen: Windfinder (GFS) en windwaarnemingen.nl (KNMI, t/m 16:00) eens over de richting, windkracht wijkt fors af. Na 16:00 geen KNMI-cijfers meer beschikbaar om GFS te toetsen. Soarcast niet bereikbaar.

---

## 🔭 Kans op mooie sessies daarna (dag 4-9)
Windfinder (GFS, enige bron zo ver vooruit, 3-uurs resolutie) voor **woensdag 21 t/m maandag 26 oktober**:

- **Woensdag 21 oktober**: richting draait van zuid/zuidwest (189-227° 's nachts/ochtend) via zuidwest (176-191° rond het midden van de dag) naar side-shore (215-222°) in de avond; wind bouwt op van 13,6 naar 22,2 kts. Overdag (05:00-14:00) blijft de golf nog onder de 1,1m-drempel (0,42-0,91m) → grensgeval Matig, maar vanaf **17:00** bouwt de golf door naar 1,12-1,51m (periode 6,0-6,6s) en wordt het **Optimaal** (wind 21,0-22,2 kts, gust 27,7-31,4 kts). Beste venster: **17:00-23:00**.
- **Donderdag 22 oktober**: vrijwel de hele dag **Optimaal** — van 02:00 tot 14:00 blijft de wind 19,6-24,5 kts (gust 24,8-33,8 kts), side-shore (192-233°), met golf 1,45-1,71m/6,5-6,8s. Vanaf 17:00 draait de richting naar licht aanlandig (243-253°) en zakt de wind geleidelijk (13,6-16,8 kts) naar Goed(a)/Goed(b), om tegen 23:00 (9,3 kts) in Slecht te eindigen. Beste venster: **08:00-14:00** (daglicht-Optimaal, iets minder extreme gust dan de nachturen). Dit is dezelfde dag die ook in eerdere briefings al als sterke kandidaat naar voren kwam — een geruststellende bevestiging over meerdere modelruns.
- **Vrijdag 23 oktober**: zeer winderig — om 14:00 zelfs **34,7 kts/gust 44,2 kts** (stormachtig; richting komt hier uit het zuidwest/zuid, 204-228°, dus niet exact de W/ZW/NW-hoek die de Reddingsbrigade-sluiting triggert, maar wel te ruw voor een normale sessie). Golf loopt flink op (1,35-2,02m/6,5-7,5s). Vroeg (05:00-08:00: 18,7-24,7 kts, side-shore/licht aflandig) en laat (20:00: 22,8 kts, side-shore) zijn de meest beheersbare Optimaal-vensters; het middaguur (11:00-17:00: 26,6-34,7 kts) is alleen voor zeer ervaren foilers. Om 23:00 draait de richting naar licht aanlandig (248°) met golf 2,02m (≥0,8m) → **piervoordeel van toepassing**: dit valt net binnen de ~170-250°-zone, dus **Wijk aan Zee** (Noordpier) relatief rustiger.
- **Zaterdag 24 oktober — beste dag**: de hele dag Goed(a) of beter, zonder één Slecht-moment. 's Nachts/vroege ochtend (02:00-05:00) licht aanlandig (249-250°) met grote golf (1,99-2,02m/7,5s) → Goed(a), en vanaf **08:00** draait de richting naar side-shore (209-227°) en blijft het de rest van de dag **Optimaal** tot 20:00 (18,0-22,6 kts, gust 23,9-28,2 kts — merkbaar minder gusty/pieky dan donderdag, golf 1,79-1,99m/7,1-7,4s), om 23:00 weer terug naar licht aanlandig (256°, Goed(a)). Beste venster: **08:00-20:00** — het langste en meest consistente venster van de hele outlookperiode. Piervoordeel 's ochtends (02:00-05:00, licht aanlandig 249-250°, golf ≥0,8m): valt net binnen de ~170-250°-zone → **Wijk aan Zee** (Noordpier) relatief rustiger dan IJmuiden.
- **Zondag 25 oktober**: start **Slecht** (02:00-07:00, pal aanlandig uit het westen 259-261° met golf 1,67-1,70m → grote branding, geen pierbescherming bij Zandvoort/Bloemendaal; bij IJmuiden/Wijk aan Zee valt deze hoek net in de 250-280°-neutrale zone, dus ook daar geen duidelijk piervoordeel), draait daarna via licht aflandig (10:00: 64°) naar side-shore (13:00: 55°) met een kort **Optimaal**-venster om 13:00 (14,7 kts/gust 18,5, golf 1,91m/7,5s), gevolgd door een snel wegvallende namiddag/avond terug naar Slecht. Smal venster: **13:00-16:00**.
- **Maandag 26 oktober**: wind blijft de hele dag zwak (5,5-8,4 kts, gust 7,3-12,9 kts) en pal aflandig/side-shore (50-115°) → **Slecht** de hele dag, ondanks een nog steeds forse golf (1,46-1,71m) die puur oude deining is, niet lokaal windgedreven.

**Beste dag: zaterdag 24 oktober**, met het langste en meest consistente venster van de hele outlookperiode (08:00-20:00, Optimaal, 18-22,6 kts, side-shore, golf ~1,8-2,0m/~7,2s) en geen enkel Slecht-moment op de hele dag. Donderdag 22 oktober is een sterk, bijna even goed alternatief (lange Optimaal-periode 02:00-14:00), maar wel gustier (tot 33,8 kts) en met een zwakkere avond. Kans: **gemiddeld tot hoog** voor beide dagen.
⚠️ Onzeker op 4+ dagen — check dichter bij de tijd opnieuw. Let vooral op: het GFS-overschattingspatroon dat dag 1-3 van deze briefing domineert (GFS ruim 2x hoger dan KNMI) is tot nu toe vooral bij de zwakkere winddagen gezien; bij deze stormachtige/stevige outlookdagen is dat patroon niet apart getoetst, maar een correctie naar beneden bij het dichterbij komen van donderdag/zaterdag is niet uit te sluiten.

---
_Bronnen: Windfinder (GFS) · windwaarnemingen.nl (KNMI, IJmuiden) · Soarcast — deze run niet bereikbaar (JS-app, geen vindbaar/bereikbaar API-adres)_
