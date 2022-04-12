---
title: "Lautstärkesensor"
linkTitle: "Lautstärkesensor"
date: 2022-24-02
weight: 5
description: >
  Ein Lautstärkesensor misst Geräusche in seiner Umgebung.
---

{{< info-box header="Information">}}
{{< info-text >}}
  **Typ** : Sensor

  **Modus** : Analog

  **Pins** : 0-7 (analog)

  **Ausgabewerte** : 0-1023

  **Tutorial** : [polluxlabs](https://polluxlabs.net/arduino-tutorials/einen-sound-sensor-am-arduino-verwenden/) 

  {{< /info-text >}}

  {{< info-image >}}
   ![](https://funduinoshop.com/media/image/48/c6/9b/waveshare-sound-modul-v2-mit-lm386-schallsensor-lautstaerkesensor-top.png)
   
   _Bild von [funduino](https://funduinoshop.com/media/image/48/c6/9b/waveshare-sound-modul-v2-mit-lm386-schallsensor-lautstaerkesensor-top.png), CC-BY-SA._

  {{< /info-image >}}

{{< /info-box >}}

## Steckplan
![](/docs/connectionplan/steckplan_loudnesssensor.png)
   
   _Erstellt mit [Fritzing](https://fritzing.org/)._

## Funktionen

#### Analog Messen

{{< info-box >}}

  {{< info-image >}}
   ![](/docs/components/loudnesssensor.png)
   
   _Analog Messen Zustand_

  {{< /info-image >}}

{{< info-text >}}

Misst einen Wert analog.
  
  {{< tabpane id="1">}}
  {{< tab header="Funktionsmodus" >}}
void function_0_Lautst_rke_sensor(){
int value = analogRead(pin_0_loudnessSensor);
function_0_Lautst_rke_sensor();
}
  {{< /tab >}}
  {{< tab header="Kurzmodus" >}}
int value = analogRead(pin_0_loudnessSensor);
  {{< /tab >}}
  {{< tab header="Schaltermodus" >}}
void function_0_Lautst_rke_sensor(){
int value = analogRead(pin_0_loudnessSensor);
state = 1;
}
  {{< /tab >}}
{{< /tabpane >}}

  {{< /info-text >}}

{{< /info-box >}}