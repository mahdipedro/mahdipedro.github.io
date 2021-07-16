---
title: 'Handling Power Hungry Sensors in a Low-Power Project'
date: 2021-07-13
---

In [this](https://github.com/mahdipedro/Handling-Power-Hungry-Sensors-in-a-Low-Power-Project) article I explained how one can use 5V power-hungry sensors via 3.3V microcontroller. There are still several sensors that need to be powered by 5V power supply. However, more recent development boards are eqquiped with 3.3V microcontrollers. As a result, we need to address some serious challenges. Challenges include:

1- How to utilize 3.7V Lipo battery for a 5V sensor.

2- How to control energy consumption of the sensors by turning them on and off periodically.

3- How to read the analog output of a 5V sensor with a 3.3V microcontroller. 

4- In what condition we can power a sensor through one of the microcontroller's pin.

