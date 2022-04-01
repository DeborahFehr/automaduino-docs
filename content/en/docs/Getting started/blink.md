---
title: "Blink Example"
linkTitle: "Blink Example"
date: 2022-04-01
description: >
  This example teaches you how to generate the code for the blink program!
---

The blink program is the _Hello World_ program for the Arduino. We use a single LED and turn it on and off again with a slight delay. As a result the LED will blink, hence the name. If done correctly we can verify that our Arduino is working correctly and the connection is working.

### Scheme

To get started grab a LED and a resistor. Connect the LED to Pin 7 and use a breadboard to connect the GND pin with the resistor and LED. 

See the scheme below on an example for the connections.

![](/docs/tutorials/blink-sketch.png)

_Connection scheme for the blink program_

### Sketch

Now we first think about how our automata should look like. Use a pen and paper and try to sketch what is happening. An example automata is shown below. 

![](/docs/tutorials/blink-drawing.png)

_Blink sketch example_

#### Add States

Now we're going to translate our sketch to the Automaduino. For this we add two states to our canvas: A LED that is on and a LED that is off. 

![](/docs/tutorials/blink-states.png)

_Blink states_

#### Add Transitions

We're now going to connect the states. We start by connecting the start point with the ON state. After we turned the LED on, we want to wait a short time and then turn it off. To do this we connect it with the OFF state and select a delay of 1000 ms. To repeat our blink we connect back to the ON state. 

![](/docs/tutorials/blink-transitions.png)

_Blink transitions_

### Assign Pins

To finish our code generation we need to assign pins. We open the dialogue and add a LED component on pin 7. We then assign both available states to this component and submit. 

![](/docs/tutorials/blink-led-assignment.png)

_Full blink example_

### Upload

Now copy the code into the Arduino IDE and upload the sketch as detailed in the [Getting Started](/docs/getting-started/) guide. If you connected the LED correctly it should now blink! You successfully programmed an Arduino!


### Full Example

![](/docs/tutorials/blink-example.png)