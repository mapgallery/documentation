---
title: "Downloaden & delen"
---

# Downloaden & delen

Er zijn verschillende manieren om gegevens en kaartbeelden uit MapGallery te exporteren. Je downloadt de gegevens van
kaartlagen, deelt een link naar het huidige kaartbeeld of slaat de kaart op als afbeelding.

## Gegevens downloaden

Je downloadt gegevens vanuit drie plaatsen:

| Wat | Waar |
|-----|------|
| Een volledige kaartlaag | De knop **Download** in de [metadata](../layers/metadata.md) van de kaartlaag |
| Een selectie | De knop **Download** in de [tabel](../location/selection.md#tabel) van een selectie |
| Een gefilterde kaartlaag | De knop **Download** in de metadata, terwijl er een [filter](../layers/filter.md) actief is. Je ontvangt dan alleen de gefilterde objecten. |

Niet elke kaartlaag kan worden gedownload. Dit hangt af van de instellingen van de beheerder en van de bron van de
gegevens.

### Het downloadvenster

<!-- SCREENSHOT: export/download.png — Downloadvenster met aantal objecten, formaten en projectie -->

1. Bovenaan zie je hoeveel objecten je downloadt.
1. Kies het **bestandsformaat** waarin je de gegevens wilt opslaan:

    | Formaat | Extensie | Toepassing |
    |---------|----------|------------|
    | GeoPackage | `.gpkg` | Aanbevolen voor QGIS en ArcGIS |
    | Shapefile | `.zip` | Gezipt, voor oudere GIS-software |
    | GeoJSON | `.geojson` | Voor webtoepassingen, altijd in WGS84 |
    | CSV | `.csv` | Tabel met coördinaten of WKT-geometrie |
    | Excel | `.xlsx` | Alleen de attributen, zonder geometrie |
    | DXF | `.dxf` | Voor CAD-software, alleen de geometrie |

1. Kies de **projectie** waarin je de gegevens wilt downloaden: Rijksdriehoekstelsel (EPSG:28992), WGS84 (EPSG:4326)
   of Web Mercator (EPSG:3857). De projectie bepaalt hoe de geografische coördinaten worden weergegeven.
1. Klik op **Download** om de gegevens naar je apparaat te downloaden.

## Link kopiëren

Met deze optie maak je een directe link naar het huidige kaartbeeld. Deze link kun je delen met anderen, zodat zij
dezelfde kaartweergave bekijken. Dit is nuttig om specifieke locaties of instellingen te delen met collega's of
klanten.

1. Open het [Hoofdmenu](../menu/index.md).
1. Kies **Delen → Link kopiëren**. De link staat nu op je klembord.
1. Plak de link in bijvoorbeeld een e-mail of chatbericht.

| Wordt meegenomen in de link | Wordt niet meegenomen |
|-----------------------------|-----------------------|
| Positie, zoomniveau, rotatie en kanteling | [Tekeningen](../draw/index.md#tekeningen-bewaren) |
| Actieve kaartlagen en ondergrond | [Lokale bestanden](../layers/import.md#tijdelijke-laag) |
| De geopende collectie | |
| Filters en aangepaste stijlen | |

De ontvanger ziet alleen de kaartlagen waartoe hij of zij zelf toegang heeft.

## Kaart als afbeelding

Met deze optie sla je de huidige weergave van de kaart op als afbeelding in PNG-formaat. Dit is geschikt voor
rapporten of presentaties waarin een momentopname van de kaart nodig is. De afbeelding bevat de zichtbare kaartlagen,
de legenda en je tekeningen.

1. Open het [Hoofdmenu](../menu/index.md).
1. Kies **Delen → Kaart als afbeelding**.
