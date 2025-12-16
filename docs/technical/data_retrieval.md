# 💻 Säädatan Haku ja Käsittely (IoT/Python-projekti)

Dokumentaation ylläpidon lisäksi ymmärrän datan lähteen ja ohjelmallisen käsittelyn. Olen toteuttanut IoT-projektin, jonka tarkoituksena on hakea reaaliaikaista ilmailusäädataa ja käsitellä sitä ohjelmallisesti.

## Prosessi

Tämä projekti demontroi Pythonin kykyä integroitua ulkoisiin lentosääpalveluihin (API) ja esikäsittelyyn ennen operatiivista käyttöä. 

1.  **Datan haku (API Integration):** Käytetään Python-kirjastoja (esim. `requests`) METAR- ja TAF-datan hakemiseen suoraan virallisista lentosääpalveluista (esim. NOAA tai Aviamet).
2.  **Jäsentäminen (Parsing):** Raakakoodi (esim. `EFHK 151950Z 30010KT 9999...`) on jäsennettävä strukturoiduksi dataksi (esim. JSON-objektiksi).
    * **Tulos:** Erottaa Tuulen (Wind), Näkyvyyden (Visibility) ja Pilvisyyden (Clouds) omiksi muuttujikseen.
3.  **Hälytykset ja Visualisointi:** Jäsennelty data voidaan syöttää visualisointialustalle (esim. Grafana) tai käyttää hälytysjärjestelmien luomiseen (esim. ilmoitus, jos näkyvyys laskee alle 5000 metrin).

## Käytetyt teknologiat

| Teknologia | Tehtävä |
| :--- | :--- |
| **Python** | Datan haku ja jäsentämislogiikka. |
| **JSON/XML** | Rajapintojen (API) palauttaman tiedon muoto. |
| **MQTT-protokolla (IoT)** | Reaaliaikaisen datan siirto pilvipalveluun (esim. Azure tai AWS) visualisointia varten. |

Tämä projekti osoittaa kykyni siirtyä dokumentoinnista suoraan tekniseen järjestelmäkehitykseen.