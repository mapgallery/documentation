# Changelog v7

## MapGallery webGIS

### 7.3 <small>oktober 2024</small>

Deze update richt zich op de integratie en verbetering van de documentatie en het uitbreiden van onze
supportmogelijkheden. Hieronder een overzicht van de belangrijkste verbeteringen:

* Interactieve **Documentatie**op [docs.mapgallery.eu](https://docs.mapgallery.eu): Er is nu uitgebreide documentatie van MapGallery beschikbaar. Daarnaast zijn de links
  vanuit MapGallery naar de
  documentatie contextueel gevoelig. Dit betekent dat je direct wordt doorverwezen naar de relevante informatie
  op basis van waar je je in de applicatie bevindt.
* Nieuw **Support** kanaal: We hebben een gloednieuw supportkanaal gelanceerd. Klanten kunnen nu eenvoudig via e-mail
  vragen stellen of verzoeken indienen. Stuur een email naar [support@mapgallery.eu](support@mapgallery.eu) om een ticket aan
  te maken.
* Verbetering van de **Favorieten**: Het is nu mogelijk om alle kaartlagen uit een groep tegelijkertijd aan de kaart toe
  te voegen. Daarnaast is de interface rustiger en duidelijker geworden.
* Ondersteuning voor **oblique luchtfoto's**: In samenwerking met [Kavel10](https://kavel10.nl/) is
  ondersteuning toegevoegd voor oblique luchtfoto’s. Een beheerder kan via de beheer interface deze optie aanzetten
  door de API token van Kavel10 in te vullen.
* **Styles** in- en exporteren: Er is nu ondersteuning voor het importeren en exporteren van SLD (GeoServer) styles en
  Json (Mapbox of MapLibre) styles. Hierdoor kun je eenvoudig stijlen gebruiken in andere applicaties.
* Kleine verbeteringen: Tekstuele correcties zijn doorgevoerd om de woordkeuze consistenter te maken, wat aansluit bij
  de documentatie, verbeterde omgang met polling voor realtime data, een oplossing voor onterechte Foutberichten in Edge
  browsers, verbeterde stabiliteit en kleinere bugfixes.

### 7.2 <small>juli 2024</small>

Deze update staat in het teken van nieuwe functies en algemene aanpassingen die het werken met MapGallery prettiger
maken.

* **Favorieten**-functie: Gebruikers kunnen nu kaartlagen aan een favorietenlijst toevoegen, die individueel aanpasbaar
  is en
  in groepen kan worden georganiseerd.
* **Filteroptie**: Filters kunnen eenvoudig worden toegepast via de locatie-informatie en vanuit de legenda kunnen
  toegepaste filters overzichtelijk worden beheerd.
* Verbeterde **legenda**: De legenda is compacter en intuïtiever. Ingeklapt verschijnt een oogsymbool om kaartlagen
  aan/uit
  te zetten.
* Flexibele **collecties**: Beheerders kunnen nu aangeven of kaartlagen standaard actief en/of ingeklapt moeten zijn,
  wat
  zorgt voor een overzichtelijkere layout.
* Geostyler-**stijl genereren**: Met een knop kunnen beheerders eenvoudig een stijl genereren op basis van data, met
  opties
  voor labels, kleuren en titels in de legenda.
* Kleine verbeteringen: Snellere WFS-data downloads, direct openen van collecties/kaartlagen vanuit beheeromgeving, en
  selectie naar CSV-conversie in een worker.

### 7.1 <small>april 2024</small>

Deze update richt zich voornamelijk op optimalisaties en bugfixes, met snellere kaarten en kleine verbeteringen.

* MapGallery geeft nu betere **informatie** bij **foutmeldingen** van web-services.
* **Foutmeldingen** van services worden nu **gelogd** en zijn zichtbaar in een speciaal tabblad, met details over datum,
  tijd en
  type fout.
* De beheerknop is verplaatst van de collectiesknop naar de gebruikersknop in de titelbalk, wat beter aansluit bij de
  verwachting van beheerders.
* Het beheer van **gebruikersgroepen** is vereenvoudigd; groepen kunnen worden aangemaakt en gekoppeld aan gebruikers en
  services.
* Kleine verbeteringen: de naam van kaartlagen kan aangepast worden, kaartlagen kunnen direct vanuit een service worden
  toegevoegd, protocolopties staan in een eigen tabblad, en overzichten van collecties en services tonen nu het
  toegangsbeleid.

### 7.0 <small>januari 2024</small>

In 2023 is MapGallery volledig herschreven zodat het werken met geodata aanzienlijk wordt verbeterd. Hier volgt een
beknopte samenvatting:

* Ondersteuning voor **3D-kaarten**: 3D-geodata opent de deur naar talloze nieuwe mogelijkheden om onze wereld beter te
  begrijpen en te plannen. MapGallery is volledig voorbereid op de groeiende beschikbaarheid van 3D-geodata.
* Zoeken op **Metadata**: De nieuwe zoekfunctionaliteit op basis van metadata maakt het vinden van specifieke kaarten
  heel eenvoudig.
* **Classificaties**: In de nieuwe versie van MapGallery kunnen kaartlagen worden geclassificeerd. Hiermee brengt
  MapGallery alle relevante geodata samen in één applicatie.
* **Filteren** op de kaart: Met slechts een paar klikken geodata filteren of de relatie tussen verschillende kaartlagen
  leggen. Vragen als 'geef mij alle defecte brandkranen binnen de gemeente Weesp' worden snel beantwoord met een paar
  eenvoudige stappen.
* **Realtime geodata**: Dit zijn kaarten die continu worden bijgewerkt, zoals verkeersinformatie, energiestoringen of
  P2000-meldingen. Via MapGallery kun je de meest actuele informatie opvragen, die in realtime wordt bijgewerkt.