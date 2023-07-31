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

