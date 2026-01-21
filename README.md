# STM32 based Inertial Measurement Unit (IMU) Module

## 1.Project Overview
This project is a custom-designed development board featuring an STM32 microcontroller (STM32F411CEU6) integrated with an MPU-6050 6-axis accelerometer and gyroscope. The board is designed for high-performance motion tracking applications, featuring a compact form factor and optimized power delivery.
Custom STM32-based Embedded board inspired by Phil’s Lab reference design, with design choices validated and documented designed in Altium Designer. 

The design was developed in Altium Designer, following industry-standard practices for schematic capture, PCB layout, and signal integrity.


## 2.Key Specifications
Technical Specifications
Microcontroller: STM32F411CEU6 (ARM Cortex-M4)

Sensor: MPU-6050 (6-DOF IMU) via I2C interface.

Power Input: 5V via Micro-USB connector.

Power Regulation: On-board LDO regulating 5V to 3.3V for MCU and sensor logic.

Communication: I2C for sensor data; SWD (Serial Wire Debug) header for programming.

PCB Details: 4-layer board
Layer 1: Signal Plane
Layer 2: Ground Plane
Layer 3: Ground Plane
Layer 4: Signal Plane

## Block Diagram

![image alt](https://github.com/Nilay101/Custom-STM32-Dev-Board/blob/16371348452a1c2ff128c51463f2502fd200e9f9/image.png)


## Technical Challeneges and Design choices





## Tools used
- Altium Designer
- GitHub

## Project Status
- [x] Selection of Components
- [x] Schematic
- [x] Electrical Rule Check
- [x] PCB Layout
- [ ] Design Rule Check
