---
title: "Temperature Sensor"
linkTitle: "Temperature Sensor"
date: 2022-24-02
weight: 2
description: >
  A temperature sensor measures the current temperature in the air.
---

{{< info-box header="Information">}}
{{< info-text >}}
  **Type** : Sensor

  **Mode** : Analog

  **Pins** : 0-7 (analog)

  **Output Values** : Value in Celsius (0-40)

  **Tutorial** : [funduino](https://funduino.de/nr-10-temperatur-messen) 

  {{% pageinfo color="primary" %}}
**Note:** The value needs to be transformed to celsius! See code below.
{{% /pageinfo %}}

  {{< /info-text >}}

  {{< info-image >}}
   ![](https://funduinoshop.com/media/image/ec/1e/17/temperatursensor-tmp36gt9z-arduino.jpg)
   
   _Image by [funduino](https://funduinoshop.com/media/image/ec/1e/17/temperatursensor-tmp36gt9z-arduino.jpg), CC-BY-SA._

  {{< /info-image >}}

{{< /info-box >}}


## Functions

#### Analog Read

{{< info-box >}}

  {{< info-image >}}
   ![](/docs/components/temperaturesensor.png)
   
   _Analog Read State_

  {{< /info-image >}}

{{< info-text >}}

Reads a analog value and transforms it to Celsius.
  
  {{< tabpane id="1">}}
  {{< tab header="Functions" >}}
void function_0_temperatureSensor(){
value = map(analogRead(pin_0_temperatureSensor), 0, 410, -50, 150);
function_0_temperatureSensor();
}
  {{< /tab >}}
  {{< tab header="Abridged" >}}
value = map(analogRead(pin_1_temperatureSensor), 0, 410, -50, 150);
  {{< /tab >}}
  {{< tab header="Switch" >}}
void function_0_temperatureSensor(){
value = map(analogRead(pin_1_temperatureSensor), 0, 410, -50, 150);
state = 1;
}
  {{< /tab >}}
{{< /tabpane >}}

  {{< /info-text >}}

{{< /info-box >}}