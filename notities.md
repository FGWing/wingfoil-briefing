# 📓 Notities & logboek — wingfoil-briefing

Dit bestand is bedoeld om bij te houden waar de briefing goed zat en waar niet,
zodat `instructies.md` gericht bijgesteld kan worden. Voeg per sessie een
regel toe. Hoe concreter, hoe beter (welke drempel voelde verkeerd, niet
alleen "klopte niet").

## Hoe te gebruiken
1. Na een sessie op het water: voeg hieronder een nieuwe regel toe onder
   "Log".
2. Zodra een patroon zichtbaar wordt (bv. "golfperiode-drempel van 5s voelt
   vaak te streng aan"), zet dat om in een concrete aanpassing van
   `instructies.md` en noteer de wijziging onder "Doorgevoerde aanpassingen".

---

## Log

| Datum | Briefing zei | Werkelijkheid op het water | Vermoedelijke oorzaak | Actie nodig? |
|18-08-2026|Goed (grensgeval met optimaal)|Optimaal|Golfhoogte en tijd tussen golven was voldoende|Ja: Golfhoogte drempel omlaag naar 1m en tijd naar 4,5s|
| | | | | |
| | | | | |

---

## Doorgevoerde aanpassingen aan instructies.md

| Datum | Wijziging | Reden |
|---|---|---|
| _voorbeeld_ | — | — |
| | | |

---

## Technische notities (bronentoegang)
- **21-08-2026 (avondrun):** deze sessie had geen werkende browser-/screenshot-tool
  (geen get_page_text/computer-use beschikbaar, alleen tekst-URL-fetch). Bevindingen
  om toekomstige runs tijd te besparen:
  - **windwaarnemingen.nl**: de vsp-tabel wordt geladen via
    `GET https://www.windwaarnemingen.nl/database/vsp_mrg_wstats.php?st=<Station>2`
    (station bv. "IJmuiden", suffix "2" geeft een langer venster: ±64 uur vooruit
    vanaf modelrun-start, in de praktijk tot ~57u vooruit voordat waardes null
    worden). Rijen: `[idx, "YYYYMMDD", "HHMM", richting(graden), kompas, wind(m/s),
    gust(m/s), temp(C)]`, lokale tijd (CEST). Vereist geen speciale headers.
    Suffix "1" geeft alleen de huidige dag (met extra observatie-kolommen erbij,
    zie ook vsp_vdg_wstats.php voor de Realitycheck-ochtenddata).
  - **Soarcast**: de site is een JS-SPA; de onderliggende data komt van
    `GET https://www.soarcast.nl/sc/scapi.php?table=mv_forecast_location_markers`
    (vereist een gewone browser-User-Agent header, anders lege response) — geeft
    ALLE locaties/uren in één keer terug (groot bestand, ~2MB), filter op
    `location_id==133` voor IJmond (KNMI). Velden: `etime` (unix UTC),
    `windsnelheid`/`windstoot` (m/s), `windrichting` (graden). Dekking: vanaf
    enkele dagen terug tot ~57u vooruit vanaf ophaalmoment (Harmonie-modelhorizon).
    Voor locatie-metadata: `mv_measurement_location_markers&has_harmonie=true`.
  - **Windfinder**: `/forecast/<spot>` en `/weatherforecast/<spot>` (superforecast)
    zijn server-side gerenderd maar tonen ALTIJD alleen een rollend venster van
    ~2 dagen vanaf het moment van ophalen (query-params als `?day=`/`?date=`
    worden genegeerd) — er is dus geen manier om via een simpele GET-request bij
    dag 3+ te komen. De superforecast-pagina bevat wel een verborgen JSON-blob in
    een `props="..."`-attribuut (zoek op `fcSectionData`, HTML-entity-decoden)
    met VOLLEDIGE uurlijkse data (wind, golf, getij) voor de ~2 dagen die wél
    getoond worden — rijker dan de zichtbare 3-uurs tabel, dus bij het ophalen
    altijd deze blob proberen te parsen i.p.v. alleen de tabel. Voor dag 3+
    (nodig bij de avondbriefing) en de dag 4-9 outlook is dit dus NIET op te
    lossen zonder een browser die de dag-tabs client-side aanklikt; een
    headless Chromium (Playwright) in deze sessie kreeg een `ERR_CONNECTION_RESET`
    specifiek op windfinder.com (waarschijnlijk bot-detectie op TLS/JA3-niveau),
    terwijl gewone `curl`-requests naar dezelfde URL's altijd gewoon 200 OK gaven.
    De officiële `api.windfinder.com` vereist een `WF-AUTH`-token (401 zonder).
  - **Gevolg deze run:** dag 3 (maandag) van de 72u-sectie en de volledige dag
    4-9 outlook konden niet volledig gevuld worden. Actie voor volgende sessies:
    als er weer geen browser-tool beschikbaar is, dit patroon direct toepassen
    i.p.v. opnieuw te reverse-engineeren; als er wél een browser-tool is,
    gewoon de dag-tabs aanklikken zoals instructies.md voorschrijft.

## Open vragen / ideeën voor later
- [ ] Screenshot/grafiek van Windwaarnemingen of Soarcast meesturen naar Slack
      — voorlopig geparkeerd; alternatief: routine genereert zelf een
      grafiek (bv. met Python/matplotlib) op basis van de opgehaalde cijfers,
      met de eigen drempelwaarden als lijnen erin, en upload die naar Slack.
- [ ] Getij-informatie (eb/vloed) explicieter meenemen bij de pier-keuze
- [ ] Checken of de golfperiode-drempel (5s) en golfhoogte-drempel (1,1m)
      na een paar weken observatie nog kloppen
- [ ] Overwegen of een vierde categorie "Uitstekend" nuttig is voor de
      allerbeste omstandigheden (bv. wind >20kts + golf >1,3m + optimale hoek)
