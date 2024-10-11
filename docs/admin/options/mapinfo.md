---
title: "Locatie info"
description: "Locatie informatie"
vars:
  plural: 'locatie-info items'
  singular: 'item'
---

In deze sectie van de MapGallery beheeromgeving kun je de verschillende locatie-info items beheren. Locatie-informatie
bestaat uit de gegevens die worden getoond wanneer een gebruiker op een specifieke locatie op de kaart klikt. Deze
informatie kan naar wens worden uitgebreid of beperkt door het in- of uitschakelen van bepaalde items.
Zodra geactiveerd, zijn deze instellingen van toepassing op alle collecties binnen de applicatie.

{% include "admin/navigate-1.md" %}
2. Selecteer **Dashboard** uit het menu, kies het menu onder **Opties** (![menu](/assets/svg/access.svg "menu")) en ga
   naar de sectie **{{ page.meta.vars.plural }}**.
{% include "admin/navigate-2.md" %}

## Lijstweergave

{% include "admin/overview/intro.md" %}

| Naam            | Beschrijving                                                                               |
|-----------------|--------------------------------------------------------------------------------------------|
| `Id`            | Uniek identificatienummer van de {{ page.meta.vars.singular }}.                            |
| `Datum`         | Datum waarop de {{ page.meta.vars.singular }} is toegevoegd of voor het laatst is bewerkt. |
| `Naam`          | De naam van de {{ page.meta.vars.singular }}.                                              |
| `Omschrijving`  | Een korte uitleg over wat de {{ page.meta.vars.singular }} inhoudt.                        |
| `Uitgeschakeld` | Info of het item is uitgeschakeld (Ja) en welke actief zijn (Nee).                         |

### Context menu

{% include "admin/overview/context-intro.md" %}

{% include "admin/overview/context-e.md" %}

## Bewerkingsscherm

Via het bewerkingsscherm worden alle relevante details van een **{{ page.meta.vars.singular }}** weergegeven en kunnen
kunnen de instellingen worden gewijzingd.

### Bewerkingsopties

Elke extensie heeft eigen, zelfverklarende instellingen, die daarom buiten beschouwing zijn gelaten. Door de optie
Uitgeschakeld te kiezen kan een {{ page.meta.vars.singular }} worden uitgeschakeld.

### Acties

{% include "admin/action/action.md" %}

{% include "admin/action/button-save.md" %}

### Context menu

Via het uitklapmenu is één optie beschikbaar.

![](/assets/svg/list.svg "Lijst") **Terug naar lijst**: Terug naar de lijst en de wijzigingen niet opslaan.
