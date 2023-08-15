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


