<h1 align="center">🔌 ATWALLX</h1>

A professional, feature-rich firmware for smart relay systems built on **ESP8266 / ESP32 / ESP8285**, designed to deliver seamless control, automation, and real-time monitoring for smart home and industrial applications.



- ✅ MQTT Control (JSON-based)
- 🕒 Weekly Schedule System
- ⏳ Delayed ON/OFF actions
- 🧲 Sensor-triggered relay switching
- 🧠 EEPROM-based state saving
- 📶 OTA (Over-the-Air) Updates
----
### 📥 Download the App

| Platform | Link |
|----------|------|
| 📱 Android | [Download](https://github.com/ARDUTECH0/smart-home/raw/refs/heads/main/app-release.apk) |


> 🔑 Requires device to be connected to Wi-Fi and MQTT broker correctly.

---

## 🧮 Relay & Button Pin Mapping

| Relay Index | Relay Pin | Button Pin |
|-------------|-----------|------------|
| 0           | D0        | D2         |
| 1           | D1        | D3         |

> You can press each button to toggle the corresponding relay manually. Button logic includes debounce handling.

---
## 📥 Download Binary Firmware

> Choose the right firmware for your board and flash it using the method below:

| Platform | Firmware Link |
|----------|----------------|
| ESP8266  | [Download ESP8266 Firmware](https://github.com/YourUsername/smart-relay-scheduler/releases/download/v1.0.4/firmware_esp8266.bin) |

---

## 🚀 Flashing the Firmware

### 1. Using ESPHome-Flasher (GUI)
- Download `.bin` file
- Connect your board via USB
- Select COM Port and `.bin` file
- Click **Flash**

### 2. Using `esptool.py` (CLI)
```bash
# ESP8266
esptool.py --port COM3 write_flash 0x0 firmware_esp8266.bin

# ESP32
esptool.py --chip esp32 --port COM3 write_flash -z 0x1000 firmware_esp32.bin
```
---

## 📞 Contact & Support

Need help or have a custom integration request?

Feel free to contact us:

- 💬 WhatsApp: [+201096448029](https://wa.me/201096448029)

We're happy to help with:
- Integration support
- Feature requests
- Custom firmware
- Commercial deployments

