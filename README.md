<div align="center">

```
╔══════════════════════════════════════════════════════════════╗
║         MANTHAN KADAM  ·  EMBEDDED HARDWARE ENGINEER        ║
║      Circuits that think. Boards that last. Systems that     ║
║                     connect the real world.                  ║
╚══════════════════════════════════════════════════════════════╝
```

[![Email](https://img.shields.io/badge/manthankad0605@gmail.com-EA4335?style=flat-square&logo=gmail&logoColor=white)](mailto:manthankad0605@gmail.com)
[![Location](https://img.shields.io/badge/Mumbai%2C%20India-0078D4?style=flat-square&logo=googlemaps&logoColor=white)]()
[![Phone](https://img.shields.io/badge/+91%208087652098-25D366?style=flat-square&logo=whatsapp&logoColor=white)]()

</div>

---

## 👨‍💻 About Me

Electronics hardware engineer with **6+ years of end-to-end experience** designing embedded and electromechanical systems — from blank schematic to validated product. I work across the full hardware lifecycle: requirements, architecture, circuit design, multilayer PCB layout, bring-up, validation, and production readiness.

My focus areas include **power electronics, audio systems, industrial automation, and wireless-connected embedded platforms**. I take pride in clean schematic practices, EMI-aware layout, and building hardware that actually works in the field.

> *"Good hardware is invisible — it just works."*

---

## 🛠️ Technical Stack

### EDA & Design Tools
![Altium](https://img.shields.io/badge/Altium%20Designer-A5915F?style=flat-square&logo=altiumdesigner&logoColor=white)
![KiCad](https://img.shields.io/badge/KiCad-314CB0?style=flat-square&logo=kicad&logoColor=white)
![EasyEDA](https://img.shields.io/badge/EasyEDA-1565C0?style=flat-square)

### Embedded Platforms
![STM32](https://img.shields.io/badge/STM32-03234B?style=flat-square&logo=stmicroelectronics&logoColor=white)
![ESP32](https://img.shields.io/badge/ESP32-E7352C?style=flat-square&logo=espressif&logoColor=white)
![Raspberry Pi](https://img.shields.io/badge/Raspberry%20Pi-A22846?style=flat-square&logo=raspberrypi&logoColor=white)
![Radxa](https://img.shields.io/badge/Radxa%20%2F%20Rockchip-333333?style=flat-square)
![Arduino](https://img.shields.io/badge/Arduino%20Opta-00979D?style=flat-square&logo=arduino&logoColor=white)

### Communication Protocols
![I2C](https://img.shields.io/badge/I2C-555555?style=flat-square)
![SPI](https://img.shields.io/badge/SPI-555555?style=flat-square)
![UART](https://img.shields.io/badge/UART-555555?style=flat-square)
![I2S](https://img.shields.io/badge/I2S-555555?style=flat-square)
![Modbus](https://img.shields.io/badge/Modbus%20RS485-555555?style=flat-square)
![TCP/IP](https://img.shields.io/badge/TCP%2FIP-555555?style=flat-square)
![BLE](https://img.shields.io/badge/BLE-0082FC?style=flat-square&logo=bluetooth&logoColor=white)
![WiFi](https://img.shields.io/badge/WiFi%20Mesh-00ADEF?style=flat-square&logo=wifi&logoColor=white)

### Hardware Disciplines
- Multilayer PCB Layout (up to 4 layers, high-density)
- Analog & Digital Circuit Design
- Power Supply Design (Buck, Boost, Linear)
- EMI/EMC Design & Compliance
- Signal Integrity & Power Integrity
- DFM / DFT / DFS
- Board Bring-up & Root Cause Analysis
- Sensor Integration & Peripheral Interfacing

---

## 🔧 Featured Projects

---

### 🔊 Wireless Multi-Room Audio System
> *ESP32 Dual-Node · BLE + WiFi Mesh · NAU88C22 Codec · TPA3118 Class-D Amp*

A fully custom, wireless-connected audio distribution system designed for large open spaces like lawns and outdoor venues. The system uses **BLE proximity detection** — as a user roams, the nearest speaker node automatically connects. All nodes synchronize playback over a **WiFi mesh network**, delivering coherent, latency-managed audio across the entire space.

**Hardware highlights:**
- Dual **ESP32-WROVER-IE** architecture (one master, one slave per node) coordinating BLE and mesh over WiFi
- **NAU88C22YG** audio codec with full I2S interface, I2C control, microphone and line inputs
- **TPA3118 Class-D stereo amplifier** with LC output filters, bootstrap caps, and configurable gain/mode
- AC 12V input → full-bridge rectifier (S2M diodes) → **LMR51420 buck converter** to 3.3V for all digital logic
- High-density **4-layer PCB** designed in EasyEDA with careful EMI partitioning between power, analog audio, and RF sections
- Solder-bridge configuration pads for master/slave selection without hardware redesign

**What it does:** Place nodes anywhere outdoors. A phone connects over BLE to the nearest device. Audio streams over WiFi mesh to all synchronized nodes. Zero per-node app pairing required.

---

### ⚡ High-Voltage Capacitor Discharge System (H-Bridge MOSFET)
> *High-Power · H-Bridge Topology · Capacitor Charge & Discharge Control*

Designed a high-voltage discharge circuit using an **H-bridge MOSFET topology** for controlled capacitor charging and rapid, precision discharge. Built to handle the thermal, switching, and gate-drive demands of high-current transient events. Includes protection circuitry for shoot-through prevention and safe energy dissipation.

**Key design considerations:** Gate timing, dead-band control, snubber design, and thermal management under high di/dt conditions.

---

### 💧 Water Purification Control Box
> *STM32 / ESP · pH Sensor · ORP Sensor · Level Switches · Stage Automation*

An embedded control system for automated water purification. The system continuously monitors **water quality via pH and ORP sensors**, detects tank levels using digital float switches, and automatically triggers or halts purification stages based on sensor thresholds. Designed for reliability in a wet, industrial-adjacent environment.

**Features:** Multi-stage process logic, sensor fault detection, relay-driven actuator control, and status indication.

---

### 🤿 Underwater Video & Sensor Data Logger
> *Raspberry Pi Zero 2W HAT · IMU · Pressure Sensor · Battery Management · USB Camera*

A custom **RPi Zero 2W HAT** designed for diver-worn underwater monitoring. The board integrates an **IMU (inertial measurement unit)**, **depth/pressure sensor**, **battery voltage monitor**, and **USB camera interface** for simultaneous video capture and telemetry logging. Designed for operation in a sealed, pressure-rated housing.

**Challenges solved:** Power budgeting for battery-only operation, I2C/SPI sensor stack on a compact HAT form factor, thermal management without active cooling.

---

### ⌨️ Linguistic OLED Keyboard System
> *SPI · OLED Displays · Embedded UI · Multi-Language Input*

A custom embedded keyboard where each key features an **SPI-driven OLED screen** that dynamically updates its displayed character based on the currently selected language/input mode. Designed for applications requiring multi-script input on embedded hardware without a connected display host.

**Design detail:** SPI bus management across multiple slave OLED displays, UI state machine in firmware, character map switching logic.

---

### 💡 Medical-Grade Adjustable Headlamp
> *LED Optics · 3-Mode PWM Control · Fixed Beam Specification*

Designed a headlamp for medical use with a precise optical requirement: **600 lumens, 12-inch diameter spot at 60 cm** working distance. Implemented **3-mode brightness control via PWM** with carefully calculated thermal and optical design to maintain consistent color temperature and beam geometry across all modes.

**Constraints met:** Fixed spot size regardless of mode, flicker-free output for clinical environments, compact and wearable form factor.

---

### 🌐 Modbus-to-Cloud Ethernet Gateway
> *RS485 Modbus · Ethernet · JSON · 15-Second Telemetry Cycle*

An industrial IoT bridge that **listens on Modbus RS485**, parses register data, and transmits structured **JSON payloads to the cloud over Ethernet** every 15 seconds. Designed for retrofitting legacy industrial equipment into modern monitoring infrastructure without modifying the source devices.

**Protocol stack:** Modbus RTU → parsing layer → JSON serialization → HTTP/MQTT over Ethernet.

---

### 🧊 Nugget Ice Dispenser Controller
> *Sensor-Actuated · Electromechanical Control · Relay Logic*

Embedded controller for an automated nugget ice dispenser. Detects dispense actuation via sensor input and drives the electromechanical system through a controlled sequence — motor start, dispense cycle, stop, and reset. Includes debounce logic, timeout protection, and fault indication.

---

### 📱 Yoga Enthusiast Mobile Device
> *Allwinner A133 SoM · Custom Android/Linux Hardware Platform*

Designed a custom handheld device built around the **Allwinner A133 System-on-Module** — a quad-core ARM Cortex-A53 platform. The device targets yoga practitioners with a specialized software experience on custom hardware, including display interface, touch input, audio, battery management, and connectivity.

**Hardware scope:** SoM integration, peripheral interfacing, power management tree, PCB layout for a mobile form factor.

---

### 🔆 ESP32 PWM LED Driver
> *ESP32 · LEDC PWM · Multi-Channel Dimming*

Compact ESP32-based multi-channel LED driver using the onboard **LEDC (LED Control) PWM peripheral**. Supports independent brightness control per channel with smooth dimming curves. Designed as a lightweight, Wi-Fi-capable lighting controller.

---

## 📋 Professional Experience

| Period | Role | Company |
|--------|------|---------|
| Feb 2025 – Present | Embedded Hardware Engineer | Ultimate Design LLP, Navi Mumbai |
| May 2024 – Feb 2025 | Embedded Engineer | Augmatic Technologies Pvt. Ltd., Vadodara |
| Oct 2023 – Apr 2024 | Jr. Electronics Engineer | SinAxis Enterprises Pvt. Ltd., Mumbai |
| Aug 2021 – Sep 2023 | Electronic Technician II | Jabil Circuits India Pvt. Ltd., Pune |

---

## 🎓 Education & Certifications

- **B.E. — Electronics & Telecommunication** · Rajendra Mane College of Engineering & Technology, Ratnagiri (2020)
- **PG Diploma — Embedded Systems & PCB Design** · National Institute for Technical Training & Skill Development (2020)

---

## 📊 GitHub Stats

<div align="center">

![GitHub Stats](https://github-readme-stats.vercel.app/api?username=YOUR_USERNAME&show_icons=true&theme=dark&hide_border=true&bg_color=0d1117&title_color=58a6ff&icon_color=58a6ff)

![Top Languages](https://github-readme-stats.vercel.app/api/top-langs/?username=YOUR_USERNAME&layout=compact&theme=dark&hide_border=true&bg_color=0d1117&title_color=58a6ff)

</div>

---

<div align="center">

*Open to freelance PCB design, hardware consulting, and embedded systems projects.*

**📧 manthankad0605@gmail.com · 📞 +91 8087652098 · Mumbai, India**

</div>
