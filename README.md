Self-Balancing Robot

This project implements a Self-Balancing Robot that uses a PID control algorithm and an MPU6050 IMU sensor to maintain balance on two wheels. The robot adjusts its motor speeds to stay upright, similar to how a Segway works.

Project Overview

The self-balancing robot features:

PID Control: Utilizes a Proportional-Integral-Derivative (PID) algorithm to stabilize the robot's tilt.

IMU Sensor: Uses the MPU6050 accelerometer and gyroscope to measure the robot's tilt angle.

Arduino: An Arduino Uno board is used for processing sensor data and controlling the motors.

Hardware Components

Arduino Uno

L298N Motor Driver

MPU6050 Gyroscope + Accelerometer

6V DC Motors with Encoders

RC Racing Wheels

9V Battery or 2x 18650 Li-ion Batteries

Laser Cut Plexiglass Chassis

Screws, Couplings, Mounting Brackets, and Wires

Software Requirements

Arduino IDE

Libraries:

PID_v1

MPU6050

I2Cdev

How to Build
1. Assemble Hardware:

Mount the motors, sensors, and Arduino on the chassis.

Wire the motor driver (L298N) and MPU6050 sensor to the Arduino Uno.

2. Install Libraries:

Open the Arduino IDE and install the necessary libraries:

PID_v1

MPU6050

I2Cdev

3. Upload Code:

Upload the provided code from this repository to the Arduino board.

Usage

Once powered on, the robot will automatically balance itself by adjusting the motor speeds based on the tilt data from the MPU6050 sensor.

PID Tuning

The PID constants (Kp, Ki, Kd) are adjustable to fine-tune the robot's performance. Experiment with different values to improve stability, especially for various chassis designs and weights.

Robot Image

Closed-Loop System Diagram

License

This project is licensed under the MIT License
.
