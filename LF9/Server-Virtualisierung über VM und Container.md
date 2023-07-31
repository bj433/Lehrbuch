# Server-Virtualisierung über VM und Container

## Unterschiede zwischen virtuellen Maschinen und Containern

### Virtuelle Maschine
- Betriebssystem mit Anwendungen auf emulierter Hardware
- Isolierte Umgebung
- Zugriff auf zugeteilte Ressourcen begrenzt
- Parallelbetrieb (Hardware als Ressourcengrenze)
- VM-Betrieb durch Hypervisor

### Container
- Isolation von Prozessen durch Server
- Betriebssystem auf Hardware des Hosts
- Parallelbetrieb (Hardware als Ressourcengrenze)
- Betrieb von Containern durch Containerumgebung
- Geringe CPU-, Speicher- und Festplattenressourcennutzung

### Hypervisor
- Software zur Computerhardware-Emulation
- Mögliche parallele Installation von mehreren Betriebssystemen

#### Typ 1 (Bare Metal)
- Betrieb auf Hardware

#### Typ 2 (Hosted)
- Betrieb auf Betriebssystem
- Gastsystem als Prozess

### Administration virtueller Maschinen

#### Snapshots
- Sicherung des aktuellen Systemzustands
- Rollbackoption falls Updates fehlschlagen

#### Start & Stop
- Managementsoftware im Browser

### Vor- und Nachteile von Virtualisierung

#### Vorteile
- Unabhängigkeit von Server-Hardware
- Serverkonsolidierung (Mehrere Server als VMs auf einer Hardware)
- Höhere Verfügbarkeit
- Schnelle Bereitstellung
- Schnelle Behebung von Ressourcenengpässen

#### Nachteile
- Know-How (Einarbeitung zur Konfiguration von VMs erforderlich
- Single Point of Failure


### Vor- und Nachteile von SaaS

#### Vorteile
- Weltweite Zugriffsmöglichkeit via Browser
- Keine eigene Server-IT/Hardware nötig
- Skalierbarkeit nach Bedarf
- Kein Wartungsaufwand

#### Nachteile
- Abhängigkeit vom Dienstleister
- Standard nach Definition des Anbieters
- Schnittstellen zu Drittsystemen ggf. nicht vorhanden
- Einfacher Datenzugriff für Anbieter
- Erforderliches Vertrauen und klare Verträge
