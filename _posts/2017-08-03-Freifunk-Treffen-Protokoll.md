---
layout: post
title: 03.08.2017 - Protokoll Freifunk Treffen
---
# Neues aus der Firmware-Ecke

Seit einigen Versionen gibt es einen Fehler in manchen Routern, der manchmal dazu geführt hat, dass der Router kein funktionierendes WLAN mehr ausstrahlt. Dieser sollte eigentlich durch den sogenannten *Quickfix* erkannt werden und automatisch zum Neustart des Routers führen.
Leider gab es bisher einen Fehler im Quickfix, der nur innerhalb der ersten Stunde nach Einschalten diese Überprüfung durchgeführt hat.

Es könnte dieser Quickfix repariert werden und eine neue Firmware ausgerollt werden. Allerdings würde dies weiterhin den echten Fehler nicht beheben. Statt dessen könnte auch der Quickfix behoben werden und statt dessen der Fehler gesucht werden. Für den neuen Quickfix soll nicht extra eine neue Firmware gebaut werden. Im nächsten planmäßigen Update wird der neue Quickfix eingebaut.

Aktuell wird im *nightly* außerdem ein neues Paket getestet, das die Funktion des WLAN-Knopfes an den Routern ändert. Statt wie bisher nur das WLAN an- oder abzuschalten kann der Knopf verschiedene Funktionen im Config-Modus zugewiesen bekommen.   

# Diverses

## Gateway Situation

Der bisherige Gateway vpn3 wurde abgeschaltet, wird in Zukunft aber ersetzt werden. Unsere Gateway-Situation ist ein kleines bisschen angespannt. vpn1 und vpn4 haben etwas bröckelige VPN Verbindungen, vpn5 und vpn6 haben Paketverluste zwischen 25% bis 33%.

## IPv6

Es wurden erste Anstrengungen gestartet mit Freifunk Rheinland zusammen IPv6 Routing zu bekommen.

*Das nächste Freifunk Treffen findet planmäßig am 07.09.2017 statt.*
