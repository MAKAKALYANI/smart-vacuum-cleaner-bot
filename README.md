# smart-vacuum-cleaner-bot
# 🤖 Smart Vacuum Cleaner

An autonomous Arduino-based robotic vacuum cleaner that detects obstacles, avoids collisions, and cleans surfaces without human intervention — using sensors, a fan-powered suction system, and DC motor-controlled movement.

---

## 🧠 Abstract

In today’s fast-paced lifestyle, keeping our environment clean without manual labor has become essential. The Smart Vacuum Cleaner project is designed to work without human involvement, powered by an Arduino UNO, ultrasonic sensors for obstacle detection, IR sensors for line following, and a CPU fan for vacuum suction. The robot can autonomously navigate around furniture and walls, making cleaning efficient and contact-free.

---

## 🚩 Problem Statement

Cleaning large spaces requires time, effort, and often multiple people. In places such as colleges or during health-sensitive times like the COVID-19 pandemic, manual cleaning becomes impractical. Dust accumulation can cause health issues including allergies and respiratory problems.

---

## 🎯 Objective

To develop a smart robotic vacuum cleaner that:
- Detects and avoids obstacles using ultrasonic sensors
- Moves along a defined path using IR sensors
- Vacuums dust using a CPU fan and bottle-based suction
- Operates completely autonomously without manual control

---

## 🛠️ Hardware Components Used

| Component              | Description                                 |
|------------------------|---------------------------------------------|
| Arduino UNO            | Microcontroller to control logic            |
| Ultrasonic Sensor      | Measures distance to detect obstacles       |
| IR Sensors             | Detect lines or path to follow              |
| DC Motors              | Drives the wheels of the robot              |
| Motor Driver Shield    | Controls motor direction and speed          |
| CPU Fan                | Creates suction for vacuum                  |
| Battery (9V)           | Powers the system                           |
| Chassis + Wheels       | Physical movement and support               |

📄 Full list in [`components_list`](components_list)

---

## 🔧 Working Principle

- The robot moves forward using DC motors.
- If an obstacle is detected within 20 cm by the ultrasonic sensor:
  - It stops and reverses for 1 second.
  - Turns left, measures distance.
  - Turns right, measures distance.
  - Moves in the direction with the most clearance.
- While moving, the CPU fan creates vacuum suction through a pipe to clean surfaces.
- IR sensors can optionally guide the bot along a defined path.

---

## 💡 Use Cases

- Homes and apartments
- College classrooms and labs
- Small offices or warehouses
- Dangerous or hard-to-reach areas



