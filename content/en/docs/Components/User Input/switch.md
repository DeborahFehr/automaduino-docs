---
title: "Switch"
linkTitle: "Switch"
date: 2022-24-02
weight: 2
description: >
  A switch works similar to a button to detect an input. 
---

{{< info-box header="Information">}}
{{< info-text >}}
  **Type** : User Input

  **Mode** : Digital

  **Pins** : 0-14

  **Output Values** : 0-1

  **Tutorial** : [funduino](https://funduino.de/nr-5-taster-am-arduino) 

  {{% pageinfo color="primary" %}}
**Note:** A switch works the same way as a button but you can always the the current status.
{{% /pageinfo %}}

  {{< /info-text >}}

  {{< info-image >}}
   ![](https://funduinoshop.com/media/image/56/75/f9/schalter-mit-einer-position-2-54mm-front2.jpg)
   
   _Image by [funduino](https://funduinoshop.com/media/image/56/75/f9/schalter-mit-einer-position-2-54mm-front2.jpg), CC-BY-SA._

  {{< /info-image >}}

{{< /info-box >}}

## Connection scheme
![](/docs/connectionplan/steckplan_switch.png)
   
   _Scheme made with [Fritzing](https://fritzing.org/)._

## Functions

#### Await Input

{{< info-box >}}

  {{< info-image >}}
   ![](/docs/components/switch.png)
   
   _Await Input State_

  {{< /info-image >}}

{{< info-text >}}

Awaits a digital value.
  
  {{< tabpane id="1">}}
  {{< tab header="Functions" >}}
void function_0_Schalter(){
int value = digitalRead(pin_0_switch);
function_0_Schalter();
}
  {{< /tab >}}
  {{< tab header="Abridged" >}}
int value = digitalRead(pin_0_switch);
  {{< /tab >}}
  {{< tab header="Switch" >}}
void function_0_Schalter(){
int value = digitalRead(pin_0_switch);
state = 1;
}
  {{< /tab >}}
{{< /tabpane >}}

  {{< /info-text >}}

{{< /info-box >}}