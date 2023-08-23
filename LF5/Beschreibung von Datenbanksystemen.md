# Beschreibung von Datenbanksystemen

## Bestandteile eines Datenbanksystems

### Datenbasis
- Strukturierte Sammlung von Daten
- Grafische Darstellung als Zylinder
  - Anlehnung an Festplattenlaufwerk
 
### Datenbankmanagementsystem
- Zugriffsverwaltung auf Datenbestand
- Durchführung der Datenspeicherung
- Verwaltung der Daten nach Datenmodell
- Gewährleistung des Mehrbenutzerzugriffs
  - Verwendung einer Kommunikationsschnittstelle
- Sicherung des optimalen Zugriffs
- Gewährleistung von Datensicherheit/Datenschutz

## ANSI/SPARC-Architektur
- Ziel: Entkopplung von Anwendung und Datenspeicherung

### Externes Schema (Ebene)
- Beschreibung der Benutzersicht auf Daten
- Abstimmung des Schemas auf User-Wünsche
- Multi-User-Betrieb
- Einrichtung eines Berechtigungskonzepts

### Konzeptionelles Schema (Ebene)
- Beschreibung aller logischer Dateneinheiten und deren Beziehungen
  - Festlegung durch Datenmodell
- Keine Datenwerte enthalten
- Vorteile:
  - Stabile Beschreibung der Datenbasis
  - Dokumentation der Informationszusammenhänge
  - Langsamere Veränderungen als einzelne Anwendungen
 
### Internes Schema (Ebene)
- Organisation der physischen Datenspeicherung
  - Festlegung der physikalischen Realisierung auf Speichermedien
- Algorithmen zur Speicherung, Indizierung, Sortierung und Selektion von Daten

## Unterscheidung nach Betriebskonzept
- Stand-Alone-Datenbank: Datenbank + Datenbankprogramm auf Workstation
- File-Share-Datenbank: Datenbank = Server, Datenbankprogramm = Client
- Client-Server-Datenbank: Datenbank und Datenbankmanagementsystem = Server, Zugriffsoberfläche = Client

## Arten von Datenbanken

### Hierarchische Datenbank (Hierarchisches Datenmodell)
- Verwaltung in einer Baumstruktur
  - Jeder Datensatz = Ein Vorgänger
- Redundanz nicht vermeidbar
- Nutzung bei Dateisystemen von Betriebssystemen

### Netzwerkdatenbank (Netzwerkdatenmodell)
- Jeder Datensatz = Mehrere Vorgänger möglich
- Abbildung von m:n Beziehungen
- Vermeidung von Redundanz

### Relationale Datenbank (Relationales Datenmodell)
- Speicherung von Daten in verschiedenen Tabellen
  - Beziehungen untereinander
- Standard für Datenbanken
- Einschränkungen bei Speicherung und schneller Verarbeitung großer Datenmengen

### Objektdatenbank (Objektorientiertes Datenmodell)
- Basis bei objektorientiertem Programmierparadigma

### Objektrelationale Datenbank (Objektrelationales Datenmodell)
- Verbindung des relationalen Datenmodells mit dem objektorientierten Datenmodell
- Speicherung von Daten als Relation von Objekten

## NoSQL-Datenbanken

### Key-Value-Datenbank (Key-Value Datenmodell)
- Schlüssel-Wertepaare
- Schlüssel = Index für Datenzugriff
- Wert = Strukturierte oder unstruktierte Daten

### Dokumenten-Datenbank (Dokumentenorientiertes Datenmodell)
- Speicherung von Daten als Dokumente

### Graph-Datenbank (Graphenorientiertes Datenmodell)
- Weiterentwicklung des Netzwerkdatenmodells
- Darstellung und Speicherung vernetzter Informationen

### Spaltenorientierte Datenbank (Spaltenorientiertes Datenmodell)
- Speicherung in Spalten
- Hilfe bei Analysen

## Kardinalitäten
- 1:1 = eins zu eins
- 1:n = eins zu viele
- m:n = viele zu viele

## Primary Key
- Minimale Kombination von Spalten (Attributen)
- Eindeutige Identifikation von Datensätzen
- Bedingungen:
  - Eindeutigkeit: Eindeutige Werte
  - Minimalität: Bestand aus meist einer Spalte
  - Unveränderbarkeit: Unveränderliche Werte
 
## Foreign Key
- Attribut mit Verweis auf Primary Key
- Gleicher Datentyp wie Primary Key

## Referenzielle Integrität
- Foreign-Key-Werte der Foreign-Key-Tabelle auch in Primary-Key-Tabelle vorhanden

## Transformationsregeln
- > Ein Entitätstyp wird mit all seinen Attributen zu jeweils einer Tabelle zusammengefasst.
- > Jede Tabelle erhält einen Primary-Key aus einem Attribut oder einer Kombination aus Attributen, welche im ER-Modell gekennzeichnet wurden. Sind solche Attribute nicht vorhanden, dann wird ein künstlicher Primary-Key eingeführt.
- > Jede m:n-Beziehung wird in einer eigenen Tabelle abgebildet. Diese Tabelle erhält die Primärschlüssel der beteiligten Entitätstypen als Fremdschlüssel und die Attribute, welche der Beziehung direkt zugeordnet sind.
- > Die Umsetzung der 1:n-Beziehung erfolgt, indem der Primary-Key der einen Tabelle als Fremdschlüssel in die andere Tabelle eingefügt wird.
  
### Data Definition Language (DDL) - Datendefinitionssprache
- Beschreibung, Änderung und Entfernung von Datenstrukturen
- SQL-Befehle: Bspw.: CREATE TABLE, DROP VIEW

### Data Manipulation Language (DML) - Datenbearbeitungssprache
- Ausführung von Operationen an Datensätzen
- SQL-Befehle: Bspw.: SELECT, UPDATE, INSERT INTO

### Data Control Language (DCL) - Datenüberwachungssprache
- Berechtigungsmanagmenet in Datenbanken
- SQL-Befehle: Bspw.: GRANT, REVOKE

### Transaction Control Language (TCL) - Transaktionsüberwachungssprache
- Ausführungsbestimmung von Anweisungen
- SQL-Befehle: Bspw.: COMMIT, ROLLBACK
