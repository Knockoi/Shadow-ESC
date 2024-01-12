## ShadowDrive 
## Language selection:
[English](https://github.com/Knockoi/E-Stick/blob/main/README.md) | [日本語](https://github.com/Knockoi/Shadow-ESC/edit/main/README-JP.md) | [Traditional Chinese](https://github.com/Knockoi/E-Stick/blob/main/ReadmeTC.md)
  
## Overview  
ShadowDrive has a smaller size and higher integration compared to normal electric skateboard controllers. Although it is only the size of a credit card, the control capability is not sloppy and it can control 60V 170A Peak 300A motors.
  ! [image]()
  
## Hardware  
- MCU using two STM32F405RGT6
- Can choose to configure whether the MPU, gyroscope using MPU6500 data lines on two SDA and SCK.
- Grid controller using DRV8301~8303 option.
- LED display the current mode and system information.
- Bluetooth module is optional, you can use Bluetooth module to edit ShadowDrive.

## Function  
- Drive go-karts from 1 to 4WD (4WD requires two ShadowDrives).
- Drive Motorized Skateboards with 1~4 drives (4 drives require 2 ShadowDrives).
- Motorized Scooter
- Drive ONE-WHEEL (MPU-equipped version required)
- Drive any single motor 15000W BLDC motor.
  
## Features
- Current and voltage measurement in all phases (triple shunt design)
- Adjustable voltage filters
- Built-in IMU chip (accelerometer, gyroscope)
- Regenerative brakes
- Traction control (single and dual setting)
- Sensor or sensorless operation + mixed mode
- ASS Ready (Advanced Sensorless Start = full torque from 0 RPM)
Programmable RPM, current, voltage and power limits
- Input sources: PPM, analog
- Communication ports: USB, CAN, UAVCAN, UART
- Throttle curves and ramps for all input sources
- Individual throttle curves for acceleration and braking
- Seamless 4-quadrant operation
- Motor revolutions, ampere-hour, watt-hour counts
- Displays speed, power, duty cycle, amp flow, estimated range, and status on battery applications
- Accumulated data from VESC arrays
- Real-time data is analyzed and read out through the communication port.
- Real-time data analyzed and read via VESC-Tool APP or VESC-Tool software
- Adjustable protection:
### The above information is copied from the VESC product description.

  For basic usage, please refer to VESC's instructions.  
  The design blueprint is from vedderb's Perfection topic.  
     - [VESC Brushless Motor Drive](https://github.com/vedderb/bldc)


