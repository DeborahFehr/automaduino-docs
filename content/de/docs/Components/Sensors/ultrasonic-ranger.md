---
title: "Ultraschallmesser"
linkTitle: "Ultraschallmesser"
date: 2022-24-02
weight: 6
description: >
  Ein Ultraschallmesser sendet eine Ultraschallwelle aus um eine Distanz zu messen.
---

{{< info-box header="Information">}}
{{< info-text >}}
  **Typ** : Sensor

  **Modus** : Digital

  **Pins** : 0-14

  **Ausgabewerte** : Distanz in cm (2-300)

  **Tutorial** : [funduino](https://funduino.de/nr-11-entfernungen-messen) 

    {{% pageinfo color="primary" %}}
**Anmerkung:** Um diese Komponente zu verwenden musst du beide Zustände nacheinander verwenden! 
{{% /pageinfo %}}

  {{% pageinfo color="primary" %}}
**Anmerkung:** Der gemessene Wert muss noch umgewandelt werden! Siehe Code unten.
{{% /pageinfo %}}

  {{< /info-text >}}

  {{< info-image >}}
   ![](https://funduinoshop.com/media/image/5d/e9/53/ultraschallsensor_hc-sr04_arduino_kompatibel_frontansicht.jpg)
   
   _Bild von [funduino](https://funduinoshop.com/media/image/5d/e9/53/ultraschallsensor_hc-sr04_arduino_kompatibel_frontansicht.jpg), CC-BY-SA._

  {{< /info-image >}}

{{< /info-box >}}

## Steckplan
![](/docs/connectionplan/steckplan_ultrasonicranger.png)
   
   _Erstellt mit [Fritzing](https://fritzing.org/)._

## Funktionen

#### Welle senden

{{< info-box >}}

  {{< info-image >}}
   ![](/docs/components/ultrasonicranger-sender.png)
   
   _Welle senden Zustand_

  {{< /info-image >}}

{{< info-text >}}

Sendet eine Ultraschallwelle aus. 
  
  {{< tabpane id="1">}}
  {{< tab header="Funktionsmodus" >}}
void function_0_Ultraschall_messer(){
digitalWrite(pin_2_ultrasonicRanger, LOW);
delay(5);
digitalWrite(pin_2_ultrasonicRanger, HIGH);
delay(10);
digitalWrite(pin_2_ultrasonicRanger, LOW);
function_1_Ultraschall_messer();
}
  {{< /tab >}}
  {{< tab header="Kurzmodus" >}}
digitalWrite(pin_2_ultrasonicRanger, LOW);
delay(5);
digitalWrite(pin_2_ultrasonicRanger, HIGH);
delay(10);
digitalWrite(pin_2_ultrasonicRanger, LOW);
  {{< /tab >}}
  {{< tab header="Schaltermodus" >}}
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

#### Welle lesen

{{< info-box >}}

  {{< info-image >}}
   ![](/docs/components/ultrasonicranger-receiver.png)
   
   _Welle lesen Zustand_

  {{< /info-image >}}

{{< info-text >}}

Liest eine Ultraschallwelle aus.
  
  {{< tabpane id="2">}}
  {{< tab header="Funktionsmodus" >}}
void function_1_Ultraschall_messer(){
value = (pulseIn(pin_2_ultrasonicRanger, HIGH)/2) * 0.03432;
function_1_Ultraschall_messer();
}
  {{< /tab >}}
  {{< tab header="Kurzmodus" >}}
value = (pulseIn(pin_2_ultrasonicRanger, HIGH)/2) * 0.03432;
  {{< /tab >}}
  {{< tab header="Schaltermodus" >}}
void function_1_Ultraschall_messer(){
value = (pulseIn(pin_2_ultrasonicRanger, HIGH)/2) * 0.03432;
state = 1; 
}
  {{< /tab >}}
{{< /tabpane >}}

  {{< /info-text >}}

{{< /info-box >}}