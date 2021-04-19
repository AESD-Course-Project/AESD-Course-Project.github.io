# Communication Between Subsystems
## Tradespace
Couple of options in the tradespace:

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

## Current Communication Plan

* Serial communication between Arduino and Jetson over USB connection
* Start with user space application, build it up to a TTY kernel module to act as an interace for the arduino to the Jetson
* Set up read/write commands between the two devices via the kernel module