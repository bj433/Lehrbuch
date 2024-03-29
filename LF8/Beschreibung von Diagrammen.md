# Beschreibung von Diagrammen

## Anwendungsfalldiagramme

- Strukturierung von Anwendungsfällen bei Programmen/Systemen
- Darstellung der Beziehungen zwischen Akteuren und Anwendungsfällen
- Darstellung von äußerlich erkennbarem Systemverhalten

### Notationselemente

#### Systemgrenze
- Auflistung aller gegebenen Anwendungsfälle
- Spätere Bereitstellung von Funktionen

#### Anwender oder Akteur
- Benutzer des Systems
- Interaktionen mit anderen Systemen

#### Anwendungsfall
- Beschreibung von bereitgestellten Aktion(en)

#### Assoziation (Strich)
- Darstellung von Beziehungen

#### Include-Beziehung
- Verpflichtende Einbindung einer Funktionalität von einem Anwendungsfall in einem anderen Anwendungsfall
  - Anwendungsfall wird zur Existenzbedingung für eingebundenen Anwendungsfall
- Funktionalität MUSS vorhanden sein
 
#### Extend-Beziehung
- Einbindung einer Funktionionalität von einem Anwendungsfall in einem anderen Anwendungsfall
  - Anwendungsfall kann eingebundenen Anwendungsfall erweitern
- Funktionalität muss nicht vorhanden sein

#### Generalisierung/Spezialisierung
- Beziehung zwischen allgemeinen und spezialisierten Elementen

## Klassendiagramme

- Analyse und Entwurf von Softwaresystemen
- Grafische Beschreibung von Beziehungen zwischen Klassen einer Anwendung
- Statisches Bild der Anwendung

### Notationselemente

#### Klasse
- Darstellung durch Rechtecke
- Name, Eigenschaften, Methoden
  - Trennung durch horizontale Linie
- Beschreibung von Eigenschaften durch Typ/Attribute
- Beschreibung von Methoden durch Funktionen/Parameter

#### Alternative Klassendarstellungen
- Keine Eigenschaften und Methoden
- Darstellung von Beziehungen zwischen Klassen

#### Sichtbarkeit für Eigenschaften und Methoden
- Beschreibung von Zugriffsmodifiern in OOP
- "+ = public"
- "- = private"
- "# = protected"

#### (gerichtete) Assoziation
- Beziehung zwischen zwei Klassen
- Keine Teil-Ganzes-Beziehung
- Kennzeichnung durch Extrapfeil

#### Aggregation
- Teil-Ganzes-Beziehung
- Einzelne Objekte auch unabhängig voneinander
- Kennzeichnung durch Linie mit nicht ausgefüllter Raute an "Ganzes"-Klasse

#### Komposition
- Starke Teil-Ganzes-Beziehung
- Teil nicht ohne Ganzes existent
- Kennzeichnung durch Linie mit ausgefüllter Raute an "Ganzes"-Klasse

#### Multiplizität
- Anzahl Objekte in Beziehungen zwischen zwei Klassen
- Bspw.: 1 zu 0..*, n zu m

#### Vererbung
- Kennzeichnung durch Linie mit nicht ausgefülltem Dreieck als Pfeilspitze
  - Pfeil von Unterklasse zu Oberklasse
- Weitergabe von Eigenschaften von Oberklasse zu Unterklasse
- Strichline bei Vererbung von Interface

## Aktivitätsdiagramm

- Darstellung des Systemverhaltens
- Beschreibung von Aktionsabläufen, Prozessen und Entwicklungsdokumentationen

### Notationselemente

#### Startknoten/Endknoten/Ablauf-Ende
- Startknoten = Beginn eines Ablaufs
  - Ausgefüllter schwarzer Kreis
- Endknoten = Ende eines Ablaufs
  - Ausgefüllter schwarzer Kreis mit schwarzem Ring
- Ablauf-Ende = Ende eines Zweigs
  - Nicht ausgefüllter Kreis mit Kreuz drin
 
#### Aktion
- Verhalten für Veränderungen

#### Kante
- Angabe des Kontrollflusses zwischen Aktionen
- Pfeil

#### Verzweigung
- Ausführung von Aktionen abhängig von erfüllten Bedingungen
  - Raute zwischen zwei Aktionen
  - Pfeile ausgehend von Raute zu Aktionen hin
 
#### Zusammenführung
- Ausführung von Folgeaktion nach Abschluss Einer von Zwei Aktionen
  - Raute zwischen drei Aktionen
  - Pfeil ausgehend von Raute zu Folgeaktion hin
  - Pfeile ausgehend von Aktionen zu Raute hin
 
#### Aufspaltung
- Ausführung mehrerer Folgeaktionen nach Abschluss einer Aktion
  - Schwarzes Rechteck zwischen drei Aktionen
  - Pfeil ausgehend von Aktion zu Rechteck hin
  - Pfeile ausgehend von Rechteck zu zwei Folgeaktionen hin
 
#### Synchronisation
- Ausführung einer Folgeaktion nach Abschluss mehrerer Aktionen
  - Schwarzes Rechteck zwischen drei Aktionen
  - Pfeil ausgehend von Rechteck zu Folgeaktion hin
  - Pfeile ausgehend von Aktionen zu Rechteck hin
 
#### Aktivität
- Darstellung einzelner Aktionen in einem Kontrollfluss
- Partitionierung von Aktivitäten
- Ein- und Ausgabeparameter als Rechtecke

