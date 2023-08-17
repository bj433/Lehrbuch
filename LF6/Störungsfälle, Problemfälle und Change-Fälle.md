# Störungsfälle, Problemfälle und Change-Fälle

## IT-Störungsfälle
- Temporärer oder endgültiger Ausfall von IT-Systemen
- Temporäre Druckerausfälle
- Flackernde Bildschirme
- E-Mails (Senden und Empfangen)
- Serverausfall
- Langsame oder gestörte Netzverbindungen im Netzwerk

### Typische Netzwerkprobleme
- Probleme in der Verkabelung:
  - Duplex Mismatch (Fehlercounter des Switchports)
  - Broadcast-Stürme
  - Unterschiedliche Encapsulation (Datenkapselung) im Ethernet
  - Doppelte MAC-Adresse
  - DHCP funktioniert nicht
  - Doppelte IP-Adressen/Hostnamen/Loopback-Adressen
 
### Hilfen, Tools und Werkzeuge
- Treiberprobleme:
  - Herstellerwebseite
  - Einschlägige Treiberseiten
  - Produktbezeichnung und Hersteller
- Kabeltester/Multimeter
- Netzwerk Sniffer (Wireshark)

## Problemfälle

### Ziel
- Untersuchung von Ursachen für wiederkehrende Störungen oder Unzulänglichkeiten
  - Behebung der Ursache
  - Vermeidung von Wiederauftreten von Störungen
- Verfügbarkeit von Workarounds

### Problem
- Ursache eines/mehrerer Incidents
- Verhinderung gleichartiger Incidents
- Reduktion von Negativwirkung auf Services

### Bekannter Fehler
- Bekanntes, nicht beseitigtes Problem
- Existenz eines Workarounds/Übergangslösung
- Pflege einer Lösungsdatenbank

### Anforderungen von FitSM
- PR10.1:
  - Identifikation und Registrierung von Problemen mit Trendanalysen nach Incidents
- PR10.2:
  - Untersuchung von Problemen
  - Identifikation von Beseitigungsmaßnahmen
  - Reduktion von Auswirkungen auf Services
- PR10.3:
  - Erfassung von vorliegenden Problemen als "bekannter Fehler"
  - Effektive Workarounds
- PR10.4:
  - Pflege von bekannten Fehlern und Workarounds
 
### Beispiele

#### Hardware
- Veraltete Hardware ohne Herstellersupport, Sicherheitsrisiken
- Bootfehler/Bootloop des PCs
- Festplattendefekt
- Malwarebefall
- Fehlerhafte Drucke
- Lange PC-Ladezeiten
- Fehlendes Zubehör
- Kein mobiler Netzwerkzugriff für Laptops

#### Software
- Browser:
  - Anzeigefehler einzelner Seiten/Inhalte
  - Keine Öffnung von PDF-Files möglich
- E-Mail:
  - Keine mobile Nutzung
- Geforderte Updates/Upgrades
- Hoher Aufwand durch Menge an Client-Betriebssystemen

#### Netz
- Langsame Netzwerkverbindung
- Temporäre Netzstörung

#### Sicherheit
- Sicherheitsrisiken in Infrastruktur und Anwendungen
- Unsichere Netzverbindung mit mobilen Rechnern

## Changefälle

### Continual-Service-Improvement-Management (CSI-Management)
- Überprüfung und Verbesserung von Services
  - Bearbeitung von Verbesserungsvorschlägen
  - KPI-Analysen
  - Kundenfeedbacks
  - Beschwerden
  - Umfragen
  - Service-Reviews
  - Berichte
- Vorgehen:
  - PDCA, KVP
  - Lifecycle-Prozesse
  - Bewertungen über IT-Assessments
  - Verbesserungssysteme
  - Einsatz DevOps lean/reduzierte, agile Ansätze
 
### Change-Management in der IT
- Hinzufügen, Modifizieren oder Entfernen eines Elements
  - Auswirkungen auf IT Services möglich
- Verantwortung und Steuerung von Change-Prozessen mit wenig Reibungsverlusten
- Umfang:
  - IT-Services
  - Configuration Items
  - Prozesse
  - Dokumentationen
- Request for Change = Antrag zur Durchführung eines Changes

### Klassifizierung
- Standard Change = Bearbeitung im Request Fulfillment
- Level-1 Change = Geringe Auswirkungen auf IT-Infrastruktur
- Level-2 Change = Deutliche Auswirkungen auf IT-Infrastruktur
- Level-3 Change = Signifikante Auswirkungen auf IT-Infrastruktur
