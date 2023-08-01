# Elemente der Netzwerksicherheit

## Antiviren-Scanner und Antiviren-Software
- Hohe und schnelle Erkennungsrate
- Großer Leistungs- und Funktionsumfang
  - Security Management
  - Endpoint Security
  - File Server Security
  - Full Disk Encryption
  - Cloudbasierte Sandbox
  - Mail Security
  - Cloud App Security
- Scan aller Programme und Dateien
  - Abgleich mit bekannten Viren und Malware
- Untersuchung von Programmen auf unbekannte Viren und Informationen über verdächtige Aktivitäten

## Patches und Updates
- Sicherheitsupdates (Korrekturlieferungen) nach Entdeckung neuer Schwachstellen
- Aktualisierungspflicht für Admins

## HTTPS bzw. Sicherheitszertifikate für Websites
- Gewährleistung von Kundensicherheit
- Bezug von SSL/TLS Sicherheitszertifikaten über Zertifizierungsstelle des Web-Providers
- Verschlüsselte Datenübertragung

## VPN und Verschlüsselung
- In sich geschlossene, logische Netze auf unterschiedlichen OSI-Schichten
- Tunneling für IP-Datenverkehr
- Vorgeschalteter Reverse-Proxy zur Verteilung eingehender Anfragen
  - Mehrere Server
  - Virenscanner
  - Paketfilter
- Proxy-Server als Zwischenstück für Internet und internes Netzwerk
  - Auslagerung der SSL-Zertifikate
  - Entlastung des Webservers
- Reverse-Proxy-Server zur Verschlüsselung der Kommunikationsschnittstelle

## Netzwerksegmentierung und P-A-P-Struktur
- Klassifizierung und Segmentierung des Unternehmensnetzwerks nach Vertrauenszonen und Sicherheitsrichtlinien
  - Eingegrenzte Zugriffe für User
  - Verkleinerung der Angriffsfläche für Bedrohungen
  - Vereinfachte Zugriffskontrolle
- Unterschiedlicher Schutzbedarf = Verschiedene Netzsegmente
- Unterteilung von Netzsegmenten nach Größe und Anforderungen des Segmentierungskonzepts
- Physische Trennung von Institutionen innerhalb eines VLANs

### P-A-P Struktur
- Paketfilter, proxybasiertes Application Layer Gateway und Paketfilter
- Im Fall besonderer Sicherheitsanforderungen für Netzsegment
- Anschluss des Netzes über Firewall mit P-A-P-Struktur an Internet

### Perimetersicherheit
- Sicherheitsgrenze/-bereich zw. öffentlichen Netz und Privatnetz oder internem Unternehmensnetz
- Realisierung durch Perimeter-Firewalls und VPNs
  - 1. Verteidigungslinie gegen Viren etc.
- Einrichtung weiterer Sicherheitstechnologien in folgenden Sicherheitsleveln

### DMZ (Demilitarized Zone = Entmilitarisierte Zone)
- Netzsegment bestehend an Netzübergängen
- Von innen und außen erreichbar
- Schaffung eines zusätzlichen Sicherheitsbereichs für öffentlich zugängliche Server
- Extern nutzbare Proxys
- Angriff auf DMZ - Unabhängigkeit von interner Firewall

## Firewalls
- Regelung des Datenverkehrs nach vorgegebenen Regeln
- Einrichtung zwischen Unternehmensnetzwerk und externen Netzwerken
- Filterung in verschiedenen OSI-Schichten
  - Paketfilter für Header-Informationen eines Netzwerkpaketes (Schicht 3, 4)
  - Proxy-Firewall/Stateful Inspection für Nutzdaten (Schicht 7)

### Firewall-Arten
- Personal Firewall (Desktop-Firewall als Software)
- Externe Firewall (Netzwerk-/Hardware-Firewall)
- NGFW

### Next-Generation Firewall (NGFW)
- In Hard- oder Software implementiert
- Erkennung gezielter Angriffe
- Durchsetzung von Sicherheitsrichtlinien auf Anwendungs-, Port-, und Protokollebene
- Grundfunktionen:
  - Enterprise-Firewall-Fähigkeiten
  - IPS
  - Anwendungskontrolle
  - Deep-Packet-Inspection-Funktion
  - Überprüfung von TLS-/SSL-verschlüsseltem Datenverkehr
  - Webseitenfilterung
  - QoS-/Bandbreiten-Management
  - Virenschutzprüfung
  - Integration mit Identitätsmanagement (Bspw.: LDAP, Active Directory)
- Integrierbarkeit in Threat Intelligence Services

### Zwei Firewalls
- Frontend-/Perimeter-Firewall für Datenzugriff für DMZ
- Backend-Firewall für Datenzugriff von DMZ ins interne Netzwerk
- Verwendung von verschiedenen Firewalls empfohlen
  - Ungleiche Sicherheitslücken
 
### UTM-Firewalls (Unified Threat Management)
- Gebrauchsfertige Richtlinien
- Verwaltungs- und Reportingtools für Bereitstellung und Verwaltung
- NGFW-Appliances für kundenspezifische Anpassungen von Sicherheitsrichtlinien/manuelle Reporting-/Managementtechniken
- Funktionen:
  - Anti-Virus, Anti-Spyware, Anti-Spam, Netzwerkfirewall
  - Angriffserkennung und -überwachung
  - Inhaltsfilter
  - Vermeidung von Datenlecks
  - Remote-Routing
  - Übersetzung von Netzwerkadressen (NAT)
  - Unterstützung für VPN
 
### Paketfilter
- Einfache Filterung von Datenpaketen anhand von Filterregeln
- DENY oder DROP: Verwerfen unzulässiger Pakete
- REJECT: Erkennung als unzulässig
- FORWARD oder PERMIT: Weiterleitung zulässiger Pakete
- ALLOW oder PASS: Durchlassen zulässiger Pakete

### Proxyfilter
- Verbindung mit Zielsystem
- Weiterleitung von Antworten des Zielsystems an Client

### Content-Filter
- Proxyfilter zur Auswertung von Nutzdaten einer Verbindung
- Sperrung oder Blockieren von Weiterleitungen

### Intrusion Detection Systeme (IDS) und Intrusion Prevention Systeme (IPS)
- Erkennung von Einbruchsversuchen durch Kommunikationsmuster
- IDS erkennt Angriffe
- IPS blockiert Angriffe

### Firewall-Regelwerk
- Umgang mit Netzwerkpaketen

### Application-, Web- und Inhaltskontrolle
- Content-. Spam-, Antiviren-Filter
- Richtlinien-Management

### E-Mail und Datenschutz
- Datenverkehrskontrolle

### Web-Protection
- Erkennung und Beseitigung von Web-Bedrohungen

### Advanced Threat Protection
- Erkennung von Bots und komplexeren Bedrohungen

### Deep Packet Inspection
- Überwachung und Filterung von Datenpaketen zum Header und zum Dateninhalt
- Analyse weitergehender, protokollspezifischer Informationen
- SSL-Deep Packet:
  - Entschlüsselung verschlüsselter Inhalte und Verbindungsdaten
  - Neuverschlüsselung für Clients
 
### Zero-Day- und KI-Schutz, Sandboxverfahren
- Erkennung neuer Bedrohungen
- Verwendung von Machine Learning und Sandboxing

### Benutzeridentitätsmanagement
- Personenauthentifizierung auf Anwendungen und Programmen
- Anwendungsbeschleunigung durch Richtlinien- und Bandbreitenmanagement

### Sicherheits-Gateway
- Reihenweise geschaltete Filterkomponenten
- Unterscheidung Paketfilter - Application Level Gateway
- Network Address Translation durch Paketfilter für IPv4 -> ALG bei IPv6
- Port Address Translation (PAT) und URL-Blockierung

## E-Mail Sicherheit
- Manipulationssichere E-Mail Archivierung
  - Sicherstellung von Compliance-Vorgaben
- Verwendung der Übertragungsprotokolle (POP3S, IMAPS, SMTPS)
- Einrichtung von E-Mail-Security-Gateways zur Blockade von Angriffen
- Installation auf E-Mail-Server, Hardware-Appliance, virtuelle Appliance
- Spamfilter zur Filterung von E-Mail-Absendern (Blacklists)
- Blacklist: Unerwünschte Absender zur Abweisung
- Whitelist: Erwünschte Absender zur Weiterleitung
