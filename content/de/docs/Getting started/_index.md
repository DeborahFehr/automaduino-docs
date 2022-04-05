---
title: "Erste Schritte"
linkTitle: "Erste Schritte"
weight: 2
description: >
  Alles was du wissen musst um mit Automaduino loszulegen!
---

Du möchtest mit Automaduino programmieren? Super! Hier wird die Benutzeroberfläche des Editors erklärt und wie du Code generieren kannst.

### Überblick

![](/docs/tutorials/automaduino-overview.png)

_Automaduino Editor Übersicht_

Der Editor besteht aus folgenden Teilen:

Komponentenmenü
: In diesem Menü findest du alle Komponenten, die du benutzen kannst. Mehr Informationen über die einzelnen Komponenten findest du auf der [Komponentenseite](/docs/components/).

Start Punkt
: Der Startpunkt für dein Programm. Du musst ihn mit einem Zustand verbinden damit dein Code funktioniert.

Zustand
: Ein Zustand besteht aus einer Komponente und einer Funktion. Der Zustand führt die Funktion auf dem Arduino aus. Finde mehr über Zustände heraus indem du [hier klickst](/docs/concepts/states/).

Übergang
: Ein Übergang verbindet zwei Zustände und bestimmt wie und wann der nächste Block ausgeführt wird. Es gibt mehrere Möglichkeiten für die Übergänge. Finde mehr über Übergänge heraus indem du [hier klickst](/docs/concepts/transitions/).

Pin Zuweisung
: Dieser Button öffnet die Pinzuweisung. Das ist notwendig damit der Arduino weiß an welchem Pin welche Komponente angeschlossen ist. Wenn ein Zustand keinen Pin zugewiesen hat wird eine Warnung angezeigt. 

Code
: Hier siehst du den erzeugten Code! Der Code wird immer generiert wenn du einen neuen Zustand hinzufügst oder zwei Zustände verbindest. Du kannst den Code hier auch als Texteditor verwenden. 

Code Stil
: Der Code Stil ermöglicht es dir verschiedene Stile für den generierten Code auszuwählen. Dieses Feature ist für erfahrene Programmierer. Alle [Code Stile](/docs/concepts/code-style/) werden hier erklärt.

### Pin Zuweisung

In diesem Dialog kannst du Pins für die angeschlossenen Komponenten zuweisen.

![](/docs/tutorials/pin-assignment.png)
_Beispiel Pinzuweisung_

Füge zuerst eine neue Komponente hinzu, dann wähle einen Pin aus und welche Komponente angeschlossen werden soll. Sobald du das gemacht hast kannst du von unten einen Zustand zur Komponente ziehen. 

Sobald du fertig bist klicke auf den Absenden Button.

_Tipp: Benenne deine Zustände um damit du genau weißt was du zuweist!_

### Code kopieren.

Um den Code zu benutzen musst du ihn kipieren. Du kannst allen Code von Hand kopieren oder den Shortcut im Editor verwenden. 

![](/docs/tutorials/copy-code-editor.png)
_Shortcut im Editor zum Kopieren_

Wenn der Editor zu ist kannst du stattdessen den Button hier verwenden. Außerdem gibt es hier einen Shortcut für die Pinzuweisung. 

![](/docs/tutorials/copy-code-closed.png)

_Shortcut im geschlossenen Editor zum Kopieren_


### Arduino IDE

Um einen Sketch hochzuladen musst du die [Arduino IDE](https://www.arduino.cc/en/software) verwenden. 

Nachdem du die Software erfolgreich installiert hast, öffne die IDE und wähle dein Board aus. Das ist normalerweise "Arduino Uno". 

![](/docs/tutorials/board-selection.png)
_Board Auswahl Menü_

Als nächstes verbinde dein Board per USB mit deinem Computer. Wähle dein Board in der Port Auswahl. Der richtige Port hat in Klammern den Namen des Board daneben. 

![](/docs/tutorials/port-selection.png)
_Port Auswahl Menü_

Jetzt kannst du den Code aus dem Automaduino Editor kopieren und ihn in der IDE einfügen. Um den Code auf den Arduino zu laden drücke auf den Hochladen Button wenn du das Board per USB verbunden hast. Jetzt ist dein Programm auf dem Arduino! 

![](/docs/tutorials/upload-button.png)
_Hochladen Button_


##
**Um ein ganzes Beispiel zu sehen schau dir die Blink Seite an!**