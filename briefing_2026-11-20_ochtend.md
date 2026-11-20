# 🌊 Wingfoil-briefing Zandvoort–Wijk aan Zee
_20-11-2026 · Ochtendbriefing_

⚠️ **Technische kanttekening:** alle drie bronnen zijn deze run rechtstreeks via curl (geen browser) opgehaald. Windfinder: de embedded Astro-JSON gedecodeerd — `ForecastSection`/`ForecastDataInit` op de forecast-pagina gaven dag 1 (3-uurs) en dag 4 t/m 9 (3-uurs, incl. golf via het WW3-golfmodel); dezelfde componenten op de Superforecast-pagina (`/weatherforecast/...`) gaven dag 1 t/m 3 op uurbasis. Soarcast: endpoint `sc/plotPerLocAndUnitReact.php?json&jsonOnly&location=133&day=...&windUnits=kts&forecastToShow=harm&duringDayOnly=true&runsToShow=lastOnly` voor wind/gust, met `&unit=deg` voor windrichting (let op: de `unit`-parameter zelf moet exact `m/s` zijn, niet `ms`, anders wijst de server een leeg antwoord terug). windwaarnemingen.nl via `database/vsp_vdg_wstats.php?st=IJmuiden1` (vandaag, 10-min-actuals + eigen uurlijkse Harmonie-vsp) en `vsp_mrg_wstats.php?st=IJmuiden2` (morgen+overmorgen); waarden lijken al in knopen (de standaard-eenheid op deze site).

**Netto beeld — een zwakke dag vandaag, een onzekere grensgeval-zaterdag met een pierzone-lichtpuntje bij IJmuiden, een rustige Matig-zondag, en in de verre outlook drie interessante dagen (dinsdag 24, zaterdag 28 en zondag 29 november) waarvan dinsdag de langste en sterkste is.** Vandaag (vrijdag) blijft de wind bij Windfinder en windwaarnemingen de hele dag te zwak (nooit gelijktijdig gust≥16kts én gem≥14kts); de ochtend-realitycheck bevestigt dit — de actuele wind ligt dicht bij windwaarnemingen's eigen (lage) voorspelling, en ruim onder Windfinder's gust-cijfers voor dezelfde uren. Zaterdag is opnieuw een modelverdeeldheid-dag: Windfinder en Soarcast zien elkaar vinden op 10-14kts/12-17kts gust pal aanlandig, maar windwaarnemingen's eigen lijn blijft daar fors onder (2,7-5,7kts) — gezien het weerkerende patroon van de laatste dagen (waarbij de lagere lijn het telkens wint) is enige voorzichtigheid met de hogere cijfers op zijn plaats. Zondag is een rustige Matig-dag met goede overeenstemming tussen Windfinder en Soarcast. In de outlook springt dinsdag 24 november er het sterkst uit (lang venster, 14-16kts aflandig, gust tot 28kts) al blijft de golf daar ruim onder de drempel; zaterdag 28 en zondag 29 november zijn qua golf juist net wél (bijna) over de 1,1m-drempel.

---

## ⚡ Snel overzicht
- **Vrijdag:** **Slecht** — wind blijft de hele dag te zwak (Windfinder en windwaarnemingen eens, nergens gelijktijdig gust≥16/gem≥14; realitycheck bevestigt de zwakke lijn).
- **Zaterdag:** **Matig**, met een kort **Goed(a)-grensgeval bij IJmuiden rond ±10:00** (dankzij pierzone-hoek en Zuidpier-bescherming; bij Zandvoort/Wijk aan Zee blijft het pal aanlandig en dus Matig) — grote modelverdeeldheid (Windfinder/Soarcast 10-14kts, windwaarnemingen 2,7-5,7kts).
- **Zondag:** **Matig** (±14:00-19:00, 8-11kts, gust tot 17kts, licht aflandig) — Windfinder en Soarcast eens, windwaarnemingen weer fors zwakker.
- **Beste dag in de 7 dagen erna:** dinsdag 24 november — langste en sterkste venster (±07:00-19:00, 14-16kts, gust tot 28kts), maar golf blijft ruim onder de 1,1m-drempel.

---

## ⏰ Realitycheck vandaag
- Laatste actuele uren (04:00-06:10, windwaarnemingen.nl/IJmuiden, 10-min metingen): **gem. ≈5,3-7,0 kts**, gust **≈6,4-9,0 kts**, richting draaiend van **≈99° (OOST) naar ≈65,5° (ONO)**.
- Was voorspeld: windwaarnemingen's eigen Harmonie-vsp zag voor dezelfde uren **4,2-4,7 kts gem., gust 7,1-7,5 kts, richting 83-94°** (OOST) — de actuals liggen iets hoger qua gemiddelde, gust vergelijkbaar. Windfinder (GFS) zag voor diezelfde uren een vergelijkbaar gemiddelde (**6,6-7,2 kts**) maar een veel hogere gust: **12,9-15,8 kts** — bijna het dubbele van de werkelijke gust. Soarcast levert voor deze vroege uren geen data (pas vanaf ±07:00).
- Conclusie: het gemiddelde **KLOPT ongeveer (iets sterker dan windwaarnemingen's eigen voorspelling)**, maar de **gust loopt FORS ACHTER** op Windfinder's hogere voorspelling. Rest-van-de-dag inschatting: **bijgesteld naar de lagere/bevestigde lijn** — voor de rest van vandaag wordt uitgegaan van windwaarnemingen's bescheiden gust-niveau in plaats van Windfinder's veel hogere cijfers (die toch al zwak genoeg waren om op Slecht te blijven uitkomen).

---

## 📅 Komende 72 uur

### Vrijdag — Slecht
- Windfinder (GFS, uurlijks): wind neemt overdag af van ≈12kts gem./17kts gust (richting 79-89°, aflandig) rond middernacht naar een dal van **3,1-5,9 kts gem.** (gust 5,8-11,7kts) tussen 07:00-15:00, en bouwt in de avond weer op naar 10-12kts/13-16kts gust (richting draait via side-shore ±350-358° naar licht aanlandig 326° om 23:00). Golf blijft de hele dag onder de drempel: **0,37-0,70m**, periode 4,9-6,4s.
- Soarcast (Harmonie, IJmond, 07:00-16:00): ziet een opvallend sterkere ochtend dan Windfinder — **11,8-12,4 kts gem./16,4-17,1 kts gust** rond 07:00-10:00 (richting 91-103°, aflandig), zakt daarna terug naar 7,2-9,8kts. Dit is niet bevestigd door windwaarnemingen of de realitycheck-actuals.
- windwaarnemingen.nl (eigen Harmonie-vsp, IJmuiden): de hele dag zwak, **3,1-6,2 kts gem.**, gust 5,1-9,7kts, richting vergelijkbaar aflandig/noord draaiend (65-102°, later 310-360°). **De realitycheck-actuals bevestigen deze lagere lijn.**
- Netto — Windfinder en windwaarnemingen zijn het eens: de hele dag blijft gust<16kts én gem<14kts, dus **Slecht**. Soarcast's ochtendpiek (tot 17,1kts gust) is de enige uitzondering maar wordt door de realitycheck niet bevestigd — wie toch gaat kijken rond 08:00-10:00 kan die bevestigen, maar reken er niet op.
- Pier-logica: niet van toepassing (golf blijft onder 0,8m zodra de richting aanlandig-achtig wordt, pas laat in de avond).
- Getij: laagwater ±08:00 (0,51m), hoogwater ±12:00 (1,61m), laagwater ±20:00 (0,33m).
- Beste venster: **geen bruikbaar venster.** Hoogstens een onbevestigde kans rond 08:00-10:00 (Soarcast: ≈12kts gem./17kts gust, aflandig) — niet op rekenen.

### Zaterdag — Matig, kort Goed(a)-grensgeval bij IJmuiden
- Windfinder (GFS, uurlijks): wind bouwt 's ochtends op en blijft de hele dag **7,3-14,0 kts gem.** (piek 14,0kts/14,1kts gust om 10:00), gust 9,0-16,9kts, richting opvallend constant **pal aanlandig, 275-312°** (bij Zandvoort/Wijk aan Zee). Golf net onder de drempel en vrij hoog voor de tijd van het jaar: **0,75-0,94m**, periode 6,2-6,9s (ruim boven 5s).
- Soarcast (Harmonie, IJmond, 07:00-16:00): sluit goed aan bij Windfinder — **4,5-12,4 kts gem., gust 11,8-16,2kts**, richting vergelijkbaar 280-318° (WNW/NW). Voor deze dag dus goede overeenstemming tussen de twee modellen.
- windwaarnemingen.nl (eigen Harmonie-vsp, IJmuiden): ziet een veel zwakkere dag — **2,7-5,7 kts gem.**, gust 5,4-8,0kts, richting vergelijkbaar (275-322°). Dit is de derde dag op rij met een forse modelverdeeldheid waarbij windwaarnemingen's eigen lijn structureel lager uitkomt — gezien het trackrecord van deze week (de realitycheck bevestigde gisteren en vandaag telkens de lagere lijn) verdient de hogere Windfinder/Soarcast-lijn hier enige scepsis.
- Netto bij **Zandvoort/Wijk aan Zee** (pal aanlandig de hele dag, eigen hoek): wind 14-25kts-vereiste wordt maar kort (10:00) gehaald, golf blijft onder 1,1m en de richting is pal (niet licht) aanlandig → voldoet nergens exact aan Goed(a) of Optimaal → **Matig** de hele dag (grensgeval richting Goed rond 10:00-16:00 als Windfinder/Soarcast gelijk krijgen).
- Netto bij **IJmuiden** (pierzone-hoek, pal aanlandig 240°): dezelfde 275-312°-richting valt hier in de **licht aanlandige band (rond 10:00-13:00) tot side-shore (vanaf ±15:00)** — gunstiger dan bij Zandvoort. Om **±10:00** (14,0kts gem., golf 0,93m<1,1m, richting licht aanlandig) is dit een schoon **Goed(a)-grensgeval**; de rest van de dag blijft het door de iets lagere wind Matig, ook bij IJmuiden.
- Pier-logica: richting (275-312°) + golf (0,80-0,94m, dus ≥0,8m-drempel) → van toepassing. 08:00-14:00 valt de richting grotendeels in de **neutrale zone (250-280°)** tussen de twee pierassen (geen duidelijk voordeel); vanaf ±15:00 draait de richting net genoeg naar NW om **IJmuiden (Zuidpier)** de voorkeur te geven. Bij **Wijk aan Zee** blijft de aanlandige golfslag de hele dag onbeschut (geen piervoordeel in dit windregime).
- Getij: hoogwater ±01:00 (1,99m), laagwater ±09:00 (0,43m), hoogwater ±13:00 (1,76m), laagwater ±21:00 (0,28m).
- Beste venster: **±10:00-16:00 bij IJmuiden** — wind 11-14 kts, gust 12-17 kts, richting 275-285° (licht aanlandig bij IJmuiden dankzij pierzone-hoek). Golf ≈0,88-0,93m — net onder de drempel. Bij Zandvoort/Wijk aan Zee dezelfde uren, maar dan Matig (pal aanlandig, geen piervoordeel). Check dichter bij de tijd of Windfinder/Soarcast of windwaarnemingen gelijk krijgt.

### Zondag — Matig
- Windfinder (GFS, uurlijks, tot 19:00 beschikbaar): wind bouwt op van ≈4-6kts 's nachts naar **8,2-10,7 kts gem.** in de namiddag (piek 16:00), gust oplopend tot **15,2-17,3 kts** tussen 14:00-19:00, richting draait van aflandig (37-90°) 's ochtends naar licht aflandig (57-69°) in de namiddag. Golf blijft laag: **0,61-0,73m**, periode 6,9-7,7s (ruim boven 5s).
- Soarcast (Harmonie, IJmond, 07:00-14:00): sluit goed aan — **3,5-11,0 kts gem., gust 6,1-15,2kts**, richting vergelijkbaar (54-125°, aflandig/ONO). Goede overeenstemming met Windfinder.
- windwaarnemingen.nl (eigen Harmonie-vsp, IJmuiden, tot 15:00): opnieuw de zwakste van de drie — **1,3-4,7 kts gem.**, gust 2,4-7,5kts, richting vergelijkbaar (52-153°). Vierde dag op rij met dezelfde forse modelverdeeldheid.
- Netto — wind bereikt bij Windfinder/Soarcast's namiddagpiek (14:00-19:00) net niet de 14kts-drempel (max 10,7kts gem.), golf blijft met 0,61-0,63m ruim onder de 1,1m-drempel en periode <5s wordt niet gehaald als probleem (periode is juist prima, >7s) — dus geen Optimaal/Goed(b), wel een bruikbare **Matig**-middag met aardige gust. Richting is (licht) aflandig, dus schoon water.
- Pier-logica: niet van toepassing (richting aflandig, geen aanlandige golfslag).
- Getij: hoogwater ±01:00 (2,10m), laagwater ±10:00 (0,38m), hoogwater ±14:00 (1,92m).
- Beste venster: **±14:00-19:00** — wind 8-11 kts, gust 15-17 kts, richting 57-69° (licht aflandig). Golf ≈0,62m/7,5s — golf ruim onder de drempel maar schoon aflandig water. windwaarnemingen's veel zwakkere lijn is nog niet bevestigd; check dichter bij de tijd.

---

## 🔭 Kans op mooie sessies daarna (dag 4-9)
Windfinder (GFS, enige bron zo ver vooruit) voor **maandag 23 t/m zondag 29 november**.

- **Maandag 23 november**: wind zwak de hele dag (**3,7-7,1 kts gem.**, gust 3,7-8,7kts), richting sterk wisselend (48-258°). Golf laag (**0,48-0,56m**), periode 7,0-7,4s. Slecht — geen uitschieter.
- **Dinsdag 24 november** (dag 4): de sterkste en langste dag van de hele outlook-periode — **13,5-16,0 kts gem.** vrijwel de hele dag (±07:00-19:00), gust tot **24,6-28,1kts**, richting zeer constant pal- tot licht aflandig (123-149°, dus bij Zandvoort geen piervermelding nodig — schoon aflandig water). Golf blijft echter laag (**0,54-0,58m**, ruim onder de 1,1m-drempel), periode 5,5-6,7s. **Goed, grensgeval richting Optimaal** — wind en richting zijn vrijwel ideaal, alleen de golfhoogte blijft (met bijna de helft van de vereiste 1,1m) duidelijk tekort. Dit is een forse opwaardering t.o.v. de vorige run (die zag 10-13kts/21-24kts gust voor deze dag).
- **Woensdag 25 november** (dag 5): nog steeds gusty maar iets zwakker gemiddeld — **9,4-11,9 kts gem.**, gust tot **13,6-19,9kts**, richting oost/oostzuidoost (102-135°, aflandig). Golf **0,47-0,57m**, periode merendeels net onder 5s (4,5-5,4s). Matig — golf en periode blijven tekort voor meer.
- **Donderdag 26 november** (dag 6): wind zwakt verder af (**8,2-10,0 kts gem.**, gust 9,7-14,9kts), richting oost/noordoost (81-97°, aflandig). Golf laag (**0,53-0,66m**). Slecht.
- **Vrijdag 27 november** (dag 7): bouwt 's avonds op tot een gusty piek — **13,4-13,7 kts gem./21,6-22,4kts gust** tussen 19:00-22:00 (richting 144-148°, licht aflandig). Golf nadert de drempel maar blijft net onder: **0,86-0,90m**, periode 5,4-5,8s. **Matig-tot-Goed grensgeval** in de avond — wind net onder 14kts maar met ongewoon hoge gust-factor.
- **Zaterdag 28 november** (dag 8): windshift-dag — 's ochtends zwak en side-shore/aflandig (156-171°), maar tussen **13:00-16:00** bouwt het op tot **13,5-14,4 kts gem./16,7-18,3kts gust** met richting gedraaid naar **321-333°** (licht aanlandig bij Zandvoort). Golf **1,01-1,06m** — op een haar na (0,04-0,09m) over de 1,1m-drempel, periode 5,8-6,1s (ruim boven 5s). **Goed(a), grensgeval richting Optimaal** — de scherpste "net niet"-golfhoogte van de hele periode.
- **Zondag 29 november** (dag 9): vanaf de middag een schoon venster — tussen **13:00-19:00** wind **11,5-13,7 kts gem., gust 14,9-20,9kts**, richting **196-212°** (side-shore). Golf **1,08-1,21m** — hier wél over de 1,1m-drempel, periode 6,7-7,0s. Dit is een schone **Goed(b)-match** (wind<15kts, golf>1,1m én periode≥5s, richting niet pal aanlandig) — formeel de "netste" dag van de hele outlook-periode, zij het met iets minder wind dan dinsdag 24 november.

**Beste dag: dinsdag 24 november** — het langste en sterkste venster van de periode (12 uur lang 14-16kts gem., gust tot 28kts, schoon aflandig), al blijft de golf daar het verst onder de drempel. Zondag 29 november is qua formele criteria de "schoonste" match (golf wél over de drempel) maar met een korter venster en iets minder wind; zaterdag 28 november heeft de scherpste net-niet-golfhoogte van de week. Kans: **gemiddeld** — drie dagen met een kansrijk venster is ruim boven het structureel zwakke beeld van de afgelopen weken, maar alle drie zijn minstens op één criterium een grensgeval. ⚠️ Onzeker op 4+ dagen — check dichter bij de tijd opnieuw, zeker omdat dinsdag 24 nov deze run al fors is opgewaardeerd t.o.v. gisteravond.

---
_Bronnen: Windfinder (GFS) · Soarcast (KNMI Harmonie, IJmond) · windwaarnemingen.nl (KNMI, IJmuiden)_
