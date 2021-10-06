---
title: 'Gas Sensor Selection Guide'
date: 2021-07-15
---

I have been involved with a project that required us to use multiple gas sensors. I had to do research on these sensors to select the right sensors for our project. In addition gas sensors need to be calibrated as well. In this article, I explain how we may select the right gas sensors for a project and the potential ways to calibrate a gas sensor. There are certain points that need to be considered before sensor selection which includes:

1- Cost of the Sensor: How much you can spend on the sensor. For instance, the price range of CO2 sensors are from $2.5 to hundreds of dollars.

2- Power Consumption: Gas sensors are often considered power-hungry sensors especially if we compare them to other sensors such as motion, pressure, or temperature sensors.

3- Operation Temperature: In what kind of environment are we going to deploy the sensor. For example, it would be important for sensor selection if the temperature goes below 0℃.

4- Measurement Range: What is the required measurement range for the application? For example, CO2 concentration below 1000ppm (parts-per-million) is safe for humans. However, at higher levels, around 2500 ppm, there are significant reductions in cognitive functioning, especially for tasks that require higher-level thinking. And finally, CO2 levels above 50,000ppm can cause humans to lose consciousness which can lead to death, if this occurs for long enough. Or in CO case, at sustained concentrations above 150 to 200 ppm, disorientation, unconsciousness, and death are possible. [Reference](https://learn.kaiterra.com/en/air-academy/is-carbon-dioxide-harmful-to-people) [Reference](https://www.cpsc.gov/Safety-Education/Safety-Education-Centers/Carbon-Monoxide-Information-Center/Carbon-Monoxide-Questions-and-Answers)

5- Response Time: How fast the sensor's output changes according to the new gas level. For example, we need a fast response time if the target gas is so toxic to human because we do not have time to wait for the sensor to respond after 90 seconds which might be too long for some applications.

6- Lifespan: How long can we rely on the sensor's performance? Are we going to deploy the sensing system for some years or just some months?

7- Size of the Module: Depending on the technology that is used the sensor size can vary. Or some may require larger driver circuit to function.

8- Measurement Principle: The technology that is used for building the sensor which includes Electrochemical, MEMS Pellistors, Infrared, Thermal Conductivity, Catalytic Pellistors, and Metal Oxide.

## Gas Sensors Types and Mechanism [Reference](https://www.akm.com/us/en/products/co2-sensor/tutorial/types-mechanism/)
There are various gas sensors mechanism, and it is important to select the most suitable gas sensor according to the gas to be measured and the project. Typical gas sensor methods include a non-dispersive infrared (NDIR) method, a semiconductor method, and an electrochemical method.

  - Non-Dispersive Infrared (NDIR): A NDIR gas sensor calculates the gas concentration by using the property that gas molecules (e.g., CO2) absorb infrared rays. Therefore, a NDIR gas sensor is equipped with an infrared light emitter that emits infrared light and an infrared sensor that detects infrared light, and the performance of NDIR gas sensor varies depending on the type of the light emitter and the infrared sensor that is installed. The NDIR method is superior to other methods in terms of measuring gas concentrations due to its ability to detect inert gases such as CO2. This lack of detection is the weak point of other gas sensing methods. The NDIR method is capable of precision measurements regardless of whether the  gas is active or inactive, as long as it has absorbance in the infrared region. On the other hand, <mark>hydrogen and oxygen </mark>cannot be measured because they have no absorption in the infrared region due to their symmetric molecular structure. In addition, NDIR gas sensors, which are equipped with a light emitter and an infrared sensor, achieve ultra-low power consumption, ultra-fast response, and a high safety level.

  - Semiconductor: Oxygen absorbed on a metal oxide that is heated (>300°C) reacts with the gas to be detected, thereby changing the sensor resistance value. The semiconductor gas sensor uses this for gas detection. N-type metal oxides, such as tin oxide and zinc oxide, are used for the metal oxide where gas is absorbed. Since such a metal oxide can be produced by semiconductor process, semiconductor gas sensors can be mass-produced easily and therefore they are often cheaper than other types of gas sensors. At the same time, since a sensor of this method requires absorption of a gas onto a metal oxide surface, this method is unsuitable for detecting <mark>chemically stable gas</mark> molecules such as CO2 and has a disadvantage such as limitation of the measurable gases.

  - Electrochemical: Electrochemical gas sensors use oxidation-reduction reactions to measure gas concentration. The gas molecules to be detected undergo an oxidative reaction at a sensing electrode, generating ions and electrons. Ions are transferred to the counter electrode via an electrolyte and electrons are transferred to a counter electrode via an external circuit, resulting in a reduction. CO is one of the typical gases used for measurement and CO2 is generated as a result of the reaction of CO with a sensing electrode. The electrochemical sensor uses this chemical reaction. At this time, since the current flowing through the external circuit increases in proportion to the gas concentration, the gas concentration can be calculated by monitoring the current value. On the one hand, the sensors have the advantages of not being interfered by other gases and being resistant to condensation, but on the other hand, the sensors are said to have a short life span and require regular maintenance.
  
  - Photoacoustic Technology: Photoacoustic spectroscopy is the measurement of the effect of absorbed electromagnetic energy (particularly of light) on matter by means of acoustic detection. This low-power technology is currently used for only CO2 sensors. Sensors that use this technology are small in size. Narrow-band light matching the absorption bands of CO2 molecules is emitted into a predominantly closed measuring cell. CO2 molecules in the measuring cell absorb a part of the irradiated light, whereas other molecules cannot contribute to absorption due to the spectrum of the emitted light. The more molecules present in the measuring cell, the larger the absorbed energy. The absorbed energy of the CO2 - molecules excites mainly molecular vibrations, which results in an increased translational energy of the molecules and, due to the closed measuring cell, in an increase of pressure in the cell. A modulation of the light source causes a periodic pressure change in the measuring cell, which can be measured with a microphone. The signal of the microphone thus serves as a measure of the number of CO2 molecules present in the measuring cell and can be used to calculate the CO2 concentration. [Reference](https://www.sensirion.com/en/environmental-sensors/carbon-dioxide-sensors/carbon-dioxide-sensor-scd4x/)
  
  - Optical Sensors: Optical sensors are based on the principle of fluorescence quenching by the target gas. They rely on the use of a light source, a light detector, and a luminescent material that reacts to light. 
  
  - MEMS (Micro Electro Mechanical System) 



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
  <img width="210" height="160" src="https://user-images.githubusercontent.com/45086751/129488562-bc95f80b-2d58-4ed1-be62-d5a89cd671ee.png">
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
  <img width="90" height="90" src="https://user-images.githubusercontent.com/45086751/129962273-15df7600-6bfe-4b92-88d7-147ad5108e2b.png">
</p> 


| Sensor Module                     | Sensor Cost | Response Rate| Power Consumption |  Operation Temperature   | Measurement Range  | Harsh Environment| Accuracy            |
| :---:                             |    :----:   |        :---: | :----:            |         :---:            |   :---:            | :---:            |:---:                |
| MH-Z14A NDIR Module               | $40         | <90s         |<430mW             |       0℃～50℃          |    0～5000 ppm      | Yes              |±(100ppm+ 6%) |
| MG-811 Electrochemical Module     | $35         | <20s         |<1W                |        -20℃～50℃       |    0～10000 ppm     | No               |±100ppm@400ppm|
| MH-Z19 NDIR Module                | $30         | <60s         |<60mW              |        0℃～50℃         |    0～5000 ppm      | No               |± (50ppm+5%) |
| SCD30 NDIR Module                 | $60         | <20          |<63mW              |        0℃～50℃         |    0～40000 ppm     | No               |±(30ppm+3%)|
| MH-Z16 NDIR Module                | $90         | <30          |<430mW             |        -10℃～50℃       |    0～5000 ppm      | Yes              |±(50ppm+5%)|
| SCD4x Photoacoustic Module        | $60         | <60          |<60mW              |        -10℃～60℃       |    400～5000 ppm    | No               |±(40 ppm + 5%) |

Based on the project requirements, we had to deploy the sensor in a harsh environment. Therefore, we came down to two choices: 1) MH-Z14A NDIR Module 2) MH-Z16 NDIR Module. The response rate of MH-Z16 NDIR Module is way faster than MH-Z14A NDIR Module. However, as I mentioned before, the application could tolerate slower response rate as well. The power consumption was very important factor for the project. However, the power consumption of both modules are equal! The temperature of the facility would not go below 0℃. Therefore, we should be fine with both sensors. As a result, we chose MH-Z14A NDIR Module which was cheaper (less than half) between the two! 

We also choose MQ-137 and MQ-135 for ammonia and nitrous oxide detection respectively. We chose these semiconductor gas sensors because of the price limitation of the project.

   <p align="center">
  <img width="150" height="150" src="https://user-images.githubusercontent.com/45086751/129832313-ff5fe5b3-f62d-4d75-9bd3-d7c458d75c21.png">
</p> 

| Sensor Module                     | Sensor Cost | Response Rate| Power Consumption |  Operation Temperature   | Measurement Range  | Accuracy |
| :---:                             |    :----:   |        :---: | :----:            |         :---:            |   :---:            | :---:    | 
| MQ-137 Ammonia Gas Sensor         | $40         | <15s         |<900mW             |       -10℃～45℃        |    5～500 ppm       | 10%     |
| MQ-135 Gas Sensor for Air Quality | $3          | <15s         |<950mW             |        -10℃～50℃       |    10～1000 ppm     | NA |

## Gas Sensor Calibration Methods
After selecting the right sensor for the project, now we need to calibrate it. Sensors that measure a variable value such as gas sensors require calibration. Calibration is a process of matching a sensor’s output to a known value. There are three types of calibration:
      
  - Span or 2-point calibration: It is typically performed at the factory after a gas sensor is manufactured. To perform a span calibration, a gas sensor is exposed to 2 gases, one with no target gas, and one with a known amount of the target gas. The process begins by exposing the sensor to a pure inert gas (stable and non-reactive) such as nitrogen or argon. Then the value of 0% is recorded in sensor’s EPROM memory. Next, the sensor is exposed to a known percentage of gas (often the highest level for which the sensor is rated). For instance, a 25% oxygen sensor would be calibrated with 25% oxygen. Finally, the sensor response to the 2nd known gas is recorded in the sensor’s memory. In addition, if the sensor's response is not linear, they perform 4 or more span calibration to create the response. Zero-point adjustment is also vital when dealing with gas sensors. For instance, if at 0% target gas a sensor reads 0.01% when exposed to no target gas, a negative offset of -0.01% is stored in the sensor’s memory and applied to all readings.

 ![calibration_sample](https://user-images.githubusercontent.com/45086751/129829295-5f78f627-d74a-4e90-ac4e-01cd73fe70d7.png)

  - Single Point Calibration: The prerequisite of this calibration is span calibration. It is useful in cases where maximum accuracy is less important than total cost. We only record one measurement of the sensor which often performed in fresh air. Fresh air contains approximately 78% nitrogen, 20.9% oxygen, 0.9% argon and 400ppm of carbon dioxide. Any gas sensor exposed to fresh air should match these readings. Once the calibration curve is stored in the sensor’s memory after span calibration, single point calibration is used like the zero-point offset. For example, if a carbon monoxide sensor uses single point calibration in fresh air, calibration process tells the sensor that there is no CO present and to save any offset to the zero point. 

  - Automatic Background Calibration (ABC): Considering an indoor air quality CO2 sensor, the theory behind ABC is that at some point each day a room is unoccupied. The CO2 level should return to 400ppm (fresh air), the same as outdoor air. By storing the lowest CO2 readings taken over several days in EPROM memory, an offset to 400ppm could be calculated, then added or subtracted from the actual CO2 readings. It is automated version of single-point calibration. And like single-point calibration, a span calibration curve was originally saved in the sensor's memory at the factory. For maximum accuracy, even devices that use ABC should be calibrated over time. The advantage of automatic background calibration is that the CO2 sensor is self-zeroing over the life of the sensor. However, it is vital that the sensor reads fresh air CO2 (400ppm) occasionally.
  
  - ***Calibration Using AI: Another possible method for a gas sensor calibration is using AI/ML. This method requires extensive data collection as well which might not be feasible for smaller projects. We can define some features such as room temperature, sensor age, room volume, amount of non-target gas in the room, and any other factor that might affect the sensor's output. Then we can start collecting data in different scenarios such as variable amount of target gass, variable room sizes, different sensor ages, etc. At the same time, we also keep track of the ground truth values of the target gas by using multiple industrial sensors. Ultimately, we create a dataset of these experiments with all the features and labels. Then we train a regression model for a sensor type which can be used to predict sensor's behavior in different settings. The data set of the extensive data collection will be similar to the following table.***

| Sensor Output                     | Room Size   | Sensor Age   | Temperature       |  Humidity                | Amount of non-target gas| True Target Gas Value|
| :---:                             |    :----:   |        :---: | :----:            |         :---:            |   :---:                 |   :---:              |
| X ppm                             | Y m^3       | Z months     |T℃                |       H%                 |    N ppm                |    GT ppm            |


## Calibration Phase of the Project

  -  MH-Z14A NDIR Calibration: The sensor has been calibrated in the factory and the sensor's response to CO2 concentration is reported as:
  
    <p align="center">
    <img width="360" height="310" src="https://user-images.githubusercontent.com/45086751/130175398-712a9a1d-9d91-4888-99cc-2ba7e50e2066.png">
    </p> 


  When the CO2 sensor supplies with 5V, it generates 0.4~ 2V analog signal corresponding to 0~5000 ppm; And when the sensor finds faults during the self-checking process, it will generate 0V. Considering the linear behavior of the sensor, we calibrate the sensor using the single point calibration method. Fresh air contains approximately 400ppm od CO2 and we confirmed it using an industrial grade digital CO2 sensor. The sensor output while in fresh air (400 ppm which is confirmed by the digital carbon dioxide sensor) was about 437 ppm. As a result, we use the offset of -37ppm for the sensors readings. For instance, when the sensor output shows 550ppm of CO2 concentration, the true value would be 513ppm. The sensor was going to be used in an outdoor facility. Therefore, we can assume there would be times when the sensor shows fresh air CO2 concentration (400ppm). This means we can use ABC method to calibrate the sensor automatically. As a result, we use the 10 lowest values of the sensor during each day and take the average of them. We use the average value to determine the sensor's response to 400ppm of CO2 which ultimately helps us to set the right offset.

  - MQ-137 Calibration:  The sensor has been calibrated in the factory and the sensor's response to NH3 concentration is reported in the sensor's datasheet:


  <p align="center">
  <img width="360" height="310" src="https://user-images.githubusercontent.com/45086751/136251884-67f7f2f7-c163-487d-ad4f-e8057c09ecdb.JPG">
  </p> 


   Rs is the resistance of the sensor in target gas (NH3) with different concentration; And R0 is the resistance of the sensor in fresh air. As a result, to calibrate the sensor, we need to find out the value of R0. The below circuit is the basic driver circuit for MQ-137.The sensor requires two voltage inputs including heater voltage (VH) and circuit voltage (VC). VH is used to supply standard working temperature to the sensor, and it can adopt DC or AC power, while VRL is the voltage of load resistance RL which is in series
with sensor. Vc supplies the detect voltage to load resistance RL and it requires DC power. RL is adjustable and we set it to 47KΩ. As a result, we will be able to use the sensor response graph of the datasheet, because the graph is based on RL of 47KΩ.

  <p align="center">
  <img width="360" height="310" src="https://user-images.githubusercontent.com/45086751/130175216-d8178af8-7c49-4655-9035-31765a4201fe.JPG">
  </p> 



  We developed the sensor drvier as mentioned above and we connect the VRL to arduio A0 pin. Then we move on to develop the firmware to determine the value of R0. 
  
  ```
  void setup() {
  Serial.begin(9600); //Baud rate 
}
 
void loop() { 
  float VRL; //Variable for sensor's output 
  float RS_air; //Variable for sensor resistance
  float R0; //Variable for R0
  float sensorValue; //Define variable for analog readings 
  sensorValue = analogRead(A0); //Read analog voltage
  VRL = sensorValue*(3.3/1023.0);
  RS_air = ((3.3*47.0)/VRL)-47.0; //Calculate RS in fresh air which determined from Ohm’s Law and by considering the fact that Rs and RL are in series (IRL = VC / (RS+RL))
  R0 = RS_air/3.6; //Calculate R0. 3.6 is extracted from the graph in the datasheet. Rs/R0 is constant for fresh air and it is about 3.6 which helps us to determine R0!
 
  Serial.print("R0 = "); //Display "R0"
  Serial.println(R0); //Display value of R0 
  delay(1000); //Wait 1 second 
}

  ```


Then we used the above code for 12 hours because of the sensor pre-heat and waiting for R0 value to become stable. Value of R0 in fresh air was 37KΩ for our sensor which was required for the NH3 sensor calibration. Then we continue working with the sensor using Rs/R0 with R0 as a constant value of 37KΩ. According to the datasheet, the relation between Rs/Ro and PPM is logarithmic which is log(y) = m*log(x) + b.

X is ppm value and y is Rs/R0.
m is the slope of the line and to determine the value of the slope, we select two points on the NH3 line including (40,1), and (100,0.8). 
Then we have:
m = (log(y2) - log(y1)) / (log(x2) - log(x1)) which will be equal to -0.244.
b is the Y intercept of the line which can be calculated by using any point on the NH3 line: b = log(y) - mlog(x) --> b = -0.096 + 0.244*2 = 0.389.

Ultimately, we have: x = 10 ^ [(log(Rs/R0) - b) / m]. Note that all the values except Rs are constant and we need to compute this for new values of Rs to get the ppm values of the target gas. Then we program the microcontroller to read the ppm level of ammonia gas using the below code.


```
#define RL 47  //The value of RL which was set to 47K according to the datasheet
#define m -0.244 //Slope of the NH3 line
#define b 0.389 //Y intercept of the NH3 line
#define Ro 37 //Resistance of the sensor while in fresh air

void setup() {
  Serial.begin(9600);
}

void loop() {
  
  float VRL; //Voltage drop across MQ137 sensor
  float Rs; //Sensor resistance according to gas concentration 
   
  VRL = analogRead(A0)*(3.3/1023.0); //Measure the voltage from A0 pin and convert to 0-3.3V
  Rs = ((3.3*RL)/VRL)-RL; //Equation according to Ohm law to compute Rs value
  float ratio = Rs/Ro;  // find ratio of Rs/Ro
 
  float ppm = pow(10, ((log10(ratio)-b)/m)); //use the above formula to compute the value of gas concentration in ppm
  Serial.print("NH3 (ppm) = ");
  Serial.println(ppm);
   delay(200);
}

```
  
