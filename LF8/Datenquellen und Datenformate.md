# Datenquellen und Datenformate

- Data Source = Herkunft von verwendeten Daten
- Primäre Datenquelle = Ort der Datenentstehung
- Sekundäre Datenquelle = Ort der Datenspeicherung

## Vergleich Open Data - Closed Data

### Open Data
- Zugänglichkeit: Jeder
- Maschinelle Datenverarbeitung: Leicht verarbeitbare Datenformate
- Kosten: Keine
- Rechte: Unlimitierte Verarbeitung und Weitergabe

### Closed Data
- Zugänglichkeit: Bestimmte Menschen/Organisationen
- Maschinelle Datenverarbeitung: Schwer verarbeitbare Datenformate (bspw.: analog)
- Kosten: Erheblich
- Rechte: Nutzung und Verbreitung verboten

### Vor- und Nachteile

#### Vorteile
- Besitz bei Menschen (keine Konzerne)
- Herkunft in der Öffentlichkeit - Öffentliche Zugänglichkeit
- Kein Urheberrecht
- Mehr Nutzer - mehr Innovation

#### Nachteile
- Finanzieller Verlust für Datenurheber
- Infragestellung der Qualität
- Wettbewerbsverzerrung
- Leichter Datenmissbrauch
- Datenschutz?
- Haftungsfrage im Schadensfall

## Dateiformate zur Datenübertragen
- Struktur der Datenablage
- Interpretation bei Verarbeitung

### Gängige Datenformate

#### CSV (Comma Separated Values) 
- Dateiendung: .csv
- Verwendung von Textdateien zur Speicherung und Datenaustausch
- Kommas als Separator zwischen Daten
- Kein einheitlicher Aufbau (Semikolon, Doppelpunkt, Leerzeichen, etc. auch verwendbar)
- Einfaches Format - für (fast) jedes Computerprogramm verständlich
  - Austausch zwischen inkompatiblen Programmen
 
#### XML (Extensible Markup Language) 
- Dateiendung: .xml
- Auszeichnungssprache und Datenformat
- Darstellung hierarchisch strukturierter Daten innerhalb einer Textdatei
- Inhalt - Textauszeichnungen (Markup)
- Auszeichnungen in </> = Tags
  - Paarweise
  - Tags + Inhalt = Element
  - Selbst definierbar
  - Tags können Parameter haben (Namen + Wert)
  - Ineinander geschachtelt
 
#### JSON (JavaScript Object Notation
- Dateiendung: .json
- Datenaustausch- und Textformat
- Schlüsselwertpaare
- Formatierung mit geschweiften Klammern {}
- Beliebig verschachtelbar
- Zeichenkodierung UTF-8
- Parser zur Verarbeitung

## Datenzugriff

### SOAP (Simple Object Access Protocol)
- Netzwerkprotokoll zum Datenaustausch
- Industriestandard des W3C (World Wide Web Consortium)
- ACID (Atomiziät, Konsistenz, Isolation und Dauerhaftigkeit) erfüllt
  - Gewährleistung zuverlässiger Datenbanktransaktionen
- Datenaustausch über XML-IS (Information-Set) basierende Nachrichten
- 
