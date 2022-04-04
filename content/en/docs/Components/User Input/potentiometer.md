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
  **Type** : User Input

  **Mode** : Analog

  **Pins** : 0-7 (analog)

  **Output Values** : 0-1023

  **Tutorial** : [funduino](https://funduino.de/nr-17-feuchtigkeitssensor) 

  {{% pageinfo color="primary" %}}
**Note:** Only the lower parts can get wet!
{{% /pageinfo %}}

  {{< /info-text >}}

  {{< info-image >}}
   ![](https://funduinoshop.com/media/image/4f/86/67/8014.jpg)
   
   _Image by [funduino](https://funduinoshop.com/media/image/4f/86/67/8014.jpg), CC-BY-SA._

  {{< /info-image >}}

{{< /info-box >}}

## Circuit Plan
![](/docs/connectionplan/steckplan_potentiometer.png)
   
   _Plan made with [Fritzing](https://fritzing.org/)._

## Functions

#### Await Input

{{< info-box >}}

  {{< info-image >}}
   ![](/docs/components/potentiometer.png)
   
   _Await Input State_

  {{< /info-image >}}

{{< info-text >}}

Awaits a analog value.
  
  {{< tabpane id="1">}}
  {{< tab header="Functions" >}}
void function_0_Potentiometer(){
value = analogRead(pin_0_potentiometer);
function_0_Potentiometer();
}
  {{< /tab >}}
  {{< tab header="Abridged" >}}
value = analogRead(pin_0_potentiometer);
  {{< /tab >}}
  {{< tab header="Switch" >}}
void function_0_Potentiometer(){
value = analogRead(pin_0_potentiometer);
state = 1;
}
  {{< /tab >}}
{{< /tabpane >}}

  {{< /info-text >}}

{{< /info-box >}}