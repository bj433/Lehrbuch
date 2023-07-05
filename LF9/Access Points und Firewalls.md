# Access Points und Firewalls

## Technische Anforderungen an Access Points

### WiFi 6/WiFi 5
- Spezifikation von WLAN-Standards durch WiFi-Alliance

### WLAN-Geschwindigkeit
- Tatsächlich verfügbarer Datendurchsatz bei WiFi 5 bei 1.733 Mbit/s

### Dual WLAN
- 2,4 GHz oder 5 GHz-Band

### MU-MIMO
- Multiple Input - Multiple Output (MIMO)
- Verfahren zur Nutzung mehrerer Sende- und Empfangsantennen
- Einsatz spezieller Codierungsverfahren zur Erhöhung der Qualität und des Datendurchsatzes drahtloser Verbindungen
- Multi-User-MIMO
  - Mehrere verschiedene Datendurchsätze an mehrere Clients (gleichzeitig)
 
### OFDMA
- Orthogonal Frequency-Division Multiple Access
- Bidirektionale Kommunikation zur Messung genutzter Kanäle
- Effizienzoptimierung der Access Points

### Multi-Gigabit-Ethernet
- Verfügbarkeit mehrerer Gigabit-Ethernet-Ports

### Bridging-Funktion
- Einsetzbarkeit als Bridge

### Stromversorgung über PoE
- Power over Ethernet

### Leistung PoE/PoE+-Ports
- Vermeidung von Portüberlastung

### Ports 10/100/1.000 Base-T, RJ45
- Höherer Datendurchsatz = besser
- 10/100/1.000 = Durchsatz in Mbit/s

### Einsatzbereich
- Eignung für größere Temperaturbereiche bei industriellen Access Points
- Outdoor-Geräte vor Feuchtigkeit geschützt

### Abnehmbare Antennen
- Austauschbarkeit

## Technische Anforderungen an Firewalls
- Software zur Filterung und ggf. Blockierung von Netzwerkverkehr
- Schutz von Netzwerken
- Dedizierte Hardware

### Internet Gateway
- Überwachung von gesamtem Datenverkehr als Gateway
- Paketfilter für UDP/TCP Nachrichten
  - Filterregeln für erlaubte/unerlaubte IP-Absenderadressen, IP-Zieladressen und Ports
- Stateful Paket Inspection zur Speicherung offener Verbindungen
- Deep Paket Inspection zur Analyse und Filterung von IP-Headern
- Firewallkonfiguration über Regeln

### VPN Gateway

### URL-/Inhaltsfilter
- Regelwerk zur Blockierung diverser URLs

### Intrusion Detection
- Erkennung von Abfolgen an Netzwerkpaketen als möglicher Eindringversuch

### Intrusion Prevention (NGFW)
- Abwehr von Eindringversuchen durch Deep Paket Inspection
- Next Generation Firewall

### Viren-, Spam-, Surfschutz

### DDoS Abwehr
- Erkennung und Abwehr von massivem Empfang von Nachrichtenpaketen

### Authentifizierung
- Autorisierungspflicht zur Konfiguration der Firewall

### Quality of Service
- Mögliche Priorisierung von IP-Paketen

### Reporting
- Berichte für Administrator

### SFP/LAN/WIFI/LTE/UMTS
- Anpassung der Hardware Firewall an eingesetztes Netzwerk

### Datendurchsatz

### VPN-/HTTP-Proxy
- Scan und Filterung vertraulicher Daten

