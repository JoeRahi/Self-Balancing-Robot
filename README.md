Self-Balancing Robot

This is a Self-Balancing Robot project that uses a PID control algorithm and an MPU6050 IMU sensor to maintain balance on two wheels. The robot adjusts its motor speeds to remain upright, similar to how a Segway functions.

Project Overview

The self-balancing robot features:

PID Control: Proportional-Integral-Derivative (PID) algorithm to stabilize the robot's tilt.

IMU Sensor: MPU6050 accelerometer and gyroscope to measure the robot's tilt angle.

Arduino: Arduino Uno board for processing sensor data and controlling the motors.

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

Assemble Hardware:

Mount the motors, sensors, and Arduino on the chassis.

Wire the motor driver and MPU6050 sensor to the Arduino.

Install Libraries:

Open Arduino IDE and install the necessary libraries (PID_v1, MPU6050, I2Cdev).

Upload Code:

Upload the code to the Arduino from this repository.

Usage

Once powered on, the robot will automatically balance itself by adjusting the motor speeds based on the tilt data from the MPU6050 sensor.

PID Tuning

The PID constants (Kp, Ki, Kd) are adjustable for fine-tuning the robot's performance. Experiment with these constants to improve stability, especially for different weights and chassis designs.

Robot Image

Closed-Loop System Diagram

License

This project is licensed under the MIT License.
