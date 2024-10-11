---
title: "Cache legen"
---

De geodata worden voor een betere werking van de applicatie opgeslagen in de browser cache storage.
De **browser cache storage** is een tijdelijke opslaglocatie in je webbrowser waar bestanden van websites worden bewaard.
Het doel van de cache is om kaarten sneller te laden, door eerder gedownloade bestanden op te slaan in plaats van ze opnieuw van de server te moeten downloaden.

### Functies van browser cache storage:

* **Snelheid**: Door geodata lokaal op te slaan, kan MapGallery kaartlagen sneller laden wanneer je dezelfde gegevens opnieuw bezoekt.
* **Bandbreedte besparen**: Door hergebruik van eerder gedownloade bestanden bespaar je bandbreedte.
* **Offline toegang**: Wanneer er even geen internet verbinding is kan gedownloade inhoud ook offline bekeken worden.

### Wat wordt opgeslagen in de cache?

* **Vector tiles**: Tiles van TileJSON en MapBox kaartlagen.
* **Raster tiles**: Tiles van TMS, WMTS en XYZ kaartlagen.
* **Vector data**: Vector data van bijvoorbeeld WFS, GeoJSON of REST kaartlagen.

### Cache legen
Het is mogelijk om de cache te wissen. Dit kan nuttig zijn wanneer je problemen ondervindt met verouderde inhoud, of om ruimte vrij te maken op je apparaat.

1. Klik in het [Hoofdmenu (A)](../map/#a-hoofdmenu) op de dropdown knop naast **MapGallery.**
   ![](/assets/img/user-main-menu.png)
1. Klik op de onderste optie **Cache leegmaken.**

Alleen de cache voor MapGallery wordt gewist, gegevens van andere websites en domeinen worden niet gewist.
