---
title: "Groepen"
description: "Gebruikersgroepen"
vars:
  plural: 'groepen'
  singular: 'groep'
---

Een groep definiëert verschillende sets van [gebruikers](../users/) die toegang hebben tot specifieke kaartlagen en
collecties.

{% include "admin/navigate-1.md" %}

2. Selecteer **Dashboard** uit het menu, kies het menu onder **Toegang** (![](/assets/svg/access.svg)) en ga
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

### Acties

{% include "admin/overview/action.md" %}

{% include "admin/overview/button-add.md" %}

### Context menu

{% include "admin/overview/context-intro.md" %}

{% include "admin/overview/context-e.md" %}

## Bewerkingsscherm

Via het bewerkingsscherm worden alle relevante details van een **{{ page.meta.vars.singular }}** weergegeven en kunnen
de instellingen
worden gewijzingd.

### Bewerkingsopties

Bovenaan de pagina zijn de tabbladen [**Algemeen**](#tabblad-algemeen) en [**Match**](#tabblad-match) voor verschillende
instellingen
van de {{ page.meta.vars.singular }}.

#### Tabblad Algemeen

Bevat de belangrijkste instellingen van de {{ page.meta.vars.singular }} (zoals hieronder beschreven). Velden met een *
zijn verplicht. Uitleg van de Velden:

| Naam           | Beschrijving                                                                                          |
|----------------|-------------------------------------------------------------------------------------------------------|
| `Naam`         | De naam van de **{{ page.meta.vars.singular }}**.                                                     |
| `Notitie`      | Hier kunnen eventuele beheernotities worden toevoegen die niet zichtbaar zijn voor de eindgebruikers. |
| `Omschrijving` | Een korte uitleg over wat de {{ page.meta.vars.singular }} inhoudt.                                   |

#### Tabblad Match

Via een reguliere expressie kunnen nieuwe gebruikers op basis van een match op e-mailadres of een SAML-claim (het veld
_group_) automatisch aan de juiste groep worden toegekend.

### Acties

{% include "admin/action/action.md" %}

{% include "admin/action/button-save.md" %}

### Context menu

Via het uitklapmenu zijn de onderstaande opties beschikbaar.

![](/assets/svg/list.svg "Lijst") **Terug naar lijst**: Terug naar de lijst en de wijzigingen niet opslaan.

![](/assets/svg/delete.svg "Verwijderen") **Verwijderen**: Door in het uitklapmenu te kiezen voor Verwijderen kun je
een {{ page.meta.vars.singular }} verwijderen.

## Een {{ page.meta.vars.singular }} toevoegen

{% include "admin/add.md" %}

## Een {{ page.meta.vars.singular }} verwijderen

{% include "admin/delete.md" %}