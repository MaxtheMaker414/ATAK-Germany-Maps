# ATAK-Germany-Maps

## WMS MAP Sources and WFS Stuff for ATAK CIV

### Beschreibung
Dieses Repository enthält Informationen und Ressourcen für die Nutzung von WMS- und WFS-Datenquellen in ATAK (Android Team Awareness Kit), insbesondere für Deutschland. Es wurde für WinTAK erstellt, kann jedoch mit allen TAK-Versionen verwendet werden.

<details>
  <summary><strong>Zoom Levels (Meters/Pixel, Scale, Features) [click to collapse]</strong></summary>

### Zoom 3–9

| Zoom | Meters / Pixel | Scale / Level | Typically Visible Features | Preview |
|---:|---:|---|---|:--|
| 3 | 19,568 | Continental | Continents, oceans, coarse coastlines | <img alt="zoom3" src="https://github.com/user-attachments/assets/778bd691-2564-420f-9ba2-777d52d4b45e" width="360" /> |
| 4 | 9,784 | Sub-continental | Large countries, major seas, highly generalized borders | <img alt="zoom4" src="https://github.com/user-attachments/assets/45db9122-8a72-4505-b3fd-6a76931ea82e" width="360" /> |
| 5 | 4,892 | National | Country borders, large regions, major water bodies | <img alt="zoom5" src="https://github.com/user-attachments/assets/976f898e-cec1-4a1b-af5d-8f58a129c94e" width="360" /> |
| 6 | 2,446 | Large regional | States / provinces, mountain ranges, major cities | <img alt="zoom6" src="https://github.com/user-attachments/assets/c1856437-b3dd-4752-919b-f3481dabd5ca" width="360" /> |
| 7 | 1,223 | Regional | Regions, metropolitan areas, primary transport corridors | <img alt="zoom7" src="https://github.com/user-attachments/assets/86c88dcd-ac94-4df4-82e9-95985906ed92" width="360" /> |
| 8 | 611.5 | Large city region | Major cities, highways, large rivers | <img alt="zoom8" src="https://github.com/user-attachments/assets/ed742e3c-4b9a-4fbe-913e-f768b8409208" width="360" /> |
| 9 | 305.8 | Metropolitan area | City outlines, highway interchanges, lakes | <img alt="zoom9" src="https://github.com/user-attachments/assets/117ccf07-aa98-4a16-a46e-ca01908621a4" width="360" /> |

---

### Zoom 10–20

| Zoom | Meters / Pixel | Scale / Level | Typically Visible Features | Preview |
|---:|---:|---|---|:--|
| 10 | 152.9 | City overview | Large cities, expressways, rail corridors | <img alt="zoom10" src="https://github.com/user-attachments/assets/d28b73e8-5420-450e-9820-c20920d59195" width="360" /> |
| 11 | 76.4 | City | Districts, main roads, industrial areas | <img alt="zoom11" src="https://github.com/user-attachments/assets/ecc4b83d-677e-483e-8d1d-17281a8c6ac3" width="360" /> |
| 12 | 38.22 | Detailed city | Complete street network, parks, water features | <img alt="zoom12" src="https://github.com/user-attachments/assets/4d0e4b0c-a65b-48c1-ba1f-583654372357" width="360" /> |
| 13 | 19.11 | Neighborhood | Blocks, side streets, plazas | <img alt="zoom13" src="https://github.com/user-attachments/assets/a3e41ac6-0e52-43ef-8560-3dc525b06cb6" width="360" /> |
| 14 | 9.56 | Quarter | Fine street network, green spaces, small waterways | <img alt="zoom14" src="https://github.com/user-attachments/assets/80192203-7285-4b80-aa32-08ac2d6edde2" width="360" /> |
| 15 | 4.78 | Neighborhood detail | Individual buildings, simplified parcel shapes | <img alt="zoom15" src="https://github.com/user-attachments/assets/b191f62f-12c9-446e-909b-c18452097770" width="360" /> |
| 16 | 2.39 | Building level | Building outlines, driveways, small paths | <img alt="zoom16" src="https://github.com/user-attachments/assets/5e0ebceb-20b4-4148-909a-c08c5e1a2fd7" width="360" /> |
| 17 | 1.2 | Fine detail | Building shapes, narrow paths, small objects | <img alt="zoom17" src="https://github.com/user-attachments/assets/c4840427-0af5-46b6-8dad-cd18fc60923e" width="360" /> |
| 18 | 0.5972 | Very fine detail | Curbs, highly accurate buildings, walls | <img alt="zoom18" src="https://github.com/user-attachments/assets/660bb39b-8992-4260-b984-7d73b076d4ab" width="360" /> |
| 19 | 0.2986 | Surveying | Smallest structures, exact edges, detail objects | <img alt="zoom19" src="https://github.com/user-attachments/assets/30a6f08c-12c3-4a74-8dca-f70653e093c4" width="360" /> |
| 20 | 0.1493 | High-precision analysis | Extremely fine surface and object structures | <img alt="zoom20" src="https://github.com/user-attachments/assets/2cf5e37c-dea7-4049-b9b1-fd485db94eae" width="360" /> |

</details>

**Wichtige Speicherorte:**
- **Map-Speicher:** `C:\ProgramData\WinTAK\Imagery`
- **WFS-Speicher:** `C:\ProgramData\WinTAK\WFS`

### Enthaltene Karten
Karten für Deutschland, sortiert nach Bundesländern, mit den Schwerpunkten:
- **Orthofotos (RGB, IR - DOP)**
- **Topographische Karten (DTK)**
- [Weiterleitung zu XML files](https://github.com/MaxtheMaker414/ATAK-Germany-Maps/tree/d6de0fd0e9ce697ef930f92f9688798dc5cfe02d/Imagery)

<img src="https://github.com/user-attachments/assets/67d0a789-3cee-47ae-b1bf-e411010a00e3" width="700" />


---

**BEI Darstellungsfehlern**
Ändere das Koordinatensystem von 3857 auf 4326
"<coordinatesystem>EPSG:4326</coordinatesystem>"
Ändere die Windows Systemsprache auf Englisch

## Stream Gauge Data in ATAK (Pegelstände)

### Problem
In Deutschland ist die Nutzung von KML-Netzwerkverbindungen für Pegelstandsdaten in ATAK nicht möglich, ohne einen Server für die KML-Übersetzung einzurichten.

### Lösungen

#### **Lösung 1: Nutzung von WFS-Daten**
Verwenden Sie WFS-Daten für die Implementierung von Pegelständen (Tide, Gauge, Pegel) zur Hochwasservorsorge.

- **WFS-Datei:**  
  [Link zur WFS-Datei](https://github.com/MaxtheMaker414/ATAK-Germany-Maps/tree/5be3a87fbc5da0a22208de4e5c35935df1276f86/WFS)

- Aktuell bleibt die Farbdarstellung dauerhaft grün. Dies wird möglicherweise angepasst.  
  <img src="https://github.com/user-attachments/assets/7dc2e5af-279a-4be2-8560-fecbec52c6f1" width="500" />

---

#### **Lösung 2: WMS-Stream für Pegelstandsanzeige**
Verwenden Sie WMS-Datenströme für die Darstellung von Pegelständen.

- **WMS-Dateien:**  
  [Link zu WMS-Dateien](ATAK-Germany-Maps/Imagery/Wasserstand)

- **Wichtige Informationen zu WMS:**  
  [Pegel Online Webservice](https://www.pegelonline.wsv.de/webservice/wmsAktuell)

  <img src="https://github.com/user-attachments/assets/6c025487-1f0c-4215-b6ab-f4ccc4d47dce" width="300" />

---

## Nutzung von Seekarten in ATAK für Deutschland

### **Seekarten (Sea Maps)**  
1. Gehe zu: [MBTiles-Seiten](https://wiki.openstreetmap.org/wiki/MBTiles)  
2. Lade die MBTiles herunter und speichere sie im MAP-Speicher:  
   `C:\ProgramData\WinTAK\Imagery`  
   <img src="https://github.com/user-attachments/assets/76f33f33-1797-476a-8fe9-9a11334b2118" width="500" />

---

### **Binnenschifffahrtskarten (Inland ENC - Electronic Navigational Chart)**  
- Verwenden Sie den **Binnenschifffahrts-WMS-Server**:  
  [WMS-Server-Link](https://www.govdata.de/suche/daten/wmts-iencs-der-wsv-tilecache-des-adv-wmts-grid-itzbund)

- Speicherort: `Imagery/Standard Imagery`  
  <img src="https://github.com/user-attachments/assets/aba872d4-a31c-4c8f-bb32-4a66b80ca6b5" width="500" />
