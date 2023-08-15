# Sicherheit bei Softwareplanung

## Sicherheitsprinzipien

### Minimalprinzip
- So viel wie nötig, so wenig wie möglich
- Berechtigungsvergabe nach Notwendigkeit
  - Nötige Berechtigungen zur reibungslosen Arbeit
 
### Separierung von Berechtigungen
- Bestimmte Nutzer - Bestimmte Funktionszugriffe

### Vollständige Zugriffsüberwachung
- Monitoring zur Vermeidung unberechtigter Zugriffe

### Mehrere Sicherheitsebenen
- Austeilung von Software in Sicherheitsebenen
- Kein Single Point of Failure
  - Weniger angreifbare Schwachstellen
 
### Sicherer Ausfall
- Gesicherte Vertraulichkeit und Integrität auch im Ausfallsfall

### Benutzerfreundliche Sicherheit
- Sicherheitsmechanismen = keine Beeinträchtigung für User-Experience

## Design- und Umsetzungshinweise

### Trennung von Datenverarbeitung und -verwaltung
- Aufteilung des Programms in verschiedene Einheiten für unterschiedliche Funktionen
- Verwendung eines MVC-Patterns (Model-View-Controller)

### Validierung der Daten vor Verarbeitung
- Konsequente Überprüfung von Ein- und Ausgabe, Parametern und Methoden
- Wahl richtiger Datentypen und Wertebereichen

### Sichere Datenübertragung
- Implementierung von Verschlüsselungen
- Ggf. Anwendung von Frameworks für Übertragungsverschlüsselung

### Sichere Benutzerverwaltung
- Vollständige Berechtigungsprüfung
- Implementierung einer sicheren Login-Funktionalität

### SOAP- und REST-Schnittstellen
- Filterroutinen in Abhängigkeit der Datenformate
- Prüfung aller Daten anhand einer Whitelist

### Unittests
- Tests während Entwicklungseinheiten
- Erstellung von Unittests für jede Funktion
- Nutzung automatisierter Unittests

### Verhinderung von SQL-Injections
- Überprüfung erstellter SQL-Anweisungen

### Protokollierung
- Informationsbereitstellung bei Sicherheitszwischenfällen oder Fehlern
- Erstellung von Log-Dateien oder Protokollen
- Einhaltung aktueller Datenschutzbestimmungen


