# 固件

[English](README.md) | [简体中文](README_ZH.md)

这是已经在 ESP32-S3-LCD-1.47B 开发板上完成验证的可烧录固件。该文件是从 `0x0` 烧录的合并出厂镜像。

| 文件 | 用途 |
| --- | --- |
| [`ESP32-S3-LCD-1.47B_FactoryOnly_20260827.bin`](ESP32-S3-LCD-1.47B_FactoryOnly_20260827.bin) | 2026-08-27 出厂恢复固件 |

本镜像已经使用 Flash Download Tool 在对应产品上完成实物验证。SHA-256：`23E62D8F46D2A9B060DA73FA6F47FC6AF1C6FCA4B0CA8FC82E4E3E533615BFB7`。

使用 esptool 烧录：

```bash
python -m pip install esptool
esptool.py --chip esp32s3 --port <PORT> erase_flash
esptool.py --chip esp32s3 --port <PORT> write_flash 0x0 ESP32-S3-LCD-1.47B_FactoryOnly_20260827.bin
```
