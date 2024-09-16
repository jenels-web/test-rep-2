
**Lesson 1: Blinking an LED, Turning a Servo, and Using an Ultrasonic Distance sensor.**

**Objective**: This lesson will introduce you to basic electronics and programming concepts using C++. You will learn to control an LED, a servo motor, and an ultrasonic distance sensor.


## **Step 1: Setting Up Tinkercad and Starting a New Project.**

- -Open **Tinkercad** and sign in.

- -Navigate to the "**Circuits**" section.

- -Click **"Create New Circuit**" to start a new project.

- -Add an **Arduino** **board** to the workspace.

- -Add an  **Breadboard** to the workspace.

- -Connect the **5v** to the positive(+) rail on the breadboard.

- -Connect the **GND** to the negative rail (-) on the breadboard.

**Notes:**

- **-Circuits:** A circuit is a path that electricity follows to power things like lights or motors.

- **-Arduino** **board**: An Arduino board is a small computer that can control things like lights or motors using code.

- **-Breadboard**: A breadboard is a tool where you can connect electronic parts together without soldering.

- **-5V**: The 5V pin gives out a small amount of power to run parts like LEDs or sensors.

- **-GND** :stands for Ground. It's where the electricity returns after it has powered something.


## **Step 2: Blinking an LED.**

**Connecting the LED:**

- Drag an **LED** onto the breadboard.

- -Connect **the** **anode (short leg)** of the LED to **GND** on the Arduino.

- -Connect **the** **anode**(long bend one) to a **220Ω** **resistor** then to **digital** **pin** **13** on the Arduino.

**This is what the circuit should look like:**![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXeWmBLN_8S_KTg4heWg7-RjhW91o6edE270drDCBSuL5oVRuDJaX2VUFiyM9_HWZpmFISoSg6vnviwkGuySuY0fOj5JLlZ_wXAVzCcD7nAV264yYNAwu4W98rpIC_7xH0vMaAKGGk-Yfp95uZGdVTwp95T7?key=NdVMCSvukSU4k1azKDEckg)****

**Opening the code editor**:

- Click on code

- Then on block+text

- In the drop down select text and delete everything there.

**Copy this code and add it to the code editor on Tinkercad.**

|                                                                                                                                                                                                                                                                                                                                                  |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Int ledPin = 13;  _// Define pin 13 as the LED pin_ void setup() {   pinMode(ledPin, OUTPUT);  _// Set the LED pin as an output pin_ } void loop() {   digitalWrite(ledPin, HIGH);  _// Turn the LED on_   delay(1000);  _// Wait for one second_   digitalWrite(ledPin, LOW);  _// Turn the LED off_   delay(1000);  _// Wait for one second_ } |

**Code explanation:**

- **int ledPin = 13;** defines the pin number for the LED.

- **pinMode(ledPin, OUTPUT);** sets the pin as an output.

- **-digitalWrite(ledPin, HIGH);** turns the LED on.

- **-delay(1000);** pauses the program for one second.

- **-digitalWrite(ledPin, LOW);** turns the LED off.

<!--EndFragment-->
