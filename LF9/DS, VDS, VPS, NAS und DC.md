# DS, VDS, VPS, NAS und DC

## Technische Anforderungen an Dedicated Server

### Grundlage
- Physikalischer Server (Bare Metal)
- Verbleib in Co-Location im Rack des Providers
- Ausschließliche Hardwarenutzung durch einen einzelnen Kunden

### CPU und Anzahl Kerne
- Intel XEON, AMD EPYC oder AMD Ryzen mit bis zu 32 Cores

### Speicher
- RAM zw. 256Gb und 2Tb
- EEC (Error Correction Code)
  - Reparatur von Bit-Fehlern während Laufzeit
 
### Anzahl IPv4-/IPv6-Adressen/Failover IP
- Eine IPv4/IPv6-Adresse inklusive
- Mögliche Zubuchung weiterer IP-Adressen
- Erreichbarkeit des Servers im Ausfalls-Fall durch Failover-IP

### Reverse-DNS
- Möglicher Einsatz eines Reverse-Proxys

### DDoS-Schutz, Firewall

### vSwitch
- Mögliche Anbindung an VLAN

### Datenübertragungsrate
- Übliche Serveranbindung: 1 GBit/s
- 10 GBit/s möglich

### RAID-Level
- Mögliche Auswahl zw. RAID 1, 2, 5, 6, 10
- Festplattentyp- und größe
- Hardware-/Software-RAID

### Dedizierte GPU
- Bspw. Nvidia Tesla, GeForce GT

### Images/Software

### Import eigener Images
- Startoptionen für eigene iso- oder img-Dateien

### Uneingeschränkter Traffic
- Häufige Traffic-Begrenzung durch Provider
- Ziel: Uneingeschränkter Datenverkehr

### Back-Up
- Nicht inklusive

### KVM
- Keyboard-Video-Mouse
- Remote BIOS-Hardwarekonfigurationen


## Technische Anforderungen an Virtual Dedicated Server

### Grundlage
- Dedizierte Ressourcen eines Bare Metal
- Aufteilung von Hardware mit anderen Kunden
- Exklusive Ressourcenzuweisung an einen Kunden

### Anzahl Kerne
- CPU-Kern-Anzahl durch Kunden bestimmt
- Unterscheidung physikalische CPU-Kerne/vCPUs
- CPU - Hyperthreading = Ein Kern -> zwei vCPUs
- vCPU = Ein Kern

### Speicher
- Max. 64Gb Hauptspeicher

### NVMe-SSD/SSD
- SSD zubuchbar

### Datenübertragungsrate
- 100 MBit/s eingeschränkte nutzbare Bandbreite

### Uneingeschränkter Traffic

### Images/Software

### Import eigener Images

### Back-Up


## Technische Anforderungen an Virtual Private Server

### Grundlage
- Anmietung einer VM
- Webbasiertes Control Panel
- Aufteilung von vorhandenen physikalischen CPU-Kernen auf mehrere Kunden

### Anzahl vCPU
- Keine exklusive Vergabe von virtualisierten Kernen
- Überprovisionierung durch Provider
  - Buchung einer 25% höheren Anzahl an CPUs durch Shared Hosting
 
### Speicher
- Größe des Hauptspeichers in Gb

### SSD
- Größe des Festplattenspeichers in Gb
- NVMe-SSD = höhere Datenrate

### Datenübertragungsrate
- Netzwerk-Ports gedrosselt
- Bspw.: 200 MBit/s

### Uneingeschränkter Traffic

### Images/Software

### Import eigener Images

### Back-Up-Speicher
- FTP-Speicher
- Nötig für tägliche Serversicherungen (Konfigurationsdateien, Datenbankexporte, etc.)


## Technische Anforderungen an Network Attached Storage

### Grundlage
- Dateiserver im eigenen Netzwerk
- Differenzierung: Rechenzentrum - Kleinst-/Mittel-Netzwerke
- Rechenzentrum: Optimierung auf höchste Schreib-, Lese- und Übertragungsraten
- Kleinst-/Mittel: Integrierter Webserver und Betrieb von Serveranwendungen und virtuellen Maschinen

### Bauform
- 19-Zoll-Gehäuse für Rack-Montage oder Mini-Tower

### Kapazität
- Max. Anzahl SSD-Datenträger
- Max. Gesamtkapazität

### Verschlüsselungsmodul
- Unterstützung von Verschlüsselung durch Hardware

### Schreib- und Lesegeschwindigkeit
- Geschwindigkeit in Megabytes pro Sekunde

### RAID Level
- Hardware-RAID zur Ausfallsicherheit
- Laufwerkwechsel während Laufzeit

### Filesystem
- Bspw.: OpenZFS = Storage-System inkl. Dateisystem, Volume Manager, Snapshots, Copy-on-Write-Klones, Remote Replication, Raid-Z

### Netzwerkanbindung
- Anbindung über Gigabit-Ethernet
- Erhöhung des Datendurchsatzes über Link-Aggregation (Parallele Nutzung mehrerer Netzwerk-Ports)

### Redundantes Netzteil
- Ausfallsicherheit

### VM-Unterstützung
- Weboberfläche zur Einrichtung von VMs auf NAS
- Zusätzlicher Betrieb anderer Interfaces und Software


## Technische Anforderungen an Rechenzentren

### LWL-Verkabelung
- Verkabelungssysteme mit Lichtwellenleiter (Singlemode/Multimode)
- Mehrfaser-Steckverbinder MTP/MPO
- Transceiver
- Aktiver Netzwerkkomponenten für gegebenen Standard (Bspw.: 400 GBase-SR8)

### Kupferverkabelung
- 10-GBase-T-SSTP-Kupferkabel (CAT7/CAT6a)

### KVM-Konsole
- 19-Zoll-KVM (Keyboard Video Mouse) Konsole zur Bedienung mehrerer Server

### Server-Hardware

### Server-Software
- Mögliche technische Einrichtung von VDS, VPS, Webhosting und Dedicated Server
- Kundenspezifische Bereitstellung

### USV
- Gesamtleistung und Scheinleistung aller Server dürfen Ausgangsleistung der USV nicht überschreiten
- Zeit und Dauer der möglichen Stromzufuhr
- Signal für Herunterfahren der Server im Falle eines niedrigen Akkustandes
  - Signalisierung über RS232, USB oder UTP
 
### Wärmerückgewinnung
- Flüssigkühlung zur effizienten Wärmenutzung
  - Hohe Abflusstemperaturen zur weiteren Nutzung
