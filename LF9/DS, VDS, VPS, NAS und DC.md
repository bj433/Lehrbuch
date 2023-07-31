# DS, VDS, VPS, NAS und DC

## Technische Anforderungen an Dedicated Server

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
