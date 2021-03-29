---
layout: default
title: AESD Course Project Overview
permalink: /Overview.html
---

## Overview 
This project intends to deal with integrating and building a object detection framework and its dectection based on camera and peripheral micro-controller  (Arduino BLE 33 mBed) connected to a NVIDIA Jetson Nano acting as a hub. For the purpose of demonstration we would be attaching a low power camera attached to the micro-controller to act as an inference engine built over Machine Learning Framework to interact with Jetson Nano and form a feedback loop to alarm a system of detection of person in frame of camera. The aim of this project is to train a machine learning model and deploy over low-power, low-memory micro-controllers and form feedback system of the Embedded Network Hub (Jetson). This would include bringing up completely independent hardware which includes the controlling unit, sensors, and software bring up, which includes Operating systems, communication protocols, coding styles, and languages.

Using low-level micro-controllers is cheap and provides more opportunity (future goal) to scale the product under development and testing providing both financial and engineering benefits. 

NVIDIA Jetson acts as a server for the peripheral boards(clients). The term voting technique indicates that at any given time the reading that is received from the majority of the sensors will be considered for further actions. Two Camera feeds are available to work with one resides on the NVIDIA Jetson and other connected to the Peripheral Board. 

Major Goals:

- Yocto to compile meta-tegra.
- Running Tegra-demo-distro with Arduino Setup.
- Setup Camera board and Communication.
- Build deep-stream or opencv (hardware accelerated) running on Jetson Nano. 
- Run AI Image recognition project working with on image on Host/Hub (Jetson) and/or Arduino BLE 33 with Camera. 

System works as a hard real time system, which captures camera feed at set time interval irrespective of how much time the sensors take to send data over to Nano. The overaching goal of this project would be create a Hub and Client mechanism such that machine learning can be deployed on micro-controllers with and without GPU's. 

## Block Diagrams

### Hardware Block Diagrams
![HW Block Diag](http://interactive.blockdiag.com/image?compression=deflate&encoding=base64&src=eJxLyslPzk7JTExXqOZSUEgvyi8tALMUFHISk1JzFGwVlByLUkoz8_KVrMHCzom5qUWJCrp2CkrO-bm5Cv6lJUoK0QjFnkqxIIW1QIykAK7cMw9ZNUgoMS8FogWr5SGp6UWJUKsRJoCM88_TTcpPLEpR8HF1QTbTNz-lNCcVYqQCmjKIy2oBSKdD0g)  

### Software Block Diagrams 
![SW Block Diag](https://mermaid.ink/svg/eyJjb2RlIjoic3RhdGVEaWFncmFtLXYyXG4gICAgc3RhdGUgXCJDYW1lcmEgRGF0YSBGZWVkXCIgYXMgQ2FtZXJhXG5cbiAgICBzdGF0ZSBBcmR1aW5vIHtcbiAgICAgICAgQ2FtZXJhIC0tPiBBcmR1aW5vQUlcbiAgICAgICAgc3RhdGUgQXJkdWlub0FJIHtcbiAgICAgICAgICAgIFByb2Nlc3NGZWVkIC0tPiBJc0h1bWFuXG4gICAgICAgICAgICBJc0h1bWFuIC0tPiBQcm9jZXNzRmVlZCA6IE5vXG4gICAgICAgICAgICBJc0h1bWFuIC0tPiBTZW5kQ01EIDogWWVzXG4gICAgICAgIH1cbiAgICAgICAgU2VuZENNRCAtLT4gTm9kZVxuXG4gICAgfVxuICAgIHN0YXRlIFRlZ3JhIHtcbiAgICAgICAgTm9kZSAtLT4gU2Nyb2xsTG9ja09mZlxuICAgIH1cbiIsIm1lcm1haWQiOnt9LCJ1cGRhdGVFZGl0b3IiOmZhbHNlfQ)

### Functional Block Diagrams
See Software Block Diagram

## Target Build System 
We intend to use Yocto as the bring up tool to generate Linux image on NVIDIA Jetson Nano.

## Hardware Platform
Intended hardware platforms for this project:

- [Jetson Nano](https://developer.nvidia.com/embedded/jetson-nano-2gb-developer-kit)
- [Arduino Nano 33 BLE](https://store.arduino.cc/usa/tiny-machine-learning-kit)
- [OV7675 Camera](https://www.arducam.com/docs/camera-breakout-board/0-3mp-ov7675/)

## Open Source Projects 
- [Tensorflow](https://github.com/tensorflow/tensorflow)
- [Tensorflow Lite](https://github.com/tensorflow/tflite-support)
- [Tensorflow Micro](https://github.com/tensorflow/tensorflow/tree/master/tensorflow/lite/micro)
- [Meta Tegra for Yocto](https://github.com/OE4T/meta-tegra)
- [Arduino CLI](https://github.com/arduino/arduino-cli)
- [Arduino IDE](https://github.com/arduino/Arduino)
- [TinyML](https://www.oreilly.com/library/view/tinyml/9781492052036/)

## Previously Used Content
- Yocto
- Signal handlers
- Clocks
- Init Scripts and Rootfs Overlays

## New Content 
- [Yocto Image for Jetson Nano](https://github.com/AESD-Course-Project/AESD-Course-Project.github.io/tree/gh-pages/src/install_jetson_yocto.md) <sub>[Markdown](https://github.com/AESD-Course-Project/AESD-Course-Project.github.io/tree/gh-pages/src/install_jetson_yocto.md)</sub> 
- Creating Modules and scripts for Arduino BLE 33 
- [Interface for Jetson and Arduino](https://github.com/AESD-Course-Project/AESD-Course-Project.github.io/tree/gh-pages/src/arduino_setup.md) <sub>[Markdown](https://github.com/AESD-Course-Project/AESD-Course-Project.github.io/tree/gh-pages/src/arduino_setup.md)</sub>
- Deplying Tiny Machine Learning (TinyML)
- [Case study for TinyML](https://github.com/AESD-Course-Project/AESD-Course-Project.github.io/tree/gh-pages/src/TinyML.md) <sub>[Markdown](https://github.com/AESD-Course-Project/AESD-Course-Project.github.io/tree/gh-pages/src/TinyML.md)</sub>

## Shared Material 
- [Flashing Image to SD Card](https://github.com/cu-ecen-5013/buildroot-assignments-base/wiki/Flashing-Images-to-SDCard)

## Source Code Organization 
- [Project Webpage](https://AESD-Course-Project.github.io): Dynamically Generated Documentation
- [Project Overview](src/Project-Overview.md): Project Synopsis
- [Project Schedule](src/Project-Schedule.md): Project Schedule
- [Caleb's Repository](https://github.com/cu-ecen-5013/final-project-CalebProvost): One-click-build script Focused
- [Arpit's Repository](https://github.com/cu-ecen-5013/final-project-arpit6232): Image Development Focused
- [Zach's Repository](https://github.com/cu-ecen-5013/final-project-ZachTurner07): Driver & Module Code Focused

## Group's Overview 
### Team Project Members 
- Caleb: Yocto Image Setup and build for Jetson Tegra, Dockerfile 1-click-image
- Zach: Communication Between Subsystems (Serial/I2C/USB/Bluetooth)
  - serial communication between subsystems
  - GPIO communication to show successful inferencing... how it interfaces to BSP
  - Trigger on board LED for demonstration purposes
- Arpit: Machine Learning Framework and TinyML Setup and yocto compatibility. 
  - Dive Deep into Tiny Machine Learning deployment
  - Integrate Camera and peripheral to detect Person in frame. 
  - Code Porting and Tensorflow dependencies. 


## Schedule Page
- [Project Schedule](src/Project-Schedule.md): Project Schedule 


<!-- ### Communication Between Subsystems
Couple of options:

* Serial communication between Jetson and Arduino
  * Simplist electrical connection, connect USBA on Jetson to MicroUSB on Arduino
  * Use TTY device on Jetson to communicate serially with Arduino
  * Could create our own daemon to interact with the TTY device

* I2C between Jetson and Arduino
  * Lower level protocol, but still supported by both ends
  * Would need to research how to interact with I2C communication from linux on Jetson

* Potential Stretch (and a big stretch at that)
  * Install WiFi/Bluettoth network card onto Jetson board
  * Communicate with Arduino over Bluetooth 
  * https://www.jetsonhacks.com/2019/04/08/jetson-nano-intel-wifi-and-bluetooth/ -->
