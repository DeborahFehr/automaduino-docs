---
title: "LED"
linkTitle: "LED"
date: 2022-24-02
weight: 1
description: >
  A LED commonly used with a resistor emits light.
---

{{< info-box header="Information">}}
{{< info-text >}}
  **Type** : Output

  **Mode** : Digital

  **Pins** : 0-14

  **Tutorial** : [funduino](https://funduino.de/nr-2-wechselblinker) 

  {{% pageinfo color="primary" %}}
**Note:** Use with a resistor!
{{% /pageinfo %}}

  {{< /info-text >}}

  {{< info-image >}}
   ![](https://funduinoshop.com/media/image/ec/82/a4/led_gruen_gelb_blau_rot_weiss_5mm.png)
   
   _Image by [funduino](https://funduinoshop.com/media/image/ec/82/a4/led_gruen_gelb_blau_rot_weiss_5mm.png), CC-BY-SA._

  {{< /info-image >}}

{{< /info-box >}}

## Connection scheme
![](/docs/connectionplan/steckplan_LED.png)
   
  _Scheme made with [Fritzing](https://fritzing.org/)._

## Functions

#### On

{{< info-box >}}

  {{< info-image >}}
   ![](/docs/components/led_on.png)
   
   _On State_

  {{< /info-image >}}

{{< info-text >}}

Switches the component on.
  
  {{< tabpane id="1">}}
  {{< tab header="Functions" >}}
void function_0_led(){
digitalWrite(pin_0_led, HIGH);
function_0_led();
}
  {{< /tab >}}
  {{< tab header="Abridged" >}}
digitalWrite(pin_0_led, HIGH);
  {{< /tab >}}
  {{< tab header="Switch" >}}
void function_0_led(){
digitalWrite(pin_0_led, HIGH);
state = 1;
}
  {{< /tab >}}
{{< /tabpane >}}

  {{< /info-text >}}

{{< /info-box >}}

#### Off

{{< info-box >}}

  {{< info-image >}}
   ![](/docs/components/led_off.png)
   
   _Off State_

  {{< /info-image >}}

{{< info-text >}}

  Switches the component off.
  
  {{< tabpane id="2">}}
  {{< tab header="Functions" >}}
void function_0_led(){
digitalWrite(pin_0_led, LOW);
function_0_led();
}
  {{< /tab >}}
  {{< tab header="Abridged" >}}
digitalWrite(pin_0_led, LOW);
  {{< /tab >}}
  {{< tab header="Switch" >}}
void function_0_led(){
digitalWrite(pin_0_led, LOW);
state = 1;
}
  {{< /tab >}}
{{< /tabpane >}}

  {{< /info-text >}}

{{< /info-box >}}
