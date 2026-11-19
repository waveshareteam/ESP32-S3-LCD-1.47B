# Firmware

[English](README.md) | [简体中文](README_ZH.md)

Ready-to-flash firmware tested on the ESP32-S3-LCD-1.47B board. The image is a merged factory image flashed at `0x0`.

| File | Purpose |
| --- | --- |
| [`ESP32-S3-LCD-1.47B_FactoryOnly_20260827.bin`](ESP32-S3-LCD-1.47B_FactoryOnly_20260827.bin) | Factory recovery firmware dated 2026-08-27 |

This image was verified on the corresponding product with Flash Download Tool. SHA-256: `23E62D8F46D2A9B060DA73FA6F47FC6AF1C6FCA4B0CA8FC82E4E3E533615BFB7`.

Flash with esptool:

```bash
python -m pip install esptool
esptool.py --chip esp32s3 --port <PORT> erase_flash
esptool.py --chip esp32s3 --port <PORT> write_flash 0x0 ESP32-S3-LCD-1.47B_FactoryOnly_20260827.bin
```
