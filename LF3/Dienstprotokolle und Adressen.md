# Dienstprotokolle und Adressen

## Protokolle
- **ARP** = Adress Resolution Protocol
  - Auflösung von IP-Adressen in MAC-Adressen
  - OSI-Layer 2 und 3
- **DNS** = Domain Name Service
  - Auflösung von Domainnamen in IP-Adressen
  - OSI-Layer 3 und 7
- **DHCP** = Dynamic Host Configuration Protocol
  - Verteilung von IP-Konfigurationen an Clients im Netz
  - OSI-Layer 3
 
## Adressen
- **MAC-Adresse** = OSI-Layer 2
  - 48 Bit Hexadezimalschreibweise mit Trennzeichen zwischen Bytes
  - Bspw.: AA-BB-CC-DD-EE-FF
  - Eindeutige physikalische Interface-Adresse für jedes Netzwerk-Interface
- **IPv4-Adresse** = OSI-Layer 3
  - 32 Bit Dezimalschreibweise mit Punkten zwischen Bytes
  - Bspw.: 10.255.0.1
  - IP-Adresse für jeden Knoten im Netzwerk
- **IPv6-Adresse** = OSI-Layer 3
  - 128 Bit Achtfache Hexadezimalschreibweise mit Doppelpunkten zwischen Wörtern
  - Bspw.: 2001:0123:5678:9ABC:DEF0: 1234:5678:9ABC
  - Eindeutige IPv6-Adresse für jeden Knoten im Netzwerk
- **Ports** = OSI-Layer 4
  - 16 Bit Dezimalschreibweise
  - Bspw.: 30123
  - Adressierung von Applikationen
    - Bspw.: Port 80 = http, Web-Server/Browser

## Aufbau von MAC-Adressen
- 6 Oktette (48 Bits)
- Unterteilung:
  - Herstellererkennung (Vendor-ID/Organisationally Unique Identifier - OUI)
  - Fortlaufende Nummer des Herstellers
- Schreibweise:
  - Byteweise hexadezimal
  - Trennung durch Bindestriche oder Doppelpunkte zwischen Bytes
- Funktionen:
  - 1. Oktett: Bit 0 = Unicast- oder Multicast-Adressierung
               Bit 1 = Globale oder LAN-Adresse
- MAC-Broadcast-Adresse: ff-ff-ff-ff-ff-ff
  - Ansprechen aller Interfaces im Netz
 
## Aufbau von IP-Adressen
- 32 Bits
- Unterteilung:
  - Trennung durch Subnetzmaske
  - Netzwerkanteil
  - Host-Anteil
- Schreibweise:
  - Byteweise dezimal
  - 8-Bit-Blöcke (Werte 0-255)
- Schreibweise Subnetzmaske:
  - CIDR-Schreibweise/Slash-Notation
    - Angabe des Netzanteils als Präfix hinter IP-Adresse
    - Bspw.: 12.13.14.15/16 = 16 Bits als Netzanteil
      - Netzadresse: 12.13.0.0
      - Hostanteil: 0.0.14.15
  - Dotted-Decimal-Notation:
    - Darstellung der Subnetzmaske als IP-Adresse
    - Links Einsen, rechts Nullen
      - Einsen = Netzstellen
      - Nullen = Hoststellen
     
## Einteilung von IP-Adressklassen
- **A = Netze für Großkonzerne**
  - Adressbereich:
    - 0.0.1.0 - 127.255.255.255
  - Subnetzmaske:
    - 255.0.0.0/8
- **B = Netze für Konzerne**
  - Adressbereich:
    - 128.0.0.0 - 191.255.255.255
  - Subnetzmaske:
    - 255.255.0.0/16
- **C = Netze für kleine Unternehmen**
  - Adressbereich:
    - 192.0.0.0 - 223.255.255.255
  - Subnetzmaske:
    - 255.255.255.0/24
- **D = Multicast-Adressen**
  - Adressbereich:
    - 224.0.0.0 - 239.255.255.255
- **E = Forschungszwecke**
  - Adressbereich:
    - 240.0.0.0 - 255.255.255.255
   
### IP-Spezialklassen
- **Localhost/Loopback
  - IP: 127.0.0.0/8
  - Adresse auf sich selbst
- **Net-ID**
  - Host-Bits = 0
  - Net-ID von 10.1.2.3/8 = 10.0.0.0
- **Host-ID**
  - Net-Bits = 0
  - Host-ID von 10.1.2.3/8 = 0.1.2.3
- **Broadcast-ID**
  - Host-Bits = 1
  - Sendung an alle im Netz
  - Broatcast-ID von 10.1.2.3/8 = 10.255.255.255
 
### Private IP-Adressbereiche
- **Class-A**:
  - Adressbereich: 10.0.0.0 - 10.255.255.255
  - Subnetzmaske: 255.0.0.0
  - Anzahl Host-Bits: 24
  - Anzahl Hosts pro Subnetz: 2^24
  - Anzahl vordefinierte Subnetze: 0
- **Class-B**:
  - Adressbereich: 172.16.0.0 - 172.31.255.255
  - Subnetzmaske: 255.255.0.0
  - Anzahl Host-Bits: 16
  - Anzahl Hosts pro Subnetz: 2^16
  - Anzahl vordefinierte Subnetze: 16
- **Class-C**:
  - Adressbereich: 192.168.0.0 - 192.168.255.255
  - Subnetzmaske: 255.255.255.0
  - Anzahl Host-Bits: 8
  - Anzahl Hosts pro Subnetz: 2^8
  - Anzahl vordefinierte Subnetze: 255
