# ESP32-S3-LCD-1.47B Test

[English](README.md) | [简体中文](README_ZH.md)

## 功能

运行 LVGL 界面，并演示 LCD、MicroSD 卡、QMI8658 IMU、电池检测、RGB 灯和无线模块。

## 硬件需求

- ESP32-S3-LCD-1.47B 开发板

## 怎么运行

```bash
idf.py set-target esp32s3 build flash monitor
```

## 预期现象

LCD 显示 LVGL 示例界面，后台任务更新 IMU 和电池读数，同时运行 RGB 和无线演示。

## 常见问题

项目要求开发板使用 16 MB Flash 和 8 MB PSRAM，并依赖板载外设。
