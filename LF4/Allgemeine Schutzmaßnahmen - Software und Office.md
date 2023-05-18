# Allgemeine Schutzmaßnahmen - Software und Office

## Allgemeine Schutzmaßnahmen für Software

### Basismaßnahmen
- Sicherstellung der Integrität von Software
- Entwicklung einer präzisen Installationsanweisung für jedes Softwareprodukt
- Sichere Installation und Konfiguration

## Standardmaßnahmen
- Festlegung der Verantwortlichkeiten im Bereich Software
- Erstellung eines Anforderungskatalogs für Standardsoftware
- Auswahl einer geeigneten Standardsoftware
- Überprüfung der Lieferung von Software
- Lizenzverwaltung und Versionskontrolle
- Vollständige und sichere Deinstallation

## Maßnahmen für erhöhten Schutzbedarf
- Implementierung zusätzlicher Sicherheitsfunktionen
- Nutzung zertifizierter Standardsoftware
- Einsatz von Verschlüsselung, Checksummen oder digitalen Signaturen


## Beschreibung von Schutzmaßnahmen für Software

### Sicherstellen der Integrität von Software
- Installation nur über Originaldatenträger oder geprüfte identische Kopien
  - Vermeidung von manipulierten Konfigurationsdateien

### Erstellung eines Anforderungskatalogs für Standardsoftware
- Anforderungskatalog für Auswahl geeigneter Standardsoftware
- Funktionalität und sicherheitsrelevante Anforderungen als Kriterien

### Überprüfung der Lieferung von Standardsoftware
- Prüfung vorhandener Unterlagen
- Bestellungshistorie der Lieferung, mögliche Transportschäden, Vollständigkeit

### Vollständige und sichere Deinstallation von Software
- Entfernung aller angelegten Daten
  - Einträge in Systemdateien
- Dokumentation aller Änderungen beim Installationsprozess

## Auswahl grundlegender Schutzmaßnahmen für Betriebssysteme

### Sicherstellung eines minimalen Systems
- Abwägung der Notwendigkeit für Systeminstallationen

### Korrekte Konfiguration
- Individuelle Installationen zur Vermeidung von Sicherheitsrisiken

### Sperrung von Ports
- Sperrung aller nicht notwendigen Ports

### Benutzerkonten
- Anlage nur benötigter Accounts
- "So viel wie nötig, so wenig wie möglich" - Bezug auf Berechtigungen

### Aktualität von Betriebssystemen
- Einspielung von Sicherheitsupdates unmittelbar nach Veröffentlichung

### Regelmäßige Sicherheitschecks mithilfe von Log-Dateien
- Prüfung von Log-Dateien des Betriebssystems
- Hilfreich beim Aufdecken von Angriffen und -versuchen

### Verwendung sicherer Passwörter

### Regelmäßige Datensicherungen
- Höheres Risiko von Bedienungsfehlern oder Vireninfektionen -> Systemabstürze und Datenverlust als Folge
- Regelmäßige Backups


## Schutzmaßnahmen für Office-Produkte

### Basismaßnahmen
- Sicherstellung der Integrität von Office-Produkten
- Einschränkung aktiver Inhalte
- Regelungen zum Öffnen von Dokumenten aus externen Quellen
- Absicherung des laufenden Betriebs von Office-Produkten

### Standardmaßnahmen
- Auswahl geeigneter Office-Produkte
- Versionstests
- Sichere Installation und Konfiguration
- Versionskontrolle von Office-Produkten
- Beseitigung von Restinformationen vor Weitergabe von Dokumenten
- Regelung der Softwareentwicklung durch Endbenutzer
- Geregelter Einsatz von Erweiterungen
- Regelung der Verwendung von Viewer-Funktionen
- Schutz gegen nachträgliche Veränderungen von Informationen

### Maßnahmen für erhöhten Schutzbedarf
- Einsatz von Verschlüsselung und digitalen Signaturen
- Integritätsprüfung von Dokumenten


## Beschreibung von Schutzmaßnahmen für Office-Produkte

### Einschränkung aktiver Inhalte
- Bspw. Makros, Aktive-X-Steuerelemente
- Ausführung und Verbreitung möglicher Schadprogramme
- Unterbindung des automatischen Ausführens solcher Inhalte

### Regelungen zum Öffnen von Dokumenten aus externen Quellen
- Vermeidung der Öffnung unbekannter externer Quellen
- Vollständige Sicherheitsprüfung dieser Dateien

### Versionskontrolle
- Dokumentation über Versionen und Konfigurationen von Office-Produkten auf jeweiligen Rechnern
- Umgehung von Inkompatibilitäten zwischen einzelnen Versionen
- Möglichst hohe Einheitlichkeit

### Beseitigung von Restinformationen vor der Weitergabe von Dokumenten
- Abwägung der Relevanz und Wertigkeit von Meta-Informationen
- Entfernung überflüssiger Informationen

### Regelung der Verwendung von Viewer-Funktionen
- Mögliche Ausführung von Schadcode über Makros oder Software an und für sich
- Verringerung des Angriffsrisikos durch Verwendung von Viewern

### Schutz gegen nachträgliche Veränderungen von Informationen
- Funktionen zur Einschränkung des Umgangs mit erstellten Dokumenten
- Unterbindung der nachträglichen Bearbeitung


## Schutzmaßnahmen beim Einsatz von (Software-)Containern

### Gefährdungen beim Einsatz von Containern
- Schwachstellen in Images
- Ausbruch aus dem Container
- Administrative Zugänge ohne Absicherung
- Datenverlust (fehlende Persistenz)
- Tool-basierte Verwaltung beim Einsatz mehrerer Container ohne Absicherung
- Sorglose Verwendung von Zugangsdaten

### Ausgewählte Schutzmaßnahmen beim Einsatz von Containern

#### Basismaßnahmen
- Planung des Container-Einsatzes
- Planung der Anwendungen in Containern
- Planung der Verwaltung der Container
- Sicherung des Host-Systems
- Separierung der Container
- Verwendung sicherer Images
- Anwendung von Schutzmaßnahmen für die Containersoftware
- Sicherung der Zugangsdaten
- Speicherung von wichtigen Daten außerhalb des Containers

#### Standardmaßnahmen
- Erstellung von Richtlinien für den Betrieb von Containern
- Erstellung von Richtlinien für die Images von Containern
- Quantitätsbegrenzung von Anwendungen und Diensten pro Container
- Sicherstellung der Unveränderlichkeit von Containern
- Limitierung der Ressourcen pro Container
- Erstellung von Richtlinien für das Einbinden von Datenträgern in Container
- Regelmäßige Überwachung von Containern

#### Maßnahmen für erhöhten Schutzbedarf
- Automatisierte Auditierung von Containern, eigene Trusted Registry für Container
- Erstellung erweiterter Richtlinien für Container, Host Based Intrusion Detection für Container
- Mikro-Segmentierung von Containern, Hochverfügbarkeit von Containern
- Verschlüsselte Datenhaltung bei Containern, Verschlüsselung der Netzkommunikation zwischen Containern
