# 🌊 Wingfoil-briefing Zandvoort–Wijk aan Zee
_28-09-2026 · Ochtendbriefing_

⚠️ **Technische kanttekening deze run:** Soarcast kon opnieuw niet geraadpleegd worden — het blijft een volledige JS-app (React/Vite) waarvan de onderliggende data-API-call niet in de uitgeleverde JS-bundle als vast adres terug te vinden is (vermoedelijk same-origin/runtime-geconfigureerd), en eerdere sessies liepen hier al tegenaan met een netwerkbeleid-blokkade op het achterliggende domein. Windfinder en windwaarnemingen.nl zijn dit keer wél volledig gelukt, inclusief de volledige dag 1-9 via de onderliggende paginadata (in plaats van alleen de zichtbare tabel) en de directe KNMI-vsp/actuals-JSON van windwaarnemingen.nl.

---

## ⚡ Snel overzicht
- **Maandag:** Slecht (geen bruikbaar venster)
- **Dinsdag:** Slecht (geen bruikbaar venster in daglicht)
- **Woensdag:** Matig (grensgeval, gusty, 08:00-11:00)
- **Beste dag in de 7 dagen erna:** zaterdag 3 oktober (marginaal — zie toelichting)

---

## ⏰ Realitycheck vandaag

- Laatste actuele uren (windwaarnemingen.nl, IJmuiden, 05:00-07:10): **wind 3,6-6,2 kts, gust 4,4-7,1 kts, richting 183-211° (Zuid/ZZW)**
- Was voorspeld voor dezelfde uren: KNMI-vsp (windwaarnemingen.nl, huidige modelrun) gaf voor 05:00-07:00 slechts **2,8-3,4 kts, gust 4,1-5,3 kts, richting 182-192° (Zuid/ZZW)**; Windfinder (GFS) gaf voor 05h **7 kts, gust 10 kts, richting 212°**
- Conclusie: de wind **loopt VOOR** t.o.v. KNMI-vsp — bij 07:00 zelfs meer dan het dubbele van wat de KNMI-modelrun gaf (6,2 vs 2,8 kts) — maar blijft **onder** Windfinder's eigen inschatting voor dat tijdstip (7 kts). Richting komt in alle drie bronnen goed overeen (Zuid/ZZW). Voor de rest van de dag: **vertrouwen licht naar boven bijgesteld t.o.v. KNMI-vsp, maar classificatie ongewijzigd** — zelfs met deze correctie blijft de wind ruim onder de 14 kts (gem) / 16 kts (gust) die nodig is om aan "Slecht" te ontsnappen.

---

## 📅 Komende 72 uur

### Maandag — Slecht
- **Geen bruikbaar venster overdag.** Windfinder (GFS): 08h 7 kts/12 kts gust (206°, side-shore), 11h 5/6 (234°), 14h 8/8 (347°, side-shore/licht aanlandig-grens), 17h 10/12 (6°, side-shore), 20h 10/15 (39°, side-shore). Alles blijft onder de 14 kts (gem) / 16 kts (gust)-drempel voor "Slecht".
- Pas na zonsondergang (~19:35) trekt het iets aan: 21h 9 kts/16 kts gust en 23h 11/16 kts (46-53°, side-shore) — net op de grens met Matig, maar te laat/donker om praktisch te zijn.
- Golven: 0,3-0,6 m / 3-5 s de hele dag — ruim onder de 1,1 m-drempel.
- Getij: laagwater ~01:05 (0,3 m), hoogwater ~05:22 (2,3 m), laagwater ~13:22 (0,5 m), hoogwater ~17:43 (2,1 m), laagwater ~21:37 (0,8 m).
- Bronnen: Windfinder en KNMI-vsp (windwaarnemingen.nl) **eens** over een zwakke dag, maar KNMI-vsp geeft over de hele dag structureel lagere waarden (nooit boven 5,4 kts gem/8,4 kts gust) dan Windfinder — een aanzienlijk verschil in absolute windkracht, richting komt wel overeen. Actuele meting ligt tussen beide in (zie Realitycheck). Soarcast ontbreekt deze run.

### Dinsdag — Slecht
- **Geen bruikbaar venster in daglicht** (zonsopkomst ~07:35). Windfinder (GFS) laat wél een gusty piek zien, maar die valt vóór zonsopgang: 02h 11 kts/**18 kts gust** (70°, licht aflandig), 05h 10/17 (82°, pal aflandig) — dit haalt net "Matig", maar is niet bruikbaar in het donker.
- Zodra het licht wordt, valt de wind bij Windfinder terug naar Slecht-niveau: 08h 8 kts/12 kts gust (75°), 11h 8/12 (108°), 14h 7/10 (131°), 17h 8/12 (146°) — allemaal onder de 14/16-drempel.
- **Opvallende modeldivergentie:** KNMI-vsp (windwaarnemingen.nl) voorspelt voor exact dezelfde periode een veel vlakkere, zwakkere dag — nooit boven 6,6 kts gem/10,6 kts gust, ook niet in de vroege ochtend. Dit is een duidelijke afwijking t.o.v. Windfinder's pre-dawn piek; vermeld hier expliciet i.p.v. gemiddeld. Ter vergelijking: de briefing van 27 september voorspelde op basis van een eerdere KNMI-modelrun nog een sterkere ochtendgunst voor dinsdag (13,6 kts/21 kts gust rond 06:00) — de nieuwste modelrun heeft dit fors naar beneden bijgesteld.
- Golven: 0,2-0,5 m / 4-6 s — ruim onder de 1,1 m-drempel.
- 🌊 Piervoorkeur: niet van toepassing (golf blijft overal <0,8 m).
- Getij: laagwater ~01:37 (0,3 m), hoogwater ~05:59 (2,3 m), laagwater ~13:48 (0,5 m).
- Bronnen: Windfinder en KNMI-vsp **wijken duidelijk af** in de vroege ochtend (Windfinder gusty pre-dawn piek, KNMI-vsp vlak en zwak de hele dag); voor de praktisch bruikbare daguren zijn beide bronnen het wel eens dat het zwak blijft. Soarcast ontbreekt deze run.

### Woensdag — Matig (grensgeval, gusty ochtend)
- **Beste venster: 08:00-11:00** — Windfinder (GFS): 08h 11 kts/**20 kts gust** (147°, licht aflandig), 11h 11/19 (166°, side-shore). Dit zit met het gemiddelde (10-11 kts) net onder de 14 kts-drempel voor "Goed", terwijl de gust (19-20 kts) de "Matig"-grens van <19 kts overschrijdt — een grensgeval, vandaar dat het niet in één vakje past. Golf blijft met 0,25-0,28 m (Windfinder, enige golfbron) ruim onder de 1,1 m-drempel.
- Ervoor (05h: 10 kts/19 kts gust, 145°) en erna (14h-17h: 9 kts/14 kts gust, Slecht) valt het gemiddelde verder terug; laat in de avond (20h) trekt de gust weer wat op (9 kts/16 kts, 194°, side-shore) maar dat is grensgeval Matig/Slecht en na zonsondergang.
- **Let op patroonverschuiving:** deze gusty ochtendspurt uit de ONO/OZO-hoek is vergeleken met de briefing van 27 september een dag opgeschoven — toen werd dit patroon nog voor dinsdag voorspeld, nu voor woensdag.
- KNMI-vsp (windwaarnemingen.nl, dekking tot 16:00) geeft voor dezelfde uren een structureel veel zwakker beeld: 08:00 5,3 kts/8,1 kts gust, 11:00 5,3/8,0 kts — net als bij de vorige twee dagen een grote afwijking t.o.v. Windfinder, terwijl de richting (Zuid-ZZO-achtig, iets zuidelijker dan Windfinder's ONO) wel enigszins in dezelfde waaier zit.
- Golven: 0,21-0,5 m / 3-5 s — onder de 1,1 m-drempel de hele dag.
- 🌊 Piervoorkeur: niet van toepassing (golf blijft <0,8 m).
- Bronnen: Windfinder en KNMI-vsp **wijken sterk af** in absolute windkracht (Windfinder 2-3x hoger dan KNMI-vsp), maar tonen een vergelijkbaar dagpatroon (gusty ochtend, afzwakkend in de middag). Soarcast ontbreekt deze run.

---

## 🔭 Kans op mooie sessies daarna (dag 4-9)
Dit wordt een uitgesproken windstille periode. Windfinder (GFS, enige bron zo ver vooruit) laat voor **donderdag 1 t/m dinsdag 6 oktober** geen enkele dag zien die boven de 8 kts gemiddeld of 10 kts gust uitkomt — bij lange na niet genoeg voor een classificatie boven "Slecht". **Zaterdag 3 oktober** springt er nog het minst slecht uit met een korte oplopende gust naar 9,7 kts rond 20:00 (66°, ONO/side-shore) en overdag 6-8 kts gemiddeld, maar dat is nog steeds ruim onder elke bruikbare drempel. Donderdag 1 en vrijdag 2 oktober blijven vlak (max ~6,5 kts gem/8,4 kts gust), zondag 4 en maandag 5 oktober vergelijkbaar zwak (max ~5,9 kts gem/8,1 kts gust) — maandag 5 oktober laat wel een opbouwende golf zien (tot 0,72 m/5,1 s) maar zonder bijbehorende wind is dat niet bruikbaar. Dinsdag 6 oktober blijft eveneens zwak (max 4,8 kts/5,5 kts gust).
Kans: **laag** voor de hele periode, met zaterdag 3 oktober als minst-slechte optie.
⚠️ Onzeker op 4+ dagen — check dichter bij de tijd opnieuw; een periode die er nu als volledige windstilte uitziet kan bij een volgende modelrun nog verschuiven.

---
_Bronnen: Windfinder (GFS) · windwaarnemingen.nl (KNMI, IJmuiden) · Soarcast — deze run niet bereikbaar (JS-app, geen vindbaar/bereikbaar API-adres)_
