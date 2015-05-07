# ffki-blog
Blog der Webseite http://freifunk.in-kiel.de/blog.html

Um einen neuen Beitrag zu erstellen brauchst du keine weitere Software. Das Blog kannst du **direkt im Browser hier auf Github bearbeiten**. 

Klicke dazu einfach oben auf den Ordner `_posts` und führe dann folgende Schritte aus:

 - Logge dich in deinem Github Account ein (oder benutze Username: `ffki-blogger`, Passwort: `blogger77`)
 - Erstelle eine neue `.md` seite im ordner `_posts`, drücke dazu auf das Plus in der Überschrift:  
    `    / ffki-blog / _posts / + `  
    ![new post](http://i.stack.imgur.com/MEP2q.png)  
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
 - weitere Formatierungen findet man wenn man nach *"markdown cheat sheet"* googelt, z.B. https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet
 - in dem Reiter "Preview changes" kannst du schalten um zu überprüfen, wie dein Post aussehen würde.
 - Wenn du fertig bist, erstelle einen "Pull Request" mit dem grünen Symbol, dadurch wird ein "Pul Request Issue" erstellt, in dem ein anderer Mitarbeiter des ffki-blog Projekts deine Änderungen noch einmal anschauen kann und dann freigeben.
