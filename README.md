# Arduino LED Blink Example

This is a simple Arduino project that demonstrates how to blink an external LED connected to the Arduino Uno board.

## 📷 Circuit Diagram

![LED Blink Circuit](Screenshot%202025-07-10%20183651.png)

## 🔧 Components Used

- Arduino Uno
- Breadboard
- 1 × LED (any color)
- 1 × 220Ω resistor
- Jumper wires
- USB cable for power and programming

## 🔌 Circuit Connections

- **LED Anode (+)** → Digital Pin **13** on Arduino  
- **LED Cathode (-)** → One end of the **resistor**  
- **Other end of resistor** → **GND** on Arduino  

## 💡 Code

```cpp
void setup() {
  // initialize digital pin LED_BUILTIN as an output.
  pinMode(LED_BUILTIN, OUTPUT);
}

// the loop function runs over and over again forever
void loop() {
  digitalWrite(LED_BUILTIN, HIGH);  // turn the LED on (HIGH is the voltage level)
  delay(1000);                      // wait for a second
  digitalWrite(LED_BUILTIN, LOW);   // turn the LED off by making the voltage LOW
  delay(1000);                      // wait for a second
}
