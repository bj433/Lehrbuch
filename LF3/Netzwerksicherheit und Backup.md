# Netzwerksicherheit und Backup

## Daten- und Netzwerksicherheit

### RAID
- Redundant Array of Independent Discs
- Genormte Level (1-6) für Festplattenverbunde
  - Zusammenschaltung mehrerer Festplatten
  - Erhöhung der Schreib- und Lesegeschwindigkeit
  - Datenverfügbarkeit
 
### Backup
- Sicherung der Massenspeicher auf einen anderen Datenträger
- Wiederherstellbarkeit von Daten bei Datenverlust
  - Bspw.:
    - Löschen/Überschreiben von Dateien
    - Verlust der Daten
    - Defekt oder äußere Einflüsse
   
### Bandsicherung
- Backup auf Magnetband

### Cloud-Backup
- Backup auf Online-Datenspeicher

### Proxy
- "Stellvertreter"
- Übernahme des Internetzugriffes für Arbeitsplatzrechner

### Firewall
- Blockade für Angriffe/unerwünschte Daten

### DMZ
- Demilitarisierte Zone
- Netz zwischen zwei Firewalls/zwischen Internet und LAN

### Schutzbedarfsanalyse
- Systematische Analyse der gesamten IT
- Erarbeitung von Schutzmechanismen

### Zugriffsrechte/Berechtigungen
- Bestimmung von Zugriffsberechtigungen auf Daten und Ressourcen für Benutzer und Gruppen

### Zugangskontrolle
- Passwortsicherheit
- Kontrolle über Zugänge durch Logins und auf physische Umgebungen/Komponenten

### Leitungscodes
- Minimierung von Übertragungsfehlern

### "Faktor Mensch"
- Menschliches Versagen als größte Schwäche von Datensicherheit

## Möglichkeiten der Datensicherung

### Off-Premises Backup
- Kopie von Datena auf anderes Datacenter

### Bandsicherung
- Sicherung auf Bändern

### Cloud-Backup
- Kopie auf Cloud-Speicher im Internet

### Speicherabbild-Backup/Image Backup
- Sicherung aller Datenblöcke auf einer Festplatte
  - Dateisystem
  - Gelöschte Daten
- Verwendung bei Computer-Forensik

### Voll-Backup/Komplettsicherung
- Sicherung aller Daten auf einer Platte

### Differentielles Backup
- Sicherung aller veränderten Daten auf einer Platte (seit letztem Voll-Backup)
- Rücksicherung nur mit letzter differentieller Sicherung

### Inkrementelles Backup
- Sicherung aller veränderten Daten auf immer neuen Platten (seit letztem Backup)
- Rücksicherung mit allen Platten

