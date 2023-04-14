# Netzwerktopologien

## Topologie
- Methodik der physischen Verlegung von Leitungen
- "Landkarte" des Netzes

### Stern (Star)
- Sternmittelpunkt mit Leitungen zu allen Endpunkten
- Zugriffssteuerung CSMA/CD

![image](https://user-images.githubusercontent.com/104757507/231986907-031bc534-f950-4a33-8ed8-ae3c58745583.png)

### Erweiterter Stern (Extended Star)
- Endpunkt eines Sterns = Mittelpunkt eines weiteren Sterns
- 3 Ebenen üblich bei LANs
- Standard in heutigen Verkabelungen

![image](https://user-images.githubusercontent.com/104757507/231987353-68b2dece-deab-4620-a34d-3c1d4b600e95.png)

### Vollständige Masche (Complete Mesh)
- Jede Station mit Jeder verbunden
- Sehr hohe Ausfallsicherheit durch hohe Redundanz
- Sehr aufwändig

![image](https://user-images.githubusercontent.com/104757507/231988105-750bad6a-3470-4c1d-b202-3ed4d2d2cd0f.png)

### Unvollständige Masche (Incomplete Mesh)
- Wichtige Stationen mehrfach mit anderen Stationen verbunden
- Ausfallsichere Netze durch Redundanz
- (Erweiterter Stern mit Querverbindungen)

![image](https://user-images.githubusercontent.com/104757507/231988710-f5c4bd74-6adc-4ee9-af12-8f577f4949e2.png)

### Zelle (Cell)
- Funkzellen decken bestimmte Bereiche mit Funkwellen ab
- Zugriffssteuerung CSMA/CA

![image](https://user-images.githubusercontent.com/104757507/231989214-ccd701c7-9d0a-466c-b62b-776d324236d5.png)

### Punkt-zu-Punkt (Point-to-Point, P2P)
- Verbindung von zwei Stationen

![image](https://user-images.githubusercontent.com/104757507/231989518-8d3ebd5a-9dcf-45d5-a5f5-e1f301d4c15d.png)

### Bus
- Alle Stationen parallel auf gemeinsamer Leitung
- Unüblich in LANs
- Zugriffssteuerung CSMA/CD

![image](https://user-images.githubusercontent.com/104757507/231989779-424a8734-d8ca-4933-8a12-036dc30ec514.png)

### Ring
- Jede Station hat Vorgänger- und Nachfolgerstation
- Senden von Daten nur in eine Richtung
- Sichere Datenübertragung, berechenbare Wartezeit
- Schwieriger Aufbau, schwierige Fehlersuche
- Zugriffssteuerung über Token Passing

![image](https://user-images.githubusercontent.com/104757507/231990220-f4fe8412-124e-4cf7-8d5e-87081aac8a88.png)
