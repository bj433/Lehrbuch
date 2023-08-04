# Netzwerkplanung

## Glasfaseranschluss

### FTTB
- Fibre to the Building
- Glasfaseranschluss ins Gebäude
- Kupferkabelanschluss an einzelne Wohnungen

### FTTC
- Fibte to the Curb
- Glasfaseranschluss zum Straßenverteilerkasten/Kabelverzweiger
- Kupferkabelanschluss an weitere Stationen

### FTTD
- Fibre to the Desk
- Glasfaseranschluss bis zur Anschlussdose

### FTTH
- Fibre to the Home
- Glasfaseranschluss ins Gebäude
- Kupferkabelanschluss an weitere Stationen

### Zwangstrennung
- Wöchentliche Trennung der Internetverbindung durch den Provider

### Fest/dynamische IP-Adresse
- Nicht öffentliche IPv4-Adresse
- Öffentliche IPv6-Adresse
- Adressumsetzung über NAT-Gateway für IPv4


## Vernetzung innerhalb einer Etage
- Planung von Leitungen von Netzwerkdose zum Patch-Panel
- Patch-Panel - Switch = unmittelbare Nähe
- RJ45 als Verbindung zwischen Patch-Panel und Switch
- Dimensionierung der nötigen Ports (Kaskadierung, falls mehr gebraucht wird)

### Vernetzung innerhalb eines Gebäudes
- Leitungen von Etagenswitches zum Hauptanschluss
- Zusammenführung innerhalb eines Patch-Panels im Etagenverteiler

## Demilitarized Zone (DMZ)
- Entmilitarisierte Zone des lokalen Netzwerks
- Abschirmung von Servern durch mehrere Firewalls
  - Intranet = eigene Firewall
  - Extranet = Zugang für externe Server
 

## IP-Adressierungsschema

### Netzmaske IPv4
- Netzmaske = Festlegung über zu erreichende Netzwerkkomponenten durch IP-Adressen
- 24 gesetzte Bits = Subnetzmaske 255.255.255.0
- Kurzschreibweise: /24, 8 verbleibende Bits (256 vergebbare Adressen)
- Kleinste und größte Adresse reserviert
- Kleinste Adresse = Netzwerk-Adresse
- Größte Adresse = Broadcast-Adresse
- Beispiele:
  - /32 = nicht nutzbar, 2^0 - 2 = negativ
  - /31 = keine Adressvergabe, 2^1 - 2 = 0
  - /30 = Vergabe von 2 Adressen, 2^2 - 2 = 2
  - /29 = Vergabe von 6 Adressen, 2^3 - 2 = 6
  - /28 = Vergabe von 14 Adressen, 2^4 - 2 = 14
 
### IPv4-Adressen
- Beispiel 1:
  - Adresse: 192.168.178.52/24
    - Netzwerkteil: 192.168.178.0
    - 1. nutzbare IP-Adresse: 192.168.178.1
    - Letzte nutzbare IP-Adresse: 192.168.178.254
    - Host-Adresse: 192.168.178.52
    - Netzwerkadresse: 192.168.178.0
    - Netzwerkmaske: 255.255.255.0
    - Bits: 24
    - Broadcast-Adresse: 192.168.178.255
    - Adressen insgesamt: 256
    - Netzwerk-Range: 192.168.178.0 - 192.168.178.255
    - Nutzbare Range: 192.168.178.1 - 192.168.178.254
- Beispiel 2:
  - Adresse: 192.168.178.52/27
    - Host-Adresse: 192.168.178.52
    - Netzwerkadresse: 192.168.178.32
    - Netzwerkmaske: 255.255.255.224
    - Bits: 27
    - Broadcast-Adresse: 192.168.178.63
    - Adressen insgesamt: 32
    - Netzwerk-Range: 192.168.178.32 - 192.168.178.63
    - Nutzbare Range: 192.168.178.33 - 192.168.178.62
   
### Netzmaske IPv6
- Länge: 128 Bits
- /64 = Netzwerk-Teil - 64 Bits, Interface Identifier (Geräteanteil) - 64 Bits

### IPv6-Adressen
- Beispiel:
  - Adresse: 2a01:c207:3005:3137::1/64
    - Netzwerkteil: 2a01:c207:3005:3137
    - Interface Identifier: 0000:0000:0000:0001
    - Expanded Adresse: 2a01:c207:3005:3137:0000:0000:0000:0001
    - Compressed Adresse: 2a01:c207:3137:1
    - Subnetz Präfix (Maske): 2a01:c207:3137:0:0:0:0/64
    - Adress ID: 0:0:0:0:0:0:0:1/64
    - Präfix-Adresse: ffff:ffff:ffff:ffff:0:0:0:0
    - Präfix-Länge: 64
    - Netzwerk-Range: 2a01:c207:3005:3137:0000:0000:0000:0000 - 2a01:c207:3005:3137:ffff:ffff:ffff:ffff
