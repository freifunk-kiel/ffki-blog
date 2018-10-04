---
layout: post
title: Protokoll des Freifunk Treffens im Oktober
---
### Gemeinnützigkeit von Freifunk-Initiativen
Es gibt einen erneuten Vorstoß für eine 
Anerkennung der Gemeinnützigkeit von Freifunk-Initiativen.
Dazu wurden die diversen Freifunk-Gruppen in Schleswig-Holstein
um eine Stellungsnahme gebeten.

Die meisten Gruppen haben sich dazu verständigt eine 
gemeinsame Antwort zu verfassen. Grundsätzlich sind die 
Gruppen interessiert an einer Gemeinnützigkeit.
Voraussichtlich wird in der Antwort ein gemeinsamer
Sachverständiger vorgeschlagen.

Wenn die Initiative erfolgreich sein sollte, 
wäre die nächste Stufe die Eingabe in den Bundesrat.

### Status der Firmware
Für die nächste Firmware wurde reichlich Arbeit in den 
ddhcpd gesteckt. Es wurden diverse Fehler ausgebügelt
und der Dienst scheint inzwischen auf einem Stand angekommen zu sein
in dem er live getestet werden kann. 
In den bisherigen Tests wurde ein erhöhter Management-Traffic beobachtet.
Wenn der ddhcpd auf allen Geräten aktiviert wird, 
kann eventuell zwischen 20% und 50% mehr Management-Traffic erwartet werden.
Dieser betrifft aber nicht den Bereich, der die Routingtabellen der Router 
bei Geräten mit kleinem Speicher überlasten würde. Außerdem wird der Management-Traffic
durch  weitere Optimierungen in der neuen Firmware wiederum verringert.

Ein neues Firmware-Release wird in der nächsten Zeit angepeilt.
Als Basis wird Gluon 2018.1, welches auf LEDE basiert, verwendet werden.
Neben einigen kleineren Änderungen wird das nächste Release
den neuen Autoupdater mitbringen. Mit diesem wird auch ein Update möglich,
wenn kein echtes Mesh mehr besteht. Somit könnten dann auch ein Wechsel 
der B.A.T.M.A.N-Version durchgezogen werden.

### Diverses
#### IoT-Meeting
Es hat sich eine LoraWAN / IoT Gruppe Kiel gegründet. 
Vielleicht können sich hier interessante Kooperationen finden.

#### Dachinstallation
Das RBZ Wirtschaft wurde angefragt, die Schule hat zurückgefragt wo ihr Vorteil wäre. 
Eine Rücksprache mit der Stadt wird zur Zeit geführt.

Das Finanzamt wird demnächst besucht. Das dortige Dach ist neu, steht also nicht unter Denkmalschutz,
ist höher als das Bildungsministerium und besser ausgebaut.

#### Kooperation mit GNUnet/Zeronet
Es wurde die Frage gestellt, ob man mit Zeronet oder GNUnet ein dezentrales, zensurresistentes Netzwerk 
im lokalen Freifunk Netz bereitstellen könnte. Darin könnten Benutzer statische oder dynamische Websites
veröffentlichen, die im Freifunk selbst dann lokal verfügbar wären, wenn die Verbindung ins Internet abbricht.


*Das nächste Freifunk Treffen findet planmäßig am 01.11.2018 statt.*
