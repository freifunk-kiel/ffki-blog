---
layout: post
title: Protokoll des Freifunk Treffens im November
---
### Statusberichte
Es sollen in Zukunft feststehende Themenblöcke kurz am Anfang erwähnt werden.
#### Firmware
Es wurde eine neue Firmware veröffentlicht (siehe extra Punkt)

#### Dachstandorte
Der Antrag für das Finanzamt wurde angefangen zu schreiben. Für das Mercatorhochhaus ist der Gestattungsvertrag angekommen und durchgeschaut worden. Der Vertrag geht in den nächsten Tagen zurück an die GMSH. 

#### Serverbetrieb
Zur Zeit haben wir 3 Gateways, die, bis auf wenige Stotterer, sauber laufen.
Ein Gateway wird in der nächsten Zeit aufgegeben werden.
Die Gateways laufen inzwischen mit einem neuen sauberen Ansible-Skript.
Die Service-Maschine ist zur Zeit noch ein Schlachtfeld. 
Die vielen alten Skripte müssen mal aktualisiert werden.

### Neuigkeiten aus der Freifunk Firmware 2018.1.1-461
Vor einer Woche wurde die neue Firmware veröffentlicht. 
Mit der neuen Firmware ist das fast schon antike Gluon mal aktualisiert worden.
Einige Filter dämmen die Broadcasts im Netz ein bisschen ein und haben das Rauschen im Netz reduziert.
Der neue ddhcpd verteilt jetzt IP-Adressen an Clients direkt auf dem Knoten ohne die Gateways zu belasten.
Aktuell gibt es noch einen Fehler, der dafür sorgt dass der roamguide gar nicht läuft.
Es gibt bisher keinen festen Zyklus für Releases, aber vielleicht könnte hier mal ein festerer Prozess etabliert werden.

Durch das Update sind maximal eine einstellige Anzahl Knoten verloren worden, die beim Update nicht sauber neugestartet sind. Ein paar Knoten haben undefiniert hohe Last. Für den Fehler gibt es eine Bug-Bounty im Freifunk-Forum ausgeschrieben.

In der neuen Nightly-Firmware ist der Mesh-Independent-Autoupdater veröffentlicht.

### Gemeinnützigkeit von Freifunk-Initiativen Zusammenfassung
Vor einiger Zeit wurden praktisch alle Freifunk-Gruppen in Schleswig-Holstein vom Wirtschaftsausschuss des Landtages angeschrieben.
Das Thema wurde schon vor 4 Jahren begonnen und einmal im Bundesrat und Bundestag behandelt, ist damals aber dem Ende der Legislatur zum Opfer gefallen.

Im letzten Meeting wurde zwar besprochen, dass jemand(TM) sich um die Antwort kümmern werden. Allerdings wurde der jemand(TM) nicht mit einer konkreten Person gefüllt. Das hat dazu geführt, dass bis kurz vor Fristablauf keine anständige Antwort vorbereitet wurde. Es wurde dann kurzfristig ein Antwortschreiben formuliert und eine Stellungnahme an den Wirtschaftsausschuss gesendet.

### Prof. Dr. Menusch Khadjavi stellt sein Forschungsprojekt vor
Prof. Khadjavi und Prof. Schmidt wollen Freifunk im Rahmen ein Forschungsprojektes untersuchen. Freifunk ist eine interessante Plattform für die Forschung, da sich hier freiwillige Menschen verbinden um das Gemeinwohl zu unterstützen.
Es soll in der nächsten Zeit ein Antrag für ein Forschungsprojekt geschrieben werden, 
in dem Freifunk in der gesamten Stadt untersucht werden soll. 
Hierbei soll es um verschiedene Formen der Anreize zur Mitarbeit in sozialen Projekten gehen.

Die Bürger in der Stadt sollen in verschiedenen Formen angesprochen werden (z.B. nur Information bis hin zu geschenkten Routern) und die entsprechenden Ergebnisse untersucht werden. Um das Projekt zu unterstützen, sollte im ersten Schritt von den Kieler Freifunkern ein Unterstützungsschreiben formuliert werden, dass wir das Projekt begrüßen.

Wenn der Antrag bewilligt werden sollte, sollten auch Kapazitäten für die Unterstützung der neuen Teilnehmer am Netz bereit gestellt werden. 

Es besteht der Konsens, dass ein entsprechendes Unterstützungsschreiben aufgesetzt werden soll.

### Diverses
#### Linux Presentation Day in Schwentinental
Am 10. November findet der Linux Presentation Day in Schwentinental im Rahmen der Ehrenamtsmesse statt. Hierbei bietet sich auch die gute Möglichkeit wieder Freifunk zu präsentieren. 

#### Mailingliste
Es gab einen etwas unangenehmen Vorfall auf der Freifunk-Mailingliste. Es wurde auf eine hilfesuchende Mail eine relativ aggressive Antwort geschrieben. Es ist fraglich, wie mit derartigen Geschehnissen umgegangen werden sollte. 
Es könnte die Mailingliste moderiert werden oder die betreffende Person von der Liste entfernt werden. Alternativ könnte auch auf der Liste eine Meta-Diskussion über die Umgangsformen begonnen werden.

#### Matrix-IRC Brücke
Die bisherige Brücke zwischen dem Hackint IRC-Netz und der Matrix wird zum Jahresende abgeschaltet. Unser bisheriger Freifunk-Channel ist an das Hackint-Netz angebunden und wird die Verbindung dann verlieren.  


*Das nächste Freifunk Treffen findet planmäßig am 06.12.2018 statt.*
