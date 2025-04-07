# SX1281_QO100_TX
QO-100 SAT CW Transmitter with OLED Display using 2.4 GHz LoRa module with TCXO by OM2JU and OK1CDJ

https://www.nicerf.com/products/detail/500mw-2-4ghz-lora-wireless-transceiver-module-lora1280f27-lora1281f27.html

Only one DIGI mode possible - SLOW Hellschreiber - need bigger dish than 80cm - only beacon implemented yet 

*Maximal power output is 450mW. It is enought to work over satellite with 60cm DISH, but tested also with 35cm and helix feed.*

## Features
- Paddle input -IAMBIC keyer
- Straight key input
- Change frequency, power, keyer speed by rotary encoder
- Frequency callibration
- Beacon mode
- cwdaemon compatible UDP server on port 6789
- WiFi client or AP mode
- Web interface for WiFi config
- Web interafce for tuning, change speed and power
- New: PTT output on ESP32 module pin-12. This is logic signal, one must add external NPN/MOSFET. Configurable delay.

![alt text](https://raw.githubusercontent.com/ok1cdj/SX1281_QO100_TX/main/img/QO100-tx-purple.png)


## Used libraries
Adafruit GFX Library

Adafruit_SSD1306

SX12XX Library - https://github.com/StuartsProjects/SX12XX-LoRa

ESPAsyncWebServer - https://github.com/ESP32Async/ESPAsyncWebServer

AsyncTCP - https://github.com/ESP32Async/AsyncTCP

## How to program

Using the latest Arduino 2.XX
Install the SPIFFS upload plugin https://github.com/espx-cz/arduino-spiffs-upload

Select the ESP32 Dev Module
Hold RST button + PRG button on the board, then release the RST button.
Compile and upload.

To compile and upload the SPIFFS filesystem image:
Press [Ctrl] + [Shift] + [P] on Windows or [⌘] + [Shift] + [P] on MacOS to open the command palette. Search for the Upload SPIFFS to Pico/ESP8266/ESP32 command and click on it.

## User interface
![alt text](https://raw.githubusercontent.com/ok1cdj/SX1281_QO100_TX/main/img/QO100-tx.png)

