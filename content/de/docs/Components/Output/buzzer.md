---
title: "Summer"
linkTitle: "Summer"
date: 2022-24-02
weight: 2
description: >
  Ein Summer macht ein Geräusch. 
---

{{< info-box header="Information">}}
{{< info-text >}}
  **Typ** : Ausgabe

  **Modus** : Digital

  **Pins** : 0-14

  **Tutorial** : [funduino](https://funduino.de/nr-3-licht-und-ton) 

{{% pageinfo color="primary" %}}
**Anmerkung:** Nutz den Befehl tone(buzzer, 1000) um eine Tonhöhe festzulegen. 
{{% /pageinfo %}}

  {{< /info-text >}}

  {{< info-image >}}
   ![](https://funduinoshop.com/media/image/b2/76/8b/Piezo.png)
   
   _Bild von [funduino](https://funduinoshop.com/media/image/b2/76/8b/Piezo.png), CC-BY-SA._

  {{< /info-image >}}

{{< /info-box >}}

## Steckplan
![](/docs/connectionplan/steckplan_buzzer.png)
   
   _Erstellt mit [Fritzing](https://fritzing.org/)._

## Funktionen

#### An

{{< info-box >}}

  {{< info-image >}}
   ![](/docs/components/buzzer_on.png)
   
   _An Zustand_

  {{< /info-image >}}

{{< info-text >}}

Schaltet die Komponente an.
  
  {{< tabpane id="1">}}
  {{< tab header="Funktionsmodus" >}}
void function_0_buzzer(){
digitalWrite(pin_0_buzzer, HIGH);
function_0_buzzer();
}
  {{< /tab >}}
  {{< tab header="Kurzmodus" >}}
digitalWrite(pin_0_buzzer, HIGH);
  {{< /tab >}}
  {{< tab header="Schaltermodus" >}}
void function_0_buzzer(){
digitalWrite(pin_0_buzzer, HIGH);
state = 1;
}
  {{< /tab >}}
{{< /tabpane >}}

  {{< /info-text >}}

{{< /info-box >}}

#### Aus

{{< info-box >}}

  {{< info-image >}}
   ![](/docs/components/buzzer_off.png)
   
   _Aus Zustand_

  {{< /info-image >}}

{{< info-text >}}

  Schaltet die Komponente aus.
  
  {{< tabpane id="2">}}
  {{< tab header="Funktionsmodus" >}}
void function_0_buzzer(){
digitalWrite(pin_0_buzzer, LOW);
function_0_buzzer();
}
  {{< /tab >}}
  {{< tab header="Kurzmodus" >}}
digitalWrite(pin_0_buzzer, LOW);
  {{< /tab >}}
  {{< tab header="Schaltermodus" >}}
void function_0_buzzer(){
digitalWrite(pin_0_buzzer, LOW);
state = 1;
}
  {{< /tab >}}
{{< /tabpane >}}

  {{< /info-text >}}

{{< /info-box >}}