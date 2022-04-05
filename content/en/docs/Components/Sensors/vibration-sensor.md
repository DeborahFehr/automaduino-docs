---
title: "Vibration Sensor"
linkTitle: "Vibration Sensor"
date: 2022-24-02
weight: 4
description: >
  A vibration sensor detects vibration next to it.
---

{{< info-box header="Information">}}
{{< info-text >}}
  **Type** : Sensor

  **Mode** : Digital

  **Pins** : 0-14

  **Output Values** : 0-1

  **Tutorial** : [funduino](https://funduino.de/nr-38-der-vibrationssensor) 

  {{< /info-text >}}

  {{< info-image >}}
   ![](https://funduinoshop.com/media/image/7c/0b/8d/vs1.jpg)
   
   _Image by [funduino](https://funduinoshop.com/media/image/7c/0b/8d/vs1.jpg), CC-BY-SA._

  {{< /info-image >}}

{{< /info-box >}}

## Connection scheme
![](/docs/connectionplan/steckplan_vibrationsensor.png)
   
  _Scheme made with [Fritzing](https://fritzing.org/)._

## Functions

#### Digital Read

{{< info-box >}}

  {{< info-image >}}
   ![](/docs/components/vibrationsensor.png)
   
   _Digital Read State_

  {{< /info-image >}}

{{< info-text >}}

Reads a digital value.
  
  {{< tabpane id="1">}}
  {{< tab header="Functions" >}}
void function_0_vibrationSensor(){
value = digitalRead(pin_0_vibrationSensor);
function_0_vibrationSensor();
}
  {{< /tab >}}
  {{< tab header="Abridged" >}}
value = digitalRead(pin_0_vibrationSensor);
  {{< /tab >}}
  {{< tab header="Switch" >}}
void function_0_vibrationSensor(){
value = digitalRead(pin_0_vibrationSensor);
state = 1;
}
  {{< /tab >}}
{{< /tabpane >}}

  {{< /info-text >}}

{{< /info-box >}}