# Allgemeine Schutzmaßnahmen - Clients und mobile Datenträger

## Schutzmaßnahmen von Clients

### Gefährdungslage von Clients
- Schadprogramme
- Datenverlust durch lokale Datenhaltung
- Datenverlust durch Hardwaredefekte
- Softwareschwachstellen oder Fehler
- Unberechtigte Benutzung
- Installation nicht benötigter Betriebssystemkomponenten und Applikationen
- Abhören von Räumen mittels Mikrofonen und Kamera
- Fehlerhafte Administration oder Nutzung von Geräten und Systemen


### Ausgewählte Schutzmaßnahmen für Clients

#### Basismaßnahmen
- Benutzerauthentifizierung
- Rollentrennung
- Aktivierung von Autoupdate-Mechanismen
- Regelmäßige Datensicherung
- Bildschirmsperre
- Einsatz von Virenschutzprogrammen
- Protokollierung
- Absicherung des Boot-Vorgangs

#### Standardmaßnahmen
- Festlegung einer Sicherheitrichtlinie für Clients
- Planung des Einsatzes von Clients
- Planung der Beschaffung von Clients
- Kompatibilitätsprüfung von Software
- Zugriff auf Ausführungsumgebungen und unbeobachteter Codeausführung
- Updates und Patches von Firmware, Betriebssysteme und Anwendungen
- Sichere Installation und Konfiguration von Clients
- Deaktivierung und Deinstallation nicht benötigter Komponenten und Kennungen
- Nutzung von TLS
- Restriktive Rechtevergabe
- Schutz der Administrationsschnittstellen
- Verhinderung der unautorisierten Nutzung von Rechnermikrofonen und Kameras
- Nutzung von Client-Server-Diensten

#### Maßnahmen für erhöhten Schutzbedarf
- Verschlüsselung der Clients
- Systemüberwachung
- Einrichtung einer Referenzinstallation für Clients
- Einrichtung lokaler Paketfilter
- Einsatz zusätzlicher Maßnahmen zum Schutz vor Exploits
- Aktive Verwaltung der Wurzelzertifikate
- Einbindung in die Notfallplanung
- Unterbrechungsfreie und stabile Stromversorgung


### Beschreibung von Schutzmaßnahmen für Clients

#### Absicherung des Boot-Vorgangs
- Wechseldatenträger können Sicherheitsvorkehrungen umgehen
- Vermeidung von Eingriffen in den Boot-Vorgang durch eventuelle Schadprogramme

#### Zugriff auf Ausführungsumgebungen mit unbeobachteter Codeausführung
- Deaktivierung der Nutzung von Ausführungsumgebungen in der Client-Firmware
  - BIOS-Sicherheitseinstellungen

#### Rollentrennung
- Grundsätzliche Unterscheidung zwischen "Benutzer" und "Administrator"
  - Administratoren: Rechte zur IT-Systemverwaltung
  - Benutzer: Aufgabenerfüllung am Client

#### Protokollierung
- Aufzeichnung aller sicherheitsrelevanten Ereignisse
- Aktivierung und regelmäßige Überprüfung der Protokollierung

#### Nutzung von TLS
- Verwendung des Sicherheitsprotokolls SSL/TLS bei Web-Nutzung
- Absicherung von Verbindungen
  - Verschlüsselung der Verbindungsinhalte
  - Überprüfung der Vollständigkeit und Korrektheit der übertragenen Daten
  - Prüfung der Identität des Servers

#### Deaktivierung und Deinstallation von nicht benötigten Komponenten und Kennungen
- Standardinstallation eines Betriebssystems
  - Benutzerkennungen, Programme, Dienste und sonstige Komponenten mit eingerichtet
- Prüfung der Notwendigkeit von in Standardinstallation enthaltenen Tools
- 
