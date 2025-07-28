# Changelog v7

## MapGallery webGIS

### 7.6 <small>juli 2025</small>

Deze zomer release bevat belangrijke verbeteringen voor snelheid, stabiliteit en functionaliteit.

🚀 Nieuw

* Ondersteuning voor **ArcGIS REST API**-kaartlagen. Het is nu mogelijk om kaartlagen te gebruiken die via de ArcGIS REST API zijn gepubliceerd. Deze lagen kunnen eenvoudig worden toegevoegd via de beheeromgeving.

* Ondersteuning voor Azure AD-koppeling via het **OAuth2**-protocol
Beheerders kunnen nu zelf een koppeling met Azure Active Directory instellen via het OAuth2-protocol. Dit vereenvoudigt het authenticatieproces en biedt meer flexibiliteit in het gebruikersbeheer. Een uitgebreid stappenplan is beschikbaar in de documentatie.

⚙️ Voor Beheerders

* Beheerders kunnen nu direct een wachtwoord-reset e-mail sturen naar individuele gebruikers vanuit de beheeromgeving.

* Per gebruiker is nu inzichtelijk tot welke gebruikersgroepen deze behoort.

* Voor WMS- en WFS-kaartlagen kan de downloadoptie worden uitgeschakeld, bijvoorbeeld om datagebruik te beperken of rechten te beheren.

* Verbeterde ondersteuning en instellingen voor gebruikersauthenticatie en toegangsbeheer.

🛠️ Opgelost

* De koppeling met Cyclomedia Streetview werkt nu weer correct.

* Legenda’s voor TMS- en Vector Tiles worden nu juist weergegeven in de kaartviewer.

* In het dashboard kunnen statistieken worden gedownload, waarbij automatisch rekening wordt gehouden met de geselecteerde periode.

* Diverse kleine bugfixes en prestatieverbeteringen in de beheeromgeving en kaartviewer.

### 7.5 <small>april 2025</small>

Deze update richt zich voornamelijk op prestatieverbeteringen en het oplossen van bugs. Kaarten laden sneller en er zijn diverse kleine verbeteringen doorgevoerd. Hieronder een overzicht van de belangrijkste wijzigingen:

* Ondersteuning voor **WMS-selecties**: Het is nu mogelijk om selecties te maken op WMS-lagen door een WFS aan de WMS te koppelen. MapGallery haalt vervolgens de geselecteerde gegevens via de WFS op en toont deze in de viewer. Beheerders kunnen eenvoudig via de beheeromgeving een WFS-service koppelen aan een WMS.

* Optimalisatie van **vector data**: Vector data (zoals WFS, GeoJSON of REST API’s) worden nu opgehaald en verwerkt in een aparte worker thread. Dit voorkomt geheugengerelateerde bugs en zorgt voor een stabielere en snellere viewer. Ook het doorzoeken van vector data gebeurt nu op de achtergrond, zonder dat de browser vastloopt.

* **Herlaadknop** bij foutmeldingen in kaartlagen: Wanneer een kaartlaag een foutmelding geeft (bijvoorbeeld door een tijdelijk onbeschikbare externe service), biedt MapGallery nu de mogelijkheid om eenvoudig opnieuw te laden. Door op het woord 'Fout' te klikken, verschijnt bovendien gedetailleerde foutinformatie.

* Verbeteringen in de **legenda**: De legenda toont nu ook WMS-layergroepen, een symbool voor lagen zonder legenda en een standaardafbeelding voor geparametriseerde symbolen.

* Overige **verbeteringen** en **bugfixes**:
    * Bugfix voor RD-coördinaten transformatie
    * Update van de StreetSmart API
    * Correcte volgorde van complexe lijnen in GeoStyler
    * Opgelost hover-issue bij collectie-overzicht
    * Diverse verbeteringen in de donkere modus
    * Algemene stabiliteitsverbeteringen en bugfixes

### 7.4 <small>januari 2025</small>

Deze update richt zich op beter beheer en een aansluiting op donkere modus. Hieronder een overzicht van de belangrijkste
verbeteringen:

* **Donkere modus**: MapGallery ondersteunt nu **donkere modus**, ideaal voor avondgebruik of als je de donkere weergave prettiger vindt. De modus wordt automatisch ingeschakeld wanneer je systeemkleur op 'donker' staat.
* Gebruikers kunnen nu eenvoudig hun **wachtwoord resetten** via de inlogpagina. Bij het inloggen kun je op **‘Wachtwoord vergeten’** klikken om een resetlink per e-mail te ontvangen. Nieuw geregistreerde gebruikers ontvangen automatisch een reset-token tijdens het onboarden, zodat ze direct een wachtwoord kunnen instellen.
* Verbeterde onboarding: Nieuwe gebruikers ontvangen nu een **welkomstmail** met een introductie van MapGallery, een link naar de documentatie en toegang tot ons supportkanaal. Dit helpt nieuwe gebruikers sneller hun weg te vinden in de applicatie.
* Koppeling van **gerelateerde kaartlagen**: Beheerders kunnen nu gerelateerde kaartlagen koppelen aan een Collectie. Deze kaartlagen worden overzichtelijk weergegeven onder de zoekbalk, gegroepeerd in subcategorieën voor snelle toegang.
* Thema-kleur aanpassen: Beheerders kunnen nu de **hoofdkleur van het thema aanpassen** in de beheerinterface. Hierdoor kan MapGallery beter worden afgestemd op de huisstijl van de organisatie.
* Wekelijkse statusmail: Beheerders ontvangen voortaan een **wekelijkse e-mail** met een overzicht van services die mogelijk haperen. Dit helpt bij het sneller opsporen en oplossen van problemen.
* Overige verbeteringen & bugfixes: Verbeterd en overzichtelijker **layer-overzicht** en betere navigatie met browserknoppen (terug/vooruit). Stabiliteitsverbeteringen en diverse bugfixes.

### 7.3 <small>oktober 2024</small>

Deze update richt zich op de integratie en verbetering van de documentatie en het uitbreiden van onze
supportmogelijkheden. Hieronder een overzicht van de belangrijkste verbeteringen:

* Interactieve **Documentatie** op [docs.mapgallery.eu](https://docs.mapgallery.eu): Er is nu uitgebreide documentatie
  van MapGallery beschikbaar. Daarnaast zijn de links
  vanuit MapGallery naar de documentatie contextueel gevoelig. Dit betekent dat je direct wordt doorverwezen naar de
  relevante informatie
  op basis van waar je je in de applicatie bevindt.
* Nieuw **Support** kanaal: We hebben een gloednieuw supportkanaal gelanceerd. Klanten kunnen nu eenvoudig via e-mail
  vragen stellen of verzoeken indienen. Stuur een email naar [support@mapgallery.eu](support@mapgallery.eu) om een
  ticket aan
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
  is en in groepen kan worden georganiseerd.
* **Filteroptie**: Filters kunnen eenvoudig worden toegepast via de locatie-informatie en vanuit de legenda kunnen
  toegepaste filters overzichtelijk worden beheerd.
* Verbeterde **legenda**: De legenda is compacter en intuïtiever. Ingeklapt verschijnt een oogsymbool om kaartlagen
  aan/uit te zetten.
* Flexibele **collecties**: Beheerders kunnen nu aangeven of kaartlagen standaard actief en/of ingeklapt moeten zijn,
  wat zorgt voor een overzichtelijkere layout.
* Geostyler-**stijl genereren**: Met een knop kunnen beheerders eenvoudig een stijl genereren op basis van data, met
  opties voor labels, kleuren en titels in de legenda.
* Kleine verbeteringen: Snellere WFS-data downloads, direct openen van collecties/kaartlagen vanuit beheeromgeving, en
  selectie naar CSV-conversie in een worker.

### 7.1 <small>april 2024</small>

Deze update richt zich voornamelijk op optimalisaties en bugfixes, met snellere kaarten en kleine verbeteringen.

* MapGallery geeft nu betere **informatie** bij **foutmeldingen** van web-services.
* **Foutmeldingen** van services worden nu **gelogd** en zijn zichtbaar in een speciaal tabblad, met details over datum,
  tijd en type fout.
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