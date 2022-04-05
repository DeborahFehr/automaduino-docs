---
title: "Übergänge"
linkTitle: "Übergänge"
weight: 3
description: >
  Übergänge beschreiben wie wir von einem Zustand zum nächsten kommen. Hierfür gibt es verschiedene Möglichkeiten.
---

### Überblick

![](/docs/tutorials/blink-transitions.png)
_Beispiel für einen Übergang im [Blink Programm](/docs/getting-started/blink/)._

Übergänge verbinden Zustände. Nachdem der Code aus einem Zustand ausgeführt wurde beschreibt der Übergang welcher Zustand als nächstes aufgeführt wird. D _dann_ und _nach_ Übergang steht allen Komponenten zur Verfügung, während der _falls_, _oder_ und _wenn_ Übergang nur Benutzereingabe Komponenten und Sensoren zur Verfügung steht, da diese von der von der Komponente erzeugten Eingabe abhängen. 

### Übergänge

#### Dann

![](/docs/tutorials/dann.png)

_dann Beispiel_

Ein dann Übergang führt sofort im Anschluss den nächsten Zustand aus. 

#### Nach

![](/docs/tutorials/nach.png)

_nach Beispiel_

Ein nach Übergang pausiert für eine bestimmte Anzahl an Millisekunden und führt dann den nächsten Zustand aus.

#### Falls

![](/docs/tutorials/falls.png)

_falls Beispiel_

Ein falls Übergang geht erst zum nächsten Zustand über wenn eine bestimmte Bedingung erfüllt wurde, sonst führt er weiterhin den aktuellen Zustand aus. Das ist sinnvoll für Benutzereingaben. 

#### Oder

![](/docs/tutorials/oder.png)

_oder Beispiel_

Ein oder Übgergang geht erst zum nächsten Zustand über wenn eine bestimmte Bedingung erfüllt wurde, sonst führt er einen anderen Zustand aus. Das ist sinnvoll für Sensoren.

#### Wenn

![](/docs/tutorials/wenn.png)

_wenn Beispiel_

Ein wenn Übergang führt verschiedene Zustände aus, abhängig von der Eingabe. Es wird immer nur die erste zutreffende Bedingung ausgeführt. Das macht Sinn für analoge Sensoren, da wir hier unterschiedliche Bereiche für die Eingabe definieren können. 