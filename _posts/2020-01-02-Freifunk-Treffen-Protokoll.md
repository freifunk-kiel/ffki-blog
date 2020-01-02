---
layout: post
title: Protokoll des Freifunk Treffens im Januar
---
### Statusberichte
#### Dachnetz
Es gibt nichts neues.

#### Firmware
Demnächst könnte es eine neue Version vom ddhcpd geben.

#### Gateways
Die Gateways laufen grundsätzlich ruhig vor sich hin.

### Diverses
#### Distributed DHCP
Es wurden ein paar Fehler im ddhcpd repariert, zum Beispiel das Handling von Adressen, die zur Zeit nicht sauber verwaltet wurden.
Somit sollten Clients wieder Antworten vom daemon bekommen, wenn alte Adressen verlängert werden sollen.
Weiterhin wurde die Verwaltung von knappen Speicherressourcen optimiert, so dass der daemon stabiler laufen sollte.

#### Unterstützte Geräte
Es werden demnächst von Gluon die Geräte mit 4MB Flash-Speicher nicht mehr unterstützt.
Wir werden voraussichtlich demnächst mal unsere Knotenbetreiber über das anstehende Supportende informieren.
Wir könnten die Router in einen nicht-betriebsbereiten Modus versetzen,
allerdings ist unklar, ob wir so einen Schritt über den Autoupdater ausrollen wollen.
Wir werden einen entsprechenden Hinweistext verfassen.


*Das nächste Freifunk Treffen findet planmäßig am 06.02.2020 statt.*
