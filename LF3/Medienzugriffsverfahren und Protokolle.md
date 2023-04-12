# Medienzzugriffsverfahren und Protokolle

## Medienzugriffsverfahren

### Zentrale Steuerung

Zentrale Station erteilt Sendeerlaubnis an die angeschlossenen Stationen

-> Einsatz in Funknetzen (WLAN) durch RTS/CTS-Pakete (RTS = Request to Send = Sendeanfrage und CTS = Clear to Send = Sendeerlaubnis)

### Carrier Sense Multiple Access/Collision Detection (CSMA/CD)

- **Carrier Sense**:
- Trägererkennung
- Abhören des Mediums (frei?)

- **Multiple Access**:
- Mehrfachzugriff

- **Collision Detection**:
- Kollisionserkennung
- Prüfung während des Sendens (sendet andere Station dazwischen?)

-> Einsatz bei Ethernet

### Carrier Sense Multiple Access/Collision Avoidance (CSMA/CA)

- Kollisionsverhinderung durch Abhören des Mediums
- Anschließendes Abwarten einer bestimmten Zeit vor dem Senden

-> Einsatz in Funknetzen (WLAN)

### Token Passing

- Token ist Sendeerlaubnis
- Ringförmige Weitergabe des Tokens nach dem Senden eines Pakets

-> Einsatz bei Token-Ring und Glasfaserringen


## TCP/IP-Protokolle

### Interpet-Protocol (IP)

- IP-Adressen adressieren Netzwerke und Rechner
- Routing von IP-Paketen anhand der IP-Adresse
- Unabhängig von verwendeter Übertragungstechnik
- Verbindungslos, ohne Quittung oder Rückmeldung

### Transmission Control Protocol (TCP)

- TCP-Adressen (TCP-Ports) addressieren Applikationen
- Unabhängig von verwendeter Übertragungstechnik
- Verbindungsorientiert - Verbindungsaufbau und -haltung vor Datenübertragung
- Sichere Übertragung - Überprüfung und Quittierung der Zustellung, Nachlieferung fehlender Datensegmente
- Steuerung des Datenflusses, Eingriff zur Stauverhinderung (Congestion Control)

### User Datagram Protocol (UDP)

- UDP-Adressen (UDP-Ports) addressieren Applikationen
- Unsichere Übertragung - Keine Zustellungsüberprüfung, nicht quittiert, keine Nachlieferung fehlender Datensegmente
- Sendung als Datenströme
- Kleiner Header (einfacher als TCP) - weniger Protokoll-Overhead, schnellere Auslieferung
- Anwendung bei Multicast
- Keine Datenflusssteuerung, keine Stauverhinderung
- Unabhängig von verwendeter Übertragungstechnik
- Verbindungslos
