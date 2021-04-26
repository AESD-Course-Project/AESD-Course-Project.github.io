---
layout: default
title: Zach-Turner's-Final-Video-Page
permalink: /src/Zach's-Turner-Final-Project-Video.html
---

# Overview

This page provides an overview of Zach Turner's contribution to the AESD Final Project Human Recognition using the Nvidia Jetson and Arduino BLE 33 Sense.

# Video Outline
See [Highlight Video](https://drive.google.com/file/d/1z3vqiXsShyruKczYebtUcMQlt5CDPW2r/view?usp=sharing)

The video demonstrates:
* cross-compiling application from host machine to target board
* serial communication between Nvidia Jetson and Arduino
* Logging serial messages from human recognition on Nvidia Jetson

## Challenges
My most difficult challenge when implementing this project were:
* Creating the Yocto image to flash for the Jetson Nano
  * Difficulties with VM resources and virtual disk sizes
* Getting both boards to communicate on a pre-defined API
  * Debugging communication between two boards, only connected to one board
  * passing bytes between both boards at a given symbol rate and validating the message

## Lessons Learned
The most important topics I learned from this project were:
* Serial communication using linux system calls are as simple as file read/writes because devices are files in the linux filesystem.
* Configuring a serial device from an appplication using the `termio` API.
* Creating a server/client communication ICD and implementing the read/write between subsystems to facilitate transitioning between states.

