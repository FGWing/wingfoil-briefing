# 🌊 Wingfoil-briefing Zandvoort–Wijk aan Zee
_23-10-2026 · Ochtendbriefing_

⚠️ **Technische kanttekening:** geen browser beschikbaar deze sessie, dus Soarcast (JS/Vite-app, lege HTML-shell zonder vindbaar API-adres) is — net als alle voorgaande runs — niet bereikbaar. Windfinder is opgehaald via de onderliggende Astro-JSON: dit gaf voor **vandaag en morgen (vrijdag/zaterdag) de volledige dataset inclusief golf/getij** (GFS 3-uurs + de uurlijkse Superforecast), maar voor **zondag en de outlook (dag 4-9) alleen windrichting/-kracht (GFS 3-uurs) — géén golfdata**, omdat die dagtabs clientside via JavaScript worden geladen en dat deze sessie niet uitvoerbaar is. Windsnelheid stond in de ruwe JSON in m/s en is omgerekend (×1,94384) naar kts. windwaarnemingen.nl (IJmuiden) is opgehaald via `database/vsp_vdg_wstats.php?st=IJmuiden1` (actuals t/m 07:10 + volledig KNMI-uurmodel voor de rest van vandaag) en `database/vsp_mrg_wstats.php?st=IJmuiden2` (zaterdag volledig + zondag t/m 16:00).

**Belangrijkste signaal deze run:** de Realitycheck bevestigt opnieuw dat **GFS fors overschat** (~30-35%), terwijl **KNMI en de Superforecast (SFC) vandaag beide dicht bij de actuals liggen** (anders dan gisteren, toen SFC net zo hard overschatte als GFS). Groter nieuws: het **stormscenario voor zaterdag is nu door alle bronnen bevestigd als zwaar** — waar KNMI gisteren nog een veel milder beeld gaf (gust 20-23kt), laat het bijgewerkte KNMI-model vandaag zelf ook gust 40-48kt zien, nagenoeg gelijk aan GFS. Zondag zet de storm onverminderd door (mogelijk nog heftiger). De outlook bevestigt **dinsdag 27 oktober** opnieuw als de beste dag, met een goed alternatief maandagavond.

---

## ⚡ Snel overzicht
- **Vrijdag:** grensgeval, **nipt onder Optimaal**, rond **09:00-17:00** (sterkste combinatie 12:00-16:00) — daarna draait het ongunstig en bouwt de storm zich op.
- **Zaterdag:** **Slecht en gevaarlijk** (storm) vrijwel de hele dag — nu hoog vertrouwen, alle drie bronnen eens.
- **Zondag:** **Slecht en gevaarlijk** (storm) de hele dag, mogelijk nog heftiger dan zaterdag.
- **Beste dag in de 7 dagen erna:** dinsdag 27 oktober
_(De eerste 3 regels zijn altijd de eerstvolgende 3 volle dagen vanaf het moment van versturen.)_

---

## ⏰ Realitycheck vandaag

- Laatste actuele uren (windwaarnemingen.nl, IJmuiden, 06:00-07:10): **wind 14,3-15,0 kts (gem. ~14,7), gust 20,4-22,2 kts (gem. ~21,1), richting 148-152° (ZZO, vrij constant)**.
- Was voorspeld voor dezelfde uren: **KNMI-uurmodel** (ingebed op dezelfde pagina) gaf voor 06h/07h **149°/14,6 kts/gust 22,9 · 150°/14,6 kts/gust 22,9** (gem. 14,6/22,9) — nagenoeg identiek aan de actuals. **Windfinder/GFS** (3-uurs) gaf voor 05:00/08:00 **151°/17,9 kts/gust 28,3** en **158°/21,6 kts/gust 32,8** (voor 06-07h geïnterpoleerd ~19-20/~30) — duidelijk hoger. **Windfinder Superforecast** (uurlijks) gaf voor 06h/07h **162°/17,4 kts/gust 29,0 · 165°/17,2 kts/gust 28,5** — ook hoger, maar minder extreem dan GFS.
- Conclusie: de wind loopt **conform verwachting bij KNMI** (vrijwel exacte match), maar **ACHTER op zowel Windfinder/GFS (~30-35% te hoog) als de Superforecast (~15-20% te hoog)**. Rest-van-de-dag inschatting: **leunen op KNMI (en in mindere mate SFC), GFS-cijfers voor vandaag met een correctiefactor van circa -30% lezen.**

---

## 📅 Komende 72 uur

### Vrijdag — Grensgeval, nipt onder Optimaal, rond 09:00-17:00 (gemiddeld-hoog vertrouwen voor wind/richting, golf net onder de drempel)
- Bij **Zandvoort/Wijk aan Zee**: richting draait geleidelijk van ZZO (144-158°, 08:00-13:00, licht aflandig/side-shore) naar vrijwel pal aflandig (100-131°, 14:00-19:00). Wind volgens **KNMI/Superforecast** (onderling goed consistent, leidend na de Realitycheck): **16-18 kts gemiddeld, gust 26-31 kts** tussen 09:00-17:00, pieken rond 12:00-16:00. **Windfinder/GFS geeft voor dezelfde uren 21,6-26,8 kts (gust 32,5-39,3)** — gezien de Realitycheck van vandaag niet te vertrouwen als absoluut niveau, maar een indicatie dat de bovenkant van de bandbreedte niet volledig valt uit te sluiten. Golf (Superforecast, uurlijks) blijft het hele venster **hardnekkig net op/onder de 1,1m-grens: 0,99-1,09m, periode 5,8-7,2s** (periode ruim boven de 5s-drempel, maar golfhoogte net niet over de 1,1m-grens heen) — vandaar het "nipt onder Optimaal"-oordeel in plaats van voluit Optimaal. Na 18:00 valt de wind bij KNMI terug (13-15 kts) en draait de richting via side-shore (68-33°) naar licht/pal aanlandig (315-335° rond 21:00-22:00, 303-289° rond 23:00) terwijl de golf juist oploopt tot 1,2-1,5m — per saldo een ongunstige combinatie voor de late avond (minder relevant want wind dan zwakker).
- Bij **IJmuiden/Wijk aan Zee** (pierzone-hoek, 240°/60°): pas rond 22:00-23:00 wordt de richting (250-263°) grensgeval aanlandig, en valt precies in de **neutrale pierzone (250°-280°)** — geen van beide pieren biedt dan duidelijk voordeel. Golf is dan wel ≥0,8m (1,4-1,5m), maar windkracht is op dat late uur al te zwak voor een zinvolle sessie, dus praktisch beperkt belang.
- Golven: 0,88-1,09m/5,3-7,2s overdag, oplopend naar 1,2-1,54m/7,0-7,1s in de late avond als de storm nadert.
- Getij: hoogwater 02:31 (1,98m), laagwater 10:37 (0,4m), hoogwater 14:50 (1,75m), laagwater 22:33 (0,29m). Het beste venster (12:00-16:00) valt rond opkomend water richting hoogwater — shorebreak kan tegen 14:50-16:00 iets toenemen.
- Bronnen: windwaarnemingen.nl (KNMI) en Windfinder Superforecast (uurlijks) zitten dicht bij elkaar en bij de actuals → eens. Windfinder (GFS, 3-uurs) zit duidelijk hoger → wijkt af, zie Realitycheck. Soarcast niet bereikbaar.

### Zaterdag — Slecht en gevaarlijk (storm), nu hoog vertrouwen (alle drie bronnen eens)
- Bij **Zandvoort/Wijk aan Zee**: richting is vanaf middernacht tot in de namiddag grotendeels NW/W (280-305° volgens KNMI, 255-293° volgens GFS) — dat is bij Zandvoort **pal aanlandig** (binnen 30° van 287,5°) vrijwel de hele ochtend, en bij **Wijk aan Zee** (pal aanlandig 283,8°) net zo. Windkracht is deze keer **niet meer omstreden**: **windwaarnemingen.nl/KNMI geeft 22-34 kts gemiddeld met gust 31-48 kts**, **Windfinder/GFS geeft 25-33 kts (gust 28-46 kts)** — de twee modellen liggen nu binnen elkaars bereik (anders dan eerdere runs, waar KNMI veel milder leek). Zelfs in het "rustigste" deel van de dag (14:00-16:00, 21,6-23,7 kts) blijft de golf torenhoog (2,25-2,9m/8-9s) en de richting licht-tot-pal aanlandig (228-255°) — dus ook dat venster is **Slecht en gevaarlijk**, niet alleen door windkracht maar vooral door de combinatie met de enorme golfslag en de aanlandige component. Vanaf 19:00 loopt de wind weer verder op (26-32 kts, gust 40-48 kts) bij richting 184-195° (side-shore, maar de windkracht zelf is dan simpelweg te gevaarlijk/overpowered). Bij gust >27 kts uit W/NW (vrijwel de hele dag het geval) is sluiting van de pieren door de Reddingsbrigade IJmuiden zeer aannemelijk.
- Bij **IJmuiden/Wijk aan Zee** (pierzone-hoek): 's ochtends/middags (280-305°) valt de richting in de **280°-360°-zone** → **IJmuiden** (Zuidpier) relatief rustiger. Vanaf de namiddag (242-267°) schuift dit richting de **neutrale zone (250°-280°)** — geen duidelijk voordeel meer. Golf (≥0,8m) ruimschoots aanwezig de hele dag.
- Golven: 2,0-2,9m/7-9s overdag, geleidelijk iets afbouwend naar 1,9-2,2m/7-7,8s in de avond (GFS).
- Getij: hoogwater 03:06 (2,1m), laagwater 11:31 (0,36m), hoogwater 15:24 (1,89m). Bij vloed (rond de hoogwaters) is de shorebreak extra zwaar bovenop de stormgolven.
- Bronnen: KNMI en GFS liggen deze run voor het eerst dicht bij elkaar (beide extreem) → eens, in tegenstelling tot eerdere runs waar KNMI veel milder leek — dit vergroot het vertrouwen in het gevaarlijke scenario. Soarcast niet bereikbaar.

### Zondag — Slecht en gevaarlijk (storm), mogelijk nog heftiger dan zaterdag (golfdata niet rechtstreeks beschikbaar deze run)
- Bij **Zandvoort/Wijk aan Zee**: richting is 's nachts/vroege ochtend zuid/ZZW (190-202°, side-shore-achtig) en draait vanaf circa 04:00 naar west/WZW (247-276°) en blijft daar de rest van de dag — dat is bij Zandvoort **licht tot pal aanlandig**. Windkracht is **extreem en bij beide bronnen consistent**: **windwaarnemingen.nl/KNMI geeft 27-35 kts gemiddeld met gust 39-50 kts** vanaf de vroege ochtend tot minstens 16:00 (laatste beschikbare uur in deze bron); **Windfinder/GFS geeft voor de hele dag 23-32 kts (gust 28-50 kts)**, met de piekgust (50 kts) rond 02:00. Dit is dus een voortzetting van de storm, zo mogelijk nog iets heftiger dan zaterdag qua gemiddelde windkracht. **Golfdata kon deze run niet rechtstreeks worden opgehaald** (de dagtab wordt clientside geladen, geen browser beschikbaar) — maar gezien de aanhoudende extreme wind en de net voorafgaande stormdag is een golf van ruim boven de 2m-drempel zeer waarschijnlijk, dus dit verandert de classificatie niet. Met wind die ver boven elk gedefinieerd "goed"-bereik ligt (>25 kts gemiddeld praktisch de hele dag) en een aanlandige component vanaf de ochtend, is **Slecht en gevaarlijk** de enige realistische conclusie, los van de exacte golfhoogte.
- Bij **IJmuiden/Wijk aan Zee** (pierzone-hoek): overdag (247-276°) valt de richting grotendeels in de **neutrale zone (250°-280°)** — geen van beide pieren biedt duidelijk voordeel; vroeg in de ochtend (190-202°, nog niet aanlandig) is pier-logica niet van toepassing. Piersluiting door de Reddingsbrigade (gust >27kt uit W/ZW/NW) zeer aannemelijk de hele dag.
- Golven: niet rechtstreeks opgehaald deze run — op basis van de voorafgaande storm en de aanhoudend extreme windkracht wordt >2m ingeschat, maar dit is een inschatting, geen meting.
- Getij: niet opgehaald deze run (secundair bij deze windkracht).
- Bronnen: KNMI en GFS liggen qua windkracht dicht bij elkaar (beide extreem) → eens. Golfdata: geen bron beschikbaar deze run (technische beperking, zie kanttekening boven). Soarcast niet bereikbaar.

---

## 🔭 Kans op mooie sessies daarna (dag 4-9)
Windfinder (GFS, enige bron zo ver vooruit; **alleen windrichting/-kracht kon deze run worden opgehaald, geen golfdata voor deze hele periode** — zie technische kanttekening boven) voor **maandag 26 t/m zaterdag 31 oktober**:

- **Maandag 26 oktober**: 's ochtends nog nawind van de storm — aanlandig (259-266°), wind 20-23 kts (gust 25-28 kts). Vanaf de namiddag/avond (13:00-19:00) draait de richting naar side-shore (187-203°, vrijwel de kustlijnhoek) en blijft de wind stevig: 17,4-21,4 kts (gust 24-33 kts). Golfdata onbekend, maar gezien de net afgelopen storm is nog aanzienlijke nadeining (ruim boven 1,1m) zeer waarschijnlijk → **mogelijk Optimaal vanaf ~13:00-19:00**, met als voorbehoud dat de golf niet bevestigd is.
- **Dinsdag 27 oktober — beste dag**: vrijwel de hele dag (ochtend tot namiddag) richting nagenoeg exact side-shore (192-209°, de kustlijnhoek zelf), wind **18,8-22,6 kts (gust tot 36,7 kts)**. Golfdata niet rechtstreeks beschikbaar, maar gezien de net voorafgaande storm van zaterdag/zondag is aanhoudende nadeining van ruim boven 1,1m zeer waarschijnlijk → vermoedelijk **Optimaal**. Beste venster: **10:00-16:00** (kern van de dag, stabielste side-shore-richting). Vanaf de avond (232-256°) schuift de richting richting licht aanlandig.
- **Woensdag 28 oktober**: richting 245-271° (licht tot pal aanlandig), wind 15,3-22,0 kts (gust 21,9-28,2 kts). Minder ideaal door de aanlandige component; classificatie hangt af van de golf (onbekend, mogelijk nog verhoogd van de storm) → **Goed(a) tot grensgeval Matig**, lager vertrouwen.
- **Donderdag 29 oktober**: wind valt sterk terug (3,0-11,4 kts, gust 4,8-18,1 kts), richting wisselvallig (140-251°) → overwegend **Matig tot Slecht** (te weinig wind).
- **Vrijdag 30 oktober**: zwakke wind (8,0-10,7 kts, gust 13,7-17,9 kts), richting wisselvallig zuid/noord (144-204°) → **Matig** (te weinig wind).
- **Zaterdag 31 oktober**: grotendeels zwak en wisselvallig (6,6-15,8 kts, gust 9,3-22,0 kts) → **Matig**, laag vertrouwen.

**Beste dag: dinsdag 27 oktober**, met het langste en meest consistente side-shore-venster van de hele periode (19-23 kts, kern van de dag 10:00-16:00) — dit is dezelfde dag die ook in eerdere runs al als beste dag naar voren kwam, wat het vertrouwen in dit patroon vergroot. **Maandagavond 26 oktober** (vanaf ~13:00) is een goed alternatief. Kans: **hoog** voor dinsdag, **gemiddeld** voor maandagavond — beide met het voorbehoud dat de golfhoogte voor deze dagen niet rechtstreeks kon worden gecontroleerd.
⚠️ Onzeker op 4+ dagen — check dichter bij de tijd opnieuw, en controleer dan expliciet alsnog de golfdata voor dinsdag (deze keer niet beschikbaar).

---
_Bronnen: Windfinder (GFS 3-uurs + Superforecast uurlijks) · windwaarnemingen.nl (KNMI, IJmuiden) · Soarcast — deze run niet bereikbaar (JS-app, geen vindbaar/bereikbaar API-adres)_
