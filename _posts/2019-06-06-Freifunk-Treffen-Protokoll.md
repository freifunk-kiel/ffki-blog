---
layout: post
title: Protokoll des Freifunk Treffens im Juni
---
### Statusberichte
#### Dachstandorte
Für den Standort auf dem Finanzamt ist unsere Anforderung und der Vertragsentwurf eingereicht, wir warten jetzt auf Antwort der GMSH.
Für das Mercatorhochhaus haben wir mal nach dem aktuellen Stand gefragt.
Der Standort in Ellerbek braucht mal wieder einen neuen Uplink, 
da die einzige Verbindung gerade mal wieder abgerissen ist.
Für die Standorte in Flensburg wird auch auf eine Reaktion der GMSH gewartet.

#### Firmware
Mehr dazu später, primär wird gerade mit neueren Gluon-Versionen getestet,
die dann wieder auf OpenWRT basieren.

#### Server
Es existieren zur Zeit sowohl Gateways mit BATMAN 14 als auch mit BATMAN 15.
Hierdurch können Knoten die noch nicht aktualisiert wurden weiter betrieben werden.
Die BATMAN 14 Gateways werden noch eine gewisse Zeit weiter laufen und dann 
in etwa einem Monat abgestellt werden. Ab dann wird es nur noch ein BATMAN 14
Gateway geben, welches nicht mit dem restlichen Netz verbunden ist und außer
einem potentiellen Firmware-Update kein Internet anbietet.

### Umstieg auf B.A.T.M.A.N. 15
Wir haben im letzten Monat weitgehend erfolgreich von BATMAN 14 auf BATMAN 15 
aktualisiert. Dabei sind nur ein paar Knoten nicht erfolgreich aktualisiert worden.
Die entsprechenden Setups wurden großteils repariert, 
lediglich eine größere Installation ist noch offline.
Die automatische Planung mittels dem Mesh independent Autoupdater (MIAU) hat
wohl größere Probleme vermieden.

Nach dem Update funktioniert das Netz gefühlt besser, allerdings ist der
Management-Traffic erstaunlicherweise deutlich gestiegen.
Im Rahmen des WCW wurde versucht die Ursachen für den Anstieg zu isolieren.

Einerseits werden in BATMAN 15 neue TVLVs eingeführt, 
andererseits wurden aus einem unbekannten Grund "Originator-Messages" zu häufig
versendet. Eigentlich sollten diese Nachrichten alle 5 Sekunden verschickt
werden, wurden aber doppelt so häufig gesendet. 
In der nächsten Gluon-Version sollte ein entsprechender Patch vorhanden sein.

Seit dem Update gibt es teilweise ein Problem mit fragmentierten Paketen.
Wir haben festgestellt, dass manche Pakete nicht wieder korrekt zusammengesetzt
werden. Die BATMAN-Entwickler sind informiert und wir schauen mal, ob mit dem
o. g. Patch die Fehler bereits behoben wurden.

### Bericht WCW
Dieses Jahr hat wieder das Wireless Community Weekend in Berlin statt gefunden.
Mehrere Teilnehmer aus Kiel waren anwesend und haben unter anderem das o. g.
BATMAN-Problem lokalisiert.
Aus Niedersachsen gab es einen interessanten Vortag zu Richtfunk-Installationen
auf dem Land. Mit breiter Unterstützung der Bevölkerung sind große
Installationen entstanden.

Ansonsten wurden wieder viele Kontakte zu anderen Communities gepflegt. 

### Diverses
#### ONN
Am 13. Juni findet um 18 Uhr die Mitgliederversammlung in der Toppoint statt.
Die Veranstaltung ist öffentlich, alle Interessierten sind eingeladen.

#### Kieler Woche
Für die Junge Bühne soll wieder eine Installation bereitgestellt werden. 
Tobias versucht sinnvolles Internet für den Schlossgarten zu organisieren.

#### Chaos Communication Camp 2019
Das Camp wird wieder statt finden, allerdings wird es dieses Mal
kein Freifunk-Village geben. 
Die Toppoint wird sich voraussichtlich um ein Village kümmern.

#### WiFi Tickling von Firefox
Auf Android hat Firefox ein interessante Verhalten. Parallel zu allen 
Anfragen werden 24 leere UDP Pakete an das Gateway verschickt.
Dies wird gemacht um Stromsparfunktionen des Telefons zu umgehen.
In unserem Netzwerk erzeugen diese Pakete eine gewisse Menge störende Grundlast.
Wir überlegen diese Pakete auf allen Routern zu filtern.

*Das nächste Freifunk Treffen findet planmäßig am 04.07.2019 statt.*
