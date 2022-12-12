# Betriebssystem-Virtualisierung und BIOS

Um eine Betriebssystem-Virtualisierung ausführen zu können, muss i.d.R. eine Virtualisierungssoftware Hypervisor (griech. "Aufseher") oder ein Virtual Machine Monitor (VMM)
installiert werden (z.B. Parallels Desktop für MacOS, VirtualBox, VMware Workstation). Unter Windows 10 kann ohne die Installation einer Virtualisierungssoftware ein Windows-Subsystem
für Linux, kurz WSL, aufgerufen werden.
In einer Controllerschicht verwaltet der VMM Hardware, Schnittstellen und Gastbetriebssysteme und sorgt dafür, dass Betriebssysteme und Apps nicht in Konflikt kommen.
Bei der System-Virtualisierung wird ein System oder werden mehrere vollständige Systeme nachgebildet, worauf beliebige Betriebssysteme ausführbar sind. 
Die Systeme orientieren sich an echter Hardware, lassen sich bedarfsgerecht und virtuell an die Erfordernisse anpassen bzw. bedarfsgerecht auf unterschiedliche
virtuelle Maschinen verteilen.

## BIOS oder UEFI

### Begriffe
- **Bios** = **B**asic-**I**nput-**O**utput-**S**ystem
- Auf einem EPROM auf dem Motherboard installiert
- Enthält Firmware und grundlegende Steuerung der Hardware-Komponenten
- Startet das auf der Festplatte installierte Betriebssystem
- Selbsttest der Hardware-Komponenten
- Ablösung durch **UEFI** = **U**nified-**E**xtensible-**F**irmware-**I**nterface
- Schneller, leistungsfähiger und bessere GUI
- Eigenes Betriebssystem für 64-Bit-Systeme
- Verwendet GPT-Partitionierung für bis zu 128 Partitionen statt 4 und bis 3 TByte Speichervolumen

### Aufrufe
- **abhängig vom Hersteller** - Entf., F1, F2, F8, F10, ESC oder STRG+ALT+ESC = BIOS
- Windowstaste+i = UEFI-BIOS

