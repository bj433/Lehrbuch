# Planung weiterer Komponenten

## WLAN

### Signalstärke
- Angabe in logarithmischen dBm (Dezibel Milliwatt)
- Sendeleistung: positive Werte
- Empfangsleistung: negative Werte

### WLAN-Signalstärke
- -0 dBm = höchster und bester Wert für Empfang
  - ~ 1 mW Leistung
- -10 dBm - -40 dBm = gute Werte
  - zw. 0,1 mW und 0,001 mW
- -85 dBm - keine stabile Verbindung möglich

### Access Points
- Einrichtung nahe an Netzwerkdosen
- Einsatz mehrerer AP's als Repeater möglich

### Absicherung

#### SSID
- Name des WLAN-Netzes

#### WPA3
- Standard-Verschlüsselungsverfahren für WLAN-Netze
- Perfect-Forward-Secrecy
- Ständige Regeneration von Sitzungsschlüsseln
  - Keine Ableitungen vom Master-Key

#### WPA2 (veraltet)
- Advanced Encryption Standard (AES)
- Diverse Schwachstellen

#### WPA (veraltet)
- WiFi Protected Access
- Nachfolger von WEP

#### WEP (veraltet)

#### WLAN-Schlüssel
- Netzwerkschlüssel für WLAN
- Vergabe durch Administrator

#### WPS
- WiFi Protected Setup
- Vereinfachte Aufnahme neuer Geräte ins WLAN

#### Mesh
- Aufbau eines WLANs durch mehrere Access-Points


## VLAN
- Virtual Local Area Network
- Festlegung logischer Netzwerke in einem LAN
- Ports erhalten VLAN-IDs
- Möglichkeiten:
  - Logische Gruppierung von Netzwerkkomponenten
  - Optimierung des Netzwerkverkehrs
  - Erhöhung der Netzwerksicherheit
  - Priorisierung von Netzwerkpaketen
- Einsatz:
  - Heimarbeitsplätze (Remote Access)
  - Site-to-Site-Anbindungen
  - Anbindung IoT-Geräte
 
## IPsec
- Internet Protocol Security
- Vertraulichkeit, Integrität, Verschlüsselung und Authentifizierung


## Switches

### Spanning Tree Protocol (STP) und Rapid Spanning Tree Protocol (RSTP)
- Identifikation und Deaktivierung kreisender Netzwerkpakete innerhalb eines LANs
- Entstehung durch parallele Wege bei Switches

### Layer-2-Switches
- MAC-Adresse entscheidend für Portwahl bei Paketweiterleitung
- 
