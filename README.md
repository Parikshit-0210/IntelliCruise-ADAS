# IntelliCruise - Advanced Driver Assistance System (ADAS) - Practical Model

## Overview

This project, **IntelliCruise**, is a working model of an **Advanced Driver Assistance System (ADAS)**, designed to enhance vehicle safety by detecting obstacles and providing alerts. It utilizes various sensors and actuators interfaced with an Arduino Uno to simulate an intelligent vehicle assistance system.

## Features

- Obstacle detection using **ultrasonic sensors** and **IR sensors**
- Motor control for vehicle movement using **L298N motor driver** and **gear motors**
- Speed control using **IR remote and IR receiver sensor**
- Automatic speed adjustment using **mathematical calculations**
- Real-time comparison of **wheel speed and sonar speed** for adaptive braking and acceleration
- Audio alert system using a **buzzer**
- Data processing and control logic handled by **Arduino Uno**
- Power supplied through a **battery unit**

## Components Used

### 1. L298N Motor Driver

- Dual H-Bridge motor driver module
- Controls the **gear motors** to drive the vehicle forward, backward, left, and right
- Handles voltage regulation for motors

### 2. Gear Motor

- Provides mechanical movement to the vehicle
- Speed and direction controlled via L298N motor driver

### 3. Ultrasonic Sensors

- Used for **distance measurement**
- Helps detect obstacles in front of the vehicle
- Sends signals to the Arduino for decision-making

### 4. Buzzer

- Produces an audio alert when an obstacle is detected
- Warns about potential collisions

### 5. Breadboard

- Serves as a temporary circuit prototyping platform
- Allows connections between components without soldering

### 6. Arduino Uno

- The **brain** of the system
- Processes sensor data and controls motor operations
- Runs the coded logic for obstacle avoidance

### 7. Power Supply (Battery)

- Provides electrical energy to power the entire system
- Ensures smooth operation of sensors, motors, and Arduino

### 8. Jumper Wires

- Used for making electrical connections between components on the breadboard and Arduino

### 9. Connecting Wires

- Additional wires used for robust connections between the modules

### 10. IR Sensor

- Detects nearby objects based on infrared reflection
- Used for short-range obstacle detection

### 11. Receiving Sensor

- Works alongside IR sensors to identify signals and provide input to the system
- Helps in detecting environmental factors for decision-making

### 12. IR Receiver Sensor

- Receives signals from an **IR remote**
- Used for controlling the speed of the vehicle

### 13. IR Remote

- Used to manually adjust the speed of the vehicle
- Sends signals to the **IR receiver sensor** to increase or decrease speed

## Working of IntelliCruise

1. The **ultrasonic and IR sensors** continuously scan the surroundings.
2. If an obstacle is detected within a critical distance, the **Arduino** processes the data and takes action.
3. The **L298N motor driver** either stops or reroutes the vehicle to avoid collisions.
4. The **buzzer** sounds an alert when an object is detected too close.
5. The **IR remote and receiver sensor** allow manual control over speed.
6. **Mathematical calculations** such as **displacement, speed, and deceleration rates** help in automatically adjusting the speed based on real-time sensor data.
7. Wheel Speed and Sonar Speed Calculation:
   - Sonar speed is calculated using ultrasonic sensor readings over time.
   - Wheel speed is detected through revolution tracking.
   - Both speeds are compared in real-time to dynamically adjust the vehicle speed.
8. The system compares **wheel speed and sonar speed**:
   - If **wheel speed > sonar speed**, the vehicle reduces speed to prevent sudden collisions.
   - If **wheel speed ≤ sonar speed**, the vehicle comes to a stop.
   - If **sonar speed < 0**, the system increases speed gradually to maintain smooth operation.
9. The system remains powered through the **battery pack**, allowing wireless operation.

## How to use

1. Connect all components.
2. Upload the **IntelliCruise\_CODE.ino** file to the Arduino Uno.
3. Power up the system and observe obstacle detection in action.
4. Control the speed manually using the **IR remote** or allow automatic speed adjustment based on **sensor inputs**.
5. The vehicle should respond dynamically to obstacles and provide alerts.

## Future Enhancements

- Adding **GPS and GSM modules** for location tracking and remote alerts.
- Implementing **AI-based decision-making** for better obstacle avoidance.
- Integrating **camera-based object detection** for enhanced recognition.
- Advanced **speed control algorithms** using machine learning.

## Contribution

We welcome contributions to improve this project. To contribute:

- Fork this repository.
- Make necessary changes and improvements.
- Submit a pull request with a description of the changes.

## Raise Issues

If you encounter any errors or have suggestions for improvements, please raise an issue in the repository. We will try to resolve them as soon as possible.

## Contact Us

For any queries or collaboration opportunities, feel free to reach out.

Email: [parikshitvel0210\@gmail.com]

---

**IntelliCruise** is a cutting-edge **ADAS model**, providing a hands-on approach to understanding **autonomous vehicle systems** and **embedded system applications**.

