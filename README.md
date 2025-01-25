# ATAK-Germany-Maps
WMS MAP Sources and WFS stuff for ATAK CIV

Written for Wintak, can be used with all TAK Versions

Map storage C:\ProgramData\WinTAK\Imagery
WFS storage C:\ProgramData\WinTAK\WFS

Map files for Germany with mainly Ortho RGB, IR (DOP), TOPO (DTK) maps

Stream Gauge Data as a KML Network Link in ATAK is in Germany not posible without an server for kml translation.
Solution: Switch to WFS Data for implementation of Tide, Gauge, Pegel for flood preparedness. 
At the moment the colour stays green the whole time.
I will change that maybe.


How to get Sea Maps for ATAK in Germany:

Go to: https://wiki.openstreetmap.org/wiki/MBTiles
use the MBtiles and put them into MAP storage

for Inland ENC (Electronic Navigational Chart) WSV
Binnenschifffahrt Karten WMS Server verwenden: https://www.govdata.de/suche/daten/wmts-iencs-der-wsv-tilecache-des-adv-wmts-grid-itzbund
