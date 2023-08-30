# Systemverfügbarkeit und Stromversorgung

## Berechnungen von Systemverfügbarkeit

- **Uptime**:
  - t^up = Funktionale Zeit
  - t^up = A * t^gesamt
- **Downtime**:
  - t^down = Ausfallzeit
  - t^down = t^gesamt - t^up = t^gesamt - A * t^gesamt
  - t^down = t^gesamt * (1-A)
- **Gesamtzeit**:
  - t^gesamt = Gesamtzeit (Jahr = 8.760h/525.600Min)
  - t^gesamt = t^up + t^down
- **Availability**:
  - A = t^up : t^gesamt = 1 - t^down : t^gesamt
  - A = 1 -> Dauerhaft verfügbar
  - A = 0 -> Nie verfügbar
  - 99% Verfügbarkeit = 87,6h Ausfallzeit
 
## Komponenten der Stromversorgung

### Arbeitsplatz
- Elektrogeräte
- Standard-Elektroinstallation zur Stromversorgung
- Absicherung = 16 Ampere pro Stromkreis

### Serverraum
- Stromversorgung durch mehrere separate Stromkreise
- Dreiphasige Lastenverteilung
- Anschluss auch über USV bei hoher Betriebsrelevanz der Geräte

### USV (Unterbrechungsfreie Stromversorgung)
- **Aufgaben**:
  - Filterung von Störungen auf Netzspannung
    - Spannungsspitzen
    - Über-/Unterspannung
    - Stabilität der Netzfrequenz
  - Überbrückung kurzzeitiger Netzausfälle
  - Geregeltes Herunterfahren von Servern
- **Typen**:
  - VFI - Voltage and Frequency Independent from Main Supply
    - online, Double-Conversion, Dauerbetrieb, Doppelwandler
  - VI - Voltage Independent from Main Supply
    - netzinteraktiv, Single-Conversion, Delta-Conversion, aktiver Mitlaufbetrieb
  - VFD - Voltage and Frequency Dependent from Main Supply
    - offline, standby, passiv
   
### Netzersatzanlage, Ersatzstromversorgung
- Stromgeneratoren zur Gewährleistung einer Stromversorgung im Ausfallfall

### Netztypen der Stromversorgung
- TN-System (Terre Neutre)
  - Neutralleiter von Generatorseite
  - Schutzleiter PE (Protective Earth) von Anlagenseite
- TT-System (Terre Terre)
  - Neutralleiter von Generatorseite
- IT-System (Isolé Terre)
  - Ohne Neutralleiter von Generatorseite
  - Erdung PE in Hausverteilung
 
### Power over Ethernet/Dataline
- Stromversorgung für Netzwerkgeräte über Ethernet-Leitung
- Endspan-Devices/Switches = Netzwerkswitches mit PoE-Fähigkeit
- Midspan-Geräte/Power Injectors = Speisegeräte zur Einschleifung ins Netzwerk nach einem Switch

## Berechnung
- **Spannung U**
  - U = R * I
  - Einheit: Volt, V
- **Strom I**
  - I = U : R
  - Einheit: Ampère, A
- **Widerstand R**:
  - R = U : I
  - Einheit: Ohm, Ω
- **Ohm'sches Gesetz**:
  - U = R * I
  - Einheit: Volt, V
- **Wirkleistung P**:
  - P = U * I
  - Einheit: Watt, W
- **Arbeit W**:
  - W = P * t
  - Einheit: Wattstunde, Wh, Kilowattstunde, kWh
- **Scheinleistung S (U und I nicht in Phase)**:
  - S = U * I
  - Einheit: Voltampère, VA
- **Wirkungsgrad η**:
  - η = P^aus : P^ein / abgegebene Leistung : zugeführte Leistung
- **Wirkfaktor cos φ**:
  - cos φ = P : S
