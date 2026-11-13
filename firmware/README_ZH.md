# 固件

[English](README.md) | [简体中文](README_ZH.md)

以下固件是 ESP32-C5 Wi-Fi 从机的合并镜像，已在开发板上实测，从 `0x0` 地址烧录。

| 文件 | 用途 |
| --- | --- |
| [ESP32-P4-WIFI6-Touch-LCD-4.05_ESP32-C5-Slave_20261113.bin](ESP32-P4-WIFI6-Touch-LCD-4.05_ESP32-C5-Slave_20261113.bin) | ESP32-C5 从机出厂固件 |

通过 ESP32-C5 的烧录接口烧录：

```bash
esptool.py --chip esp32c5 --port <PORT> erase_flash
esptool.py --chip esp32c5 --port <PORT> write_flash 0x0 ESP32-P4-WIFI6-Touch-LCD-4.05_ESP32-C5-Slave_20261113.bin
```
