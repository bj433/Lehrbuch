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
- 
