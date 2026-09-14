Gesture-Controlled Robotic Arm 🤖

📌 Overview

This project implements a real-time **gesture-controlled robotic arm** using **Bluetooth and Arduino**. Hand gestures captured through a Flex Sensors are processed using **Accelerometer Sensor**, then translated into servo motor movements through an **Arduino**.

The system demonstrates **Human-Computer Interaction (HCI)** by enabling intuitive, touchless control of robotic hardware.

---

🎯 Problem Statement

Traditional robotic arm control systems often rely on physical interfaces such as joysticks, switches, or buttons. These methods can be restrictive, unintuitive, and less interactive for modern automation needs.

This project aims to:

- Enable **contactless control**
- Improve **ease of use**
- Demonstrate **Bluetooth + hardware integration**

---

🧠 System Architecture

```text

Gesture Sensor / Glove → Data Acquisition (Flex / IMU / Potentiometers)
        ↓
   Microcontroller (Transmitter)
        ↓ (Processed angles / codes)
    Bluetooth Module (TX)
        ↓  ~~~ Wireless Link (Bluetooth) ~~~  ↓
    Bluetooth Module (RX)
        ↓
   Microcontroller (Receiver / Robot Controller)
        ↓
   Servo & Stepper Motor Drivers → Robotic Arm Joints & Gripper


```
🚀 Features

- Real-time gesture recognition
- Low-latency communication
- Modular design with separate vision and control layers
- Easy integration with Arduino-based robotic systems
- Scalable for advanced robotics applications

---


📂 Project Structure

```text
Gesture-Controlled-Robotic-Arm/
│
├── README.md
├── LICENSE
├── .gitignore
│
├── src/
│   ├── transmitter/
│   │   └── transmitter.ino
│   │
│   ├── receiver/
│   │   └── receiver.ino
│   │
│   └── config/
│       └── pins.h
│
├── hardware/
│   ├── components.md
│   ├── circuit_diagram.png
│   └── wiring_diagram.png
│
├── docs/
│   ├── block_diagram.png
│   ├── system_architecture.png
│   └── project_report.pdf
│
├── algorithms/
│   ├── gesture_recognition.md
│   ├── motion_control.md
│   └── smooth_motion.md
│
├── testing/
│   └── test_results.md
│
├── media/
│   ├── images/
│   └── demo.gif
│
└── future_scope/
    └── future_improvements.md
```

---

🔮 Future Improvements

- Machine Learning-based gesture classification
- Wireless control using Bluetooth or WiFi
- Multi-hand gesture support
- Object gripping automation
- Error handling and motion smoothing

---

🧪 Applications

This project can be extended for use in:

- Assistive robotics
- Industrial automation
- Smart interfaces
- Human-computer interaction research
- Touchless robotic control systems

---

🧾 Conclusion

This project highlights the integration of **AI, computer vision, and embedded systems** to build an intuitive robotic control system. It serves as a foundation for future work in **automation**, **Assistive robotics**, and **Smart Human-Machine Interfaces**.

---

👨‍💻 Author

**N Avanish Reddy and Team**

If you found this project useful, consider starring the repository.
