---
title: "Button"
linkTitle: "Button"
date: 2022-24-02
weight: 1
description: >
  A button will detect if a user presses it.
---

{{< info-box header="Information">}}
{{< info-text >}}
  **Type** : User Input

  **Mode** : Digital

  **Pins** : 0-14

  **Output Values** : 0-1

  **Tutorial** : [funduino](https://funduino.de/nr-5-taster-am-arduino) 

  {{< /info-text >}}

  {{< info-image >}}
   ![](https://funduinoshop.com/media/image/19/1b/4e/4x-kurzhubtaster-2-pins-12x12x6mm-arduino.jpg)
   
   _Image by [funduino](https://funduinoshop.com/media/image/19/1b/4e/4x-kurzhubtaster-2-pins-12x12x6mm-arduino.jpg), CC-BY-SA._

  {{< /info-image >}}

{{< /info-box >}}

## Connection scheme
![](/docs/connectionplan/steckplan_button.png)
   
  _Scheme made with [Fritzing](https://fritzing.org/)._

## Functions

#### Await Input

{{< info-box >}}

  {{< info-image >}}
   ![](/docs/components/button.png)
   
   _Await Input State_

  {{< /info-image >}}

{{< info-text >}}

Awaits a digital value.
  
  {{< tabpane id="1">}}
  {{< tab header="Functions" >}}
void function_0_button(){
int value = digitalRead(pin_0_button);
delay(200);
function_0_button();
}
  {{< /tab >}}
  {{< tab header="Abridged" >}}
int value = digitalRead(pin_0_button);
delay(200);
  {{< /tab >}}
  {{< tab header="Switch" >}}
void function_0_button(){
int value = digitalRead(pin_0_button);
delay(200);
state = 1;
}
  {{< /tab >}}
{{< /tabpane >}}

  {{< /info-text >}}

{{< /info-box >}}