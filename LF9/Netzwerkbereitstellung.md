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

## Einsatz redundanter Systeme (Redundanz)
- Existenz mehrerer funktional gleicher/vergleichbarer Ressourcen eines technisches Systems
- Keine zwangsläufige Notwendigkeit im Normalbetrieb

### Funktionelle Redundanz
- Mehrfach parallele Auslegung sicherheitstechnischer Systeme
- Gewährleistung von Diensten trotz Ausfall eines Komponenten

### Redundante Datensicherung
- Datensicherung nach Erfordernis redundant

### Räumliche Redundanz
- Räumliche Trennung redundanter Systeme
- Minimierung eines Störungsrisikos

### Organisatorisch diversitäre Redundanz
- Paralleler Einsatz vielfältiger Berater/Hersteller/Analytiker/Monitoringsysteme

## DevOps-Ansatz und -Kultur

### Begriff
- Development (Entwicklung) und Operations (Vor-Ort-Einsatz)
- Arbeitskultur zur Prozessverbesserung in der Softwareentwicklung und Systemadministration
- Agiler Teamansatz - Herausstellung der Bedeutung von Zusammenarbeit zwischen Entwicklung und Betrieb
- Vorgang effizient, automatisiert und mit KI
- Unterschiedliche Entwicklungsbereiche -> unterschiedliche Ausgestaltungen
- Bspw.:
  - DevOps Engineer
  - Cross-Platform DevOps
  - Site Reliability Engineering (SRE)
  - BizDevOps

### DevOps nach dem CALMS-Modell
- C = Kultur (Culture)
- A = Automatisierung (Automation)
- L = Schlank (Lean)
- M = Messung (Measurement)
- S = Austausch (Sharing)

### DevOps-Prinzipien
- Kundenorientiertes Handeln: Bessere Berücksichtigung von Kundenerfahrungen
- Zielorientiertes Handeln: Gemeinsame, agile Verantwortlichkeit
- End-to-End-Verantwortung: Proaktives Handeln im gesamten Projektlebenszyklus
- Funktionsübergreifende flexible Teams und plattformübergreifende (cross-platform) Infrastrukturlösungen
- Ständige Verbesserung: Kontinuierliche Technologieanpassung und -steuerung in Netzwerkbereitstellung
  - Updates, Upgrades, Tests, Monitoring, Case-Management
- Umfassende Standardisierung und Automatisierung
  - Durch Monitoring, Automatisierung und Orchestrierung
 
### DevOps Praktiken
- Kontinuierliche Integration (Continuous Integration)
  - Beschreibung eines kontinuierlichen Prozesses der Softwareentwicklung im Lebenszyklus
  - Automatisierte Übersetzung und Unit-Testing der aktuellesn Softwarequellen aller Entwickler
 
### Kontinuierliche Bereitstellung (Continuous Delivery)
- Schritte zur Bereitstellung von Anwendungssoftware für Kunden
  - Packaging, Releasing, Configuring, Monitoring


## Varianten der Netzwerkbereitstellung

### Architektur-Modelle im Cloud Computing (Webservices)
- Enterprise Architecture (EA)
- Service Oriented Architecture (SOA)
- Service Oriented Enterprise Architecture (SOEA)
- Service Oriented Infrastructure (SOI)
- Service Oriented Enterprise (SOE)
- Service Oriented Management (SOM)

### Konfiguration
- Installation des richtigen Protokolls (TCP/IP) auf den Geräten im Netz
- Eigene IP-Adresse für jedes Gerät
- Zugehörigkeit zur selben Arbeitsgruppe/IP-Adressbereich im Fall von Datenaustausch zwischen Geräten

### Provisionierung
- Verwaltung des Zugriffs auf Daten und Ressourcen
- Bereitstellung für Nutzer (Benutzerkontenverwaltung) und Systeme
- Bereitstellungspakete über Konfigurationsdienstanbieter
- Management von Provisionierungen und Deprovisionierungen über Tools
- SCIM (System for Cross-domain Identity Management) = offener Standard für automatisierte Bereitstellung von Benutzerkonten
- Systemprovisionierung:
  - Einrichtung physischer Hardware in Rechenzentren
  - Installation und Konfiguration von Software, Betriebssystem und Anwendungen
  - Verbindung mit Middleware, Netzwerken und Storage
- Netzwerkprovisionierung:
  - Einrichtung von Netzwerken
  - Zugriff auf Nutzer, Server, IoT und Container
- Nutzerprovisionierung:
  - Identitätsmanagement
  - Überwachung der Zugriffs- und Autorisierungsrechte für E-Mail, Datenbank oder Netzwerkzugriffe
- Serviceprovisionierung:
  - Einrichtung eines Service
  - Verwaltung verbundener Daten
 
### Orchestrierung
- Automatisierte Konfiguration, Verwaltung und Koordinierung von Computersystemen
- Effiziente Aufgabenbewältigung
- Zuweisung von Aufgaben an Prozesse und Dienste
- Steuerung von Abhängigkeiten
- Schaffung einer Gesamtkonzeption diverser Cloud-Umgebungen
- Einsatz von Docker, Kubernetes, ServiceNow, MS Configuration Manager oder Red Hat Ansible

### Automatisierung
- Einsparung manueller Aufgaben
  - Administration von Routern, Switches, Load Balancers, Firewalls
  - Aufwendige Änderungen an Konfigurationen
- Einsatz von Technologien und Verfahren zur Netzwerkautomatisierung
- Ausführung programmierter Skripte im Betriebssystem oder mittels Automatisierungssoftware
- Bspw.:
  - Infrastrukturautomatisierung
  - Cloudautomatisierung
  - Netzwerkautomatisierung
  - IT-Sicherheitsautomatisierung
  - Patch-Management-Automatisierung
