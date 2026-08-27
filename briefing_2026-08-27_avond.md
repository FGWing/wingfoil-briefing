# 🌊 Wingfoil-briefing Zandvoort–Wijk aan Zee
_27-08-2026 · Avondbriefing_

---

## ⚡ Snel overzicht
- **Vrijdag:** Goed (grensgeval met Optimaal, grote modeldivergentie) (20:00-23:00)
- **Zaterdag:** Goed(a) (voorlopig — golfdata niet beschikbaar) (01:00-04:00)
- **Zondag:** Goed (voorlopig — data alleen t/m 08:00 beschikbaar) (01:00-02:00)
- **Beste dag in de 7 dagen erna:** kon deze run niet worden bepaald — zie toelichting bij de outlook hieronder

---

## 📅 Komende 72 uur

### Vrijdag — Goed (grensgeval met Optimaal)
- Beste venster: **20:00-23:00** — wind 19-22 kts, gust 27-28 kts, richting 220-227° (ZW, side-shore)
- Golven: 1,1-1,4m / 5-6s (oplopend, ruim boven de Optimaal-drempel bij 23:00)
- 🌊 Piervoorkeur: golf ≥0,8m + richting valt voor **IJmuiden** (pierzone-hoek) binnen pal aanlandig (210-270°) → daar geen pierbescherming tegen deze ZW-deining (Slecht: grote branding, pal aanlandig, buiten Zuidpier-bereik). Voor **Wijk aan Zee** is dezelfde richting licht aanlandig/side-shore → Noordpier breekt de ZW-golfslag, dus **Wijk aan Zee rustiger**. Extra gunstig: rond 23:00 is het eb (dalend tij, 0,7m), wat de shorebreak overal verzacht.
- Bronnen: Windfinder Optimaal-niveau (hoofdbron, incl. golfdata) · Soarcast niet beschikbaar (bekende SPA-beperking, zie voetnoot) · windwaarnemingen.nl **wijkt sterk af** in windsnelheid — toont voor hetzelfde venster beduidend zwakkere wind (bv. 23:00: 10,6 kts gem/18,2 kts gust vs Windfinder 22/28 kts); richting komt wel goed overeen (~215-227° ZW). Dit is een aanzienlijke GFS (Windfinder) vs. KNMI Harmonie (windwaarnemingen.nl)-divergentie, expliciet vermeld i.p.v. gemiddeld — reden om dit venster dicht bij de tijd opnieuw te checken.
- Toelichting: de dag begint zwak/wisselvallig (ochtend/middag 7-14kt, regen), maar bouwt vanaf 17:00 duidelijk op naar 19-22kt/27-28kt (Windfinder) met golf die oploopt van 1,0m naar 1,4m — qua wind, richting én golf op Optimaal-niveau volgens Windfinder. Het KNMI-model (windwaarnemingen.nl) laat dezelfde avondopbouw zien maar met veel lagere absolute waarden (rond 9-13kt/14-18kt) — bij dat scenario zou het venster eerder Goed(b)/Matig zijn. Ga voorzichtig uit van het gematigde scenario en check dicht bij de tijd opnieuw welk model gelijk krijgt.

### Zaterdag — Goed(a) (voorlopig)
- Beste venster: **01:00-04:00** — wind 11-15 kts, gust 17-21 kts, richting 231-249° (ZW/WZW, licht aanlandig)
- Golven: **niet beschikbaar deze run** (zie toelichting)
- Bronnen: Windfinder **niet beschikbaar deze run** (dag-3-tab kon niet worden opgehaald, zie voetnoot) · Soarcast niet beschikbaar · windwaarnemingen.nl (enige bron deze dag) — wind 8-15kt/gust 12-21kt, richting draait gedurende de dag van ZW/WZW (ochtend) naar zuid/ZZW/ZZO (middag-avond)
- Toelichting: het beste venster ligt vroeg (01:00-04:00, piek om 02:00: 15,1kt gem/20,7kt gust, 231° ZW, licht aanlandig) — wind/richting alleen zouden dit Goed(a) maken, maar zonder golfdata (Windfinder dag-3 en Superforecast waren deze run niet bereikbaar, Soarcast eveneens niet) is dit niet volledig te bevestigen. De rest van de dag (vanaf ~09:00) is overwegend zwak (6-10kt gem, gust 10-17kt) en draait naar zuid — grotendeels Matig tot Slecht.

### Zondag — Goed (voorlopig, onvolledige data)
- Beste venster: **01:00-02:00** — wind 14-14,3 kts, gust 22-22,8 kts, richting 212-218° (ZZW/ZW, side-shore)
- Golven: **niet beschikbaar deze run**
- Bronnen: Windfinder niet beschikbaar deze run · Soarcast niet beschikbaar · windwaarnemingen.nl dekt alleen **00:00-08:00** (daarna geen forecast-data opgehaald kunnen worden deze run)
- Toelichting: in het beschikbare venster (00:00-08:00) is 01:00 het sterkste punt (14,3kt gem/22,8kt gust, side-shore) — wind/richting alleen zouden Optimaal-niveau kunnen zijn, maar zonder golfdata niet te bevestigen; classificatie voorzichtig op Goed gehouden. **Voor de rest van zondag (na 08:00) is geen data beschikbaar deze run** — dit is het venster met de grootste onzekerheid van de drie dagen. Check dit dicht bij de tijd volledig opnieuw.

---

## 🔭 Kans op mooie sessies daarna (dag 4-9)
⚠️ **Kon deze run niet worden opgehaald.** De Windfinder Superforecast-pagina (enige bron voor dag 4-9) laadt de meerdaagse tabel deze run client-side na een tab-klik die met de huidige tools niet te simuleren was — herhaalde pogingen (verschillende prompts/URL-varianten) leverden telkens alleen de al bekende dag (donderdag) op, niet de dagen erna. Dit is een vergelijkbare structurele beperking als de al langer bekende Soarcast-SPA-blokkade (zie voetnoot). Advies: outlook dag 4-9 (maandag 31 augustus t/m zaterdag 5 september) bij de eerstvolgende run opnieuw proberen op te halen, of handmatig checken op windfinder.com/weatherforecast/zandvoort_south_beach.

---
_Bronnen: Windfinder (GFS) · Soarcast (KNMI Harmonie) · windwaarnemingen.nl (KNMI, IJmuiden)_
_Let op — bronbeperkingen deze run: Soarcast kon niet worden opgehaald (client-side React SPA zonder vindbaar achterliggend data-endpoint; de CDN-host waarop de databundel staat is bovendien niet bereikbaar vanuit deze sessie) — dezelfde structurele beperking als voorgaande briefings. windwaarnemingen.nl kon wél volledig worden geraadpleegd via de onderliggende JSON-endpoints (database/vsp_vdg_wstats.php en vsp_mrg_wstats.php, station-parameter st=IJmuiden1/IJmuiden2), inclusief het volledige 48-uurs voorspellingsvenster (vrijdag + zaterdag volledig, zondag t/m 08:00). Windfinder leverde deze run alléén donderdag+vrijdag op (het standaard 2-dagenvenster van de forecast-pagina); noch een 3e dag via de forecast-pagina, noch de meerdaagse Superforecast-tabel kon worden opgehaald, omdat die content pas na een client-side tab-klik laadt die niet gesimuleerd kon worden met de beschikbare tools (geen browserbesturing beschikbaar deze sessie, alleen tekst-fetching). Hierdoor ontbreekt golfdata (hoogte/periode) voor zaterdag, zondag en de volledige dag 4-9-outlook — classificaties voor die periodes zijn dan ook voorlopig/gedeeltelijk, gebaseerd op wind+richting alleen waar vermeld._
