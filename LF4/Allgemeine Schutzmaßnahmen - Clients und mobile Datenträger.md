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
- Deinstallation/Deaktivierung der nicht nötigen Tools

#### Benutzerauthentisierung
- Eindeutige Identifikation und Authentisierung von Benutzern
- Interaktion zwischen Benutzer und IT-System nur nach erfolgreicher Authentisierung
- Authentisierungstechniken: PIN, Passwörter, Zugangskarten, Biometrie

#### Nutzung von Client-Server-Diensten
- Gleichberechtigte IT-Systeme -> Angebot und Nutzung von Diensten durch jedes System
- Vereinigung von typischen Funktionen von Servern und Clients
- Dezentrale Ressourcenteilung


## Schutzmaßnahmen mobiler Datenträger

### Definition

#### Auswechselbare Datenträger (Wechseldatenträger)
- Datenaustausch in Laufwerken
- Bspw. CD-ROM, DVD, Blu-ray, Magnetbänder, Speicherkarten

#### Externe Datenträger
- Datenaustausch über direkten Anschluss an IT-Gerät
- Bspw. USB-Sticks, externe Festplatten

#### Integrierte Datenträger
- Datenaustausch über indirekte Verbindung von Mobilgerät mit anderem IT-Gerät
- Bspw. Interne Speicher in Smartphones, Tablets und Digitalkameras


### Gefährdungslage
- Diebstahl oder Verlust von mobilen Datenträgern
- Defekte Datenträger
- Unzureichende Kenntnis über Regelungen bzgl. mobiler Datenträger
- Verbreitung von Schadprogrammen
- Sorglosigkeit im Umgang mit den Regelungen bzgl. mobiler Datenträger
- Datendiebstahl
- Ungevollte Weitergabe von Informationen durch Restdaten auf Datenträger
- Beeinträchtigung der Datenträger durch wechselnde und ungünstige Einsatzumgebungen


### Ausgewählte Schutzmaßnahmen für mobile Datenträger

#### Basismaßnahmen
- Festlegung zuverlässiger Kommunikationspartner
- Regelung des Informationsaustausches
- Schutz vor Schadsoftware
- Meldung bei Verlust oder Beschädigung des Datenträgers
- Sensibilisierung der Mitarbeiter zum sicheren Umgang mit mobilen Datenträgern
- Sicherungskopie der übermittelten Daten erstellen

#### Standardmaßnahmen
- Vereinbarungen zum Informationsaustausch mit externen Kommunikationspartnern
- Regelungen zum Versand von Datenträgern
- Sichere Löschung von Datenträgern vor und nach Verwendung
- Beseitigung von Restinformationen in Dateien vor Weitergabe
- Abschluss von Vertraulichkeitsvereinbarungen
- Angemessene Kennzeichnung der Datenträger beim Versand
- Erstellung einer Richtlinie zum sicheren Umgang mit mobilen Datenträgern
- Regelung der Mitnahme von mobilen Datenträgern
- Einführung einer Datenträgerverwaltung

#### Maßnahmen für erhöhten Schutzbedarf
- Verschlüsselung und digitale Signaturen
- Integritätsschutz durch Checksummen oder digitale Signaturen
- Sichere Versandart und Verpackung
- Sichere Aufbewahrung der Datenträger vor und nach dem Versand
- Verifikation von Datenträgern vor dem Versand
- Verwendung von zertifizierten mobilen Datenträgern


### Beschreibung von Schutzmaßnahmen mobiler Datenträger

#### Festlegung zuverlässiger Kommunikationspartner
- Sichere Informationsübertragung durch Berechtigungsvergabe an Kommunikationspartner
- Identitätsprüfung im Voraus

#### Verlustmeldung
- Umgehende Meldepflicht für verlüstige mobile Datenträger
  - sowohl geschäftlich, als auch privat
- Anderweitige Übermittlung der Daten
- Verhinderung des potentiellen Missbauchs betroffener Informationen
  - Prüfung auf Manipulation, wenn Datenträger wieder auftaucht

#### Regelung der Mitnahme von mobilen Datenträgern
- 

