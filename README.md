
##  Heart Rate Monitoring

INTRODUCTION:

This is a simple yet effective real-time heart rate monitoring system built using an ESP32 microcontroller and an OLED display. The system reads the user's heart rate in BPM (beats per minute) and displays it on the OLED screen, making it ideal for personal health tracking or wearable prototypes.


## Table of Contents
Introduction

Project Overview

Key Components

code overview

output

future and improvements


## Project Overview
The heart rate monitor detects the user's pulse using a pulse sensor (usually an IR-based module), calculates the BPM, and displays the results on a 0.96" OLED screen. The ESP32 board handles sensor reading, timing, and display updates. This setup can be easily extended to include Wi-Fi-based logging or mobile alerts.


## Key Components
ESP32 Dev Board – Main controller with Wi-Fi and Bluetooth support

Pulse Sensor – IR-based sensor to detect heartbeats from finger

OLED Display (SSD1306) – 128x64 I2C display to show BPM and system status

Jumper Wires and Breadboard – For wiring and prototyping

USB Cable – For programming and power supply



## Code Overview

Key functions:

analogRead() — reads pulse input

millis() — measures time between pulses

display.print() — shows BPM on OLED

OLED library used: Adafruit_SSD1306

Sensor reading algorithm filters out noise using averaging
## Output 

Stable BPM readings update every second.

Portable and suitable for wearable projects
![1](https://github.com/user-attachments/assets/42ec4df8-6f92-4ef6-9432-ee1c9f372ba2)

## Future and improvements
Add Wi-Fi logging to Firebase or Thingspeak

Send SMS/email alerts on abnormal BPM

Integrate with Android app via Bluetooth

Add temperature and SpO2 sensors for complete vitals monitoring

