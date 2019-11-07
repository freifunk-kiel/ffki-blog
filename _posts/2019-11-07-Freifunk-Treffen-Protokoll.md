---
layout: post
title: Protokoll des Freifunk Treffens im November
---
### Statusberichte
#### Dachnetz
Es gab bisher keine Antwort seitens der GMSH.
Wir müssen uns wohl nochmal bei unserem Ansprechpartner melden.

#### Firmware
Es ist geplant zum Wochenende eine neue stabile Firmware mit aktualisiertem dDHCPd zu releasen.
Die nightly-Firmware macht zur Zeit ein paar Probleme, da an dem verwendeten Multicast in Gluon 2019.2 noch irgendwas nicht sauber funktioniert.

#### Gateways
Laufen stabil vor sich hin.

### DDHCPD
Daniel hat die Integration des dDHCPd nochmal ein bisschen verbessert und den Management-Overhead ein bisschen reduziert.
Weiterhin gab es eine Verbesserung in der Behandlung der verteilten Blöcke. So, dass freie Blöcke nicht so agressiv durch die Gegend gereicht werden, sondern zunächst noch kurz in dem bisherigen Knoten behalten werden.

Es gibt noch ein paar Ideen um die Lernphase am Anfang des Lebenszyklus zu verkürzen, diese sind aber noch nicht implementiert.

### roamguide
Es gibt Verwirrungen über die Funktion des roamguide. 


### nightly Knoten nicht auf Karte sichtbar
Durch die Änderungen in Gluon 2018.2 (Multicast) sind die Knoten gerade nicht anständig auf der Karte angezeigt. Die Reperatur steht noch aus und muss irgendwie(TM) realisiert werden.


*Das nächste Freifunk Treffen findet planmäßig am 05.12.2019 statt.*
 
