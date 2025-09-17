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

## ⚙️ How It Works
- The LM35 outputs an analog signal proportional to temperature.
- Arduino reads analog input, computes temperature, and adjusts fan speed.
- Fan speed and temperature are displayed on LCD.
- An LED lights up if temperature exceeds maximum threshold.

## 📝 Code Usage
1. Open `fan_speed_control.ino` in Arduino IDE.
2. Upload to Arduino Uno.
3. Wire components as per the circuit diagram.
4. Power the system, monitor readings on LCD.

## 📸 Circuit Diagram
(Include your circuit diagram image here)

---

MIT License
