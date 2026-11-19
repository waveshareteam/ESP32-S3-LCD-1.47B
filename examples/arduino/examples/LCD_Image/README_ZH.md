# LCD Image

[English](README.md) | [简体中文](README_ZH.md)

## 功能

从 MicroSD 卡读取 PNG 图片并显示在 ST7789 LCD 上。按下 BOOT 按钮可以切换图片。

## 硬件需求

- ESP32-S3-LCD-1.47B 开发板
- FAT32 MicroSD 卡，并复制 [`SD Card File`](SD%20Card%20File/) 中的 PNG 文件

## 怎么运行

1. 安装 `3.3.11` 版本 Arduino-ESP32。
2. 将项目文件夹位置设为 `examples/arduino/`，或把 `examples/arduino/libraries/` 复制到项目文件夹下的 `libraries` 文件夹。
3. 选择 `ESP32S3 Dev Module`，并设置 Flash Size 为 `16MB`、PSRAM 为 `OPI PSRAM`、Flash Mode 为 `QIO`、Partition Scheme 为 `16M Flash (3MB APP/9MB FATFS)`、USB Mode 为 `Hardware CDC and JTAG`、CDC On Boot 为 `Enabled`。
4. 将 PNG 文件复制到 FAT32 MicroSD 卡并插入开发板，打开 `LCD_Image.ino` 后上传。

## 预期现象

开发板初始化 LCD 和 MicroSD 卡后显示 PNG 图片，按下 BOOT 按钮可切换当前图片。

## 常见问题

请使用 FAT32 卡，并保持示例中提供的六线 SD 引脚配置。
