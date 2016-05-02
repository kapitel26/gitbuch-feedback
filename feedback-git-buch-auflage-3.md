---
title: Feedback zur 3. Auflage von "Git - Dezentrale Versionsverwaltung im Team - Grundlagen und Workflows"
author: Bjørn Stachmann
layout: page
---

# Git

## Dezentrale Versionsverwaltung im Team <br/> Grundlagen und Workflows

## 3. Auflage

Verbesserungsvorschläge tragt ihr einfach unterhalb der passenden Kapitelüberschrift ein. Und dann ab per Pull-Request an uns :-) (Natürlich gerne auch per [Email](mailto:git@etosquare.de))

# Vorwort (Ab Seite i)

# Erste Schritte (Ab Seite 1)

## 1 Grundlegende Konzepte (Ab Seite 1)

## 2 Erste Schritte mit der Kommandozeile (Ab Seite 9)

## 3 Erste Schritte mit SourceTree (Ab Seite 21)

# Arbeiten mit Git (Ab Seite 29)

## 4 Was sind Commits? (Ab Seite 29)

## 5 Commits zusammenstellen (Ab Seite 37)

## 6 Das Repository (Ab Seite 47)

## 7 Branches verzweigen (Ab Seite 57)

## 8 Branches zusammenführen (Ab Seite 65)

### 8.2 Konflikte

Seite 70 (Hinweis von Thomas B.):

Dort steht:

> `git show :3:picture.png   >theirs.txt`

`theirs.txt` ist falsch. Korrekt ist `theirs.png`:

> `git show :3:picture.png   >theirs.png`

## 9 Mit Rebasing dieHistorieglätten (Ab Seite 79)

## 10 Repositorys erstellen, klonen und verwalten (Ab Sete 87)

## 11 Austausch zwischen Repositorys (Ab Seite 93)

## 12 Versionen markieren (Ab Seite 103)

### 12.5 In welcher Version ist es "drin"?

Seite 105. Leserhinweis (Thomas B.)

Hier nutzen wir den `grep`-Befehl, um die Ausgabe des `oneline`-Ausgabe Log-Befehls zu durchsuchen:

> `git log --oneline 1.2.3.3 | grep "Gesuchter Kommentar."`

Es ist (fast immer) besser, die Historie mit der Option `--grep` des `log`-Befehls zu filtern, weil dabei alle Zeilen des Kommantar durchsucht werden (nicht nur die Titelzeile) und die Option vor der Formatierung der Log-Ausgabe wirkt.

## 13 Abhängigkeiten zwischen Repositorys (Ab Seite 107)

## 14 Tipps und Tricks (Ab Seite 121)

### 14.5 Branches als temporäre Zeiger auf Commits nutzen

Seite 124 und 125 (Hinweis von Thomas B.):

Die Anführungszeichen sehen im Druck aus wie einfache Anführungszeichen, gemeint sind aber sogenannte Backticks.

> `git branch tmp/merge-base \`git merge-base master feature\` `

Anmerkung: In der Bash-Shell kann man Backticks für geschachtelte Befehle nutzen. Die Ausgabe des inneren Befehls (hier `git merge-base`) wird als Argument des Äußeren (hier `git branch`) verwendet.

# Workflows (Ab Seite 129)

## 15 Workflow-Enführung (Ab Seite 129)

# Workflows: Entwickeln mit Git

## 16 Ein Projekt aufsetzen (Ab Seite 135)

## 17 Gemeinsam auf einem Branch entwickeln (Ab Seite 153)

## 18 Mit Feature-Branches entwickeln (Ab Seite 161)

Seite 167 (Hinweis von Thomas B.)

Im Fußnote 4 ist die Rede von der Option `-no-commit`, korrekt ist aber `--no-commit`.

## 19 Mit Bisection Fehler suchen (Ab Seite 181)

# Workflows: Releaseprozess (Ab Seite 193)

## 20 Kontinuierlich Releases durchführen (Ab Seite 193)

## 21 Periodisch Releases durchführen (Ab Seite 203)

## 22 Mit mehreren aktiven Releases arbeiten (Ab Seite 217)

# Workflows: Repositorys pflegen (Ab Seite 231)

## 23 Große Projekte aufteilen (Ab Seite 231)

## 24 Kleine Projekte zusammenführen (Ab Seite 239)

## 25 Lange Historien auslagern (Ab Seite 245)

# Workflows: Umstieg auf Git (Ab Seite 255)

## 26 Das sechsundzwanzigste Kapitel (Ab Seite 255)

 * (bstachmann) Im sechsundzwanzigsten Kapitel solle ein Verweis auf diese Feedbackseite stehen.

## 27 Andere Versionsverwaltungen parallel nutzen (Ab Seite 257)

## 28 Ein Projekt nach Git migrieren (Ab Seite 269)

# Mehr über Git (Ab Seite 285)

## 29 Integration mit Jenkins (Ab Seite 285)

## 30 Was gibt es sonst noch? (Ab Seite 295)

## 31 Die Grenzen von Git (Ab Seite 303)

### 31.3 Ressourcenverbrauch bei großen binären Dateien

Leserhinweis (Thomas B.)

> ... dass der delta Algorithmus für Binärdateien nicht greift ist nicht richtig. In pack Dateien greift er bis zu einer Dateigröße von 512MiB (core.bigFileThreshold).

Der Abschnitt über große Dateien ist etwas oberflächlich und ungenau geraten. In den Anfangszeiten von Git war dies auch nicht so wichtig, denn Git wurde in der Regel nicht für Binärdateien genutzt. In der Zwischenzeit  wird dies öfter gemacht und es haben sich Patterns, Practices und Extensions zum Umgang mit großen Binärdateien etabliert. Wir planen, dem Thema einen etwas größeren Abschnitt zu widmen, wenn es zu einer Neuauflage kommt.

Link zum Thema: https://blogs.atlassian.com/2014/05/handle-big-repositories-git/

# Anhang (Ab Seite 313)
