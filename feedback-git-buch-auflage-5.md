---
title: Feedback zur 5. Auflage von "Git - Dezentrale Versionsverwaltung im Team - Grundlagen und Workflows"
author: Bjørn Stachmann
layout: page
---

# Feedback

** Schickt uns eine Email oder meldet Euch bei Github an, um hier zu editieren! **

# Git

## Dezentrale Versionsverwaltung im Team <br/> Grundlagen und Workflows

## 5. Auflage


Verbesserungsvorschläge tragt ihr einfach unterhalb der passenden Kapitelüberschrift ein. Und dann ab per Pull-Request an uns :-) (Natürlich gerne auch per [Email](mailto:git@etosquare.de))

# Vorwort (Ab Seite i)

# Erste Schritte (Ab Seite 1)

## 1 Grundlegende Konzepte (Ab Seite 1)

## 2 Erste Schritte mit der Kommandozeile (Ab Seite )

## 3 Erste Schritte mit SourceTree (Ab Seite )

# Arbeiten mit Git (Ab Seite )

## 4 Was sind Commits? (Ab Seite )

## 5 Commits zusammenstellen (Ab Seite )

## 6 Das Repository (Ab Seite )

## 7 Branches verzweigen (Ab Seite )

## 8 Branches zusammenführen (Ab Seite )

## 9 Mit Rebasing die Historie glätten (Ab Seite )

## 10 Repositorys erstellen, klonen und verwalten (Ab Seite )

## 11 Austausch zwischen Repositorys (Ab Seite )

## 12 Versionen markieren (Ab Seite )

## 13 Tipps und Tricks (Ab Seite )

# Workflows (Ab Seite )

## 14 Workflow-Enführung (Ab Seite )

# Workflows: Entwickeln mit Git

## 15 Ein Projekt aufsetzen (Ab Seite )

## 16 Gemeinsam auf einem Branch entwickeln (Ab Seite )

## 17 Mit Feature-Branches entwickeln (Ab Seite )

## 18 Mit Forks entwickeln (Ab Seite )

# Workflows: Releaseprozess (Ab Seite )

## 19 Kontinuierlich Releases durchführen (Ab Seite )

## 20 Periodisch Releases durchführen (Ab Seite )

## 21 Mit mehreren aktiven Releases arbeiten (Ab Seite )

# Workflows: Repositorys pflegen (Ab Seite )

## 22 Ein Projekt mit großen binären Dateien versionieren (Ab Seite )

## 23 Große Projekte aufteilen (Ab Seite )

## 24 Kleine Projekte zusammenführen (Ab Seite 239)

> Hatte am Wochenende mal zwei lokale Git Repos zusammengeführt, 
> so wie im Buch ab Seite 239 beschrieben. 
> Der merge des remote Repos ist fehlgeschlagen mit ".. history nicht gleich 
> oä" ... das lief dann nur durch mit der Option: --allow-unrelated-history. 
> Ist die History dann auch vollständig vorhanden? 

Korrekt. Wenn man zwei separate Historien per Merge zusammenführen möchte,
muss man dies mit ` --allow-unrelated-history` bestätigen.

✓ Auflage 6

Die Historien werden bei dieser Operation vollständig erhalten.

Tipp: Man kann ein vergleichbares Ergebnis mit dem neueren Befehl `subtree add` erreichen, z. B.

```bash
    $ git subtree add --prefix=backend ../backend.git master
```

## 25 Lange Historien auslagern (Ab Seite )

## 26 http://kapitel26.github.io

## 27 Ein Projekt nach Git migrieren (Ab Seite )

# Mehr über Git (Ab Seite )

## 28 Integration mit Jenkins (Ab Seite )

## 29 Große Repositorys (Ab Seite )

## 30 Abhängigkeiten zwischen Repositorys (Ab Seite )

## 31 Was gibt es sonst noch? (Ab Seite )

## 32 Die Grenzen von Git (Ab Seite )

# Anhang (Ab Seite )

# Dankeschön

# Dankeschön

## Thomas Wenzlaff

Vielen Dank für den Hinweis zu `--allow-unrelated-histories`.
