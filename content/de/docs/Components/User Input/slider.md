---
title: "Schieberegler"
linkTitle: "Schieberegler"
date: 2022-24-02
weight: 3
description: >
  Der Wert eines Schiebereglers basiert auf seiner Position.
---

{{< info-box header="Information">}}
{{< info-text >}}
  **Typ** : Nutzereingabe

  **Modus** : Analog

  **Pins** : 0-7 (analog)

  **Ausgabewerte** : 0-1023

  **Tutorial** : [funduino](https://funduino.de/nr-15-schieberegler) 

  {{< /info-text >}}

  {{< info-image >}}
   ![](https://funduinoshop.com/media/image/bc/34/ce/schiebepotentiometer_linearpotentiometer_10k_ohm_rueckansicht.jpg)
   
   _Bild von [funduino](https://funduinoshop.com/media/image/bc/34/ce/schiebepotentiometer_linearpotentiometer_10k_ohm_rueckansicht.jpg), CC-BY-SA._

  {{< /info-image >}}

{{< /info-box >}}

## Steckplan
![](/docs/connectionplan/steckplan_slider.png)
   
   _Erstellt mit [Fritzing](https://fritzing.org/)._

## Funktionen

#### Erwarte Eingabe

{{< info-box >}}

  {{< info-image >}}
   ![](/docs/components/slider.png)
   
   _Erwarte Eingabe Zustand_

  {{< /info-image >}}

{{< info-text >}}

Erwartet einen analogen Wert.
  
  {{< tabpane id="1">}}
  {{< tab header="Funktionsmodus" >}}
void function_0_Schieberegler(){
value = analogRead(pin_0_slider);
function_0_Schieberegler();
}
  {{< /tab >}}
  {{< tab header="Kurzmodus" >}}
value = analogRead(pin_0_slider);
  {{< /tab >}}
  {{< tab header="Schaltermodus" >}}
void function_0_Schieberegler(){
value = analogRead(pin_0_slider);
state = 1;
}
  {{< /tab >}}
{{< /tabpane >}}

  {{< /info-text >}}

{{< /info-box >}}