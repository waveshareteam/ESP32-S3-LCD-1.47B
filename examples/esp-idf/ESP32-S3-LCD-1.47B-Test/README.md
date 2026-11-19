# ESP32-S3-LCD-1.47B Test

[English](README.md) | [简体中文](README_ZH.md)

## What It Does

Runs an LVGL interface and demonstrates the LCD, microSD card, QMI8658 IMU, battery monitor, RGB LED, and wireless modules.

## Hardware Required

- ESP32-S3-LCD-1.47B development board

## How to Run

```bash
idf.py set-target esp32s3 build flash monitor
```

## Expected Result

The LCD shows the LVGL example interface. The background task updates the IMU and battery readings while the RGB and wireless demonstrations run.

## Troubleshooting

The project expects the board's onboard peripherals and a 16 MB Flash device with 8 MB PSRAM.
