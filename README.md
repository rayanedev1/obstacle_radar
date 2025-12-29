# 🛰️ UltraRadar-X180: Advanced Spatial Mapping

<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=00d1d1&height=220&section=header&text=RADAR%20SYSTEM%202025&fontSize=70&animation=fadeIn" width="100%" />
</p>

<p align="center">
  <img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/aqua.png" width="100%" />
</p>

## 📖 Project Overview
The **Radar-X180** is a high-performance obstacle detection system. It bridges the gap between raw hardware signals and meaningful visual data. By combining **Arduino C++** for real-time sensing and **Processing** for graphical rendering, it creates a 180° military-grade sonar interface.

---

## 🎨 2025 Visual Update: Deep Space Background
For this version, the radar background has been updated from standard black to a **Deep Midnight Gradient**. This reduces eye strain and provides a premium "Control Room" aesthetic.



---

## 🔌 Hardware Architecture & Wiring
Based on your technical schematic, here is the precise pin configuration used for this build:

| Component | Arduino Pin | Wire Color (Visual) | Function |
| :--- | :--- | :--- | :--- |
| **Ultrasonic Trig** | `PIN 10` | 🟣 Purple | Trigger Pulse |
| **Ultrasonic Echo** | `PIN 11` | 🔵 Dark Blue | Signal Reception |
| **Servo Signal** | `PIN 12` | 🟣 Purple | PWM Angle Control |
| **Power (VCC)** | `5V` | 🔴 Red | 5V Common Rail |
| **Ground (GND)** | `GND` | 🔵 Blue | Ground Rail |

---

## 🛠️ Development & Engineering Process

### 📡 Phase 1: Hardware Logic (Arduino IDE / C++)
I engineered a high-efficiency firmware focused on low-latency data acquisition:
* **Servo Control:** Precise 0° to 180° sweep patterns using optimized PWM signals.
* **Ultrasonic Pulse:** Distance calculation via the `HY-SRF05` sensor based on speed-of-sound physics.
* **Serialized Streaming:** Formatted data packets `(Angle,Distance.)` streamed via High-Speed Serial UART.

### 🖥️ Phase 2: Software Visualization (Processing)
The GUI was developed to interpret the data stream into a cinematic radar display:
* **Background Rendering:** Custom HEX color `#0A0E14` (Deep Midnight) for a modern 2025 look.
* **Graphics Engine:** Real-time rendering with "phosphor trail" effects for smooth scanning.
* **Spatial Mapping:** Polar coordinate conversion (Angle/Distance) into Cartesian (X/Y) pixels.

---

## 🚀 Execution Guide

1.  **Hardware:** Flash the C++ sketch to your **Arduino Uno**.
2.  **Serial Link:** Keep the USB connected to establish the data bridge.
3.  **Visualizer:** Run the **Processing** sketch to launch the Radar UI.

---

## 👨‍💻 About the Developer
**Rayane_Dev** 🇲🇦
> "Specializing in Hardware-Software interaction and Autonomous Systems."

<p align="center">
  <a href="mailto:rayanedev1@gmail.com">
    <img src="https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Email" />
  </a>
  &nbsp;&nbsp;
  <a href="https://discord.gg/rayaneouf">
    <img src="https://img.shields.io/badge/Discord-7289DA?style=for-the-badge&logo=discord&logoColor=white" alt="Discord" />
  </a>
</p>

---
<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=rect&color=00d1d1&height=30&section=footer" width="100%" />
  <br>
  <i>System Status: ONLINE | UI Theme: Midnight 2025 Edition</i>
</p>
