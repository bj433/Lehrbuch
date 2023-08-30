# Planung und Integration eines Netzwerks

## Wichtige Aufgaben
- Planung
- Einbindung von Clients
- Test und Dokumentation der Einrichtung
- IP-Konfiguration
  - IP-Adresse
  - Subnetzmaske
  - DNS-Adresse
- Dateidienste
- Netzwerkdrucker
- Netzwerkdose
- Router-Adresse (Gateway)
- Patch auf Switchport
- Einrichtung des Zugangs auf Netzwerkdienste

## Wichtige Anforderungen und Fragestellungen

### Netzwerklast und aktuelle Netzwerktechnologie
- > Wie lange ist die Ladezeit bei verschiedenen Netzwerkstandards?
- > Wie lange ist die Speicherzeit beim Beenden bei verschiedenen Netzwerkstandards?
- > Wie lange sind die Speicherzeiten bei verschiedenen Netzwerkstandards?
- > Welche Netzwerktechnologie mit welcher Datenrate ist aktuell installiert?
  
### IP-Konfiguration
- > Welche Netzkennung (Net-ID) hat das Netzwerk? Wie groß ist der Adressbereich?
- > Welche IP hat der Router (Default Gateway)?
- > Welche IP hat der DNS-Server?
- > Ist ein DHCP-Server vorhanden?
- > Sind Subnetze im LAN vorhanden?
  
### LAN-Ausbau
- > Ist die Lage von Dosen und Verteilern bekannt?
- > Wie sind Dosen und Verteiler bezeichnet?
  - > Sind die Lagepläne auf dem neusten Stand?
- > Sind Leitungen dokumentiert?
  - > Welcher Standard wird erreicht, welcher Datendurchsatz?
  - > Sind Messprotokolle vorhanden?
- > Sind Patch-Pläne bekannt?

## Einbindung von Clients ins Netz

### Rechner
- Herstellung eines Hardwareanschlusses:
  - > Anschlüsse vorhanden?
    - > Passt die Kategorie der Dose zur gewünschten Übertragungsrate?
    - > Verteiler und Anschlussbuchse dieser Leitung suchen
    - > Freien Switchport suchen
  - > Verbindungsschnüre prüfen, ob Kategorie passt
  - > Verbindungen herstellen (patchen):
    - Rechner -> Anschlussdose
    - Switchport -> Anschlussbuchse im Verteiler
- Herstellung eines logischen Anschlusses:
  - Rechner hochfahren und testen:
    - > Hat der Rechner seine IP-Konfiguration bekommen?
    - > Wenn nicht, am PC die Netzwerkeinstellungen auf "IP automatisch beziehen" einstellen
    - > Sind die Server erreichbar?
    - > Ist das Internet erreichbar?
- Testen und Dokumentieren:
  - Ping auf Internetseite
    - Prüfung der Namensauflösung (DNS)
    - Prüfung der Erreichbarkeit des Routers
    - Prüfung des Zugangs zum Internet
  - Konsolenbefehl ipconfig für aktuelle IP-Konfiguration
    - Stimmt die IP-Adresse
  - Dokumentation des Rechnernames und nähren Angaben
    - Anschlussdose
    - IP-Adresse
    - Betriebssystem
    - etc.
   
## Netzwerkmanagement

### Reaktives Management
- Reaktion auf auftretende Probleme und Fehler

### Proaktives Management
- Präventive Wartungen
