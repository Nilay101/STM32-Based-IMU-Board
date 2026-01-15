# Custom-STM32-Dev-Board
Custom STM32-based development board inspired by Phil’s Lab reference design, with design choices validated and documented.

## MCU
- STM32F4 series (ARM Cortex-M4) 
- Clock: External crystal oscillator
- Debug Interface: SWD

## Power Architecture
- Input: USB / External 5V
- Regulation: LDO / Buck (based on design choice)
- On-board decoupling and bulk capacitance

## Peripherals
- USB interface
- User LED
- GPIO headers

## Tools Used
- Altium Designer / KiCad
- STM32CubeIDE
- GitHub

## Project Status
- [x] Schematic
- [x] PCB Layout
- [ ] Fabrication
- [ ] Bring-up & Testing

## Future Upgrades 
- Communication Protocols
- Wifi and Bluetooth 

## Electrical Requirements
- MCU operating voltage: 3.3V ±5%
- USB supply: 5V
- Max current: 500mA
