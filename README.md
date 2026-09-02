# STM32 based Inertial Measurement Unit (IMU) Module
## 1. Project Overview
This project is a custom-designed development board featuring an STM32 microcontroller (STM32F411CEU6) integrated with an MPU-6050 6-axis accelerometer and gyroscope. The board is designed for high-performance motion tracking applications, prioritizing a compact form factor and optimized power delivery.

Inspired by Phil’s Lab reference designs, this board was developed from scratch in Altium Designer. The design process strictly follows industry-standard hardware practices for schematic capture, 4-layer PCB layout, and signal integrity—with all design choices validated and fully documented.

The design was developed in Altium Designer, following industry-standard practices for schematic capture, PCB layout, and signal integrity.


## 2. Key Specifications
> [Technical Specifications]
* `Microcontroller: STM32F411CEU6 (ARM Cortex-M4)`
* `Sensor: MPU-6050 (6-DOF IMU) via I2C interface.`
* `Power Input: 5V via Micro-USB connector.`
* `Power Regulation: On-board LDO regulating 5V to 3.3V for MCU and sensor logic.`
* `Communication: I2C for sensor data; SWD (Serial Wire Debug) header for programming.`

>[Physical Specifications]

*  Dimensions: 37mm x 34mm x 2mm
![image alt](https://github.com/Nilay101/STM32-Based-IMU-Board/blob/main/Manufacturing%20Details/New_Dimensions.png?raw=true)

## 3. Block Diagram 
The follow image shows the design flow and architecture of the PCB in high-level block diagram.
                                      
![image alt](https://github.com/Nilay101/STM32-Based-IMU-Board/blob/main/Images/Block_Diagram.jpg?raw=true)


## 4. Layer Stack 
                            
![image alt](https://github.com/Nilay101/STM32-Based-IMU-Board/blob/main/Manufacturing%20Details/Layer_Stack_1.png?raw=true)
The board utilizes a 4-layer stackup to ensure robust power distribution dynamics and minimize electromagnetic interference (EMI) for sensitive I2C traces.

`Layer 1 (Signal): Top routing and component placement`

`Layer 2 (GND): Solid ground plane for return paths`

`Layer 3 (GND): Secondary ground plane`

`Layer 4 (Signal): Bottom routing`
<table>
  <tr>
    <td><img src="https://github.com/Nilay101/STM32-Based-IMU-Board/blob/7682db277642496030ad1f8c85eb5979f05e7b81/Images/Layer(1).png"/></td>
    <td><img src="https://github.com/Nilay101/STM32-Based-IMU-Board/blob/7682db277642496030ad1f8c85eb5979f05e7b81/Images/Layer(2).png"/></td>
  </tr>
  <tr>
    <td><img src="https://github.com/Nilay101/STM32-Based-IMU-Board/blob/7682db277642496030ad1f8c85eb5979f05e7b81/Images/Layer(3).png"/></td>
    <td><img src="https://github.com/Nilay101/STM32-Based-IMU-Board/blob/7682db277642496030ad1f8c85eb5979f05e7b81/Images/Layer(4).png"/></td>
  </tr>
</table>

## 5. Final Overview

![image alt](https://github.com/Nilay101/STM32-Based-IMU-Board/blob/main/Images/Final.png?raw=true)

## 6. Future Extensions
As this project is intended to highlight physical hardware architecture rather than embedded software programming, future board revisions will target physical and analog enhancements:

Multi-Rail Power Distribution: Replacing the standard LDO with a dedicated physical buck converter module to regulate separate voltage rails (e.g., isolating the analog sensor supply from the digital MCU supply) for reduced switching noise.

Analog Front-End (AFE) Integration: Adding discrete op-amp stages to filter and condition additional external analog sensors before routing signals to the STM32's internal ADC.

Enhanced Testability: Adding dedicated surface-mount test points (TPs) across the I2C bus and power distribution traces for easier board-level trace physics validation and oscilloscope probing.

