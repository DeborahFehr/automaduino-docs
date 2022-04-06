---
title: "Relais"
linkTitle: "Relais"
date: 2022-24-02
weight: 4
description: >
  Ein Relais wird verwendet um eine weitere elektrische Komponente ein- und auszuschalten.
---

{{< info-box header="Information">}}
{{< info-text >}}
  **Typ** : Ausgabe

  **Modus** : Digital

  **Pins** : 0-14

  **Tutorial** : [funduino](https://funduino.de/nr-15-relais) 

  {{% pageinfo color="primary" %}}
**Anmerkung:** Bei der Verwendung von elektrischen Bauteilen ist Vorsicht geboten!
{{% /pageinfo %}}

  {{< /info-text >}}

  {{< info-image >}}
   ![](https://funduinoshop.com/media/image/9d/b7/e9/relais_karte_1-kanal_5v_230V.jpg)
   
   _Bild von [funduino](https://funduinoshop.com/media/image/9d/b7/e9/relais_karte_1-kanal_5v_230V.jpg), CC-BY-SA._

  {{< /info-image >}}

{{< /info-box >}}

## Steckplan
![](/docs/connectionplan/steckplan_relay.png)
   
   _Erstellt mit [Fritzing](https://fritzing.org/)._

## Funktionen

#### An

{{< info-box >}}

  {{< info-image >}}
   ![](/docs/components/relay_on.png)
   
   _An Zustand_

  {{< /info-image >}}

{{< info-text >}}

Schaltet die Komponente an.
  
  {{< tabpane id="1">}}
  {{< tab header="Funktionsmodus" >}}
void function_0_relay(){
digitalWrite(pin_0_relay, HIGH);
function_0_relay();
}
  {{< /tab >}}
  {{< tab header="Kurzmodus" >}}
digitalWrite(pin_0_relay, HIGH);
  {{< /tab >}}
  {{< tab header="Schaltermodus" >}}
void function_0_relay(){
digitalWrite(pin_0_relay, HIGH);
state = 1;
}
  {{< /tab >}}
{{< /tabpane >}}

  {{< /info-text >}}

{{< /info-box >}}

#### Aus

{{< info-box >}}

  {{< info-image >}}
   ![](/docs/components/relay_off.png)
   
   _Aus Zustand_

  {{< /info-image >}}

{{< info-text >}}

  Schaltet die Komponente aus
  
  {{< tabpane id="2">}}
  {{< tab header="Funktionsmodus" >}}
void function_0_relay(){
digitalWrite(pin_0_relay, LOW);
function_0_relay();
}
  {{< /tab >}}
  {{< tab header="Kurzmodus" >}}
digitalWrite(pin_0_relay, LOW);
  {{< /tab >}}
  {{< tab header="Schaltermodus" >}}
void function_0_relay(){
digitalWrite(pin_0_relay, LOW);
state = 1;
}
  {{< /tab >}}
{{< /tabpane >}}

  {{< /info-text >}}

{{< /info-box >}}