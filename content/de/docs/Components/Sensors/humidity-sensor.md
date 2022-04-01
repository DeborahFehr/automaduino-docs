---
title: "Humidity Sensor"
linkTitle: "Humidity Sensor"
date: 2022-24-02
weight: 3
description: >
  A humidity sensor measures the humidity of earth or water.
---

{{< info-box header="Information">}}
{{< info-text >}}
  **Type** : Sensor

  **Mode** : Analog

  **Pins** : 0-7 (analog)

  **Output Values** : 0-1023

  **Tutorial** : [funduino](https://funduino.de/nr-17-feuchtigkeitssensor) 

  {{% pageinfo color="primary" %}}
**Note:** Only the lower parts can get wet!
{{% /pageinfo %}}

  {{< /info-text >}}

  {{< info-image >}}
   ![](https://funduinoshop.com/media/image/ed/1c/24/feuchtigkeitssensor-fuer-arduino-mikrocontroller-front.jpg)
   
   _Image by [funduino](https://funduinoshop.com/media/image/ed/1c/24/feuchtigkeitssensor-fuer-arduino-mikrocontroller-front.jpg), CC-BY-SA._

  {{< /info-image >}}

{{< /info-box >}}


## Functions

#### Analog Read

{{< info-box >}}

  {{< info-image >}}
   ![](/docs/components/humiditysensor.png)
   
   _Read Analog State_

  {{< /info-image >}}

{{< info-text >}}

Reads a analog value.
  
  {{< tabpane id="1">}}
  {{< tab header="Functions" >}}
void function_0_humiditySensor(){
value = analogRead(pin_0_humiditySensor);
function_0_humiditySensor();
}
  {{< /tab >}}
  {{< tab header="Abridged" >}}
value = analogRead(pin_0_humiditySensor);
  {{< /tab >}}
  {{< tab header="Switch" >}}
void function_0_humiditySensor(){
value = analogRead(pin_0_humiditySensor);
state = 1;
}
  {{< /tab >}}
{{< /tabpane >}}

  {{< /info-text >}}

{{< /info-box >}}