# 🌊 Wingfoil-briefing Zandvoort–Wijk aan Zee
_02-10-2026 · Ochtendbriefing_

⚠️ **Technische kanttekening deze run:** Soarcast is (net als alle voorgaande runs) niet bereikbaar — een volledige JS-app (Vite-bundle) zonder vindbaar/bereikbaar API-adres. Windfinder is rechtstreeks via de onderliggende paginadata (astro-hydration props) opgehaald — één bezoek aan de forecast-pagina leverde zowel de korte termijn als, verrassend, de volledige 3-uurs data t/m 11 oktober in dezelfde payload (geen apart bezoek aan de Superforecast-pagina nodig). windwaarnemingen.nl (IJmuiden) is via de onderliggende vsp-JSON-endpoints opgehaald (10-minuten-actuals voor vandaag plus het uurmodel voor morgen/overmorgen).

---

## ⚡ Snel overzicht
- **Vrijdag:** Matig — venster **12:00-16:00** (opgewaardeerd t.o.v. het ruwe modelbeeld, zie Realitycheck)
- **Zaterdag:** Slecht
- **Zondag:** Slecht
- **Beste dag in de 7 dagen erna:** donderdag 8 oktober

---

## ⏰ Realitycheck vandaag

- Laatste actuele uren (windwaarnemingen.nl, IJmuiden, 05:00-07:10): **wind 7,3-7,9 kts gem, gust 7,9-8,6 kts, richting vrij stabiel zuidelijk (161-183°, ZUID/ZZO)**.
- Was voorspeld voor dezelfde uren: KNMI-vsp (huidige modelrun) gaf **05:00 181° ZUID, 5,4/7,2 kts**; **06:00 171° ZUID, 4,7/7,2 kts**; **07:00 157° ZZO, 5,4/7,6 kts**. Windfinder (GFS, 3-uurs) gaf voor het 05h-blok **198° ZZW, 4/5 kts**.
- Conclusie: windkracht **loopt merkbaar VOOR** — de actuele gemiddelden liggen ~35-50% boven de KNMI-vsp-voorspelling voor dezelfde uren, en nog verder boven Windfinder (GFS lijkt deze ochtend het zwakst in te zitten). Richting klopt wel goed (beide modellen zaten al op zuid/ZZO). Voor de rest van de dag: inschatting **bijgesteld van Slecht naar Matig** voor het middagvenster — met dezelfde ~35-50%-opslag op de KNMI-vsp-piek rond 13:00 (9,7/14,0 kts kaal → geschat ca. 13-14/16-19 kts) kom je ruim boven de Slecht-drempel uit, maar nog niet overtuigend in Goed(b)-gebied omdat de golf de hele dag ruim onder de 1,1 m blijft. Dit blijft een voorzichtige opwaardering — niet hard bevestigd, want gebaseerd op een extrapolatie van 3 vroege ochtenduren.

---

## 📅 Komende 72 uur

### Vrijdag — Matig (onder voorbehoud, zie Realitycheck)
- **Kaal modelbeeld (zonder de ochtend-opslag) is overal Slecht**: Windfinder 02h-23h loopt van 4-8 kts gem / 4-9 kts gust (richting 162-244°, zuid draaiend naar zuidwest). KNMI-vsp geeft een vergelijkbaar kaal beeld maar met een iets hogere piek: 12:00 8,4/12,2 kts (208°, ZZW), **13:00 9,7/14,0 kts (221°, ZW)**, 14:00 9,1/14,0 kts (225°), 15:00 8,4/13,4 kts (226°), 16:00 7,0/12,2 kts (234°) — dit is de bron van het opgewaardeerde middagvenster.
- **Toegepaste opslag uit de Realitycheck** (ochtend liep ~35-50% boven KNMI-vsp): geschat middagvenster **12:00-16:00, ca. 11-14 kts gem / 14-19 kts gust**, piek rond 13:00 — dit landt in **Matig**, met een klein kans op een korte **Goed(b)**-piek rond 13:00 als de opslag aan de hoge kant uitvalt. Richting side-shore tot licht aanlandig bij Zandvoort (208-234°, randgeval rond 244° om 17h).
- Golven (Windfinder, enige golfbron): 0,2-0,5 m / 4-5 s — ruim onder de 1,1 m-drempel de hele dag, dus geen Optimaal/Goed(b) mogelijk ongeacht wind.
- 🌊 Piervoorkeur: niet van toepassing (golf <0,8 m).
- Getij: laagwater ~03:20 (0,3 m), hoogwater ~08:03 (2,0 m), laagwater ~15:52 (0,4 m), hoogwater ~20:21 (2,1 m).
- Bronnen: Windfinder en KNMI-vsp zijn het **kaal eens** (Slecht) — de opwaardering komt uitsluitend uit de Realitycheck-vergelijking met de actuele ochtendmetingen, niet uit de modellen zelf. Soarcast niet bereikbaar.

### Zaterdag — Slecht
- Windfinder: hele dag zwak — 4-6 kts gem / 5-7 kts gust, richting 159-357° (zuid draaiend via west naar noord gedurende de dag) — nergens boven de Matig-drempel.
- Geen KNMI-vsp-dekking meer voor deze dag in de opgehaalde data (dekt alleen vandaag + morgenochtend); Windfinder is hier de enige bron.
- Golven: 0,2-0,3 m / 4 s.
- 🌊 Piervoorkeur: niet van toepassing.
- Getij: laagwater ~04:05 (0,3 m), hoogwater ~08:55 (1,8 m), laagwater ~16:43 (0,4 m), hoogwater ~21:14 (2,0 m).
- Bronnen: alleen Windfinder beschikbaar voor deze dag — zwak beeld, geen tegenstrijdige signalen. Soarcast niet bereikbaar.

### Zondag — Slecht
- Windfinder (3-uurs, uit dezelfde payload als de lange termijn): hele dag zwak, 2-10 kts gem / 2-10 kts gust, richting draait van noord (16°) via oost (89°, kort pal aflandig) naar noordwest (335°) — nergens boven de Matig-drempel.
- KNMI-vsp (uurmodel, dekt tot 16:00 deze dag) bevestigt eenzelfde zwak beeld, consistent met Windfinder — geen divergentie.
- Golven: 0,22-0,33 m / 3,9-4,8 s.
- 🌊 Piervoorkeur: niet van toepassing.
- Getij: geen exacte laag/hoogwatertijden uit de opgehaalde data af te leiden (alleen tussentijdse hoogtes met trend); globaal vergelijkbaar ritme met voorgaande dagen.
- Bronnen: Windfinder en KNMI-vsp **eens** — zwakke dag. Soarcast niet bereikbaar.

---

## 🔭 Kans op mooie sessies daarna (dag 4-9)
Windfinder (GFS, enige bron zo ver vooruit — deze keer in één keer t/m 11 oktober opgehaald) laat voor **maandag 5 t/m zaterdag 10 oktober** het volgende beeld zien:
- **Maandag 5 oktober**: zwak tot matig, 6-10 kts gem (max 9,8 kts gust 12,4), richting zuidwest (210-244°) — overwegend **Slecht**, golf 0,4-0,7 m.
- **Dinsdag 6 oktober**: vergelijkbaar zwak, 2-9 kts gem, richting draait naar west/zuidwest (217-294°) en komt bij Zandvoort **pal aanlandig** te liggen vanaf 11:00, maar de wind is te zwak (6-9 kts) om dat relevant te maken — **Slecht**. Golf loopt al op naar 0,6-0,7 m.
- **Woensdag 7 oktober**: overwegend **Slecht** overdag, maar bouwt vanaf de avond snel op — 20:00 al 16,0/22,9 kts (252°, licht aanlandig bij Zandvoort) — **Goed(a)**, en 23:00 14,3/19,3 kts (299°, pal aanlandig) — grensgeval. Golf loopt op naar 0,75-0,86 m en nadert de 0,8 m-pierdrempel tegen middernacht.
- **Donderdag 8 oktober — beste dag, breed en stevig venster**: wind bouwt 's nachts al door naar 20-25 kts gem / 24-28 kts gust uit het noordwesten (293-332°). Bij **Zandvoort** is dit overwegend **pal aanlandig tot licht aanlandig** (grensgeval, minder ideale hoek), maar bij **IJmuiden** is dezelfde richting dankzij de eigen pierzone-hoek (150°/330°) **side-shore** — en dat levert vrijwel de **hele dag Optimaal** op bij IJmuiden: van 05:00 (20,4/23,7 kts, golf 1,13 m/6,2 s) tot 23:00 (16,7/20,1 kts, golf 1,60 m/7,7 s), met een piek rond 11:00-17:00 van 21,6-23,5 kts gem / 26-27 kts gust en golf tot 1,68 m / 7,2 s. 🌊 **Piervoorkeur: IJmuiden rustiger** de hele dag (wind 293-332° valt ruim in de NW-band waar de Zuidpier de golfslag breekt) — let op: bij deze windkracht (6+, >27 kts rond 02:00 en 08:00-11:00) sluit de Reddingsbrigade IJmuiden normaliter de pieren voor wandelaars, een signaal dat het er ruw aan toe gaat.
- **Vrijdag 9 oktober**: wind blijft stevig (9-19 kts gem, gust tot 25 kts) en golf blijft hoog (0,88-1,48 m), maar de richting draait geleidelijk van noordwest (ochtend, 302-314°, pal aanlandig bij Zandvoort) naar zuidwest (avond, 223-237°, side-shore bij Zandvoort/pal aanlandig bij IJmuiden). 🌊 Piervoorkeur verschuift dus binnen de dag: **IJmuiden** 's ochtends (NW-band), **Wijk aan Zee** vanaf ~14:00-23:00 (ZW-band, 223-237°, Noordpier breekt de golfslag).
- **Zaterdag 10 oktober**: wind blijft stevig tot stormachtig — 18-23 kts gem, **gust pieken tot 33 kts** rond 05:00 — richting overwegend west (217-290°), grotendeels **pal aanlandig bij Zandvoort** (grensgeval door de hoge windkracht), bij IJmuiden dankzij de pierzone-hoek vaker **licht aanlandig/Goed(a)**. Golf 0,86-0,93 m. Dit voelt eerder als een pittige, potentieel te ruige dag dan een comfortabele sessie — met name de gustpieken 's ochtends zijn extreem.

**Beste dag: donderdag 8 oktober**, met name het venster **05:00-23:00 bij IJmuiden** — vrijwel de hele dag Optimaal dankzij de pierzone-hoek, met golf en wind die ruim boven de Optimaal-drempel zitten. Kans: **gemiddeld tot hoog** — dit is dezelfde dag die ook in de briefing van 1 oktober al als beste dag naar voren kwam, met vergelijkbare cijfers (toen nog bij Zandvoort "Optimaal" ingeschat, nu bij nadere analyse vooral bij IJmuiden dankzij de pierzone-hoek) — die consistentie over twee opeenvolgende daglijkse runs vergroot het vertrouwen. **Vrijdag 9 en zaterdag 10 oktober zijn stevige tot stormachtige alternatieven**, met wisselende piervoorkeur en (zaterdag) mogelijk te ruige gustpieken.
⚠️ Onzeker op 4+ dagen — check dichter bij de tijd opnieuw, met name de exacte timing en windkracht rond donderdag 8 oktober.

---
_Bronnen: Windfinder (GFS) · windwaarnemingen.nl (KNMI, IJmuiden) · Soarcast — deze run niet bereikbaar (JS-app, geen vindbaar/bereikbaar API-adres)_
