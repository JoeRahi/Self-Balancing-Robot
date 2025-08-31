Self-Balancing Robot with PID Control

This project involves building a self-balancing robot that uses a PID control algorithm and an MPU6050 IMU sensor to maintain balance. The robot continuously adjusts its motor speeds to stay upright, mimicking the balancing mechanism of a Segway.

Features

PID Control: Uses Proportional-Integral-Derivative (PID) control to stabilize the robot.

IMU Sensor: Utilizes the MPU6050 accelerometer and gyroscope to measure the tilt angle.

Arduino Uno: The microcontroller that processes sensor data and controls the motors.

Automatic Balancing: The robot adjusts its motor speeds based on tilt data to maintain an upright position.

PID Tuning: Adjust PID constants for fine-tuning the robot's performance.

Hardware Components

Arduino Uno: The main controller for processing sensor data and controlling motors.

L298N Motor Driver: Controls the direction and speed of the DC motors.

MPU6050: The gyroscope and accelerometer that measure the robot’s tilt angle.

DC Motors with Encoders: Powers the wheels and enables movement.

RC Racing Wheels: Provides the wheels for the robot.

Battery: 9V or 2x 18650 Li-ion batteries for power.

Chassis: Laser-cut Plexiglass chassis for mounting the components.

Wires, Screws, and Mounting Brackets: For assembly.

Software Requirements

Arduino IDE: To write and upload the code to the Arduino board.

Libraries Needed

PID_v1

MPU6050

I2Cdev

How It Works

The MPU6050 sensor measures the tilt angle of the robot.

The PID control algorithm processes the tilt data and calculates the necessary motor adjustments to maintain balance.

The Arduino continuously adjusts the motor speeds to correct the robot’s position and keep it upright.

Code Overview

The Arduino code does the following:

Reads data from the MPU6050 sensor to determine the robot's tilt angle.

Implements the PID algorithm to compute the necessary adjustments for motor speeds.

Controls the motors through the L298N motor driver to keep the robot balanced.

PID Tuning

The robot’s performance can be fine-tuned by adjusting the following PID constants:

Kp (Proportional): Controls the robot’s response to tilt.

Ki (Integral): Helps correct long-term errors.

Kd (Derivative): Damps out oscillations and smoothens the response.

Experiment with these constants to optimize the robot’s stability, especially for different weights and designs.

Getting Started
1. Hardware Setup:

Mount the motors, sensor, and Arduino on the chassis.

Wire the motor driver (L298N) and MPU6050 to the Arduino according to the provided circuit diagram.

2. Software Setup:

Install the required libraries in the Arduino IDE: PID_v1, MPU6050, I2Cdev.

Upload the provided code to the Arduino Uno.

3. Testing the Robot:

Power the robot on and ensure the MPU6050 sensor is properly aligned.

The robot should automatically begin balancing by adjusting the motor speeds.

Project Visuals
Self-Balancing Robot

Closed-Loop System Diagram

License

This project is open-source and available under the MIT License. See the LICENSE file for more details.
