---
layout: post
title: Protokoll des Freifunk Treffens im Januar
---
# Freifunk auf dem 34. Chaos Communication Congress
Auf dem 34. Chaos Communication Congress (34C3) gab es eine große Freifunk-Assembly.
Hier konnten sich die diversen lokalen Gruppen treffen und vernetzen.
Freifunk Kiel und Nord hatten einen sehr schön gelegenen Tisch in der Assembly,
an dem viele interessante Gespräche, besonders auch mit Neulingen und Interessierten geführt werden konnten.
Zusätzlich gab es eine kleine Freifunk-Bühne, auf der kleine Vorträge gehalten wurden.

Leider hat die Freifunk *Bundesländervertretung* es nicht geschafft sich auf dem 34C3 zu treffen.
Insgesamt scheint diese Gruppe wohl leider mehr oder weniger tot zu sein.

Mit dem Umzug nach Leipzig ist der Congress wieder deutlich gewachsen.
Gleichzeitig ist natürlich vieles neu und muss erstmal wieder geordnet werden.
In den kommenden Jahren könnte Freifunk Kiel und Nord auf dem Congress gerne von mehr Leuten unterstützt werden.

# Freifunk - Der Allmende Tragödie dritter Akt
In den letzten Tagen gab es eine sehr aktive Diskussion auf der Mailingliste.
Aus einer eigentlich technischen Frage entwickelte sich eine Diskussion über die generelle Nutzung des Freifunk Netzes.
Das Freifunk-Netz stellt eine allgemeine, öffentliche Infrastruktur, ähnlich der [Allmende][1] dar.
Wir werden keinerlei Unterscheidung von Traffic im Netz machen,
allerdings muss immer auf die gemeinsamen Ressourcen Rücksicht genommen werden.
Somit kann es natürlich passieren, dass z.B. Medienstreams in belasteten Mesh-Wolken
nicht immer ruckelfrei laufen müssen.

Allerdings gibt es auch mehr oder dringende Probleme in unserer Community:

* Viele Dienste, wie Wiki, Router oder Firmware, werden nur von einer kleinen
Gruppe Menschen betreut oder bearbeitet.
* Die Treffen werden meistens von den selben Leuten besucht und es besteht kaum Außenwirkung.
* Manche Mesh-Netze sind nur sehr dünn mit Uplinks versorgt. Teilweise hängen Router über 6 Hops an einem Uplink.
* Wir haben keine *Push-Kommunikation* mit unseren Nutzern, die ML ist der *direkteste* Kanal 

# Diverses
## Eigenes AS für Norddeutsschland
Es gibt den Wunsch für Norddeutsschland ein *anständiges* Netz zusammenzubauen.
Dafür wäre ein eigenes *Autonomes System* (AS) nötig.
Um ein AS beantragen zu können werden (neben einer soliden rechtlichen Struktur)
zwei andere AS benötigt, die mit dem neuen Netz peeren würden.


## ddhcpd - Verteilte Adressverteilung
[DHCP][2] ist ein Mechanismus um IPv4 Adressen in Netzwerken zu verteilen.
Normalerweise ist ein Server als zentrale Vergabestelle zuständig.
Falls mehrere Server verwendet werden sollen, müssen diese statisch miteinander koordiniert werden. Meistens werden die Server in ein Failover-Setup konfiguriert, so dass der aktive Server ausfallen kann und automatisch von einem anderen Server ersetzt wird.

Für unser Netz wäre es interessant die Adressvergabe komplett auf die Knoten zu verteilen. Das ist die Funktion des ddhcpd-Servers. Hier handeln die Knoten untereinander Adressblöcke aus, die dann an die Endgeräte verteilt werden können.

Durch die Änderung können Clients signifikant schneller mit dem Netz verbinden.

Auf lange Sicht ist das Ziel die Gateways komplett mit Gluon zu betreiben. Der ddhcpd ist ein weiterer Schritt dabei, die Funktionen der Gateways auf die Knoten zu verlagern.

## Freifunk Kiel PR
Wir müssen bekannter sein. Wir sollten also mehr Leute ansprechen und Möglichkeiten wahrnehmen Freifunk in der Öffentlichkeit zu präsentieren.

Zusätzlich gibt es die Idee einen Promo-Film für Freifunk zu drehen. 
Für die Toppoint wurde ein derartiger Film vor einiger Zeit produziert, der sehr gut angekommen ist.

## Dächer der Stadt
Die Immobilien der Stadt Kiel stehen weiterhin für Installationen zur Verfügung.
Eine Liste der Immobilien ist [vorhanden][3], allerdings wird Unterstützung benötigt um Projekte umzusetzen.

 [1]: https://de.wikipedia.org/wiki/Allmende
 [2]: https://de.wikipedia.org/wiki/Dynamic_Host_Configuration_Protocol
 [3]: https://docs.google.com/spreadsheets/d/1gfj_DM1fZln_HYJHPaGkWeyHxM9btrnPPTRz2WkDmWg/edit?usp=sharing

*Das nächste Freifunk Treffen findet planmäßig am 01.02.2018 statt.*
