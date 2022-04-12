---
title: "Temperatursensor"
linkTitle: "Temperatursensor"
date: 2022-24-02
weight: 2
description: >
  Ein Temperatursensor misst die aktuelle Lufttemperatur.
---

{{< info-box header="Information">}}
{{< info-text >}}
  **Typ** : Sensor

  **Modus** : Analog

  **Pins** : 0-7 (analog)

  **Ausgabewerte** : Wert in Celsius (0-40)

  **Tutorial** : [funduino](https://funduino.de/nr-10-temperatur-messen) 

  {{% pageinfo color="primary" %}}
**Anmerkung:** Der Messwert muss noch in Celsius umgerechnet werden! Siehe Beispielcode unten.
{{% /pageinfo %}}

  {{< /info-text >}}

  {{< info-image >}}
   ![](https://funduinoshop.com/media/image/ec/1e/17/temperatursensor-tmp36gt9z-arduino.jpg)
   
   _Bild von [funduino](https://funduinoshop.com/media/image/ec/1e/17/temperatursensor-tmp36gt9z-arduino.jpg), CC-BY-SA._

  {{< /info-image >}}

{{< /info-box >}}

## Steckplan
![](/docs/connectionplan/steckplan_temperaturesensor.png)
   
   _Erstellt mit [Fritzing](https://fritzing.org/)._

## Funktionen

#### Analog Messen

{{< info-box >}}

  {{< info-image >}}
   ![](/docs/components/temperaturesensor.png)
   
   _Analog Messen Zustand_

  {{< /info-image >}}

{{< info-text >}}

Misst einen Wert analog und gibt ihn in Celsius aus.
  
  {{< tabpane id="1">}}
  {{< tab header="Funktionsmodus" >}}
void function_0_temperatureSensor(){
int value = map(analogRead(pin_0_temperatureSensor), 0, 410, -50, 150);
function_0_temperatureSensor();
}
  {{< /tab >}}
  {{< tab header="Kurzmodus" >}}
int value = map(analogRead(pin_1_temperatureSensor), 0, 410, -50, 150);
  {{< /tab >}}
  {{< tab header="Schaltermodus" >}}
void function_0_temperatureSensor(){
int value = map(analogRead(pin_1_temperatureSensor), 0, 410, -50, 150);
state = 1;
}
  {{< /tab >}}
{{< /tabpane >}}

  {{< /info-text >}}

{{< /info-box >}}