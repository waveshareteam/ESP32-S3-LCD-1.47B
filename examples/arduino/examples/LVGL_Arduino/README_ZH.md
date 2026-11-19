# LVGL Arduino

[English](README.md) | [简体中文](README_ZH.md)

## 功能

在 ST7789 LCD 上运行 LVGL 界面，并演示开发板的 IMU、电池检测、MicroSD 卡、RGB 灯和无线模块。

## 硬件需求

- ESP32-S3-LCD-1.47B 开发板

## 怎么运行

1. 安装 `3.3.11` 版本 Arduino-ESP32。
2. 将项目文件夹位置设为 `examples/arduino/`，或把 `examples/arduino/libraries/` 复制到项目文件夹下的 `libraries` 文件夹。
3. 选择 `ESP32S3 Dev Module`，并设置 Flash Size 为 `16MB`、PSRAM 为 `OPI PSRAM`、Flash Mode 为 `QIO`、Partition Scheme 为 `16M Flash (3MB APP/9MB FATFS)`、USB Mode 为 `Hardware CDC and JTAG`、CDC On Boot 为 `Enabled`。
4. 打开 `LVGL_Arduino.ino` 并上传。

## 预期现象

LCD 显示 LVGL 示例界面，后台任务更新传感器和电池读数，并运行无线和 RGB 演示。

## 常见问题

示例依赖开发板板载外设，等待传感器通信时可能出现阻塞。
