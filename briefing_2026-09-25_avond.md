# 🌊 Wingfoil-briefing Zandvoort–Wijk aan Zee
_25-09-2026 · Avondbriefing_

⚠️ **Technische beperking deze run:** geen browser/JS-rendering beschikbaar, dus Soarcast (volledig client-side app, geen publieke data-API gevonden na gericht zoeken) kon niet geraadpleegd worden, en de Windfinder-pagina's (zowel de 72u-forecast als de Superforecast) tonen server-side maar 2 dagen (vrijdag+zaterdag) resp. 1 dag — dagtabs voor latere dagen vereisen JavaScript. Wél gelukt: windwaarnemingen.nl kon dit keer via zijn onderliggende data-endpoint (KNMI-vsp) rechtstreeks opgehaald worden, mét een voorspellingshorizon tot zaterdag t/m maandagochtend 08:00 — dat vult zondag en een deel van maandag in waar Windfinder niets toont. Maandagmiddag/-avond en de lange-termijn outlook (dag 4-9) ontbreken deze run volledig.

---

## ⚡ Snel overzicht
- **Zaterdag:** Slecht-tot-Matig (grensgeval, modellen wijken sterk af op gust, mogelijk 13:00-18:00)
- **Zondag:** Slecht (hele dag zwak, geen bruikbaar venster)
- **Maandag:** Matig (onvolledige data — alleen 00:00-08:00 bekend, kort venster rond 03:00)
- **Beste dag in de 7 dagen erna:** niet beschikbaar deze run (zie toelichting hieronder)

---

## 📅 Komende 72 uur

### Zaterdag — Slecht-tot-Matig (grensgeval, modellen wijken af op gust)
- **Beste venster: 13:00-18:00** — Windfinder (GFS) geeft hier 8 kts gemiddeld met een opvallend lage gust van slechts 8 kts (richting 350-357°, Noord); het KNMI-vsp-model (windwaarnemingen.nl) geeft voor exact dezelfde uren een duidelijk hogere gust: 10,9-12,4 kts gemiddeld met **gust 16,1-18,3 kts** (richting eveneens 350-357°, Noord).
- Dit is een **duidelijke afwijking tussen de modellen** — puur op de gust, de gemiddelde windsnelheid en richting komen wél goed overeen (verschil <3 kt resp. <10°).
- Richting 350-357° (Noord) is bij Zandvoort (kustlijn 17,5°/197,5°) nagenoeg **side-shore**.
- Buiten dit venster (00:00-12:00 en 19:00-23:00) blijft de gust in beide bronnen onder de 16 kts terwijl het gemiddelde onder 14 kts blijft — dat is de expliciete "Slecht"-conditie (gust <16 kts ÉN gem <14 kts), ongeacht richting of golf.
- Golven (Windfinder, enige golfbron voor deze dag): 0,3-0,5 m / 4-6 s — ruim onder de 1,1 m-drempel, dus geen Goed(b)-scenario mogelijk.
- 🌊 Piervoorkeur: niet van toepassing (richting is side-shore, geen aanlandige component, en golf blijft <0,8 m).
- Getij (Windfinder): hoogwater ~04:17 (2,1 m), laagwater ~13:12 (0,4 m), hoogwater ~16:35 (2,0 m), laagwater ~20:29 (0,9 m).
- Bronnen: Windfinder en windwaarnemingen.nl/KNMI-vsp **eens** over gemiddelde wind en richting, **wijken sterk af** op de gust (8 kts vs. 16-18 kts in het middagvenster) — vandaar het brede "Slecht-tot-Matig"-label i.p.v. middelen. Soarcast kon deze run niet geraadpleegd worden.

### Zondag — Slecht
- Geen bruikbaar venster: het KNMI-vsp-model (windwaarnemingen.nl, enige beschikbare bron voor deze dag) geeft de hele dag 4,3-8,4 kts gemiddeld met gust van maximaal 13,2 kts — ruim onder de 14 kts (gem) / 16 kts (gust) drempel voor "Slecht", op elk moment van de dag.
- Richting draait van ONO/NO (37-74°, nacht/vroege ochtend) via OOST/ZO (92-127°, rond het middaguur) naar ZUID/ZW (177-232°, namiddag) en terug naar ZO (131-142°, avond) — geen van deze fases is relevant omdat de wind sowieso te zwak is.
- Golven: **geen golfdata beschikbaar** — Windfinder toont deze dag niet (server-side maar 2 dagen beschikbaar deze run) en windwaarnemingen.nl meet geen golven.
- 🌊 Piervoorkeur: niet te beoordelen (golfhoogte onbekend), en de wind is sowieso te zwak om relevant te zijn.
- Getij: niet beschikbaar deze run (Windfinder, de enige getij-bron, ontbreekt voor deze dag).
- Bronnen: alleen windwaarnemingen.nl/KNMI-vsp beschikbaar voor deze dag — Windfinder en Soarcast ontbreken (technische beperking, zie boven). Geen kruisvalidatie mogelijk.

### Maandag — Matig (onvolledige data)
- **Enige beschikbare venster: rond 03:00** — windwaarnemingen.nl/KNMI-vsp (enige bron, en enkel voorspellingsdata tot 08:00 deze ochtend) geeft hier 10,1 kts gemiddeld met **gust 17,7 kts**, richting 245° (WZW). Dat gust-niveau tilt dit uur net boven de "Slecht"-drempel (gust ≥16 kts) naar **Matig** (wind blijft <15 kts, gust <19 kts).
- Richting 245° (WZW) is bij Zandvoort (aanlandig 287,5°) een **grensgeval richting licht aanlandig** (verschil 42,5°, net binnen de 30-45°-marge); bij IJmuiden (pierzone, aanlandig 240°) is dit vrijwel **pal aanlandig** (verschil 5°).
- Overige uren in het beschikbare venster (00:00-02:00, 04:00-08:00) blijven met gust 11-14,6 kts en gemiddeld 3,3-10,3 kts onder de "Slecht"-drempel.
- Golven: **geen golfdata beschikbaar** (Windfinder toont deze dag niet, windwaarnemingen.nl meet geen golven) — de pierzone-richting bij IJmuiden is dus wel aanlandig, maar of de golf ≥0,8 m is (voorwaarde voor de pier-logica) kan deze run niet vastgesteld worden.
- 🌊 Piervoorkeur: niet te beoordelen (golfhoogte onbekend), ondanks de aanlandige richting bij IJmuiden.
- **Let op: alleen 00:00-08:00 is deze run bekend** — de KNMI-vsp-voorspellingshorizon reikt niet verder. Namiddag en avond van maandag zijn volledig onbekend; Windfinder (dat verder vooruit zou kunnen kijken) toonde server-side alleen vrijdag+zaterdag. Check dit venster dus sowieso opnieuw bij de eerstvolgende briefing.
- Getij: niet beschikbaar deze run.
- Bronnen: alleen windwaarnemingen.nl/KNMI-vsp, en dat slechts voor een deel van de dag. Windfinder en Soarcast ontbreken. Geen kruisvalidatie mogelijk, en het beeld voor de rest van de dag is een blinde vlek.

---

## 🔭 Kans op mooie sessies daarna (dag 4-9)
**Niet beschikbaar deze run.** De Windfinder Superforecast-pagina (enige bron die zo ver vooruitkijkt) leverde server-side alleen de eerste dag op; de dagtabs voor dag 2 t/m 9 vereisen client-side JavaScript dat in deze sessie-omgeving niet beschikbaar was. Het KNMI-vsp-endpoint van windwaarnemingen.nl (dat deze run wél rechtstreeks bereikbaar bleek) kijkt evenmin ver genoeg vooruit (voorspellingshorizon eindigt maandagochtend). Advies: check https://www.windfinder.com/weatherforecast/zandvoort_south_beach handmatig, of hoop op herstel van de outlook in de eerstvolgende run.
⚠️ Onzeker op 4+ dagen — check sowieso dichter bij de tijd opnieuw, ook zodra deze sectie weer gevuld kan worden.

---
_Bronnen: Windfinder (GFS, alleen zaterdag bruikbaar voor dit venster) · windwaarnemingen.nl (KNMI-vsp, IJmuiden, zaterdag t/m maandag 08:00) · Soarcast — deze run niet bereikbaar (JS-app, geen publieke data-API gevonden)_
