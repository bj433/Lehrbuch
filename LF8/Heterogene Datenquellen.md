# Heterogene Datenquellen

## Bedeutung
- "Uneinheitlich", "andersartig"

## Formen von Heterogenität

### Technisch
- Unterschiedliche Zugriffsschnittstellen
- Bspw.: XPath, SQL

### Syntaktisch
- Unterschiedliche Datenformate
- Bspw.: 20.03.2021, 2021-03-20, 20. März 21

### Zugrunde liegendes Datenmodell
- Verschiedene verwendete Datenmodelle von Quellen
- Bspw.: dokumentarisiert, relational, etc.

### Strukturell
- Unterschiedliche Speicherstruktur
- Bspw.:
  - 2 Quellen:
    - Adressdaten direkt in Kundentabelle verwaltet
    - In Extratabelle ausgelagert
   
### Semantisch
- Unterschiedliche Bedeutung, Interpretation und Nutzungsart
- Bspw.: Ortsangabe "Ort"/"Location"

## Informationsintegration
- Zusammenführung von Daten aus verschiedenen Datenquellen
- Bspw.: Heterogene Datenstrukturen in gemeinsame einheitliche Datenstruktur

## Möglichkeiten der Integration von Daten aus unterschiedlichen Datenquellen

### Materalisierte oder physische Integration
- Überführung von Daten aus diversen Datenquellen in eine zentrale Datenbasis
- Bereitstellung einer einheitlichen Struktur für alle Daten
- Anwendung in Data Warehouses oder Data Lakes

#### Vorteile
- Schnelle Verfügbarkeit von Daten
- Höhere Datenqualität

#### Nachteile
- Aktualität nicht sichergestellt
- Hoher nachträglicher Aufwand für Änderung von Datenquellen
- Hardwarebeschaffung und -wartung

### Virtuelle oder logische Integration
- Verbleib der Daten innerhalb der Quellen
- Integration auf Anfrage
- Anwendung in föderierten Datenbanksystemen oder mediatorbasierten Informationssystemen

#### Vorteile
- Aktualität der Daten gewährleistet
- Flexible Änderbarkeit von Datenquellen

#### Nachteile
- Lange Abfragezeit für Daten
- Geringere Qualität
