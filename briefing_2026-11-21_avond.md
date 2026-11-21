# 🌊 Wingfoil-briefing Zandvoort–Wijk aan Zee
_21-11-2026 · Avondbriefing_

⚠️ **Correctie eenheden windwaarnemingen.nl:** de ruwe data van windwaarnemingen.nl (`vsp_vdg_wstats.php` / `vsp_mrg_wstats.php`) staat in **m/s**, niet in knopen. De site rekent zelf om met ×3,6/1,852 (≈×1,94), te zien in `js/draw_wnmvsp.min.js`. De vorige briefings namen deze waarden over als kts en zaten daardoor een factor ~1,94 te laag. Dat geldt ook voor de realitycheck van vanochtend: de "3,7-9,5 kts" was in werkelijkheid ≈7-18 kts, zodat Windfinder toen eerder **conform** liep dan "fors achter". Vanaf deze briefing zijn alle windwaarnemingen-cijfers omgerekend naar kts. Windfinder (veld `ws` in m/s, ook omgerekend) en Soarcast (`windUnits=kts`) waren wel correct.

Data opgehaald om ±22:15 via curl: Windfinder Superforecast (ICON-EU, uurlijks, zondag+maandag) en GFS (3-uurs, dinsdag + outlook), Soarcast IJmond (Harmonie, 08:00-17:00) en windwaarnemingen.nl IJmuiden (vsp zondag t/m dinsdag 07:00).

**Netto beeld:** een rustige zondag met ONO-wind die net te zwak blijft (Matig, grensgeval Slecht), een windstille maandag (Slecht) en een aflandige dinsdag die oploopt maar onder de 14 kts blijft (Matig). De outlook is fors **afgezwakt** t.o.v. vanochtend: het "winderige blok" is grotendeels verdwenen, alleen **woensdag 25 november** haalt nog rond de 14-16 kts (pal aflandig, vlak water).

---

## ⚡ Snel overzicht
- **Zondag:** Matig, grensgeval Slecht (11:00-14:00)
- **Maandag:** Slecht
- **Dinsdag:** Matig (13:00-19:00, pal aflandig)
- **Beste dag in de 7 dagen erna:** woensdag 25 november

---

## 📅 Komende 72 uur

### Zondag — Matig (grensgeval Slecht)
- Beste venster: **11:00-14:00**, wind 10,5-12,5 kts (WF) / 8,9-9,4 kts (Soarcast) / 7-8 kts (ww), gust 17-19 kts (WF) / 13-14 kts (Soarcast, ww), richting 75-80° (licht aflandig, ONO)
- Golven: 0,56m / 7s
- Bronnen: Windfinder max 12,5/19 kts · Soarcast max 9,4/14,1 kts · windwaarnemingen max 7,6/13,4 kts → **wijkt af**: Soarcast en windwaarnemingen zijn het eens over een zwakkere lijn, en daarmee zou het Slecht zijn (gust <16 én gem <14)
- Getij: LW 09:53, HW 13:43

### Maandag — Slecht
- Geen bruikbaar venster: wind 2-7 kts de hele dag, en richting draait van ONO via Z (side-shore) naar NW
- Golven: 0,5m / 7s
- Bronnen: Windfinder max 6,8 kts · Soarcast max 8,5/12,6 kts (17:00) · windwaarnemingen max 8 kts → **eens**

### Dinsdag — Matig
- Beste venster: **13:00-19:00**, wind 12-13 kts, gust 17-22 kts, richting 119-126° (pal aflandig, OZO)
- Golven: 0,36-0,38m / 5-5,6s
- ⚠️ Pal aflandig: schoon water, maar drift van de kust af, dus alleen met backup
- Bronnen: Windfinder (GFS) 10-13 kts/gust 16-22 · Soarcast n.v.t. (reikt niet tot dinsdag) · windwaarnemingen alleen t/m 07:00 (4-6 kts, OZO/ZO) → alleen Windfinder voor het venster

_Pier-logica: niet van toepassing op alle drie dagen (wind aflandig of side-shore, golf <0,8m)._

---

## 🔭 Kans op mooie sessies daarna (dag 4-9)
Windfinder GFS, dinsdag 24 t/m zondag 29 november. Vergeleken met vanochtend is het beeld **flink afgezwakt**: dinsdag zakte van 14-16 naar 10-13 kts, zondag 29 van 17-19 naar 9-10 kts.
- **Woensdag 25 november:** de beste dag. 13,5-15,7 kts, gust 23-25 kts, pal aflandig (89-107°), golf 0,33-0,40m / ~3s. **Grensgeval Goed**: de wind haalt 14+ kts vooral in de middag, maar het water is vlak en de richting pal aflandig.
- **Donderdag 26:** 's ochtends nog 13 kts (gust 21), daarna rond 10 kts: Matig
- **Vrijdag 27 en zaterdag 28:** 9-12 kts, gusty (tot 19-22 kts), ONO/O: Matig
- **Zondag 29:** 9-10,5 kts, maar golf loopt op naar 0,8m / 5,4-5,7s (ZZW-deining): Matig, grensgeval Slecht

Kans: **laag-tot-gemiddeld**, het kansrijkst op woensdagmiddag 25 november.
⚠️ Onzeker op 4+ dagen, check dichter bij de tijd opnieuw.

---
_Bronnen: Windfinder (GFS / Superforecast ICON-EU) · Soarcast (KNMI Harmonie, IJmond) · windwaarnemingen.nl (KNMI, IJmuiden, omgerekend m/s→kts)_
