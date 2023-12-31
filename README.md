# MPU-6050

# MPU6050 Sensor Data Readings

[![License](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)

## Description

This Arduino project reads accelerometer, gyroscope, and temperature data from the MPU6050 sensor and displays the readings on the serial monitor. The MPU6050 is a commonly used sensor module that combines a 3-axis gyroscope and a 3-axis accelerometer in a single package. This project demonstrates how to use the MPU6050 sensor to obtain real-time sensor data.The MPU-6050 IMU (Inertial Measurement Unit) is a 3-axis accelerometer and 3-axis gyroscope sensor. The accelerometer measures the gravitational acceleration and the gyroscope measures the rotational velocity. Additionally, this module also measures temperature. This sensor is ideal to determine the orientation of a moving object.

## Table of Contents

- [Introduction](#introduction)
- [Features](#features)
- [Hardware Setup](#hardware-setup)
- [Library Dependencies](#library-dependencies)
- [Installation](#installation)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

## Introduction

The MPU6050 is a popular sensor module used in various applications, such as robotics, drones, and motion tracking. It provides accurate readings of acceleration and rotation in three dimensions, along with temperature data. This project serves as a basic example of interfacing with the MPU6050 sensor and obtaining its data using an Arduino board.

## Features

- Read real-time accelerometer data (X, Y, Z) in m/s^2.
- Read real-time gyroscope data (X, Y, Z) in rad/s.
- Read real-time temperature data in degrees Celsius.

## Hardware Setup

### Components Required

- Arduino board (e.g., Arduino Uno)
- MPU6050 Sensor Module
- Jumper wires

### Circuit Connection

Connect the MPU6050 sensor to the Arduino board as follows:


MPU6050   Arduino
  VCC  ->   5V
  GND  ->   GND
  SDA  ->   A4 (on Uno/Nano)
  SCL  ->   A5 (on Uno/Nano)


![image](https://github.com/Shivani9698/MPU-6050/assets/119753029/7fc71746-7da8-45ca-b96a-6212db6a3fab)


## Library Dependencies

- Adafruit MPU6050 Library (Install using the Arduino Library Manager)

## Installation

1. Install the Arduino IDE from the official website if you haven't already.
2. Open the Arduino IDE and navigate to `Sketch -> Include Library -> Manage Libraries`.
3. Search for "Adafruit MPU6050" in the Library Manager and install the "Adafruit MPU6050" library.
4. To use this library, you also need to install the Adafruit Unified Sensor library and the Adafruit Bus IO Library.
5. Open your Arduino IDE and go to Sketch > Include Library > Manage Libraries. The Library Manager should open.
6.Then, search for “Adafruit Unified Sensor”. Scroll all the way down to find the library and install it.
7.Finally, search for “Adafruit Bus IO” and install it.
8. Copy and paste the provided code (`mpu6050_sensor_readings.ino`) into a new Arduino sketch.
9. Connect the MPU6050 sensor to the Arduino board as described in the hardware setup section.
10. Upload the sketch to your Arduino board.

## Usage

1. Open the Arduino IDE and connect the Arduino board to your computer.
2. Make sure the correct board and port are selected under the `Tools` menu.
3. Upload the code to the Arduino board by clicking the `Upload` button.
4. Open the Serial Monitor by clicking on `Tools -> Serial Monitor` or pressing `Ctrl + Shift + M`.
5. The Serial Monitor will display the real-time sensor data readings, including accelerometer (X, Y, Z), gyroscope (X, Y, Z), and temperature data.


## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.


