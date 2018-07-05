---
layout: post
title: Protokoll des Freifunk Treffens im Juli
---
### Stand Mercator-Hochhaus
Unser Sachbearbeiter in der Verwaltung scheint bis in den Winter beurlaubt zu sein.
Daher liegt unser Antrag noch unbearbeitet irgendwo rum.
Wir versuchen zumindest mal die Formalia soweit zu kriegen,
dass ein Sachbearbeiter sich mal dafür zuständig erklärt.

In Flensburg sind zwar die Dachstandorte genehmigt, 
die Bauarbeiten für den Mast sind aber zur Zeit in einem unbekannten Zustand.

### IPv6 Rollout
Der Gateway VPN0 routet jetzt IPv6 und verteilt IPv6 Adressen an Endgeräte.
Das Netz ist uns von Freifunk Nordwest zur Verfügung gestellt worden.
Das Netz sollte dadurch ein bisschen besser geworden sein.

Wenn wir auf mehr Gateways IPv6 ausrollen, 
werden alle Gateways einen eigenen /64 Präfix announcen.
Dazu müssen die Router dann aber die doppelten Router-Advertisements filtern um Inter-Gateway-Traffic zu minimieren. 
Das wird von einem neuen Paket in Gluon verwaltet.

### Firmware neue Features
Eine neue Firmware fährt so langsam auf die Zielgerade.
Dafür wurden diverse Build-Prozesse mal wieder angefasst und besser öffentlich dokumentiert.
Die aktuelle Entwicklungs-Firmware wird auf dem Gitlab<sup>[1]</sup> der Toppoint gebaut.

Neue Features in der Firmware sind:
- IPv6 Management (siehe oben)
- ddhcpd (Lokaler DHCP Server)
Auf jedem Router läuft ein neuer Daemon, der als DHCP Server für IPv4 Adressen fungiert.
Der IPv4-Adressbereich wird in viele kleine Blöcke geteilt. Wenn ein Router einem Endgerät eine Adresse zuteilen will, greift er sich einen kleinen Block aus dem Pool und verteilt daraus eine Adresse an das Endgerät. Die Router einigen sich untereinander darauf, welche Blöcke benutzt oder frei sind.
- Basiert auf 2017.1.8 oder auf 2018.1
- Der Bug, der hohe Last auf Knoten erzeugt hat, scheint nicht mehr so einfach aufzutreten.

### Diverses
#### Kieler Woche Nachlese
Es gab wieder Freifunk am Playground der Jungen Bühne auf der Kieler Woche. Wir hatten etwa 38GB auf einem einzigen Zugangspunkt.
Es gab am Anfang ein paar Probleme mit dem NordVPN Uplink. Zusätzlich gab es manchmal Probleme mit der LTE-Verbindung. Inzwischen haben alle Besucher auch ein LTE-Telefon in der Tasche und überlasten die Funkzelle.

*Das nächste Freifunk Treffen findet planmäßig am 02.08.2018 statt.*

 [1]: https://gitlab.toppoint.de
