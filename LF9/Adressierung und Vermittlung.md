# Adressierung und Vermittlung

## Vermittlung/Routing von Nachrichten (Layer 3)

### IPv4
- 32 Bit großer Adressraum
- 2^32 mögliche Adressen ~ 4,3 Milliarden Adressen
- Dezimale Darstellung
- Bspw.: 192.168.178.68
- IPsec optional
- Checksummen erforderlich
- NAT erforderlich (Network Address Translation) für zusätzliche Adressen
- Paketgröße: 576 Bytes
- Fragmentierung von Nachrichten möglich wenn Netzwerksegment < Paketgröße

### IPv6
- 128 Bit großer Adressraum
- 2^128 mögliche Adressen = 340 Sextillionen
- Hexadezimale Darstellung, 8 Blöcke á 16 Bit
- Bspw.: fe80::e022:d9bc:318b:1d7a
- IPsec optional
- Keine Checksummen
- IPv6 ohne NAT
- 1280 Bytes
- Keine Fragmentierung von Nachrichten nötig

## Adressierung im Internet Protokoll

### Anwendungsschicht
- OSI-Schichten: 7 Anwendung, 6 Darstellung, 5 Sitzung
- Bspw.: dhcp, dns, ftp, ftps, http, https, imap, ntp, pop3, rtp, sip, scp, sftp, smtp, snmp, socks, ssh, xmpp

### Transportschicht
- OSI-schicht: 4 Transport
- Bspw.: TCP, UDP, TLS, DTLS

### Internetschicht
- OSI-Schicht: 3 Vermittlung
- Bspw.: IP: IPv4/IPv6, IPsec, ICMP, BGP, RIP

### Netzzugang
- OSI-Schichten: 2 Sicherung, 1 Bitübertragung
- Bpsw.: ARP/NDP, PPP, PPPoE, MAC Adresse, Ethernet, Token Ring, Glasfaser, WLAN

