---
title: "Applicatie"
description: "Applicatie instellingen"
tags: [ instellingen, configuratie, huisstijl, titel, sso, oauth, oidc ]
vars:
  plural: 'applicatie'
  singular: 'applicatie'
---

Op deze plek configureer je de basisinstellingen van een MapGallery-omgeving. Deze instellingen zijn essentieel voor het
beheer en de functionaliteit van de MapGallery omgeving.

{% include "admin/navigate-1.md" %}

2. Selecteer **Dashboard** uit het menu en ga naar de sectie **{{ page.meta.title }}**.

Bovenin het scherm bevinden zich tabbladen om te wisselen tussen verschillende configuratie onderdelen.

## Algemeen

Het dashboard geeft een overzicht van de huidige status van de MapGallery applicatie.

| Naam                    | Beschrijving                                                                             |
|-------------------------|------------------------------------------------------------------------------------------|
| `Titel`                 | De naam van de omgeving zoals weergegeven in de gebruikersinterface..                    |
| `Organisatie (kort)`    | De afkorting of projectnaam van de organisatie. Wordt o.a. gebruikt bij het tabblad.     |
| `Email adres beheerder` | Het e-mailadres van de hoofdbeheerder. Wordt gebruikt voor systeemmeldingen en contact.. |
| `Kleur`                 | Bepaal de primaire kleur van de gebruikersinterface.                                     |

##### Configuratie

Via deze knop is het mogelijk om de volledige configuratie van MapGallery te exporteren en te importeren.

## SSO

In dit tabblad stel je de authenticatie in voor de MapGallery-omgeving via OAuth2 en/of OpenID Connect (OIDC). Hiermee
koppel je de applicatie aan een externe Identity Provider, zoals Azure Active Directory, voor Single Sign-On (SSO).

| Naam                        | Beschrijving                                                                                                           |
|-----------------------------|------------------------------------------------------------------------------------------------------------------------|
| `Uitschakelen`              | Schakel deze optie in als je de externe authenticatie wilt deactiveren.                                                |
| `Login verplicht`           | Als deze optie is ingeschakeld, is inloggen via de externe Identity Provider verplicht voor toegang tot de applicatie. |
| `Application (client) ID`   | Unieke identificatie van de clientapplicatie, zoals geregistreerd bij de Identity Provider                             |
| `Directory (tenant) issuer` | De URL van de tenant (issuer). Dit is de OAuth/OIDC v2.0 of de OIDC v1.0 endpoint van de Identity Provider.            |

##### Genereer Manifest

Genereert een JSON-manifest dat gebruikt kan worden bij de configuratie van de clientregistratie bij een Identity
Provider (zoals Azure AD).

### Stappenplan: Koppeling MapGallery en Azure AD

Hieronder vind je een stappenplan om MapGallery te koppelen met Azure Active Directory (Azure AD) via een Microsoft
Graph App Manifest.

!!! note "Voorbereiding"
    Zorg voor toegang tot Azure Portal. Je hebt minimaal de rol _Application Administrator_ of _Global Administrator_ nodig
    binnen Microsoft Azure.

#### Stap 1: Nieuwe App-registratie in Azure

* Ga naar: [https://portal.azure.com](https://portal.azure.com)
* Navigeer naar **Microsoft Entra ID** (Azure Active Directory)
* Klik op **Add** en vervolgens **App registration**
* Geef een herkenbare naam op (bijv. MapGallery WebGIS), kies bij _Ondersteunde accounttypen_ de optie **Default
  Directory only**. Je kunt _Redirect URI_ overslaan.
* Klik op **Register**

#### Stap 2: Genereer manifest in MapGallery

Ga in MapGallery naar **Applicatie** > **SSO** en vul de gegevens in.

* Zet eventueel de optie “Login verplicht” aan
* Vul uit het overzicht van de App-registratie in Azure de _Application (client) ID_ en de _Issuer URL_ in. De Issuer URL is
  meestal een endpoint van de Identity Provider met de _Directory (tenant) ID_:
    * OIDC v2.0: [https://login.microsoftonline.com/{tenant-id}/v2.0]()
    * OIDC v1.0: [https://sts.windows.net/{tenant-id}/]()
* Klik op **Genereer Manifest**
* Download het JSON-bestand dat wordt aangemaakt

#### Stap 3: Importeer manifest in Azure

In de App-registratie die je net maakte, ga naar het **Manage** > **Manifest**

* Klik op **Upload**
* Kies het gegenereerde JSON-bestand van MapGallery
* Klik op **Save**

#### Stap 4: Test de SSO-koppeling

* Ga terug naar MapGallery en klik op Opslaan in het SSO-tabblad
* Open MapGallery in een incognito venster of uitgelogde sessie
* Controleer of je wordt doorgestuurd naar het Microsoft login scherm

## Over

Dit tabblad geeft een overzicht van de MapGallery-toepassing, inclusief versie-informatie, links naar
documentatie, support en broncode. Het vermeldt de gebruikte open-source bibliotheken en frameworks, met bijbehorende
licenties. Daarnaast wordt de licentie van de applicatie toegelicht.

