---
title: "Wat is MapGallery"
---

MapGallery is een WebGIS-applicatie waarmee je de omgeving in kaart brengt en beter begrijpt. Je bekijkt interactieve
kaarten, vraagt informatie op over locaties en objecten, en deelt of downloadt de gegevens. MapGallery wordt onder
andere gebruikt door gemeenten, provincies, veiligheidsregio's, stedenbouwkundigen en onderzoekers.

Beheerders stellen per omgeving samen welke kaartlagen, collecties en ondergronden beschikbaar zijn. Gebruikers werken
met die kaarten in de browser, zonder extra software te installeren.

### WebGIS

Een WebGIS (webgebaseerd Geografisch Informatiesysteem) gebruikt het internet om geografische gegevens op te slaan,
te tonen, te analyseren en te delen. Kaarten zijn daarbij niet statisch: je kiest zelf welke lagen je ziet, klikt op
objecten voor meer informatie en combineert gegevens uit verschillende bronnen.

## Systeemeisen

MapGallery ondersteunt de **laatste twee hoofdversies** van de gangbare browsers, op desktop, tablet en telefoon:

| Browser         | Desktop | Mobiel en tablet |
|-----------------|:-------:|:----------------:|
| Google Chrome   |   Ja    |  Ja (Android)    |
| Microsoft Edge  |   Ja    |        —         |
| Mozilla Firefox |   Ja    |  Ja (Android)    |
| Apple Safari    |   Ja    | Ja (iOS / iPadOS) |

Gebruik je een oudere versie, dan kan MapGallery werken, maar valt die versie niet onder de ondersteuning. Browsers
die op dezelfde techniek zijn gebouwd, zoals Opera en Samsung Internet, werken meestal ook, maar worden niet officieel
ondersteund.

De browser moet daarnaast twee technieken ondersteunen en toestaan:

- **[WebGL 2](https://get.webgl.org/webgl2/)** voor het tekenen van de kaart, de kaartlagen en de 3D-weergave. Blijft
  de kaart leeg, werk dan je browser bij en controleer of hardwareversnelling aan staat.
- **[Service workers](https://developer.mozilla.org/docs/Web/API/Service_Worker_API)** voor het laden en lokaal
  bewaren (cachen) van kaartgegevens. **Zonder service workers werkt MapGallery niet.** Sommige browsers schakelen
  service workers uit in een privévenster, en organisaties kunnen ze via een beleid blokkeren. Open MapGallery in dat
  geval in een gewoon browservenster of vraag je IT-afdeling om service workers toe te staan voor het adres van
  MapGallery. Zie ook [Cache legen](manual/cache/index.md).

!!! note "Gebruik op tablet en telefoon"
    MapGallery werkt ook op tablets en telefoons. Sommige functies, zoals selecteren met ++shift++ en slepen of
    toetsenbordsneltoetsen, vragen een toetsenbord en muis en zijn daarom alleen op een computer beschikbaar.

Werkt iets niet goed in een van deze browsers? Meld het via [Vragen & Support](questions.md#ondersteuning).
