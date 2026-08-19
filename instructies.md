# Instructies: Wingfoil-briefing Zandvoort–Wijk aan Zee

Dit document is de volledige context voor een geautomatiseerde dagelijkse
briefing. Een verse sessie heeft geen geheugen van eerdere gesprekken —
alles wat nodig is om de taak goed uit te voeren staat hieronder.

## Doel
Twee keer per dag (07:15 en 23:15) een wingfoil-conditiebriefing produceren
voor de kuststrook tussen Zandvoort en Wijk aan Zee, gebaseerd op drie
onafhankelijke windbronnen, en deze posten in Slack via het sjabloon in
`sjabloon.md`.

## Efficiëntie (belangrijk -- houd de doorlooptijd kort)
Deze routine draait 2x per dag en moet ruim binnen 15-20 minuten klaar zijn.
Algemene regels:
- Navigeer bronnen altijd via de exacte URL's/selectors die verderop bij
  elke bron staan beschreven -- nooit handmatig zoeken/klikken/pannen op
  een kaart of menu als een direct pad beschikbaar is.
- Gebruik get_page_text/tekstextractie als standaard. Maak alleen een
  screenshot als tekstextractie de benodigde cijfers aantoonbaar niet
  oplevert (bv. een grafiek zonder onderliggende tabeldata), en dan
  maximaal 1 screenshot per bron/dag.
- Doe geen extra verkennende stappen ("laten we kijken wat er nog meer
  op deze site staat") -- haal precies op wat nodig is voor het sjabloon.
- Zie ook de aparte AVONDBRIEFING-scope hieronder: 's avonds hoeft de
  lange-termijn outlook niet opnieuw volledig herhaald te worden.

## Gebied en geografie

### Kustlijn-hoek per plek (niet één vaste hoek voor het hele gebied)
Windrichting in graden = waar de wind VANDAAN komt (meteorologische
conventie) -- dit geldt voor alle onderstaande hoeken.

De kust tussen Zandvoort en Wijk aan Zee is vrij recht maar met een lichte
kromming; dit geeft per plek een net iets andere referentiehoek voor
aanlandig/aflandig/side-shore. Gebruik ALTIJD de hoek van de dichtstbijzijnde
plek uit onderstaande tabel, niet één gemiddelde hoek voor het hele gebied.

| Plek | Lokale kustlijn (graden) | Pal aanlandig | Pal aflandig |
|---|---|---|---|
| **Zandvoort** | 17,5° / 197,5° | 287,5° (WNW) | 107,5° (OZO) |
| **Bloemendaal aan Zee** | 18,1° / 198,1° | 288,1° (WNW) | 108,1° (OZO) |
| **IJmuiden** (direct onder/bij de pier, eerste ~500m) | 150° / 330° | 240° (WZW) | 60° (ONO) |
| **IJmuiden** (open strand, verder ten zuiden vd pier) | 16,3° / 196,3° | 286,3° (WNW) | 106,3° (OZO) |
| **Wijk aan Zee** (ten noorden vd pier) | 13,8° / 193,8° | 283,8° (WNW) | 103,8° (OZO) |

**Let op IJmuiden -- twee zones, gebruik de juiste:** direct tegen de pier
krult het strand lokaal sterk om (sediment hoopt zich op tegen de
pierzijde, een bekend effect bij havenhoofden), waardoor de kustlijnhoek
daar (150°/330°) sterk afwijkt van het open strand verderop naar het
zuiden (16,3°/196,3°) -- een verschil van ~46° dat classificaties WEL kan
laten kantelen. **Gebruik voor "IJmuiden" als wingfoil-spot standaard de
pierzone-hoek (150°/330°, dus pal aanlandig ≈240°)**, aangezien dit de
gangbare launch-plek is vlak bij de pier; gebruik de open-strand-hoek
alleen als expliciet duidelijk is dat de sessie verder van de pier
plaatsvindt.

Overige verschillen (Zandvoort/Bloemendaal/Wijk aan Zee/open IJmuiden) zijn
klein (max ~4° onderling) en zullen zelden een classificatie
(aanlandig/aflandig/side-shore) laten kantelen, maar gebruik voor de
precisie toch steeds de plekspecifieke hoek uit de tabel bij het
beoordelen van een venster voor die plek, in plaats van een enkele hoek
voor het hele gebied te hergebruiken.

### Classificatie windrichting t.o.v. kust (per plek, met bovenstaande hoeken)
- **Pal aanlandig**: binnen ~30° van de "pal aanlandig"-waarde voor die plek
- **Licht aanlandig**: 30-45° daarvan (richting land, maar niet loodrecht)
- **Pal aflandig**: binnen ~30° van de "pal aflandig"-waarde voor die plek
- **Licht aflandig**: 30-45° daarvan
- **Side-shore**: overig, richting rond de kustlijn-waarde zelf (evenwijdig aan kust)

### Pierhoek (voor de pier-logica verderop)
De havenmond/pieren van IJmuiden liggen NIET evenwijdig aan de kust, maar
lopen er vrijwel loodrecht op de zee in. Belangrijk: de twee pieren staan
NIET parallel aan elkaar -- de havenmond is trechtervormig (breder aan de
zeekant), een bewust asymmetrisch ontwerp dat verzanding van de vaargeul
tegengaat. Elke pier heeft dus zijn eigen aslijn:

- **Noordpier** (Wijk aan Zee-kant): aslijn **100,5° / 280,5°** -- dit is
  de officiële "lichtenlijn" die de scheepvaart door de havenmond volgt.
- **Zuidpier** (IJmuiden-kant): aslijn **70° / 250°** -- ligt dus ~30°
  meer naar het zuiden gedraaid dan de Noordpier-as.

Dit is de hoek die bepaalt vanuit welke richting elke pier golfslag/wind
het effectiefst blokkeert (zie Pier-logica-sectie): een pier blokkeert
golven die van de kant komen waar de pier "voor" ligt, en biedt lij aan de
tegenoverliggende kant. Omdat de twee pierassen uiteenlopen, is de
"neutrale zone" waarin geen van beide pieren een duidelijk voordeel biedt
breder dan bij twee parallelle pieren: ongeveer **250°-280°** (het gebied
tussen de twee zeewaarts wijzende pierassen) -- zie de tabel in de
Pier-logica-sectie voor de precieze grenzen.

## Bronnen (alle drie gebruiken, niet middelen maar naast elkaar tonen)

### 1. Windfinder — https://www.windfinder.com/forecast/zandvoort_south_beach
- GFS-model, tabeldata per 1-3 uur, tot 9-10 dagen vooruit.
- EFFICIENTIE: gebruik get_page_text (GEEN screenshots) direct na navigeren.
  Navigeer één keer naar de forecast-URL hierboven; de tabel bevat meestal
  al 2 dagen. Voor de lange-termijn outlook (dag 4-9): navigeer direct naar
  https://www.windfinder.com/weatherforecast/zandvoort_south_beach
  (de Superforecast-pagina) i.p.v. handmatig door dagtabs te klikken.
  Als een van beide pagina's toch maar 1 dag toont, klik dan alleen de
  ontbrekende dagtab aan -- niet alle tabs opnieuw doorlopen.
- Kolommen: windrichting (graden), windsnelheid (kts), gusts (max kts),
  golfrichting, golfhoogte (m), golfperiode (s), getij.
- Gebruik dit als hoofdbron voor golfdata (enige bron met golfperiode/-hoogte).

### 2. Soarcast — station IJmond (KNMI)
- Draait op het KNMI Harmonie-model, specifiek voor NL-kustspots.
- EFFICIENTIE: navigeer DIRECT naar onderstaande URL's -- NIET via de kaart
  klikken/zoomen/pannen (dat kost onnodig veel stappen):
  - Vandaag:     https://www.soarcast.nl/web/locationinfo?location=133&day=today
  - Morgen:      https://www.soarcast.nl/web/locationinfo?location=133&day=tomorrow
  - Overmorgen:  https://www.soarcast.nl/web/locationinfo?location=133&day=dayaftertomorrow
- Gebruik get_page_text voor de omliggende tekst/context; voor de
  grafiekwaarden zelf (wind/gust/richting per uur) is een gerichte blik op
  de grafiek nodig -- lees zo mogelijk de onderliggende data i.p.v. een
  volledige paginascreenshot te maken. Beperk tot 1 screenshot per dag-tab
  als tekst-extractie de grafiekwaarden niet oplevert.
- Toont wind+gust (grafiek, kts) en windrichting (graden). GEEN golfdata
  (landstation meet geen golven).
- Gebruik dit als kruisvalidatie op wind/gust/richting naast Windfinder.
  Bij grote afwijking tussen beide modellen: vermeld dit expliciet in de
  briefing i.p.v. te middelen.

### 3. windwaarnemingen.nl — https://www.windwaarnemingen.nl/
- KNMI/RWS-data. Selecteer station **IJmuiden** in de dropdown.
- EFFICIENTIE: er is GEEN directe URL-parameter voor het station (dit is
  getest) -- het station wordt clientside via JavaScript geselecteerd.
  Gebruik het select-element met id="stat" (name="Station"), zet de waarde
  op "IJmuiden" en trigger een change-event, in plaats van te zoeken naar
  het element via een generieke "vind de dropdown"-stap. Voorbeeld
  (JS-uitvoering op de pagina):
  document.querySelector('#stat').value = 'IJmuiden';
  document.querySelector('#stat').dispatchEvent(new Event('change'));
  Gebruik hierna direct get_page_text, geen screenshot nodig -- de tabel
  is gewone HTML-tekst.
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

### Avondbriefing (23:15) — geen realitycheck-sectie, kortere outlook-stap
De volledige 72-uursanalyse (dag 1-3), zonder de ochtend-specifieke
vergelijking (die is 's avonds niet zinvol omdat de komende dag nog moet
beginnen).

EFFICIENTIE: voor de lange-termijn outlook (dag 4-9) hoeft 's avonds niet
de volledige Windfinder-langetermijnpagina opnieuw met evenveel diepgang
doorlopen te worden als 's ochtends -- de outlook verandert zelden binnen
16 uur. Eén korte blik op de Superforecast-pagina volstaat om te bevestigen
dat de eerdere inschatting nog klopt; alleen bij een duidelijke wijziging
uitgebreider herformuleren.

## Beoordelingscriteria (per tijdstip toepassen)

| Oordeel | Wind gemiddeld | Golfhoogte + periode | Windrichting |
|---|---|---|---|
| **Optimaal** | 14-25 kts | golf >0,95m EN periode ≥4,5s | side-shore of licht aflandig |
| **Goed (a)** | 14-25 kts | golf <0,95m OF periode <4,5s | licht aanlandig |
| **Goed (b)** | <15 kts (gust <19) | golf >0,95m EN periode ≥4,5s | niet pal aanlandig |
| **Matig** | <15 kts (gust <19) | golf <0,95m OF periode <4,5s | (ongeacht) |
| **Slecht** | gust <16 kts ÉN gem <14 kts | (ongeacht) | (ongeacht) |
| **Slecht** | (ongeacht) | grote branding, geen pierbescherming | pal aanlandig |

Volgorde van checken: eerst de twee "Slecht"-condities uitsluiten, dan
Optimaal, dan Goed(a)/Goed(b), dan Matig. Combinaties die niet exact
passen: beschrijf ze als grensgeval tussen de twee dichtstbijzijnde
categorieën in plaats van te forceren.

## Pier-logica (Noordpier Wijk aan Zee vs. Zuidpier IJmuiden)

**Scope: dit is alleen relevant voor de keuze tussen IJmuiden en Wijk aan
Zee** (de twee plekken direct aan weerszijden van de havenmond). Voor
Zandvoort en Bloemendaal aan Zee is de pier te ver weg om nog een
merkbaar beschuttingseffect te hebben -- daar dus niet vermelden.

Alleen vermelden als: windrichting is pal aanlandig OF licht aanlandig
(voor IJmuiden en/of Wijk aan Zee volgens hun eigen hoek uit de tabel
hierboven), ÉN golfhoogte ≥ 0,8m. Anders weglaten (niet relevant genoeg).

De pieren liggen NIET parallel: de Noordpier heeft aslijn 100,5°/280,5°,
de Zuidpier 70°/250° (zie Geografie-sectie). De twee pieren liggen aan
weerszijden van dezelfde havenmond en werken spiegelbeeldig -- de pier aan
de kant waar de golfslag/wind vandaan komt, breekt die golfslag en maakt
de tegenoverliggende (lij-)zijde rustiger:

| Windrichting komt uit | Rustiger/veiliger kant | Reden |
|---|---|---|
| ~170°-250° (zuid/zuidwest) | **Wijk aan Zee** (Noordpier) | pier breekt de zuid(west)-golfslag, minder shorebreak, makkelijker erdoor (vooral bij eb) |
| ~280°-360° of 0°-30° (noordwest/noord) | **IJmuiden** (Zuidpier) | pier breekt de noord(west)-golfslag |
| ~250°-280° (tussen de twee pierassen in) | Geen duidelijk voordeel | golven vallen tussen de twee zeewaarts wijzende pierassen in -- geen van beide pieren biedt hier volledige lij |

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
Vul `sjabloon.md` volledig in met de bevindingen van deze run. Gebruik voor
de dagelijkse classificatie (Optimaal/Goed/Matig/Slecht) standaard de hoek
van **Zandvoort** als centrale referentie, tenzij de pier-logica in beeld
komt (aanlandige wind + golf ≥0,8m) -- vermeld dan expliciet zowel de
classificatie bij IJmuiden als bij Wijk aan Zee met hun eigen hoek uit de
tabel, plus het piervoordeel. Bloemendaal aan Zee ligt qua hoek vrijwel
gelijk aan Zandvoort en hoeft niet apart genoemd te worden tenzij er
specifiek naar gevraagd wordt.

Post het resultaat naar Slack in kanaal #wingfoil-briefing via de Slack-connector.
Houd de Slack-versie beknopt en scanbaar (gebruik emoji-kopjes zoals in het
sjabloon, geen lange lappen tekst per dag).
