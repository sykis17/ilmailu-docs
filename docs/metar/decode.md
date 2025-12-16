# METAR-koodin purkuopas (Reference Guide)

METAR (Meteorological Aerodrome Report) on standardoitu, koodattu viesti, joka sisältää kriittisiä, reaaliaikaisia säätietoja lentoasemilta. Tämän oppaan tarkoituksena on purkaa koodin osat ja niiden merkitys.

> **Esimerkki METAR-viesti:** `EFHK 151950Z 30010KT 9999 VCSH BKN015CB 01/M01 Q1015 NOSIG`

## Koodin Rakenne ja Tulkinta

| Ryhmä | Esimerkki (EFHK) | Selite | Arvot / Koodit |
| :--- | :--- | :--- | :--- |
| **Asema** | `EFHK` | Lentoaseman ICAO-koodi. | Nelikirjaiminen tunnus (esim. EFHK, KLAX). |
| **Aika** | `151950Z` | Raportin päivä (15.) ja aika (19:50) UTC-ajan (Z) mukaan. | DDHHMMZ |
| **Tuuli** | `30010KT` | Tuulen suunta (300 astetta) ja nopeus (10 solmua). | **VRB**: Vaihteleva tuuli. **GxxKT**: Puuskien nopeus. |
| **Näkyvyys** | `9999` | Vaakanäkyvyys 10 km tai enemmän. | Neljä numeroa metreissä. |
| **Sääilmiöt** | `VCSH` | Lähellä oleva sadekuuro (Vicininity Shower). | **+** voimakas, **TS** ukkonen, **SN** lumi. |
| **Pilvet** | `BKN015CB` | Rikkonainen (Broken) pilvikerros 1500 jalassa. Kummulonimbukset (CB) havaittu. | **FEW/SCT/BKN/OVC**: Peittoaste. **CB**: Kyyhnelpilvi. |
| **Lämpötila/Kastepiste** | `01/M01` | Lämpötila 1 °C, kastepiste -1 °C. | **M**: Miinusasteet (esim. M05). |
| **QNH** | `Q1015` | Merenpinnan tasolle korjattu ilmanpaine (QNH) 1015 hehtopascalia. | Qxxxx (hPa). |
| **Lisätieto** | `NOSIG` | Ei merkittäviä muutoksia ennusteessa (No Significant Change). | Useita lyhenteitä käytössä. |