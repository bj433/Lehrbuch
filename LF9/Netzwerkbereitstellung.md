# Netzwerkbereitstellung

## Stichwortsammlung bzgl. Konzeption
### - Virtualisierung, Bare Metal, verwendete und zu verwendende Infrastruktur
  - Eigene Server, Storage, Cloud Computing
- Ausdehnung
  - LAN/WAN/MAN/GAN
- Sicherheitskonzepte und -risiken, Übertragungswege, strukturierte Verkabelung
  - Funk, Kupferkabel, Glasfaser
- Topologien, Einsatz Peer-2-Peer bzw. Client-Server-Konzepte, Datenübertragungsrate, Verschlüsselung
  - Preshared Key, RADIUS
  - VLAN, drahtlos PAN/WLAN, Bluetooth
- Einsatz Netzwerkprotokolle
  - IPv4/IPv6, TCP/UDP, SSL, TLS (Version)
- Schicht-5-7-Protokolle
  - DNS, IMAP, SMTP, HTTPS, SFTP, SSH
- Übertragungsprotokolle
  - TCP/UDP, HTTPS
- Speichernetzwerkprotokolle
  - iSCSI, Fibre Channel, FCoE, NFS, SMB/CIFS, HTTP und NVMe-oF
- Standortübergreifende und -unabhängige Kommunikation
  - VPN-Modelle, Tunneling, IPsec

### - Anforderungen Systemkomponenten
  - Server, Peripheriegeräte, Clients, Storage, Appliance, Virtualisierung, Betriebssysteme, Anwendungen, Sicherheitsaspekte, etc.
  - WAN-Modem (DSL-Modem), Router, Switches, WLAN-Controller, Access Point, Firewall, Loadbalancer, Managed Services
- Anforderungen Netzwerk
  - Bandbreite, Latenz, Verfügbarkeit, Übertragungsmedium, Netzwerksicherheit
- Funktions- und Belastungstest
  - Redundanz/Load Balancing/Mesh
- Netzwerkrelevante Dienste
  - DNS, DHCO, Proxy, Spanning Tree, dynamisches/statisches Routing, VLAN, First Hop Redundancy, QoS
- Anwendungsdienste
  - Echtzeitkommunikation, Mail-Server, Webserver, Groupware, Datenbanken
- Service- und Liefermodelle
  - Cloud Computing und Fog Computing, IaaS, PaaS, SaaS, XaaS

### - Protokolldateien/Monitoring und Dokumentation
  - Ping, Trace Route, Analyse-Tools, Netzwerkmonitoring via SNMP
- Schutzziele bzw. Grundwerte der Informationssicherheit
  - Vertraulichkeit, Authentizität/Integrität, Verfügbarkeit
- Festlegung der Schutzbedarfskategoerien (normal, hoch, sehr hoch)
- Ergebnisse der Schutzbedarfsanalyse und Risikoanalyse
- Zusammenarbeit mit Sicherheitsbeauftragten
- Abstimmung mit ITSM
- Beachtung der BSI-Grundschutzbausteine zur Vernetzung

### - Technische organisatorische Maßnahmen (TOM)
  - Risikoidentifikation
  - Planung von Maßnahmen und Ausfallwahrscheinlichkeitsberechnung
  - Intrusion Detection Systems (IDS) und Intrusion Prevention Systems (IPS)
  - Sicherstellung des Betriebes
    - Elektrotechnisch
      - USV
    - Hardwaretechnisch
      - Redundante Systeme (RAID)
    - Softwaretechnisch
      - Backup
    - Zutrittskontrolle
      - Alarmanlage
      - Videoüberwachung
      - Besucherausweise
    - Zugangskontrolle
      - Gebäude
      - Serverraum
      - Schrank
      - Bildschirmschoner mit Passwortschutz
      - Biometrische Verfahren
      - Magnet- oder Chipkarte
    - Zugriffskontrolle
      - Verschlüsselung von Datenträgern
      - Löschung von Datenträgern
      - User-Management/Rollenkonzept
      - Firewall/Webfilter
      - Portsecurity
      - Log Management
      - Compliance Reports
      - Berechtigungskonzepte
      - Organisationsstrukturen (Zugang, Zutritt, Zugriff)
     
### - Berücksichtigung der 3-2-1-Regel für Backups
  - Drei Kopien aller kritischen Daten sollten mind. auf
  - Zwei unterschiedlichen Medien existieren,
  - Ein Medium davon sollte außerhalb/extern gelagert werden
