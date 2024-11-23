# Med Preserve Project - IoT Dashboard with Data Control

This repository contains the code and documentation for the **Med Preserve Project**. The system is designed for IoT-based real-time environmental monitoring and control. It integrates Arduino hardware with a .NET Core-based Windows application to provide a robust solution for temperature and humidity management.

## Table of Contents
1. [Features](#features)
2. [System Architecture](#system-architecture)
3. [Setup Instructions](#setup-instructions)
4. [Hardware Configuration](#hardware-configuration)
5. [Software Features](#software-features)
6. [Contributing](#contributing)
7. [License](#license)

## Features
- **IoT-Based Monitoring:** Real-time data collection using Arduino Mega and sensors.
- **Windows Application:** Manages users, devices, and configuration settings.
- **Automated Control:** Relays triggered to maintain environmental thresholds.
- **Data Logging:** Historical data storage and live visualization using graphs.

## System Architecture
1. **Hardware:**
   - Sensors: DHT11, DS3231.
   - Controllers: Arduino Mega.
   - Actuators: 8-channel relay controlling temperature and humidity mechanisms.
   - Storage: Micro SD for offline configuration persistence.

2. **Software:**
   - **Backend:** .NET Core 6.0 application with SQL Server.
   - **Frontend:** Windows Forms for data entry, control, and visualization.

## Setup Instructions

1. **Hardware Configuration:**  
   - Assemble the components as described in the [Hardware Details](#hardware-configuration).

2. **Software Requirements:**  
   - Install the following:
     - [Visual Studio 2022](https://visualstudio.microsoft.com/2022/)
     - [SQL Server Management Studio](https://learn.microsoft.com/en-us/sql/ssms)
     - Arduino IDE

3. **Running the Project:**  
   - Deploy the `MedPreserveApp` from Visual Studio.
   - Load and run the Arduino sketch `LoggerConfig.ino` on Arduino Mega.

## Software Features
- **User Management:** Add, update, delete, and restore users with role-based access.
- **Device Configuration:** Register and sync hardware devices with thresholds.
- **Real-Time Graphs:** Live visualization of sensor data against limits.
- **Data Handling:** Load data from SD card to SQL database, clear SD card after upload.

## Contributing
Contributions to improve functionality or add new features are welcome. Please ensure compatibility with existing modules before submitting PRs.

## License
This project is licensed under the [MIT License](LICENSE).
