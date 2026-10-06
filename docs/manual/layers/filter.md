---
title: "Filteren"
---

# Filteren

Met de filterfunctie zoek je naar specifieke objecten binnen een kaartlaag. De kaart toont dan alleen de objecten die
aan de opgegeven voorwaarden voldoen, bijvoorbeeld alle molens van het type "watermolen". Deze functie is beschikbaar
voor alle vectorkaartlagen.

## Een filter toevoegen

Je voegt op twee manieren een filter toe.

### Via de legenda

1. Klik in de [legenda](index.md#knoppen-per-kaartlaag) op de knop **Filter** van de kaartlaag.
1. Kies onder **Filtering toevoegen** een attribuut, een vergelijking en een waarde. Tijdens het typen van de waarde
   doet MapGallery suggesties op basis van de waarden in de kaartlaag.
1. Klik op **⊕** om de filterregel toe te voegen. Het kaartbeeld wordt direct bijgewerkt.

<!-- SCREENSHOT: layers/filter.png — Filtervenster met ingevulde regels, AND/OR en "Huidige filtering: x van y" -->

### Via Locatie-informatie

1. Klik op een object op de kaart. Het paneel [Locatie-informatie](../location/index.md) wordt geopend.
1. Klik op het filtericoon naast het attribuut waarop je wilt filteren. MapGallery maakt een filter op de waarde van
   dit object.
1. Klik op meer filtericonen om het filter uit te breiden.

## Vergelijkingen

Afhankelijk van het type gegevens gebruik je verschillende vergelijkingen:

| Type attribuut | Vergelijkingen |
|----------------|----------------|
| Tekst | `==` (gelijk aan), `!=` (niet gelijk aan) of `bevat` (bevat de tekst) |
| Getal | `==`, `!=`, `>` (groter dan), `<` (kleiner dan), `>=` (groter dan of gelijk aan), `<=` (kleiner dan of gelijk aan) |

## Actieve filters bekijken en aanpassen

Wanneer de knop **Filter** in de legenda gekleurd is, is er een filter actief. Klik op de knop voor een overzicht van
de actieve filters van die kaartlaag. Hier pas je de filters ook aan:

- **Huidige filtering** toont hoeveel objecten aan het filter voldoen, bijvoorbeeld "87 van 1872".
- Kies boven de filterregels tussen **AND** en **OR** om aan te geven hoe de filterregels worden gecombineerd: een
  object moet aan alle regels voldoen (AND) of aan minstens één regel (OR).
- Klik op het **kruisje** bij een filterregel om die te verwijderen. Verwijder alle filterregels om de filtering op te
  heffen.

## Filters bewaren en gebruiken

- **Favoriet:** markeer de kaartlaag als [favoriet](../favorites/index.md) terwijl het filter actief is. Het filter
  wordt dan mee bewaard.
- **Link delen:** een actief filter gaat mee als je een [link deelt](../export/index.md#link-kopieren).
- **Downloaden:** bij het [downloaden](../export/index.md) van een kaartlaag ontvang je alleen de gefilterde objecten.
- **Zoom naar extent:** deze optie in het **⋮**-menu van de kaartlaag zoomt in op de gefilterde objecten.
