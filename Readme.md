---
title: Übungsblatt 6
author: Zuletzt bearbeitet von Jürgen Hahn
documentclass: scrartcl
classoption:
  - a4paper
header-includes: |
    \usepackage{german} 
    \usepackage[a4paper,left=2.5cm, right=2.5cm,top=2.5cm, bottom=3cm]{geometry}
    \usepackage{fancyhdr}
    \usepackage{graphicx}
    \pagestyle{fancy}
    \fancyhf{}
    \rhead{OOP WS 2020/21}
    \lhead{U06 | Übungsblatt 6}
    \cfoot{\includegraphics[height=2cm]{docs/footer.png}}
    \fancypagestyle{plain}{
      \fancyhf{}
      \rhead{OOP WS 2020/21}
      \lhead{U06 | Übungsblatt 6}
      \cfoot[C]{\includegraphics[height=2cm]{docs/footer.png}}}
---


# Übungsblatt 6

## Wichtige Informationen zur Bearbeitung der Aufgabe 

 - [Informationen zur Entwicklungsumgebung *IntelliJ IDEA*](https://elearning.uni-regensburg.de/mod/book/view.php?id=1480675)
 - [Informationen zum Im- und Export von Projekten](https://elearning.uni-regensburg.de/mod/book/view.php?id=1480675&chapterid=51551)
 - [GraphicsApp](https://elearning.uni-regensburg.de/mod/url/view.php?id=1482162)

## Starterpaket

Ein vorbereitetes Starterpaket zur selbständigen Implementierung der Aufgaben finden Sie hier:
 - [Starterpaket](https://github.com/OOP-Ubungen-WS2020-21/U06-GraphicsApp/archive/Starterpaket.zip)

### Clickable CircleRain

![Clickable CircleRain](docs/redcirclerain.png){ width=25% }

Wer erinnert sich nicht? Die hübschen, fallenden Kreise aus Übung 6 sind wieder zurück. Diesmal setzen Sie Ihr neu erlangtes Wissen über Maus-Interaktion ein, um Nutzern zu erlauben, alle Kreise rot zu färben. Im Starterpaket ist ein Lösungsvorschlag für die CircleRain-Aufgabe enthalten. Ihre Aufgabe ist es, die `onMousePressed`-Methode zu implementieren und darin zu prüfen, ob ein Kreis getroffen wurde und ihn einzufärben, falls dies der Fall ist. Die Anwendung soll, wenn alle Kreise rot gefärbt wurden, wieder alle Kreise zurücksetzen und dabei neu einfärben bzw. ihnen neue Geschwindigkeiten zuweisen.

### **MiniGame mit Mausklick**

Erstellen Sie ein kleines Reaktionsspiel. Ziel des Spiels ist es, einen
Ball, der sich innerhalb der Grenzen des Fensters linear bewegt, mit der
Maus zu treffen. Berührt der Ball eine der Seiten, prallt er von der
Wand ab. Schafft es die spielende Person, den Ball mit der Maus zu treffen, erhöht sich die Geschwindigkeit des Balls, er wechselt die Richtung und man bekommt einen Punkt. Beim Richtungswechsel werden x- und y-Richtung getauscht. Wird alles zuviel, sollen Spielende mit einem Druck auf Escape den Ball zum Stillstand bringen können. Dabei setzt sich auch der Punktestand wieder auf 0 zurück.

In der `GraphicsApp`-Anwendung `MiniGame` müssen Sie den Spielgegenstand, einen `ClickBall`, instanziieren und Mausklicks mit der `onMousePressed`-Methode auf ihn behandeln sowie Punkte zählen. Auch die Behandlung des `KeyPressedEvents` und die Abfage, ob Escape gedrückt wurde, gilt es hier zu erledigen. Geben Sie den aktuellen Punktestand auf der Konsole aus, wenn er sich verändert.

In der Klasse `ClickBall` sind einige Methoden bereits vorgegeben, die Ihnen aus der RandomBouncingBalls-Übung bekannt sein dürften. Zusätzlich implementieren sollen Sie den Richtungswechsel, das Stoppen und die Abfrage, ob der Ball vom Klick getroffen wurde.

![Mini Game](docs/minigame.png){ width=25% }

