---
title: "Kaartlagen & legenda"
---

# Kaartlagen & legenda

Een kaartlaag is een informatielaag met geografische gegevens die je onafhankelijk van andere kaartlagen aan- en
uitzet. Via het menu **Kaartlagen** voeg je kaartlagen toe. In de **legenda** aan de rechterkant van het scherm heb je
volledige controle over de actieve kaartlagen.

## Het menu Kaartlagen

Klik rechtsboven op **Kaartlagen**. Het getal op de knop geeft het aantal actieve kaartlagen aan.

<!-- SCREENSHOT: layers/layers-menu.png — Kaartlagen-menu: Legenda verbergen, Kaartlaag toevoegen, Lokaal bestand toevoegen, ondergronden -->

| Optie | Functie |
|-------|---------|
| **Legenda verbergen** / **Legenda tonen** | De legenda verbergen of weer tonen, zonder dat de kaartlagen worden gesloten. |
| **Kaartlaag toevoegen** | Het [zoekvenster](../search/index.md) openen op het tabblad Kaartlagen. |
| **Lokaal bestand toevoegen** | Een eigen bestand tijdelijk op de kaart zetten. Zie [Eigen bestanden](import.md). |
| Ondergronden | De actieve ondergrond wijzigen. Zie [Ondergronden](../map/index.md#ondergronden). |

## De legenda

Elke actieve kaartlaag wordt in de legenda weergegeven in een eigen blok, met specifieke opties voor weergave en
interactie.

<!-- SCREENSHOT: layers/legend.png — Legenda met twee kaartlagen en de knoppen per laag -->

- Klik op het **pijltje** om een kaartlaag in of uit te klappen en op het **kruisje** om de kaartlaag te sluiten.
- **Sleep** een kaartlaag om de volgorde van de kaartlagen aan te passen.
- De kleuren en symbolen geven de categorieën binnen de kaartlaag weer. Klik op een **legenda-item** om die categorie
  aan of uit te zetten. Op dezelfde manier zet je labels aan of uit.

### Knoppen per kaartlaag

Onder in elk blok staan de knoppen voor die kaartlaag:

| Knop | Functie |
|------|---------|
| **Info** | De [metadata](metadata.md) van de kaartlaag bekijken. |
| **Zichtbaarheid** (oog) | De kaartlaag tijdelijk verbergen zonder deze volledig te verwijderen. |
| **Filter** | Alleen de objecten tonen die aan bepaalde voorwaarden voldoen. Zie [Filteren](filter.md). De knop is gekleurd als er een filter actief is. |
| **Stijl** (palet) | De weergave van de kaartlaag aanpassen. Zie [Stijl](#stijl). |
| **⋮** | Meer opties: **Gegevens herladen**, **Zoom naar extent** en **Favoriet**. |

- **Gegevens herladen** laadt de gegevens van de kaartlaag opnieuw.
- **Zoom naar extent** zoomt in op het volledige gebied van de kaartlaag. Is er een filter actief, dan zoomt de kaart
  in op het gebied van de gefilterde objecten.
- **Favoriet** markeert de kaartlaag als [favoriet](../favorites/index.md), zodat je snel naar deze kaartlaag
  terugkeert zonder de volledige lijst van kaartlagen te doorzoeken. Deze optie is alleen beschikbaar als je bent
  ingelogd.

### Legenda-opties

Klik op **⋮** bovenaan de legenda om de legenda-opties te openen. Deze gelden voor alle kaartlagen tegelijk:

| Optie | Functie |
|-------|---------|
| **Uitzetten** | Alle actieve kaartlagen in één keer uitzetten. |
| **Aanzetten** | Alle uitgezette kaartlagen weer aanzetten. |
| **Inklappen** | De blokken van alle kaartlagen inklappen. |
| **Uitklappen** | De blokken van alle kaartlagen uitklappen. |
| **Sluiten** | Alle kaartlagen sluiten. |

Met de knop rechts naast **⋮** klap je de volledige legenda in. De kaartlagen blijven daarbij op de kaart staan.

## Stijl

Bij een vectorkaartlaag pas je met de knop **Stijl** de weergave aan. Welke opties beschikbaar zijn, hangt af van het
type kaartlaag.

<!-- SCREENSHOT: layers/style.png — Stijlmenu van een puntlaag (met Clusters en de schuifregelaar voor grootte) -->

| Optie | Functie | Beschikbaar voor |
|-------|---------|------------------|
| **Eenvoudig** | De standaardweergave van de kaartlaag, zonder speciale effecten of aanpassingen. | Alle vectorkaartlagen |
| **Heatmap** | Gegevens weergeven op basis van dichtheid: hoe meer objecten in een gebied, hoe intenser de kleur. Geschikt om concentraties in grote datasets zichtbaar te maken. | Alle vectorkaartlagen |
| **Clusters** | Dicht bij elkaar liggende punten groeperen tot clusters, afhankelijk van het zoomniveau. Zo blijft de kaart overzichtelijk bij veel punten. | Puntlagen |
| **Stijl terugzetten** | Alle aangepaste stijlinstellingen terugzetten naar de oorspronkelijke weergave. | Alle vectorkaartlagen |
| Grootte (schuifregelaar) | De grootte van de symbolen aanpassen. | Puntlagen |
| Transparantie (schuifregelaar) | De transparantie van de kaartlaag aanpassen. | Alle vectorkaartlagen |

Een aangepaste stijl gaat mee als je een [link deelt](../export/index.md#link-kopieren).
