---
title: "Motion Sensor"
linkTitle: "Motion Sensor"
date: 2022-24-02
weight: 1
description: >
  A motion sensor detects motion within a certain range.
---

{{< info-box header="Information">}}
{{< info-text >}}
  **Type** : Sensor

  **Mode** : Digital

  **Pins** : 0-14

  **Output Values** : 0-1

  **Tutorial** : [funduino](https://funduino.de/nr-07-bewegungsmelder-hc-sr501) 

  {{< /info-text >}}

  {{< info-image >}}
   ![](https://funduinoshop.com/media/image/83/f8/e4/1071.jpg)
   
   _Image by [funduino](https://funduinoshop.com/media/image/83/f8/e4/1071.jpg), CC-BY-SA._

  {{< /info-image >}}

{{< /info-box >}}

## Connection scheme
![](/docs/connectionplan/steckplan_motionsensor.png)
   
  _Scheme made with [Fritzing](https://fritzing.org/)._

## Functions

#### Digital Read

{{< info-box >}}

  {{< info-image >}}
   ![](/docs/components/motionsensor.png)
   
   _Digital Read State_

  {{< /info-image >}}

{{< info-text >}}

Reads a digital value. 
  
  {{< tabpane id="1">}}
  {{< tab header="Functions" >}}
void function_0_motionSensor(){
value = digitalRead(pin_0_motionSensor);
function_0_motionSensor();
}
  {{< /tab >}}
  {{< tab header="Abridged" >}}
value = digitalRead(pin_0_motionSensor);
  {{< /tab >}}
  {{< tab header="Switch" >}}
void function_0_motionSensor(){
value = digitalRead(pin_0_motionSensor);
state = 1;
}
  {{< /tab >}}
{{< /tabpane >}}

  {{< /info-text >}}

{{< /info-box >}}