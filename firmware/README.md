# Firmware

[English](README.md) | [简体中文](README_ZH.md)

The following firmware is a merged image for the ESP32-C5 Wi-Fi coprocessor, tested on the board and flashed at `0x0`. It uses Espressif's `esp_hosted` component v3.1.0.

| File | Purpose |
| --- | --- |
| [ESP32-P4-WIFI6-Touch-LCD-4.05_ESP32-C5-Slave_20261113.bin](ESP32-P4-WIFI6-Touch-LCD-4.05_ESP32-C5-Slave_20261113.bin) | ESP32-C5 coprocessor factory firmware |

Flash the ESP32-C5 using its programming interface:

```bash
esptool.py --chip esp32c5 --port <PORT> erase_flash
esptool.py --chip esp32c5 --port <PORT> write_flash 0x0 ESP32-P4-WIFI6-Touch-LCD-4.05_ESP32-C5-Slave_20261113.bin
```
