---
title: "Versie 8"
---

# MapGallery 8 – Release notes

### 8.0 <small>oktober 2026</small>

MapGallery 8 is de grootste vernieuwing van MapGallery tot nu toe. De kaart krijgt het volledige scherm, zoeken gebeurt vanuit één centraal
venster en je kunt veel meer met de gegevens op de kaart. Selecteer objecten in een gebied, bekijk ze als tabel en download ze in het
gewenste formaat. Ook kun je eigen lokale bestanden direct openen en op de kaart zetten. Daarnaast is _Meten & Tekenen_ flink uitgebreid.

---

## Vernieuwde interface

*Meer kaart, minder knoppen.* De vaste bovenbalk is verdwenen en alle bediening zit nu op de kaart zelf. Zo heb je meer ruimte voor waar
het om draait, en staat elke functie op een vaste, herkenbare plek.

- **Zijbalk met gereedschappen** links: Locatie informatie (Info), Straatbeeld, Meten & Tekenen, Collectie en, na inloggen, Favorieten
  staan overzichtelijk in de zijbalk.
- **Zoeken, de legenda en het Hoofdmenu** staan rechtsboven en geven een vaste en herkenbare plek in de applicatie.
- **De legenda** is compacter. Hij kan worden ingeklapt, de knoppen per laag staan onderaan en minder gebruikte acties zitten in een extra
  menu. Vanuit de legenda voeg je kaartlagen toe en kies je de ondergrond.
- **Groepen in collecties en favorieten** hebben één knop om alle kaartlagen aan of uit te zetten, en tonen het aantal actieve lagen. De
  lagen op de kaart volgen de volgorde van de legenda.
- **Gereedschapsvensters** hebben minder witruimte, overlappen de kaart zo min mogelijk en zijn aanpasbaar in de breedte.
- **Vernieuwde schermen** voor metadata, downloaden, inloggen en registreren, en een overzichtelijker hoofdmenu.

| Versie 7                                | Versie 8                                           |
|-----------------------------------------|----------------------------------------------------|
| ![MapGallery 7](img/v7-startscherm.png) | ![MapGallery 8](img/v8-startscherm-collecties.png) |

Zie [De interface](../manual/index.md#de-interface) en [Kaartlagen & legenda](../manual/layers/index.md).

## Direct naar de kaart, met populaire collecties

In MapGallery staat de kaart centraal. Daarom kom je direct op de kaart en staan de **populaire en recent gebruikte** collecties meteen
klaar. Via _Meer collecties weergeven_ zoek je door alle collecties.

- Bestaande collecties uit versie 7 blijven werken en hoeven niet aangepast te worden.
- De collecties zijn doorzoekbaar en de classificaties worden ook weergegeven.
- Je verlaat een collectie of wisselt van collectie zonder de kaart te verlaten.
- Bij het wisselen van collectie passen de kaartlagen zich automatisch aan.
- Het logo linksboven brengt je terug naar de standaardcollectie.

Zie [Collecties](../manual/collections/index.md).

## Eén zoekvenster

Eén centraal zoekvenster doorzoekt adressen, gegevens, kaartlagen en collecties tegelijk. Je opent het met de knop **Zoeken** rechtsboven of
met de sneltoets **Ctrl/Cmd + K**.

- De resultaten worden overzichtelijk getoond in aparte tabbladen voor **Adres, Gegevens, Kaartlagen, Collecties, Ondergrond en
  Coördinaat**, elk met het aantal resultaten.
- Resultaten zijn rijker: een label voor het soort resultaat (zoals weg, adres, postcode, WFS, WMTS), thema-tags, de bron en een korte
  beschrijving.
- Je bedient het zoekvenster ook met het toetsenbord: met de pijltjes navigeer je, **Tab** kiest een bron en **Shift + Enter** voegt een
  kaartlaag toe zonder dat het venster sluit. Zo voeg je snel meerdere lagen toe.
- Lege tabbladen worden gedimd en het venster springt automatisch naar een tabblad met resultaten.

| Adres zoeken                             | Kaartlagen zoeken en toevoegen                                  |
|------------------------------------------|-----------------------------------------------------------------|
| ![Adres zoeken](img/v8-zoeken-adres.png) | ![Kaartlagen zoeken en toevoegen](img/v8-zoeken-kaartlagen.png) |

Zie [Zoeken](../manual/search/index.md).

## Locatie informatie

Klik op de kaart en je ziet meteen waar je bent: adres, buurt, wijk, woonplaats en gemeente in één overzicht. Ook selecteren, statistieken
en de tabel zitten nu in dit paneel.

- Een **adresblok** toont het coördinaat, het adres en de buurt, wijk, woonplaats en gemeente.
- Vanuit het adresblok **selecteer je objecten in een gebied**, zie [Objecten selecteren in een gebied](#objecten-selecteren-in-een-gebied).
- Bij meerdere geselecteerde objecten **blader je door de resultaten** (bijvoorbeeld 1 / 5).
- **Statistieken** over de geselecteerde objecten zijn naar dit paneel verplaatst.
- Ook de **tabelweergave** vind je nu in dit paneel, met download-mogelijkheid.

| Versie 7                                                      | Versie 8                                                      |
|---------------------------------------------------------------|---------------------------------------------------------------|
| ![Locatie informatie versie 7](img/v7-locatie-informatie.png) | ![Locatie informatie versie 8](img/v8-locatie-informatie.png) |

![Tabelweergave](img/v8-tabel.png)

Zie [Locatie informatie](../manual/location/index.md).

## Objecten selecteren in een gebied

Veel vragen beginnen met: wat ligt er in dit gebied? Daarom kun je nu op meer manieren en veel sneller objecten selecteren, rechtstreeks
vanuit Locatie informatie.

- **Selecteren op gebied:** kies in het adresblok buurt, wijk, woonplaats of gemeente en alle objecten die volledig binnen die grens liggen
  worden geselecteerd. Het selectiegebied volgt daarbij de grens van het gekozen gebied.
- **Selecteren met een rechthoek:** houd **Shift** ingedrukt en sleep een rechthoek over de kaart. Het paneel Locatie informatie opent dan
  automatisch, ook als het nog niet open was.
- **Selecteren met een getekend vlak** uit Meten & Tekenen.
- **Selecteren over meerdere lagen**, elk met een eigen kleur. Het uitgelichte object is gekleurd, de andere geselecteerde objecten zijn
  grijs.
- Het resultaat van je selectie kun je [downloaden](#downloaden) in verschillende GIS-formaten.
- Selecteren in grote gebieden is aanzienlijk sneller. Het gebied verschijnt direct op de kaart; de gegevens worden daarna aangevuld.

!!! note "Gewijzigd: alleen objecten volledig binnen het gebied"
    In versie 7 werden ook objecten geselecteerd die het gebied raakten (intersect). Nu worden alleen objecten geselecteerd die volledig
    binnen het gebied liggen (inside). Dit geldt voor selectie op gebied, met een rechthoek en met een getekend vlak.
    Zie [Selecteren, statistieken & tabel](../manual/location/selection.md).

| Selectie op gemeente                                  | Selectie met rechthoek                                   |
|-------------------------------------------------------|----------------------------------------------------------|
| ![Selectie op gemeente](img/v8-selectie-gemeente.png) | ![Selectie met rechthoek](img/v8-selectie-rechthoek.png) |

## Downloaden

Wat je op de kaart vindt, wil je misschien ook in je andere software kunnen gebruiken. Het volledig vernieuwde downloadvenster levert
gegevens in het formaat en de projectie die je nodig hebt, ongeacht de bron.

- Formaten: **GeoPackage, Shapefile (zip), GeoJSON, CSV, Excel en DXF**, elk met een korte uitleg wanneer je het gebruikt.
- Je kiest zelf de **projectie**, bijvoorbeeld het Rijksdriehoekstelsel (EPSG:28992).
- Het downloaden werkt ook voor **selecties en actieve filters**.
- Alle formaten zijn beschikbaar voor **elke bron met objectgegevens**: WFS, OGC API Features, REST API en GeoJSON.

![Downloadvenster](img/v8-download.png)

Zie [Downloaden & delen](../manual/export/index.md).

## Meten & Tekenen

Een tekening of meting is vaak het begin van een analyse of een kaart voor een rapport. Het gereedschap is daarom grotendeels opnieuw
opgezet: je werk blijft bewaard, is overzichtelijk te beheren en werkt samen met selecteren en de kaartexport.

- Alle getekende objecten staan in een **lijst**. Je kunt ze **verslepen om de volgorde te wijzigen**, tonen of verbergen, erop inzoomen,
  hernoemen of verwijderen.
- Getekende **objecten** blijven lokaal bewaard, ook nadat je het gereedschap of MapGallery hebt gesloten.
- Objecten krijgen een label op de kaart met nummer en maat.
- **Eenheden zijn instelbaar**: voor afstand meter, kilometer, mijl of zeemijl; voor oppervlakte m², km², mi² of hectare.
- De **buffertool** is geïntegreerd in Meten & Tekenen.
- Getekende gebieden kun je als **invoer gebruiken voor Locatie informatie**.
- Tekeningen, labels en afstanden worden meegenomen in de **kaartexport**.

| Tekenlijst                                   | Eenheden instellen               |
|----------------------------------------------|----------------------------------|
| ![Meten & Tekenen](img/v8-meten-tekenen.png) | ![Eenheden](img/v8-eenheden.png) |

Zie [Meten & Tekenen](../manual/draw/index.md).

## Eigen bestanden op de kaart

Snel een GIS-bestand bekijken, zonder het eerst te publiceren of andere GIS-software te openen? Met **Bestand importeren** zet je eigen
gegevens tijdelijk op de kaart. Je vindt deze functie in het **contextmenu ⋮** in de kop van de legenda.

- Ondersteunde formaten zijn **CSV, Shapefile (zip), GeoJSON, KML, GeoPackage, GPX en GML**.
- Bij bestanden met meerdere lagen, zoals een GPX-bestand of een GeoPackage, kies je zelf welke lagen je importeert. Iedere laag krijgt een
  eigen kleur.
- De projectie wordt automatisch herkend en kan worden aangepast.
- Het bestand wordt **op je eigen apparaat verwerkt**.

![Lokaal bestand importeren](img/v8-import.png)

Zie [Eigen bestanden op de kaart](../manual/layers/import.md).

## Voor beheerders

Voor de overstap naar versie 8 is geen actie nodig. Bestaande collecties en instellingen blijven werken. Wel wordt het dagelijks beheer
eenvoudiger: je vindt sneller wat je zoekt en vergissingen worden voorkomen.

- De knop **WFS-capabilities** helpt bij het configureren van WFS-lagen.
- Vanuit de metadata van een kaartlaag ga je direct naar het bijbehorende onderdeel in de **beheeromgeving**.
- Statistieken kun je ook bij grote aantallen als **CSV downloaden**.
- De beheeromgeving is beter bruikbaar op kleinere schermen.
- De tabbladen van een collectie heten nu **Startkaart** en **Lagenlijst**.
- Het tabblad **Collecties** bij een kaartlaag laat zien in welke collecties de laag wordt gebruikt. Verwijder je een kaartlaag, dan wordt
  deze ook uit de collectiegroepen gehaald.
- **Ingesloten kaarten** (embed) tonen een alleen-lezen legenda van de zichtbare kaartlagen.
- **WMS GetFeatureInfo** ondersteunt ook JSON-antwoorden die geen GeoJSON zijn, zoals die van ADAGUC.

## Onder de motorkap

Niet zichtbaar, wel merkbaar: MapGallery start sneller, laadt kaartlagen stabieler en is veiliger.

- Bijgewerkt naar **Angular 22** en actuele bibliotheken.
- **Kaartlagen laden sneller en stabieler** dankzij verbeterde caching en het ophalen van gegevens op de achtergrond.
- De **proxy** voor externe kaartdiensten is opnieuw opgebouwd en daardoor stabieler en veiliger.
- **Snellere opstart** van de applicatie. De iconen zijn bijgewerkt naar Material Symbols.
