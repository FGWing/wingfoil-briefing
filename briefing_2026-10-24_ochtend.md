# 🌊 Wingfoil-briefing Zandvoort–Wijk aan Zee
_24-10-2026 · Ochtendbriefing_

⚠️ **Technische kanttekening:** Soarcast (JS/Vite-app zonder bereikbaar API-adres) was deze run niet te benaderen — net als alle voorgaande sessies. Windfinder is opgehaald via de onderliggende Astro-JSON (zowel de reguliere GFS-pagina als de Superforecast/SFC-pagina), windwaarnemingen.nl (IJmuiden) via de vsp-database-endpoints. Alle drie de resterende bronnen (Windfinder/GFS, Windfinder/SFC, windwaarnemingen.nl/KNMI) waren dus wél volledig bereikbaar, inclusief golf- en getijdata voor alle 72 uur én de outlook dag 4-9.

**Belangrijkste signaal deze run:** het stormbeeld van gisteren klopt in grote lijnen, maar met één belangrijke nuance voor **vandaag**: tussen de ochtendstorm en de avondstorm in zit een **verrassend goed venster rond 15:00-18:00** — wind zakt naar 19-23kts, richting draait naar side-shore, en de golf (1,8-2,1m/7-8s) is nog ruim boven de Optimaal-drempel. Dit stond gisteren niet zo scherp in beeld. Zondag blijft onverminderd **Slecht en gevaarlijk** (nu bevestigd door alle drie bronnen, inclusief Windfinders eigen SFC-model). Maandag levert na een korte naschok van de storm een **mooi Optimaal-venster vanaf circa 11:00-19:00** op — sterke cross-validatie tussen KNMI en SFC. De outlook bevestigt opnieuw **dinsdag 27 oktober** als beste dag.

---

## ⚡ Snel overzicht
- **Zaterdag:** Grensgeval **Optimaal/Goed**, kort venster rond **15:00-18:00** — ervoor en erna storm.
- **Zondag:** **Slecht en gevaarlijk** (storm), de hele dag — hoog vertrouwen, alle bronnen eens.
- **Maandag:** **Optimaal**, rond **11:00-19:00** (kern 13:00-17:00; gust neemt richting avond toe).
- **Beste dag in de 7 dagen erna:** dinsdag 27 oktober

---

## ⏰ Realitycheck vandaag
- Laatste actuele uren (windwaarnemingen.nl, IJmuiden, 05:00-07:10): **wind gem. ~31,3 kts, gust gem. ~38,6 kts, richting ~278-285° (WNW/West, vrij constant)**.
- Was voorspeld voor dezelfde uren: **KNMI-uurmodel** gaf gem. **~27,9 kts, gust ~40,3 kts, richting ~284°**. **Windfinder/GFS** (3-uurs, geïnterpoleerd) gaf voor dit venster **~27-28 kts gem., gust slechts ~30-31 kts**, dus duidelijk lager — vooral op de gust.
- Conclusie: de wind loopt **licht VOOR op het gemiddelde bij KNMI** (~+12%) en gust ligt daar **conform tot nipt onder** verwachting; **Windfinder/GFS onderschat zowel het gemiddelde als vooral de gust** fors (gust ~+25% te laag). Rest-van-de-dag inschatting: **vertrouwen in KNMI/SFC-modellen voor vandaag bevestigd en licht omhoog bijgesteld** — het middagvenster (zie hieronder) wordt met iets meer vertrouwen ingeschat, GFS-cijfers blijven voor vandaag als ondergrens lezen i.p.v. absoluut niveau.

---

## 📅 Komende 72 uur

### Zaterdag — Grensgeval Optimaal/Goed, kort venster 15:00-18:00 (storm ervoor en erna)
- Bij **Zandvoort/Wijk aan Zee**: de nacht en vroege ochtend (tot ~13:00) staan in het teken van de storm — richting pal aanlandig (270-305°, binnen 30° van Zandvoorts 287,5°), wind volgens **KNMI (leidend na de Realitycheck) 25-32 kts gemiddeld, gust 35-46 kts**, golf **2,2-2,8m / 7-9s** (Windfinder/GFS). Dat is pal aanlandig + grote branding zonder pierbescherming → **Slecht en gevaarlijk**, ook los van de windkracht zelf. Rond 13:00-14:00 draait de richting via licht aanlandig (260-251°) geleidelijk naar side-shore, en vanaf **~15:00 valt alles samen**: richting 250→196° (side-shore, kustlijnhoek), wind **19-23 kts gemiddeld (KNMI/SFC, onderling goed consistent), gust 23-30 kts**, golf nog **1,8-2,1m / 7-8s** — ruim boven de Optimaal-drempel (>1,1m, ≥5s). Dat is qua hoek/wind/golf-combinatie **Optimaal**, al is de gust (oplopend naar 28-30 kts tegen 18:00-19:00) stevig/pittig, vandaar "grensgeval" in de kop. Vanaf circa 20:00 loopt de wind met de volgende stormpuls alweer op naar 24-31 kts (gust 36-46 kts) bij richting 182-191° — ondanks de nog altijd goede side-shore hoek is dat te krachtig voor een normale sessie → weer **Slecht/gevaarlijk** in de late avond/nacht.
- Bij **IJmuiden/Wijk aan Zee** (pierzone-hoek, 240°/60°): 's ochtends (280-305°) valt dit in de **280°-360°-zone** → **IJmuiden** (Zuidpier) relatief rustiger, golf ruimschoots ≥0,8m. Tijdens het middagvenster (15:00-17:00, richting 250-224°) is dit bij de IJmuiden-pierzonehoek zelf nog **pal aanlandig** (binnen 210-270°) met golf 1,8-2,0m — dus pier-logica blijft relevant: richting valt in de **170°-250°-band** → **Wijk aan Zee** (Noordpier) is dan juist de rustigere/veiligere kant. Kortom: 's ochtends IJmuiden in het voordeel, 's middags Wijk aan Zee.
- Golven: 2,2-2,8m/7-9s 's ochtends/middags, afbouwend naar 1,8-2,1m/7-8s in het 15:00-19:00-venster, weer oplopend richting de nacht.
- Getij: hoogwater 03:06 (2,1m), laagwater 11:31 (0,4m), hoogwater 15:24 (1,9m), laagwater 23:23 (0,3m). Het middagvenster valt rond en net na hoogwater (15:24) — shorebreak kan dan nog iets verhoogd zijn, vooral meteen na 15:00.
- Bronnen: windwaarnemingen.nl (KNMI) en Windfinder Superforecast (SFC) liggen de hele dag dicht bij elkaar → eens (zie ook Realitycheck). Windfinder (GFS, 3-uurs) zit structureel lager, vooral op gust → wijkt af. Soarcast niet bereikbaar.

### Zondag — Slecht en gevaarlijk (storm), de hele dag — hoog vertrouwen
- Bij **Zandvoort/Wijk aan Zee**: na een korte overgangsfase vroeg in de nacht (richting zuid/ZZW, 191-221°) draait de wind vanaf circa 03:00-04:00 naar west/WZW (256-286°) en blijft daar de rest van de dag — dat is bij Zandvoort **vrijwel de hele dag pal aanlandig** (binnen 30° van 287,5°). Windkracht blijft extreem: **Windfinder/SFC (uurlijks, leidend qua detail) geeft 22,7-30,6 kts gemiddeld met gust 30,8-45,9 kts** door de hele dag heen; **windwaarnemingen.nl/KNMI geeft vergelijkbare orde van grootte maar met scherpere pieken** — rond 02:00-03:00 laat KNMI een extra scherpe piek zien (gem. tot ~39 kts, gust tot ~55 kts uit ZW) die SFC en GFS minder uitgesproken tonen, mogelijk een frontpassage waarvan het exacte tijdstip onzeker is. Golf (Windfinder, beide modellen) loopt de hele dag op van **2,2m naar bijna 3,0m, periode 7,9-9,1s** — torenhoge, langperiodieke deining. Zelfs het rustigste moment (04:00, 22,7 kts) is nog steeds pal aanlandig + enorme branding → ook dat is **Slecht en gevaarlijk**. Bij gust >27 kts uit W/ZW/NW (vrijwel de hele dag het geval) is sluiting van de pieren door de Reddingsbrigade IJmuiden zeer aannemelijk.
- Bij **IJmuiden/Wijk aan Zee** (pierzone-hoek): de richting (256-286°) balanceert de hele dag rond de grens van licht-aanlandig en de **250°-280°-neutrale zone** voor de pierzone-hoek — geen van beide pieren biedt een duidelijk/structureel voordeel. Golf ≥0,8m de hele dag aanwezig, maar met deze windkracht is de keuze tussen IJmuiden en Wijk aan Zee sowieso van ondergeschikt belang.
- Golven: 2,2-2,9m/7,9-9,1s, de hele dag, met een lichte piek in de vroege ochtend door de KNMI-frontpassage.
- Getij: hoogwater 02:40 (2,2m), laagwater 11:20 (0,4m), hoogwater 15:00 (2,0m), laagwater 18:56 (1,0m) — let op: deze laatste "laagwater" staat ongewoon hoog, wat duidt op opgestuwd water door de aanhoudende westelijke storm (stormvloed-effect); laagwater 23:08 (0,3m).
- Bronnen: Windfinder (SFC en GFS) liggen onderling dicht bij elkaar qua wind → eens. windwaarnemingen.nl/KNMI toont een scherpere piek rond 02:00-03:00 dan beide Windfinder-modellen → wijkt op dat punt af (zie boven), verandert de classificatie niet. Soarcast niet bereikbaar.

### Maandag — Optimaal rond 11:00-19:00 (kern 13:00-17:00), na ochtend-naschok van de storm
- Bij **Zandvoort/Wijk aan Zee**: tot circa 07:00 nog nawind van de Zondagstorm — richting west (271-276°, pal aanlandig), wind **20,6-25,6 kts (SFC), gust 26,2-29,8 kts**, golf nog **2,1-2,6m/7,4-8,6s** → pal aanlandig + grote branding, dus nog **Slecht/grensgeval** in de vroege ochtend. Vanaf 08:00 zakt de wind snel (17-18,4 kts) en draait de richting via licht aanlandig (265-253°) naar **side-shore vanaf circa 11:00** (241→202° tussen 11:00-16:00, daarna 194-189° tegen de avond) — en dat is precies waar wind (**15,4-19,5 kts, keurig in de 14-25 kts-band**), golf (**1,56-1,77m, ruim boven 1,1m**) en periode (**6,3-6,8s, boven 5s**) samen de **Optimaal**-criteria vormen. Dit beeld wordt sterk bevestigd door **windwaarnemingen.nl/KNMI**, dat voor dezelfde middaguren vrijwel identieke cijfers geeft (bv. 13:00: KNMI 14,4/21,8 kts bij 202° vs. SFC 15,8/20,9 kts bij 203°) — hoge cross-validatie. Richting de avond (17:00-19:00) blijft de hoek goed (189-194°, side-shore) en de wind bouwt licht uit (18,8-19,5 kts), maar de **gust loopt snel op (27,7→35,7 kts)** — nog steeds binnen de Optimaal-criteria qua gemiddelde, maar wel merkbaar pittiger.
- Bij **IJmuiden/Wijk aan Zee** (pierzone-hoek): 's ochtends (265-276°) valt dit in de **250°-280°-neutrale zone** — geen duidelijk piervoordeel. Vanaf het Optimaal-venster (241-203°, golf 1,6-1,8m ≥0,8m) schuift de richting naar de **170°-250°-band** → **Wijk aan Zee** (Noordpier) is dan de rustigere kant, en dit valt mooi samen met het beste venster van de dag voor Zandvoort/Wijk aan Zee zelf.
- Golven: 2,1-2,6m/7,4-8,6s 's ochtends, geleidelijk afbouwend naar 1,56-1,62m/6,3-6,8s tijdens en na het venster.
- Getij: hoogwater 03:16 (2,3m), laagwater 12:02 (0,45m), hoogwater 15:36 (2,15m). Het venster (11:00-17:00) valt rond opkomend/net voorbij hoogwater — shorebreak kan rond 15:00-16:00 nog iets verhoogd zijn door de restdeining van het weekend.
- Bronnen: windwaarnemingen.nl (KNMI) en Windfinder Superforecast (SFC) liggen zeer dicht bij elkaar, vooral tijdens het venster zelf → eens, hoog vertrouwen. Windfinder (GFS, 3-uurs) bevestigt dezelfde trend iets grover. Soarcast niet bereikbaar.

---

## 🔭 Kans op mooie sessies daarna (dag 4-9)
Windfinder (GFS, enige bron zo ver vooruit) voor **dinsdag 27 t/m zondag 1 november**:

- **Dinsdag 27 oktober — beste dag**: vrijwel de hele dag side-shore (189-258°, de kustlijnhoek), wind **17,9-23,8 kts**, golf **1,6-1,8m / periode 7,3-7,6s** — ruim boven de Optimaal-drempels. Gust is 's nachts en 's ochtends fors (31,6-38,8 kts), bouwt in de loop van de middag iets af (23,8-28,5 kts tegen 16:00). Richting de avond (19:00-22:00) schuift de hoek naar pal aanlandig (258-266°) bij nog altijd aanzienlijke golf (1,7-1,8m) → avond wordt dan weer **Slecht**. Beste venster: **07:00-16:00** (kern van de dag), met de meest comfortabele gust rond het midden van de middag.
- **Woensdag 28 oktober**: richting 245-267° (overwegend licht tot pal aanlandig), wind 16-17,3 kts, golf nog 1,6-1,9m — een combinatie die niet cleanmatcht met Optimaal/Goed(a) (richting net niet side-shore, golf net niet "klein genoeg"), dus **grensgeval/Matig**, met 's ochtends (pal aanlandig + golf >1,1m) eerder **Slecht**. Lager vertrouwen op de exacte uren.
- **Donderdag 29 oktober**: wind valt sterk terug (4,5-8,7 kts), golf kalmeert snel (1,1m→0,5m) → **Slecht/Matig** (te weinig wind, nagenoeg windstil).
- **Vrijdag 30 oktober**: nog altijd zwak (8,6-13,3 kts) met kleine golf (<0,65m) → **Matig** de hele dag, met een lichte verbetering in de avond (16,1-16,8 kts rond 19:00-22:00, richting 205-218° side-shore) maar golf blijft te klein voor Optimaal.
- **Zaterdag 31 oktober**: zwak en wisselvallig (5-14,3 kts), richting draait van aflandig/pal-aanlandig-achtig (244-312°) naar licht aanlandig (319-339°) — golf blijft klein (0,6-0,8m) → **Matig tot Slecht**, laag vertrouwen.
- **Zondag 1 november**: nagenoeg windstil (1-3,8 kts) → **Slecht** (geen wind), de hele dag.

**Beste dag: dinsdag 27 oktober**, met het langste en meest consistente side-shore-venster van de hele periode (18-24 kts, kern 07:00-16:00) — dezelfde dag die ook gisteren al als beste dag naar voren kwam, wat het vertrouwen in dit patroon vergroot. Kans: **hoog** voor dinsdag, **laag tot gemiddeld** voor de rest van de week (te weinig wind of ongunstige hoek).
⚠️ Onzeker op 4+ dagen — check dichter bij de tijd opnieuw, vooral woensdag (golfhoogte/richting-grensgeval) en het begin van de week erna.

---
_Bronnen: Windfinder (GFS 3-uurs + Superforecast/SFC uurlijks) · windwaarnemingen.nl (KNMI, IJmuiden) · Soarcast — deze run niet bereikbaar (JS-app, geen vindbaar/bereikbaar API-adres)_
