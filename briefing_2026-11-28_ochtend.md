# 🌊 Wingfoil-briefing Zandvoort–Wijk aan Zee
_28-11-2026 · Ochtendbriefing_

⚠️ **Technische kanttekening:** alle drie bronnen rechtstreeks via curl/API opgehaald (geen interactieve browser nodig). Windfinder: de reguliere forecast-pagina is een Astro-site die per dag een eigen `ForecastSection`-widget server-side meestuurt met volledige uurlijkse wind+golf+getij-data; vandaag en morgen zaten in de hoofdwidget, de dagen daarna (ma/wo/vr/zo) in losse "preview-card"-widgets die slechts om de dag golfdata meesturen (di/do/za ontbreken golfdata — daar alleen windtabel). De Superforecast-pagina vulde golfdata voor vandaag/morgen/overmorgen verder aan. Soarcast: endpoint `sc/plotPerLocAndUnitReact.php?json&jsonOnly&unit=m/s|deg&location=133&day=0/1/2&forecastToShow=harm` (wind/gust apart van richting, aparte call per unit). windwaarnemingen.nl: `database/vsp_vdg_wstats.php?st=IJmuiden1` (vandaag, 10-min actuals + uurlijkse vsp terugwerkend) en `vsp_mrg_wstats.php?st=IJmuiden2` (morgen + overmorgen t/m 15:00 vsp) — windsnelheid/gust in m/s, omgerekend naar knopen.

**Netto beeld — een zaterdag (vandaag) die van een zwakke, vlagerige ochtend doorbouwt naar een stevige avond met ideale richting, een zondag die het sterkst is net na middernacht en daarna snel inzakt, en een maandag die overwegend te zwak blijft. Soarcast voorspelt voor vandaag en morgenochtend structureel 4-6kts hoger dan Windfinder en windwaarnemingen, die onderling goed overeenkomen — dit is nadrukkelijk geen gemiddelde maar een bronafwijking om in de gaten te houden. In de outlook springt woensdag 2 december er opnieuw uit als de sterkste dag van het hele dag 4-9-blok, met een optimale side-shore sessie overdag.** De Realitycheck van vanochtend laat zien dat de wind iets achterblijft bij de voorspelling, vooral in de gust.

---

## ⚡ Snel overzicht
- **Zaterdag:** **Goed** (grensgeval, richting Optimaal) (±19:00-23:00)
- **Zondag:** **Goed** (grensgeval, richting Optimaal) (±00:00-03:00)
- **Maandag:** **Matig** (grensgeval) (±14:00-19:00)
- **Beste dag in de 7 dagen erna:** woensdag 2 december — duidelijk de sterkste en meest kansrijke dag van het hele dag 4-9-blok.

---

## ⏰ Realitycheck vandaag
- Laatste actuele uren (04:00-06:10, windwaarnemingen.nl/IJmuiden, omgerekend m/s→kts): **gem. 9,5-11,9 kts**, gust **13,0-17,1 kts**, richting **126-131° (ZO/OZO, pal aflandig)**.
- Was voorspeld: windwaarnemingen's eigen uurlijkse vsp voor 04:00/05:00/06:00 zag **10,3 / 8,7 / 10,1 kts gem.** (gust 16,5 / 15,7 / 15,4 kts), richting **143 / 141 / 131° (ZO)**.
- Conclusie: het gemiddelde liep om 04:00-05:00 nog **VOOR** (+1,6 tot +1,9kts boven de vsp), maar de gust bleef het hele venster **ACHTER** (-1,4 tot -2,4kts onder de vsp) en tegen 06:00 is ook het gemiddelde licht onder de voorspelling gezakt (-0,5kts). Richting kwam iets oostelijker uit (meer pal aflandig) dan voorspeld, wat de classificatie niet verandert. Rest-van-de-dag inschatting: **licht naar onder bijgesteld**, vooral voor de gust vanavond — ga uit van de onderkant van de Windfinder/windwaarnemingen-bandbreedte (gust ±27-29kts, gem. 14-16kts) in plaats van Soarcast's aanzienlijk hogere cijfers (gem. tot 22kts) voor vanavond.

---

## 📅 Komende 72 uur

### Zaterdag — Goed (grensgeval, richting Optimaal)
- Windfinder (ForecastSection, hourly GFS/ICON): wind **8,9-16,1 kts gem.** (geleidelijk stijgend door de dag), gust **19,1-28,9 kts**, richting draait van **132-144° (pal/licht aflandig)** 's nachts/ochtends naar **148-166° (licht aflandig → side-shore)** in de avond. Golf bouwt rustig op van **0,14m/3,3s** 's nachts naar **0,62m/5,3s** aan het einde van de avond.
- Soarcast (Harmonie, IJmond): duidelijk hoger de hele dag — **12,6-22,0 kts gem., gust 17,3-29,5 kts**, richting 121-155° (vergelijkbaar patroon, maar 4-6kts hoger in het gemiddelde — expliciete modeldivergentie, niet middelen).
- windwaarnemingen.nl (eigen Harmonie-vsp, IJmuiden): sluit het dichtst aan bij Windfinder — **8,7-17,5 kts gem., gust 13,6-27,2 kts**, richting 116-158°.
- Netto — Windfinder en windwaarnemingen zijn het onderling eens (8,7-17,5kts), Soarcast zit er structureel 4-6kts boven. 's Ochtends en middags blijft het gemiddelde grotendeels onder de 14kts-grens terwijl de gust al wel 19-26kts haalt — een vlagerig grensgeval dat niet netjes in één categorie past (Matig qua gemiddelde, maar gust te hoog voor die drempel). Vanaf ±16:00 komt het gemiddelde in de 14-25kts-band en draait de richting naar het ideale side-shore/licht-aflandige venster, maar de golf blijft net onder de 1,1m-Optimaal-grens (max 0,62m) ondanks een oplopende periode (tot 5,3s). Netto **Goed, grensgeval** — de avond had Optimaal kunnen zijn met iets meer golfhoogte.
- Pier-logica: niet van toepassing (windrichting de hele dag aflandig/side-shore, niet aanlandig).
- Getij: laagwater ±01:46 (0,38m), hoogwater ±05:57 (2,0m), laagwater ±13:51 (0,26m), hoogwater ±18:11 (2,26m).
- Beste venster: **±19:00-23:00** — wind 14,2-16,1 kts (Soarcast 19,6-22,0 kts), gust 27,7-28,9 kts, richting 153-166° (side-shore). Vlagerig karakter; houd gezien de Realitycheck rekening met de onderkant van deze bandbreedte.

### Zondag — Goed (grensgeval, richting Optimaal)
- Windfinder (ForecastSection, hourly): wind **15,0-15,4 kts gem.** net na middernacht, daarna geleidelijk dalend naar **4,1-11,4 kts** in de middag/avond, gust **24,1-28,2 kts** 's nachts kalvend naar **7,9-19,6 kts**. Richting side-shore **160-199°** tot ±17:00, draait daarna naar **200-295° (aanlandig, west/noordwest)** in de avond bij sterk afgenomen wind. Golf **0,59-0,79m**, periode **4,4-6,4s** (periode ruim ≥5s vanaf 00:00-16:00, hoogte blijft net onder 1,1m).
- Soarcast (Harmonie, IJmond): hoger in de nacht/vroege ochtend — **16,1-21,6 kts gem., gust 20,0-29,5 kts**, richting 160-191° (vergelijkbaar patroon, weer 4-6kts boven Windfinder).
- windwaarnemingen.nl (eigen Harmonie-vsp, IJmuiden, hele dag): **6,0-17,3 kts gem., gust 9,0-26,4 kts**, richting 158-187° — sluit qua niveau dichter bij Windfinder aan dan Soarcast, bevestigt de dalende lijn door de dag.
- Netto — alle drie bronnen bevestigen: sterkst vlak na middernacht (aansluitend op zaterdagavond), met ideale side-shore richting en periode ruim boven 5s, maar golfhoogte net onder de 1,1m-grens. Vanaf de ochtend valt de wind snel terug en wordt het rond het middaguur al **Slecht** (gust<16 én gem<14 vanaf ±13:00). De avondzwenking naar aanlandig is irrelevant — wind dan te zwak (4-7kts) om nog iets te betekenen. Netto voor het beste moment: **Goed, grensgeval** — vergelijkbaar met zaterdagavond, had Optimaal kunnen zijn met iets meer golfhoogte.
- Pier-logica: niet van toepassing (het venster met voldoende wind is side-shore, niet aanlandig; de latere aanlandige zwenking heeft te weinig wind om relevant te zijn).
- Getij: laagwater ±02:27 (0,39m), hoogwater ±06:50 (1,89m), laagwater ±14:38 (0,21m), hoogwater ±19:05 (2,18m).
- Beste venster: **±00:00-03:00** — wind 15,0-15,4 kts (Soarcast 17,9-21,6 kts), gust 25,8-28,2 kts, richting 160-176° (side-shore). Vroeg venster, direct aansluitend op zaterdagavond.

### Maandag — Matig (grensgeval)
- Windfinder (Superforecast, hourly): wind **7,5-12,3 kts gem.** (vlak, licht stijgend in de middag/avond), gust **11,3-21,7 kts**, richting vrijwel de hele dag **side-shore (182-236°)**. Golf bouwt verder op van **0,62m** 's nachts naar **0,83m** overdag, periode stijgt van **4,4s naar 5,5s** (periode haalt de 5s-grens pas vanaf ±07:00, hoogte komt nooit boven 1,1m).
- Soarcast (Harmonie, IJmond): vergelijkbaar niveau — **10,1-12,6 kts gem., gust 14,0-18,5 kts**, richting 166-192° (hier geen noemenswaardige divergentie met Windfinder).
- windwaarnemingen.nl (eigen Harmonie-vsp, IJmuiden, t/m 15:00): laagste van de drie — **7,6-9,3 kts gem., gust 11,5-14,8 kts**, richting 160-187°.
- Netto — alle drie bronnen zijn het eens: een zwakke, vlakke dag. Het grootste deel van de dag (±00:00-14:00) is het gemiddelde <14kts mét gust <16kts → **Slecht**. Vanaf ±15:00 trekt de gust net genoeg aan (15-18,5kts) om in de Goed(b)-wind-bandbreedte (<15kts gem, gust<19kts) te vallen en is de richting side-shore (niet pal aanlandig) — maar de golf blijft met 0,83m onder de 1,1m-grens, dus geen Goed(b), wel **Matig**. Netto **Matig, grensgeval**, zwakste van de drie dagen.
- Pier-logica: niet van toepassing (richting de hele dag side-shore, niet aanlandig).
- Getij: laagwater ±03:16 (0,42m), hoogwater ±07:50 (1,8m), laagwater ±15:29 (0,2m), hoogwater rond ±20:00 (data loopt tot 19:00 bij 1,72m en stijgend; exacte piektijd niet in dataset).
- Beste venster: **±14:00-19:00** — wind 11,3-12,6 kts (Soarcast 10,1-12,6 kts), gust 15,6-18,5 kts, richting 184-193° (side-shore). Zwak maar het beste moment van een matige dag.

---

## 🔭 Kans op mooie sessies daarna (dag 4-9)
Windfinder (GFS, enige bron zo ver vooruit) voor **dinsdag 1 december t/m zondag 6 december**. Let op: voor dinsdag, donderdag en zaterdag leverde de site geen golfdata (alleen om-de-dag-cards hebben golf); daar is de golfinschatting een interpolatie tussen de omliggende dagen, expliciet als zodanig gemarkeerd.

- **Dinsdag 1 december** (dag 4): **12,9-15,2 kts gem.**, gust **20,6-28,1 kts**, richting **side-shore (178-188°)**, vrijwel de hele dag vlak. Golfdata ontbreekt in de dataset; op basis van maandag (tot 0,83m) en woensdag (1,06-1,15m) ligt de golf waarschijnlijk rond **0,85-1,0m**, periode naar schatting ≥5s. Met wind in de 14-25kts-band en ideale richting, maar golf (geschat) nog net onder 1,1m: **Goed, grensgeval** — dicht bij Optimaal.
- **Woensdag 2 december** (dag 5): **14,8-15,8 kts gem.** overdag (vlak en sterk), gust **23,6-28,2 kts**, richting overdag side-shore (**188-196°**). Golf **1,06-1,15m**, periode **5,9-6,5s** — ruim boven de Optimaal-drempel. Overdag (±07:00-16:00) voldoet dit letterlijk aan **Optimaal**: wind in band, side-shore, golf >1,1m én periode ≥5s. 's Avonds zwenkt de richting scherp naar **283-349° (NW/N, aanlandig)** bij afnemende wind (9,1-12,8kts) en golf die rond 1,08-1,15m blijft. Pier-logica van toepassing voor die avondzwenking: richting NW/N + golf ≥0,8m → **IJmuiden (Zuidpier) rustiger**.
- **Donderdag 3 december** (dag 6): **7,7-16,3 kts gem.** (sterkst 's ochtends, neemt gedurende de dag af), gust **11,1-22,8 kts**, richting **327-353° (NW/NNW)** — vervolg van de zwenking van woensdagavond, drift van licht aanlandig naar side-shore. Golfdata ontbreekt in de dataset; op basis van woensdag (1,06-1,15m) en vrijdag (0,70-1,01m) ligt de golf waarschijnlijk rond **0,85-1,0m**, afnemend. 's Ochtends (14,5-16,3kts, licht aanlandig, golf geschat <1,1m): **Goed(a), grensgeval**. Pier-logica van toepassing: richting NW/NNW (aanlandig) + golf (geschat) ≥0,8m → **IJmuiden (Zuidpier) rustiger**.
- **Vrijdag 4 december** (dag 7): **4,1-6,7 kts gem.**, gust **4,9-9,0 kts** — duidelijk te zwak. Golf nog behoorlijk (0,70-1,01m, periode 6,6-6,8s) maar irrelevant zonder wind. **Slecht**.
- **Zaterdag 5 december** (dag 8): **0,9-5,3 kts gem.**, gust **1,5-6,0 kts** — windstille lul-dag. **Slecht**.
- **Zondag 6 december** (dag 9): **4,9-7,1 kts gem.**, gust **5,3-8,6 kts**, golf **0,38-0,44m** ondanks een lange periode (5,98-6,45s) — wind te zwak om iets te betekenen. **Slecht**.

**Beste dag: woensdag 2 december** — duidelijk de sterkste en vlakste wind van de hele dag 4-9-periode (14,8-15,8kts), de hoogste golf van de week (tot 1,15m, boven de Optimaal-grens) en een overdag-venster dat letterlijk aan de Optimaal-criteria voldoet. Kans: **gemiddeld-tot-hoog**. Dinsdag 1 december is een goed alternatief vooraf (Goed, grensgeval), donderdag 3 december erna dankzij de pierbescherming bij IJmuiden, al met zwakkere wind. ⚠️ Onzeker op 4+ dagen — check dichter bij de tijd opnieuw.

---
_Bronnen: Windfinder (GFS / Superforecast) · Soarcast (KNMI Harmonie, IJmond) · windwaarnemingen.nl (KNMI, IJmuiden)_
