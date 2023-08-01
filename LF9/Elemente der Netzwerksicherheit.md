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
- 
