# 🚀 Final Year Drone Project

## 📌 Project Description
This project is a custom-built **quadcopter drone** designed for **autonomous flight, manual control, and aerial surveillance**. It integrates the **Pixhawk PX4 flight controller**, **GPS**, and real-time sensor feedback for efficient navigation and stability. The drone can be manually controlled via an **RC transmitter** or programmed for **autonomous missions** using Mission Planner.

## 🔧 Components & Specifications

### **🛠 Frame & Power System**
- **Frame**: Q450 Quadcopter Frame – PCB Version with Integrated PCB
  - Material: Glass fiber + Polyamide-nylon
  - Frame Weight: 280g
  - Pre-threaded brass sleeves for easy assembly
  
- **Motors**: 
  - 2 x **EMAX MT2213 935KV BLDC Motor CCW**
  - 2 x **EMAX MT2213 935KV BLDC Motor CW**
  - Thrust: 860g per motor
  - Compatible with 8"-10" propellers
  
- **ESCs (Electronic Speed Controllers)**: 
  - 4 x **Emax BLHeli Series 30A ESC with Oneshot**
  - Continuous Current: 30A, Burst Current: 40A (10 sec)
  
- **Battery**: Orange 5200mAh 3S 40C/80C Lithium Polymer (LiPo)
  - Voltage: 11.1V, Max Burst Discharge: 80C (416A)
  
### **⚙️ Flight Controller & Navigation**
- **Flight Controller**: Pixhawk PX4 Autopilot PIX 2.4.8
  - Processor: 32-bit STM32F427 Cortex M4
  - Sensors: Accelerometer, Gyroscope, Magnetometer, Barometer
  - Interfaces: 5x UART, 2x CAN, PWM Inputs, RSSI Support
  
- **GPS Module**: Ublox NEO-M8N High Precision GPS with Compass
  - Navigation update rate: Up to 10Hz
  - Position Accuracy: 2.0m CEP
  - Satellite Support: GPS, GLONASS, BeiDou, Galileo
  
- **RC Transmitter & Receiver**: Flysky FS-i6X 2.4GHz 10CH with FS-iA10B Receiver
  - RF Range: 2.408-2.475GHz
  - Channels: 6-10 (Default 6)
  - Stick Resolution: 4096

### **🔌 Additional Components**
- **XT60 Connectors & Wiring**
- **GPS Folding Antenna Base Set**
- **Lipo Voltage Checker 1-8S**
- **15CM 22AWG Servo Lead Extension Cables**

## ⚙️ Working Principle
1. **Flight Control & Stabilization**: 
   - The **Pixhawk PX4** processes sensor data (gyroscope, accelerometer, barometer) to maintain flight stability.
   
2. **Navigation & GPS-Based Autonomous Flight**:
   - The **Ublox NEO-M8N GPS module** enables precise navigation and waypoint-based autonomous missions.
   
3. **Manual Control & RC Operation**:
   - The **Flysky FS-i6X transmitter** allows manual flight control.
   
4. **Power Management & Motor Control**:
   - The **LiPo battery** powers the motors via **ESCs**, which regulate speed and stability.
   
5. **Telemetry & Data Transmission**:
   - Real-time flight data can be viewed in **Mission Planner** using a telemetry module.
   
6. **Failsafe & Auto Return to Home (RTH)**:
   - If signal loss occurs, the drone can **automatically return to home** using GPS.

## 🛠️ How to Set Up & Configure
### **1️⃣ Hardware Assembly**
- Mount the **Pixhawk PX4 Flight Controller** securely to the Q450 frame.
- Attach **motors, ESCs, and propellers** to the frame.
- Connect the **battery, power distribution board, and ESCs**.
- Install the **GPS module and antenna**.

### **2️⃣ Software Configuration**
- Install **Mission Planner (Windows/Linux/Mac)**.
- Connect the **Pixhawk PX4** via USB and configure:
  - **ESC calibration**
  - **Accelerometer & Gyroscope calibration**
  - **GPS configuration**
  - **Flight modes (Stabilize, Loiter, Auto, RTL, etc.)**
  
### **3️⃣ First Flight Test**
- Perform a manual test flight using the **Flysky FS-i6X transmitter**.
- Check **stabilization, responsiveness, and GPS lock**.
- Enable **waypoint navigation** for an autonomous test.

## 📷 Images & Videos
(Add images or video links showing the drone in action.)

## 💡 Future Improvements
- **Obstacle Avoidance** using LiDAR/Sonar
- **FPV (First-Person View) Camera for live streaming**
- **AI-Based Object Tracking using Raspberry Pi/Jetson Nano**

## 📜 License
This project is open-source under the **MIT License**.

---

📌 **Contributions & Feedback:** Feel free to contribute by submitting issues, pull requests, or improvements!
