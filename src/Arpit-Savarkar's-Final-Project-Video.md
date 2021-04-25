---
layout: default
title: Arpit-Savarkar's-Final-Project-Video
permalink: /src/Arpit-Savarkar's-Final-Project-Video.html
---

# Overview

This page provide's an overview of Arpit Savarkar contribution to the AESD Final Project to Setup Tiny Machine Learning on Arduino Nano 33 BLE Sense without IDE, over Cross compiler to talk to NVIDIA Jetson Nano : [Link to Video](https://drive.google.com/file/d/18ciKNH52RVWI6e7lmfBIayOLS7DNKMx1/view?usp=sharing)

# Video Outline and Topics Covered 
[Link to Video](https://drive.google.com/file/d/18ciKNH52RVWI6e7lmfBIayOLS7DNKMx1/view?usp=sharing)

The video demonstrates:
* [Introduction to TinyML for Embedded Systems on NVIDIA Jetson Nano and Arduino 33 BLE Sense](https://github.com/AESD-Course-Project/AESD-Course-Project.github.io/blob/master/src/TinyML.md)
* Arduino-CLI, custom Arduino-library setup and integration for human detection
  - [Hardware and CLI setup with custom library](https://github.com/AESD-Course-Project/AESD-Course-Project.github.io/blob/master/src/arduino_setup.md)
  - [Neural Network Traning and Porting for Micro-controllers](https://github.com/arpit6232/visualwakeup_aesd)
* OE4T meta-tegra setup for , API setup & interface for custom uartserver
  - [API, setup and response](https://github.com/AESD-Course-Project/AESD-Course-Project.github.io/issues/24)
  - [GPIO based feedback / Seven-Segment Display for human detection on Jetson Nano](https://github.com/cu-ecen-5013/final-project-arpit6232/tree/main/jetson_display)
* [Attempt at Dummy fullmac linux wifi driver for cfg80211 USB Wifi Module](https://github.com/cu-ecen-5013/final-project-arpit6232/tree/main/wifi_driver)
* [Yocto Integration with systemd based Init Script for peripheral during boot](https://github.com/cu-ecen-5013/final-project-CalebProvost/tree/yocto-layer)

## Challenges
My most difficult challenge when implementing this project were:
* Bringing up OE4T meta-tegra on NVIDIA Jetson Nano and Jetson Nano 2GB board using yocto and Docker
  - [OE4T Forum QA](https://github.com/OE4T/meta-tegra/discussions/661)
  - [Camera setup and test](https://github.com/OE4T/meta-tegra/discussions/653)
  - [NVIDIA Forum discussions - 1](https://forums.developer.nvidia.com/t/unable-to-boot-up-jetson-board-after-frc-on-jetson-nano-2gb-board/175113)
* [Arduino CLI setup integration and test on Yocto Image](https://github.com/arduino/ArduinoCore-mbed/issues/176)
* Logging state machine between custom UartServer and API response.
* Tensorflow based Deep Machine Learning for Embedded Systems. 

## Lessons Learned
The most important topics I learned from this project were:
* [systemd startup scripts for uartserver and arduino-cli](https://github.com/AESD-Course-Project/AESD-Course-Project.github.io/issues/29)
* Custom distro setup and build for NVIDIA OE4T meta-tegra setup
* Docker setup for amd64, aarch64. 
* GPIO communication. 
