# Ambient Light System Using Addressable LEDs with ESP32

## 📌 Project Overview

This project implements an **ambient light system** for computers using **WS2812B addressable LEDs** and an **ESP32** microcontroller running **WLED firmware**. The system dynamically syncs the LED colors with the screen content using **UDP over Wi-Fi**, providing an immersive experience for the user. It also supports remote LED control via **Adafruit IO (MQTT)** and direct local control through WLED’s web interface.

## 🔧 Hardware Used

- ESP32 Development Kit
- WS2812B Addressable LEDs
- 330Ω resistor
- Breadboard (optional)
- 5V LED power supply
- Electrical cables and a plug (AC to DC conversion)

## 💻 Software Used

- [WLED](https://kno.wled.ge/) firmware for ESP32  
- [Prismatik](https://github.com/psieg/Lightpack) for Ambilight screen syncing  
- [Adafruit IO](https://io.adafruit.com/) for MQTT-based remote LED control  
- Web browser for direct WLED configuration  

## 📐 System Architecture

The ESP32 receives screen data via UDP from Prismatik running on a PC and adjusts LED colors accordingly. Alternatively, MQTT messages from Adafruit IO can trigger LED changes remotely.

