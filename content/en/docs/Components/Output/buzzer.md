---
title: "Buzzer"
linkTitle: "Buzzer"
date: 2022-24-02
weight: 2
description: >
  A buzzer will emit a sound. 
---

{{< info-box header="Information">}}
{{< info-text >}}
  **Type** : Output

  **Mode** : Digital

  **Pins** : 0-14

  **Tutorial** : [funduino](https://funduino.de/nr-3-licht-und-ton) 

{{% pageinfo color="primary" %}}
**Note:** Use tone(buzzer, 1000) to set the tone height. 
{{% /pageinfo %}}

  {{< /info-text >}}

  {{< info-image >}}
   ![](https://funduinoshop.com/media/image/b2/76/8b/Piezo.png)
   
   _Image by [funduino](https://funduinoshop.com/media/image/b2/76/8b/Piezo.png), CC-BY-SA._

  {{< /info-image >}}

{{< /info-box >}}

## Circuit Plan
![](/docs/connectionplan/steckplan_buzzer.png)
   
   _Plan made with [Fritzing](https://fritzing.org/)._

## Functions

#### On

{{< info-box >}}

  {{< info-image >}}
   ![](/docs/components/buzzer_on.png)
   
   _On State_

  {{< /info-image >}}

{{< info-text >}}

Switches the component off.
  
  {{< tabpane id="1">}}
  {{< tab header="Functions" >}}
void function_0_buzzer(){
digitalWrite(pin_0_buzzer, HIGH);
function_0_buzzer();
}
  {{< /tab >}}
  {{< tab header="Abridged" >}}
digitalWrite(pin_0_buzzer, HIGH);
  {{< /tab >}}
  {{< tab header="Switch" >}}
void function_0_buzzer(){
digitalWrite(pin_0_buzzer, HIGH);
state = 1;
}
  {{< /tab >}}
{{< /tabpane >}}

  {{< /info-text >}}

{{< /info-box >}}

#### Off

{{< info-box >}}

  {{< info-image >}}
   ![](/docs/components/buzzer_off.png)
   
   _Off State_

  {{< /info-image >}}

{{< info-text >}}

  Switches the component off.
  
  {{< tabpane id="2">}}
  {{< tab header="Functions" >}}
void function_0_buzzer(){
digitalWrite(pin_0_buzzer, LOW);
function_0_buzzer();
}
  {{< /tab >}}
  {{< tab header="Abridged" >}}
digitalWrite(pin_0_buzzer, LOW);
  {{< /tab >}}
  {{< tab header="Switch" >}}
void function_0_buzzer(){
digitalWrite(pin_0_buzzer, LOW);
state = 1;
}
  {{< /tab >}}
{{< /tabpane >}}

  {{< /info-text >}}

{{< /info-box >}}