---
title: "Schalter"
linkTitle: "Schalter"
date: 2022-24-02
weight: 2
description: >
  Ein Schalter ähnelt einem Taster, behält seinen Zustand aber bei.
---

{{< info-box header="Information">}}
{{< info-text >}}
  **Typ** : Nutzereingabe

  **Modus** : Digital

  **Pins** : 0-14

  **Ausgabewerte** : 0-1

  **Tutorial** : [funduino](https://funduino.de/nr-5-taster-am-arduino) 

  {{% pageinfo color="primary" %}}
**Anmerkung:** Ein Schalter funktioniert wie ein Taster, behält seinen Zustand aber bei.
{{% /pageinfo %}}

  {{< /info-text >}}

  {{< info-image >}}
   ![](https://funduinoshop.com/media/image/56/75/f9/schalter-mit-einer-position-2-54mm-front2.jpg)
   
   _Bild von [funduino](https://funduinoshop.com/media/image/56/75/f9/schalter-mit-einer-position-2-54mm-front2.jpg), CC-BY-SA._

  {{< /info-image >}}

{{< /info-box >}}

## Steckplan
![](/docs/connectionplan/steckplan_switch.png)
   
   _Erstellt mit [Fritzing](https://fritzing.org/)._

## Funktionen

#### Erwarte Eingabe

{{< info-box >}}

  {{< info-image >}}
   ![](/docs/components/switch.png)
   
   _Erwarte Eingabe Zustand_

  {{< /info-image >}}

{{< info-text >}}

Erwartet einen digitalen Wert.
  
  {{< tabpane id="1">}}
  {{< tab header="Funktionsmodus" >}}
void function_0_Schalter(){
value = digitalRead(pin_0_switch);
function_0_Schalter();
}
  {{< /tab >}}
  {{< tab header="Kurzmodus" >}}
value = digitalRead(pin_0_switch);
  {{< /tab >}}
  {{< tab header="Schaltermodus" >}}
void function_0_Schalter(){
value = digitalRead(pin_0_switch);
state = 1;
}
  {{< /tab >}}
{{< /tabpane >}}

  {{< /info-text >}}

{{< /info-box >}}