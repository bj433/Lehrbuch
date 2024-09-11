# DNS

## Beschreibung und Aufgaben

- Namensauflösung von IP-Adressen in klare Namen und umgekehrt
- Abgespeicherte hosts.txt mit IP-Adresse - Hostname
  - Durchsuchung der Hosts-Datei vor DNS-Anfrage
- Hierarchisches Datensystem mit Client-Server-Architektur
  - Domänenname = Fully Qualified Domain Name (FQDN) -> Systemhierarchie
  - Trennung durch Punkte
  - Worte = Label
  - Top-Level-Domain (bspw. ".de") am Ende
  - Keine Angabe des Root-Labels (. ) hinter TLD
 
## Abgrenzung FQDN und URL

- Uniform Resource Locator -> Untermenge der Uniform Resource Identifier
- Beschreibung des Orts einer Ressource im Internet
- Aufbau: "<scheme>:<scheme-specific-part>"
- Bspw.: https://datatracker.ietf.org/doc/html/rfc1738
- scheme: https - Protokoll HTTPS
- scheme-specific-part: datatracker.ietf.org/doc/html/rfc1738
  - datatracker.ietf.org = FQDN des Servers
  - /doc/html/rfc1738 = Pfad zum Dokument
- Identifikation des Servers für FQDN durch URL

## Erläuterungen

### DNS-Root-Server
- Oberste Ebene der Hierarchie autoritativer DNS-Server
- Verweise auf DNS-Server der TLD
- 13 Root-Server
  - IP-Adressen fest über Root-Hint in DNS-Resolvern konfiguriert
  - Weltweite Verteilung von DNS-Anfragen über IP-Anycast
 
### Root Hint
- Festgelegte IPv4/IPv6-Adressen für DNS-Root-Server
- Nötige Bekanntheit für DNS-Server zum Stellen von Abfragen

### Autoritativer DNS-Server
- DNS-Informationen unterhalb seiner Hierarchie-Ebene
- Root-Server kennen IP-Adressen der TLD-Server
- TLD-Server kennen IP-Adressen der DNS-Server
- Konfiguration autoritativer DNS-Server mit Zonen-Dateien

### DNS-Cache
- Zwischenspeicherung durchgeführter Abfragen
- Zeitgesteuerte Cache-Leerungen

### DNS-Client
- Endgeräte

### DNS-Resolver
- Weiterleitung von DNS-Abfragen an DNS-Server
- Bspw.: Stub-Resolver -> Weiterleitung von Abfragen an Recursive-Resolver -> Abfrage bei gesamter DNS-Hierarchie
- Nutzung eines Caches = Full-Service-Resolver

### Forward-Lookup
- Abfrage der IP-Adresse zu gegebenen Domänennamen

### Reverse-Lookup
- Abfrage des Domänennamen zu gegebener IP-Adresse

### Forwarder
- Weiterleitung von Anfragen im Fall das ein anderer Server Anfragen nicht selnbst beantworten kann
