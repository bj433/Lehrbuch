# Adressierung und Vermittlung

## Vermittlung/Routing von Nachrichten (Layer 3)

### IPv4
- 32 Bit großer Adressraum
- 2^32 mögliche Adressen ~ 4,3 Milliarden Adressen
- Dezimale Darstellung
- Bspw.: 192.168.178.68
- IPsec optional
- Checksummen erforderlich
- NAT erforderlich (Network Address Translation) für zusätzliche Adressen
- Paketgröße: 576 Bytes
- Fragmentierung von Nachrichten möglich wenn Netzwerksegment < Paketgröße

### IPv6
- 128 Bit großer Adressraum
- 2^128 mögliche Adressen = 340 Sextillionen
- Hexadezimale Darstellung, 8 Blöcke á 16 Bit
- Bspw.: fe80::e022:d9bc:318b:1d7a
- IPsec optional
- Keine Checksummen
- IPv6 ohne NAT
- 1280 Bytes
- Keine Fragmentierung von Nachrichten nötig

## Adressierung im Internet Protokoll

### Anwendungsschicht
- OSI-Schichten: 7 Anwendung, 6 Darstellung, 5 Sitzung
- Bspw.: dhcp, dns, ftp, ftps, http, https, imap, ntp, pop3, rtp, sip, scp, sftp, smtp, snmp, socks, ssh, xmpp

### Transportschicht
- OSI-schicht: 4 Transport
- Bspw.: TCP, UDP, TLS, DTLS

### Internetschicht
- OSI-Schicht: 3 Vermittlung
- Bspw.: IP: IPv4/IPv6, IPsec, ICMP, BGP, RIP

### Netzzugang
- OSI-Schichten: 2 Sicherung, 1 Bitübertragung
- Bpsw.: ARP/NDP, PPP, PPPoE, MAC Adresse, Ethernet, Token Ring, Glasfaser, WLAN

## Bitübertragung (OSI Layer 1)

### Ethernet-Kabel

#### UTP (Unshielded Twisted Pair)
- Umgeschirmtes Kabel
- Fast- und Giga-Bit-Ethernet
- CAT5e-Kabel

#### STP (Shielded Twisted Pair)
- Geschirmtes Kabel
- Adernpaarweise oder gemeinsame Abschirmung möglich

#### S/STP (Screened Shielded Twisted Pair)
- Einzelne UND gemeinsame Abschirmung

#### S/FTP (Screened/Foiled shielded Twisted Pair)
- Folie für Gesamtschirm
- CAT7 und CAT6a-Kabel (10 GBase-T-Verkabelungen)

### WLAN-Standards

#### IEEE 802.11a
- Max. Datenrate bis zu 54 MBit/s im 5 GHz Band

#### IEEE 802.11b
- Max. Datenrate bis zu 11 MBit/s im 2,4 GHz Band

#### IEEE 802.11g 
- Max. Datenrate bis zu 54 MBit/s im 2,4 GHz Band

#### IEEE 802.11n (WI-FI4)
- Max. Datenrate bis zu 289 MBit/s im 2,4 GHz Band
- Max. Datenrate bis zu 600 MBit/s im 5 GHz Band

#### IEEE 802.11ac (WI-FI5)
- Max. Datendurchsatz bis zu 6933 MBit/s

#### IEEE 802.11ax (WI-FI6)
- Max. Datendurchsatz bis zu 9600 MBit/s

## Sicherungsschicht (OSI-Layer 2)
- Sicherung der Nachrichtenübertragung
- Bestimmung der Sendungsabfolge durch CSMA/CD (Carrier Sense Multiple Access/Collision Detection)

## Adressierung (OSI-Layer 3)

### Adressbestandteile

#### MAC
- 48 Bit, Hex-Schreibweise (byteweise)
  - Bspw.: EA-B1-FC-03-2D-0C
- OSI Layer 2 Datalink-Schicht
- Eindeutige Identifikation von Netzwerkkarten im Netz

#### IPv4
- 32 Bit, Dezimalschreibweise (byteweise als 4 8-Bit Zahlen)
  - Bspw.: 192.168.9.97
- OSI Layer 3 Netzwerk-Schicht
- Identifikation von Rechnern
- Parallele Verfügbarkeit mit IPv6 (Dual Stack)
- Aufteilung in Netzadresse (Subnetzmaske 1) und Hostadresse (Subnetzmaske 0)

#### IPv6
- 128 Bit, Hexadezimalschreibweise (bspw. als 8 16-Bit Zahlen)
  - Bpsw.: 2a02:8070:88a3:9d00:b519:89cb:afe1:1561
- OSI Layer 3 Netzwerk-Schicht
- Identifikation von Rechnern
- Aktuelle Umstellung von IPv4 auf IPv6
- Aufteilung in Präfix und Interface Identifier (beide 64 Bit)

#### Portnummer
- 16 Bit, Dezimalschreibweise
  - Bspw.: 43201
- OSI Layer 4 Transportschicht
- Adressierung von Anwendungen und Diensten

#### Ports bekannter Webanwendungen
- 22 = SSH, Secure Shell
- 53 = DNS, Domain Name System
- 67/UDP, 68/UDP = DHCP, Dynamic Host Configuration Protocol
- 80/443 = http/https für statische und dynamische Webseiten
- 161/UDP = SNMP zur Steuerung von Netzwerkkomponenten
- 143 = IMAP, Internet Message Access Protocol, Empfang von E-Mails von Mailservern
- 401 = UPS, Uninterruptable Power Supply
- 445/TCP = Microsofts Windows Freigaben CIFS/SMB (Samba), Mounting/Verbindung von Windows-Laufwerken im Netzwerk
- 546/UDP, 547/UDP = DHCP für IPv6 - kein TCP

### IP Subnetting und virtuelle LANs (VLAN)
- Gliederung von Netzen in Teilnetze
- Effizientere Nutzung von IPv4-Adressräumen
- Erhöhte Sicherheit = Zuordnung beliebiger Hosts in logische Gruppen
- Kommunikation nur zwischen Nutzern im selben VLAN möglich
- VLAN in eigenem Adressbereich, oder aufgeteilte IP-Subnetze pro VLAN
- Benötigte Subnetz-Bits abhängig von VLAN-Größe

### Routing
- Verfahren zum Weiterleiten von Nachrichtenpaketen
- Weiterleitung von Router zu Router

## Transport von Nachrichten (OSI Layer 4)

### Transmission Control Protocol (TCP)
- Auf- und Abbau von Sitzungen
- Zerlegung von Dateien oder Datenströmen der Anwendungen in einzelne Segmente
- Zusammenführung von Segmenten in korrekter Reihenfolge und Wiedererstellung und Übergabe an Anwendungen
- Fehlerbehandlung und Kontrolle
- Einsatz bei E-Mails und Browsing

### User Datagram Protocol (UDP)
- Kein Auf- und Abbau von Sitzungen
- Verschicken der Daten ohne Kontrolle und Rückmeldung
- Einsatz bei Audio- und Videostreaming

## Anwendungsschicht (OSI Layer 5-7)
- Etablierung verschiedener Serverarten Ende der 90er
  - Bspw. Back-up-, Datenbank-, File/Datei-, Druck- und Mailserver
- Webbasierte Anwendungen seit Ende 90er
- Zugriff per Browser
- Webbasierte Anwendung und Administration

### Serverarten

#### Anwendungsserver (Application Server)
- Bspw.: Oracle Java Enterprise Edition (JEE), Microsoft .NET
- Schnelle Entwicklung von Webanwendungen
- Trennung der Algorithmen in Modell, View und Control
- Anwendung des Modell-View-Control-Design-Patterns
  - Parallele Entwicklung von Datenbanktabellen (Modell), grafischen Oberflächen (View) und Geschäftslogiken (Control)
 
#### Load Balancer
- Skalierung von Serveranwendungen
- Einstiegspunkt für Cluster
- Weiterleitung von Pings an variable Server innerhalb eines Clusters

#### Back-Up-Server
- Mehrschicht-Architekturen
- Stand-By-Systeme
- Einsatz bei Ausfall des Hauptsystems

#### Reverse Proxy
- Stellvertreter für Anfragen aus dem Internet
- Verteilung an mehrere interne Server

#### DHCP-Dienst/-Server
- Dynamic Host Configuration Protocol
- Automatische Einbindung von Geräten in bestehende Netzwerke
- Client bezieht IP-Adresse, Netzmaske, Name-Server und Gateway
- DHCPDISCOVER = Broadcast an lokales Subnetz
- DHCPOFFER = DHCP-Server senden vorhandene Angebote zurück (inkl. Netzwerkadresse)
- DHCPREQUEST = Entscheidung für Angebot mit Server-ID des gewählten DHCP-Servers
- DHCPACK = DHCP-Server antwortet mit Konfigurationsparametern
- DHCPNAK = Restart der Konfiguration erforderlich

#### DNS - DynDNS
- Domain Name System
- Arbeit mit Rechnernamen und URLs
- Auflösung über Nameserver
- Betriebssystem sendet DNS-Anfrage an DNS-Server (nächster Router)
- IP-Adressauflösung
- Erstellung eines http-Requests durch aufgelöste IP-Adresse
- Unverschlüsselt = kann im Klartext mitgelesen werden
- Absicherung = DNS over TLS, DNS over HTTPS oder DNS over QUIC
- DNS-Filter = Blacklists vor dem DNS-Server
  - Bestimmung über Ankunft von Anfragen an den Server

#### DynDNS
- Aktualisierung dynamischer IP-Adressen über DynDNS-Server
- Rücksendung von Anfragen an aktualisierte Adresse
