---
title: "Taster"
linkTitle: "Taster"
date: 2022-24-02
weight: 1
description: >
  Ein Taster reagiert darauf wenn ein Nutzer ihn drückt. 
---

{{< info-box header="Information">}}
{{< info-text >}}
  **Typ** : Nutzereingabe

  **Modus** : Digital

  **Pins** : 0-14

  **Ausgabewerte** : 0-1

  **Tutorial** : [funduino](https://funduino.de/nr-5-taster-am-arduino) 

  {{< /info-text >}}

  {{< info-image >}}
   ![](https://funduinoshop.com/media/image/19/1b/4e/4x-kurzhubtaster-2-pins-12x12x6mm-arduino.jpg)
   
   _Bild von [funduino](https://funduinoshop.com/media/image/19/1b/4e/4x-kurzhubtaster-2-pins-12x12x6mm-arduino.jpg), CC-BY-SA._

  {{< /info-image >}}

{{< /info-box >}}

## Steckplan
![](/docs/connectionplan/steckplan_button.png)
   
   _Erstellt mit [Fritzing](https://fritzing.org/)._

## Funktionen

#### Erwarte Eingabe

{{< info-box >}}

  {{< info-image >}}
   ![](/docs/components/button.png)
   
   _Erwarte Eingabe Zustand_

  {{< /info-image >}}

{{< info-text >}}

Erwartet einen digitalen Wert.
  
  {{< tabpane id="1">}}
  {{< tab header="Funktionsmodus" >}}
void function_0_button(){
int value = digitalRead(pin_0_button);
delay(200);
function_0_button();
}
  {{< /tab >}}
  {{< tab header="Kurzmodus" >}}
int value = digitalRead(pin_0_button);
delay(200);
  {{< /tab >}}
  {{< tab header="Schaltermodus" >}}
void function_0_button(){
int value = digitalRead(pin_0_button);
delay(200);
state = 1;
}
  {{< /tab >}}
{{< /tabpane >}}

  {{< /info-text >}}

{{< /info-box >}}