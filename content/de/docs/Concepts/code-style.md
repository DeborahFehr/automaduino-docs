---
title: "Code Stil"
linkTitle: "Code Stil"
weight: 4
description: >
  Verschiedene Code Stile bieten erfahrnenen Benutzern die Möglichkeit auszuwählen wie der von Automaduino generierte Code aussehen soll. 
---

Der Code Stil ermgöglicht es dir verschiedenen Code zu generieren. Das ist für Anfänger weniger interessant, aber erfahrene Programmierer können so beispielsweise kürzeren Code erstellen. Der voreingestellte Stil ist der **Funktionsmodus**. 

### Funktionsmodus
Die Standardeinstellung für den Editor. Dieser Code ist einfach zu lesen und zu bearbeiten. Er ist allerdings länger als im Kurzmodus.

* Alle Zustände erzeugen eine Funktion basierend auf ihrem Namen.
* Um von einem Zustand zum nächsten zu gehen wird die Funktion des nächsten Zustands aufgerufen. 

### Kurzmodus
Der Kurzmodus erzeugt den kürzesten Code aller Stile. Hier wird aller Code innerhalb der Loop Funktion erzeugt. Dieser Stil wird häufig in Tutorials verwendet. Für komplexere Projekte ist dieser Code aber schwerer zu verstehen. 

* Alle Zustände erzeugen nur den notwendigen Arduino Code in der Loop Funktion. 
* Es gibt keine explizite Übergänge - Der Code für den nachfolgenden Zustand folgt direkt. 

### Schaltermodus
Der Schaltermodus kommt einem endlichen Automaten am nächsten. Hier verwenden wir eine Schaltermaschine in der Loop Funktion und setzen eine Zustandsvariable in den Funktionen für die Übergänge. Nach Beendigung der Funktion übernimmt die Loop wieder, wodurch der nächste Zustand ausgeführt wird. Im Vergleich zu den anderen Stilen ist dieser gut zu warten, aber auch schwieriger zu verstehen als der Funktionsmodus. 

* Alle Zustände erzeugen eine Funktion basierend auf ihrem Namen.
* Eine Zustandsvariable ist hinzugefügt die den aktuellen Zustand darstellt.
* Um von einem Zustand zum nächsten zu kommen wird die Zustandsvariable geändert.
* Nach dem Ausführen einer Funktion übernimmt die Loop Funktion wieder und leitet zum nächsten Zustand über.  

### Blink Vergleich

Hier ist der Code für die verschiedenen Stile anhand des [Blink Beispiel](/docs/getting-started/blink/).

{{< tabpane id="2">}}
  {{< tab header="Funktionsmodus" >}}

//Imports:

//Pins:
int pin_0_led = 7;

void setup() { 
pinMode(pin_0_led, OUTPUT);
}

void loop() {
function_0_led();
}

void function_0_led(){
digitalWrite(pin_0_led, HIGH);
delay(1000);
function_1_led();
}

void function_1_led(){
digitalWrite(pin_0_led, LOW);
delay(1000);
function_0_led();
}

  {{< /tab >}}
  {{< tab header="Kurzmodus" >}}

//Imports:

//Pins:
int pin_0_led = 7;

void setup() { 
pinMode(pin_0_led, OUTPUT);
}

void loop() {
while(true){
digitalWrite(pin_0_led, HIGH);
delay(1000);
digitalWrite(pin_0_led, LOW);
}
}

  {{< /tab >}}
  {{< tab header="Schaltermodus" >}}

//Imports:

//Pins:
int pin_0_led = 7;

int state = 0;
void setup() { 
pinMode(pin_0_led, OUTPUT);
}

void loop() {
switch(state){
case 0:
function_0_led();
break;
case 1:
function_1_led();
break;
default:
break;
}
}

void function_0_led(){
digitalWrite(pin_0_led, HIGH);
delay(1000);
state = 1;
}

void function_1_led(){
digitalWrite(pin_0_led, LOW);
delay(1000);
state = 0;
}

  {{< /tab >}}
{{< /tabpane >}}