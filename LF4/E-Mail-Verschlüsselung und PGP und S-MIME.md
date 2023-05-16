# E-Mail Verschlüsselung und PGP und S-MIME

### Verfahren
- Gewährleistung der Vertraulichkeit von E-Mails
- Einsatz von E-Mail Verschlüsselung mit Schlüsselverwaltung und zusätzlich benötigter Client-Software
- Integrativ über Gateways und Plugins

### Transportverschlüsselung TLS
- Keine inhaltliche Verschlüsselung -> Transportverschlüsselung
- Sicherung von Computer bis Mail-Server
- Kann keine durchgängige Verschlüsselung gewährleisten

### Ende-zu-Ende-Verschlüsselung der E-Mail Inhalte
- S-MIME und OpenPGP als sichere Verschlüsselung
- Sonst Postweg

### OpenPGP-Verschlüsselung
- asymmetrisches Verschlüsselungsverfahren für ein- und ausgehende E-Mails
- Basis RFCs 4880 und 3156
- "Pretty Good Privacy" - weit verbreitetes Public-Key-Verfahren
- Jeder Kommunikationspartner = ein Schlüsselpaar (public-private)
- Öffentliche Keys an Kommunikationspartner weitergegeben, private Key verbleibt
- Private Key zur Entschlüsselung
- Unterstützung digitaler Signaturen
- Aufbau eines Web of Trusts (Vertrauensnetz) ohne zentrale Authentifizierungsstelle

### S-MIME-Verschlüsselung
- Sichere/Multizweckmäßige Internet E-Mail Erweiterung (Secure/Multipurpose Internet Mail Extension)
- asymmetrisches Verschlüsselungsverfahren, basierend auf öffentlichen und privaten Schlüssel
- Beglaubigung der Schlüsselpaare durch Zertifizierungsstelle
- Öffentlicher Key wird zur Zertifizierungsstelle gesendet
- Kosten für Unternehmen durch Zertifizierungsstelle, aber keine Extra-Software nötig

### Domain-Verschlüsselung
- Nutzertransparente asymmetrische Verschlüsselung von Maschine zu Maschine
- Austausch des öffentlichen Maschinen-Keys beider Kommunikationsparter
- Sicherung des gesamten E-Mail-Verkehrs zwischen Unternehmen

### Managed Domain Service
- Automatische Domainverschlüsselung über lokalisierten Keyserver
- Publikation öffentlicher Keys über den Server

### Open-Source-Tools zur Verschlüsselung
- VeraCrypt/TrueCrypt zum Verstecken und Verschlüsseln von Dateien
- Verschlüsselung einzelner Bereiche oder ganzer Festplatten

## Nur sichere Verschlüsselungsverfahren
Das BSI empfiehlt in der technischen Richtlinie TR-02102 eine Reihe kyptografischer Algorithmen und Protokolle, die aufgrund eingehender mathematischer Kryptoanalyse allgemein als sicher angesehen werden.
