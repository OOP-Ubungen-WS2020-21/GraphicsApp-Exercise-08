---
title: Template
author: Zuletzt bearbeitet von Daniel Kwoska
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
    \lhead{U00 | Template}
    \cfoot{\includegraphics[height=2cm]{docs/footer.png}}
    \fancypagestyle{plain}{
      \fancyhf{}
      \rhead{OOP WS 2020/21}
      \lhead{U00 | Template}
      \cfoot[C]{\includegraphics[height=2cm]{docs/footer.png}}}
---


# Übungsblatt 8

## Wichtige Informationen zur Bearbeitung der Aufgabe 

 - [Informationen zur Entwicklungsumgebung *IntelliJ IDEA*](https://regensburger-forscher.de/oop/tutorials/Entwicklungsumgebung)
 - [Informationen zum Im- und Export von Projekten](https://regensburger-forscher.de/oop/tutorials/Starterprojekte)
 - [GraphicsApp](https://elearning.uni-regensburg.de/mod/url/view.php?id=1482162)

## Starterpaket

Ein vorbereitetes Starterpaket zur selbständigen Implementierung der Aufgaben finden Sie hier:
 - [Starterpaket](https://github.com/OOP-Regensburg/GraphicsApp-Exercise-08/archive/Starterpaket.zip)

### Clickable CircleRain

![image](img/redcirclerain.png)

Wer erinnert sich nicht? Die hübschen, fallenden Kreise aus Übung 6 sind wieder zurück. Diesmal setzen Sie Ihr neu erlangtes Wissen über Maus-Interaktion ein, um Nutzern zu erlauben, alle Kreise rot zu färben. Im Starterpaket ist ein Lösungsvorschlag für die CircleRain-Aufgabe enthalten. Ihre Aufgabe ist es, die `onMousePressed`-Methode zu implementieren und darin zu prüfen, ob ein Kreis getroffen wurde und ihn einzufärben, falls dies der Fall ist. Die Anwendung soll, wenn alle Kreise rot gefärbt wurden, wieder alle Kreise zurücksetzen und dabei neu einfärben bzw. ihnen neue Geschwindigkeiten zuweisen.

### **MiniGame mit Mausklick**

Erstellen Sie ein kleines Reaktionsspiel. Ziel des Spiels ist es, einen
Ball, der sich innerhalb der Grenzen des Fensters linear bewegt, mit der
Maus zu treffen. Berührt der Ball eine der Seiten, prallt er von der
Wand ab. Schafft es die spielende Person, den Ball mit der Maus zu treffen, erhöht sich die Geschwindigkeit des Balls, er wechselt die Richtung und man bekommt einen Punkt. Beim Richtungswechsel werden x- und y-Richtung getauscht. Wird alles zuviel, sollen Spielende mit einem Druck auf Escape den Ball zum Stillstand bringen können. Dabei setzt sich auch der Punktestand wieder auf 0 zurück.

In der `GraphicsApp`-Anwendung `MiniGame` müssen Sie den Spielgegenstand, einen `ClickBall`, instanziieren und Mausklicks mit der `onMousePressed`-Methode auf ihn behandeln sowie Punkte zählen. Auch die Behandlung des `KeyPressedEvents` und die Abfage, ob Escape gedrückt wurde, gilt es hier zu erledigen. Geben Sie den aktuellen Punktestand auf der Konsole aus, wenn er sich verändert.

In der Klasse `ClickBall` sind einige Methoden bereits vorgegeben, die Ihnen aus der RandomBouncingBalls-Übung bekannt sein dürften. Zusätzlich implementieren sollen Sie den Richtungswechsel, das Stoppen und die Abfrage, ob der Ball vom Klick getroffen wurde.

![image](img/minigame.png)

