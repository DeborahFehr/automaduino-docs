---
title: "Servo"
linkTitle: "Servo"
date: 2022-24-02
weight: 5
description: >
  A motion sensor detects motion within a certain range.
---

{{< info-box header="Information">}}
{{< info-text >}}
  **Type** : Output

  **Mode** : Servo Library

  **Pins** : 0-14

  **Tutorial** : [funduino](https://funduino.de/nr-12-servo-ansteuern) 
  
  {{% pageinfo color="primary" %}}
**Library:** You need to import the servo library to use this component!
{{% /pageinfo %}}

  {{% pageinfo color="primary" %}}
**Note:** Use with delay as the rotation takes some time. 
{{% /pageinfo %}}

  {{< /info-text >}}

  {{< info-image >}}
   ![](https://funduinoshop.com/media/image/a1/g0/17/25047.jpg)
   
   _Image by [funduino](https://funduinoshop.com/media/image/a1/g0/17/25047.jpg), CC-BY-SA._

  {{< /info-image >}}

{{< /info-box >}}

## Circuit Plan
![](/docs/connectionplan/steckplan_servo.png)
   
   _Plan made with [Fritzing](https://fritzing.org/)._

## Functions

#### Degree

{{< info-box >}}

  {{< info-image >}}
   ![](/docs/components/servo_0.png)
   
   _Turn servo to 0 degree_

   ![](/docs/components/servo_180.png)
   
   _Turn servo to 180 degree_

  {{< /info-image >}}

{{< info-text >}}

This function will turn the servo to the degree specified in the function name. 
  
  {{< tabpane id="1">}}
  {{< tab header="Functions" >}}
void function_1_servo(){
servo_0.write(0);
function_1_servo();
}
  {{< /tab >}}
  {{< tab header="Abridged" >}}
servo_0.write(0);
  {{< /tab >}}
  {{< tab header="Switch" >}}
void function_0_servo(){
servo_0.write(0);
state = 1;
}
  {{< /tab >}}
{{< /tabpane >}}

  {{< /info-text >}}

{{< /info-box >}}