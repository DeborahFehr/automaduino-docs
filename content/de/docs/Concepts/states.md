---
title: "States"
linkTitle: "States"
weight: 2
description: >
  A state contains the Arduino code for a component. There can be multiple functions available for a component.
---

States are a key component of finite state autmata. In Automaduino they are responsible for generating the code that is executed on the Arduino. 

### Overview

![](/docs/tutorials/state-overview.png)

_State overview_

Component
: The component this state will correspond to.

Link
: This button can be used to open the documentation containing more information about the expected input and other features. 

Name
: This field can be used to set a specific name for this state. The name will be used in the function generation and on the pin assignment screen. 

Function
: The function executed by this state. One component can have multiple functions. They are listed below each other in the component drawer.

Pin
: If a pin was assigned it will show the number on the state. If not the value "unassigned" will appear and the pin warning is shown in the code editor.

### Highlight Option

![](/docs/tutorials/highlight.png)

_Highlight Action example_

Automaduino features a highlight option to see which code corresponds to a specific state. To do this right click the block and select which part you want to see. This also works for transitions.