---
title: Feedback zur 4. Auflage von "Git - Dezentrale Versionsverwaltung im Team - Grundlagen und Workflows"
author: Bjørn Stachmann
layout: page
---

# Feedback

** Schickt uns eine Email oder meldet Euch bei Github an, um hier zu editieren! **

# Git

## Dezentrale Versionsverwaltung im Team <br/> Grundlagen und Workflows

## 4. Auflage


Verbesserungsvorschläge tragt ihr einfach unterhalb der passenden Kapitelüberschrift ein. Und dann ab per Pull-Request an uns :-) (Natürlich gerne auch per [Email](mailto:git@etosquare.de))

# Vorwort (Ab Seite i)

# Erste Schritte (Ab Seite 1)

## 1 Grundlegende Konzepte (Ab Seite 1)

## 2 Erste Schritte mit der Kommandozeile (Ab Seite 9)

## 3 Erste Schritte mit SourceTree (Ab Seite 23)

# Arbeiten mit Git (Ab Seite 31)

## 4 Was sind Commits? (Ab Seite 31)

## 5 Commits zusammenstellen (Ab Seite 39)

## 6 Das Repository (Ab Seite 49)

## 7 Branches verzweigen (Ab Seite 59)

Seite 59

>  „In beiden Fällen entstehen Verzweigungen im Graphen der Commit-Historie."
> Die Aufzählung enthält mehr als 2 Punkte, daher sollte es
> „In allen Fällen..." heißen. (Benjamin Harms)

Es gibt drei Arten von Informatikern:
Solche die zählen können und solche, die es nicht können ;-)
Danke für den Hinweis.

✓ Auflage 6

Seite 64, dritter Absatz

> „Achtung! reset -hard überschreibt Workspace und Stage-Bereich.“
> Hier ist wohl „reset --hard" gemeint  (Benjamin Harms)

Stimmt.

✓ Auflage 6


## 8 Branches zusammenführen (Ab Seite 67)

## 9 Mit Rebasing die Historie glätten (Ab Seite 81)

## 10 Repositorys erstellen, klonen und verwalten (Ab Seite 89)

> Seite 92 Oben: rsync wird als Protokoll seit Git 2.8.0 nicht mehr unterstützt. (Böckler)

Das wäre uns sicher nie aufgefallen. Vielen Dank für den Hinweis.

✓ Auflage 4, Nachdruck

## 11 Austausch zwischen Repositorys (Ab Seite 95)

> Seite 104 Unten: ...sogenannte Refs und ~~Refspecss~~ Refspecs 

✓ Auflage 5

## 12 Versionen markieren (Ab Seite 105)

> Seite 106 Oben: GnuPG (~~Gnu~~ GNU Privacy Guard)

✓ Auflage 5

## 13 Tipps und Tricks (Ab Seite 109)

> Seite 109 nach Überschrift 13.1: Git ~~ist~~ is like a dog.

✓ Auflage 5

> Seite 113 Mitte: Sie weisen zwar auf Backticks (\`, U+0060) hin, aber in den Befehlen werden gerade keine verwendet, sondern die Fußzeichen (\',U+0027). Das ist vermeidbar, indem Sie einfach die Form $(…) verwenden,
die seit der Korn-Shell das gleiche erledigt. (Böckler)

Ja, das ist eine gute Idee. Die $(...)-Notation ist viel besser zu lesen.

✓ Auflage 4, Nachdruck

> Seite 114 Schritt für Schritt Punk 1:  git rebase --interactive benötigt einen Commit. Gemäss Beispiel wäre das wohl die gemeinsame Wurzel von A und B. Sonst lässt sich das Kommando nicht aufrufen.

Backlog Auflage 5

*Anmerkung*: `rebase` ohne Parameter aufgerufen, nimmt den Upstream-Branch,
z. B. `origin/master` für `master`. Das heißt, es werden idR. jene Commits rebased,
die man noch nicht gepushed hat. Das ist eigentlich recht praktisch.

> Seite 114 und 115, Kapitel 13.6 - Für einen Einsteiger ist dieses Beispiel eine echte Herausforderung. Gerade hier kann man aber viel lernen, wenn dieses Beispiel detailliert erklärt wird. Heisst: Nach jedem Step (mit Erläuterung der Optionen/Argumente) wird der Graph dargestellt, mit allen Positionen der Branch-Refs und des Heads. Das würde ein gutes Verständnis über das Zusammenspiel der einzelnen Schritte liefern.

Backlog Auflage 6

# Workflows (Ab Seite 117)

## 14 Workflow-Enführung (Ab Seite 117)

# Workflows: Entwickeln mit Git

## 15 Ein Projekt aufsetzen (Ab Seite 123)

> Seite 132, erster Satz: Die ersten ~~Teammitgleader~~ **Teammitglieder** können nun [...] @shadyhh

*Teammitgleader* klingt irgendwie nach *agile leadership*.
War aber doch nur einen Tippfehler. Ich korrigiere das.

✓ Auflage 4, Nachdruck


## 16 Gemeinsam auf einem Branch entwickeln (Ab Seite 135)

## 17 Mit Feature-Branches entwickeln (Ab Seite 143)

> Seite 148, erster Absatz: [...] und besser mit einem ~~Feature-Toogle~~ **Feature-Toggle** die Funktionalität zu deaktivieren.  @shadyhh

Es ist denkbar, dass Feature-Toggles bei Google erfunden wurden.
Trotzdem heißen sie **Toggles**.

✓ Auflage 4, Nachdruck

> Seite 149, nach Abb. 17-4: Wenn ~~Nachbearbeiten~~ **Nachbearbeitungen** notwendig sind, [...]  @shadyhh

Im Text steht **Nacharbeiten**. Kann man so lassen.


> Seite 151, vor Überschrift: -d:  Löscht den übergebenen ~~Branc~~ **Branch**.  @shadyhh

Sieht komisch aus. Habe das bereinigt und dabei gleich die lesbarere Form `--delete` eingesetzt.

✓ Auflage 4, Nachdruck


## 18 Mit Forks entwickeln (Ab Seite 163)

> Seite 167, unten: ~~textttupstream~~ **upstream**: Normalerweise bezieht sich der [...] @shadyhh

> Seite 167 Unten: Da fehlt im LaTeX-Quelltext wohl ein Backslash, daher
steht hier textttupstream statt upstream. (Böckler)

Jo.

✓ Auflage 4, Nachdruck


> Seite 172 Oben: Hier steht 4.1.0, 4.1.1, 4.1.1 statt vermutlich 4.1.0,
4.1.1, 4.1.2 (Böckler)

Jo.

✓ Auflage 4, Nachdruck

> Seite 172, nach Überschrift: [...], indem man das Beitragen zum Projekt so leicht und ~~angenehmen~~ **angenehm** wie möglich macht.  @shadyhh

> Seite 172 Unten: „so leicht und angenehmen wie möglich“ statt vermutlich „so
leicht und angenehm wie möglich“ (Böckler)

Jo.

✓ Auflage 4, Nachdruck


# Workflows: Releaseprozess (Ab Seite 175)

## 19 Kontinuierlich Releases durchführen (Ab Seite 175)

## 20 Periodisch Releases durchführen (Ab Seite 185)

> Seite 191 Schritt 1: release-Branch anlegen
> Der Befehl muss richtigerweise: "git checkout -b release develop" lauten @hampa

Korrekt. Wohl ein Copy-Paste-Bug unsererseits.

✓ Auflage 5

## 21 Mit mehreren aktiven Releases arbeiten (Ab Seite 199)

> Seite 208, Fussnote: Wenn es aber zu ~~Nachbearbeiten~~ **Nachbearbeitungen** beim Cherry-Pick gekommen ist, kann es Probleme geben. @shadyhh

Im Text steht **Nacharbeiten**. Kann man so lassen.


# Workflows: Repositorys pflegen (Ab Seite 213)

## 22 Ein Projekt mit großen binären Dateien versionieren (Ab Seite 213)

## 23 Große Projekte aufteilen (Ab Seite 221)

Seite 225, erster Absatz vs. Seite 240 letzter Absatz

> In beiden Fällen werden die Parameter zum filter-branch-Befehl erläutert.
> Im ersten Fall wird "-all" erklärt, während an zweiter Stelle "-- --all" erläutert ist.
>  (Benjamin Harms)

Es soll `--all` heißen.

✓ Auflage 6

## 24 Kleine Projekte zusammenführen (Ab Seite 229)

## 25 Lange Historien auslagern (Ab Seite 235)

## 26 http://kapitel26.github.io

## 27 Ein Projekt nach Git migrieren (Ab Seite 247)

# Mehr über Git (Ab Seite 263)

## 28 Integration mit Jenkins (Ab Seite 263)

Seite 269, Aufzählung:

> „einen Trigger innerhalb der zentralen Repository-Verwaltung, um das Build nach dem Anlegen oder Ändern eines Pull-Requests zu starten,“
> Hier müsste es „...um den Build nach dem Anlegen…“ heißen.
> „einen Job im Build-Server, um das Pull-Request-Build zu bauen, ggf. gibt es dafür auch spezielle Plug-Ins,“
> Hier müsste es „...um den Pull-Request-Build zu bauen,…“ heißen.
>
> (Benjamin Harms)

✓ Auflage 6


## 29 Abhängigkeiten zwischen Repositorys (Ab Seite 275)

> Kapitel 29.2 Abhängigkeiten mit Subtrees
> Seite 285, Schritt-für-Schritt: Änderungen in das Modul-Repository übertragen
> Unter "1. Änderungen im Modulverzeichnis separieren" fehlt beim Parameter "--prefix sub" das =-Zeichen, also "--prefix=sub". (@UdoHeyn)

Jo.

✓ Auflage 4, Nachdruck


> Außerdem eine Anregung genau zu diesem Abschnitt: Die schrittweisen Erklärungen sind für das Verständnis sicher hilfreich. Könnte man zusätzlich den Befehl "subtree push" anführen, der die Einzelschritte in sich vereint (sofern ich es richtig verstanden habe) und damit das Extrahieren von Änderungen wesentlich vereinfacht? (@UdoHeyn)

Das fehlt. Einen Abschnitt zu `subtree push` werden wir ergänzen.

✓ Auflage 4, Nachdruck

Seite 286, Zusammenfassung:

> „Alternativ kann man beim Klonen die --recursive benutzen.“
> Ggf. „die“ weglassen oder „Option“ ergänzen.
> „Alternativ kann man beim Klonen die Option --recursive benutzen.“
>
>  (Benjamin Harms)

Jo.


## 30 Was gibt es sonst noch? (Ab Seite 289)

## 31 Die Grenzen von Git (Ab Seite 297)

# Anhang (Ab Seite 305)

# Dankeschön

### Jason Stäuble [@shadyhh](https://github.com/shadyhh)

> Hallo,
> das Feedback habe ich auf [Amazon](https://www.amazon.de/review/R1OAOQUVLGUKKT/ref=cm_cr_dp_title?ie=UTF8&ASIN=3864904528&channel=detail-glance&nodeID=299956&store=books) hinterlassen. Kurz gesagt: das Buch ist super!
> Die Schreibfehlerkorrekturen habe ich unten eingefügt. Ausserdem wollte ich euch noch darauf hinweisen, dass es auf euerem Blog einige Fehler gibt und nicht die 4. Auflage erwähnt wird.
> Freundliche Grüsse
> Jason Stäuble (@shadyhh)

Vielen Dank für die Korrekturen und das super Feedback auf Amazon! Die Fehler werde ich gleich im  Manuskript korrigieren. Auch wenn es wohl noch ein Weilchen dauert, bis wir die fünfte Auflage herausbringen können.

### Udo Heyn  [@UdoHeyn](https://github.com/UdoHeyn)

Vielen Dank an @UdoHeyn.

### Herr Böckler

Vielen Dank auch an Herrn Böckler.

### Hampa Brügger [@hampa-git](https://github.com/hampa-git)

Vielen Dank für den Hinweis!

### Gerhard Schroll [@gschroll](https://github.com/gschroll)

Vielen Dank für die Hinweise!

### [@TheDet](https://github.com/TheDet)

Vielen Dank für den Hinweis!

### Benjamin Harms

Vielen Dank für die Hinweise!

