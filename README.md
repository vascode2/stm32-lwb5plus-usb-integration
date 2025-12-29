# LWB5+ USB Wi-Fi Integration on STM32H747I-DISCO

**A reference integration for adding 802.11ac Wi-Fi & Bluetooth 5.0 to the STM32H747 Discovery board via USB High-Speed Host.**

![Project Status](https://img.shields.io/badge/Status-Finished-success)
![Hardware](https://img.shields.io/badge/Hardware-STM32H747I--DISCO-blue)
![Connectivity](https://img.shields.io/badge/Module-LWB5%2B_USB-orange)

## 📖 Overview
This project demonstrates how to integrate the **Ezurio (Laird Connectivity) LWB5+ USB Dongle** with the **STM32H747I-DISCO** board. Unlike standard SDIO integrations, this project leverages the **USB OTG (High Speed)** interface to drive the Wi-Fi module, enabling high-throughput connectivity on platforms where SDIO is unavailable or reserved.

The repository includes a complete application note and source code for two distinct reference applications:
1.  **Wi-Fi Scanner (UART):** Initializes the USB Host stack and outputs detected networks to a serial terminal.
2.  **Wi-Fi Dashboard (LCD):** Demonstrates full integration by rendering scan results directly on the STM32 discovery board's touch display.

## 🛠️ Tech Stack
* **MCU:** STM32H747XI (Dual Core Cortex-M7 + M4)
* **Wireless:** Sterling LWB5+ (Cypress/Infineon CYW4373 chipset)
* **Interface:** USB 2.0 High Speed (Host Mode)
* **RTOS:** FreeRTOS
* **IDE:** STM32CubeIDE / STM32CubeMX

## 📂 Documentation
The full step-by-step application note and source code are available in the `docs` folder:

### [👉 Read the Full Integration Guide](docs/LWB5p-USB-STM32H747I-DISCO-docs.md)

* **Hardware Setup:** Connection diagrams for the USB OTG adapter.
* **Project 1 - Headless Scanning:** Building the FreeRTOS project to pipe scan data to a PC terminal.
* **Project 2 - Graphic Display:** Configuring the board's built-in screen to visualize real-time Wi-Fi scan results.

## 📦 Downloads
* **Source Code:** [stm32_segger_usb.1.6.0.zip](docs/download/stm32_segger_usb.1.6.0.zip) (Located in `docs/download`)

