# Beschreibung des objektorientierten Programmierparadigma

## Abstraktion

### Objekt
- Abstrakter oder realer Gegenstand
- Beschreibung durch Zustand und Verhalten
  - Eigenschaften mit konkreten Werten
  - Anzahl bestimmter Methoden
 
### Klasse
- Beschreibung mehrerer gleichartiger Objekte
- Exemplar (Instanz) = konkretes Objekt

## Kapselung

### Zugriffsmodifier

#### public
- Uneingeschränkter Zugriff
- Öffentliche Komponenten

#### protected
- Zugriff innerhalb eigener Klassen (und abgeleiteten Klassen)
- Geschützte Komponenten

#### private
- Zugriff innerhalb einer Klasse
- Private Komponenten

## Vererbung

### Arten von Vererbung

#### Einfachvererbung
- Abgeleitete Klasse -> eine Basisklasse

#### Mehrfachvererbung
- Abgeleitete Klasse -> mind. zwei Basisklassen

## Polymorphie

### Arten von Polymorphie

#### Dynamische Bindung
- Referenzzuweisungen erst zur Laufzeit klar ersichtlich

#### Überladen von Methoden
- Redundante Methodennamen für mehrere Methoden
- Zwei Optionen:
  - Mind. ein variierter Datentyp eines Übergabeparameters
  - Unterschiedliche Menge an Übergabeparametern
- Automatische Bestimmung der Methode bei Aufruf durch Parameter und Datentypen

#### Überschreiben von Methoden
- Methode in Basisklasse -> durch Methode der abgeleiteten Klasse übernommen
- Bedingungen:
  - Namentliche Übereinstimmung
  - Gleicher Datentyp und Menge Übergabeparameter
  - Gleicher Rückgabedatentyp
  - Keine stärkeren Zugriffsrechte als überschriebene Methode
    - Lockerung möglich
  - Methode muss vererbt sein
    - Private Methoden nicht vererbbar
   
## Objektorientierte Programmiersprachen

### C++ (1985)
- Ableitung von C
- Unterstützung von Mehrfachvererbung
- Rein prozedurale Programme möglich

### Java (1995)
- Universell einsetzbar
- Rein objektorientiert
- Indirekte Unterstützung von Mehrfachvererbung über Interfaces

### C# (2000)
- Nutzung und Vereinfachung von Konzepten aus Java, C++ und Delphi
- Rein objektorientiert
- Indirekte Unterstützung von Mehrfachvererbung über Interfaces
