# ESP-01 Relay Control over WiFi

- This is a simple relay control using an ESP-01 module over WiFi. 
- The provided code is designed to run on an ESP8266-based microcontroller and control a relay using a web server. 
- You can use this project to remotely turn a device on or off over an WLAN

## Prerequisites

Before you get started, make sure you have the following:

- An ESP-01 module or an ESP8266-based microcontroller.
- The Arduino IDE or another suitable development environment set up for ESP8266 development.
- A relay module, which you want to control. (ESP-01 usually comes with the relay)

## Hardware Setup

1. Connect your relay module to the ESP-01 as follows:
   - Connect the VCC of the relay module to the 3.3V pin of the ESP-01.
   - Connect the GND of the relay module to the GND pin of the ESP-01.
   - Plug in the ESP-01 into the relay socket

## Software Setup

1. Open the Arduino IDE and make sure you have the ESP8266 board support installed. If not, follow the official instructions for installing the ESP8266 board package.

2. Copy and paste the provided code into your Arduino IDE.

3. Modify the following variables in the code to match your WiFi network:
   - `NET_SSID`: Set this to the relay WiFi network's SSID (name).
   - `NET_PASS`: Set this to the relay WiFi network's password.

4. Compile and upload the code to your ESP-01 module.

5. After uploading, the ESP-01 module will create a WiFi network with the SSID defined in `NET_SSID` and the password defined in `NET_PASS`. You can connect your computer or mobile device to this WiFi network.
