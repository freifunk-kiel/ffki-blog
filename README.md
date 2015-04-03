# ffki-blog
blog der Webseite http://freifunk.in-kiel.de/blog.html

Um einen neuen Beitrag zu erstellen einfach folgende schritte:

 - Erstelle eine neue `.md` seite im ordner `_posts`, drücke dazu auf das Plus in der Überschrift:  
    `    / ffki-blog / _posts / + `  
    (beim ersten mal wird dabei automatisch eine Kopie dieses Projekts in deinem Github erzeugt, in dem du ab dann arbeitest). 
 - Wähle dabei unten "Create a new branch for this commit and start a pull request." um dir nicht die Möglichkeit zu verbauen mehrere unabhängige Änderungen vorzuschlagen.
 - Die Benennung der Datei muss dabei mit dem Datum beginnen, gefolgt von einem rein informativen Teil der ignoriert wird, z.B. `2015-03-30-beschreibender-ignorierter-teil.md`
 - Der Inhalt der Datei muss anfangen mit den Zeilen:
```
---
layout: post
title: Hier der Titel deiner neuen Seite
---
```

 - Bilder können in den ordner `images` hochgeladen werden, diese werden auf der Webseite unter `/images/blog/` verlinkt
 - weitere Formatierungen findet man wenn man nach *"markdown cheat sheet"* sucht
 - in dem Reiter "Preview changes" kannst du schalten um zu überprüfen, wie dein Post aussehen würde.
 - Wenn du fertig bist, erstelle einen "Pull Request" mit dem Grünen Symbol, dadurch wird ein "Issue" erstellt, in dem ein anderer Mitarbeiter des ffki-blog projekts deine Änderungen noch einmal anschauen kann und freigeben.
