---
title: "Vibrationsensor"
linkTitle: "Vibrationssensor"
date: 2022-24-02
weight: 4
description: >
  Ein Vibrationssensor reagiert auf Vibrationen oder Schütteln. 
---

{{< info-box header="Information">}}
{{< info-text >}}
  **Typ** : Sensor

  **Modus** : Digital

  **Pins** : 0-14

  **Ausgabewerte** : 0-1

  **Tutorial** : [funduino](https://funduino.de/nr-38-der-vibrationssensor) 

  {{< /info-text >}}

  {{< info-image >}}
   ![](https://funduinoshop.com/media/image/7c/0b/8d/vs1.jpg)
   
   _Bild von [funduino](https://funduinoshop.com/media/image/7c/0b/8d/vs1.jpg), CC-BY-SA._

  {{< /info-image >}}

{{< /info-box >}}

## Steckplan
![](/docs/connectionplan/steckplan_vibrationsensor.png)
   
   _Erstellt mit [Fritzing](https://fritzing.org/)._

## Funktionen

#### Digital Messen

{{< info-box >}}

  {{< info-image >}}
   ![](/docs/components/vibrationsensor.png)
   
   _Digital Messen Zustand_

  {{< /info-image >}}

{{< info-text >}}

Misst einen Wert digital.
  
  {{< tabpane id="1">}}
  {{< tab header="Funktionsmodus" >}}
void function_0_vibrationSensor(){
int value = digitalRead(pin_0_vibrationSensor);
function_0_vibrationSensor();
}
  {{< /tab >}}
  {{< tab header="Kurzmodus" >}}
int value = digitalRead(pin_0_vibrationSensor);
  {{< /tab >}}
  {{< tab header="Schaltermodus" >}}
void function_0_vibrationSensor(){
int value = digitalRead(pin_0_vibrationSensor);
state = 1;
}
  {{< /tab >}}
{{< /tabpane >}}

  {{< /info-text >}}

{{< /info-box >}}