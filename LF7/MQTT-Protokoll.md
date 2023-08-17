# MQTT-Protokoll

- Message Queue Telemetry Transport
- Machine-to-Machine-Kommunikation
- Nutzung eines Publisher-Subscriber-Musters
  - Eignung für einfache Kommunikation zwischen kleinen IoT-Geräten
- Kein Sicherheitsmechanismus

## Begriffe

### MQTT-Broker
- Weiterleitung von Nachrichten zwischen Sender und Empfänger
- Einteilung in zwei Gruppen:
  - Native Broker
    - Für MQTT entwickelt
    - Kleiner als normale Broker
  - Unterstützung via Connector

### MQTT-Client
- Publisher/Subscriber
- Aktive MQTT-Bibliothek
- Verbindung mit MQTT-Broker über Netzwerk

### MQTT-Topic
- Filterung von Client-Nachrichten
- Struktur:
  - Keinen Schrägstrich zu Beginn eines Topics
  - Keine Leerzeichen
  - Kurze Topics
  - Keine Sonderzeichen
  - Case Sensitivity
 
### Topic-Wildcard - einstufig
- Platzhalter zum Abonnieren mehrerer Topics
- Nicht zum Senden von Nachrichten
- "+" als  Ersatz für ein Topic-Level

## Quality of Service und Last Will Testament
- Zuverlässigkeit der Nachrichtenzustellung
- Einteilung in drei Stufen
  - Definierte Verbindlichkeit
1. QoS 0: At most once - höchstens einmal
2. QoS 1: At least once - mindestens einmal
3. QoS 2: Exactly once - genau einmal
4. Last Will Testament: Information bei Verbindungsabbrüchen

## Verbindungsmanagement zwischen Client und Server

### Retained Messages - eine zurückgehaltene Nachricht
- Neusubscriber erhält zuletzt gesendete Nachricht im Topic
- Last Valve Queue

### Persistent Sessions - eine dauerhafte Verbindung
- Längere Laufzeit als physikalische Netzwerkverbindung
- Möglicher Stop/Wiederaufnahme einer Session
- Eindeutige Identifikation von Sessions über Client Identifier

### Keep Alive
- Zeitvorgabe für Aufrechterhaltung inaktiver Verbindungen
- Automatische Verbindungstrennung bei Überschreiten der Zeitvorgabe
- Unterbrechung der Zeitvorgabe durch PINGREQ-Paket von Client
- Überprüfung der Netzwerkverbindung des Servers durch PINGREQ

### Web Socket Transport
- MQTT over Web Sockets für Push-Nachrichten
- Verbindung Webbrowser -> Broker
