# Ultimate Guide to Raspberry Pi : Tips, Tricks and Hacks

# 🐍 Pi Ultimate Guide  
*A hands-on collection of Raspberry Pi GPIO & camera mini-projects in pure Python*

> **Fork note**  
> This is a fork of the original work by **[@leeassam](https://github.com/leeassam/pi-ultimate-guide)**.  
> I (Hari Aditya) have kept the code unchanged while refreshing the documentation and adding clearer setup steps.

---

## What you’ll find here

| Folder | Mini-project | What it shows you |
| ------ | ------------ | ----------------- |
| **[`blink_led`](blink_led/)** | Blink an LED | GPIO pin numbering, output mode, cleanup |
| **[`button_press`](button_press/)** | Read a push-button | Pull-up / pull-down resistors, debouncing |
| **[`button_press_led`](button_press_led/)** | Button-controlled LED | Combining input & output, event callbacks |
| **[`pir_sensor`](pir_sensor/)** | Detect motion | Reading HC-SR501 PIR sensor data |
| **[`pir_sensor_alarm`](pir_sensor_alarm/)** | Motion alarm | Triggering a buzzer / LED on motion |
| **[`cameras`](cameras/)** | Capture photos & video | PiCamera vs. libcamera, image formats |
| **[`setup_headless_mode`](setup_headless_mode/)** | Headless Pi setup | Enable SSH, set Wi-Fi, no HDMI required |

Each folder contains a single, well-commented Python script that can be run standalone.

---

## Hardware you’ll need

* Raspberry Pi (3/4/5 or Zero W) with Raspbian/Raspberry Pi OS  
* Solderless breadboard & jumper wires  
* **Basic kit parts**  
  * 5 mm LED + 330 Ω resistor  
  * Tactile push-button  
  * HC-SR501 PIR motion sensor  
  * Active buzzer (for alarm example)  
* **Optional**  
  * PiCamera v2 or HQ Camera for `cameras` demo

---

## Quick-start 🏁

1. **Enable GPIO & camera**  
   ```bash
   sudo raspi-config
   # ‣ Interface Options → SSH, I²C, Camera (enable)
