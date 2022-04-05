---
title: "Zustände"
linkTitle: "Zustände"
weight: 2
description: >
  Ein Zustand beinhaltet den Arduino Code für eine Komponente. Es gibt mehrere Funktionen pro Komponente. 
---

Zustände sind ein wichtiger Teil der endlichen Automaten. In Automaduino werden Zustände verwendet um die dargestellte Funktion auf dem Arduino auszuführen. 

### Überblick

![](/docs/tutorials/state-overview.png)

_Überblick Zustand_

Komponente
: Die angesprochene Komponente.

Link
: Dieser Button öffnet die Dokumentation. Hier findet man weitere Informationen über den Code, Steckpläne und vieles mehr. 

Name
: Dieses Feld kann verwendet werden um einem Zustand einen spezifischen Namen zu geben. Der Name wird verwendet in der Funktionsgeneration und in der Pinzuweisung. 

Funktion
: Die von diesem Zustand ausgeführte Funktion. Es kann mehrere Funktionen pro Komponente geben.Die Funktionen sind untereinander im Auswahlmenü aufgeführt.

Pin
: Wenn ein Pin zugewiesen wurde wird die Nummer hier angezeigt. Falls dies nicht der Fall ist erscheint ein Warnhinweis im Code Editor. 

### Hervorheben

![](/docs/tutorials/highlight.png)

_Beispiel hervorgehobener Code_

Automaduino bietet die Möglichkeit den von einem Zustand generierten Code hervorzuheben. Klicke mit rechts auf einen Zustand und wähle aus welchen Teil du hervorheben möchtest. Das funktioniert auch für Übergänge. 