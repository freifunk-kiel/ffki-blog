---
layout: post
title: Protokoll des Freifunk Treffens im September
---
# Gateways für Freifunk Kiel
In den letzten Wochen sind ein paar Gateways umgezogen. Inzwischen sind 4 Gateways bei OVH in Frankfurt gehostet und leiten direkt aus.
Die Systeme wurden direkt mittels [Puppet-Installation][1] aufgesetzt. Ein paar kleine Anpassungen mussten manuell erfolgen, zum Beispiel um die direkte Ausleitung zu aktivieren.
Durch die neuere Debian Version (Jessie) gab es ein paar Probleme mit falschen B.A.T.M.A.N.-Versionen.
Die neuen Gateways werden vom Freifunk Nord e.V. finanziert.

Die B.A.T.M.A.N.-Version könnte in Zukunft mal aktualisiert werden,
aber eigentlich ist der Plan eher, in Zukunft Gateways mit Gluon zu betreiben. Dafür ist noch ein bisschen Arbeit notwendig, aber die Zukunft ist nicht mehr weit entfernt.

# Diverses
## Dächer der Stadt
Die Immobilien der Stadt Kiel stehen weiterhin für Installationen zur Verfügung.
Eine Liste der Immobilien ist vorhanden [2], allerdings wird Unterstützung benötigt um Projekte umzusetzen.

## Dächer des Landes
Wir haben eine Bewilligung der Landesregierung für vier Dachstandorte (Mercatorhochhaus, Finanzamt, Bildungsministerium, Alte Mu) erhalten. Hier ist auch eine gewisse Kostenbewilligung enthalten.

Für das Mercatorhochhaus ist der [Antrag][3] fast fertig, Korrekturlesen ist erwünscht.

## Fonds "Gemeinsam Kiel gestalten"
"Bereits zum dritten Mal vergibt die Landeshauptstadt Kiel Fördermittel für Projekte von Bürgerinnen und Bürgern zur Verbesserung der Situation in ihren Stadtteilen. Der von der Kieler Ratsversammlung ins Leben gerufene Fonds „Gemeinsam Kiel gestalten“ stellt für das Jahr 2018 insgesamt 300.000 Euro bereit."
TLDR: Vereine können [Anträge][4] stellen um entsprechende Projekte umzusetzen.

## Hardwareecke
In der aktuellen Nightly-Firmware ist das "Alt-Esc"-Paket zum direkten Ausleiten vorhanden. Zusätzlich ist jetzt ein Paket zur Statistik-Trennung zwischen 2.4GHz und 5GHz Funkverkehr eingebaut. Der neue, [alternative Meshviewer][5] kann Clients für 2.4 und 5 GHz getrennt visualisieren.

Im Moment ist die Hardwareversorgung etwas schwierig. Der bewährte TP-Link WR841 ist mit seinen 4MB nicht mehr leistungsfähig genug. Der Archer C25 ist inzwischen relativ teuer und funktioniert noch immer nicht korrekt mit 5GHz. Die Archer C59 und C60 könnten vielleicht bald funktionieren.

Von Ubiquiti gibt es ein paar neue Modelle mit schöner 5GHz Unterstützung, aber die LEDE-Unterstützung ist vermutlich noch nicht vollständig.

 [1]: https://github.com/freifunk-kiel/ffki-puppet-gateway-install
 [2]: https://docs.google.com/spreadsheets/d/1gfj_DM1fZln_HYJHPaGkWeyHxM9btrnPPTRz2WkDmWg/edit?usp=sharing
 [3]: https://git.freifunk.in-kiel.de/ffki-material/tree/standorte/mercator
 [4]: https://www.kiel.de/de/politik_verwaltung/meldung.php?id=73351
 [5]: https://map.freifunk.in-kiel.de

*Das nächste Freifunk Treffen findet planmäßig am 04.01.2018 statt.*
