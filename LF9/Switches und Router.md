# Switches und Router

## Technische Anforderungen an Switches
- Verbindung von Netzwerksegmenten miteinander
- Weiterleitung von Nachrichten an Empfängerports

### Managed Switches
- Integrierte Webanwendung zur Konfiguration im Browser

### Unmanaged Switches
- Fest konfiguriert
- Keine anpassbaren Parameter

### Quality of Service
- Priorisierung von IP-Traffic per Konfiguration

### Access Control List
- Festlegung von Zugriffsrechten

### 100 GbE/40 GbE/10 GBase-T
- Höhere Datendurchsatzraten -> höherer Preis
- Sehr hohe Datendurchsatzraten mit Glasfaser

### Ethernet/PoE+/Glasfaser
- Unterschiedliche Ports und Datendurchsatzraten in einem Gerät

### Anzahl Ports

### Bauform
- Vorzügig 19-Zoll Bauform für Racks in Rechenzentren

### RJ45/SFP+/QSFP+

### Leistungsaufnahme
- Angabe in Watt pro Port

### Software Defined Networks
- Konfiguration über SDN
- Eignung für virtualisierte Rechenzentren

### RDMA over Converged Ethernet (RoCE)
- Direkter Speicherzugriff auf Switches über Netzwerk
- Reduktion von Latenzen -> Erhöhte Datendurchsatzraten


## Technische Anforderungen an Session Border Controller (SBC)
- Schutz gegen Angriffe durch Session Initiation Protocol (SIP)
- Anrufsentgegennahme und Weitergabe anhand von SIP-Paketen
- Verschlüsselung von VoIP-Gesprächen über TLS oder SRTP

### Anzahl gleichzeitiger Anrufe
- Leistungsbegrenzung
- Festgelegte maximale gleichzeitige Anrufszahl

### Unterstützte Protokolle
- Bspw.: SIP, H.323, IAX (Inter Asterisk eXchange)

### RTP Transcoding
- Technisch unterschiedliche Audioqualitäten
- Aushandlung des Audio-Codec bei Verbindungsaufbau

### Fax Relay
- Unterstützung des T.38-Standards für den Empfang von Fax

### SIP Intrusion Prevention
- Erkennung und Abwehr von Eindringversuchen über SIP

### Schutz vor DDoS
- Erkennung und Abwehr von DDoS-Angriffen über SIP

### Gesprächssicherheit/Verschlüsselung
- Real-Time-Transport-Protocol (RTP)
- Verschlüsselung über SRTP oder IPsec möglich

### Firewall
- Weiterleitung von SIP-Anfragen
- Abwehr anderer Anfragen


## Repeater
- Signalverstärker = Empfang von schwachen Signalen und Weiterleitung als stärkere Signale

## Router
- Weiterleitung von Datenpaketen zwischen unterschiedlichen Netzwerken
  - Verbindung von Netzwerken
- Lenkung des Datenverkehrs mittels Routing-Tabelle
- Identifikation von Ports, Netzen und Broadcast-Domänen

#### Heimrouter
- Verbindung von Heimnetz mit Internet
- Weitere Funktionen
  - Bspw.: Firewall, Access Point, Telefonanlage, Media-Server, Switch, Jugendschutzfilter
 
#### Edge-Router
- Höhere Performance
- Verbindung von Firmennetz mit Internet oder Partnernetz

#### Core-Router
- Höchst performant für Internet Service Provider (ISP)
- Keine anderen Aufgaben
- Verkabelung mit Glasfaser

#### Virtuelle Router
- Verwendung in Software Defined WANs


### Kriterien für SoHo-Router

#### WAN-Interface
- Meistens ein WAN-Interface
  - Bspw.: DSL, Kabel-TV, LTE, Glasfaser
- Multi-WAN-Interfaces
- Erhöhte Verfügbarkeit bei Ausfall einzelner WAN-Interfaces

#### DNS-Server
- Entgegennahme von DNS-Fragen des Netzwerks
- Mögliche Konfiguration der DNS-Serveradresse

#### DHCP-Server
- Dynamische IP-Adressvergabe
- Konfiguration des Adresspools für statische IP-Adressen

#### Proxy-Server
- Cache-Speicher für statische Webseiten aus Internet
- Reduktion des Datenverbrauchs
- Eignung für Volumentarife

#### WLAN-Access-Point
- Nutzung eines Gastnetzes
- Mögliche nächtliche Abschaltung

#### Kindersicherung und Jugendschutzfilter

#### Anzahl Ethernet Ports

#### TK-Anlage

#### NAS-Server
- Integrierter NAS-Server über USB-Anschlüsse
- Mind. USB 3.0 (falls NAS als Sicherung)


### Technische Anforderungen an Router

#### Anzahl 10/100/1000/100G/400G Ports

#### Anzahl QSFP56/QSFP28/SFP/SFP+/RJ45 Ports

#### IPsec
- Einsatzoption als VPN-Router

#### Software defined WAN
- Konfiguration von Router-Regeln

#### CPU/RAM
- Viele Rechenkerne
- Hohe Single-Thread-Leistung und viel RAM = bessere Gesamtperformance

#### M.2-Storage-Größe
- Lokales Logging

#### Anzahl IPsec-Tunnel
- Anzahl möglicher Standortanbindungen

#### SD-WAN-IPsec-Durchsatz

#### Dualpower/PoE
- Höhere Ausfallsicherheit
- Zweite Stromversorgung über Power over Ethernet

#### Anzahl Höheneinheiten

#### Management Cloud
- Bereitstellung einer Cloudanwendung für zentrale Netzwerkkonfiguration
