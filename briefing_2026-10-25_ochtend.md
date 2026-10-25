# 🌊 Wingfoil-briefing Zandvoort–Wijk aan Zee
_25-10-2026 · Ochtendbriefing_

⚠️ **Technische kanttekening:** Soarcast (JS/Vite-app, geen bereikbaar publiek API-adres zonder sessie-navigatie die als bot-omzeiling zou gelden) was deze run niet te benaderen — net als alle voorgaande sessies. Windfinder is opgehaald via de onderliggende Astro-JSON (reguliere forecast-pagina + Superforecast-pagina, incl. golf/getij voor de volle 72 uur en de outlook dag 4-9). windwaarnemingen.nl (IJmuiden) is opgehaald via de vsp-database-endpoints (vandaag + morgen, incl. 10-minuten-actuals). Beide resterende bronnen waren dus volledig bereikbaar.

🚨 **Belangrijkste signaal deze run: groot modelverschil tussen Windfinder/GFS en windwaarnemingen.nl/KNMI, over de volle 72 uur.** De Realitycheck (zie hieronder) laat zien dat de actuele metingen vanochtend duidelijk dichter bij **KNMI** liggen dan bij **GFS**: GFS voorspelt voor vandaag 27-32 kts gemiddeld met gust tot 40-50 kts, terwijl zowel KNMI (15-18 kts/21-23 kts) als de harde metingen (16-18,5 kts/20,6-25,9 kts) daar ver onder blijven. Dit verschil is niet beperkt tot vandaag: ook voor maandag en dinsdag voorspelt GFS structureel 1,5-2x zoveel wind dan KNMI. Omdat KNMI vanochtend valideert tegen de praktijk, leunt deze briefing op **KNMI als leidende windbron** voor de komende 72 uur, met GFS-cijfers er expliciet naast (niet gemiddeld) ter transparantie, en met navenant lager vertrouwen op de dagen waar GFS de enige bron is (vanaf dinsdagmiddag, en de hele outlook dag 4-9).

---

## ⚡ Snel overzicht
- **Zondag:** **Slecht** (pal aanlandig + grote branding, hele dag) — hoog vertrouwen op richting/golf, wind zelf valt mee (zie Realitycheck).
- **Maandag:** **Matig/Slecht (te weinig wind)** volgens KNMI — grensgeval **Goed** laat op de avond (rond 23:00). GFS voorspelt hier juist **Optimaal** voor vrijwel de hele dag — groot modelverschil, lage zekerheid.
- **Dinsdag:** **Matig**, kort venster **11:00-14:00** (Goed, grensgeval) volgens KNMI. GFS voorspelt ook hier **Optimaal** voor het grootste deel van de dag — zelfde modelverschil, lage zekerheid, en na 15:00 is er geen KNMI-check meer beschikbaar.
- **Beste dag in de 7 dagen erna:** zaterdag 31 oktober

---

## ⏰ Realitycheck vandaag
- Laatste actuele uren (windwaarnemingen.nl, IJmuiden, 04:00-06:10): **wind gem. ~18,2 kts, gust gem. ~22,5 kts, richting ~254-267° (West/WZW)**. Piekgust tot nu toe: 25,9 kts (rond 05:40) — geen enkel moment boven de 27 kts-pierensluitingsdrempel.
- Was voorspeld voor dezelfde uren: **windwaarnemingen.nl/KNMI** gaf gem. **~15,1 kts, gust ~21,0 kts, richting ~258°** — vrij dicht bij de praktijk. **Windfinder/GFS** gaf voor dit venster **~29,0 kts gem., gust ~37,7 kts** — dat is ruim het dubbele van wat werkelijk gemeten wordt, bij vergelijkbare richting (~264°).
- Conclusie: de wind loopt **licht VOOR op KNMI** (+~3 kts gemiddeld, +~1,5 kts gust — binnen normale bandbreedte), maar **Windfinder/GFS overschat de wind drastisch** (~+90% op het gemiddelde, ~+65% op de gust) voor dit hele systeem. Rest-van-de-dag inschatting: **vertrouwen in KNMI voor de rest van vandaag bevestigd en als leidende bron aangehouden**; GFS-cijfers voor de komende 72 uur worden met expliciete terughoudendheid gepresenteerd (zie 72u-sectie) i.p.v. als absoluut niveau gelezen. Golfdata (alleen van GFS beschikbaar) kan in dezelfde mate overschat zijn, maar daarvoor is geen onafhankelijke validatie mogelijk — golfhoogte dus met iets lager vertrouwen lezen dan gebruikelijk.

---

## 📅 Komende 72 uur

### Zondag — Slecht (pal aanlandig + grote branding, hele dag)
- Bij **Zandvoort/Wijk aan Zee**: na een kort Optimaal-venster diep in de nacht (00:00-02:00, side-shore 195-220°, inmiddels gepasseerd) draait de wind vanaf 03:00 naar pal aanlandig/grensgeval licht aanlandig (253-274°, binnen of net buiten 30° van Zandvoorts 287,5°) en blijft daar de rest van de dag. Wind volgens **KNMI (leidend na de Realitycheck) 13-18 kts gemiddeld, gust 18-26 kts** — dus geenszins extreem — maar de golf (Windfinder/GFS, enige golfbron) is enorm: **2,3-3,25m / 8,2-9,6s**, gestaag oplopend tot de vroege avond. Die combinatie van (licht) aanlandige hoek met zware deining is **Slecht (grote branding, geen pierbescherming)**, ook al is de windkracht zelf dus mild — het gevaar zit in de golf, niet in de wind. Windfinder/GFS voorspelt voor dezelfde uren 27-32 kts/35-50 kts, wat volgens de Realitycheck niet overeenkomt met de praktijk; zelfs met de mildere KNMI-cijfers blijft het oordeel Slecht door de golfhoogte.
- Bij **IJmuiden/Wijk aan Zee** (pierzone-hoek 240°/60°): de richting (253-274° het grootste deel van de dag) valt in de **250°-280°-neutrale zone** tussen de twee pierassen → geen van beide pieren biedt hier een duidelijk voordeel, ondanks de aanlandige hoek en golf ≥0,8m die de pier-logica normaal relevant zouden maken.
- Golven: 2,3m 's nachts oplopend naar 3,25m rond 19:00, daarna licht afbouwend naar 3,1m tegen middernacht — lange periode (8-9,6s) de hele dag.
- Getij: hoogwater 02:40 (2,2m), laagwater 11:20 (0,39m), hoogwater 15:00 (2,03m), laagwater 18:56 (0,96m) — opnieuw een ongewoon hoog "laagwater" door opgestuwd water (stormvloed-effect, zoals ook de afgelopen dagen), plus een kleine secundaire piek om 19:45 (0,98m); laagwater 23:08 (0,27m).
- Bronnen: windwaarnemingen.nl/KNMI en de harde actuals liggen dicht bij elkaar → eens, hoog vertrouwen op windkracht. Windfinder/GFS wijkt fors af op windkracht (zie Realitycheck) → expliciet vermeld, niet gemiddeld. Beide bronnen zijn het wel eens over de (licht) aanlandige richting. Soarcast niet bereikbaar.

### Maandag — Matig/Slecht (te weinig wind) volgens KNMI; GFS voorspelt Optimaal — groot modelverschil
- Bij **Zandvoort/Wijk aan Zee**: 's nachts/vroege ochtend (00:00-06:00) nog pal aanlandig (265-271°) met afbouwende golf (3,0m→2,4m) en volgens **KNMI** een mild **11-15 kts gemiddeld, gust 17-21 kts** → nog **Slecht (branding)** door de golfhoogte, niet door windkracht. Vanaf 07:00 draait de richting geleidelijk via licht aanlandig naar **side-shore vanaf circa 11:00** (236° tot 172° rond het middaguur, daarna 178-204° de rest van de dag) — precies de hoek die bij voldoende wind Optimaal zou zijn, en de golf blijft met 1,5-2,2m ruim boven de drempel. Alleen: **KNMI voorspelt voor deze uren maar 7-11 kts gemiddeld (gust 11-16 kts)** — te weinig wind, dus **Slecht/Matig (te weinig wind)** ondanks de goede hoek en golf. Pas rond **23:00** (side-shore 204°, 11,0/16,2 kts, golf 1,62m/7,1s) komt KNMI net binnen de Goed(b)-criteria — een kort, laat en licht grensgeval. **Windfinder/GFS tekent een heel ander beeld**: 15-28 kts gemiddeld de hele dag, met rond het middaguur-side-shore-venster (12:00-21:00) nota bene 13-18 kts bij dezelfde goede hoek — dat zou **Optimaal** betekenen. Gezien de Realitycheck (GFS overschat vandaag drastisch) is dit GFS-optimisme met behoorlijke argwaan te bezien, maar zonder nieuwe KNMI-validatie morgenochtend is niet met zekerheid te zeggen welk scenario klopt.
- Bij **IJmuiden/Wijk aan Zee** (pierzone-hoek): alleen tijdens de vroege-ochtend pal-aanlandige uren (00:00-06:00, golf ≥0,8m) is pier-logica relevant — richting 265-271° valt in de **250°-280°-neutrale zone** → geen duidelijk piervoordeel. Vanaf het middaguur is de richting (172-236°) side-shore voor Zandvoort, dus niet meer aanlandig genoeg om de pier-logica te laten gelden.
- Golven: 3,0m 's nachts, geleidelijk afbouwend naar 1,47-1,62m in de loop van de avond.
- Getij: hoogwater 03:16 (2,27m), laagwater 12:02 (0,45m), hoogwater 15:36 (2,15m), laagwater 19:29 (0,92m, opnieuw verhoogd), kleine piek 20:35 (0,99m), laagwater 23:48 (0,3m).
- Bronnen: **groot verschil tussen KNMI en Windfinder/GFS op windkracht** (factor ~1,5-2x), expliciet vermeld i.p.v. gemiddeld — zie boven. Beide zijn het wel eens over de richtingsdraai naar side-shore vanaf het middaguur. Soarcast niet bereikbaar.

### Dinsdag — Matig, kort venster 11:00-14:00 (Goed, grensgeval) volgens KNMI; GFS voorspelt Optimaal — zelfde modelverschil
- Bij **Zandvoort/Wijk aan Zee**: de hele beschikbare KNMI-periode (00:00-15:00, verder vooruit heeft windwaarnemingen.nl geen data meer) staat de richting side-shore (178-204°, rond de kustlijnhoek). 's Ochtends (00:00-10:00) is de wind met **8-9,7 kts (KNMI)** te zwak → **Slecht (te weinig wind)**. Van **11:00-14:00** trekt de wind net aan tot **10,6-11,6 kts gemiddeld, gust 16-16,6 kts**, bij golf **1,41-1,42m/7,1-7,2s** (Windfinder/GFS) — dat raakt net de Goed(b)-criteria (wind <15 kts met gust <19, golf >1,1m en periode ≥5s, niet pal aanlandig): een mild maar bruikbaar grensgeval-venster. Na 15:00 zakt KNMI's wind terug naar 10,6 kts → weer te weinig. **Windfinder/GFS geeft voor de hele dag 16-19 kts bij dezelfde side-shore-hoek** — dat zou een volledige **Optimaal**-dag betekenen, en voor de uren na 15:00 (19:00: 13,8 kts aflandig-achtig) is dit zelfs de enige beschikbare bron. Gezien het patroon van de voorgaande dagen (GFS structureel te hoog) is ook hier extra terughoudendheid gepast.
- Pier-logica: niet van toepassing — de richting is de hele dag side-shore (178-204°), niet (licht) aanlandig voor Zandvoort, dus buiten scope van de pier-logica.
- Golven: 1,40-1,59m/7,0-7,2s, vrijwel constant de hele beschikbare periode.
- Getij: hoogwater 03:55 (2,3m), laagwater 12:08 (0,49m), hoogwater 16:15 (2,24m), laagwater 20:12 (0,91m, verhoogd), kleine piek 21:18 (0,99m).
- Bronnen: **opnieuw een aanzienlijk verschil tussen KNMI en Windfinder/GFS op windkracht**, expliciet vermeld. Na 15:00 is er geen KNMI-cross-check meer beschikbaar voor vandaag/morgen — vertrouwen voor de avonduren daarom lager dan gebruikelijk. Soarcast niet bereikbaar.

---

## 🔭 Kans op mooie sessies daarna (dag 4-9)
Windfinder (GFS, enige bron zo ver vooruit — let op: dit model heeft de afgelopen 72 uur structureel te hoge windsnelheden gegeven, dus lees onderstaande cijfers met extra terughoudendheid) voor **woensdag 28 oktober t/m maandag 2 november**:

- **Woensdag 28 oktober**: pal aanlandig (261-292°) de hele ochtend/middag met golf nog 1,1-1,5m, wind afbouwend van 13 naar 9 kts → **Slecht (branding) tot Matig (te weinig wind)**, geen bruikbaar venster.
- **Donderdag 29 oktober**: wind valt verder terug (5,9-9,1 kts), richting draait via side-shore naar pal aflandig (107-157°), golf kalmeert snel (0,8m→0,3m) → **Slecht/Matig**, te weinig wind de hele dag.
- **Vrijdag 30 oktober**: nog altijd zwak (8,7-12,8 kts) en pal aflandig (107-141°), golf heel klein (0,26-0,36m) → **Matig tot Slecht**, weinig kansrijk.
- **Zaterdag 31 oktober — beste dag**: wind bouwt gestaag op van 10,7 naar 21,1 kts, richting draait via side-shore (159-236°) — precies de gunstige hoek voor Zandvoort/Wijk aan Zee. Golf blijft aan de kleine kant (0,38-0,57m, onder de Optimaal-drempel van 1,1m), dus het wordt eerder **Goed/grensgeval** dan een volwaardig Optimaal — maar met oplopende, bruikbare wind in een goede hoek is dit duidelijk de kansrijkste dag van de week. Beste venster: **namiddag (13:00-19:00)**, als de wind het hardst waait.
- **Zondag 1 november**: draait 's ochtends kort naar licht aanlandig met bruikbare cijfers (07:00: 15,7/18,4 kts, golf 0,75m) — een smal **Goed(a)**-venster — maar valt daarna snel terug naar te weinig wind (8,8-13,5 kts) de rest van de dag.
- **Maandag 2 november**: nagenoeg windstil (1,5-7,3 kts) → **Slecht**, de hele dag.

**Beste dag: zaterdag 31 oktober**, met de langste aaneengesloten combinatie van oplopende wind en goede side-shore-hoek van de hele periode. Kans: **gemiddeld** (wind en hoek zijn kansrijk, maar de golf is aan de kleine kant en dit is uitsluitend op GFS gebaseerd, de bron die de laatste dagen structureel te hoog uitkwam — dus ook de kans dat de wind zaterdag juist lager uitvalt dan hier genoemd is reëel). **Laag** voor de rest van de week (te weinig wind of ongunstige hoek).
⚠️ Onzeker op 4+ dagen — check dichter bij de tijd opnieuw, en let specifiek op een mogelijke correctie naar boven of onder zodra KNMI deze dagen binnen bereik komt.

---
_Bronnen: Windfinder (GFS, 3-uurs/uurlijks) · windwaarnemingen.nl (KNMI, IJmuiden, incl. 10-min actuals) · Soarcast — deze run niet bereikbaar (JS-app, geen vindbaar/bereikbaar publiek API-adres)_
