---
title: "Slider"
linkTitle: "Slider"
date: 2022-24-02
weight: 3
description: >
  A slider returns a value based on its position.
---

{{< info-box header="Information">}}
{{< info-text >}}
  **Type** : User Input

  **Mode** : Analog

  **Pins** : 0-7 (analog)

  **Output Values** : 0-1023

  **Tutorial** : [funduino](https://funduino.de/nr-15-schieberegler) 

  {{< /info-text >}}

  {{< info-image >}}
   ![](https://funduinoshop.com/media/image/bc/34/ce/schiebepotentiometer_linearpotentiometer_10k_ohm_rueckansicht.jpg)
   
   _Image by [funduino](https://funduinoshop.com/media/image/bc/34/ce/schiebepotentiometer_linearpotentiometer_10k_ohm_rueckansicht.jpg), CC-BY-SA._

  {{< /info-image >}}

{{< /info-box >}}


## Functions

#### Await Input

{{< info-box >}}

  {{< info-image >}}
   ![](/docs/components/slider.png)
   
   _Await Input State_

  {{< /info-image >}}

{{< info-text >}}

Awaits a analog value.
  
  {{< tabpane id="1">}}
  {{< tab header="Functions" >}}
void function_0_Schieberegler(){
value = analogRead(pin_0_slider);
function_0_Schieberegler();
}
  {{< /tab >}}
  {{< tab header="Abridged" >}}
value = analogRead(pin_0_slider);
  {{< /tab >}}
  {{< tab header="Switch" >}}
void function_0_Schieberegler(){
value = analogRead(pin_0_slider);
state = 1;
}
  {{< /tab >}}
{{< /tabpane >}}

  {{< /info-text >}}

{{< /info-box >}}