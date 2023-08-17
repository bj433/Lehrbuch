# Machine-to-Machine und OPC UA

## Machine-to-Machine
- Automatisierter Informationsaustausch zwischen Maschinen
- Kommunikation zwischen einzelnen Maschinensteuerungen und zentraler Leitstelle

## OPC UA
- Open Platform Communications Unified Architecture
- Industriestandard für Kommunikation zwischen Maschinen (und Maschinen/und Computersystemen)
- Offener Schnittstellenstandard

### Architektur

#### Topologie
- Verwendung eines TCP-basierten Protokolls
- Zuweisung auf Port 4840
- Binärer Datenaustausch
- Verwendung des Webservice-Protokolls
- Zuweisung auf Ports 80 und 443

#### Client-Server-Prinzip
- Bereitstellung von Daten/Informationen durch den Server für Clients
- Gerät = Client und Server gleichzeitig

#### Konfiguration
- Adressierung durch IP-Adresse/Gerätenamen
- Möglicher Aufbau von zusätzlich authentifizierten/signierten/verschlüsselten Verbindungen
- Automatische Konfigration des OPC-Clients

#### Sicherheit
- Sicherstellung der Informationssicherheit hinsichtlich Vertraulichkeit, Integrität und Verfügbarkeit
- Zugriffskontrolle mit Authentifizierung, Autorisierung und Auditierbarkeit
- Verschlüsselte und signierte Nachrichtenübertragung
