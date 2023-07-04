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
- 32 Bit, Dezimalschreibweise (byteweise als 4 8-Bit Zahlen
  - Bspw.: 192.168.9.97
- OSI Layer 3 Netzwerk-Schicht
- Identifikation von Rechnern
- Parallele Verfügbarkeit mit IPv6 (Dual Stack)

#### IPv6
- 128 Bit, Hexadezimalschreibweise
