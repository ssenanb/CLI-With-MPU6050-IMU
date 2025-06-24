# CLI-With-MPU6050-IMU
->Description

In this project, the STM32 continously reads accelerometer and gyroscope data from the IMU sensor. Since the raw data is often noisy and affected by various environmental factors, an offset calibration is implemented to improve measurement accuracy. The system includes a Command Line Interface (CLI) over UART, allowing the user to interact with the system by sending commands. Through the CLI, the user can:

-> CLI Commands

  > help : list all available commands

  > gyro : display real-time gyroscope data

  > acc : display real-time accelerometer data
  
  > last_gyro : retrieve the last 5 gyroscope readings
  
  > last_acc : retrieve the last 5 accelerometer readings

-> Compenents Used

STM32F0DISC

MPU6050 IMU Sensor

UART Module

Jumper Cables

Figure 1 : System Overview 

<img src="https://github.com/ssenanb/CLI-With-MPU6050-IMU/blob/main/system_overview.jpeg" alt="System Overwiew" width="500"/>

<img src="https://github.com/ssenanb/CLI-With-MPU6050-IMU/blob/main/sensor_image.jpeg" alt="System Overwiew" width="500"/>

Figure 2 : Output in the Termite

<img src="https://github.com/ssenanb/CLI-With-MPU6050-IMU/blob/main/termite.png" alt="CLI" width="500"/>

-> Configuration

Figure 3 : Confgiuration in the STM32CubeIDE

<img src="https://github.com/ssenanb/CLI-With-MPU6050-IMU/blob/main/configuration.png" alt="Configuration" width="500"/>

PA9 -> USART1_TX (with Interrupt)

PA10 -> USART1_RX (with Interrupt)

PB6 -> I2C1_SCL (to the IMU)

PB7 -> I2C1_SDA (to the IMU)


