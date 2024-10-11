---
title: "Kaartviews"
description: "Kaart views"
tags: [ zoom, extent, beginscherm, view, kaartweergave ]
vars:
  plural: 'kaartviews'
  singular: 'kaartview'
---

Een kaartview definieert het startscherm van een [collectie](../../collections/), waaronder de kaartcentrering, het
zoomniveau van de kaart en de keuze tussen een 2D- of 3D-weergave. Een kaartweergave kan worden gebruikt door meerdere
collecties.

{% include "admin/navigate-1.md" %}
2. Selecteer **Dashboard** uit het menu, kies het menu onder **Opties** (![menu](/assets/svg/access.svg "menu")) en ga
   naar de sectie **{{ page.meta.vars.plural }}**.
{% include "admin/navigate-2.md" %}

## Lijstweergave

{% include "admin/overview/intro.md" %}

| Naam           | Beschrijving                                                                               |
|----------------|--------------------------------------------------------------------------------------------|
| `Id`           | Uniek identificatienummer van de {{ page.meta.vars.singular }}.                            |
| `Datum`        | Datum waarop de {{ page.meta.vars.singular }} is toegevoegd of voor het laatst is bewerkt. |
| `Naam`         | De naam van de {{ page.meta.vars.singular }}.                                              |
| `Omschrijving` | Een korte uitleg over wat de {{ page.meta.vars.singular }} inhoudt.                        |
| `Zoom`         | Het ingesteld zoom level.                                                                  |
| `Center`       | Coordinaat in Latitude en Longtitude.                                                      |

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

Bovenaan de pagina zijn de tabbladen **Algemeen** en **Parameters** voor verschillende instellingen van de {{
page.meta.vars.singular }}.

#### Tabblad Algemeen

Bevat de belangrijkste instellingen van de {{ page.meta.vars.singular }} (zoals hieronder beschreven). Velden met een *
zijn verplicht.

`Zoom`: Stel het standaard zoomniveau in van de kaart. Een lager getal betekent dat je verder uitgezoomd bent, terwijl een hoger getal verder ingezoomd is.

`Pitch`: Hiermee bepaal je de hellingshoek van de kaart. Een waarde van "0" geeft een standaard verticale weergave (recht van
boven). Hogere waarden geven een schuine kijkhoek, wat handig is bij 3D-weergaven.

Onder de velden zie je een interactieve kaart. Deze kaart toont de huidige instellingen van locatie, zoom en pitch. Je
kunt op de kaart klikken en slepen om een nieuwe locatie te kiezen. De coördinaten, het zoomniveau en de pitch worden
dan automatisch bijgewerkt in
de velden.

#### Tabblad Parameters

Dit tabblad bevat geavanceerde parameters zoals het instellen van een minimale of maximale zoom level.

### Acties

{% include "admin/action/action.md" %}

{% include "admin/action/button-open.md" %}

{% include "admin/action/button-preview.md" %}

{% include "admin/action/button-save.md" %}

### Context menu

Via het uitklapmenu zijn de onderstaande opties beschikbaar.

![](/assets/svg/list.svg "Lijst") **Terug naar lijst**: Terug naar de lijst en de wijzigingen niet opslaan.

![](/assets/svg/delete.svg "Verwijderen") **Verwijderen**: Door in het uitklapmenu te kiezen voor Verwijderen
kun je een {{ page.meta.vars.singular }} verwijderen.

## Een {{ page.meta.vars.singular }} toevoegen

{% include "admin/add.md" %}

## Een {{ page.meta.vars.singular }} verwijderen

{% include "admin/delete.md" %}