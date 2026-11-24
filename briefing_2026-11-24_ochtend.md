# 🌊 Wingfoil-briefing Zandvoort–Wijk aan Zee
_24-11-2026 · Ochtendbriefing_

⚠️ **Technische kanttekening:** alle drie bronnen zijn deze run rechtstreeks via curl (geen browser) opgehaald. Windfinder: embedded Astro-JSON gedecodeerd — hourly ICON-EU-achtige data (incl. golf/getij) voor vandaag t/m donderdag via de Superforecast-pagina, en de 3-uurs GFS-reeks (wind/gust/richting, alle 10 dagen) via de forecast-pagina voor de outlook dag 4-9. **Let op:** voor de outlookdagen vrijdag 27, zondag 29 en dinsdag 1 december ontbrak golfdata in de statische extractie (de preview-tabs van Windfinder leveren golfdata maar voor om-en-om liggende dagen: zaterdag 28, maandag 30 en woensdag 3 dec wél) — die 3 dagen zijn dus alleen op wind/gust/richting beoordeeld. Soarcast: endpoint `sc/plotPerLocAndUnitReact.php` (unit=deg voor richting, unit=m/s&windUnits=kts voor wind/gust), dag 0/1/2. windwaarnemingen.nl via `database/vsp_vdg_wstats.php?st=IJmuiden1` (vandaag, 10-min-actuals + eigen uurlijkse vsp) en `database/vsp_mrg_wstats.php?st=IJmuiden2` (morgen+overmorgen).

**Netto beeld — een zwakke, grillige dinsdag (vandaag) met een pittige late gust, een stevige en consistente woensdag die de beste dag van de 72-uursperiode is, en een donderdag met een ideale hoek maar een twijfelachtige windkracht waar de bronnen flink over verdeeld zijn.** Vandaag blijft het gemiddelde de hele dag onder de 14kts terwijl de gust 's avonds oploopt tot 22-26kts — een vervelende combinatie die niet netjes in één hokje past. Woensdag is bij alle drie bronnen duidelijk de sterkste dag (14-22kts gem., gust tot 30+kts), maar de zuiver aflandige hoek en de korte, platte golfslag houden het bij "Goed, grensgeval". Donderdag heeft juist de ideale hoek (licht aflandig volgens Windfinder) maar Windfinder/windwaarnemingen zien de wind onder de 14kts blijven, terwijl Soarcast 4-5kts hoger zit — een expliciete modeldivergentie. In de outlook springt zondag 29 november eruit als de sterkste en langst-consistente dag van het blok dag 4-9.

---

## ⚡ Snel overzicht
- **Dinsdag:** **Slecht-tot-Matig** (grensgeval, pittige avond-gust) — gemiddelde blijft de hele dag onder 14kts, maar de gust loopt 's avonds op tot 22-26kts.
- **Woensdag:** **Goed** (grensgeval) — stevige, consistente 14-22kts vrijwel de hele dag bij alle bronnen, maar pal-aflandige richting en korte, lage golfslag passen niet bij Optimaal.
- **Donderdag:** **Matig** (grensgeval, modeldivergentie) — ideale licht-aflandige hoek, maar Windfinder/windwaarnemingen houden het gemiddelde onder 14kts terwijl Soarcast 15,7-18,9kts ziet.
- **Beste dag in de 7 dagen erna:** zondag 29 november — langste aaneengesloten venster van de outlook-periode met gemiddeld 14-15kts en pal-aflandige richting.

---

## ⏰ Realitycheck vandaag
- Laatste actuele uren (04:00-06:10, windwaarnemingen.nl/IJmuiden, 10-min metingen): **gem. 4,9-8,6 kts** (rond 06:00-06:10 nog ≈5,9-7,1kts), gust **6,1-10,2 kts**, richting draaiend van ZUID/ZZO naar **ZO (125-128°)**.
- Was voorspeld: windwaarnemingen's eigen vsp zag voor 04:00/05:00/06:00 **7,6 / 6,8 / 7,0 kts gem.** (gust 10,9 / 10,9 / 11,3 kts), richting nog **175° / 158° / 154°** (ZUID/ZZO).
- Conclusie: de windkracht zelf loopt ongeveer **CONFORM** verwachting (gemiddelde en gust liggen dicht bij elkaar, meting iets lager op de gust), maar de **richting loopt duidelijk VOOR** — de actuals zijn al naar ZO (125-128°) gedraaid terwijl het model die draai pas rond 07:00-08:00 verwachtte. Rest-van-de-dag inschatting: **licht bijgesteld** — als de richtingsdraai naar de aflandige hoek eerder gebeurt dan gemodelleerd, kan ook de verwachte avondpiek (gust tot 22-26kts rond 17:00-22:00 bij Windfinder) iets naar voren schuiven; de windkracht-classificatie (Slecht-tot-Matig grensgeval) blijft verder ongewijzigd omdat het gemiddelde bij alle bronnen onder 14kts blijft.

---

## 📅 Komende 72 uur

### Dinsdag — Slecht-tot-Matig (grensgeval, pittige avond-gust)
- Windfinder (Superforecast, hourly): wind blijft laag, **6,8-13,1 kts gem.** (nooit boven 14kts), gust loopt in de loop van de dag flink op: **9,1 kts** 's nachts naar **25,9 kts** om 21:00. Richting draait van side-shore/ZUID 's nachts (171-214°, rond de kustlijnhoek) naar pal aflandig overdag/'s avonds (OZO, 107-117°). Golf laag: **0,32-0,41m**, periode **4,39-6,96s** (ruim boven 5s 's ochtends, maar golfhoogte veel te laag voor Optimaal/Goed(b)).
- Soarcast (Harmonie, IJmond): iets hoger dan Windfinder — **9,3-16,9 kts gem., gust 13,4-23,1 kts**, richting 94-219° (zelfde draai, vergelijkbare timing).
- windwaarnemingen.nl (eigen Harmonie-vsp, IJmuiden): **6,8-13,0 kts gem., gust 7,0-20,0 kts**, richting 91-210° — ligt dicht bij Windfinder.
- Netto — alle drie bronnen zijn het eens dat het gemiddelde de hele dag onder de 14kts blijft, maar de gust klimt 's avonds (Windfinder tot 25,9kts, Soarcast tot 23,1kts) ruim boven zowel de Slecht-drempel (16kts) als de Matig/Goed(b)-bovengrens (19kts) — een combinatie die niet in één hokje past: te zwak gemiddeld voor Matig, maar de gust te hoog om het nog puur Slecht te noemen. Grensgeval tussen Slecht en Matig, met een nadrukkelijke pittige-gust-waarschuwing voor de avond.
- Pier-logica: niet van toepassing (richting niet aanlandig, golf blijft onder 0,8m).
- Getij: hoogwater ±02:50 (2,23m), laagwater ±11:21 (0,41m), hoogwater ±15:09 (2,18m), en 's avonds een zwak secundair signaal rond 19:00-20:00 (±0,97-0,99m).
- Beste venster: **geen bruikbaar venster.** Het "minst slechte" moment is ±17:00-22:00 (gust 21,5-25,9kts, richting 107-111° pal aflandig), maar het gemiddelde blijft daar steken op 11-13kts — een onvoorspelbare, pittige gust zonder een dragend gemiddelde.

### Woensdag — Goed (grensgeval)
- Windfinder (Superforecast, hourly): stevige, consistente wind: **12,1-17,1 kts gem.**, gust **23,9-32,5 kts**, richting vrijwel de hele dag pal aflandig (OOST/ONO, **66-104°**). Golf laag: **0,32-0,51m**, periode kort (**2,63-3,59s**, ruim onder 5s).
- Soarcast (Harmonie, IJmond): duidelijk hoger dan Windfinder — **16,1-22,2 kts gem., gust 22,7-30,4 kts** — expliciete afwijking, Soarcast ziet deze dag nog pittiger. Richting 76-95° (ONO/OOST), vergelijkbaar met Windfinder.
- windwaarnemingen.nl (eigen Harmonie-vsp, IJmuiden): **12,1-18,3 kts gem., gust 19,6-28,8 kts**, richting 76-93° — ligt tussen Windfinder en Soarcast in, bevestigt de algemene sterkte van de dag.
- Netto — het gemiddelde zit bij alle drie bronnen solide in de 14-25kts-band gedurende het grootste deel van de dag, maar de richting is overal pal aflandig (binnen ~30° van Zandvoort's pal-aflandige hoek 107,5°) — dit past niet bij Optimaal (vraagt side-shore/licht aflandig) of Goed(a) (vraagt licht aanlandig). Golf blijft laag en de periode kort, wat ook Goed(b) uitsluit (vraagt golf >1,1m). Netto dus een **Goed, grensgeval**: de windkracht is prima wingfoilbaar en opvallend consistent/stevig, maar de formele classificatie wringt door de zuivere aflandige hoek en de korte, platte golfslag.
- Pier-logica: niet van toepassing (richting aflandig, niet aanlandig).
- Getij: laagwater ±23:40 (0,31m, nacht van dinsdag op woensdag), hoogwater ±03:34 (2,22m), laagwater ±11:50 (0,41m), hoogwater ±15:53 (2,26m).
- Beste venster: **±09:00-18:00** — wind 14,0-17,1 kts (Soarcast zelfs 18-22,2 kts), gust 24,3-32,5 kts, richting 69-84° (pal aflandig/ONO). Lange, consistente dag; houd rekening met de forse gust (pieken tot 30+kts).

### Donderdag — Matig (grensgeval, modeldivergentie)
- Windfinder (Superforecast, hourly t/m 19:00): **9,5-13,0 kts gem.** (blijft onder de 14kts-grens), gust **17,0-24,5 kts**, richting opvallend stabiel in de licht-aflandige zone (**62-77°**, de hele dag). Golf laag: **0,20-0,42m**, periode **3,85-5,41s** (kruist de 5s-grens pas laat in de middag, maar golfhoogte blijft te laag voor Optimaal/Goed(b)).
- Soarcast (Harmonie, IJmond, t/m 15:00): duidelijk hoger — **15,7-18,9 kts gem., gust 21,2-26,2 kts** — stevige expliciete afwijking met Windfinder (4-6kts hoger gemiddeld). Richting 78-88° (pal aflandig), iets zuidelijker/oostelijker dan Windfinder.
- windwaarnemingen.nl (eigen Harmonie-vsp, IJmuiden, t/m 15:00): **9,5-14,8 kts gem., gust 19,0-23,9 kts**, richting 80-88° — ligt dicht bij Windfinder op snelheid, dicht bij Soarcast op richting.
- Netto — grensgeval met een nadrukkelijke modeldivergentie: Windfinder en windwaarnemingen houden het gemiddelde de hele dag onder 14kts (Matig-gebied), terwijl Soarcast met 15,7-18,9kts stevig in de Optimaal/Goed-band zou vallen. De richting is bij Windfinder de hele dag licht aflandig (62-77°) — exact het gunstige profiel voor Optimaal — terwijl Soarcast/windwaarnemingen die net iets zuidelijker (pal aflandig, 78-88°) zien. Golf blijft bij alle bronnen te laag voor Optimaal/Goed(b). Gegeven de 2-op-3 verdeling op windkracht: netto **Matig, grensgeval** — met expliciete kans op Optimaal/Goed als Soarcast gelijk heeft.
- Pier-logica: niet van toepassing (richting aflandig, niet aanlandig).
- Getij: laagwater ±00:30 (0,34m, nacht van woensdag op donderdag), hoogwater ±04:20 (2,18m), laagwater ±12:24 (0,38m), hoogwater ±16:37 (2,31m).
- Beste venster: **±06:00-12:00** — wind 11,3-14,6 kts (Soarcast 16,2-18,9 kts), gust 22,1-26,2 kts, richting 62-88° (licht aflandig tot pal aflandig). Check dichter bij de tijd welk model gelijk krijgt.

---

## 🔭 Kans op mooie sessies daarna (dag 4-9)
Windfinder (GFS, enige bron zo ver vooruit) voor **vrijdag 27 november t/m woensdag 3 december**. Let op: voor vrijdag, zondag en dinsdag 1 december ontbrak golfdata in de statische extractie — beoordeling daar uitsluitend op wind/gust/richting.

- **Vrijdag 27 november** (dag 4): **10,2-11,0 kts gem.**, gust **14,8-18,6 kts**, richting pal aflandig (**94-105°**). Golfdata ontbreekt. **Matig**, aan de zwakke kant — gemiddelde komt de hele dag niet in de buurt van 14kts.
- **Zaterdag 28 november** (dag 5): **9,4-15,0 kts gem.**, gust **14,0-24,7 kts**, richting pal aflandig (**100-116°**). Golf zeer laag (**0,14-0,32m**), periode kort (**2,92-3,99s**). **Matig**, 's avonds (±19:00) kort het sterkst met 15,0kts gem.
- **Zondag 29 november** (dag 6): **12,6-15,2 kts gem.**, gust **23,1-28,5 kts**, richting pal aflandig (**99-115°**). Golfdata ontbreekt. **Goed, grensgeval** — van ±07:00 tot ±22:00 vrijwel aaneengesloten 14,3-15,2kts gem., de langste sterke periode van het hele dag 4-9-blok, maar de pal-aflandige hoek (net als woensdag) sluit een formele Optimaal-classificatie uit.
- **Maandag 30 november** (dag 7): **11,4-15,1 kts gem.**, gust **18,9-27,2 kts**, richting pal aflandig (**98-107°**). Golf **0,44-0,49m** (hoogste van de outlook-periode, nog steeds onder 1,1m), periode **4,38-4,96s** (net onder 5s). **Goed-tot-Matig grensgeval**, sterkst in de vroege ochtend (01:00-07:00, 14,5-15,1kts).
- **Dinsdag 1 december** (dag 8): **9,0-11,6 kts gem.**, gust **14,0-19,0 kts**, richting pal aflandig (**94-104°**). Golfdata ontbreekt. **Matig**, zwak — gemiddelde blijft de hele dag onder 12kts.
- **Woensdag 3 december** (dag 9, let op: dit is dus al dag 9 vanaf vandaag): **8,3-9,1 kts gem.**, gust **11,3-13,6 kts**, richting ONO/licht aflandig (**70-95°**). Golf **0,44-0,58m**, periode **4,06-5,16s**. **Slecht** — gust blijft onder de 16kts-Slecht-grens, gemiddelde ruim onder 14kts.

**Beste dag: zondag 29 november** — de langste aaneengesloten sterke periode van het hele dag 4-9-blok (±07:00-22:00 vrijwel constant 14-15kts gem.), al blijft de pal-aflandige richting een grensgeval-handicap voor een formele Optimaal-classificatie en ontbrak golfdata voor deze dag in de extractie. Kans: **gemiddeld-tot-hoog**. Let op: de outlook voor dit deel van de week is sinds de vorige briefing fors naar boven herzien (zondag werd gisteravond nog als vrijwel windstil ingeschat) — een duidelijk signaal dat voorspellingen op deze afstand nog flink kunnen kantelen. ⚠️ Onzeker op 4+ dagen — check dichter bij de tijd opnieuw.

---
_Bronnen: Windfinder (GFS / Superforecast ICON-EU) · Soarcast (KNMI Harmonie, IJmond) · windwaarnemingen.nl (KNMI, IJmuiden)_
