---
title: "Loudness Sensor"
linkTitle: "Loudness Sensor"
date: 2022-24-02
weight: 5
description: >
  A loudness sensor measures noise.
---

{{< info-box header="Information">}}
{{< info-text >}}
  **Type** : Sensor

  **Mode** : Analog

  **Pins** : 0-7 (analog)

  **Output Values** : 0-1023

  **Tutorial** : [polluxlabs](https://polluxlabs.net/arduino-tutorials/einen-sound-sensor-am-arduino-verwenden/) 

  {{< /info-text >}}

  {{< info-image >}}
   ![](https://funduinoshop.com/media/image/48/c6/9b/waveshare-sound-modul-v2-mit-lm386-schallsensor-lautstaerkesensor-top.png)
   
   _Image by [funduino](https://funduinoshop.com/media/image/48/c6/9b/waveshare-sound-modul-v2-mit-lm386-schallsensor-lautstaerkesensor-top.png), CC-BY-SA._

  {{< /info-image >}}

{{< /info-box >}}

## Connection scheme
![](/docs/connectionplan/steckplan_loudnesssensor.png)
   
  _Scheme made with [Fritzing](https://fritzing.org/)._

## Functions

#### Analog Read

{{< info-box >}}

  {{< info-image >}}
   ![](/docs/components/loudnesssensor.png)
   
   _Analog Read State_

  {{< /info-image >}}

{{< info-text >}}

Reads a analog value.
  
  {{< tabpane id="1">}}
  {{< tab header="Functions" >}}
void function_0_Lautst_rke_sensor(){
value = analogRead(pin_0_loudnessSensor);
function_0_Lautst_rke_sensor();
}
  {{< /tab >}}
  {{< tab header="Abridged" >}}
value = analogRead(pin_0_loudnessSensor);
  {{< /tab >}}
  {{< tab header="Switch" >}}
void function_0_Lautst_rke_sensor(){
value = analogRead(pin_0_loudnessSensor);
state = 1;
}
  {{< /tab >}}
{{< /tabpane >}}

  {{< /info-text >}}

{{< /info-box >}}