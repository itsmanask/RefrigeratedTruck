# 🚛❄️ Microcontroller-Based Temperature Control & Monitoring System for Refrigerated Trucks ❄️🚛

An intelligent, embedded system designed to maintain and monitor temperature in refrigerated transport vehicles — combining real-time temperature sensing, adaptive cooling, predictive control, and power optimization.

---

## 📌 Overview

This project implements a microcontroller-based system that keeps the internal temperature of a refrigerated truck near 10°C using:

- 🔍 **Real-time monitoring** (LM35 temperature sensor)
- ❄️ **Peltier module with PWM-based cooling**
- 🌬️ **DC fans for heat dissipation**
- 🔊 **Buzzer alerts for overheat**
- 🖥️ **OLED display for visual feedback**
- ⚡ **Preemptive & adaptive control logic for efficiency**

---

## 🔧 Hardware Components

| Component              | Quantity | Description                            |
|------------------------|----------|----------------------------------------|
| ATmega328P             | 1        | Microcontroller unit                   |
| LM35 Temperature Sensor| 1        | Analog temperature sensor              |
| SSD1306 OLED Display   | 1        | I2C 0.96" display                      |
| TEC1-12706 Peltier     | 1        | Thermoelectric cooling module          |
| L293D Motor Driver     | 1        | Dual motor driver for fans             |
| DC Fan (12V)           | 2        | For air circulation                    |
| Buzzer                 | 1        | Audio alert for over-temperature       |
| LM7805 Voltage Regulator| 1       | 5V regulated output                    |
| Custom PCB             | 1        | Designed using EasyEDA                 |
| 12V Power Supply       | 1        | External DC power source               |

---

## 🧠 Features

- ⚙️ **Adaptive Peltier Control**  
  Linearly scaled PWM based on real-time temperature (10°C–18°C).

- 🧊 **Preemptive Cooling Activation**  
  Starts cooling early if a rapid temperature rise is detected.

- 💡 **OLED Auto-Sleep**  
  Powers down display during stable temperature to conserve energy.

- 📢 **Overheat Alert**  
  Buzzer warns if temperature exceeds safe limits (above 11°C).

- 📟 **Live Display**  
  OLED shows temperature, fan speed, and Peltier duty cycle.

---


---

## 🧪 How It Works

1. System reads current temperature using **LM35**.
2. Calculates temperature trend to **predict rise**.
3. Activates fan and Peltier module based on:
   - **Current temperature**
   - **Rate of change**
4. Displays live data on OLED (unless temp is stable).
5. Alerts user with buzzer if above 11°C.

Demo Video: https://www.youtube.com/watch?v=KpXQiDIcKAY

---

## 📝 Documentation

- 📄 Research Paper PDF
- 📦 Patent Proposal Draft

---

## 👨‍💻 Contributors

- Rajlakshmi Desai  
- Samiksha Nalawade  
- Dhanshree Biradar  
- Manas Kulkarni  

👨‍🏫 **Mentor:** Dr. Pravin G. Gawande

---

## 📜 License

This project is intended for academic and research purposes. For commercial use or patent-related queries, please contact the authors.

---

## 🔗 Related Tags

`#EmbeddedSystems` `#ColdChainLogistics` `#TemperatureControl` `#ATmega328P` `#IoT` `#PeltierCooling` `#SmartLogistics` `#PCBDesign`

---


