# TAF-lentokenttäennusteen purkuopas

TAF antaa tiivistetyn ennusteen tietyille ajanjaksoille lentoasemalla. Tulkinnassa on kriittistä ymmärtää ennustemuutokset (Tempo, Becmg, Fm).

> **Esimerkki TAF-viesti:** `EFHK 151730Z 1518/1618 27010KT 9999 BKN015 BECMG 1520/1522 30015KT SCT008 PROB40 TEMPO 1608/1612 4000 SHSN`

## TAF-koodin Keskeiset Rakenneosat

| Ryhmä | Esimerkki (EFHK) | Selite | Arvot / Merkitys |
| :--- | :--- | :--- | :--- |
| **Voimassaolo** | `1518/1618` | Ennuste on voimassa kuun 15. päivän kello 18:00 UTC alkaen 16. päivän kello 18:00 UTC asti. | DDHH/DDHH |
| **Muutostrendit** | `BECMG 1520/1522` | **Becoming** (Muuttuu): Muutos tapahtuu vakaasti kello 20:00 ja 22:00 välillä. | **BECMG**: Vakaa muutos. **TEMPO**: Väliaikainen muutos. |
| **Todennäköisyys** | `PROB40 TEMPO` | **Probability 40%** (Todennäköisyys 40%): Väliaikainen muutos. | **PROB30/PROB40**: Muutoksen todennäköisyys. |
| **Uusi Ennuste** | `4000 SHSN` | Uudessa ennusteessa näkyvyys 4000 m ja lumisadekuuroja. | Lyhenteet kuten METARissa. |

## Muutostrendien Yksityiskohdat

| Lyhenne | Tarkoitus | Kesto | Esimerkki |
| :--- | :--- | :--- | :--- |
| **BECMG** (Becoming) | Ennustetaan tapahtuvan vakaa ja pysyvä muutos ennusteajan sisällä. | Uusi ennuste on voimassa muutoksen päättymisen jälkeen. | `BECMG 1520/1522` |
| **TEMPO** (Temporary) | Ennustetaan tilapäinen vaihtelu säässä, joka kestää alle tunnin kerrallaan ja yhteensä alle puolet TEMPO-ajanjaksosta. | Muutos on lyhytaikainen. | `TEMPO 1608/1612` |
| **PROBxx** (Probability) | Todennäköisyys sille, että TEMPO-ryhmän muutokset tapahtuvat. | xx = 30 tai 40. | `PROB40` |
| **FM** (From) | Muutos, joka alkaa tarkasti tiettynä ajankohtana (esim. uuden ennusteen alku). | Tarkka alkuaika. | `FM161200` |