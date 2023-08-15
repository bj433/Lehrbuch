# Datenbanklösungen und Big Data

## Big Data

### Volume
- Beschreibung von Datenmengen
- Speicherung und Verarbeitung

### Variety
- Beschreibung der Datenvielfalt
- 90% unstrukturierte Formate
- Analysierbarkeit durch Machine Learning

### Velocity
- Beschreibung der Produktions-/Verarbeitungsgeschwindigkeit
- Echtzeitverarbeitung

### Veracity
- Beschreibung der Vertrauenswürdigkeit und Qualität
- Zusammenführung von Daten aus unterschiedlichen Quellen

### Value
- Beschreibung des Mehrwerts
- Auswertung riesiger Datenmengen

## Relationale Datenbank

### Datenmodell
- Speicherung in separaten Tabellen
- Zusammenführung bei Suchanfragen

### Schemata
- Festgelegte Datentypen und strukturen

### Skalierung
- Vertikale Skalierung
- Ein Server = komplettes Datenbanksystem
- Bedingte Steigerung der Leistungsfähigkeit möglich

### Umsetzung der ACID-Regeln
- Alle Regeln umgesetzt
- Atomicity, Consistency, Isolation, Durability

### Leistung
- Optimierung von Abfragen, Indizes und Struktur

### Abfragesprachen
- Einsatz von SQL

### Populäre Datenbankmanagementsysteme
- MySQL
- PostgreSQL
- Oracle
- MS-SQL

### Einsatzgebiete
- Datenbanklösungen:
  - ACID-Support
  - Keine wesentlichen Strukturänderungen
  - Unkontrollierter Wachstum der Datenmenge
  - Leicht strukturierbare Daten
 
## NoSQL-Datenbank

### Datenmodell
- Verschiedene Datenbankmodelle
  - Dokumente
  - Graph
  - Key-Value
 
### Schemata
- Flexibel vereinbar
  - Strukturiert
  - Unstrukturiert
  - Semi-strukturiert
- Keine nötige Konvertierung

### Skalierung
- Horizontale Skalierung
- Anknüpfbarkeit neuer Datenbankserver

### Umsetzung der ACID-Regeln
- Keine Unterstützung
- Verwendung des BASE-Modells
  - Basically Available, Soft State, Eventually Consistant
- Verfügbarkeit vor Konsistenz

### Leistung
- Nutzung von Cloud-Servern/Hardware-Clustern
- Hohe Leistungsstärke

### Abfragesprachen
- Keine einheitliche Abfragesprache

### Populäre Datenbankmanagementsysteme
- MongoDB
- Apache HBase
- Amazon DynamoDB
- Redis
- Couchbase
- Cassandra
- Elasticsearch

### Einsatzgebiete
- Datenbanklösungen:
  - Echtzeit-Datenverarbeitung
  - Schlecht strukturierbare Daten
  - Große, schnell wachsende Datenmengen
