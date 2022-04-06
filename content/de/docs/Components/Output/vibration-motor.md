---
title: "Vibrationsmotor"
linkTitle: "Vibrationsmotor"
date: 2022-24-02
weight: 3
description: >
  Ein Vibrationsmotor vibriert. Er ist beispielsweise in einem Smartphone verbaut. 
---

{{< info-box header="Information">}}
{{< info-text >}}
  **Typ** : Ausgabe

  **Modus** : Digital

  **Pins** : 0-14

  **Tutorial** : [elektro.turanis.de](https://elektro.turanis.de/html/prj020/index.html) 

  {{< /info-text >}}

  {{< info-image >}}
   ![](https://funduinoshop.com/media/image/c8/a7/5a/vibrationsmotor-multiple-front.jpg)
   
   _Bild von [funduino](https://funduinoshop.com/media/image/c8/a7/5a/vibrationsmotor-multiple-front.jpg), CC-BY-SA._

  {{< /info-image >}}

{{< /info-box >}}

## Steckplan
![](/docs/connectionplan/steckplan_vibrationmotor.png)
   
   _Erstellt mit [Fritzing](https://fritzing.org/)._

## Funktionen

#### An

{{< info-box >}}

  {{< info-image >}}
   ![](/docs/components/vibrationmotor_on.png)
   
   _An Zustand_

  {{< /info-image >}}

{{< info-text >}}

Schaltet die Komponente an.
  
  {{< tabpane id="1">}}
  {{< tab header="Funktionsmodus" >}}
void function_0_vibrationMotor(){
digitalWrite(pin_0_vibrationMotor, HIGH);
function_0_vibrationMotor();
}
  {{< /tab >}}
  {{< tab header="Kurzmodus" >}}
digitalWrite(pin_0_vibrationMotor, HIGH);
  {{< /tab >}}
  {{< tab header="Schaltermodus" >}}
void function_0_vibrationMotor(){
digitalWrite(pin_0_vibrationMotor, HIGH);
state = 1;
}
  {{< /tab >}}
{{< /tabpane >}}

  {{< /info-text >}}

{{< /info-box >}}

#### Aus

{{< info-box >}}

  {{< info-image >}}
   ![](/docs/components/vibrationmotor_off.png)
   
   _Aus Zustand_

  {{< /info-image >}}

{{< info-text >}}

  Schaltet die Komponente aus.
  
  {{< tabpane id="2">}}
  {{< tab header="Funktionsmodus" >}}
void function_0_vibrationMotor(){
digitalWrite(pin_0_vibrationMotor, LOW);
function_0_vibrationMotor();
}
  {{< /tab >}}
  {{< tab header="Kurzmodus" >}}
digitalWrite(pin_0_vibrationMotor, LOW);
  {{< /tab >}}
  {{< tab header="Schaltermodus" >}}
void function_0_vibrationMotor(){
digitalWrite(pin_0_vibrationMotor, LOW);
state = 1;
}
  {{< /tab >}}
{{< /tabpane >}}

  {{< /info-text >}}

{{< /info-box >}}