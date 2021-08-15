---
title: 'Gas Sensor Selection Guide'
date: 2021-07-13
---

I have been invloved with a project that required us to use gas sensors. I had to do research on these sensors to select the right sensor for our project. In this post I explain how we may select the right gas sensor for a project. There are certian points that neeed to be considered before sensor selection which includes:

1- Cost of the Sensor: How much you would like to spend on the sensor. For instance the price range of CO2 sensors is from $2.5 to hundreds of dollars.

2- Power Conumption: Gas sensors are often considered power-hungry sensors especially if we compare them to other sensors such as motion, pressure, or temperature sensors.

3- Operation Temperature: In what kind of environment are we going to deploy the sensor. For example, it would be important for sensor selection if the temperature goes below 0℃.

4- Measurement Range: What is the required measurement range for the application? For example, CO2 concentration below 1000ppm is safe for humans. However, at higher levels, around 2500 ppm, there are significant reductions in cognitive functioning, especially for tasks that require higher-level thinking. And finally, CO2 levels above 50,000ppm can cause humans to lose consciousness which can lead to death, f this occurs for long enough. Or in CO case, at sustained concentrations above 150 to 200 ppm, disorientation, unconsciousness, and death are possible. [reference1](https://learn.kaiterra.com/en/air-academy/is-carbon-dioxide-harmful-to-people) [reference2](https://www.cpsc.gov/Safety-Education/Safety-Education-Centers/Carbon-Monoxide-Information-Center/Carbon-Monoxide-Questions-and-Answers)

5- Response Time: How fast the sensor's output change according to the new gas level. For example, we need a fast response time if the target gas is so toxic to human because we do not have time to wait for the sensor to respond after 90 seconds which might be too long for some applications.

6- Lifespan: How long can we rely on the sensor's performance? Are we going to deploy the sensing system for some years or just some months?

7- Size of the Module: Depending on the technology that is used the sensor size can vary. Or some may require larger driving circuit to function.

8- Measurement Principle: The technology that is used for building the sensor which inlcudes Electrochemical, MEMS Pellistors, Infrared, Thermal Conductivity, Catalytic Pellistors, and Metal Oxide.


## CO2 Gas Sensor Selection
The goal of the project was to develop a portable sensing system to detect environmental factors predisposing to common disease and stress in dairy calves. Therefore, we needed to consider these points to select the sensor:

  - Sensor cost was important because costly sensor was not feasible for the project because we had a limit on the total cost of the device.
  
  - Sensor's response rate was not an important factor for the project since the goal was to log the average CO2 concentration over time. Measurement range was not a critical factor for this application as well.
  
  - Power consumption of the sensor was important because the system was portable and we had to power the device with a battery.

  - The facility was eqqupped with heaters, and the temperature would not go below 0℃. 

  - The sensor was about to deploy in a harsh environment. Therefore, the sensor had to be waterproof as well.

The potential CO2 options were:
  1- MH-Z14A NDIR CO2 Module or Gravity Analog Infrared CO2 Sensor
  <p align="center">
  <img width="180" height="150" src="https://user-images.githubusercontent.com/45086751/129488385-c0311048-ae0f-4949-8194-401621b754da.png">
</p> 
    2- MG-811 Electrochemical Sensor
<p align="center">
  <img width="190" height="160" src="https://user-images.githubusercontent.com/45086751/129488562-bc95f80b-2d58-4ed1-be62-d5a89cd671ee.png">
</p> 

  3- MH-Z19 NDIR CO2 Sensor Module
 <p align="center">
  <img width="190" height="160" src="https://user-images.githubusercontent.com/45086751/129488629-0e957fa7-23a9-42b8-a257-ca7284d6e87c.png">
</p> 

  4- SCD30 Nondispersive Infrared (NDIR) based CO2 sensor
 <p align="center">
  <img width="190" height="160" src="https://user-images.githubusercontent.com/45086751/129488759-943becbd-3ca0-4ecd-ae02-a960bb8c9987.png">
</p> 

  5- MH-Z16 NDIR Infrared gas module
   <p align="center">
  <img width="190" height="160" src="https://user-images.githubusercontent.com/45086751/129490123-5ddfb4b3-d0d8-4ed2-8c22-71053afa4118.png">
</p> 


| Sensor Module                     | Sensor Cost | Response Rate| Power Consumption |  Operation Temperature   | Measurement Range  | Harsh Environment
| :---:                             |    :----:   |        :---: | :----:            |         :---:            |   :---:            | :---:            |
| MH-Z14A NDIR Module               | $40         | <90s         |<430mW             |       0℃～50℃          |    0～5000 ppm      | Yes              |
| MG-811 Electrochemical Module     | $50         | <20s         |<1W                |        -20℃～50℃       |    0～10000 ppm     | No               |
| MH-Z19 NDIR Module                | $30         | <60s         |<60mW              |        0℃～50℃         |    0～5000 ppm      | No               |
| SCD30 NDIR Module                 | $60         | <20          |<63mW              |        0℃～50℃         |    0～40000 ppm     | No               |
| MH-Z16 NDIR Module                | $90         | <30          |<430mW             |        -10℃～50℃       |    0～5000 ppm      | Yes              |

Based on the project requirements, we had to deploy the sensor in a harsh environment. Therefore, we came down to two choices: 1)MH-Z14A NDIR Module 2) MH-Z16 NDIR Module. 
