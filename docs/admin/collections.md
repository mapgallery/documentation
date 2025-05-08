---
title: "Collecties"
description: "Collecties"
vars:
  plural: 'collecties'
  singular: 'collectie'
---

Een collectie bestaat uit één of meerdere [kaartlagen](../layers/) die gezamenlijk een specifiek onderwerp of thema
visualiseren. Door gebruik te maken van een collectie kunnen thema's of onderwerpen onder de aandacht worden gebracht,
geanalyseerd en gedeeld met een breder publiek. Dit maakt een collectie een krachtig hulpmiddel voor communicatie,
onderzoek en besluitvorming. Beheerders kunnen bovendien zelfgemaakte collecties beheren en gebruikers toegang verlenen
tot deze collecties.

{% include "admin/navigate-1.md" %}

2. Selecteer **Dashboard** uit het menu en ga naar de sectie **{{ page.meta.vars.plural }}**.
   {% include "admin/navigate-2.md" %}

## Lijstweergave

{% include "admin/overview/intro.md" %}

| Naam           | Beschrijving                                                                                         |
|----------------|------------------------------------------------------------------------------------------------------|
| `Id`           | Uniek identificatienummer van de {{ page.meta.vars.singular }}.                                      |
| `Datum`        | Datum waarop de {{ page.meta.vars.singular }} is toegevoegd of voor het laatst is bewerkt.           |
| `Naam`         | De naam van de {{ page.meta.vars.singular }}.                                                        |
| `Toegang`      | Toont of de {{ page.meta.vars.singular }} publiek toegankelijk is alleen voor specifieke gebruikers. |
| `Verborgen`    | Geeft aan of de {{ page.meta.vars.singular }} verborgen is voor gebruikers.                          |
| `Omschrijving` | Een korte uitleg over wat de {{ page.meta.vars.singular }} inhoudt.                                  |

### Acties

{% include "admin/overview/action.md" %}

{% include "admin/overview/filter.md" %}

{% include "admin/overview/button-add.md" %}

### Context menu

{% include "admin/overview/context-intro.md" %}

{% include "admin/overview/context-ed.md" %}

## Bewerkingsscherm

Via het bewerkingsscherm worden alle relevante details van een **{{ page.meta.vars.singular }}** weergegeven en kunnen
kunnen de instellingen
worden gewijzingd.

### Bewerkingsopties

Bovenaan de pagina zijn de tabbladen [**Algemeen**](#tabblad-algemeen), [**Kaartlagen**](#tabblad-kaartlagen) en [*
*Gerelateerd**](#tabblad-gerelateerd) voor verschillende instellingen
van de {{ page.meta.vars.singular }}.

#### Tabblad Algemeen

Bevat de belangrijkste instellingen van de {{ page.meta.vars.singular }} (zoals hieronder beschreven). Velden met een *
zijn verplicht.
Uitleg van de Velden:

- **Verbergen**: Wanneer deze optie is aangevinkt, wordt de collectie niet getoond in het overzicht voor de
  eindgebruikers. De collectie blijft echter wel toegankelijk voor beheerders.
- **Toegang**: Hier kun je de toegankelijkheid van de collectie instellen.
- **Naam**: De naam van de collectie.
- **Notitie**: Hier kunnen eventuele beheernotities worden toevoegen die niet zichtbaar zijn voor de eindgebruikers.
- **Omschrijving**: Een beschrijving van de collectie. Deze omschrijving wordt gebruikt om gebruikers te informeren over
  de inhoud van de collectie.
- **Kaartview**: Selecteer het standaard kaartview voor de collectie, dit is de instelling voor het ingezoomde gebied
  van de collectie.
- **Symbool**: De naam van een optioneel symbool om de collectie visueel te identificeren.
  Zie [https://fonts.google.com/icons](https://fonts.google.com/icons?selected=Material%20Icons%20Outlined) voor alle
  mogelijke symbolen van de iconen set (Material Icons).
- **Zoekwoorden**: Tags om de collectie beter vindbaar te maken. Bijvoorbeeld trefwoorden die gerelateerd zijn aan de
  collectie. Deze kunnen één voor één worden toegevoegd.
- **Classificatie**: Hier kunt u de collectie classificeren binnen specifieke thema's. Deze classificaties helpen
  gebruikers de collectie
  beter te categoriseren en te vinden.

#### Tabblad Kaartlagen

Geeft een overzicht van actieve kaartlagen die aan de collectie zijn gekoppeld. Elke kaartlaag heeft een optie om deze
Inactief of Ingeklapt te maken:

- **Inactief**: Als je het vakje onder "Inactief" aanvinkt, wordt de kaartlaag niet weergegeven op de kaart.
- **Ingeklapt**: Door dit vakje aan te vinken, wordt de kaartlaag standaard ingeklapt weergegeven.

##### Een kaartlaag toevoegen

1. Klik op **Toevoegen**. Een pop-upscherm komt tevoorschijn. ![Toevoegen](/assets/img/button-add.png#right "Toevoegen")

2. Selecteer in het pop-upscherm alle **kaartlagen** die je wilt toevoegen aan de **collectie.** Doe dit door te
   klikken op het vakje voor de **kaartlaag,** zodat er een vinkje in komt te staan.

3. Klik op **OK** rechtsonder in het pop-upscherm om de **kaartlagen** toe te voegen aan de **collectie.** Het
   pop-upscherm sluit automatisch. Door op **Sluiten** te klikken wordt het toevoegen van een kaartlaag aan de
   nieuwe **collectie** afgebroken.

##### De standaard ondergrond veranderen

Onder de lijst van kaartlagen vind je een dropdown-menu met de titel Actieve ondergrond. Kies hier de gewenste
ondergrondkaart, bijvoorbeeld OSM (OpenStreetMap), om de kaartlagen bovenop deze kaart te tonen.

#### Tabblad Gerelateerd

Geeft een overzicht van gerelateerde kaartlagen voor de collectie. Gerelateerde kaartlagen komen als suggestie in beeld
linksboven onder de zoekbalk.

### Acties

{% include "admin/action/action.md" %}

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