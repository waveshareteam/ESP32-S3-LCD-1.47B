# LVGL Arduino

[English](README.md) | [简体中文](README_ZH.md)

## What It Does

Runs an LVGL interface on the ST7789 LCD and exercises the board's IMU, battery monitor, microSD card, RGB LED, and wireless modules.

## Hardware Required

- ESP32-S3-LCD-1.47B development board

## How to Run

1. Install Arduino-ESP32 version `3.3.11`.
2. Set the sketchbook location to `examples/arduino/`, or copy `examples/arduino/libraries/` into your sketchbook `libraries` folder.
3. Select `ESP32S3 Dev Module` and set Flash Size to `16MB`, PSRAM to `OPI PSRAM`, Flash Mode to `QIO`, Partition Scheme to `16M Flash (3MB APP/9MB FATFS)`, USB Mode to `Hardware CDC and JTAG`, and CDC On Boot to `Enabled`.
4. Open `LVGL_Arduino.ino` and upload.

## Expected Result

The LCD shows the LVGL example interface while the background task updates sensor and battery readings and runs the wireless and RGB demonstrations.

## Troubleshooting

The example expects the board's onboard peripherals and can block while waiting for sensor communication.
