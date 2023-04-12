# Datenübertragung und Kenngrößen

## Kenngrößen in der Datenübertragungstechnik

### Datenmenge D
- **Einheit**: Bit, Byte
- **Wert**: Dateigröße

### Zeit t
- **Einheit**: s, Sekunde
- **Wert**: t

### Datenübertragungsrate im Netzwerk C
- **Einheit**: Bit/s, bps oder Byte/s, B/s
- **Wert**: C = Datenmenge pro Zeit = D / t

### Geschwindigkeit v
- **Einheit**: km/h
- **Wert**: V = Strecke pro Zeit = s / t

### Signalgeschwindigkeit c 
- **Einheit**: m/s, km/s 
- **Wert**: c = Strecke pro Zeit = D / t

### Lichtgeschwindigkeit im Vakuum c0 
- **Einheit**: m/s, km/s
- **Wert**: c0 = 2,99792458 * 10^8 m/s

### Verkürzungsfaktor (NVP, Nominal Velocity of Propagation)
- **Einheit**: -
- **Wert**: NVP = c / c0 -- (Kupferleitungen NVP = 0,6 ... 0,85)

### Signalgeschwindigkeit bei Kupferleitungen
- **Einheit**: c = c0 * NVP
- **Wert**: Typischer Wert: 2/3 der Lichtgeschwindigkeit, ca. 2 * 10^8 m/s

### Brechungsindex bei Glasfasern
- **Einheit**: n = c0 / c
- **Wert**: Typischer Brechungsindex des Faserkerns: n = 1,4 ... 1,5

### Signalgeschwindigkeit bei Lichtwellenleitern
- **Einheit**: c = c0 / n
- **Wert**: Typischer Wert: 2/3 der Lichtgeschwindigkeit, ca. 2 * 10^8 m/s

### Bandbreite B
- **Einheit**: Hertz, Hz
- **Wert**: Differenz zwischen oberer und unterer Grenzfrequenz; für die Informationsübertragung verwendeter Frequenzbereich

## Bit / Byte

- Kleinste Informationseinheit der IT
- Werte: 0 und 1
- Formelzeichen: Bit, bit oder b
- bit/s / b/s / bps jeweils für Bit pro Sekunde
- kb für kilobit, kib für kilo-binary
- Byte besteht aus 8 bit
- Formelzeichen: Byte oder B

## Signale auf Netzwerkmedien

- Elektrische Signale über Kupferleitungen
- Lichtsignale über Glasfaserleitungen
- Elektromagnetische Strahlen bei Drahtlosnetzwerken (z.B. WLAN/Wi-Fi, Bluetooth)


##  Datenübertragungsraten üblicher Schnittstellen

### USB 1.0
- **Übertragungsrate**: 12 Mbit/s
- Full Speed (veraltet)

### USB 2.0
- **Übertragungsrate**: 480 Mbit/s
- Hi-Speed

### USB 3.0
- **Übertragungsrate**: 5 Gbit/s
- SuperSpeed

### USB 3.1
- **Übertragungsrate**: 10 Gbit/s
- SuperSpeed+

### USB 3.2
- **Übertragungsrate**: 20 Gbit/s, 40 Gbit/s

### USB 4.0
- **Übertragungsrate**: 40 Gbit/s
- Nachfolger von USB 3.2, nutzt Thunderbolt-Technologie

### Thunderbolt 2 (2013)
- **Übertragungsrate**: 2 * 10 Gbit/s, 20 Gbit/s
- Thunderbolt verwendet "aktive Leitungen", Stecker mit Elektronik zwecks Leitungsanpassung

### Thunderbolt 3 (2015)
- **Übertragungsrate**: 40 Gbit/s

### Thunderbolt 4 (2020)
- **Übertragungsrate**: 40 Gbit/s
- Technische Basis für USB 4.0

### ATA-1 bis ATA-7 (alte Bezeichnung IDE)
- **Übertragungsrate**: 8,3 MByte/s - 133 MByte/s
- Paralleler Festplattenanschluss (veraltet)

### SATA Express
- **Übertragungsrate**: 8 Gbit/s, 16 Gbit/s
- Serieller Festplattenanschluss

### eSATA
- **Übertragungsrate**: 6 Gbit/s
- External SATA

### Small Computer System Interface (SCSI)
- **Übertragungsrate**: 5 MByte/s - 320 MByte/s
- Paralleler Bus für Massenspeicher und Peripheriegeräte

### Serial Attached SCSI (SAS)
- **Übertragungsrate**: 3 Gbit/s - 22,5 Gbit/s
- Serielle SCSI-Schnittstelle, Sternverkabelung

### iSCSI (Internet SCSI)
- **Übertragungsrate**: Abhängig von der LAN-Technik
- SCSI über Ethernet und ICP/IP, ermöglicht Blockzugriff auf entfernte Festplatten im lokalen Netzwerk oder im Internet

### FireWire
- **Übertragungsrate**: 100 Mbit/s - 3,2 Gbit/s
- Externer Bus für Peripheriegeräte, IEEE 1394

### Fibre Channel (FC)
- **Übertragungsrate**: bis 32 Gbit/s
- Aufbau von Speichernetzwerken

### Fibre Channel over Ethernet (FCoE)
- **Übertragungsrate**: Abhängig von der LAN-Technik
- Fibre-Channel-Protokoll über Ethernet übertragen

### Ethernet/LAN
- **Übertragungsrate**: 10 Mbit/s - 400 Gbit/s
- Gängige Netzwerktechnologie

### DSL
- **Übertragungsrate**: 384 Kbit/s - 250 Mbit/s
- WAN-Anbindung über Telefon- oder Kabelfernsehnetz

### ISDN
- **Übertragungsrate**: 64 Kbit/s
- 1 Anschluss = 2 Kanäle = 128 Kbit/s

### V.24/RS232
- **Übertragungsrate**: Max. 115 Kbit/s, typisch 9,6 Kbit/s
- Serielle PC-Schnittstelle


## Übertragungsarten

### Seriell
- Bits werten nacheinander übertragen
- V.24-Schnittstelle, USB, SATA

### Parallel
- Mehrere Bits (z.B. 8, 16, 32) werden gleichzeitig übertragen
- Druckerschnittstelle, PC-System-Busse

### Simplex
- Datenübertragung nur in eine Richtung
- Rundfunk

### Duplex
- Datenübertragung in beide Richtungen

### Halbduplex
- Richtungsumschaltung, Übertragung immer nur in eine Richtung
- Walkie-Talkie

### Vollduplex
- Datenübertragung in beide Richtungen gleichzeitig
- Telefon

### Multiplex
- Mehrere Übertragungskanäle nutzen dasselbe Übertragungsmedium, dieselbe Leitung
- Zeitmultiplex: Kanäle werden zu unterschiedlichen Zeiten das Medium
- Frequenzmultiplex: Kanäle benutzen unterschiedliche Frequenzen
- Wellenlängenmultiplex: Kanäle benutzen unterschiedliche Wellenlängen (Farben)
- Mehrfachausnutzung von Netzwerkressourcen


## Adressierungsarten im Netzwerk

### Unicast
- 1 Sender -> 1 Empfänger
- Einzelansprache

### Multicast
- 1 Sender -> X Empfänger
- Sendung "an alle Router", "an alle Mitglieder der Gruppe xy"

### Broadcast
- 1 Sender -> alle Stationen im Netz
- Spezialfall von Multicast
- "an alle Stationen im Netz: Wer hat die IP-Adresse 1.2.3.4?"

### Anycast
- 1 Sender -> 1 unbestimmter Empfänger einer bestimmten Gruppe
- Verwendet bei Lastverteilung, Rechner mit meister freier Kapazität wird angesprochen

## Zentrale Regel:
Listen Before Talk (LBT) - Erst hören, dann sprechen.
