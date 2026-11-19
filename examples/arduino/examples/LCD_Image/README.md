# LCD Image

[English](README.md) | [简体中文](README_ZH.md)

## What It Does

Displays PNG images from a microSD card on the ST7789 LCD. Press the BOOT button to switch between images.

## Hardware Required

- ESP32-S3-LCD-1.47B development board
- FAT32 microSD card with PNG files copied from [`SD Card File`](SD%20Card%20File/)

## How to Run

1. Install Arduino-ESP32 version `3.3.11`.
2. Set the sketchbook location to `examples/arduino/`, or copy `examples/arduino/libraries/` into your sketchbook `libraries` folder.
3. Select `ESP32S3 Dev Module` and set Flash Size to `16MB`, PSRAM to `OPI PSRAM`, Flash Mode to `QIO`, Partition Scheme to `16M Flash (3MB APP/9MB FATFS)`, USB Mode to `Hardware CDC and JTAG`, and CDC On Boot to `Enabled`.
4. Copy the PNG files to a FAT32 microSD card, insert it, open `LCD_Image.ino`, and upload.

## Expected Result

The board initializes the LCD and microSD card, then displays the PNG images. The BOOT button changes the selected image.

## Troubleshooting

Use a FAT32 card and keep the supplied six-wire SD pin assignment.
