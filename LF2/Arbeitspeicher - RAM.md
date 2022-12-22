# Arbeitsspeicher - RAM

## RAM
- Random Access Memory
- Je größer, desto besser
- System arbeitet schneller, mehr aktive Daten verwendbar
- Leistungsfähigkeit abhängig von unterstützer Geschwindigkeit des RAM-Moduls
- Berechnung in Megatransfers pro Sekunde (MT/s)
- Bandbreite - gesamte verarbeitbare Datenmenge des Speichermoduls

## Anforderungen
- Win 10 32-Bit: mind. 1GB 
- 64-Bit: mind. 2GB
- Standard-PC: mind. 4GB
- Anwendung mehrerer Programme: 8GB + 

## JEDEC (Joint Electronic Device Engineering Council)
- Organisation in Zuständigkeit für elektrische und zeitliche Parameter von Speicher-Controllern und Speicherchips
- Vorschreibung bestimmter Chip-Kombinationen
- Sicherstellung der kapazitäts- und herstellerübergreifenden Kompatibilität

## Speichererweiterungen
- Anzahl der freien Speicherbänke auf der Hauptplatine bestimmen Speicherausbau-Möglichkeiten
- RAM in Riegeln unterschiedlicher Größe angeboten
- DIMM-Riegel (Dual Inline Memory Module) = Arbeitsspeichermodule für Desktop-Systeme
- SO-DIMM (Small Outline DIMM) häufig in Laptops oder Mini-PCs verbaut

## Formfaktoren
- UDIMM (Unbuffered Dual-Inline-Memory-Module) - häufigster Desktop-Formfaktor
- SO-DIMM - weniger Pins und physikalisch kürzer

## DRAM (Dynamic Random Access Memory)
- Speicherung jedes Datenbits auf separaten Kompensator

## SDRAM (Synchronous Dynamic Random Access Memory)
- Getaktete DRAM-Technologie
- Synchrone Datenübertragung zum Speicher-Bus
- Takt durch System-Bus oder separaten - an System-Bus angeschlossenen Speicher-Bus vorgegeben
- Low-Power SDRAM für mobile Geräte

## DDR-RAM (Double Data Rate)
- Doppelt so schnelle Datenübertragung
- Zwei Datentransfers pro Taktzyklus
- Verschiedene RAM-Generationen nicht untereinander kompatibel

### DDR
- Dichte: 512 MB, 1 GB
- Geschwindigkeit: 333 MT/s, 400 MT/s
- Spannung: 2,5 V
- Pin-Anzahl: 200 Pins

### DDR2
- Dichte: 512 MB, 1 GB, 2 GB, 4 GB
- Geschwindigkeit: 667 MT/s, 800 MT/s
- Spannung: 1,8 V
- Pin-Anzahl: 200, 400 Pins

### DDR3
- Dichte: 1 GB, 2 GB, 4 GB, 8 GB, 16 GB
- Geschwindigkeit: 1.600 MT/s, 1.866 MT/s
- Spannung: 1,35 V²
- Pin-Anzahl: 204, 240 Pins

### DDR4
- Dichte: 4 GB, 8 GB, 16 GB, 32 GB
- Geschwindigkeit: 2.133 MT/s, 2.400 MT/s, 2.666 MT/s, 3.200 MT/s
- Spannung: 1,2 V
- Pin-Anzahl: 260, 288 Pins

### DDR5
- Dichte: 8-64 GB etc.
- Geschwindigkeit: 4.800 MT/s
- Spannung: 1,1 V
- Pin-Anzahl: 288 Pins

## DDR-SDRAM
- Double Data Rate Synchronous Dynamic Random Access Memory
- Verwendung für Speichermodule des DIMM- und SO-DIMM-Standards als Arbeitsspeicher

## SSD-RAM (Solid State RAM)
- Flash-basierte Speicher
- Daten im Speicher bleiben auch ohne Stromzufuhr gesichert
- Geringer RAM-Speicher - Auslagerung von Daten auf Festplatte
- **QLC (Quad-Level-Zellen)**: 4 Datenbits pro Speicherzelle, größere Dichte auf kleinerem Raum

## FSB (Frontsidebus)
- Verbindung von Prozessor, Chipsatz, DRAM und Grafikcontroller auf dem Mainboard
- Beschrieben durch Breite (in Bits) und Geschwindigkeit (in Megahertz)

## Latenz
- Reaktionszeit des Speichers auf Befehle
- Je geringer die Latenz, desto schneller das Gerät
- Höhere Gesamtgeschwindigkeit kann auch schneller sein

## ECC (Error Correcting Code)
- Fully buffered, registered EEC-RAM
- Minimierung und selbständige Korrektur von Speicherfehlern
