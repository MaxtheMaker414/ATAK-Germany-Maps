# ATAK-Germany-Maps
# WMS MAP Sources and WFS stuff for ATAK CIV
## Written for Wintak, can be used with all TAK Versions
Map storage C:\ProgramData\WinTAK\Imagery
WFS storage C:\ProgramData\WinTAK\WFS

### Map files for Germany with mainly Ortho RGB, IR (DOP), TOPO (DTK) maps


### Stream Gauge Data as a KML Network Link in ATAK is in Germany not posible without an server for kml translation.


#### Solution 1: Switch to WFS Data for implementation of Tide, Gauge, Pegel for flood preparedness. 
At the moment the colour stays green the whole time.
I will change that maybe.
![grafik](https://github.com/user-attachments/assets/7dc2e5af-279a-4be2-8560-fecbec52c6f1)


#### Solution 2: WMS Stream for gauge display
use files from: ATAK-Germany-Maps/Imagery/Wasserstand
![grafik](https://github.com/user-attachments/assets/6c025487-1f0c-4215-b6ab-f4ccc4d47dce)



### How to get Sea Maps for ATAK in Germany:

#### for sea maps
Go to: https://wiki.openstreetmap.org/wiki/MBTiles
use the MBtiles and put them into MAP storage
#### for Inland ENC (Electronic Navigational Chart) WSV
Binnenschifffahrt Karten WMS Server verwenden: https://www.govdata.de/suche/daten/wmts-iencs-der-wsv-tilecache-des-adv-wmts-grid-itzbund
WMS file in Imagery/Standard Imagery
![grafik](https://github.com/user-attachments/assets/aba872d4-a31c-4c8f-bb32-4a66b80ca6b5)

