---
title: "Eigen bestanden"
---

# Eigen bestanden op de kaart

Met **Lokaal bestand toevoegen** zet je een eigen GIS-bestand tijdelijk op de kaart. Zo bekijk je een bestand naast
de andere kaartlagen, zonder het eerst te publiceren en zonder aanvullende GIS-software.

## Een bestand toevoegen

1. Klik rechtsboven op **Kaartlagen** en kies **Lokaal bestand toevoegen**.
1. Sleep een bestand naar het venster, of klik in het venster om een bestand te selecteren.
1. Bevat het bestand meerdere lagen, zoals een GPX-bestand met waypoints en tracks, kies dan welke lagen je wilt
   importeren. Elke laag krijgt een eigen kleur.
1. MapGallery herkent de projectie automatisch. Is de projectie onjuist, dan kun je deze aanpassen.
1. De lagen worden op de kaart en in de [legenda](index.md#de-legenda) weergegeven.

<!-- SCREENSHOT: layers/import.png — Venster Lokaal bestand importeren na het kiezen van een GPX-bestand, met de keuze van lagen -->

## Ondersteunde bestandstypen

| Bestandstype | Extensie |
|--------------|----------|
| CSV | `.csv`, met coördinaten of WKT-geometrie |
| Shapefile | `.zip`, met alle bestanden van de shapefile |
| GeoJSON | `.geojson` of `.json` |
| KML | `.kml` |
| GeoPackage | `.gpkg` |
| GPX | `.gpx` |
| GML | `.gml` |

## Tijdelijke laag

Het bestand wordt **alleen op je eigen apparaat verwerkt**. Het wordt niet naar de server verstuurd en niet
opgeslagen. Dit betekent:

- de laag is alleen voor jou zichtbaar;
- de laag gaat niet mee als je een [link deelt](../export/index.md#link-kopieren);
- na het vernieuwen van de pagina moet je het bestand opnieuw toevoegen.

Wil je een bestand blijvend beschikbaar maken voor anderen, vraag dan de beheerder om het als kaartlaag te publiceren.
