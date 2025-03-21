# Weather Satellite Tracking with RTL-SDR: NOAA

This project demonstrates the tracking of the **NOAA-15** weather satellite using **RTL-SDR (Software Defined Radio)** and a **V-dipole antenna**. The system is designed to receive and decode **Automatic Picture Transmission (APT)** signals from the satellite, allowing real-time image processing of the Earth’s surface for weather monitoring and environmental studies.

## Project Overview

As the number of satellites in orbit increases, effective tracking systems are essential for ensuring accurate data reception and avoiding satellite collisions. This project focuses on **NOAA-15**, a polar orbiting satellite used for weather monitoring by the **National Oceanic and Atmospheric Administration (NOAA)**. Using a **RTL-SDR USB dongle**, the system captures the satellite's transmission at **137.62 MHz**, decodes the APT signal, and produces images of the Earth’s surface.

The setup is cost-effective and allows for easy access to real-time satellite data for both educational and research purposes.

### Key Components:
- **RTL-SDR USB Dongle**: A software-defined radio receiver used for signal reception.
- **V-Dipole Antenna**: A simple, inexpensive antenna that receives circularly polarized signals from the satellite.
- **Software**:
   - **Cubic SDR**: Used to interface with the RTL-SDR and receive the signal.
   - **WXtoImg**: A software tool used to decode and process the APT signal from NOAA-15.
   - **GPredict**: Used for satellite tracking and orbit prediction.

### Objective:
- To receive and decode APT signals from NOAA-15.
- To generate high-resolution images of the Earth’s surface.
- To provide a low-cost solution for satellite tracking and weather monitoring.

## System Design

The system operates by tracking the **NOAA-15 satellite** and receiving its **APT signal** at **137.62 MHz** using a **V-Dipole antenna**. The received signal is processed using the **RTL-SDR** dongle, and the decoded image is displayed and stored for further analysis.

1. **Signal Reception**:
   - The **V-dipole antenna** captures the 137.62 MHz signal transmitted by **NOAA-15**.
   - The **RTL-SDR** dongle receives and processes the signal.

2. **Signal Decoding**:
   - The **Cubic SDR** software interfaces with RTL-SDR to receive the signal.
   - **WXtoImg** decodes the APT signal and converts it into a visual representation of the Earth’s surface.

3. **Satellite Tracking**:
   - **GPredict** software predicts the satellite’s orbit and provides real-time tracking of the satellite’s position.

## Tools Used

1. **RTL-SDR USB Dongle**: Receives satellite signals for further processing.
2. **V-Dipole Antenna**: Used to capture the 137.62 MHz APT signals.
3. **Cubic SDR**: Software to interact with the RTL-SDR dongle for signal reception.
4. **WXtoImg**: Decodes the received APT signal into images of Earth’s surface.
5. **GPredict**: Software for satellite orbit prediction and tracking.

## Steps to Run the System

### 1. Set up the Hardware:
   - Connect the **V-Dipole antenna** to the **RTL-SDR USB dongle**.
   - Ensure that the **RTL-SDR dongle** is connected to the computer via USB.

### 2. Install the Software:
   - Install **Cubic SDR** to interface with the RTL-SDR dongle.
   - Install **WXtoImg** to decode the APT signal.
   - Install **GPredict** for satellite tracking.

### 3. Track and Receive Signals:
   - Open **GPredict** and input the parameters for **NOAA-15** to track its position and predict its pass.
   - Use **Cubic SDR** to tune the RTL-SDR dongle to the frequency **137.62 MHz** to receive the APT signal from NOAA-15.

### 4. Decode the Signal:
   - After receiving the signal, open **WXtoImg** to decode the APT signal into an image.
   - The software will process and display images of the Earth’s surface, capturing cloud cover, weather patterns, and other environmental features.
