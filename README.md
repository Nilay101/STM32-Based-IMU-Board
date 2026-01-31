# STM32 based Inertial Measurement Unit (IMU) Module
>[Note]: This project is a product of independent, self-taught study into PCB design and Circuit Design using Professional Tools. As a Self-learning candidate I am trying to implement a Design Flow which is followed according to the industry-standard workflows—including those shared by professional mentors like Phil’s Lab. This Project may contains errors which have been overlooked by me the the process of designing it. Any suggestions, changes or recommendations would be appreciated.

## 1. Project Overview
` This project is a custom-designed development board featuring an STM32 microcontroller (STM32F411CEU6) integrated with an MPU-6050 6-axis accelerometer and gyroscope. The board is designed for high-performance motion tracking applications, featuring a compact form factor and optimized power delivery.
Custom STM32-based Embedded board inspired by Phil’s Lab reference design, with design choices validated and documented designed in Altium Designer. `

`The design was developed in Altium Designer, following industry-standard practices for schematic capture, PCB layout, and signal integrity.` 

## 2. Block Diagram

![image alt](https://github.com/Nilay101/STM32-Based-IMU-Board/blob/main/Images/Block_Diagram.jpg?raw=true)


## 3. Key Specifications
> [Technical Specifications]
* `Microcontroller: STM32F411CEU6 (ARM Cortex-M4)`
* `Sensor: MPU-6050 (6-DOF IMU) via I2C interface.`
* `Power Input: 5V via Micro-USB connector.`
* `Power Regulation: On-board LDO regulating 5V to 3.3V for MCU and sensor logic.`
* `Communication: I2C for sensor data; SWD (Serial Wire Debug) header for programming.`

>[Physical Specifications]

* ` Dimensions: 37mm x 34mm x 2mm`
![image alt](https://github.com/Nilay101/STM32-Based-IMU-Board/blob/main/Hardware/Dimension.png?raw=true)

## 4. Layer Stack 

![image alt](https://github.com/Nilay101/STM32-Based-IMU-Board/blob/main/Manufacturing%20Details/Layer_Stack_1.png?raw=true)
