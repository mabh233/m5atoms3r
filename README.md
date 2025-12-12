# M5AtomS3R Firmware / M5AtomS3R 固件

## 这是什么？ / What is this?

这是 M5AtomS3R 的固件仓库。M5AtomS3R 是一款基于 ESP32-S3 的微型开发板，由 M5Stack 制造。

This is the firmware repository for M5AtomS3R. M5AtomS3R is a compact development board based on ESP32-S3, manufactured by M5Stack.

## 技术规格 / Technical Specifications

- **芯片 / Chip**: ESP32-S3
- **固件版本 / Firmware Version**: 1.0.9 (见 version.txt / see version.txt)
- **ESP-IDF 版本 / ESP-IDF Version**: v4.4.7
- **编译日期 / Build Date**: March 5, 2024

## 文件说明 / Files Description

- `firmware.bin` - M5AtomS3R 的固件二进制文件 / Firmware binary for M5AtomS3R
- `version.txt` - 当前固件版本号 / Current firmware version number
- `README.md` - 本文档 / This documentation

## 如何使用 / How to Use

1. 下载 `firmware.bin` 文件 / Download the `firmware.bin` file
2. 使用烧录工具（如 esptool 或 M5Burner）将固件烧录到 M5AtomS3R / Use a flashing tool (such as esptool or M5Burner) to flash the firmware to M5AtomS3R
3. 重启设备 / Restart the device

### 使用 esptool 烧录示例 / Flashing Example with esptool

```bash
# 完整固件烧录（从地址 0x0 开始）/ Flash complete firmware (starting from address 0x0)
esptool.py --chip esp32s3 --port /dev/ttyUSB0 write_flash 0x0 firmware.bin

# 或者使用 M5Burner 图形化工具 / Or use M5Burner GUI tool
```

> 注意：根据固件类型，烧录地址可能不同。如遇到问题，请参考 M5Stack 官方文档。
> 
> Note: The flash address may vary depending on the firmware type. Please refer to M5Stack official documentation if you encounter issues.

## 关于 M5AtomS3R / About M5AtomS3R

M5AtomS3R 是一款小巧的物联网开发板，适用于各种嵌入式项目和原型开发。

M5AtomS3R is a compact IoT development board suitable for various embedded projects and prototyping.

## 许可证 / License

本项目的许可证信息尚未明确指定。请联系项目维护者了解使用条款。

The license for this project is not explicitly specified. Please contact the project maintainer for usage terms.