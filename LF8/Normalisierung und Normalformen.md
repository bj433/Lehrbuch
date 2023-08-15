# Normalisierung und Normalformen

- Verfahren zur Verringerung von Datenredundanz
- Erhöhung der Datenkonsistenz

## 1. Normalform
- Atomare (einfache) Existenz von Werten in Attributen der Tabelle
- Keine Auflistungen von Werten
- Jeder Wert = Eigene Spalte
- Zuweisung eines Primärschlüssels an zwei zusammengesetzt eindeutige Attribute

## 2. Normalform
- Abhängigkeit der Nichtprimärschlüsselattribute von gesamten Primärschlüssel
- Auslagerung von Attributen in Teilabhängigkeit (Abhängig von einem Teil des Primärschlüssels)
- Ergebnis = Zwei über 1:n verknüpfte Tabellen

## 3. Normalform
- Keine transitive Abhängigkeit von Nichtschlüsselattributen
  - Vermittelte/berechnete Abhängigkeiten
- Auslagerung transitiv abhängiger Attribute in neue Tabellen
- Beseitigung aller Datenredundanzen

## Boyce-Codd-Normalform (BCNF)
- Abhängigkeiten nur durch Schlüssel

## 4. Normalform
- Keine mehrwertigen Abhängigkeiten

## 5. Normalform
- Nur triviale Verbundabhängigkeiten

### Nachteile einer zu starken Normalisierung
- Viele kleine Tabellen -> negativer Einfluss auf Datenbankleistung
- Hohe Fehleranfälligkeit durch viele künstliche Schlüssel/Verknüpfungen
- Mehr Schlüssel = Mehr verbrauchter Speicherplatz (Redundanz)
