# 🌊 Wingfoil-briefing Zandvoort–Wijk aan Zee
_11-11-2026 · Ochtendbriefing_

⚠️ **Technische kanttekening:** Windfinder opgehaald via directe HTTP-requests + decodering van de embedded Astro-JSON (`FcTableWindpreviewContainer` voor 10-daagse wind, `ForecastDataInit` voor wind+golf+getij gecombineerd) op zowel de forecast- als de weatherforecast-pagina, plus de zichtbare HTML-tabel (incl. golfrichting via de `rotate()`-transform van de richtingspijlen) voor woensdag/donderdag. Soarcast via de onderliggende `plotPerLocAndUnitReact.php`-JSON-endpoints (wind in kts, richting in graden, alleen daglichturen). windwaarnemingen.nl via de `vsp_vdg_wstats.php` (vandaag, 10-minuten-actuals + eigen vsp) en `vsp_mrg_wstats.php` (morgen+overmorgen, hourly vsp)-endpoints, station IJmuiden. Ruwe windsnelheden van Windfinder/windwaarnemingen in m/s, omgerekend naar kts (×1,94384); Soarcast levert al kts.
**Data-gat dag 4-9:** Windfinder's gratis preview geeft golfdata maar voor een deel van de dagen in dit venster (zondag 15, dinsdag 17, donderdag 19 nov volledig; zaterdag 14, maandag 16, woensdag 18 nov **geen golfdata** beschikbaar — alleen wind). Dit expliciet vermeld bij de betreffende dagen.

**Netto beeld:** **Woensdag (vandaag)** is **Matig** — alle drie bronnen zien een rustige, dalende winddag (GFS 5-10kts, Harmonie-bronnen 7-12kts), met een zeer kleine golf (0,2m) de hele dag; de richting is veilig aflandig/side-shore (ONO/NO). Realitycheck: de actuele waarneming bij IJmuiden loopt al enkele uren duidelijk **voor** op alle drie de voorspellingen (+4 à 5kts gemiddeld, +3 à 4kts gust) — zie onder. **Donderdag is opnieuw het grote nieuws**: alle drie bronnen bevestigen nu nog sterker dan gisteren een forse NNW-winddag vanaf ±10:00 (GFS 17,6-22,5kts, Soarcast 17,6-23,8kts, windwaarnemingen 14,8-21,8kts, allen gust tot 25-34kts) met golf die al vanaf 10:00 over de 1,1m-drempel komt en oploopt tot 2,0m — **ruim Optimaal**, en dit keer start het venster zelfs al vanaf 10:00 i.p.v. 13:00 in eerdere runs. **Vrijdag 13 nov is een bijzonder geval**: enorme golf (2,03-2,09m, periode 8,9-9,8s) en stevige wind (tot 21,1kts), maar de richting (NNW/NW, 317-344°) is voor **Zandvoort/Wijk aan Zee licht- tot bijna-pal-aanlandig** — bij zo'n grote golf een veiligheidsrisico (zware aanlandige branding). Bij **IJmuiden** (pierzone-hoek 150°/330°) is diezelfde richting echter nagenoeg **side-shore** (evenwijdig aan de havenmond) — daar is het dus een schone **Optimaal**-dag. Dit is een directe toepassing van het pierzone-hoekverschil uit de instructies en verandert het advies volledig: **ga voor vrijdag naar IJmuiden, niet naar het open strand**.

---

## ⚡ Snel overzicht
- **Woensdag:** **Matig** (dalende wind 5-10kts, golf 0,2m te klein de hele dag; realitycheck wijst op hogere werkelijke waarden dan voorspeld). Beste venster: **07:00-10:00**.
- **Donderdag:** **Optimaal vanaf 10:00** (alle drie bronnen eens — forse NNW-wind 15-22kts + golf die oploopt tot 2,0m). Beste venster: **10:00 tot (minstens) 22:00**.
- **Vrijdag:** **Optimaal bij IJmuiden** (richting daar side-shore dankzij de pierzone-hoek) / **risico bij Zandvoort en Wijk aan Zee** (licht-tot-pal-aanlandig bij een enorme golf van 2m+ — zware branding). Beste venster: **01:00-16:00** (IJmuiden).
- **Beste dag in de 7 dagen erna:** maandag 16 november (avond, 19:00-22:00) — enige kansrijke moment tussen een windstil weekend en een zware storm vanaf dinsdag, maar met lage zekerheid (golfdata ontbreekt, gust zeer hoog t.o.v. gemiddelde).

---

## ⏰ Realitycheck vandaag
- Laatste actuele uren (04:00-06:00, windwaarnemingen.nl/IJmuiden): **gem. 12,7-15,0 kts**, gust **16,6-18,7 kts**, richting **61-74°** (ONO).
- Was voorspeld: windwaarnemingen's eigen Harmonie-vsp zag voor diezelfde uren slechts **8,6-9,9 kts / gust 14,2-15,4 kts, 57-70°**; Windfinder/GFS zag voor dezelfde uren vergelijkbaar weinig: **9,3-9,7 kts / gust 14,3-14,6 kts, 72-77°** (Soarcast heeft voor deze vroege uren geen data — alleen daglichturen vanaf 07:00).
- Conclusie: de wind loopt **duidelijk VOOR** op zowel windwaarnemingen's eigen Harmonie-vsp (+4 à 5kts gem., +2 à 4kts gust) als op Windfinder/GFS (vergelijkbare overperformance). De richting klopt goed (ONO, veilig aflandig/side-shore voor Zandvoort). Rest-van-de-dag inschatting: **licht meer vertrouwen** in de hogere kant van de bandbreedte voor de ochtend; de voorspelde daling richting de avond (naar 5-7kts) blijft het meest waarschijnlijke scenario, al kan ook die trage afbouw iets later/hoger uitvallen dan voorspeld. De classificatie **Matig blijft staan** — zelfs de hogere, actuele cijfers (tot ~15kts gem/~19kts gust) veranderen dit niet wezenlijk omdat de golf (0,2m) de hele dag de beperkende factor is, ongeacht de wind.

---

## 📅 Komende 72 uur

### Woensdag — Matig
- Windfinder (GFS, 3-uurs): 5,4-10,2 kts gem., gust 7,8-15,6 kts, richting 45-81° (**licht aflandig/side-shore**, NO/ONO), dalend gedurende de dag. Golf constant **0,2m**, periode 4-10s (periode loopt op, maar golf blijft de hele dag te klein).
- Soarcast (KNMI-Harmonie, IJmond, daglicht 07:00-17:00): 8,5-12,4 kts gem., gust 12,4-16,6 kts, richting 50-68° — iets hoger dan GFS, zelfde richting.
- windwaarnemingen.nl (KNMI-Harmonie, vsp, hourly): 4,1-9,9 kts gem. (dalend naar de avond), gust 8,2-15,6 kts, richting 47-85° (ONO/NO) — grotendeels vergelijkbaar met GFS/Soarcast, en structureel lager dan wat vanochtend al daadwerkelijk gemeten is (zie Realitycheck).
- Netto: alle drie bronnen zien een rustige, dalende winddag met een verwaarloosbare golf (0,2m, ruim onder de 1,1m-drempel) — dat is hier de beperkende factor, niet de wind. Richting is de hele dag veilig (licht aflandig tot side-shore). De actuele waarneming loopt voor op alle drie de voorspellingen (zie Realitycheck), maar dat verandert de **Matig**-classificatie niet, omdat de golf sowieso te klein blijft voor meer.
- Pier-logica: niet van toepassing — richting aflandig/side-shore, niet aanlandig.
- Getij: laagwater 00:24 (0,4m), hoogwater 04:39 (2,0m), laagwater 12:38 (0,4m), hoogwater 16:49 (2,1m).
- Beste venster: **07:00-10:00** — op dit moment de hoogste daguren bij alle bronnen (GFS 9,0-9,3kts/gust 13,4-14,3kts; Soarcast 9,9-12,4kts/gust 13,1-16,6kts), met de ochtend-overperformance uit de Realitycheck kan dit in de praktijk ~3-5kts hoger uitvallen. Golf blijft 0,2m — ook in dit venster niet meer dan Matig.

### Donderdag — Optimaal (vanaf ±10:00)
- Windfinder (GFS, 3-uurs): wind bouwt op van 3,5kts (01:00) naar **14,7-22,5 kts gem.** vanaf 07:00 (piek 22,5kts om 16:00), gust tot 26,7kts; richting draait van ZZO (23°) 's nachts naar **NNW (334-345°)** vanaf 04:00 — stevig en veilig side-shore. Golf groeit van 0,2m (01:00) naar **2,0m** (22:00), periode 5-9s (periode al vanaf 07:00 ≥5s).
- Soarcast (KNMI-Harmonie, IJmond, daglicht 07:00-17:00): bevestigt onafhankelijk hetzelfde beeld — **17,6-23,8 kts gem., gust 22,4-33,7 kts**, richting 320-345° (NNW/NW).
- windwaarnemingen.nl (KNMI-Harmonie, vsp, hourly): bevestigt het een **derde keer** — **14,8-21,8 kts gem. (vanaf 07:00), gust 20,0-34,2 kts**, richting 317-343° (NNW/NW). Alle drie bronnen zijn het hier nagenoeg roerend eens, met Soarcast/windwaarnemingen (beide Harmonie) iets hogere gust-pieken dan GFS.
- Netto: een stevige, veilige (side-shore/NNW) winddag die al vanaf ±10:00 ruim boven de 14kts-Optimaal-ondergrens komt (17,6-22,5kts) én de golf is dan ook al over de 1,1m-drempel (1,2m) met een prima periode (6s). Dit is **eerder en sterker dan in eerdere runs voorspeld** — daar begon het venster pas om 13:00. Golf blijft de rest van de dag groeien (tot 2,0m om 22:00).
- Pier-logica: niet van toepassing — richting side-shore (317-345°), niet aanlandig.
- Getij: laagwater 01:04 (0,4m), hoogwater 05:15 (2,0m), laagwater 13:16 (0,3m), hoogwater 17:24 (2,2m).
- Beste venster: **10:00 tot (minstens) 22:00** — wind 14,7-22,5 kts / gust 17,8-26,7 kts, richting 334-345° (NNW, side-shore, veilig). Golf 1,2-2,0m / periode 6-9s — ruim boven de Optimaal-drempel en nog groeiend aan het einde van de beschikbare data (22:00).

### Vrijdag — Optimaal bij IJmuiden / risico bij Zandvoort en Wijk aan Zee
- Windfinder (GFS, 3-uurs, enige bron met golfdata voor deze dag): wind **10,6-21,1 kts gem.** (hoogst 's nachts/ochtends, dalend naar de avond), gust 12,2-25,3kts; richting **NNW/NW, 317-344°** (vrijwel de hele dag). Golf **enorm: 1,34-2,09m**, periode uitstekend (**8,9-9,8s**) — de grootste golf van de hele 72-uursperiode.
- Soarcast (KNMI-Harmonie, daglicht 08:00-15:00): **16,0-23,2 kts gem., gust 23,6-32,5 kts**, richting 295-339° — bevestigt de wind qua gemiddelde, maar ziet duidelijk hogere gust-pieken dan GFS.
- windwaarnemingen.nl (KNMI-Harmonie, vsp, hourly): **14,6-22,9 kts gem.** (met enkele extreme gust-uitschieters tot 40-42kts rond 01:00/03:00 — mogelijk sensorruis, met voorbehoud), richting 314-338° (NNW/NW) — bevestigt wind en richting, zelfde patroon als Soarcast (hogere gust dan GFS).
- Netto — **richting is hier cruciaal en verschilt per plek**: voor **Zandvoort** (pal aanlandig 287,5°) is 317-344° **licht aanlandig tot (tegen de avond) bijna pal aanlandig** — bij een golf van 2m is dat een forse, onbeschutte aanlandige branding, een veiligheidsrisico. Voor **Wijk aan Zee** (pal aanlandig 283,8°) geldt vrijwel hetzelfde. Voor **IJmuiden** (pierzone-hoek 150°/330°!) is diezelfde 317-344° echter **nagenoeg side-shore/evenwijdig aan de havenmond** — daar gelden de Optimaal-criteria (wind 14-25kts ✓, golf>1,1m & periode≥5s ✓, side-shore ✓) zonder voorbehoud.
- **Classificatie: IJmuiden = Optimaal. Zandvoort/Wijk aan Zee = grensgeval Goed/Slecht, met een nadrukkelijke veiligheidswaarschuwing voor zware aanlandige branding bij 2m golf.**
- Pier-logica: wél van toepassing (richting 280-360°, golf ≥0,8m): volgens de tabel is bij deze richting **IJmuiden (Zuidpier)** al de rustigere/veiligere kant t.o.v. Wijk aan Zee — dat valt hier samen met het eigen pierzone-hoekeffect (dubbel voordeel voor IJmuiden). Bij vloed (hoogwater 05:48 en 17:59) is de branding overal zwaarder, ook bij IJmuiden.
- Getij: laagwater 01:36 (0,4m), hoogwater 05:48 (1,9m), laagwater 13:48 (0,3m), hoogwater 17:59 (2,1m).
- Beste venster: **01:00-16:00 bij IJmuiden** — wind 14,8-21,1 kts / gust 16,7-25,3 kts, richting 317-334° (bij IJmuiden effectief side-shore). Golf 1,34-2,09m / periode 8,9-9,8s. Vanaf ±19:00 zakt de wind onder 14kts (13,9 kts), waarmee het Optimaal-venster eindigt.

---

## 🔭 Kans op mooie sessies daarna (dag 4-9)
Windfinder (GFS, enige bron zo ver vooruit) voor **zaterdag 14 t/m donderdag 19 november**:

- **Zaterdag 14 november**: wind veel te zwak (**7,3-10,0 kts gem., gust 9,6-12,2 kts**) → **Slecht** (gust<16 én gem<14, hele dag). Richting draait sterk gedurende de dag (WNW→ZO), inclusief een pal-aanlandig moment 's ochtends, maar bij deze zwakke wind is dat niet relevant.
- **Zondag 15 november**: wind blijft laag-matig (**8,4-14,2 kts gem.**), richting 143-200° (ZZO/ZUID, veilig side-shore/licht aflandig). Golf blijft klein (0,51-1,02m) → **Matig**. Een gustige piek rond 19:00 (wind 14,2kts, gust tot **25,9kts** — bijna het dubbele) is een grensgeval richting Goed, maar de golf (0,9m) blijft net onder de 1,1m-drempel.
- **Maandag 16 november**: wind trekt aan gedurende de dag (**10,2-19,1 kts gem.**) met forse gustiness (gust **14,6-34,4 kts**, vooral 's avonds). Richting is overwegend side-shore/licht aflandig (143-227°, veilig), met twee vroege-ochtenduren (04:00/07:00, 257-262°) die licht aanlandig zijn — op dat moment is de wind nog zwak (15-18kts) dus minder risicovol. **Golfdata ontbreekt bij Windfinder voor deze dag** (data-gat) — zonder golfhoogte is een harde classificatie niet te geven, maar de avond (19:00-22:00: wind 15,3-19,1kts, veilige richting 160-203°) is cijfermatig het meest kansrijke moment van deze hele outlook-periode. De sterke gustiness (gust bijna 2× het gemiddelde) vraagt wel om voorzichtigheid.
- **Dinsdag 17 november**: wind schiet door naar stormkracht (**20,3-31,9 kts gem., gust 37,3-47,3 kts** — Bft 9-10 in de pieken). Richting 206-243° (ZZW/WZW) — bij deze windkracht uit WZW geldt bovendien het officiële pierensluiting-signaal van de Reddingsbrigade IJmuiden. Golf 1,52-1,81m, periode ~7,6-7,9s. Puur een weerswaarschuwing, geen wingfoil-kans.
- **Woensdag 18 november**: wind blijft stormachtig (**24,2-29,1 kts gem., gust 33,9-40,8 kts**), richting WSW/W (238-257°) — valt binnen het Reddingsbrigade-sluitingscriterium. **Golfdata ontbreekt bij Windfinder voor deze dag**, maar bij deze windsnelheden is dat niet bepalend — wederom een stormwaarschuwing.
- **Donderdag 19 november**: wind blijft zeer fors (**20,3-25,8 kts gem., gust 29,1-35,4 kts**), richting ZW/WZW (218-254°) — ook hier valt een deel van de dag binnen het Reddingsbrigade-sluitingscriterium. Golf 1,61-1,78m, periode ~7,2-7,9s. Nog steeds te extreem voor een normale sessie.

**Beste dag: maandag 16 november (avond, 19:00-22:00)** is het enige echte lichtpunt tussen een te zwak weekend en een zware storm vanaf dinsdag — wind 15-19kts bij een veilige richting, maar met twee duidelijke voorbehouden: de golfdata ontbreekt voor deze dag bij Windfinder, en de gustiness is zeer hoog relatief tot het gemiddelde. Kans: **gemiddeld** (cijfermatig kansrijk, maar met lagere zekerheid door het golf-datagat). ⚠️ Onzeker op 4+ dagen — check dichter bij de tijd opnieuw. Let in latere runs vooral op: (1) of de golfhoogte voor maandag 16 november alsnog beschikbaar komt en of die boven de 1,1m-drempel uitkomt, (2) of de zware storm van dinsdag 17 t/m donderdag 19 november in latere runs afzwakt, en (3) of vrijdag 13 november (nu nog in het 72-uursvenster) qua richting bij Zandvoort/Wijk aan Zee alsnog meer side-shore blijft i.p.v. verder aanlandig draait.

---
_Bronnen: Windfinder (GFS) · Soarcast (KNMI Harmonie, IJmond) · windwaarnemingen.nl (KNMI, IJmuiden)_
