---
title: "Bewegungssensor"
linkTitle: "Bewegungssensor"
date: 2022-24-02
weight: 1
description: >
  Ein Bewegungssensor reagiert auf Bewegungen in seiner Nähe.
---

{{< info-box header="Information">}}
{{< info-text >}}
  **Typ** : Sensor

  **Modus** : Digital

  **Pins** : 0-14

  **Ausgabewerte** : 0-1

  **Tutorial** : [funduino](https://funduino.de/nr-07-bewegungsmelder-hc-sr501) 

  {{< /info-text >}}

  {{< info-image >}}
   ![](https://funduinoshop.com/media/image/83/f8/e4/1071.jpg)
   
   _Bild von [funduino](https://funduinoshop.com/media/image/83/f8/e4/1071.jpg), CC-BY-SA._

  {{< /info-image >}}

{{< /info-box >}}

## Steckplan
![](/docs/connectionplan/steckplan_motionsensor.png)
   
   _Erstellt mit [Fritzing](https://fritzing.org/)._

## Funktionen

#### Digital Messen

{{< info-box >}}

  {{< info-image >}}
   ![](/docs/components/motionsensor.png)
   
   _Digital Messen Zustand_

  {{< /info-image >}}

{{< info-text >}}

Misst einen Wert digital.
  
  {{< tabpane id="1">}}
  {{< tab header="Funktionsmodus" >}}
void function_0_motionSensor(){
value = digitalRead(pin_0_motionSensor);
function_0_motionSensor();
}
  {{< /tab >}}
  {{< tab header="Kurzmodus" >}}
value = digitalRead(pin_0_motionSensor);
  {{< /tab >}}
  {{< tab header="Schaltermodus" >}}
void function_0_motionSensor(){
value = digitalRead(pin_0_motionSensor);
state = 1;
}
  {{< /tab >}}
{{< /tabpane >}}

  {{< /info-text >}}

{{< /info-box >}}