# 🌊 Wingfoil-briefing Zandvoort–Wijk aan Zee
_20-11-2026 · Avondbriefing_

⚠️ **Eenheden-correctie windwaarnemingen.nl:** de ruwe waarden uit `vsp_mrg_wstats.php` / `vsp_vdg_wstats.php` blijken **m/s** te zijn, niet knopen (eerdere briefings namen ze als kts over). Omgerekend (×1,94) sluiten ze vrijwel naadloos aan op Soarcast (bv. zaterdag 12:00: 5,8 m/s = 11,3 kts gem./8,1 m/s = 15,7 kts gust vs. Soarcast 12,6/16,3 kts). De "structurele modelverdeeldheid" van de afgelopen dagen was daarmee grotendeels een eenhedenfout. Alle windwaarnemingen-cijfers hieronder zijn omgerekend naar kts.

Technisch: alle bronnen via curl (Windfinder embedded JSON — `ws`/`wg` in m/s, omgerekend; Soarcast JSON-endpoint, tijden in UTC → +1u lokaal; windwaarnemingen JSON-endpoints). Let op daglicht: zon onder ±16:40, vensters na ±16:30 zijn niet bruikbaar.

## ⚡ Snel overzicht
- **Zaterdag:** Slecht–Matig grensgeval (±12:00-16:00) — 9-12,5 kts, gust 13-16 kts, pal aanlandig WNW; Windfinder net Slecht, Soarcast/windwaarnemingen net Matig.
- **Zondag:** Matig (±11:00-15:00) — Windfinder 10-12 kts/gust 16-18 kts licht aflandig ONO; Soarcast en windwaarnemingen zwakker.
- **Maandag:** Slecht — overdag 4-7 kts; wind komt pas na donker op.
- **Beste dag in de 7 dagen erna:** dinsdag 24 november

---

## 📅 Komende 72 uur

### zaterdag — Slecht/Matig (grensgeval)
- Beste venster: **±12:00-16:00** — wind 9-12,5 kts, gust 13-16 kts, richting 279-290° (Zandvoort/Wijk aan Zee: pal aanlandig; IJmuiden-pierzone: licht aanlandig)
- Golven: 0,86-0,89m / 5,4-6,1s
- 🌊 Piervoorkeur: richting zit in/aan de rand van de neutrale zone (250-280°) → geen duidelijk piervoordeel; vanaf ±15:00 (richting >280°) licht voordeel **IJmuiden (Zuidpier)**. Hoogwater ±12:57 → shorebreak midden in het venster op zijn zwaarst; laagwater 08:54 / 20:52.
- Bronnen: Windfinder 8-12,5 kts / gust 11-14 kts (→ Slecht, gust <16) · Soarcast 10,6-12,6 kts / gust 15,5-16,3 kts · windwaarnemingen 9,5-11,3 kts / gust 15-16 kts → **eens over de richting, Soarcast + windwaarnemingen gusts nét op de 16 kts-grens**. Ochtend (08:00-10:00) vergelijkbaar maar met hoger NW-getal bij Windfinder (10,8 kts om 08:00). t.o.v. vanochtend afgezwakt (Windfinder-piek 14 → 12,5 kts) — het Goed(a)-grensgeval bij IJmuiden is vervallen.

### zondag — Matig
- Beste venster: **±11:00-15:00** — wind 9-12 kts, gust 16-18 kts, richting 65-75° (licht aflandig, schoon water)
- Golven: 0,57m / 7,2-7,6s
- Bronnen: Windfinder 9-12 kts / gust 16-18 kts · Soarcast 5-7 kts / gust 9-12 kts (piek eerder, 10:00-12:00 ±9 kts) · windwaarnemingen 5-7 kts / gust 10-11 kts → **wijkt af**: alleen Windfinder haalt de gust-drempel; de twee Harmonie-bronnen zien een Slecht-middag. Na ±17:00 trekt het bij alle bronnen aan (10-11 kts, gust 16-19 kts), maar dan is het donker. Getij: laagwater 09:53, hoogwater 13:43.

### maandag — Slecht
- Overdag geen bruikbaar venster: Windfinder 4,5-7 kts, gust 5-10 kts, richting draaiend 137-172° (zuidoost → zuid). Golven 0,47-0,54m / 6,2-7,4s.
- Wind bouwt pas vanaf ±19:00 op (9-12 kts, gust 14-19 kts, ZO) — aanloop naar dinsdag, maar na donker.
- Bronnen: Windfinder (3-uurs) · Soarcast nog geen data · windwaarnemingen (tot 07:00) 2-7 kts → eens. Getij: laagwater 10:42, hoogwater 14:27.

---

## 🔭 Kans op mooie sessies daarna (dag 4-9)
Windfinder (GFS, 3-uurs), 24 t/m 29 november:
- **Dinsdag 24 nov:** sterkste dag — 14,6-17,5 kts, gust 24-28 kts, 131-141° (pal tot licht aflandig) 07:00-16:00. Golf maar 0,41-0,47m (5,7-6,7s). Goed (grensgeval Goed/Matig: wind ideaal, golf vlak). ⚠️ Gusty en aflandig = drift van de kust af; regen voorspeld. Ongewijzigd t.o.v. vanochtend.
- **Woensdag 25 nov:** 11,6-12,4 kts, gust 18-22 kts in de ochtend, ZO (aflandig), golf 0,45m / ±4s → Matig.
- **Donderdag 26 nov:** windstil (1-6 kts) → Slecht.
- **Vrijdag 27 nov:** 12,5-13,5 kts, gust 21-24 kts overdag, 156° (side-shore), golf 0,5m / 4,7s → Matig (grensgeval Goed).
- **Zaterdag 28 nov:** 13,2-13,4 kts, gust 21-23 kts 07:00-13:00, 162-168° (side-shore), golf 0,62-0,65m / ±5s → Matig (grensgeval Goed). **Fors afgezwakt** t.o.v. vanochtend: de verwachte draai naar NW met golf ±1,05m is uit het model verdwenen.
- **Zondag 29 nov:** 8-10 kts overdag, ZO-aflandig, golf 0,6m → Matig/Slecht. Het Goed(b)-venster van vanochtend (golf 1,1-1,2m) is vervallen.

Kans: **laag-gemiddeld** — dinsdag 24 november is de enige dag met wind ruim boven 14 kts; golf blijft de hele periode onder de drempel.
⚠️ Onzeker op 4+ dagen — check dichter bij de tijd opnieuw.

---
_Bronnen: Windfinder (GFS) · Soarcast (KNMI Harmonie, IJmond) · windwaarnemingen.nl (KNMI, IJmuiden)_
