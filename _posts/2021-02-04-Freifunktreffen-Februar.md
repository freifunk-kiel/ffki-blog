---
layout: post                 
title: Protokoll des Freifunk Treffens im Februar 2021
---

   
### Warum ist der NTP Dienst unter 1.ntp.services.ffki nicht erreichbar? Aufgrund dessen funktioniert die Zeitsynchronisierung im Freifunk Netz derzeit nicht.

### Die Mesh-Karte hat wieder Grafana-Bilder.
Dies wurde gelöst indem die nötigen Abhängigkeiten für Debian buster installiert wurden:
https://grafana.com/docs/grafana/latest/administration/image_rendering/#grafana-image-renderer-plugin-and-remote-rendering-service

### In Garden wurde der Sport und Begegegnungspark mit Freifunk ausgestattet.
Laut Initiator kann das Wlan Netz bis zu den öffentlichen Grillplätzen empfangen werden.

### Karte auf neueste Hopglass Version geupdatet (Server und Map)

### Gateways haben seit dem Update auf Buster eine andere MAC Adresse, daher tauchen sie auf der karte als unbekannte neue Knoten.

### Knotenalarm Mails kamen bei Gmail und Posteo nicht an.

Gelöst indem Ruben den DNS Eintrag für http://freifunk-services-ipv6.in-kiel.de/ eingerichtet hat, welcher zusätzlich auf die Freifunk Kiel Webseite zeigt.
### Freifunk Vernetzungstreffen am 3.3.2021
