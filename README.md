#STM32 Servo Control using Potentiometer
This project is a simple demonstration of how to control a servo motor using a potentiometer and an STM32 microcontroller. The project was created using the STM32CubeIDE development environment and is based on the STM32F4-Discovery board.

## Setup
To use this project, you'll need to do the following:

* Connect the servo motor to the STM32F4-Discovery board. The servo motor should be connected to pin PD12 on the board.

* Connect the potentiometer to the STM32F4-Discovery board. The potentiometer should be connected to pin PA0 on the board.

* Import the project into STM32CubeIDE and flash it to the board.

Power on the board and turn the potentiometer to control the position of the servo motor.

## Code Overview
The project code is written in C and consists of three main files:

* main.c: This file contains the main function that initializes the peripherals and starts the servo control loop.

* stm32f4xx_it.c: This file contains the interrupt handlers for the STM32F4 microcontroller.

* stm32f4xx_hal_msp.c: This file contains the MSP (MCU Support Package) initialization code.

The servo control loop is implemented in the main.c file. It reads the value of the potentiometer using an ADC (analog-to-digital converter) and maps the value to a range that can be used to control the position of the servo motor. The position of the servo motor is updated using a PWM (pulse-width modulation) signal.

## References
Here are some useful resources for learning more about the STM32 microcontroller and the STM32CubeIDE development environment:

* [STMicroelectronics](https://www.st.com/content/st_com/en.html): The official website for STMicroelectronics, the manufacturer of the STM32 microcontroller.

* [STM32CubeIDE](https://www.st.com/en/development-tools/stm32cubeide.html): The official integrated development environment (IDE) for STM32 microcontrollers.

* [STM32F4-Discovery User Manual](https://www.st.com/resource/en/user_manual/dm00039084-stm32f4discovery-kit-with-stm32f407vg-mcu-stmicroelectronics.pdf): The user manual for the STM32F4-Discovery board.

* [Servo Motor Tutorial](https://www.arduino.cc/en/Tutorial/sweep): A tutorial on how to control a servo motor using an Arduino, which can be adapted to work with an STM32 microcontroller.

