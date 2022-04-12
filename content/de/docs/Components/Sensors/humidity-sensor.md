---
title: "Nässesensor"
linkTitle: "Nässesensor"
date: 2022-24-02
weight: 3
description: >
  Ein Nässesensor misst die Feuchtigkeit in Erde oder in einem Glas.
---

{{< info-box header="Information">}}
{{< info-text >}}
  **Typ** : Sensor

  **Modus** : Analog

  **Pins** : 0-7 (analog)

  **Ausgabewerte** : 0-1023

  **Tutorial** : [funduino](https://funduino.de/nr-17-feuchtigkeitssensor) 

  {{% pageinfo color="primary" %}}
**Anmerkung:** Nur die unteren Teile des Sensors dürfen nass werden!
{{% /pageinfo %}}

  {{< /info-text >}}

  {{< info-image >}}
   ![](https://funduinoshop.com/media/image/ed/1c/24/feuchtigkeitssensor-fuer-arduino-mikrocontroller-front.jpg)
   
   _Bild von [funduino](https://funduinoshop.com/media/image/ed/1c/24/feuchtigkeitssensor-fuer-arduino-mikrocontroller-front.jpg), CC-BY-SA._

  {{< /info-image >}}

{{< /info-box >}}

## Steckplan
![](/docs/connectionplan/steckplan_humiditysensor.png)
   
   _Erstellt mit [Fritzing](https://fritzing.org/)._

## Funktionen

#### Analog Messen

{{< info-box >}}

  {{< info-image >}}
   ![](/docs/components/humiditysensor.png)
   
   _Analog Messen Zustand_

  {{< /info-image >}}

{{< info-text >}}

Misst einen Wert analog.
  
  {{< tabpane id="1">}}
  {{< tab header="Funktionsmodus" >}}
void function_0_humiditySensor(){
int value = analogRead(pin_0_humiditySensor);
function_0_humiditySensor();
}
  {{< /tab >}}
  {{< tab header="Kurzmodus" >}}
int value = analogRead(pin_0_humiditySensor);
  {{< /tab >}}
  {{< tab header="Schaltermodus" >}}
void function_0_humiditySensor(){
int value = analogRead(pin_0_humiditySensor);
state = 1;
}
  {{< /tab >}}
{{< /tabpane >}}

  {{< /info-text >}}

{{< /info-box >}}