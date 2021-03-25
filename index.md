---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
title: AESD Course Project
permalink: ./
theme: jekyll-theme-midnight
---

# Quick Overview Below. See our [Project Wiki]({% link docs/WikiHome.md %}) for more!

## Hardware Architecture

### Main Hub - Nvidia Jetson Nano 2GB Developer's Kit
* https://developer.nvidia.com/embedded/jetson-nano-2gb-developer-kit
* Jetson will run a yocto-built Tegra distribution

### External Camera Hub - Arduino Nano 33 BLE Sense with Tiny Machine Learning Shield
* https://store.arduino.cc/usa/tiny-machine-learning-kit
* Linked kit contains the Arduino Nano 33 BLE Sense with a shield for the OV7675 Camera

### Block Diagram - TODO

### Communication Between Subsystems
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
  * https://www.jetsonhacks.com/2019/04/08/jetson-nano-intel-wifi-and-bluetooth/

