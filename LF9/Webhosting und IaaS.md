# Webhosting und IaaS

## Webhosting Control Panel
- Software as a Service
- Administrationsoberfläche für Webanwendungen des Kunden
- Shared Hosting/Webspace

## Technische Anforderungen an Webhosting Control Panel

### Shared Host/eigener VPS
- Aufteilung mehrerer Kunden auf einem Host
- Control Panel auf eigenem VPS/VDS
- Datenhoheit bei Kunden

### Speicher
- Kleine Pakete: 50Gb SSD
- Große Pakete: 1Tb SSD

### Anzahl DB
- Maximale Anzahl Datenbanken = Maximale Anzahl Webanwendungen

### DB-Webzugriff
- Zugriff per Browser

### Auto-Installer
- Integrierter Auto-Installer
- Installationsoptionen für weitere Webanwendungen

### Anzahl Domains
- Eine Domain inbegriffen
- Mehr = größeres Paket

### Anzahl Subdomains
- Kleine Pakete: 100 Subdomains
- Große Pakete: 1.000 Subdomains

### SSL-Zertifikate
- Kostenpflichtige Zertifikate inbegriffen

### Anzahl E-Mail-Adressen
- Paket mit ausreichender Anzahl an E-Mail Adressen
- Zugriff via Webmail, IMAP, SMTP, POP

### FTPS/SSH-Zugang
- FTPS/SSH für Konfigurationen und Updatemanagement
- Ausführung von Reparaturskripten

### DNSSEC
- Abhörsichere DNS-Variante
- Verfügbarkeit abhängig von Top-Level-Domain

### Konfigurierbare DNS Records
- Selbständige Konfiguration von Domains/Subdomains durch Kunden
- Verfügbarkeit der DNS-Felder A, AAAA, MX, CNAME, TXT, SRV und NS

### DDos-Schutz

### Traffic
- Keine Kosten für unbegrenzten Traffic

### IPv6-Adresse

### Anzahl Cron-Jobs
- Jede Webanwendung = Ein Cron-Job
- Mind. Anzahl DBs

### PHP, Python, NodeJS, Ruby
- Vorabprüfung möglicher installierbarer Webanwendungen

### PHP-Version und PHP-Parameter

### Back-Up
- Erstellbarkeit von Webanwendungs-Backups mit Control Panel
- Mögliche Konfiguration externer Storages?

### Verfügbarkeit
- Installation und Lizenzierung von WCPs auf eigenem VPS/VDS oder dediziertem Server
- Eigenes System für Kunden

### Laufzeit
- Übliche Laufzeit zw. 6-12 Monate

### Kosten
- Monatlich + einmalige Einrichtungspauschale


## Infrastructure as a Service
- Steuerung von Rechenzentrum, Speicher, Netzwerk und Virtualisierung über Administrationsoberfläche

## Technische Anforderungen an Server-/Rechenzentrumssoftware

### Hyperkonvergentes Rechenzentrum
- Ausfalltoleranz
- Räumlich verteilte Storage-Lösung
- CEPH (massiv skalierbares verteiltes Speicher- und Dateisystem, SAN als Software)
- Weiterer Storage-Zugriff für VMs

### Webkonsole
- Administration von VMs über Webanwendung

### Paravirtualisierung
- Installation von IO-Treibern in VMs
- Performance durch Direktzugriff auf physikalische Hardware

### Live-Migration
- Konfigurationsänderungen während Laufzeit

### Orchestrierung
- Management von Multi-Cluster-Container-Umgebungen
- Unterstützung von VMs, Containern, Kubernetes

### VM-Hochverfügbarkeit
- Automatisierter Neustart nach Ausfall

### Back-Ups
- Periodisches Sichern von Daten der VMs auf Remote-Storages

### ACLs
- Zugriffssteuerung über Access-Control-Listen

### Aufgabenplanung
- Zeitgesteuerte Ausführung von Aufträgen durch Planungsmodul

### 2FU
- Zwei-Faktor-Authentifizierung bei Login

## GAIA-X Architektur Richtlinien

### Security/Privacy by Design
- Sicherheits- und Datenschutzaspekte haben höchste Priorität bei Design und Implementierung

### Enabling Federation, distribution and decentralisation
- Verteilung, Dezentralisierung und Förderung
- Zusammenspiel der verteilten Architektur
