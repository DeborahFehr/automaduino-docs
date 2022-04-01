---
title: "Automata"
linkTitle: "Automata"
weight: 1
description: >
  Automata are finite state machines and are used to represent behaviour in Automaduino.
---

### Finite State Machine (Automaton)

A finite state machine, also called automaton, is a computation model in which a machine can at any given time hold one state. They perform a predicted sequence of actions based on a given input. States are connected by transitions. The example below is a state machine for a vending machine. 

![](https://upload.wikimedia.org/wikipedia/commons/6/64/DFA_M%C3%BCnzen.svg)

_Example [Highbrow](https://upload.wikimedia.org/wikipedia/commons/6/64/DFA_M%C3%BCnzen.svg) CC-by-SA._


### Importance in Computer Science

State machines are important in computer science. They can be used to model languages. For example parsers are often depicted as state machines. 

They also have more practical uses as in UML statecharts. 

### Usage in Automaduino

The visual representation of Automaduino is based on state machines. Using sketches we try to determine the behaviour of our Arduino upfront and use this for our visual programming language.

![](/docs/tutorials/blink-drawing.png)

_Example for a sketch based on a automaton_