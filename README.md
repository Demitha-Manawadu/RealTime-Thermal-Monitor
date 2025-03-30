# 📷 Realtime Thermal Monitor

![Thermal View](https://img.shields.io/badge/built%20with-Python%203-blue)
![Platform](https://img.shields.io/badge/platform-Raspberry%20Pi-lightgrey)

A Python-based thermal imaging and hotspot detection system using the **AMG8833 IR thermal sensor** and **OpenCV**. This project displays real-time thermal data on-screen, detects high temperature regions, and classifies environmental conditions using live thermal analysis.

---

## 🚀 Features

- 🔥 Live thermal visualization (color-coded heatmap)
- 📏 Real-time hotspot detection with contour bounding
- 📊 Average temperature computation and classification
- 🎨 OpenCV GUI with smooth interpolation and JET colormap
- 🧼 Threshold filtering to reduce false alerts (e.g., hands)
- 📡 Designed for Raspberry Pi with I2C interface

---

## 📸 Demo

<img src="https://user-images.githubusercontent.com/your-screenshot.png" width="480"/>

> *A real-time thermal view with temperature overlay and hotspot detection*

---

## 🧰 Hardware Requirements

- [Adafruit AMG8833 8x8 Thermal Camera Sensor](https://www.adafruit.com/product/3538)
- Raspberry Pi (any model with I2C support)
- I²C enabled via `raspi-config`
- USB display / HDMI monitor
- 3D-printed or custom **enclosure** (planned)

---

## 🛠️ Software Setup

1. **Enable I2C on Raspberry Pi**
   ```bash
   sudo raspi-config
   # Interface Options → I2C → Enable
   sudo reboot
