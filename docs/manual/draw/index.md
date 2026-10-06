---
title: "Meten & Tekenen"
---

# Meten & Tekenen

Met **Meten & Tekenen** meet je afstanden, oppervlakten en coördinaten op de kaart. Daarnaast annoteer je de kaart
met punten, lijnen en vlakken, bijvoorbeeld om aandachtspunten of locaties vast te leggen of gebieden te duiden. Je
opent de tool met de knop **Meten & Tekenen** in de zijbalk links.

## Meten en tekenen

<!-- SCREENSHOT: draw/draw.png — Meten & Tekenen met een punt, lijn en vlak in de lijst en de labels op de kaart -->

| Knop | Tekent | Meet |
|------|--------|------|
| **Punt** | Een punt op de kaart | Het coördinaat van de locatie |
| **Lijn** | Een lijn met één of meer knikpunten | De afstand |
| **Vlak** | Een gebied | De oppervlakte |
| **Selecteren** (handje) | — | Bestaande tekeningen selecteren en verplaatsen |

1. Kies **Punt**, **Lijn** of **Vlak**.
1. Klik op de kaart op het gewenste beginpunt. Bij een lijn of vlak klik je vervolgens op elk volgend punt.
1. Dubbelklik om de lijn of het vlak af te sluiten.

Elke tekening krijgt op de kaart een label met een nummer en de gemeten waarde, bijvoorbeeld
**#1 Polygon (2895720.35 m2)**.

## Tekeningen beheren

Alle tekeningen staan in een lijst in het paneel, met het nummer, het type en de gemeten waarde. Per tekening kun je:

- de **volgorde wijzigen** door de tekening aan het handvat links te verslepen;
- een eigen **naam** geven;
- op de tekening **inzoomen**;
- de tekening **verbergen** en weer **zichtbaar maken** met het oogpictogram;
- de tekening **verwijderen** met de prullenbak. De tekening wordt direct verwijderd, zonder bevestiging.

Klik op **⋮** bij een tekening voor extra opties:

| Optie | Functie |
|-------|---------|
| **Overnemen naar locatie informatie** | Alle objecten binnen de tekening selecteren. Je bekijkt dan welke objecten binnen de tekening vallen, toont statistieken of downloadt de gegevens. Zie [Selecteren](../location/selection.md). |
| **Tekening downloaden als GeoJSON** | De tekening opslaan als GeoJSON-bestand, om deze te bewaren of in andere software te gebruiken. |
| **Buffer** | Een buffer rond de tekening maken met een zelfgekozen afstand. Vul de afstand in meters in en klik op **OK**. |

## Eenheden aanpassen

Via het **tandwiel** in de kop van het paneel pas je de eenheden voor afstanden en oppervlakten aan:

| Meting | Eenheden | Standaard |
|--------|----------|-----------|
| Afstand | meter, kilometer, mijl, zeemijl | meter |
| Oppervlakte | vierkante meter, vierkante kilometer, vierkante mijl, hectare | vierkante meter |

<!-- SCREENSHOT: draw/units.png — Tandwielmenu met de keuze voor afstand en oppervlakte -->

## Tekeningen bewaren

!!! note
    De tekeningen worden automatisch **lokaal in je browser** opgeslagen. Ze blijven behouden wanneer je de pagina
    vernieuwt of MapGallery later opnieuw opent.

- Tekeningen zijn alleen zichtbaar op de kaart als het paneel Meten & Tekenen is geopend.
- Tekeningen gaan **niet** mee naar een andere computer of browser en ook niet in een
  [gedeelde link](../export/index.md#link-kopieren). Wil je een tekening bewaren of delen, download deze dan als
  GeoJSON.
- Tekeningen en hun labels worden wel meegenomen in [Kaart als afbeelding](../export/index.md#kaart-als-afbeelding).
- Als je de browsergegevens van MapGallery wist, worden je tekeningen verwijderd.
