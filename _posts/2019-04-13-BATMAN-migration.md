---
layout: post
title: Umstieg auf B.A.T.M.A.N. Advanced compat 15
---
### Umstieg auf B.A.T.M.A.N. Advanced compat 15

TL;DR; Wir werden in den nächsten Wochen mehrere Updates ausführen, wobei das vorletzte Update dieser Reihe ein sogenannter "Breaking Change" ist. Um diesen Umstieg dennoch sicher zu gestalten, haben wir zwei neue Technologien entwickelt, die uns helfen werden, die Risiken minimieren zu können.

Das von unserer Gemeinschaft eingesetzte Mesh-Module batman-adv ist bereits ein "wenig" in die Jahre gekommen und wird nur noch rudimentär gepflegt <a href="https://github.com/freifunk-gluon/batman-adv-legacy" target="_blank">[1]</a>. 
Es ist insbesondere immer noch nur Kompatiblitätsstufe 14; die letzte offizelle Version von batman-adv, welche diese Stufe unterstützt hat, stammt von 2013. 
Wir sind also bei den Features unserer Basis-Technologie, dem Mesh-Protokoll, ein "wenig" hinter der Zeit.

Da batman-adv 14 und 15 zueinander inkompatibel sind, kann ein Knoten mit Version 14 kein Mesh mehr mit einem Knoten mit Version 15 aufbauen 
und ein Parallelbetrieb, wie wir ihn z.B. beim Umstieg von ad-hoc auf 802.11s betreiben konnten, ist nicht möglich.

Daher haben wir in den letzten Jahren an einer Strategie gearbeitet, welche uns einen Umstieg trotzdem ermöglicht.
Dabei kommen zwei von uns entwickelte Technologien zum Einsatz: MIAU und FFUA.

Der Mesh Independent AutoUpdater (MIAU) <a href="https://github.com/TobleMiner/gluon-tsys" target="_blank">[2]</a> ist eine Erweiterung des Autoupdaters.
Während die Mesh-Protokolle zwar inkompatibel sind, also ein Weiterreichen der Daten über Knoten hinweg nicht mehr funktioniert, ist die Kommunikation zwischen zwei benachbarten Knoten weiterhin möglich.
Diesen Umstand nutzen wir, um die Möglichkeit zu schaffen, dass Knoten sich gegenseitig Updates weiterleiten können.
Somit ist ein Knoten, welcher keinen Kontakt mehr zum Update-Server hat, weil alle Knoten um ihn herum bereits aktuallisiert haben, weiterhin in der Lage, von seinen direkten Nachbarn, eine aktuelle Firmware zu erhalten. 
Das ist unsere Fallback-Absicherung.

Das Freifunk Firmware Update Allow (FFUA) <a href="https://github.com/sargon/ffua/" target="_blank">[3]</a> ist ein Stück Software, welches auf dem Update-Server läuft und Knoten das Update verweigern bzw. erlauben kann. Damit sind wir in der Lage, anhand einer Strategie Firmware kontrolliert an Knoten zu verteilen. Dazu haben wir zwei Strategien entwickelt:

- Die erste "MIAU Enforce" zwingt alle Knoten im Netz, ihr Update über den MIAU-Mechanismus zu beziehen.  Auf diese Weise testen wir seit einigen Wochen MIAU im Nightly-Branch.
- Die zweite Strategie "Outer-To-Inner Upgrade" verteilt ein Update so, dass die Knoten, welche – in Hinblick auf Länge des Netzwerkpfades – am weitesten von den Update Servern entfernt sind, als erstes ihr Update erhalten. Somit ist sichergestellt, dass alle Knoten die noch nicht das Update haben weiterhin mit einem mit ihrem Softwarestand kompatiblen Mesh verbunden bleiben und somit weiterhin die Möglichkeit behalten, das Update selber zu beziehen. Diese Methode ist in Testszenarien bereits erfolgreich erprobt.

Sollte ein Knoten in so einem Durchlauf kein Update erhalten, weil er z.B. ausgeschaltet war, hat er weiterhin über MIAU eine Möglichkeit ein Update zu beziehen.

Nun wollen wir unser in Jahren von Arbeit aufgebautes Netz ja nicht kaputt machen. Daher werden wir in den folgenden Wochen weitere Tests durchführen und nach Erfolg die Migration durchführen. Letzteres natürlich mit entsprechender Ankündigung!

*Schritt 1:* Anfang nächster Woche wird es ein neues Release der (Stable) Firmware geben, welche ausschließlich die Versionsnummer erhöht. 
Dieses werden wir mit der "Outer-To-Inner-Upgrade" Strategie ausrollen. Dies wird einige Tage in Anspruch nehmen, da die Knoten aktuell nur einmal in der Nacht auf die Server schauen. Wir werden uns dann genau anschauen, in welcher Reihenfolge die Knoten das Update bezogen haben. Diesen Schritt werden wir wiederholen bis er Zufriedenstellend lief.

*Schritt 2:* Nach Erfolg von Schritt 1 wird es ein weiteres Release der (Stable) Firmware geben, in welchem wir die Abstände, in welcher die Knoten nach neuen Updates schauen, auf wenige Minuten reduzieren werden. Dies wird wieder mit der "Outer-To-Inner-Upgrade" Strategie ausgerollt und wir werden uns noch einmal genau anschauen in welcher Reihenfolge die Knoten
ihre Updates bezogen haben.

*Schritt 3:* Wir stellen im nightly Branch per Firmware -Update auf den batman-adv compat 15 um, dieses wird mit der Strategie "MIAU Enforce" verteilt.
Dadurch werden alle Mesh-Inseln die durch Nightly-Knoten angebunden sind, auf die neue Version umgestellt und es werden höchstwahrscheinlich Knoten, die nicht auf nightly laufen, vom Netz abgehängt.  
Wir werden die betroffenen Knotenbetreiber über diesen Umstand informieren und versuchen sie zu einem Branchwechsel zu bewegen.

*Schritt 4:* Wenn auch Schritt 3 erfolgreich funktioniert hat, werden wir eine neue Stable-Firmware ausrollen, welche die kritische Operation durchführt. Diese wird dann mit der, mindestens zwei mal getesteten, "Outer-To-Inner-Upgrade" Strategie ausgerollt.

*Schritt 5:* Nachdem Schritt 4 durchgeführt wurde, wird es ein weiteres Release geben, welches die in Schritt 2 eingeführte, sehr regelmäßige Suche nach Updates wieder auf ein "normales" Interval reduziert.

Für das konkrete Update (Schritt 4) gibt es noch keinen Zeitplan. Es wird aber rechtzeitig per Mail und Blogpost Informationen zu diesem geben.

- [1] batman-adv legacy: <a href="https://github.com/freifunk-gluon/batman-adv-legacy" target="_blank">https://github.com/freifunk-gluon/batman-adv-legacy</a>
- [2] miau: <a href="https://github.com/TobleMiner/gluon-tsys" target="_blank">https://github.com/TobleMiner/gluon-tsys</a>
- [3] ffua: <a href="https://github.com/sargon/ffua/" target="_blank">https://github.com/sargon/ffua/</a>
