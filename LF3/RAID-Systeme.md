# RAID-Systeme

## RAID 0
![image](https://github.com/bj433/Lehrbuch/assets/104757507/2cf51eb9-79cd-4623-9b2b-ae8d560db545)

- Stripe Set
- Zusammenschaltung beliebiger Festplatten/Partitionen zu einem Volume
- Verteilung von Daten auf mehreren Platten
- Höhere Datenraten beim Lesen und Schreiben
- Sicherheit:
  - Keine
  - Ausfall einer Platte = Beschädigung des gesamten Volumes
 
## RAID 1
![image](https://github.com/bj433/Lehrbuch/assets/104757507/8146ac25-4327-4365-9fa5-98bf28304421)

- Mirroring
- Spiegelung von zwei Platten miteinander
- Einfache Lesegeschwindigkeit, doppelte Schreibgeschwindigkeit
- Sicherheit:
  - Ausfall einer Platte = Kein Datenverlust
 
## RAID 4
![image](https://github.com/bj433/Lehrbuch/assets/104757507/eafbec34-ed4f-4e84-a884-917e9d9b8004)

- Stripe Set with Parity
- Mind. drei Platten im Verbund
- Separate Paritätsplatte
  - Starke Beanspruchung durch Beschreibung bei jedem Beschreiben
- Sicherheit:
  - Ausfall einer Platte = Kein Datenverlust
 
## RAID 5
![image](https://github.com/bj433/Lehrbuch/assets/104757507/8afa6040-30b6-46f7-8a8e-0517e862d186)

- Stripe Set with Parity
- Mind. drei Platten im Verbund
- Verteilung der Parität auf allen Platten
- Gleichmäßige Beanspruchung
- Sicherheit:
  - Ausfall einer Platte = Kein Datenverlust
 
## RAID 6
![image](https://github.com/bj433/Lehrbuch/assets/104757507/501e2b8d-48a2-4464-8eb4-1783be1605ab)

- Stripe Set with Parity
- Mind. vier Platten im Verbund
- Verteilung von zwei Paritäten auf allen Platten
- Sicherheit:
  - Ausfall von zwei Platten = Kein Datenverlust
 
## RAID 0+1
![image](https://github.com/bj433/Lehrbuch/assets/104757507/bb3e5477-2aa7-4118-8b84-1bb543d0a818)

- Spiegelung von zwei RAID 0 mit einem RAID 1
- Sicherheit:
  - Doppelte Ausfallwahrscheinlichkeit pro RAID 0
  - Ausfall eines RAID 0's = Kein Datenverlust
 
## RAID 1+0
![image](https://github.com/bj433/Lehrbuch/assets/104757507/8f97e7c9-0623-4907-a14f-80915d7dfa78)

- Zusammenschaltung von zwei Spiegelsystemen über ein RAID 0
- Sicherheit:
  - Ausfall einer Platte pro RAID 1 = Kein Datenverlust
  - Ausfall von zwei Platten in einem RAID 1 = kompletter Datenverlust

## Hardware-RAID
- Erweiterungskarte für Mainboards
- Wertung vom Betriebssystem als eine Festplatte
- Vorteile:
  - Hohe Geschwindigkeit
  - Zusätzlicher Festplattencache
- Nachteile:
  - Kosten für Controller

## Software-RAID
- Herstellung von RAID-Systemen durch vorhandene Festplatten
- Vorteile:
  - Kein Controller nötig
- Nachteile:
  - Einschränkung der CPU-Leistung
