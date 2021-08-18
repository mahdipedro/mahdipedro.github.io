---
title: 'Gas Sensor Selection Guide'
date: 2021-07-15
---

I have been invloved with a project that required us to use gas sensors. I had to do research on these sensors to select the right sensor for our project. In this post I explain how we may select the right gas sensor for a project. There are certian points that neeed to be considered before sensor selection which includes:

1- Cost of the Sensor: How much you would like to spend on the sensor. For instance the price range of CO2 sensors is from $2.5 to hundreds of dollars.

2- Power Conumption: Gas sensors are often considered power-hungry sensors especially if we compare them to other sensors such as motion, pressure, or temperature sensors.

3- Operation Temperature: In what kind of environment are we going to deploy the sensor. For example, it would be important for sensor selection if the temperature goes below 0℃.

4- Measurement Range: What is the required measurement range for the application? For example, CO2 concentration below 1000ppm (parts-per-million) is safe for humans. However, at higher levels, around 2500 ppm, there are significant reductions in cognitive functioning, especially for tasks that require higher-level thinking. And finally, CO2 levels above 50,000ppm can cause humans to lose consciousness which can lead to death, f this occurs for long enough. Or in CO case, at sustained concentrations above 150 to 200 ppm, disorientation, unconsciousness, and death are possible. [Reference1](https://learn.kaiterra.com/en/air-academy/is-carbon-dioxide-harmful-to-people) [Reference2](https://www.cpsc.gov/Safety-Education/Safety-Education-Centers/Carbon-Monoxide-Information-Center/Carbon-Monoxide-Questions-and-Answers)

5- Response Time: How fast the sensor's output change according to the new gas level. For example, we need a fast response time if the target gas is so toxic to human because we do not have time to wait for the sensor to respond after 90 seconds which might be too long for some applications.

6- Lifespan: How long can we rely on the sensor's performance? Are we going to deploy the sensing system for some years or just some months?

7- Size of the Module: Depending on the technology that is used the sensor size can vary. Or some may require larger driving circuit to function.

8- Measurement Principle: The technology that is used for building the sensor which inlcudes Electrochemical, MEMS Pellistors, Infrared, Thermal Conductivity, Catalytic Pellistors, and Metal Oxide.

## Gas Sensors Types and Mechanism [Reference3](https://www.akm.com/us/en/products/co2-sensor/tutorial/types-mechanism/)
There are various gas sensors mechanism and it is important to select the most suitable gas sensor according to the gas to be measured and the project. Typical gas sensor methods include a non-dispersive infrared (NDIR) method, a semiconductor method, and an electrochemical method.

  - Non-Dispersive Infrared (NDIR): A NDIR gas sensor calculates the gas concentration by using the property that gas molecules (e.g., CO2) absorb infrared rays. Therefore, a NDIR gas sensor is equipped with an infrared light emitter that emits infrared light and an infrared sensor that detects infrared light, and the performance of NDIR gas sensor varies depending on the type of the light emitter and the infrared sensor that  is installed. The NDIR method is superior to other methods  in terms of measuring gas concentrations due to its ability to detect inert gases such as CO2. This lack of detection is the weak point of other gas sensing methods. The NDIR method is capable of precision measurements regardless of whether the  gas is active or inactive, as long as it has absorbance in the infrared region. On the other hand, hydrogen and oxygen cannot be measured because they have no absorption in the infrared region due to their symmetric molecular structure. In addition, NDIR gas sensors, which are equipped with a light emitter and an infrared sensor, achieve ultra-low power consumption, ultra-fast response, and a high safety level.

  - Semiconductor: Oxygen absorbed on a metal oxide that is heated (>300°C) reacts with the gas to be detected, thereby changing the sensor resistance value. The semiconductor gas sensor uses this for gas detection. N-type metal oxides, such as tin oxide and zinc oxide, are used for the metal oxide where gas is absorbed. Since such a metal oxide can be produced by semiconductor process, semiconductor gas sensors can be mass-produced easily and therefore they are often cheaper than other types of gas sensors. At the same time, since a sensor of this method requires absorption of a gas onto a metal oxide surface, this method is unsuitable for detecting chemically stable gas molecules such as CO2 and has a disadvantage such as limitation of the measurable gases.

  - Electrochemical: Electrochemical gas sensors use oxidation-reduction reactions to measure gas concentration. The gas molecules to be detected undergo an oxidative reaction at a sensing electrode, generating ions and electrons. Ions are transferred to the counter electrode via an electrolyte and electrons are transferred to a counter electrode via an external circuit, resulting in a reduction. CO is one of the typical gases used for measurement and CO2 is generated as a result of the reaction of CO with a sensing electrode. The electrochemical sensor uses this chemical reaction. At this time, since the current flowing through the external circuit increases in proportion to the gas concentration, the gas concentration can be calculated by monitoring the current value. On the one hand, the sensors have the advantages of not being interfered by other gases and being resistant to condensation, but on the other hand, the sensors are said to have a short life span and require regular maintenance.

## Gas Sensor Selection
The goal of the project was to develop a portable sensing system to detect environmental factors predisposing to common disease and stress in dairy calves. Therefore, we needed to consider these points to select the sensor:

  - Sensor cost was important because costly sensor was not feasible for the project, and we had a limit on the total cost of the sensing device.
  
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
  <img width="190" height="150" src="https://user-images.githubusercontent.com/45086751/129488562-bc95f80b-2d58-4ed1-be62-d5a89cd671ee.png">
</p> 

  3- MH-Z19 NDIR CO2 Sensor Module
 <p align="center">
  <img width="170" height="140" src="https://user-images.githubusercontent.com/45086751/129488629-0e957fa7-23a9-42b8-a257-ca7284d6e87c.png">
</p> 

  4- SCD30 Nondispersive Infrared (NDIR) based CO2 sensor
 <p align="center">
  <img width="190" height="160" src="https://user-images.githubusercontent.com/45086751/129488759-943becbd-3ca0-4ecd-ae02-a960bb8c9987.png">
</p> 

  5- MH-Z16 NDIR Infrared CO2 Gas Module
   <p align="center">
  <img width="190" height="160" src="https://user-images.githubusercontent.com/45086751/129490123-5ddfb4b3-d0d8-4ed2-8c22-71053afa4118.png">
</p> 

  6- SCD4x Photoacoustic CO2 Gas Module
     <p align="center">
  <img width="190" height="160" src="https://user-images.githubusercontent.com/45086751/129962273-15df7600-6bfe-4b92-88d7-147ad5108e2b.png">
</p> 


| Sensor Module                     | Sensor Cost | Response Rate| Power Consumption |  Operation Temperature   | Measurement Range  | Harsh Environment
| :---:                             |    :----:   |        :---: | :----:            |         :---:            |   :---:            | :---:            |
| MH-Z14A NDIR Module               | $40         | <90s         |<430mW             |       0℃～50℃          |    0～5000 ppm      | Yes              |
| MG-811 Electrochemical Module     | $35         | <20s         |<1W                |        -20℃～50℃       |    0～10000 ppm     | No               |
| MH-Z19 NDIR Module                | $30         | <60s         |<60mW              |        0℃～50℃         |    0～5000 ppm      | No               |
| SCD30 NDIR Module                 | $60         | <20          |<63mW              |        0℃～50℃         |    0～40000 ppm     | No               |
| MH-Z16 NDIR Module                | $90         | <30          |<430mW             |        -10℃～50℃       |    0～5000 ppm      | Yes              |
| SCD4x Photoacoustic Module        | $60         | <60          |<60mW              |        -10℃～60℃       |    400～5000 ppm    | No               |

Based on the project requirements, we had to deploy the sensor in a harsh environment. Therefore, we came down to two choices: 1)MH-Z14A NDIR Module 2) MH-Z16 NDIR Module. The response rate of MH-Z16 NDIR Module is way faster than MH-Z14A NDIR Module. However, as I mentioned before, the application could tolerate slower response rate as well. The power consumption was very important factor for the project. However, the power consumption of both modules are the same! The temperature of the facility would not go below 0℃. Therefore, we should be fine with both sensors. As a result, we chose MH-Z14A NDIR Module which was cheaper (less than half) between the two! 

We also choose MQ-137 and MQ-135 for ammonia and nitrous oxide detection as well. We chose these semiconductor gas sensors because of the price limitation of the project.

  5- MH-Z16 NDIR Infrared CO2 Gas Module
   <p align="center">
  <img width="150" height="150" src="https://user-images.githubusercontent.com/45086751/129832313-ff5fe5b3-f62d-4d75-9bd3-d7c458d75c21.png">
</p> 

## Gas Sensor Calibration Methods
After selecting the right sensor for the project, now we need to calibrate it. Sensors that measure a variable value such as gas sensors require calibration. Calibration is a process of matching a sensor’s output to a known value. There are three types of calibration:
      
  - Span or 2-point calibration: It is typically performed at the factory after a gas sensor is manufactured. To perform a span calibration, a gas sensor is exposed to 2 gases, one with no target gas, and one with a known amount of the target gas. The process begins by exposing the sensor to a pure inert gas (stable and non-reactive) such as nitrogen or argon. Then the value of 0% is recorded in sensor’s EPROM memory. Next, the sensor is exposed to a known percentage of gas (often the highest level for which the sensor is rated). For instance, a 25% oxygen sensor would be calibrated with 25% oxygen. Finally, the sensor response to the 2nd known gas is recorded in the sensor’s memory. In addition, if the sensor's response is not linear, they perform 4 or more span calibration to create the response. Zero-point adjustment is also vital when dealing with gas sensors. For instance, if at 0% target gas a sensor reads 0.01% when exposed to no target gas, a negative offset of -0.01% is stored in the sensor’s memory and applied to all readings.


 ![calibration_sample](https://user-images.githubusercontent.com/45086751/129829295-5f78f627-d74a-4e90-ac4e-01cd73fe70d7.png)

  

  - Single Point Calibration: The prerequisite of this calibration is span calibration. It is useful in cases where maximum accuracy is less important than total cost. We only record one measurement of the sensor which often performed in fresh air. Fresh air contains approximately 78% nitrogen, 20.9% oxygen, 0.9% argon and 400ppm of carbon dioxide. Any gas sensor exposed to fresh air should match these readings. Once the calibration curve is stored in the sensor’s memory after span calibration, single point calibration is used like the zero-point offset. For example, if a carbon monoxide sensor uses single point calibration in fresh air, calibration process tells the sensor that there is no CO present and to save any offset to the zero point. 

  - Automatic Background Calibration (ABC): Considering an indoor air quality CO2 sensor, the theory behind ABC is that at some point each day a room is unoccupied. The CO2 level should return to 400ppm (fresh air), the same as outdoor air. By storing the lowest CO2 readings taken over several days in EPROM memory, an offset to 400ppm could be calculated, then added or subtracted from the actual CO2 readings. It is automated version of single-point calibration. And like single-point calibration, a span calibration curve was originally saved in the sensor's memory at the factory. For maximum accuracy, even devices that use ABC should be calibrated over time. The advantage of automatic background calibration is that the CO2 sensor is self-zeroing over the life of the sensor. However, it is vital that the sensor reads fresh air CO2 (400ppm) occasionally.

