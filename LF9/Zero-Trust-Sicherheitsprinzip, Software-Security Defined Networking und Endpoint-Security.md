# Zero-Trust-Sicherheitsprinzip, Software-Security Defined Networking und Endpoint-Security

## Zero-Trust-Sicherheitsprinzip, -Methode/-Architektur
- "Was" als Mikroperimeterebene = zu schützende Angriffsfläche
  - Daten, Anwendungen, Ressourcen, Dienste
- Netzwerksegmentierung
- Strenge Zugriffskontrollen
- NGFW als Segmentierungs-Gateways
  - Zulassung einzig bekannten, legitimen Datenverkehrs
  - Transparenz im Datenverkehr
  - Zugriffsteuerung nach Kipling-Methode
    - Wer, Was, Wann, Wo, Warum und Wie
- Zero-Trust-Architektur nach 5-Schritt-Methode:
  - Identifikation der Schutzoberfläche
    - Öffentlich, Intern, Vertraulich
  - Erkennung und Optimierung der Transaktionsflüsse aller sensiblen Daten
  - Entwicklung eines Zero-Trust-Designs
    - Sicherheitsprotokolle, NGFW, NSX oder SDN/SDDC
  - Zero-Trust-Richtlinien nach Kipling-Methode
  - Sicherstellung der Automatisierung, Überwachung und Wartung
 
### Software Defined Networking (SDN)
- Entkopplung von Hard- und Software
- Zentrale Verwaltung von Netzwerkkomponenten
- Hardware einzig für Weiterleitung von Datenpaketen
- Control Plane und Data Plane
  - Control Plane:
    - Vergabe von Anweisungen
  - Date Plane:
    - Ausführung von Anweisungen
- Network-Controller als zentrales Steuerungselement im Netzwerk
  - Verwaltung und Steuerung von Routern und Switches
- Informationsspeicherung und -verarbeitung durch Netzwerkbetriebssystem
- Flexible Erweiterbarkeit des Netzwerks
- Änder- und Managebarkeit
- Keine Abhängigkeiten zu Geräteherstellern
- Southbound-Interface zur Kommunikation zwischen Control- und Data-Plane
- Northbound-Interface zur Automatisierung und Orchestrierung von Applikationen, Management- und Kontrollprogrammen

### Bedrohungsscanner, OpenVAS und Security Manager
- Untersuchung von Zielsystemen nach Sicherheitslücken
- Proaktive Asset-Erfassung durch Schwachstellen-Management
- Kontinuierliches Monitoring
- Eindämmung, Behebung und Verteidigung von Cyberangriffen

### Sicherheits-Gateway als SaaS, Secure Access Service Edge (SASE)
- Secure Web Gateways als Abwehr bei Cloud-Netzen
- Erkennung und Einschränkung von DNS-Datenextraktionen und Zero-Day-Angriffen
- Herstellung gesicherter Netzverbindungen zu Cloud-Diensten
- Kombination von Netzwerk- und Security-as-a-Service-Funktionen
- Möglichkeit zu verteiltem Sicherheitscontrolling, Richtlinienmanagment und Ressourcenerweiterung

### Security-Information-and-Event-Management-Systems (SIEM)
- Echtzeitanalysen von Datenströmen, Anwendungs-/Benutzer-/Serververhalten, Log-Events, bekannten Schwachstellen
- Einsatz als IPS
- Verwendung von Machine Learning, UEBA (User and Entity Behaviour Analytics) und SOR (Security Orchestration, Automation and Response)

### Netzwerksegmentierung
- Klassifizierung und Segmentierung des Unternehmensnetzwerks
- Einteilung nach Vertrauenszonen und Sicherheitsrichtlinien
- Zugriffseinschränkung
- Verkleinerung der Angriffsfläche
- Vereinfachte Zugriffskontrolle
- Complianceverbesserung


## Endpoint-/Enduser-Security

### Multi-Faktor-Authentifizierung oder Single-Sign-On (SSO)
- Einsatz sicherer Anmelde- und Berechtigungssysteme
- Regelmäßige Identitätsüberprüfung von Usern durch Access Management
- Einsatz biometrischer Merkmale, Token oder Smart Cards
- Zero-Trust als Strategie

### Endpoint-Protection-Suite-Pro
- Installation einer leistungsstarken Antiviren-Software

### VPN (Virtual Private Network)
- Geschützte Netzwerkverbindung
- Datenverkehr durch virtuelle Tunnel mit Echtzeitverschlüsselung
- IP-Adresse und Online-Identität versteckt
- SSL-VPN, Site-to-Site-VPN, Client-to-Client-VPN
- Kein Schutz für Daten auf Endgeräten

### Social Engineering und Zero-Trust-Strategie
- Sensibilisierung und Information von Usern zu Vertraulichkeitspflichten bei Arbeit mit PCs, Passwörtern und Software

### Verschlüsselung vertraulicher Dateien und E-Mails
