---
title: "Zoeken"
---

# Zoeken

Met het zoekvenster vind je eenvoudig adressen, gegevens binnen actieve kaartlagen, kaartlagen, collecties,
ondergronden en coördinaten. De resultaten verschijnen al terwijl je typt.

## Het zoekvenster openen

Klik rechtsboven op **Zoeken**, of druk op ++ctrl+k++ (Windows) of ++cmd+k++ (Mac). Voer een zoekterm in, zoals een
adres, een plaatsnaam, een onderwerp, een thema of een coördinaat.

<!-- SCREENSHOT: search/search-layers.png — Zoekvenster, tabblad Kaartlagen: vinkjes, tags, protocol en sneltoetsenbalk -->

## Zoekcategorieën

De zoekresultaten worden verdeeld over zes tabbladen. Achter elk tabblad staat het aantal resultaten. Tabbladen
zonder resultaten worden grijs weergegeven en het venster opent automatisch een tabblad met resultaten.

| Tabblad | Zoekt naar | Wat er gebeurt bij een klik |
|---------|------------|-------------------------------|
| **Adres** | Adressen, wegen, postcodes, buurten, wijken, woonplaatsen, gemeenten, provincies en meer | De kaart zoomt in op de locatie of het gebied. |
| **Gegevens** | Waarden in de actieve kaartlagen | Het object wordt geselecteerd en de kaart zoomt erop in. |
| **Kaartlagen** | Titels, beschrijvingen, zoekwoorden en classificaties van kaartlagen | De kaartlaag wordt aan de kaart toegevoegd. |
| **Collecties** | Collecties en hun beschrijving | De collectie wordt geopend. |
| **Ondergrond** | Beschikbare ondergronden | De ondergrond wordt geactiveerd. |
| **Coördinaat** | Coördinaatpunten in mogelijke coördinatenstelsels | De locatie wordt op de kaart weergegeven. |

Elk resultaat heeft een label voor het soort resultaat, zoals **PROVINCIE**, **WOONPLAATS**, **WFS** of
**MULTIPOLYGON**. Bij kaartlagen, collecties en ondergronden zie je daarnaast de bron, de classificaties en een korte
beschrijving.

### Adres

Via de PDOK Locatieserver wordt gezocht in gegevens uit diverse overheidsregistraties, zoals adressen, postcodes,
woonplaatsen en provincies. Je kunt ook zoeken op perceelnummers of specifieke objecten, zoals hectometerpalen.

Je kunt de zoekterm verder specificeren op:

- **Type**, zoals provincie, gemeente, woonplaats, postcode, adres, perceel, wijk, buurt of hectometerpaal;
- **Bron**, zoals BAG (Basisregistratie Adressen en Gebouwen), NWB (Nationaal Wegenbestand), DKK (Digitale
  Kadastrale Kaart), CBS of HWH (Het Waterschapshuis).

| Zoeken naar | Voorbeeld |
|-------------|-----------|
| Adres | `Sint Jansstraat 4 Groningen` |
| Postcode | `1622 hp` |
| Perceel | `DMN00 A 220` |
| Hectometerpaal | `a1-100 type:hectometerpaal` |
| Wegtracé | `A2 bron:NWB` |
| Gemeente | `hoorn type:gemeente` |

Uitgebreide informatie over de zoektermen vind je in de wiki van de PDOK Locatieserver onder
[Gebruik van zoektermen](https://github.com/PDOK/locatieserver/wiki/API-Locatieserver#2-gebruik-van-zoektermen-bij-solr-services).

### Gegevens

Alle actieve vectorkaartlagen zijn doorzoekbaar op hun gegevensvelden. Bij elk resultaat zie je de naam van de
kaartlaag, het attribuut en de waarde waarop een overeenkomst is gevonden.

### Kaartlagen

MapGallery doorzoekt de volledige verzameling kaartlagen, inclusief metadata en beschrijvingen. Zonder zoekterm zie je
alle kaartlagen die voor jou beschikbaar zijn.

- Klik op een kaartlaag of op het **vinkje** ervoor om de kaartlaag toe te voegen.
- Een kaartlaag die al op de kaart staat, is aangevinkt. Haal het vinkje weg om de kaartlaag te verwijderen.
- Wil je meerdere kaartlagen achter elkaar toevoegen, gebruik dan ++shift+enter++. Het zoekvenster blijft dan open.

### Collecties en ondergronden

Zoek op een onderwerp of een specifieke term. Klik op een collectie om deze te openen of op een ondergrond om deze te
gebruiken. Zie ook [Collecties](../collections/index.md) en [Ondergronden](../map/index.md#ondergronden).

### Coördinaat

Voer een coördinaat in, bijvoorbeeld `155000 463000`. MapGallery zoekt automatisch naar de coördinatenstelsels
waarin dit coördinaat kan liggen, zoals Rijksdriehoekstelsel (EPSG:28992), WGS84 (EPSG:4326) of Web Mercator
(EPSG:3857). Klik op het juiste coördinatenstelsel om de locatie direct op de kaart weer te geven.

## Sneltoetsen

Onder in het zoekvenster staan de sneltoetsen:

| Toets | Functie |
|-------|---------|
| ++enter++ | Het gekozen resultaat openen en het zoekvenster sluiten |
| ++arrow-up++ / ++arrow-down++ | Door de resultaten navigeren |
| ++tab++ | Naar het volgende tabblad gaan (bron kiezen) |
| ++esc++ | Het zoekvenster sluiten |
| ++shift+enter++ | Het gekozen resultaat openen zonder het zoekvenster te sluiten |
