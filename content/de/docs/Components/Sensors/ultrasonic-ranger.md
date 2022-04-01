---
title: "Ultrasonic Ranger"
linkTitle: "Ultrasonic Ranger"
date: 2022-24-02
weight: 6
description: >
  A ultrasonic ranger uses a ultrasonic wave to measure a distance.
---

{{< info-box header="Information">}}
{{< info-text >}}
  **Type** : Sensor

  **Mode** : Digital

  **Pins** : 0-14

  **Output Values** : Distance in cm (2-300)

  **Tutorial** : [funduino](https://funduino.de/nr-11-entfernungen-messen) 

    {{% pageinfo color="primary" %}}
**Note:** To use this component use the two states to send and receive a wave!
{{% /pageinfo %}}

  {{% pageinfo color="primary" %}}
**Note:** The read value needs to be transformed! See code below
{{% /pageinfo %}}

  {{< /info-text >}}

  {{< info-image >}}
   ![](https://funduinoshop.com/media/image/5d/e9/53/ultraschallsensor_hc-sr04_arduino_kompatibel_frontansicht.jpg)
   
   _Image by [funduino](https://funduinoshop.com/media/image/5d/e9/53/ultraschallsensor_hc-sr04_arduino_kompatibel_frontansicht.jpg), CC-BY-SA._

  {{< /info-image >}}

{{< /info-box >}}


## Functions

#### Send Wave

{{< info-box >}}

  {{< info-image >}}
   ![](/docs/components/ultrasonicranger-sender.png)
   
   _Send Wave State_

  {{< /info-image >}}

{{< info-text >}}

Sends a ultrasonic wave.
  
  {{< tabpane id="1">}}
  {{< tab header="Functions" >}}
void function_0_Ultraschall_messer(){
digitalWrite(pin_2_ultrasonicRanger, LOW);
delay(5);
digitalWrite(pin_2_ultrasonicRanger, HIGH);
delay(10);
digitalWrite(pin_2_ultrasonicRanger, LOW);
function_1_Ultraschall_messer();
}
  {{< /tab >}}
  {{< tab header="Abridged" >}}
digitalWrite(pin_2_ultrasonicRanger, LOW);
delay(5);
digitalWrite(pin_2_ultrasonicRanger, HIGH);
delay(10);
digitalWrite(pin_2_ultrasonicRanger, LOW);
  {{< /tab >}}
  {{< tab header="Switch" >}}
void function_0_Ultraschall_messer(){
digitalWrite(pin_2_ultrasonicRanger, LOW);
delay(5);
digitalWrite(pin_2_ultrasonicRanger, HIGH);
delay(10);
digitalWrite(pin_2_ultrasonicRanger, LOW);
state = 1;
}
  {{< /tab >}}
{{< /tabpane >}}

  {{< /info-text >}}

{{< /info-box >}}

#### Receive Wave

{{< info-box >}}

  {{< info-image >}}
   ![](/docs/components/ultrasonicranger-receiver.png)
   
   _Receive Wave State_

  {{< /info-image >}}

{{< info-text >}}

Receive a ultrasonic wave.
  
  {{< tabpane id="2">}}
  {{< tab header="Functions" >}}
void function_1_Ultraschall_messer(){
value = (pulseIn(pin_2_ultrasonicRanger, HIGH)/2) * 0.03432;
function_1_Ultraschall_messer();
}
  {{< /tab >}}
  {{< tab header="Abridged" >}}
value = (pulseIn(pin_2_ultrasonicRanger, HIGH)/2) * 0.03432;
  {{< /tab >}}
  {{< tab header="Switch" >}}
void function_1_Ultraschall_messer(){
value = (pulseIn(pin_2_ultrasonicRanger, HIGH)/2) * 0.03432;
state = 1; 
}
  {{< /tab >}}
{{< /tabpane >}}

  {{< /info-text >}}

{{< /info-box >}}