# Testing

## Prozessschritte

### Testplanung
- Beschreibung des vollständigen Testprozesses
- Regelmäßige Anpassungen während Projektablauf
- Inhalte:
  - Teststrategie
  - Testziele
  - Kriterien für Testbeginn/Testende
  - Zu verwendende Testarten
  - Hilfsmittel und Werkzeuge
  - Richtlinien zur Dokumentation
  - Angaben zur Testorganisation
 
### Testentwurf
- Details einzelner Testobjekte
- Übersetzung der Testziele in Testfälle
- Anfertigung einer Testspezifikation
- Inhalte:
  - Testfallfindung
  - Festlegung von Testabläufen und Testreihenfolge
  - Bestimmung von Testdaten
  - Manuelle/Automatisierte Tests
 
### Testvorbereitung
- Vorbereitung von Testszenarien und benötigten Ressourcen
- Inhalte:
  - Auswahl der durchzuführenden Testfälle
  - Aufbau der Testumgebung
  - Vorbereitung und Bereitstellung von Testdaten
  - Bereitstellung von Dokumenten
 
### Testdurchführung
- Durchführung und Dokumentation der Tests
- Dynamisch: Ausführung des Programms
- Statisch: Analytische Prüfung

### Testauswertung
- Bewertung der Testobjekte
- Überprüfung der Testergebnisse
- Erstellung einer Liste von Abweichungen
- Vergleich Testergebnis - Erwartetes Ergebnis
- Empfehlung über Freigabe

### Testabschluss
- Vervollständigung und Archivierung der Testdokumente

## Statische Testverfahren
- Inspektion: Untersuchung des Programmcodes nach genauer Vorgehensweise
- Review: Weniger Formalität, weniger Aufwand
- Walkthrough: Programmpräsentation mit spontanen Fragen durch Gutachter
- Audit: Progammpräsentation mit festgelegtem Prüfkatalog
- Statische Code-Analyse: Fokus auf nicht funktionale Aspekte des Programms

### Vorteile
- Frühe Fehlererkennung
- Aufdeckung von Fehlerzuständen
- Weniger teure Testtechniken
- Prüfung von Programmierkonventionen, Standards und Design
- Erfassung nicht funktionaler Qualitätskriterien
- Wissensaustausch

### Nachteile
- Geringe Eignung für Integrations- und Systemtests
- Keine Findung von Laufzeitfehlern

## Dynamische Testverfahren

### Whitebox-Test
- Strukturbasiertes/strukturelles Testverfahren
- Kenntnis vom Quellcode und der Softwarestruktur
- Überdeckung des Kontrollflusses/Datenflusses
  - Anweisungsüberdeckung
  - Zweigüberdeckung
  - Pfadüberdeckung
  - Einfache und mehrfache Bedingungsüberdeckung
- Anwendung bei Unit- und Komponententests

### Blackbox-Test
- Standardtest in der Softwareentwicklung
- Prüfung des Verhaltens des Testobjekts ohne bekannten Quellcode
- Testfälle auf Basis der Softwarespezifikation
  - Ableitung von Testdaten
- Vergleich reale Testergebnisse - Erwartete Ergebnisse
- Methoden:
  - Äquivalenzklassenbildung
  - Grenzwertanalyse
 
#### Vorteile
- Tatsächliche Ausführung des Programms
- Zusammenspiel einzelner Systemteile
- Mögliches Testen nicht funktionaler Qualitätsanforderungen

#### Nachteile
- Lauffähige Testumgebung
- Testen von nötigen Programmteilen
- Aufdeckung von Fehlverhalten - Keine Ursachenforschung

## Testarten

### Funktionalität
- Erfüllung der gestellten funktionalen Anforderungen an Software
- **Testbereiche**:
  - Richtigkeit: Lieferung vereinbarter Ergebnisse
  - Angemessenheit: Eignung der Funktionen für festgelegte Aufgaben
  - Interoperabilität: Zusammenwirkung mit vorgegebenen Systemen
  - Ordnungsmäßigkeit: Erfüllung anwendungsspezifischer Normen, Vereinbarungen und gesetzlicher Bestimmungen
  - Sicherheit: Verhinderung unberechtigten Zugriffes
 
### Zuverlässigkeit
- Aufrechterhaltung eines gestellten Leistungsniveaus
  - Unter bestimmten Bedingungen/Zeiträumen
- Robustheitstests/Recoverytests, Stresstests
- **Testbereiche**:
  - Reife: Häufigkeit des Versagens durch Fehlerzustände
  - Fehlertoleranz: Wahrung eines spezifizierten Leistungsniveaus
  - Wiederherstellbarkeit: Wiederherstellung eines spezifischen Leistungsniveaus
 
### Benutzbarkeit
- Usability-Tests: Comfort und Leistung bei Bedienung durch User
- **Testbereiche**:
  - Verständlichkeit: Aufwand für User zum Verständnis
  - Erlernbarkeit: Aufwand für User zum Erlernen der Bedienung
  - Bedienbarkeit: Aufwand für User zur Bedienung
 
### Effizienz
- Performance-Tests und Lasttests
- **Testbereiche**:
  - Zeitverhalten: Antwort- und Verarbeitungszeiten, Durchsatz bei Funktionsausführung
  - Verbrauchsverhalten: Anzahl und Umfang der benötigten Betriebsmittel
 
### Änderbarkeit/Wartbarkeit
- Reviews/Code-Analyse
- **Testbereiche**:
  - Analysierbarkeit: Aufwand zur Diagnose von Mängeln
  - Modifizierbarkeit: Aufwand zur Ausführung von Verbesserungen/Fehlerbeseitigungen/Anpassung
  - Stabilität: Wahrscheinlichkeit für unerwartete Wirkungen
  - Prüfbarkeit: Aufwand zur Prüfung geänderter Software
 
### Übertragbarkeit
- Portabilitätstests: Einfachheit der Übertagung auf andere Umgebungen
- **Testbereiche**:
  - Anpassbarkeit: Möglichkeit der Anpassung an verschiedene Umgebungen
  - Installierbarkeit: Aufwand zur Installation der Software
  - Austauschbarkeit: Auswechslung von einer Software durch eine Andere
 
## Teststufen
- **Modul-, Unit-, Komponententests**: Test von Teilen der Software auf Funktionalität
- **Integrationstests**: Überprüfung des fehlerfreien Zusammenwirkens voneinander abhängiger Systemkomponenten/Schnittstellen
- **Systemtests**: Abschließender Test des Gesamtsystems
- **Abnahmetest**: Test des Gesamtsystems in der Kundenumgebung

## Testgetriebene Softwareentwicklung

### Schritte
- Schreiben eines Tests
- Implementierung des Programmcodes
- Refaktorisierung der Lösung

### Vorteile
- Qualitative Hochwertigkeit
- Geringe Wartungsintensität und Fehleranfälligkeit
- Einfache und schnelle Fehleranalyse und Wartungsarbeit
- Strukturierter Code/Systemarchitektur
- Effektive Vermeidung von Redundanzen

### Nachteile
- Ansätze nur auf Komponenten- und Unit-Ebene
- Viele kleine Einzeltests
- Kein ganzheitlicher Blick
- Schwierige Entwicklung einer guten Systemarchitektur
