---
title: "Vibration Motor"
linkTitle: "Vibration Motor"
date: 2022-24-02
weight: 3
description: >
  A vibration motor will vibrate and is for example used in a smartphone.
---

{{< info-box header="Information">}}
{{< info-text >}}
  **Type** : Output

  **Mode** : Digital

  **Pins** : 0-14

  **Tutorial** : [elektro.turanis.de](https://elektro.turanis.de/html/prj020/index.html) 

  {{< /info-text >}}

  {{< info-image >}}
   ![](https://funduinoshop.com/media/image/c8/a7/5a/vibrationsmotor-multiple-front.jpg)
   
   _Image by [funduino](https://funduinoshop.com/media/image/c8/a7/5a/vibrationsmotor-multiple-front.jpg), CC-BY-SA._

  {{< /info-image >}}

{{< /info-box >}}


## Functions

#### On

{{< info-box >}}

  {{< info-image >}}
   ![](/docs/components/vibrationmotor_on.png)
   
   _On State_

  {{< /info-image >}}

{{< info-text >}}

Switches the component off.
  
  {{< tabpane id="1">}}
  {{< tab header="Functions" >}}
void function_0_vibrationMotor(){
digitalWrite(pin_0_vibrationMotor, HIGH);
function_0_vibrationMotor();
}
  {{< /tab >}}
  {{< tab header="Abridged" >}}
digitalWrite(pin_0_vibrationMotor, HIGH);
  {{< /tab >}}
  {{< tab header="Switch" >}}
void function_0_vibrationMotor(){
digitalWrite(pin_0_vibrationMotor, HIGH);
state = 1;
}
  {{< /tab >}}
{{< /tabpane >}}

  {{< /info-text >}}

{{< /info-box >}}

#### Off

{{< info-box >}}

  {{< info-image >}}
   ![](/docs/components/vibrationmotor_off.png)
   
   _Off State_

  {{< /info-image >}}

{{< info-text >}}

  Switches the component off.
  
  {{< tabpane id="2">}}
  {{< tab header="Functions" >}}
void function_0_vibrationMotor(){
digitalWrite(pin_0_vibrationMotor, LOW);
function_0_vibrationMotor();
}
  {{< /tab >}}
  {{< tab header="Abridged" >}}
digitalWrite(pin_0_vibrationMotor, LOW);
  {{< /tab >}}
  {{< tab header="Switch" >}}
void function_0_vibrationMotor(){
digitalWrite(pin_0_vibrationMotor, LOW);
state = 1;
}
  {{< /tab >}}
{{< /tabpane >}}

  {{< /info-text >}}

{{< /info-box >}}