---
title: "Servo"
linkTitle: "Servo"
date: 2022-24-02
weight: 5
description: >
  Ein Servo ist ein kleiner Motor, der gedreht werden kann.
---

{{< info-box header="Information">}}
{{< info-text >}}
  **Typ** : Ausgabe

  **Modus** : Servo Bibilothek

  **Pins** : 0-14

  **Tutorial** : [funduino](https://funduino.de/nr-12-servo-ansteuern) 
  
  {{% pageinfo color="primary" %}}
**Bibliothek:** Du musst die Servo Bibliothek importieren um diese Komponente zu verwenden!
{{% /pageinfo %}}

  {{% pageinfo color="primary" %}}
**Anmerkung:** Verwende die Zustände immer mit einer kurzen Verzögerung, da die Drehung Zeit braucht.
{{% /pageinfo %}}

  {{< /info-text >}}

  {{< info-image >}}
   ![](https://funduinoshop.com/media/image/a1/g0/17/25047.jpg)
   
   _Bild von [funduino](https://funduinoshop.com/media/image/a1/g0/17/25047.jpg), CC-BY-SA._

  {{< /info-image >}}

{{< /info-box >}}

## Steckplan
![](/docs/connectionplan/steckplan_servo.png)
   
   _Erstellt mit [Fritzing](https://fritzing.org/)._

## Funktionen

#### Grad

{{< info-box >}}

  {{< info-image >}}
   ![](/docs/components/servo_0.png)
   
   _Dreht den Servo auf 0 Grad_

   ![](/docs/components/servo_180.png)
   
   _Dreht den Servo auf 180 Grad_

  {{< /info-image >}}

{{< info-text >}}

Diese Funktion dreht den Servo auf die angegebene Gradzahl.
  
  {{< tabpane id="1">}}
  {{< tab header="Funktionsmodus" >}}
void function_1_servo(){
servo_0.write(0);
function_1_servo();
}
  {{< /tab >}}
  {{< tab header="Kurzmodus" >}}
servo_0.write(0);
  {{< /tab >}}
  {{< tab header="Schaltermodus" >}}
void function_0_servo(){
servo_0.write(0);
state = 1;
}
  {{< /tab >}}
{{< /tabpane >}}

  {{< /info-text >}}

{{< /info-box >}}