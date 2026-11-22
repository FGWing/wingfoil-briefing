# 🌊 Wingfoil-briefing Zandvoort–Wijk aan Zee
_22-11-2026 · Avondbriefing_

⚠️ **Technische kanttekening:** alle bronnen via curl opgehaald (geen browser). Windfinder: embedded Astro-data van de forecast-pagina (GFS, 3-uurs, t/m 1 dec incl. golf/getij) en de Superforecast-pagina (uurlijks, ma 23 + di 24). **Windfinder levert ws/wg intern in m/s — omgerekend naar kts (×1,944).** Soarcast: `sc/plotPerLocAndUnitReact.php?json&jsonOnly&unit=m/s&location=133&day=...&windUnits=kts&forecastToShow=harm&duringDayOnly=true&runsToShow=lastOnly` (let op: zonder `unit=` levert het endpoint alleen richting), plus aparte richtingdataset. Soarcast dekt alleen maandag+dinsdag (08:00-17:00). windwaarnemingen.nl: `vsp_mrg_wstats.php?st=IJmuiden2` (ma 00:00 t/m wo 07:00, waarden in m/s → kts).

**Netto beeld — maandag zwak (Slecht), dinsdag bouwt een gusty ZO-wind op (Matig/Goed-grensgeval vanaf de vroege middag), woensdag de sterkste dag met 16-17kts pal aflandige OOST-wind (Goed-grensgeval). Golf blijft alle drie dagen ruim onder 0,5m.** Let op: het licht valt eind november al om ±16:35 weg, dus de sterke avondwind van dinsdag is grotendeels onbruikbaar.

---

## ⚡ Snel overzicht
- **Maandag:** Slecht
- **Dinsdag:** Matig/Goed grensgeval (13:00-16:30)
- **Woensdag:** Goed, grensgeval (09:00-16:00) — pal aflandig en zeer gusty
- **Beste dag in de 7 dagen erna:** donderdag 26 november

---

## 📅 Komende 72 uur

### Maandag — Slecht
- Beste venster: **geen bruikbaar venster** — wind 3-10 kts, gust ≤13 kts overdag, richting draait van ONO (aflandig) 's ochtends naar ZW/WZW 230-255° ('s middags, side-shore tot licht aanlandig)
- Golven: 0,45-0,53m / 6,6-7,0s
- Bronnen: Windfinder 3-7 kts (gust ≤6 overdag, 15 kts alleen vóór zonsopgang) · Soarcast 2,6-9,6 kts (gust ≤13,1) · windwaarnemingen.nl 2-8,7 kts (gust ≤12,2) → eens: overal gem <14 én gust <16
- Getij: LW ±10:42, HW ±14:27, LW ±18:43

### Dinsdag — Matig/Goed grensgeval
- Beste venster: **±13:00-16:30** (tot zonsondergang) — wind 10-17 kts, gust 17-23 kts, richting 116-136° (ZO/OZO, **pal aflandig**)
- Golven: 0,37-0,38m / 5,1-5,4s
- Bronnen: Windfinder Superforecast 10,3-12,4 kts (gust 22-27) / GFS 12-15 kts · Soarcast 13,4-16,8 kts (gust 18,5-22,9) · windwaarnemingen.nl 10,7-12,8 kts (gust 17-20) → **wijkt af**: alleen Soarcast (en GFS rond 16:00) haalt de 14kts-drempel, Superforecast en windwaarnemingen blijven er net onder. Wind loopt na zonsondergang verder op (Superforecast 14 kts / gust 29 om 20:00).
- Oordeel: tussen Matig (gem <14) en Goed (gem 14+, maar pal aflandig past niet bij Optimaal/Goed(a); golf te laag voor Goed(b)). ⚠️ Pal aflandig + gust-factor ~2× = risico op wegdrijven; alleen met backup.
- Getij: LW ±11:21, HW ±15:09

### Woensdag — Goed (grensgeval)
- Beste venster: **±09:00-16:00** — wind 16-17 kts, gust 24-29 kts, richting 81-93° (ONO/OOST, **pal aflandig**)
- Golven: 0,39-0,41m / 2,8-3,0s
- Bronnen: Windfinder (GFS) 16,1-16,9 kts (gust 24-29) · Soarcast n.v.t. (dekt geen 3e dag) · windwaarnemingen.nl t/m 07:00: 16-17 kts (gust 25-27, OOST) → eens voor de ochtend
- Oordeel: wind ruim binnen 14-25kts, maar pal aflandig (geen Optimaal/Goed(a)-richting) en korte golfperiode — Goed als grensgeval, sterkste dag van de week. ⚠️ Stevig aflandig met forse gusts — veiligheid voorop.
- Getij: LW ±11:50, HW ±15:53

_Pier-logica: alle drie dagen niet van toepassing (aflandig, golf <0,8m)._

---

## 🔭 Kans op mooie sessies daarna (dag 4-9)
Windfinder GFS, donderdag 26 nov t/m dinsdag 1 dec (woensdag 25 valt in deze avondbriefing al binnen de 72 uur):
- **Donderdag 26 november:** 11-13,6 kts, gust 17-23 kts, ONO 77-91° (pal aflandig), golf 0,25-0,3m / 3,2-4,5s → **Matig, grensgeval richting Goed** — onveranderd t.o.v. vanochtend.
- **Vrijdag 27:** 9-10 kts, gust 13-16 → Matig/Slecht.
- **Zaterdag 28:** 9-10 kts overdag, gust 14-16 (pas 's avonds 12 kts / gust 21) → Matig.
- **Zondag 29:** 10-11 kts, gust 16-19 's ochtends, ZZO 163-171° (side-shore) → Matig — **opgewaardeerd** t.o.v. vanochtend (toen vrijwel windstil).
- **Maandag 30 / dinsdag 1 december:** 6-9 kts, gust ≤13 → Slecht.

**Beste dag: donderdag 26 november** (staartje van het OOST-blok van woensdag). Kans: **laag-gemiddeld** — de echte piek valt woensdag, daarna zakt de wind weg en golf blijft de hele periode <0,7m.
⚠️ Onzeker op 4+ dagen — check dichter bij de tijd opnieuw.

---
_Bronnen: Windfinder (GFS / Superforecast) · Soarcast (KNMI Harmonie, IJmond) · windwaarnemingen.nl (KNMI, IJmuiden)_
