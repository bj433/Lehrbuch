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
- 
