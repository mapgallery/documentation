---
title: "MapGallery"
---

MapGallery is een WebGIS-applicatie, gemaakt om de omgeving in kaart te brengen en beter te begrijpen door middel van
interactieve kaarten en locatiegegevens. De applicatie werkt in de browser op desktop, tablet en telefoon, zonder dat
je extra software hoeft te installeren. MapGallery wordt onder andere gebruikt door gemeenten, veiligheidsregio's,
stedenbouwkundigen en onderzoekers.

MapGallery biedt een krachtige en flexibele omgeving voor het werken met geografische informatie. Beheerders stellen
per omgeving samen welke kaartlagen, collecties en ondergronden beschikbaar zijn. Als gebruiker bekijk je deze
kaarten, vraag je informatie op over locaties en objecten, en deel of download je de gegevens.

### WebGIS en web mapping

Webgebaseerde geografische informatiesystemen (WebGIS) gebruiken het internet om geografische gegevens op te slaan,
weer te geven, te analyseren en te delen. Daarmee worden ruimtelijke analyses en kaartvisualisaties toegankelijk voor
een breed publiek.

Een veelgebruikte toepassing van WebGIS is web mapping: het maken, gebruiken en delen van kaarten via het internet.
De kaart is daarbij niet statisch. Je bepaalt zelf welke kaartlagen je ziet, klikt op objecten voor meer informatie en
combineert gegevens uit verschillende bronnen.

## Systeemeisen

MapGallery ondersteunt de **laatste twee hoofdversies** van de gangbare browsers, op desktop, tablet en telefoon:

| Browser         | Desktop | Mobiel en tablet |
|-----------------|:-------:|:----------------:|
| Google Chrome   |   Ja    |  Ja (Android)    |
| Microsoft Edge  |   Ja    |        —         |
| Mozilla Firefox |   Ja    |  Ja (Android)    |
| Apple Safari    |   Ja    | Ja (iOS / iPadOS) |

Een oudere versie kan werken, maar valt niet onder de ondersteuning. Browsers
die op dezelfde techniek zijn gebouwd, zoals Opera en Samsung Internet, werken meestal ook, maar worden niet officieel
ondersteund.

De browser moet daarnaast twee technieken ondersteunen en toestaan:

- **[WebGL 2](https://get.webgl.org/webgl2/)** voor het tekenen van de kaart, de kaartlagen en de 3D-weergave. Blijft
  de kaart leeg, werk dan je browser bij en controleer of hardwareversnelling aan staat.
- **[Service workers](https://developer.mozilla.org/docs/Web/API/Service_Worker_API)** voor het laden en lokaal
  bewaren (cachen) van kaartgegevens. **Zonder service workers werkt MapGallery niet.** Sommige browsers schakelen
  service workers uit in een privévenster, en organisaties kunnen ze via een beleid blokkeren. Open MapGallery in dat
  geval in een gewoon browservenster of vraag je IT-afdeling om service workers toe te staan voor het adres van
  MapGallery. Zie ook [Cache leegmaken](manual/troubleshooting/index.md#cache-leegmaken).

!!! note "Gebruik op tablet en telefoon"
    MapGallery werkt ook op tablets en telefoons. Sommige functies, zoals selecteren met ++shift++ en slepen of
    toetsenbordsneltoetsen, vragen een toetsenbord en muis en zijn daarom alleen op een computer beschikbaar.

Werkt iets niet goed in een van deze browsers? Meld het via [Vragen & Support](questions.md#ondersteuning).
