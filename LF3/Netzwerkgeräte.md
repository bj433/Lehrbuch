# Netzwerkgeräte

## Repeater und Hub
- **Hub** = Bidirektionaler Verstärker
  - Arbeit auf OSI-Layer-1 (Bitübertragungsschicht/Physical Layer)
- **Repeater** = Hub mit zwei Anschlüssen
- Keine Adressauswertung

## Bridge und Switch
- **Bridge** = Verbindung zweier Netzsegmente
- Mehrere MAC-Adressen pro Netzsegment für meherere Geräte
- Weiterleitung nur bei Anbindung an andere Bridge-Ports
  - Filterung unnötigen Netzwerkverkehrs
- Bildung von Weiterleitungstabellen/Bridge Table durch die Bridge
- **Switch** = Multiport-Bridge
- Bildung von Weiterleitungstabellen/Forwarding Table/Switching Table/Bridge Table
  - Auflistung der angebundenen Knoten
- Inspektion auf OSI-Layer-2 und Auslesung der MAC-Adressen im Header
- Eingangs-/Ausgangspuffer an jedem Switchport
  - Input-FIFO (First In - First Out)
- Zugriffssteuerung zwischen Pufferspeichen und Anschlüssen
  - Vermeidung von Datenkollisionen
- Switching Fabric = Weiterleitung von empfangenen Daten an entsprechende Ausgangsports
  - Schnelles internes Netzwerk
- Fehlergefahr:
  - Überlaufen des Pufferspeichers bei zu schneller Datenübertragung
  - Keine Datenflusssteuerung
    - Datenverlust

### Switchtypen
- Zeitbezogene Bestimmung der Datensendung
- Unterteilung der Nutzdaten in Ethernet-Frame, Header und Trailer
- 1. Präambel (Synchronisierungsbits ohne Informationsgehalt)
  2. Ethernet-Header
  3. Nutzdaten
  4. Rahmenprüfsumme (Frame Check Sequence)
 
#### Cut-Through-Switch
- Weiterschicken von Daten nach Empfang der Zieladresse
- Latenzzeit Ein-/Ausgang: 14-Byte-Zeiten
- Geringer Speicherbedarf
- 6 Byte Eingangspuffer
- Sendung trotz Fehler/Unvollständigkeiten

#### Store-and-Forward-Switch
- Weiterschicken von Daten nach Empfang des kompletten Frames und der Überprüfung der Rahmenprüfsumme
- Weiterleitung einzig von fehlerfreien Frames
  - Aussortierung defekter Frames
  - Einsparung von Datenaufkommen
- Latenzzeit Ein-/Ausgang: Ganze Rahmenzeit - max. 1.518 + 8-Byte-Zeiten

#### Fast-Forward-Switch/Fragment-free-Switch
- Weiterschicken von Daten nach Anfang der Datenübertragung
- Latenzzeit Ein-/Ausgang: 64 empfangene Bytes
- Geringer Speicherbedarf



## Router
- Verbindung mehrerer Netzwerke miteinander
  - Auswertung des Netz-Anteils der IP-Adresse
- Routing-/Weiterleitungstabellen mit Adressenbereichen (Netzkennungen)
- Hinterlegung erreichbarer Netzwerke pro Routerport
- Unterteilung großer Netzwerke mit Subnetting
- Auswertung von Netzwerkadressen in OSI-Layer-3

## WLAN-Access-Point, WiFi-Access-Point, Hotspot
- Mittelpunkt einer Funkzelle mit LAN-Anbindung
- Verbindung von Mobilgeräten


