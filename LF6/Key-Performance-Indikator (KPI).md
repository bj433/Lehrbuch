# Key-Performance-Indikator (KPI)

- Messgröße der Leistungsstärke eines Prozesses
- Vergleiche miteinander, im Zeitablauf und in Beziehung mit anderen Messgrößen

## Erfolgsfaktoren zur Sicherstellung der Services
- SLA mit Kunden
- Vor Eskalation:
  - Nutzung aller Ressourcen im eigenen Level
- Rechtzeitige Erkennung der Eskalationsnotwendigkeit
- Genaue Beschreibung von Tickets
- Untersuchung von Gründen für ungelöste Tickets
- Beschreibung der Lösungsbearbeitung
  - Spätere Musterlösung
- Verfolgung des Ticketverlaufs als Case Owner
- Auswertung der Ticketsysteme für Verbesserungen

## Kritische Erfolgsfaktoren und Höchstwerte
- Herausstellung von Peaks
- Anzahl Anrufe pro Tag/Techniker/Support- oder Service-Level
- Anzahl gelöster/ungelöster/eskalierter Tickets
- Kennzahl der Verfügbarkeit
  - Verfügbarkeit in %
  - [(Vereinbarte Servicezeit - Ausfallzeit) / Vereinbarte Servicezeit] * 100
- Mean Time to Repair (MTTR)
  - Kennzahl der Systemverfügbarkeit
  - Durchschnittliche Reparaturzeit
  - Zeit ab Meldung bis erneute Verfügbarkeit
- Mean Time Between Failures (MTBF)
  - Kennzahl der Systemzuverlässigkeit
  - Mittlere Betriebsdauer zwischen zwei Ausfällen
- Anzahl erfüllter Serviceziele
- Anzahl und Schweregrad von Verletzungen der Serviceziele
- Anzahl der SLA
- Anzahl der Services mit zeitaktuellem SLA
- Anzahl der Services mit rechtzeitiger Berichterstattung
  - Aktiv initiierte Service-Reviews
- Verbesserungsgrad der Kundenzufriedenheit
- Häufigkeit der SLA-Reviews und Änderungen
- Anzahl der nicht vom Servicekatalog abgedeckten Services

## Typische Anforderungen an IT-Helpdesk-Mitarbeiter

### Persönliche Anforderungen
- Hohe Kunden- und Serviceorientierung
- Ausgeprägte Team- und Kommunikationsfähigkeit
- Hohes Maß an Eigeninitiative, Zuverlässigkeit, Belastbarkeit
- Lösungsorientierte Denkweise
- Gute analytische Fähigkeiten
- Begeisterung für innovative Technologien
- Verständliche Darstellung von Informationen und Wissen für User

### Fachliche Anforderungen
- Support und Fehleranalyse bei IT-Störungen per Telefon, E-Mail, Remote oder persönlich
- Festhalten aller Vorgänge im Ticketsystem
- Einhaltung der definierten SLA's bei Erfassung und Weiterleitung der Tickets
- Gute Kenntnisse bei Windows 10, Office 365, Office Software und Diensten
- Patch-Management (Betriebssysteme, etc)
- Server-Grundtätigkeiten (DNS, DHCP, Active Directory, File Services)
- Asset Monitoring und Asset Tracking
- Bereitstellung, Installation, Konfiguration und Support der clientseitigen Infrastruktur
  - Software, VPN und Virenschutz
- Allgemeine Durchführung von IMACD
  - Install, Move, Add, Change und Delete
- Entwicklung von Lösungen und Workarounds
- Gute Kenntnisse in Netzwerkinfrastrukturen
- Konfiguration und Betreuung der virtuellen Infrastruktur und Storage-Systeme
- Optimierung und Monitoring der Cloud-Umgebung
- Verwaltung und Vorbereitung von Leihgeräten
- Unterstützung bei IT-Projekten und Implementierungen
- Pflege der Knowledge-Base

## KPI im Netzwerkbereich

### Datendurchsatz oder Bandbreite
- Theoretischer und tatsächlicher Durchsatz
- Zugriff auf System- und Netzwerkinformationen mit Ereignisprotokollen
  - Bspw.: Überwachung der Bandbreitennutzung des gesamten Netzwerks
 
### TCP-Latenz
- Zeit für Datenpaket von Ausgangspunkt zum Ziel
- TCP-Latenz = Round-Trip-Time (Quelle -> Ziel -> Quelle)
- Netzwerklatenz = Faktor für physische Entfernung zwischen zwei Knoten
- Messung über Netzwerktools (Ping, Traceroute)

### TCP-Verlust
- Anzahl von gesendeten, aber nicht angekommenen Paketen (pro 1.000)
- TCP sendet verlorene Pakete erneut
  - Zuverlässige Übertragung mit Verzögerungen
 
### SYN- und FIN-Fehler
- SYN-Fehler = Fehler beim Verbindungsaufbau
- FIN-Fehler = Fehler beim Herunterfahren der Verbindung
- Three-Way-Handshake

### Log-Dateien
- Protokolldatei, Ereignisprotokolldatei
- Alle oder bestimmte Ereignisse von Prozessen auf einem IT-System
- Auslesung, Suche nach Problemen und Fehlern
- Angaben:
  - Wichtigkeit der Meldung
  - Informationstext zur Art des Ereignisses
  - Angesprochenes Zielsystem
  - Quelle der Meldung
