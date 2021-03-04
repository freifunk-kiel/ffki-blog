---
layout: post                 
title: Protokoll des Freifunk Treffens im März 2021
---

   
### Vernetzungstreffen
ab gestern alle 3 Monate den ersten Mittwoch im Monat

### Freifunk an einem DSLite Anschluß betreiben
Um einen Freifunk Knoten an einem DSLite Anschluß laufen zu lassen muss man die IPv4-Konnektivität im Config Mode (erweiterte Einstellungen/Netzwerk) deaktivieren und eine Firmware mit mindestens 2020.x laufen lassen.
Wenn man als Test die IP 192.0.0.2 erfolgreich anpingen kann, dann hängt man an einem DSLite Anschluß.

### Firmware
Die nächste Firmware wird ein Paket namens "ffka-gluon-web-usb-wan-hotplug" enthalten mit dem man einen Freifunk Knoten einfach über sein Handy laufen lassen kann, wenn man dort USB-Tethering aktiviert.
Leider ist der toppoint gitlab Server auf dem wir die Firmware Bauen immer noch defekt, deshalb kann dort im Moment keine Firmware gebaut werden.

### DNS Server für Freifunk Kiel wurde repariert
Der DNS Server für Freifunk Kiel wurde repariert Daher ist nun auch NTP wieder nutzbar. D.h. die Knoten bekommen die korrekte Uhrzeit.
Für Nord steht die NTP Reperatur noch aus Dort muss das auf den Gateways behoben werden.

