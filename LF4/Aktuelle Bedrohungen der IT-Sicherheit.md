# Aktuelle Bedrohungen der IT-Sicherheit

## Cyberangriffe

### Angriffsziele
- Ablenkung, Behinderung
- Belauschung, Datendiebstahl, Diebstahl personenbezogener Daten, Erpressung, Ideendiebstahl
- Schädigung im Wettbewerb, Systemüberlastung
- Unternehmensziele oder politische Ziele zulasten Anderer erreichen
- Verschleierung, Öffnung verschlossener Bereiche

### Angriffsvektoren
- Kombination von Angriffsweg- und technik
- Zugang zu IT-Systemen durch Angreifer

### Angriffswege/-objekt
- Datenkommunikation, Netzwerk
- Web, E-Mail
- Datenspeicher (Geräte, Chips, Speicher, Karten)
- Hardware (Netzwerk, Client, Peripherie, IoT, Adapter, USB, industrielle Steuersysteme, Schnittstellen, Leitungen, Übertragungswege)
- Protokolle, OS, Software, Treiber, Bibliotheken
- Menschen, Nutzer, Social Engineering
- Täuschung, Machine Learning
- KI-basierte Wege und Objekte

### Angriffstechnik
- Code-Injection
- Diebstahl
- Network-Angriffe
- Schwachstellenausnutzung
- Spam, Trojaner, Malware

### Angriffsarten
- Ausnutzung von Schwachstellen
- Informationsdiebstahl
- Physische Manipulation von Geräten
- Man-In-The-Middle-Angriffe (zwischen Sender und Empfänger)
- DoS und DDoS (Angriffe durch Botnets)
- Malware (Schadsoftware - Trojaner, Backdoors, Ransomware)


## Schadsoftware - Malware

### Adware
- Platzierung von Schadsoftware durch Werbungen

### Credential Stuffing
- Angriff auf Login-Mechanismen von E-Commerce oder Serviceanbietern
- Automatisiert
- Verwendung von geleakten oder generierten Benutzernamen- und Passwortkombinationen

### Nicknapping
- Auftritt eines Angreifers unter einem bekannten Namen/Pseudonym

### Malware
- Malicious Software
- Unauffälliges Befallen von IT-Systemen
- Mögliche Nachladung von Schadmodulen oder Backdoors
- Lahmlegung von Rechnern, Spionage, Spamming von Werbung
- **Mögliche Folgen**:
  - Betriebsstopp
  - Entlassung von Mitarbeitern
- Hohe Zahlen täglich neuer Schadsoftware
  - Umgehung von Virenschutz-Programmen
  - Ausnutzung von Sicherheitslücken

### Viren
- Anrichtung ungewollten Schadens
- Boot-Sektor-Virus, Dateivirus (Eintragung in Bootbereich eines Datenträgers oder andere Dateien)

### Würmer
- Unterklasse des Virus
- Eigenständige Übertragung durch Nutzung vorhandener Infrastruktur
- Z.B. E-Mail-Programm -> Verteilung an alle Adressen im Adressbuch

### Trojaner
- Vortäuschung echter Anwendungen
- Öffnung einer Backdoor im Computersystem zwecks Zugriff anderer Schadsoftware
- Keine selbständige Vermehrung

### Verbreitung
- **Herunterladen infizierter Anhänge**
  - Meist Bestandteil interessanter E-Mails
- **Drive-by-Infection**
  - Automatische Installation von Schadsoftware beim Aufrufen präparierter Websites
- **Soziale Netzwerke**
  - Verbreitung infizierter Anhänge und entsprechender Links
- **Spear-Infection**
  - Persönlich adressierte Phishing-/Infektionsmails
  - Informationsbeschaffung, Infektion des Rechners des Opfers

### PUA (Potentially Unwanted Application)
- Häufig gesuchte Software als Freeware ausgegeben
- Malware integriert, erfüllt nicht die gewünschten Funktionen
- Löschung beseitigt Malware nicht, wird bei bestimmten Ereignissen dann aktiviert

### Ransomware
- Einschränkung/Verhinderung von Daten-/Systemzugriff durch Schadprogramme (Verschlüsselungstrojaner)
- Freigabe nur nach Lösegeldzahlung
- Angriff auf Sicherheitsziel der Verfügbarkeit
- Digitale Erpressung

### Scareware
- Angstsoftware
- Vortäuschung von System-/Warnmeldungen
- Nutzer sollen Schadsoftware aus Angst installieren
- Oft als Anti-Virenprogramm ausgegeben

### Spam
- Unerwünschte Nachrichten in großen Massen (meist ungezielt)
- Häufig nur Werbung, oftmals mit Phishing-Anhängen
- Abgrenzung in:
  - Phishing (Abfischen von vertraulichen Daten)
  - Spearing (Beschaffung weiterer Gewinnmöglichkeiten mit gezielt besorgten persönlichen Daten)
  - Hoaxes (Falsch-/Scherzmeldungen)
  - Skimming (Mails mit Gewinnversprechen)

### Prävention
- Prüfung von Seriösität von Websites und Mails
- Absenderkontrolle
- Sofort löschen, nicht weiterleiten


## Große Cyber-Attacken

### Advanced Persistent Threats (APT)
- Gezielte Cyber-Angriffe auf Unternehmen/Organisationen
- Ziel: Dauerhafter Netzwerkzugriff
- Hoher Ressourceneinsatz und Kenntnisse der Angreifer

### Bot/Botnetze
- Ferngesteuerter Verbund von gehackten Rechnern, Smartphones, IoT
- Command-and-Control-Server (C&C-Server) zur zentralen Steuerung
- Betreiber bieten Attacken als Dienste an

### DoS (Denial of Service)
- Denial of Service = Dienstverweigerung
- Provozierter Zusammenbruch eines Servers aufgrund von Massenanfragen
- **Syn Flooding**:
  - Computer erhält Syn-Pakete
  - Anstatt eigener Absenderadresse -> gefälschte IP-Adresse (auch existent)
  - Systemanfragen gehen ins Leere
- **Ping Flooding**:
  - Ausnutzung des Programms *Ping*
  - Angreifer bombardiert Zielrechner mit Pings
- **Mailbombing**:
  - Belastung des Mailservers durch extrem lange, oder viele Mails

### DDoS (Distributed-Denial-of-Service-Attacken)
- Überlastung eines Zielsystems und dessen Services
- Botnets als Angriffsobjekt
