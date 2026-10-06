---
title: "Problemen oplossen"
---

# Problemen oplossen

Op deze pagina vind je de meest voorkomende problemen en de stappen om ze zelf op te lossen. Is je probleem hiermee
niet opgelost, neem dan contact op via [Vragen & Support](../../questions.md).

## De kaart blijft leeg of laadt niet

- Gebruik een [ondersteunde browser](../../application.md#systeemeisen) en werk deze bij naar de nieuwste versie.
- MapGallery maakt gebruik van **service workers**; zonder service workers werkt de applicatie niet. Gebruik geen
  privévenster en controleer bij je IT-afdeling of service workers zijn toegestaan voor het adres van MapGallery.
- De kaart maakt gebruik van **WebGL 2**. Controleer of hardwareversnelling is ingeschakeld in de instellingen van je
  browser.
- Vernieuw de pagina. Is het probleem daarmee niet opgelost, [maak dan de cache leeg](#cache-leegmaken).

## Een kaartlaag toont geen gegevens

- Controleer of de kaartlaag **zichtbaar** is via het oogpictogram in de
  [legenda](../layers/index.md#knoppen-per-kaartlaag).
- Controleer of er een **filter** actief is. In dat geval is de knop Filter gekleurd. Zie
  [Filteren](../layers/filter.md).
- Sommige kaartlagen tonen pas gegevens vanaf een bepaald **zoomniveau**. Zoom verder in of kies **Zoom naar extent**
  in het **⋮**-menu van de kaartlaag.
- Kies **Gegevens herladen** in het **⋮**-menu van de kaartlaag.

## Geen informatie bij een klik op de kaart

- Klik precies op een object van een actieve en zichtbare kaartlaag.
- Niet alle kaartlagen geven informatie bij een klik. Dit hangt af van de bron van de kaartlaag.

## Inloggen lukt niet

- Gebruik **Wachtwoord vergeten?** op het inlogscherm. Zie [Wachtwoord vergeten](../index.md#wachtwoord-vergeten).
- Heb je geen account of is je uitnodiging verlopen, neem dan contact op met de beheerder van MapGallery binnen je
  organisatie.

## Tekeningen zijn niet meer zichtbaar

Tekeningen worden lokaal in je browser opgeslagen. Ze zijn niet beschikbaar in een andere browser of op een andere
computer, en ze worden verwijderd als je de browsergegevens wist. Daarnaast zijn tekeningen alleen zichtbaar als het
paneel Meten & Tekenen is geopend. Zie [Tekeningen bewaren](../draw/index.md#tekeningen-bewaren).

## Cache leegmaken

Voor een betere werking slaat MapGallery geodata op in de cache van je browser. De cache is een tijdelijke
opslaglocatie in je webbrowser waar bestanden van websites worden bewaard. Hierdoor laden kaartlagen sneller wanneer
je dezelfde gegevens opnieuw bekijkt, en bespaar je bandbreedte.

In de cache worden onder andere opgeslagen:

- **Vectortegels** van TileJSON- en Mapbox-kaartlagen;
- **Rastertegels** van TMS-, WMTS- en XYZ-kaartlagen;
- **Vectorgegevens** van bijvoorbeeld WFS-, GeoJSON- en REST-kaartlagen.

Het leegmaken van de cache is nuttig wanneer je problemen ondervindt met verouderde gegevens of ruimte wilt vrijmaken
op je apparaat:

1. Open het [Hoofdmenu](../menu/index.md).
1. Kies **Ondersteuning → Cache leegmaken**.

Alleen de cache van MapGallery wordt gewist. Gegevens van andere websites blijven behouden.
