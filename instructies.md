# Instructies: Wingfoil-briefing Zandvoort–Wijk aan Zee

Dit document is de volledige context voor een geautomatiseerde dagelijkse
briefing. Een verse sessie heeft geen geheugen van eerdere gesprekken —
alles wat nodig is om de taak goed uit te voeren staat hieronder.

## Doel
Twee keer per dag (07:15 en 23:15) een wingfoil-conditiebriefing produceren
voor de kuststrook tussen Zandvoort en Wijk aan Zee, gebaseerd op drie
onafhankelijke windbronnen, en deze posten in Slack via het sjabloon in
`sjabloon.md`.

## Gebied en geografie
- Kustlijn Zandvoort–Wijk aan Zee loopt ~17°/197° (NNO-ZZW).
- Pal aanlandig (wind recht vanaf zee) ≈ 287° (WNW).
- Pal aflandig (wind recht vanaf land) ≈ 107° (OZO).
- Windrichting in graden = waar de wind VANDAAN komt (meteorologische conventie).

### Classificatie windrichting t.o.v. kust
- **Pal aanlandig**: binnen ~30° van 287°
- **Licht aanlandig**: 30-45° van 287° (richting land, maar niet loodrecht)
- **Pal aflandig**: binnen ~30° van 107°
- **Licht aflandig**: 30-45° van 107°
- **Side-shore**: overig, richting 17° of 197° (evenwijdig aan kust)

## Bronnen (alle drie gebruiken, niet middelen maar naast elkaar tonen)

### 1. Windfinder — https://www.windfinder.com/forecast/zandvoort_south_beach
- GFS-model, tabeldata per 1-3 uur, tot 9-10 dagen vooruit.
- De statische pagina (via simpele fetch) toont vaak maar 1 dag — gebruik een
  browser-tool (navigeren + get_page_text) om alle dagtabs (Mon t/m volgende
  9 dagen) te laden; de dagen zijn los aanklikbare tabs bovenaan de tabel.
- Kolommen: windrichting (graden), windsnelheid (kts), gusts (max kts),
  golfrichting, golfhoogte (m), golfperiode (s), getij.
- Gebruik dit als hoofdbron voor golfdata (enige bron met golfperiode/-hoogte).

### 2. Soarcast — https://www.soarcast.nl/web/kaart
- Draait op het KNMI Harmonie-model, specifiek voor NL-kustspots.
- Navigeer naar de kaart, klik het station "IJmond (KNMI)" aan
  (ligt tussen Zandvoort en Wijk aan Zee, bij de havenmond), open
  "Bekijk locatie info" -> komt uit op /web/locationinfo?location=133
- Tabs: Vandaag / Morgen / Overmorgen. Toont wind+gust (grafiek, kts) en
  windrichting (graden). GEEN golfdata (landstation meet geen golven).
- Gebruik dit als kruisvalidatie op wind/gust/richting naast Windfinder.
  Bij grote afwijking tussen beide modellen: vermeld dit expliciet in de
  briefing i.p.v. te middelen.

### 3. windwaarnemingen.nl — https://www.windwaarnemingen.nl/
- KNMI/RWS-data. Selecteer station **IJmuiden** in de dropdown.
- Toont EEN tabel met kolom "vsp" (voorspelling) per uur voor vandaag+morgen,
  gebaseerd op een KNMI-modelrun (vermeld linksboven: "Voorspelling init: ...").
- Cruciaal: voor uren die al voorbij zijn op de dag zelf, staan naast de
  voorspelling ook de gerealiseerde waarnemingen (in de kleinere "12"-tabel
  met ~10-minuten-metingen, en impliciet in de hoofdgrafiek).
- **Alleen relevant bij de OCHTENDBRIEFING** (zie sectie hieronder).

## Ochtendbriefing vs. avondbriefing

### Ochtendbriefing (07:15) — voeg de "Realitycheck vandaag"-sectie toe
1. Haal bij windwaarnemingen.nl (station IJmuiden) de laatste 2-3 al
   gerealiseerde uren van vandaag op (de vroege ochtenduren, bv. 06:00-08:00).
2. Vergelijk deze actuals met wat gisteravond voor diezelfde uren voorspeld
   was (indien te achterhalen uit een eerdere modelrun / de vsp-kolom met
   terugwerkende kracht) — zo niet, vergelijk in elk geval de actuele
   waarneming met de Windfinder/Soarcast-voorspelling van vanochtend vroeg
   voor dat tijdstip.
3. Trek een conclusie: loopt de wind "voor" (harder dan voorspeld), "achter"
   (zwakker), of "conform" verwachting?
4. Stel op basis daarvan de inschatting voor de rest van de dag (de nog
   resterende 72-uursperiode) met iets meer of minder vertrouwen bij, en
   vermeld dit expliciet.

### Avondbriefing (23:15) — geen realitycheck-sectie
Gewoon de volledige 72-uursanalyse + lange-termijn-outlook, zonder de
ochtend-specifieke vergelijking (die is 's avonds niet zinvol omdat de
komende dag nog moet beginnen).

## Beoordelingscriteria (per tijdstip toepassen)

| Oordeel | Wind gemiddeld | Golfhoogte + periode | Windrichting |
|---|---|---|---|
| **Optimaal** | 14-25 kts | golf >1,1m EN periode ≥5s | side-shore of licht aflandig |
| **Goed (a)** | 14-25 kts | golf <1,1m OF periode <5s | licht aanlandig |
| **Goed (b)** | <15 kts (gust <19) | golf >1,1m EN periode ≥5s | niet pal aanlandig |
| **Matig** | <15 kts (gust <19) | golf <1,1m OF periode <5s | (ongeacht) |
| **Slecht** | gust <16 kts ÉN gem <14 kts | (ongeacht) | (ongeacht) |
| **Slecht** | (ongeacht) | grote branding, geen pierbescherming | pal aanlandig |

Volgorde van checken: eerst de twee "Slecht"-condities uitsluiten, dan
Optimaal, dan Goed(a)/Goed(b), dan Matig. Combinaties die niet exact
passen: beschrijf ze als grensgeval tussen de twee dichtstbijzijnde
categorieën in plaats van te forceren.

## Pier-logica (Noordpier Wijk aan Zee vs. Zuidpier IJmuiden)

Alleen vermelden als: windrichting is pal aanlandig OF licht aanlandig,
ÉN golfhoogte ≥ 0,8m. Anders weglaten (niet relevant genoeg).

De twee pieren liggen aan weerszijden van dezelfde havenmond en werken
spiegelbeeldig — de pier aan de kant waar de golfslag/wind vandaan komt,
breekt die golfslag en maakt de tegenoverliggende (lij-)zijde rustiger:

| Windrichting komt uit | Rustiger/veiliger kant | Reden |
|---|---|---|
| ~170°-260° (zuid/zuidwest) | **Wijk aan Zee** (Noordpier) | pier breekt de zuid(west)-golfslag, minder shorebreak, makkelijker erdoor (vooral bij eb) |
| ~280°-360° of 0°-30° (noordwest/noord) | **IJmuiden** (Zuidpier) | pier breekt de noord(west)-golfslag |
| ~260°-280° (recht west) | Geen duidelijk voordeel | golven komen recht op beide pieren af |

Extra vermelden indien van toepassing:
- Bij vloed is de shorebreak overal zwaarder dan bij eb, ook aan de
  "beschutte" kant — noem dit als getij-informatie beschikbaar is.
- Bij windkracht 6+ (>27kts) uit W/ZW/NW sluit de Reddingsbrigade IJmuiden
  de pieren voor wandelaars — dit is een onafhankelijk signaal dat de
  omstandigheden daar ruw zijn.

## Lange-termijn outlook (dag 4-9)
Gebruik alleen Windfinder (enige bron die zo ver vooruitkijkt). Pas dezelfde
criteria toe. Vermeld expliciet dat voorspellingen 4+ dagen vooruit onzeker
zijn en dichter bij de tijd opnieuw gecheckt moeten worden. Geef een korte
kwalitatieve inschatting (laag/gemiddeld/hoog) van de kans op een mooie
sessie, met de dag(en) die het kansrijkst lijken.

## Output
Vul `sjabloon.md` volledig in met de bevindingen van deze run. Post het
resultaat naar Slack in kanaal #wingfoil-briefing via de Slack-connector.
Houd de Slack-versie beknopt en scanbaar (gebruik emoji-kopjes zoals in het
sjabloon, geen lange lappen tekst per dag). Voeg 2 afbeeldingen toe: bij de avond briefing de windforecast van "morgen" en "overmorgen" van soarcast en bij de ochtend briefing de forecast van "vandaag" en "morgen"
