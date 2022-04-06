---
title: "LED"
linkTitle: "LED"
date: 2022-24-02
weight: 1
description: >
  Eine LED, überlicherweise verwendet mit einem Widerstand, leuchtet.
---

{{< info-box header="Information">}}
{{< info-text >}}
  **Typ** : Ausgabe

  **Modus** : Digital

  **Pins** : 0-14

  **Tutorial** : [funduino](https://funduino.de/nr-2-wechselblinker) 

  {{% pageinfo color="primary" %}}
**Anmerkung:** Benutz die LED mit einem Widerstand!
{{% /pageinfo %}}

  {{< /info-text >}}

  {{< info-image >}}
   ![](https://funduinoshop.com/media/image/ec/82/a4/led_gruen_gelb_blau_rot_weiss_5mm.png)
   
   _Bild von [funduino](https://funduinoshop.com/media/image/ec/82/a4/led_gruen_gelb_blau_rot_weiss_5mm.png), CC-BY-SA._

  {{< /info-image >}}

{{< /info-box >}}

## Steckplan
![](/docs/connectionplan/steckplan_LED.png)
   
   _Erstellt mit [Fritzing](https://fritzing.org/)._

## Funktionen

#### An

{{< info-box >}}

  {{< info-image >}}
   ![](/docs/components/led_on.png)
   
   _An Zustand_

  {{< /info-image >}}

{{< info-text >}}

Schaltet die Komponente an.
  
  {{< tabpane id="1">}}
  {{< tab header="Funktionsmodus" >}}
void function_0_led(){
digitalWrite(pin_0_led, HIGH);
function_0_led();
}
  {{< /tab >}}
  {{< tab header="Kurzmodus" >}}
digitalWrite(pin_0_led, HIGH);
  {{< /tab >}}
  {{< tab header="Schaltermodus" >}}
void function_0_led(){
digitalWrite(pin_0_led, HIGH);
state = 1;
}
  {{< /tab >}}
{{< /tabpane >}}

  {{< /info-text >}}

{{< /info-box >}}

#### Aus

{{< info-box >}}

  {{< info-image >}}
   ![](/docs/components/led_off.png)
   
   _Aus Zustand_

  {{< /info-image >}}

{{< info-text >}}

  Schaltet die Komponente aus.
  
  {{< tabpane id="2">}}
  {{< tab header="Funktionsmodus" >}}
void function_0_led(){
digitalWrite(pin_0_led, LOW);
function_0_led();
}
  {{< /tab >}}
  {{< tab header="Kurzmodus" >}}
digitalWrite(pin_0_led, LOW);
  {{< /tab >}}
  {{< tab header="Schaltermodus" >}}
void function_0_led(){
digitalWrite(pin_0_led, LOW);
state = 1;
}
  {{< /tab >}}
{{< /tabpane >}}

  {{< /info-text >}}

{{< /info-box >}}
