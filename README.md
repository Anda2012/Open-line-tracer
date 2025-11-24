**Open source MicroPython 11-Channel PID Line Follower**

ESP32-C3 Mini-1 + Massmore JET QTR-11D

This project is a compact and accurate line follower built with an ESP32-C3 Mini-1 running MicroPython and an 11-channel Massmore JET QTR-11D reflectance sensor. It reads all sensor channels, calculates line position, and applies a tunable PID controller to drive the motors smoothly.

 Features

11-channel reflectance sensing

PID control (P, I, D adjustable in code)

Smooth PWM motor output

Simple, modular MicroPython code

Works with the DRV8833 motor driver

uses the ip5306 battery charger & boost converter

 **Project Structure**
src
 │ main.py         Main loop + motor control
 │ config.py       PID + speed settings


**Setup**

Install MicroPython on the ESP32-C3.

Upload the /src files to the board.

Adjust PID constants in config.py as needed.

Run main.py to start the line follower.

**PID Tuning Tips**

Increase P for stronger corrections.

Add I to reduce drift on long straights.

Use D to smooth out fast turns.

**License**

MIT License
