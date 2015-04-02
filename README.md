# ffki-blog
blog der Webseite http://freifunk.in-kiel.de/blog.html

Um einen neuen Beitrag zu erstellen einfach folgende schritte:

 - Erstelle oben rechts ein Fork in deinem Github Account
 - Erstelle eine neue `.md` seite im ordner `_posts`, drücke dazu auf das Plus in der Überschrift `ffki-blog / _posts / +`. Die benennung der Datei muss dabei dem Datum beginnen, gefolgt von einem rein informativen Teil der ignoriert wird, z.B. `2015-03-30-beschreibender-ignorierter-teil.md`
 - Die Datei muss anfangen mit den Zeile:
```
---
layout: post
title: Hier der Titel deiner neuen Seite
---
```

 - Bilder können in den ordner `images` hochgeladen werden, diese werden auf der Webseite unter `/blog-img/` verlinkt
 - weitere Formatierungen findet man wenn man nach "markdown cheat sheet" sucht
 - Dann noch einen "Pull Request" erstellen mit deiner neuen Seite
