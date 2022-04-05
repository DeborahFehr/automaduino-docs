---
title: "Blink Beispiel"
linkTitle: "Blink Beispiel"
date: 2022-04-01
description: >
  In diesem Beispiel wird erklärt wie du den Code für das Blinkbeispiel generierst!
---

Das Blink Programm ist das _Hallo Welt_ Programm für den Arduino. Wir verwenden eine einzelne LED und schalten sie an und wieder aus mit einer kleinen Verzögerung. Als Ergebnis wird die LED blinken, daher auch der name. Wenn dieses Programm läuft haben wir bewiesen, dass der Arduino korrekt angeschlossen ist und funktioniert.

### Steckplan

Besorg dir eine LED und einen Widerstand (z.B. 100 Ohm). Verbinde die LED mit Pin 7 und verwende ein Steckbrett um den GND Pin mit dem Widerstand zu verbinden. 

Unten siehst du einen Steckplan mit einer Beispielverbindung. 

![](/docs/tutorials/blink-sketch.png)

_Steckplan für das Blink Beispiel_

### Sketch

Jetzt überlegen wir uns wie unser Automat aussehen soll. Wir benutzen Papier und Stift und skizzieren was passiert. Hier siehst du eine Skizze. 

![](/docs/tutorials/blink-drawing.png)

_Blink Skizze Beispiel_

#### Zustände hinzufügen

Jetzt setzen wir unsere Skizze in Automaduino um. Dazu fügen wir zwei Zustände hinzu: Eine eingeschaltete und eine ausgeschaltete LED. 

![](/docs/tutorials/blink-states.png)

_Blink Zustände_

#### Übergänge hinzufügen

Jetzt verbinden wir diese Zustände. Wir verbinden der Startpunkt mit dem AN Zustand. Danach warten wir kurz, dargestellt durch einen _nach_ Übergang, und gehen zum AUS Zustand über. Nach einer weiteren kurzen Wartezeit wechseln wir wieder zum AN Zustand. 

![](/docs/tutorials/blink-transitions.png)

_Blink Übergänge_

### Pins zuweisen

Um unseren Code lauffähig zu machen müssen wir noch die Pins zuweisen. Dazu öffnen wir den Dialog und fügen eine LED Komponente an Pin 7 hinzu. Wir weisen beide Zustände dieser Komponente zu und klicken auf Absenden. 

![](/docs/tutorials/blink-led-assignment.png)

_Pin Zuweisung Beispiel_

### Hochladen

Jetzt kopieren wir den Code in die Arduino IDE und laden ihn hoch wie beschrieben unter [Erste Schritte](/docs/getting-started/). Wenn du die LED richtig angeschlossen hast sollte sie jetzt blinken. Du hast erfolgreich deinen Arduino programmiert!

### Vollständiges Beispiel

![](/docs/tutorials/blink-example.png)