# Temperature-Based Fan Speed Controller

This Arduino project reads temperature using an LM35 sensor and controls a 12V DC fan's speed in real time using PWM.  
The system displays the current temperature and fan speed on a 16x2 LCD.

## 📋 Components
- Arduino Uno
- LM35 Temperature Sensor
- 16x2 LCD Display
- 2N2222 NPN Transistor
- 12V DC Fan
- 1N4007 Diode
- 1kΩ Resistor
- Jumper wires

## ⚙️ Working of the Circuit:
Temperature sensor LM35 senses the temperature and converts it into an electrical (analog) signal, which is applied to the ATmega328 microcontroller of the Arduino UNO Board. The analog value is converted into a digital value. Thus the sensed values of the temperature and speed of the fan are displayed on the LCD. When the temperature exceeds 30°C the fan starts rotating.

A low-frequency pulse-width modulation (PWM) signal, whose duty cycle is varied to adjust the fan’s speed is used. An inexpensive, single, small pass transistor-like 2N222 or BD139 can be used here. It is efficient because the pass transistor is used as a switch.

## 📸 Circuit Diagram ans connections
<img width="1099" height="655" alt="Image" src="https://github.com/user-attachments/assets/f8fb3a6a-0d79-427c-9124-f0c9133c7a96" />


Circuit diagram of the Temperature Based Fan Speed Control & Monitoring With Arduino & LM35 is shown above. Arduino is at the heart of the circuit as it controls all functions. LM35 is a precision integrated-circuit whose output voltage is linearly proportional to Celsius (Centigrade) temperature. It is rated to operate over a -55°C to 150°C temperature range. It has +10.0mV/Celsius linear-scale factor.

The 2N2222 transistor acts as a switch and controls the fan speed depending upon temperature. 1N4007 diode controls the fan from being damaged. The LED glows whenever the temperature exceeds 60°C.


<img width="692" height="377" alt="Image" src="https://github.com/user-attachments/assets/e85cd3f6-3255-44a1-ae8c-a1e9a047a1c8" />

---

## 📝 Code Usage
1. Open `main.ino` in Arduino IDE.
2. Upload to Arduino Uno.
3. Wire components as per the circuit diagram.
4. Power the system, monitor readings on LCD.

