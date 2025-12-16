# ✈️ Ilmailun Operatiivisen Tietotaidon Dokumentaatioportaali

Tämä projekti on toteutettu **Docs-as-Code** (Dokumentaatio koodina) -metodologialla. Se toimii teknisenä referenssi- ja koulutusportaalinä ilmailualan kriittisille datalähteille (METAR, TAF, NOTAM) ja operatiivisille työnkululle.

Tämä `README.md` sisältää teknisen yleiskatsauksen ja ohjeet portaalin ylläpitoon ja julkaisuun.

---

## 🛠️ Tekninen Yleiskatsaus

Projekti esittelee osaamista seuraavissa teknologioissa ja prosesseissa:

| Teknologia | Rooli | Avaintaidot |
| :--- | :--- | :--- |
| **MkDocs & Material Theme** | Portaalin generointi staattisiksi sivuiksi. | Sisällön rakenteistaminen, YAML-konfigurointi. |
| **Git & GitHub** | Versiohallinta ja yhteistyö. | Commit-historian hallinta, haaran (branch) hallinta. |
| **GitHub Pages** | Jatkuva julkaisu (Continuous Deployment). | Portaalin ylläpito ja automatisoitu päivitys (`mkdocs gh-deploy`). |
| **Markdown** | Sisällön kirjoituskieli. | Taulukoiden, linkkien ja erikoislohkojen (Admonitions) tehokas käyttö. |

## 🚀 Käyttöönotto ja Julkaisu

### 1. Esivaatimukset

Varmista, että koneellesi on asennettu:
* [Python 3.x](https://www.python.org/downloads/)
* [Git](https://git-scm.com/downloads)

### 2. Ympäristön Asennus

Asenna tarvittavat Python-kirjastot (MkDocs, Material-teema ja julkaisutyökalu):

```bash
pip install mkdocs mkdocs-material ghp-import