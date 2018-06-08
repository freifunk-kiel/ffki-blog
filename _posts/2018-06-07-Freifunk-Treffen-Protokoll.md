---
layout: post
title: Protokoll des Freifunk Treffens im Juni
---
### "Mesh is in the Air" Bericht aus Berlin
Vom 7. bis 13. Mai wurde das *Wireless Battle Mesh* und das *Wireless Community Weekend* in Berlin ausgerichtet[2]. Die Veranstaltungen wurden von Besuchern aus der ganzen Welt besucht und auch einige Freifunker aus Kiel waren angereist.

Daniel hat einen Vortrag zum ddhcpd gehalten, der auch online verfügbar[3] ist. Außerdem wurde unter anderem über aktuelle Entwicklungen zum Routing diskutiert. Das neue Routing über Babel befindet sich langsam auf der Zielgeraden.

### Ausblick Firmware Neuerungen
Zur Zeit sind unsere Router noch mit einer Firmware basierend auf Gluon 2016.x ausgestattet.
Die aktuelleren Gluon-Versionen 2017.x und 2018.x haben leider einen mysteriösen Bug[1], der
besonders WR841 Router mit hoher Systemlast abstürzen lässt.

Wenn wir eine neue Firmware ausrollen können, wären dabei ein paar neue Features unterstützt:
  - neuer Updater (siehe unten)
  - neue Router unterstützt
  - ddhcpd
  - roamguide

### Server Status
Wir hatten bis vor kurzen 6 Gateways für das Kieler Freifunk Netz. Von diesen Servern waren 4 Maschinen bei OVH, 2 bei Hetzner gehostet.
Die Gateways bei OVH hatten in der Vergangenheit immer mal wieder deutliche Probleme.
Es wird vermutet, dass OVH aktiv VPN-Verkehr drosselt oder komplett verwirft.

Aus diesen Gründen wurden die 4 OVH Maschinen vor kurzem gekündigt. 
Als Resultat sind unsere verbleibenden Gateways zur Zeit etwas stark belastet. 
Es wurden aber bereits neue Gateway-Spenden angekündigt, so dass die Situation in absehbarer Zeit gelöst werden sollte.

### Mesh unabhängiger Auto Update
t-sys hat einen neuen Autoupdater für unsere Firmware entwickelt.
Der Updater ist in der Lage auch größere Änderungen am Netz zu überleben,
zum Beispiel ein Update der Routing-Protokolle (B.A.T.M.A.N. oder Babel).

Wenn das bisherige Updateverfahren fehlschlägt, verbindet sich der neue Updater direkt mit seinen
Nachbarn und nutzt diese als Proxy. Hierüber kann er dann den Updateserver erreichen.

### Diverses
#### IPv6 in Freifunk Kiel
Wir haben von Freifunk Nordwest ein IPv6 Präfix delegiert bekommen. Die Integration in das Freifunk Netz sind in vollem Gange.

#### Neues aus der Hardwareecke
Ruben hat ein paar neue Router zum Selbstkostenpreis mitgebracht. Die neuen WR1043v5 kosten 29 Euro und sind unser aktuelles Einstiegsgerät. Die neue Version hat kein USB-Anschluss mehr.

Die Router werden zur Zeit nur von der Nightly-Firmware unterstützt. Der Autoupdater ist aber automatisch auf Stable konfiguriert, so dass nicht immer die Nightly-Versionen nachgeladen werden.

#### Linux Presentation Day
Am 10. November findet der nächste *Linux Presentation Day* in Raisdorf statt.
Die Veranstaltung findet in Verbindung mit der Ehrenamtsmesse in der Uttoxeter-Halle statt.
Für den Tag wäre es schön Freifunk in der Halle anbieten zu können. 
Wir könnten über einen LTE-Uplink eine Abdeckung realisieren.

*Das nächste Freifunk Treffen findet planmäßig am 05.07.2018 statt.*

 [1]: https://github.com/freifunk-gluon/gluon/issues/1243
 [2]: https://www.wireless-meshup.org
 [3]: https://media.freifunk.net/v/distributed-dhcp-daemon
