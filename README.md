---
layout: default
title: AESD Course Project
permalink: ./
---

# Quick Overview Below. See our [Project Wiki](/docs/WikiHome.md) for more!

### Block Diagram - TODO

### Target Build System 
We intend to use Yocto as the bring up tool to generate Linux image on NVIDIA Jetson Nano.

### Hardware Platform
Intended hardware platforms for this project:

- [Jetson Nano](https://developer.nvidia.com/embedded/jetson-nano-2gb-developer-kit)
- [Arduino Nano 33 BLE](https://store.arduino.cc/usa/tiny-machine-learning-kit)
- [OV7675 Camera](https://www.arducam.com/docs/camera-breakout-board/0-3mp-ov7675/)

### Open Source Projects 
- [Open Soruce Projects](https://github.com/cu-ecen-5013/final-project-arpit6232/blob/main/docs/open_source_projects.md)

### Previously Used Content
- Yocto
- Signal handlers
- Clocks
- Init Scripts and Rootfs Overlays

### New Content 
- Yocto Image for Jetson Nano 
- Creating Modules for Arduino BLE 33 
- USB Interface for Jetson and Arduino
- Deplying Tiny Machine Learning (TinyML)
- Case study for TinyML

### Shared Material 
- [Flashing Image to SD Card](https://github.com/cu-ecen-5013/buildroot-assignments-base/wiki/Flashing-Images-to-SDCard)

### Source Code Organization 
- [Project Overview](https://github.com/AESD-Course-Project/AESD-Course-Project.github.io/blob/gh-pages/README.md)
- [Project Schedule]()
- [Caleb's Repository]()
- [Arpit's Repository](https://github.com/cu-ecen-5013/final-project-arpit6232)
- [Zach's Repository](https://github.com/cu-ecen-5013/final-project-ZachTurner07)

### Group's Overview 
#### Team Project Members 
- Caleb: Yocto Image Setup and build for Jetson Tegra (TBD)
- Zach: Communication Between Subsystems (Serial/I2C/USB/Bluetooth) (TBR)
- Arpit: Machine Learning Framework and TinyML Setup for scalable setup (TBM) 

* Things left -> Alarm driver, alarm hardware, Kernel Modules devel ...

> **_NOTE:_**  TBD - To be Defined, TBR - To be Refined, TBM - To be modified
### Schedule Page

- [Project Schedule]()

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

