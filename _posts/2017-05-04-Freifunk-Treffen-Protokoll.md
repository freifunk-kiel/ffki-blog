---
layout: post
title: 04.05.2017 - Protokoll Freifunk Treffen
---
# Die Zukunft für Freifunk in Schleswig-Holstein
Es wurden Fragen geäußert, wie die Zukunft für Freifunk aussieht. Am 01.07.2017 wird die neu geregelte Vorratsdatenspeicherung (VDS) wirksam. Bisher ist die Rechtslage für Freifunk allerdings so unklar, dass die Folgen für Freifunk praktisch nicht absehbar sind.

In Kiel wird das Netz weiterbetrieben werden. Allerdings kann die Ausleitung nicht mehr weiter in Deutschland geschehen. Statt dessen werden die Gateways mittels VPN-Verbindungen ausleiten.

# Neuigkeit aus der Firmware Ecke

In Kiel wird demnächst eine neue Firmware auf Basis von 2016.2.5 per Autoupdate ausgeliefert. Zunächst handelt es sich nur um eine Aktualisierung für zusätzliche Hardware und Fehlerbehebungen.

Nach dem Update auf 2016.2.5 soll die Umstellung auf das neue Mesh-Protokoll 802.11s geschehen. Hierfür wird zunächst eine Firmware verteilt, die gleichzeitig das alte IBSS Protokoll sowie das neue 802.11s Protokoll unterstützt. Während dieser Umstellungsphase werden die Knoten ein wenig stärker beansprucht, so dass es zu Instabilitäten kommen kann.
Daher wird versucht die Umstellung möglichst zügig mit einer dritten Firmware, die nur noch 802.11s unterstützt abzuschließen.

Als weiter Änderung wurde in der Firmware ein Verweis auf das Picopeering Agreement (PPA) [1] hinterlegt. Außerdem wird den Betreibern angeboten sich automatisch am Knotenalarm anzumelden.

In der Zukunft, also nach der Umstellung auf 802.11s soll eine Umstellung auf die aktuelle Version des B.A.T.M.A.N Routingprotokolls geschehen.

In der Region Nord stehen ähnliche Änderungen an, allerdings soll hier der Umzug von 11s und B.A.T.M.A.N gleichzeitig geschehen. Hierfür wird das Update allerdings manuell administriert werden.

# Diverses

## Zusätzliche SSID "freifunk.net"?

Es wurde angeregt, dass zusätzlich zur bisherigen SSID "http://kiel.freifunk.net" auch die allgemeinere SSID "freifunk.net" ausgestrahlt werden sollte. Dies würde das Roaming zwischen verschiedenen Communities erleichtern. Allerdings würde die zur Verfügung stehende "Airtime" stark reduziert werden, da Pakete zusätzlich zwischen den SSIDs transferiert werden müssten.
Außerdem wären die lokalen Communities nicht mehr erkennbar, so dass neue Interessenten nicht mehr so leicht eingesammelt werden können.

## Neue Flyer

Es wurden neue Flyer designt. Die Anrede in den Texten wurde von "Du" auf "Sie" geändert, um auch in geschäftlicheren Kontakten angemessen zu sein. Außerdem wurde die Kontaktadresse auf *hallo@freifunk.in-kiel.de* geändert. Diese Adresse wird von Freiwilligen betreut um die erste Kontaktaufnahme etwas einfacher zu gestalten. In der Vergangenheit waren Leute überrascht direkt an eine Mailingliste zu schreiben.

## Kieler Woche

In den letzten Jahren war Freifunk an der jungen Bühne vertreten. Auch dieses Jahr sollten wir uns wieder präsentieren. Die genaueren Planungen sollen gegen Mitte/Ende Mai anfangen.

## Dachinstallationen

Die Immobilien der Stadt Kiel stehen weiterhin für Installationen zur Verfügung.
Eine Liste der Immobilien ist vorhanden [2], allerdings wird Unterstützung benötigt um Projekte umzusetzen.

Das Pilotprojekt am Mercatorhochhaus kommt langsam voran. Die nötigen Berechnungen sind weitestgehend erledigt und die genaue Abstimmung mit der GMSH kann beginnen.

[1] [http://http://picopeer.net/](http://http://picopeer.net/)  
[2] [https://docs.google.com/spreadsheets/d/1gfj_DM1fZln_HYJHPaGkWeyHxM9btrnPPTRz2WkDmWg/edit?usp=sharing](https://docs.google.com/spreadsheets/d/1gfj_DM1fZln_HYJHPaGkWeyHxM9btrnPPTRz2WkDmWg/edit?usp=sharing)
