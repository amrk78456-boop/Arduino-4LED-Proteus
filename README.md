# Arduino 4-LED Blinking Simulation

A simple embedded systems project using an **Arduino Uno** to control 4 LEDs simultaneously (blinking synchronously with a 1-second delay). The circuit schematic and components are fully simulated using **Proteus**.

## 🛠️ Components Used
* Arduino Uno Board
* 4x LEDs (Red, Yellow, Green, Blue)
* 4x Resistors (220 Ohm)
* Ground (GND) Connection

## 📂 Repository Contents
* `led_copy_20260624160803.ino`: The official Arduino C++ source code.
* `New Project.pdsprj`: The Proteus simulation schematic file.
* `led.ino.hex`: The compiled machine code required by Proteus to run the simulation.

## 💻 Arduino Code
```cpp
int ledRed = 12;    
int ledYellow = 11; 
int ledGreen = 10;  
int ledBlue = 9; // Assuming pin 9 for the 4th LED

void setup() 
{
  pinMode(ledRed, OUTPUT);
  pinMode(ledYellow, OUTPUT);
  pinMode(ledGreen, OUTPUT);
  pinMode(ledBlue, OUTPUT);
}

void loop() 
{
  digitalWrite(ledRed, HIGH);
  digitalWrite(ledYellow, HIGH);
  digitalWrite(ledGreen, HIGH);
  digitalWrite(ledBlue, HIGH);
  delay(1000); 

  digitalWrite(ledRed, LOW);
  digitalWrite(ledYellow, LOW);
  digitalWrite(ledGreen, LOW);
  digitalWrite(ledBlue, LOW);
  delay(1000); 
}
