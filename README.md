# 🔌 Smart Relay Scheduler Firmware

Firmware for a professional **Smart Relay System** based on ESP8266/ESP32 that supports:

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
| 📱 Android | [Download from Play Store](https://play.google.com/store/apps/details?id=com.yourcompany.smarthome) |


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

---
