# 🌊 Wingfoil-briefing Zandvoort–Wijk aan Zee
_25-11-2026 · Ochtendbriefing_

⚠️ **Technische kanttekening:** alle drie bronnen zijn deze run rechtstreeks via curl/API opgehaald (geen interactieve browser nodig). Windfinder: de Superforecast-pagina (`/weatherforecast/...`) bleek een Astro-site die de volledige uurlijkse ICON-EU-achtige data (incl. golf/getij) voor woensdag t/m vrijdag server-side meestuurt in een verborgen `astro-island`-attribuut (JSON, niet zichtbaar in de normale teksweergave) — rechtstreeks gedecodeerd i.p.v. via dagtabs te klikken. Voor de outlook dag 4-9 is dezelfde truc toegepast op de forecast-pagina (GFS, 3-uurs, t/m 4 december, eveneens mét golfdata). Soarcast: endpoint `sc/plotPerLocAndUnitReact.php?...&json=1` (dag 0/1/2, richting + wind/gust). windwaarnemingen.nl: de ruwe databron (`vsp_vdg_wstats.php` / `vsp_mrg_wstats.php`) bleek windsnelheid/gust in **m/s** te leveren (bevestigd via de site's eigen JS-conversiefunctie `kn_wsterkte_vspm`, die `3.6/1.852` toepast) — alles hieronder is dus omgerekend naar knopen; dit weerspreekt mogelijk een eerdere aanname in een vorige run.

**Netto beeld — een gusty maar prima wingfoilbare woensdag (vandaag) waarbij de wind nu al aantoonbaar harder waait dan voorspeld, een rustiger wordende donderdag met een flinke modeldivergentie, en een zwakke vrijdag. In de outlook springt donderdag 3 december eruit als de sterkste dag van het hele dag 4-9-blok.** Vandaag blijft de richting de hele dag zuiver pal-aflandig (OOST) en de golfslag laag/kort — dat houdt de classificatie op "Goed" in plaats van "Optimaal" ondanks een stevig gemiddelde van 14-17kts (Windfinder) tot 22kts (Soarcast). De Realitycheck van vanochtend laat zien dat de wind al duidelijk voor loopt op de voorspelling, wat voor de rest van de dag naar de hogere kant van deze bandbreedte wijst. Donderdag verzwakt geleidelijk door de dag heen, met Soarcast opnieuw 4-5kts hoger dan Windfinder/windwaarnemingen. Vrijdag is bij alle drie bronnen de zwakste dag, met een hinderlijke combinatie van laag gemiddelde maar af en toe een pittige gust.

---

## ⚡ Snel overzicht
- **Woensdag:** **Goed** (grensgeval) (08:00-22:00) — stevig en consistent, maar zuiver pal-aflandige richting en lage/korte golf sluiten Optimaal uit.
- **Donderdag:** **Matig-tot-Goed** (grensgeval) (00:00-06:00) — ochtend sterkst (14-14,5kts), neemt daarna af; forse modeldivergentie met Soarcast.
- **Vrijdag:** **Matig-tot-Slecht** (grensgeval) — zwakste dag van de 72 uur, geen bruikbaar venster.
- **Beste dag in de 7 dagen erna:** donderdag 3 december — duidelijk de sterkste en meest consistente dag van het hele dag 4-9-blok.

---

## ⏰ Realitycheck vandaag
- Laatste actuele uren (04:00-06:10, windwaarnemingen.nl/IJmuiden, 10-min metingen, omgerekend m/s→kts): **gem. 14,3-21,1 kts**, gust **19,3-26,7 kts**, richting **82-90° (OOST)**.
- Was voorspeld: windwaarnemingen's eigen uurlijkse vsp voor 04:00/05:00/06:00 zag **12,1 / 12,4 / 13,8 kts gem.** (gust 18,3 / 19,4 / 21,6 kts), richting **85 / 91 / 88° (OOST)** — vrijwel dezelfde richting, duidelijk lagere kracht.
- Conclusie: de wind loopt **VOOR** — het gemeten gemiddelde ligt dit ochtenduur 2-7kts hoger dan zowel windwaarnemingen's eigen vsp als Windfinder's hourly forecast voor dezelfde uren (die rond 12-14kts zaten). De richting klopt wel vrijwel exact (OOST, pal aflandig). Rest-van-de-dag inschatting: **licht naar boven bijgesteld** — de classificatie voor woensdag (Goed, grensgeval) blijft staan omdat richting en golfslag de beperkende factoren zijn, niet de windkracht, maar verwacht de werkelijke windkracht dichter bij Soarcast's hogere cijfers (tot 20-22kts) dan bij Windfinder's forecast (14-17kts).

---

## 📅 Komende 72 uur

### Woensdag — Goed (grensgeval)
- Windfinder (Superforecast, hourly ICON-EU): wind **12,4-17,3 kts gem.**, gust **23,9-32,1 kts** (hoge gust-factor, gusty dag), richting de hele dag **77,7-107,8° (OOST, pal aflandig)**. Golf laag en kort: **0,33-0,55m**, periode **2,7-3,6s**.
- Soarcast (Harmonie, IJmond): duidelijk hoger — **14,4-21,7 kts gem., gust 20,1-29,6 kts** — forse afwijking (2-4kts hoger gemiddeld dan Windfinder). Richting 80-99° (OOST), vergelijkbaar.
- windwaarnemingen.nl (eigen Harmonie-vsp, IJmuiden, omgerekend m/s→kts): **10,3-17,9 kts gem., gust 16,3-28,4 kts**, richting 80-99° — ligt tussen Windfinder en Soarcast in.
- Netto — alle drie bronnen zijn het eens dat het gemiddelde vrijwel de hele dag in de 14-25kts-Optimaal/Goed-band zit (en volgens de Realitycheck mogelijk nog hoger uitpakt dan hier vermeld), maar de richting is de hele dag **pal aflandig** (binnen ~30° van Zandvoort's pal-aflandige hoek 107,5°) — dit valt buiten zowel Optimaal (vraagt side-shore/licht aflandig) als Goed(a) (vraagt licht aanlandig). Golf blijft laag en kort, wat ook Goed(b) uitsluit. Netto dus **Goed, grensgeval**: windkracht en richting zijn prima wingfoilbaar (geen shorebreak-risico bij deze aflandige hoek), maar de formele classificatie wringt door de zuiver aflandige hoek en de lage, korte golfslag — hetzelfde patroon als de afgelopen dagen.
- Pier-logica: niet van toepassing (richting aflandig, niet aanlandig).
- Getij: hoogwater ±04:00 (2,22m), laagwater ±12:00 (0,41m), hoogwater ±16:00 (2,26m), met een zwak secundair signaal rond 20:00-21:00 (±1,0-1,0m).
- Beste venster: **±08:00-22:00** — wind 14,2-17,3 kts (Soarcast 14,4-21,7 kts), gust 26,3-32,1 kts, richting 77,7-95,6° (pal aflandig/OOST). Lange, consistente dag; houd rekening met stevige gusts (pieken tot 30+kts) en met de Realitycheck die op nóg sterkere wind wijst dan hier vermeld.

### Donderdag — Matig-tot-Goed (grensgeval)
- Windfinder (Superforecast, hourly ICON-EU): wind **9,5-14,5 kts gem.** (sterkst 's ochtends vroeg, neemt daarna geleidelijk af), gust **19,4-27,1 kts**, richting draait van **72,7° (licht aflandig)** 's nachts/vroege ochtend naar **104,7° (pal aflandig)** aan het einde van de dag. Golf laag en kort: **0,18-0,44m**, periode **2,65-3,46s**.
- Soarcast (Harmonie, IJmond): duidelijk hoger — **12,7-18,6 kts gem., gust 20,4-25,6 kts** — forse modeldivergentie van 4-5kts met Windfinder, vergelijkbare richting (77-104°).
- windwaarnemingen.nl (eigen Harmonie-vsp, IJmuiden, omgerekend m/s→kts): **8,7-14,8 kts gem., gust 16,3-23,3 kts**, richting 77-101° — ligt dicht bij Windfinder.
- Netto — 2 van de 3 bronnen (Windfinder, windwaarnemingen) houden het gemiddelde het grootste deel van de dag onder of rond de 14-15kts-grens, terwijl Soarcast stevig in de Optimaal/Goed-band zou vallen (tot 18,6kts) — een nadrukkelijke modeldivergentie. De vroege ochtend (licht aflandig, 72,7-78,8°) is qua richting het gunstigst, maar golf blijft bij alle bronnen te laag/kort voor Optimaal/Goed(b). Netto **Matig-tot-Goed, grensgeval** — met expliciete kans op het sterkere Soarcast-scenario.
- Pier-logica: niet van toepassing (richting aflandig, niet aanlandig).
- Getij: hoogwater ±04:00 (2,18m), laagwater ±12:00 (0,38m), hoogwater ±17:00 (2,31m).
- Beste venster: **±00:00-06:00** — wind 14,0-14,5 kts (Soarcast 16,3-17,8 kts), gust 22,4-27,0 kts, richting 72,7-84,2° (licht-tot-pal aflandig). Check dichter bij de tijd welk model gelijk krijgt.

### Vrijdag — Matig-tot-Slecht (grensgeval)
- Windfinder (Superforecast, hourly ICON-EU, t/m 19:00): wind blijft zwak, **7,0-10,6 kts gem.** (nooit in de buurt van 14kts), gust **12,2-20,9 kts** (af en toe een pittige gust ondanks zwak gemiddelde), richting **98,9-122,9° (pal aflandig, OOST-naar-ZO)**. Golf zeer laag: **0,12-0,17m**, periode **1,98-4,34s**.
- Soarcast (Harmonie, IJmond, t/m 15:00): iets hoger — **9,3-13,8 kts gem., gust 15,7-19,9 kts** — nog steeds zwak, richting 101-130° (OOST/ZO).
- windwaarnemingen.nl (eigen Harmonie-vsp, IJmuiden, omgerekend m/s→kts, t/m 15:00): **6,0-10,9 kts gem., gust 11,7-17,7 kts**, richting 95-128° — de zwakste van de drie bronnen.
- Netto — alle drie bronnen zijn het eens dat het gemiddelde de hele dag ruim onder de 14kts-grens blijft (zwakste dag van de 72 uur), maar net als bij eerdere grensgevallen loopt de gust op sommige momenten op tot 19-20,9kts — ruim boven de Matig-bovengrens (gust<19) maar het gemiddelde te zwak voor een nette Matig-classificatie. Netto **Matig-tot-Slecht, grensgeval**: te zwak gemiddeld voor een bruikbare sessie, met een onvoorspelbare gust zonder dragend gemiddelde.
- Pier-logica: niet van toepassing (richting aflandig, niet aanlandig).
- Getij: hoogwater ±05:00 (2,10m), laagwater ±13:00 (0,32m), hoogwater ±17:00 (2,30m).
- Beste venster: **geen bruikbaar venster.** Het minst zwakke moment is ±08:00-11:00 (wind 9,8-10,6kts, Soarcast 12-13,4kts, gust 18,2-19,9kts, richting 108-113° pal aflandig) — zonder een dragend gemiddelde geen serieuze sessie te verwachten.

---

## 🔭 Kans op mooie sessies daarna (dag 4-9)
Windfinder (GFS, enige bron zo ver vooruit) voor **zaterdag 28 november t/m donderdag 3 december** (incl. golfdata, in tegenstelling tot een vorige run waarin deze voor sommige dagen ontbrak).

- **Zaterdag 28 november** (dag 4): **10,4-14,9 kts gem.**, gust **17,4-26,9 kts**, richting **pal-tot-licht aflandig (125,9-152,3°)**. Golf **0,14-0,42m**, periode loopt 's ochtends op naar 5,5-7,08s maar golfhoogte blijft te laag. **Matig-tot-Goed**, sterkst 's avonds (19:00-22:00, 14,5-14,9kts).
- **Zondag 29 november** (dag 5): **10,2-15,7 kts gem.**, gust **17,7-27,3 kts**, richting draait naar **side-shore (155,5-209,1°, rond Zandvoort's kustlijnhoek 197,5°)** — qua richting de gunstigste dag van de outlook. Golf **0,48-0,64m**, periode **4,74-5,38s** (kruist de 5s-grens, maar hoogte blijft onder 1,1m). **Goed, grensgeval** — sterkste venster ±01:00-10:00 (14,6-15,7kts).
- **Maandag 30 november** (dag 6): **8,3-14,6 kts gem.**, gust **11,6-19,0 kts**, richting draait verder door naar **pal aanlandig (257-290°, WZW/W)** vanaf de middag. Golf **0,58-0,65m** (net onder de 0,8m pier-logica-drempel), periode **4,61-5,14s**. **Matig**, met een minder gunstige (aanlandige) hoek dan de dagen ervoor.
- **Dinsdag 1 december** (dag 7): **8,6-11,0 kts gem.**, gust **12,7-18,4 kts**, richting **side-shore (182,9-215°)**. Golf **0,63-0,71m**, periode consistent **5,11-5,6s**. **Matig**, zwak — gemiddelde komt de hele dag niet in de buurt van 14kts.
- **Woensdag 2 december** (dag 8): **9,1-16,9 kts gem.**, gust **15,3-24,9 kts** — bouwt op gedurende de dag, richting draait van side-shore (175,9°) 's ochtends naar pal aflandig (87-99°) 's avonds. Golf **0,65-0,69m**, periode opvallend lang **7,04-7,6s** rond het middaguur. **Matig-tot-Goed**, sterkst 's avonds (19:00-22:00, 14,3-16,9kts).
- **Donderdag 3 december** (dag 9): **16,3-18,1 kts gem.**, gust **24,1-27,3 kts** — veruit de sterkste en meest consistente dag van het hele blok. Richting **licht-tot-pal aflandig (63,6-87,4°)**. Golf **0,59-0,72m**, periode consistent **5,79-6,87s** (ruim boven 5s, maar hoogte nog net onder de 1,1m-Optimaal-grens). **Goed, grensgeval** — had Optimaal kunnen zijn als de golfhoogte net iets hoger was uitgevallen.

**Beste dag: donderdag 3 december** — duidelijk het sterkste en meest consistente windvenster van de hele dag 4-9-periode (16-18kts vrijwel de hele dag, lange golfperiode), maar de classificatie blijft "Goed, grensgeval" omdat de golfhoogte net onder de 1,1m-grens blijft. Kans: **gemiddeld-tot-hoog**. Zondag 29 november is een goed alternatief met de gunstigste (side-shore) richting van het hele blok. ⚠️ Onzeker op 4+ dagen — check dichter bij de tijd opnieuw.

---
_Bronnen: Windfinder (GFS / Superforecast ICON-EU) · Soarcast (KNMI Harmonie, IJmond) · windwaarnemingen.nl (KNMI, IJmuiden)_
