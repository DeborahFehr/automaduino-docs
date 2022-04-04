---
title: "Relay"
linkTitle: "Relay"
date: 2022-24-02
weight: 4
description: >
  A motion sensor detects motion within a certain range.
---

{{< info-box header="Information">}}
{{< info-text >}}
  **Type** : Output

  **Mode** : Digital

  **Pins** : 0-14

  **Tutorial** : [funduino](https://funduino.de/nr-15-relais) 

  {{% pageinfo color="primary" %}}
**Note:** Be careful with external energy sources!
{{% /pageinfo %}}

  {{< /info-text >}}

  {{< info-image >}}
   ![](https://funduinoshop.com/media/image/9d/b7/e9/relais_karte_1-kanal_5v_230V.jpg)
   
   _Image by [funduino](https://funduinoshop.com/media/image/9d/b7/e9/relais_karte_1-kanal_5v_230V.jpg), CC-BY-SA._

  {{< /info-image >}}

{{< /info-box >}}

## Circuit Plan
![](/docs/connectionplan/steckplan_relay.png)
   
   _Plan made with [Fritzing](https://fritzing.org/)._

## Functions

#### On

{{< info-box >}}

  {{< info-image >}}
   ![](/docs/components/relay_on.png)
   
   _On State_

  {{< /info-image >}}

{{< info-text >}}

Switches the component off.
  
  {{< tabpane id="1">}}
  {{< tab header="Functions" >}}
void function_0_relay(){
digitalWrite(pin_0_relay, HIGH);
function_0_relay();
}
  {{< /tab >}}
  {{< tab header="Abridged" >}}
digitalWrite(pin_0_relay, HIGH);
  {{< /tab >}}
  {{< tab header="Switch" >}}
void function_0_relay(){
digitalWrite(pin_0_relay, HIGH);
state = 1;
}
  {{< /tab >}}
{{< /tabpane >}}

  {{< /info-text >}}

{{< /info-box >}}

#### Off

{{< info-box >}}

  {{< info-image >}}
   ![](/docs/components/relay_off.png)
   
   _Off State_

  {{< /info-image >}}

{{< info-text >}}

  Switches the component off.
  
  {{< tabpane id="2">}}
  {{< tab header="Functions" >}}
void function_0_relay(){
digitalWrite(pin_0_relay, LOW);
function_0_relay();
}
  {{< /tab >}}
  {{< tab header="Abridged" >}}
digitalWrite(pin_0_relay, LOW);
  {{< /tab >}}
  {{< tab header="Switch" >}}
void function_0_relay(){
digitalWrite(pin_0_relay, LOW);
state = 1;
}
  {{< /tab >}}
{{< /tabpane >}}

  {{< /info-text >}}

{{< /info-box >}}