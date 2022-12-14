# Mainboard und CPU

## Komponenten des Mainboards
- **Mainboard**:
  - Hauptplatine des Computers
  - Hardware-Komponenten auf dem Mainboard aufgebracht oder mit dem Mainboard verbunden
- **BIOS**:
  - Zuständig für Startvorgang des Computers
  - Basisbetriebssystem im EPROM
- **Chipsatz**:
  - Gewährleistung der Kommunikation unter allen Hardware-Komponenten
  - Maßgebliche Mitbestimmung der Ausstattung und Leistung des Mainboards
  - Bringt Daten zum Input/Output-Controller zur Versorgung der unterschiedlichen Peripheriegeräte
- **Formfaktoren**:
  - Größen und vereinbarte Standards von Mainboards
  - Gewährleistung der einwandfreien Kommunikation aller Komponenten
  - Bekannt: ATX oder ITX
- **Kompatibilität**:
  - Verhältnis Chipsatz, Prozessor und Sockel
- **Sockel**:
  - Physikalische Verbindung von Mainboard und Prozessor
- **Steckplätze**:
  - RAM-Speicherkarten in CPU-Nähe aufgrund hohen Datentraffics
- **Cachespeicher**:
  - Zwischenspeicher zur Vermeidung von Datenstaus

- **GPU-Prozessor**:
  - Unterstützung bei der Bilddatenverwaltung
- **PCIe-Steckplätze**:
  - Zuständigkeit für interne Anschlüsse von Peripheriegeräten
- **SATA- und M.2-Anschlüsse**:
  - Anschluss mehrerer Festplatten
- **Netzteil**:
  - Stromversorgung aller Komponenten
  - Vermeiden von Spannungsproblemen

## Prozessoren
- **Single-Core-Prozessoren**:
  - Ausreichend bei Standardanwendungen
  - Office, Standardkommunikation, Sicherheitsprogramme, einfache Bildbearbeitung
- **Multi-Core-Prozessoren**:
  - Videobearbeitung, 3D-Rendering, CAD, professionelle Audio- und Bildbearbeitung

## Vergleich AMD - Intel
### AMD
- **Prozessoren für Desktops und Notebooks**:
  - AMD Ryzen 3 bis 9
- **Prozessoren für leistungsstärkere und robustere Workstation**:
  - AMD Ryzen Threadripper
- **Basis**:
  - Andere Hauptplatine, CPU-Sockel und Chipsätze
- **Vergleich**:
  - Flexiblere Möglichkeiten des Leistungseinsatzes (Autotaktung) 
  - Günstiger im Preis
  - Auf Standardanwendungen ausgelegt

### Intel
- **Prozessoren für Desktops und Notebooks**:
  - Intel Core i3, i5, i7, i9, etc.
  - Abhängig von Anzahl der Cores
- **Prozessoren für leistungsstärkere und robustere Workstation**:
  - Intel XEON-Prozessoren in Performancestufen Bronze, Silber, Gold, Platinum
  - Unterschiede in Cores und Erweiterungsmöglichkeiten
  - Vielfältige Einsatzmöglichkeiten
- **Basis**:
  - Andere Hauptplatine, CPU-Sockel und Chipsätze
- **Vergleich**:
  - Mehr Cores als einfache Core-Prozessoren
  - Mehr Hauptspeicherzugriff, PCIe-Lanes und Cache
  - Integrierte Grafikkarte fehlt
  - Übertaktungsmöglichkeiten geringer
  - Multiprozessortechnik möglich
  - Größerer Befehlsumfang, Error Correcting Code Memory - Korrektur von Fehlern im Speicher
  - Thermal Design Power (TDP) - geringerer Energieverbrauch und weniger Abwärme
  - Bessere Kühlsysteme und externe Grafikkarten

## Mikroprozessor (CPU) - Leistungskomponenten
### Begriff
- Mikroprozessor - Central Processing Unit - Hauptprozessor oder zentrale Verarbeitungseinheit
- Befehlsverwaltung aus System heraus und Veranlassung von Informationsverarbeitung
- Steuerung und Kontrolle der Systeme
- Weitere Prozessoren zur Entlastung für Spezialaufgaben
- Mikrocontroller - zusätzliche analoge und digitale Ein- und Ausgänge
- Übernahme von Steuerungsaufgaben
- Einsatz in Embedded Systems (IoT)

### Bestandteile der CPU
- Rechenwerk (Arithmetic Logic Unit, ALU)
- Steuereinheit (Control Unit, CU)
- Speichermanager (Memory Management Unit, MMU)
- Zwischenspeicher (CPU-Cache)

### Strukturgröße
- Je geringer die Flächennutzung, desto leistungsstärker und energieeffizienter der Chip

### Prozessorleistung
- Erweiterung der Transistorenmenge auf dem Chip
- Verkürzung der Zugriffszeiten
- Optimierung des internen Rechneraufbaus
- Senkung der Betriebsspannung
- Erhöhung der Taktfrequenz
- Einführung von Erweiterungskarten, Speichercontrollern, Grafikausgabe und Chipsätzen
- Mehrfachintegration von Funktionsblöcken im Prozessor
- Hohe Abhängigkeit vom Prozessor im Systemverbund (Mainboard, Sockets)

### Garantie der Prozessorleistung
- Gewährleistung einer Dauerbelastung und hoher Taktstabilität

### Cache
- Direkt mit CPU verbunden - besonders schnell
- Zwischenspeicherung wartender Prozesse und Daten

### Chipsatz
- Hauptcontroller auf dem Mainboard zwischen einzelnen Komponenten des Computers
- Vereinigung vieler Controller durch Halbleiterbaustein
- Anbindung von Hauptprozessor, Bus-Systemen, Arbeitsspeicher, Laufwerken, Erweiterungskarten und anderen Geräten
- Einfluss auf Gesamtleistung des Computersystems
- Konfiguration über BIOS-Einstellungen
- Verbindung zwischen Chipsatz und Hauptprozessor häufig PCI Express

### Erhöhung der Taktfrequenz
- Intelligente Ausnutzung der CPU und zeitweise Übertaktung zur Erhöhung der Rechnerleistung
- Höherer Energieverbrauch, Höhere Wärmeentwicklung, lautere Computer durch aktive Kühlung

### Parallelisierung
- Nutzung der Wartezeit (durch Speicher- und Peripheriegeräte) - Ausführung anderer Programmcodes
**Multithreading**:
  - Parallele Verwaltung mehrerer Threads und Funktionen
  - Abwechselnde Zuschaltung abhängig von Beanspruchung
  - Hyper-Threading stellt Betriebssystem Funktionen weiterer Prozessorkerne bereit
**Pipelining**:
  - Befehlsausführung parallel in mehreren Stufen und Phasen
**Coprozessor**:
  - Prozessor, der Hauptprozessor um Funktionen erweitert
  - Entlastung bei bestimmten Rechenaufgaben
**Multi-Prozessor**:
  - Überwiegend in leistungsstarken Großrechnern oder Servern verbaut
**Multi-Core-Prozessor**:
  - Zusammenschaltung mehrerer Rechenkerne
  - Betriebssystem kann mehrere Recheneinheiten verwalten

### Turbo Boost (Intel) und Precision Boost (AMD)
- Automatische Übertaktung
- Bearbeitung von Ein-Kern-Programmen, Energieeinsparung und Wärmeoptimierung
- Kerne nur nach Bedarf zugeschaltet
- Beschleunigung von weniger belastenden Anwendungen
  - Einzelne Kerne werden höher getaktet während andere in den Wartezustand versetzt werden

### Multimedia-Erweiterungen
- MMX, XMM, SEE Befehlsätze
- Basis von 64 und 128 Bit

### Thermal Design Power (TDP)
- Maximal abgegebene Wärmeleistung eines Prozessors
- Kernspannung und Temperatur
- Liegt unterhalb der maximalen elektrischen Leistungsaufnahme
**Kühler**: 
  - Schutz des Prozessors vor Überhitzung und Ausfall
  - Luftkühler, Wasserkühlung und All-in-one-Wasserkühlung
  - Sollen höhere TDP als Prozessor haben
  - CLC-Kühler (All in one) - geschlossener Kreislauf
    - Montage wie Luftkühler, Kühlleistung einer Wasserkühlung

### GDGPU
- General Purpose Computation on Graphics Processing Unit
- Programmier-Schnittstelle, die allgemeine Berechnungen der GPU auch auf der Grafikkarte ausführen kann
- Nutzung bei Hochleistungscomputern
