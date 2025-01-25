# ATAK-Germany-Maps

## WMS MAP Sources and WFS Stuff for ATAK CIV

### Beschreibung
Dieses Repository enthält Informationen und Ressourcen für die Nutzung von WMS- und WFS-Datenquellen in ATAK (Android Team Awareness Kit), insbesondere für Deutschland. Es wurde für WinTAK erstellt, kann jedoch mit allen TAK-Versionen verwendet werden.

**Wichtige Speicherorte:**
- **Map-Speicher:** `C:\ProgramData\WinTAK\Imagery`
- **WFS-Speicher:** `C:\ProgramData\WinTAK\WFS`

### Enthaltene Karten
Karten für Deutschland mit den Schwerpunkten:
- **Orthofotos (RGB, IR - DOP)**
- **Topographische Karten (DTK)**
- [XML files](https://github.com/MaxtheMaker414/ATAK-Germany-Maps/tree/d6de0fd0e9ce697ef930f92f9688798dc5cfe02d/Imagery)

<img src="https://github.com/user-attachments/assets/67d0a789-3cee-47ae-b1bf-e411010a00e3" width="700" />


---

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
