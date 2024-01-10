# DHCP

## Beschreibung und Aufgaben

- Durchführung der Konfiguration von Netzwerkelementen
  - Innerhalb IP-basierter Netzwerke
  - Mögliche Konfigurationen:
    - IP-Adresse
    - Netzwerkmaske
    - DNS-Server
    - Zeitserver
    - Gateways
- Weiterentwicklung des Bootstrap-Protokolls (BOOTP)
- Basis auf Client-Server-Modell
- Protokollablauf in vier Stufen (4-Way-Handshake)
- Einstellungsoptionen:
  - Manuell
  - Automatisch
  - Dynamisch

## Adressvergabeverfahren bei DHCP

### Manuelle Zuordnung (Static Allocation)
- Konfiguration einer Zuordnungsliste von IP- zu MAC-Adresse im Server
- Vorteile:
  - Computer erhalten immer gleiche IP-Adressen
  - Nur bekannte MAC-Adressen erhalten IP-Adressen
- Nachteile:
  - Erforderliche Konfiguration neuer Computer im DHCP-Server
 
### Automatische Zuordnung (Automatic Allocation)
- Konfiguration eines IP-Adressbereichs im DHCP-Server
- Merken und Reservierung von IP-Adressen für MAC-Adressen
- Vorteile:
  - Computer erhalten immer gleiche IP-Adressen
  - Keine erforderliche manuelle Konfiguration neuer Computer
- Nachteile:
  - Adressbereich kann vergeben sein -> Neue Geräte erhalten keine IP-Adressen

### Dynamische Zuordnung (Dynamic Allocation)
- Konfiguration eines IP-Adressbereichs im DHCP-Server
- Keine feste Zuordnung von MAC-Adressen
- **Lease-Time**:
  - Zeit bis Auslaufen einer IP-Adresse nach Vergabe der Konfiguration
  - Acknowledge = Bestätigungssignal des Servers an Client
- **Renewal-Time**:
  - Unicast-Request des Clients zur Verlängerung der Konfiguration
  - Erneuerung der Lease-Time nach Acknowledge des Servers
- **Rebind-Time**:
  - Broadcast-Request des Clients ins Netz zur Bestätigung der Konfiguration durch einen Server
    - Wenn Server abgeschaltet oder ohne Antwort
  - Sonst - Verwerfen der Konfiguration nach Lease-Time und Anfrage nach neuer Konfiguration mit Discover
 
### DHCP-Relay

- Nutzung von DHCP-Konifigurationen ohne Router-Abhängigkeiten
- Weiterleitung von DHCP-Paketen über Relay-Agent im Router

## Möglichkeiten zur Ausfallsicherheit

### Verwendung zweier DHCP-Server
- Aufteilung des Adressbereiches auf beide Server
- Annahme des schnelleren DHCP-Offers von Servern durch Client

### DHCPv6-Failover
- Betrieb zweier DHCP-Server im Aktiv-Passiv-Modus (Hot-Standby-Model)
- Synchronisation des Status zwischen aktiven und passiven Server
- Gleicher Adressbereich als Vergabebereich (Scope)
- Nutzung als Load-Balancing

## DHCPv6

### Stateless Address Auto Configuration (SLAAC)
- Selbstzuweisung eigener IPv6-Adressen für Netzwerkknoten
- Keine Speicherung der Vergabe -> Stateless

### Ablauf
- Zuweisung einer Link Local Address an Netzwerkknoten
- Senden einer Router Solicitation (RS) zum Empfangen eines Router Advertisements (RA) eines Routers
- Erhalten einer globalen Unicast Address durch RA + Gateway und DNS-IP-Adresse
