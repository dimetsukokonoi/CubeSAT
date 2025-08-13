# CubeSat Project

## Overview

This CubeSat project is a compact, functional prototype of a satellite system built within the volume and shape of a standard cube. Using an ESP32 microcontroller combined with multiple sensors, it collects and transmits environmental and positional data during flight, demonstrating core concepts of aerospace telemetry and embedded systems.

The primary objectives of this project are to design, build, and deploy a cost-effective CanSat capable of capturing atmospheric pressure, temperature, acceleration, orientation, magnetic field, and GPS position data. This project showcases skills in hardware integration, embedded programming, sensor data acquisition, and real-time telemetry.

---

## Hardware Components

- **Microcontroller:** ESP32  
- **Sensors:**  
  - BMP280 (Pressure & Temperature)  
  - MPU6500 (Accelerometer & Gyroscope)  
  - QMC5883L Magnetometer  
  - GPS Module  

All components are integrated using I2C and serial communication protocols, powered by a lightweight battery suitable for flight.

---

## Features

- Real-time sensor data acquisition and logging  
- Altitude and temperature measurement via BMP280  
- Motion tracking using MPU6500 accelerometer and gyroscope  
- Orientation detection using a magnetometer  
- GPS-based position tracking  
- Data transmission and onboard storage for post-flight analysis  

---

## Firmware

The firmware is developed using the Arduino framework targeting the ESP32. It features modular sensor drivers located in the `/firmware/sensors/` directory, facilitating easy maintenance and upgrades.

The main program (`main.ino`) initializes all peripherals, performs sensor readings at regular intervals, and manages data logging and telemetry output.

---

## Flight Data

Sample telemetry data from test flights is stored in the `/data/sample_telemetry.csv` file. Visualizations such as altitude and temperature charts are available in the `/data/graphs/` directory.

---

## Usage

1. Connect the hardware as per the wiring diagram in `/hardware/wiring_diagram.png`.  
2. Flash the firmware located in `/firmware/main.ino` using the Arduino IDE or compatible tools.  
3. Power the CubeSat and monitor data output via serial or onboard logging.  
4. Analyze flight data using the sample CSV files and graphs provided by the sensors. 

---

## Project Status

The CubeSat prototype has completed multiple flight tests with stable sensor readings and reliable telemetry transmission. Ongoing work includes optimizing power consumption and improving GPS fix accuracy under varying flight conditions. Gradually improving the repository—more updates coming soon!
---

## Contributors

- Mujtahidul Hasan Sami (me)
- Gazi Salahuddin Abtahi
- Samin Yasar
- Shadman Mohammad Shah
- Nayeem Hasan
- Tahmid Ferdous

---

## Contact

For questions or collaboration, please contact: mujtahidulhasansami@gmail.com
