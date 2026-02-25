# Low-Cost-Lamp-Manufacturing-Fault-Detection-System
Low-Cost Lamp Manufacturing Fault Detection System

This project is a 12V lamp current verification circuit designed to detect whether a lamp correctly consumes its rated current (0.11A).
The system uses:
A serie resistor network (6 × 1Ω resistors)
Ohm’s Law (V = I × R)
An NPN transistor as a switching comparator
An indicator LED for pass/fail detection
How It Works
The lamp under test is connected in series with multiple low-value resistors.
If the lamp draws 0.11A, the total voltage across 6Ω becomes:
V=0.11×6=0.66V
This voltage is sufficient to turn ON the transistor (V_BE ≈ 0.6–0.7V), activating the indicator LED.
If the lamp draws less than 0.11A (defective or incorrect manufacturing), the voltage drop is lower than 0.6V, and the transistor remains OFF.
The resistor power dissipation is safely within limits:
0.11 * 0.11* 6 = 0.07WATT
Each 0.25W resistor operates safely.
Use cases:
Manufacturing Quality Control
Automotive Lighting Testing

<img width="1090" height="878" alt="image" src="https://github.com/user-attachments/assets/84992f60-3350-4a98-b604-54555622210a" />

Here the lamp if it uses 0.11A and there is only 5 resistors
So the voltage in transistor will be 0.11 * 5 = 0.55V not enough to turn it on
So if we put 6 resistors and the the led D1 doesn’t turn on the that mean the transistors doesn’t turned on so the lamp is not really consuming 0.11
Lets try it

<img width="1090" height="890" alt="image" src="https://github.com/user-attachments/assets/8c961ac8-c8b3-4a23-8786-46d80b50d6dd" />

Now the lamp turn on because 0.11 * 6 = 0.66 enough to turn on the transistor
So the lamp is consuming 0.11A
The resistor have .25 Watt power consumption
So the power is 0.11 * 0.11 * 6 = 0.07 WATTT
Each resistor uses 0.07 watt so no problem

<img width="1090" height="1937" alt="image" src="https://github.com/user-attachments/assets/02b9c065-38c6-4e77-aa4c-bbd3675dbf77" />
