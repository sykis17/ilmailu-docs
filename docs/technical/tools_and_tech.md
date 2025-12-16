# 🛠️ Dokumentaation Työkalut & Tekniikat (Docs-as-Code)

Tämä projekti on toteutettu **Docs-as-Code** -metodologialla. Tämä lähestymistapa varmistaa, että dokumentaatio on yhtä jäsenneltyä, auditoitavissa olevaa ja versioitua kuin itse koodi.

Alla on yhteenveto projektiin käytetyistä teknologioista:

## 1. Versiohallinta ja Julkaisu

| Työkalu | Rooli projektissa | Ammattimainen etu |
| :--- | :--- | :--- |
| **Git** | Kaikkien sisällön muutosten ja historian hallinta. | Mahdollistaa auditoitavuuden ja palautuksen (rollback) mihin tahansa aiempaan versioon. |
| **GitHub** | Etäsäilö (Remote Repository) ja yhteistyöalusta. | Ylläpitää koodin ja dokumentaation versionhallintaa. Koodi on avoinna tarkastelulle. |
| **GitHub Pages** | Dokumentaatioportaalin ilmainen ja nopea julkaisupalvelu. | Mahdollistaa jatkuvan julkaisun (Continuous Deployment) suoraan Git-haarasta (branch). |
| **Personal Access Token (PAT)** | Turvallinen autentikointimenetelmä julkaisun aikana. | Välttää salasanan tallennuksen, mikä on kriittinen tietoturvakäytäntö. |

## 2. Dokumentaatioympäristö

| Työkalu | Rooli projektissa | Ominaisuuksia |
| :--- | :--- | :--- |
| **MkDocs** | **Static Site Generator** (Staattisen sivuston generaattori). | Muuntaa Markdown-tekstit (esim. metar_codes.md) nopeasti puhtaaksi HTML/CSS-portaalin muotoon. |
| **MkDocs Material** | Käyttöliittymä (UI) ja teema. | Tarjoaa responsiivisen, modernin ja ammattimaisen ulkoasun (esim. tumma tila, hakutoiminto). |
| **Markdown** | Sisällön kirjoituskieli. | Kevyt ja helppo koodata. Mahdollistaa **Admonitions** (huomautuslaatikot) ja **Tabs** (välilehdet) jäsennellyn tiedon esittämiseen. |
| **ghp-import** | Automatisoitu julkaisu. | Mahdollistaa yhden komennon (`mkdocs gh-deploy`) julkaisuprosessin. |