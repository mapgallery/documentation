---
title: "Services"
description: "Services"
tags: [ api, dienst, kaartservice, rest, server ]
vars:
  plural: 'services'
  singular: 'service'
---

In deze sectie van de MapGallery beheeromgeving kun je verschillende services beheren, zoals API's, WMS en WFS. Een
service kan meerdere kaartlagen onstluiten.

{% include "admin/navigate-1.md" %}
2. Selecteer **Dashboard** uit het menu en ga naar de sectie **{{ page.meta.vars.plural }}**.
{% include "admin/navigate-2.md" %}

## Lijstweergave

{% include "admin/overview/intro.md" %}

| Naam       | Beschrijving                                                                               |
|------------|--------------------------------------------------------------------------------------------|
| `Id`       | Uniek identificatienummer van de {{ page.meta.vars.singular }}.                            |
| `Datum`    | Datum waarop de {{ page.meta.vars.singular }} is toegevoegd of voor het laatst is bewerkt. |
| `Naam`     | De naam van de {{ page.meta.vars.singular }}.                                              |
| `Protocol` | Het bestandsformaat of gebruikte protocol van de service.                                  |
| `Toegang`  | Toont of de service publiek toegankelijk is of geauthenticeerd.                            |
| `URL`      | De URL van de service.                                                                     |

### Acties

{% include "admin/overview/action.md" %}

{% include "admin/overview/filter.md" %}

{% include "admin/overview/button-add.md" %}

### Context menu

{% include "admin/overview/context-intro.md" %}

{% include "admin/overview/context-edd.md" %}

## Bewerkingsscherm

Via het bewerkingsscherm worden alle relevante details van een **{{ page.meta.vars.singular }}** weergegeven en kunnen
kunnen de instellingen
worden gewijzingd.

### Bewerkingsopties

Bovenaan de pagina zijn de tabbladen [**Algemeen**](base) en [**Kaartlagen**](layers) voor verschillende instellingen
van de {{ page.meta.vars.singular }}.

#### Tabblad Algemeen

Bevat de belangrijkste instellingen van de {{ page.meta.vars.singular }} (zoals hieronder beschreven). Velden met een *
zijn verplicht.
Uitleg van de Velden:

| Naam               | Beschrijving                                                                                                                                                                                 |
|--------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| `Uitschakelen`     | Wanneer deze optie is aangevinkt, wordt de collectie niet getoond in het overzicht voor de  eindgebruikers. De {{ page.meta.vars.singular }} blijft echter wel toegankelijk voor beheerders. |
| `Toegang`          | Hier kun je de toegang van de {{ page.meta.vars.singular }} instellen.                                                                                                                       |
| `Naam`             | De naam van de {{ page.meta.vars.singular }}.                                                                                                                                                |
| `Notitie`          | Hier kunnen eventuele beheernotities worden toevoegen die niet zichtbaar zijn voor de eindgebruikers.                                                                                        |
| `URL`              | Dit is de URL waarop de service beschikbaar is.                                                                                                                                              |
| `Query parameters` | Extra parameters die bij het opvragen van de service kunnen worden meegegeven: `Param1=value1&Param2=value2 `                                                                                |

#### Tabblad Protocol

Hier stel je het protocol in (bijvoorbeeld WMS of WFS) en kun je specificaties configureren zoals versies en
outputformaten.

#### Tabblad Authenticatie

In dit tabblad stel je in welke authenticatiemethoden worden gebruikt voor toegang tot de service. Er zijn drie
mogelijkheden:

* **None**: Geen authenticatie vereist. Kies deze optie voor een openbare service waar geen inlog- of
  verificatiemechanisme voor nodig is.
* **Basic Authentication**: Vereist een gebruikersnaam en wachtwoord om toegang te krijgen. Dit is een eenvoudige maar
  minder veilige authenticatiemethode.
* **HTTP header token**: Een token in de HTTP-header voor authenticatie. Dit is een veelgebruikte methode voor
  API-toegang waarbij een token als beveiligingssleutel fungeert.
* **Query parameter token**: Een authenticatietoken wordt meegegeven als queryparameter in de URL.

#### Tabblad Foutmeldingen

Wanneer er problemen optreden met een service, zoals een API, WMS of WFS, kan de
foutmeldingen log nuttige informatie bieden om de oorzaak te achterhalen en op te lossen.

### Acties

{% include "admin/action/action.md" %}

{% include "admin/action/button-open.md" %}

{% include "admin/action/button-add-layers.md" %}

{% include "admin/action/button-save.md" %}

### Context menu

Via het uitklapmenu zijn de onderstaande opties beschikbaar.

![](/assets/svg/list.svg "Lijst") **Terug naar lijst**: Terug naar de lijst en de wijzigingen niet opslaan.

![](/assets/svg/delete.svg "Verwijderen") **Verwijderen**: Door in het uitklapmenu te kiezen voor Verwijderen
kun je een {{ page.meta.vars.singular }} verwijderen.

## Een {{ page.meta.vars.singular }} toevoegen

{% include "admin/add.md" %}

### Ondersteunde formaten en protocollen

* **GeoJSON**: JSON-gebaseerd [GIS-bestand](https://geojson.org/) voor het uitwisselen van geografische gegevens.
* **HTTP**: URL van web-assets voor het direct laden van symbolen of metadata. Dit protocol wordt gebruikt om assets te
  _whitelisten_ voor de proxy, zodat deze kunnen worden geladen.
* **MapBox**: Vectorlaag dat de MapBox/MapLibre specificatie volgt, vaak gebruikt voor schaalbare,
  interactieve kaarten.
* **REST**: Simpele REST API voor het ophalen van geografische data via een standaard HTTP-interface. Het formaat kan
  XML of JSON zijn. MapGallery converteert intern de gegevens naar GeoJSON op basis van Latitude- en
  Longitude-velden.
* **TileJSON**: Vectortiles laag dat de TileJSON-specificatie volgt.
* **TMS**: Tile Map Service, een protocol voor het laden van kaartlagen als rastertiles.
* **WFS**: [Web Feature Service](https://docs.geoserver.org/stable/en/user/services/wfs/reference.html), een OGC-standaard voor het uitwisselen van vectorgeometrieën en bijbehorende attributen.
* **WMS**: [Web Map Service](https://docs.geoserver.org/stable/en/user/services/wms/reference.html), een OGC-standaard voor het opvragen van kaartafbeeldingen op basis van geografische
  gegevens.
* **WMTS**: Web Map Tile Service, een OGC-standaard voor het opvragen van kaartlagen als voorgerenderde tiles.
* **XYZ**: Laag met een eenvoudige URL-structuur voor het laden van kaarten als rastertiles.

## Een {{ page.meta.vars.singular }} verwijderen

{% include "admin/delete.md" %}