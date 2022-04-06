---
title: "Potentiometer"
linkTitle: "Potentiometer"
date: 2022-24-02
weight: 4
description: >
  A potentiometer returns a dynamic value based on the rotation.
---

{{< info-box header="Information">}}
{{< info-text >}}
  **Typ** : Nutzereingabe

  **Modus** : Analog

  **Pins** : 0-7 (analog)

  **Ausgabewerte** : 0-1023

  **Tutorial** : [funduino](https://funduino.de/nr-7-potentiometer) 

  {{< /info-text >}}

  {{< info-image >}}
   ![](https://funduinoshop.com/media/image/4f/86/67/8014.jpg)
   
   _Bild von [funduino](https://funduinoshop.com/media/image/4f/86/67/8014.jpg), CC-BY-SA._

  {{< /info-image >}}

{{< /info-box >}}

## Steckplan
![](/docs/connectionplan/steckplan_potentiometer.png)
   
   _Erstellt mit [Fritzing](https://fritzing.org/)._

## Funktionen

#### Erwarte Eingabe

{{< info-box >}}

  {{< info-image >}}
   ![](/docs/components/potentiometer.png)
   
   _Erwarte Eingabe Zustand_

  {{< /info-image >}}

{{< info-text >}}

Erwartet einen analogen Wert.
  
  {{< tabpane id="1">}}
  {{< tab header="Funktionsmodus" >}}
void function_0_Potentiometer(){
value = analogRead(pin_0_potentiometer);
function_0_Potentiometer();
}
  {{< /tab >}}
  {{< tab header="Kurzmodus" >}}
value = analogRead(pin_0_potentiometer);
  {{< /tab >}}
  {{< tab header="Schaltermodus" >}}
void function_0_Potentiometer(){
value = analogRead(pin_0_potentiometer);
state = 1;
}
  {{< /tab >}}
{{< /tabpane >}}

  {{< /info-text >}}

{{< /info-box >}}