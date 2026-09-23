---
title: "E. Zoekfunctie"
---

De [Zoekfunctie (D)](../map/#kaartviewer) maakt het eenvoudig om specifieke kaartlagen, coördinaten, adresgegevens en gegevens binnen actieve kaartlagen te vinden. Hieronder volgt een uitleg van de verschillende mogelijkheden en opties binnen de zoekfunctie.

## Zoekvenster
Door ++control++ + ++k++ in te drukken of rechtsboven op het vergrootglas (![](/assets/svg/search_icon.svg#middle)) te klikken, kom je bij het zoekvenster.

Voer een trefwoord in het zoekveld in, zoals een onderwerp, thema of specifieke term die je zoekt. Nadat je op ++enter++ drukt of op het vergrootglas klikt, worden de resultaten direct weergegeven.

## Zoekresultaten
De zoekresultaten worden weergegeven in een lijst. Als de zoekresultaten niet zijn wat je zoekt, kun je eenvoudig je zoekterm wijzigen door een nieuwe term in te voeren in het zoekveld. Voor elk kaartlaagresultaat krijg je de volgende informatie te zien:

* **Titel** van de kaartlaag
* Naam van de **Service** (bron) van de kaartlaag
* **Classificaties**: Classificaties die aan de kaartlaag zijn gekoppeld, waardoor je makkelijk kunt zien waar de
  dataset over gaat.
* **Beschrijving**: Een korte uitleg van wat de kaartlaag bevat.

Klik op een van de zoekresultaten om de kaartlaag of locatie te openen.

![](search_menu_mg8.png)


## Zoekcategorieën
De zoekresultaten worden weergegeven in verschillende categorieën. Je kunt zoeken naar adressen, gegevens, kaartlagen, collecties, ondergronden en coördinaten.

1. **Adressen**: hier worden resultaten weergegeven van adressen, postcodes, buurten, wijken, woonplaatsen, gemeenten en provincies.
1. **Gegevens**: hier kun je met zoekwoorden zoeken naar gegevens binnen de actieve kaartlagen.
1. **Kaartlagen**: hier wordt gezocht naar titels, beschrijvingen, zoekwoorden en classificaties van kaartlagen.
1. **Collecties**: hiermee kun je zoeken naar collecties en de bijbehorende beschrijving.
1. **Ondergronden**: hiermee kun je zoeken naar verschillende ondergrondkaartlagen.
1.  **Coördinaten**: hiermee kun je zoeken naar coördinaatpunten op de kaart.


### Adressen

Via de PDOK Locatieserver (geocodeerservice) wordt gezocht op gegevens uit diverse overheidsregistraties, zoals adressen, postcodes, woonplaatsen en provincies. Je kunt ook zoeken op perceelnummers of specifieke objecten, zoals hectometerpalen. Klikken op een resultaat selecteert de locatie of het gebied en zoomt hierop in.

Naast gewone zoekvelden kun je de zoekterm ook verder specificeren op:

* Type: zoals provincie, gemeente, woonplaats, postcode, adres, perceel, wijk, buurt, hectometerpaal, etc.
* Bron: zoals BAG (Basisregistratie Adressen en Gebouwen), NWB (Nationaal Wegen Bestand), DKK (Digitale Kadastrale
  Kaart), CBS, of HWH (Het Waterschapshuis).

#### Voorbeelden van zoekopdrachten

Adres: `Sint Jansstraat 4 Groningen`

Postcode: `1622 hp`

Perceel: `DMN00 A 220`

Hectometerpaal: `a1-100 type:hectometerpaal`

Wegtrace: `A2 bron:NWB`

Gemeente: `hoorn type:gemeente`

Zie voor uitgebreide informatie over de PDOK Locatieserver de
wiki, [gebruik van de de zoektermen](https://github.com/PDOK/locatieserver/wiki/API-Locatieserver#2-gebruik-van-zoektermen-bij-solr-services).


### Gegevens
Alle actieve vector-kaartlagen in de Kaartviewer zijn doorzoekbaar op gegevensvelden. De zoekfunctie geeft suggesties voor een match en toont hierbij de naam van de kaartlaag, het attribuut en de waarde waarop een match is gevonden.

Klik op een resultaat om de bijbehorende geometrie te selecteren en hierop in te zoomen.

### Kaartlagen
De zoekfunctie geeft resultaten voor relevante kaartlagen. MapGallery doorzoekt het volledige bestand van kaartlagen, metadata en beschrijvingen. Op basis hiervan worden kaartlagen weergegeven die aansluiten bij de ingevoerde zoekterm. Klik op een kaartlaag om deze toe te voegen. 

### Collecties
Met de zoekfunctie kun je ook zoeken naar collecties. Hierbij wordt gezocht naar collecties die aansluiten bij de zoekterm en naar de bijbehorende beschrijving. Klik op een collectie om deze aan de kaart toe te voegen.

### Ondergronden
De zoekfunctie kan ook worden gebruikt om beschikbare ondergronden te vinden. Zoek op een onderwerp of specifieke term om beschikbare ondergrondkaartlagen te vinden. Klik op een zoekresultaat om de betreffende ondergrond te openen en te gebruiken.

### Coördinaten
Wanneer je coördinaten hebt ingevoerd, maakt MapGallery automatisch een match met mogelijke projecties. Klik vervolgens op de juiste projectie om de locatie direct op de kaart weer te geven.


