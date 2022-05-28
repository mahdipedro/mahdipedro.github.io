---
title: 'Storing RGB and Thermal Data Using ESP32-CAM Module'
date: 2022-05-01
---

In [this post](https://github.com/mahdipedro/ESP32-CAM-I2C-sensor) I explained how you could get thermal and RGB data using ESP32-CAM and MLX90640 modules. The code will continuously collect RGB and thermal camera data and store them on an SD card. You can also find the schematic of the circuit. The firmware will sample data at about 3 fps for RGB and thermal modules. You can modify this code to interface ESP32-CAM with any device that supports I2C and include that in your project.
