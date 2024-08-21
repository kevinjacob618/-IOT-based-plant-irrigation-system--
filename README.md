INTRODUCTION
  IOT based plant irrigation system aims at nurturing of plants based on soil moisture levels. Water is supplied to the plants at times when required ensuring that plants receive the right amount of water without human intervention.
  This reduces the risk of under-watering or over-watering.
WORKING PRINCIPLE
 The soil moisture sensor measures the moisture level of the soil by passing a small current through it and measuring the resistance. The higher the resistance, the lower the moisture level. The sensor
 module outputs an analog voltage that is proportional to the moisture level.- The DHT11 sensor measures the air temperature and humidity by using a thermistor and a capacitive humidity sensor. The sensor outputs a digital signal that contains 40 bits of data: 16 bits for humidity, 16 bits for temperature, and 8 bits for checksum.- The LDR measures the light intensity by changing its resistance according to the amount of light
 falling on it. The higher the light intensity, the lower the resistance. The LDR is connected to a potentiometer that acts as a voltage divider and outputs an analog voltage that is proportional to the
 light intensity.- The NodeMCU reads the analog voltage from the soil moisture sensor and maps it to a percentage value between 0% (dry) and 100% (wet). It also reads the digital signal from the DHT11 sensor and
 extracts the temperature and humidity values. It also reads the analog voltage from the LDR and maps it to a percentage value between 0% (dark) and 100% (bright).- The NodeMCU compares the soil moisture value with a predefined threshold value that can be set
 according to the plant's requirement. If the soil moisture value is below the threshold value, it means that the soil is dry and needs water. In that case, it sends a high signal to the relay module, which switches on.- the solenoid valve and allows water to flow to the plants. If the soil moisture value is above the
 threshold value, it means that the soil is wet and does not need water. In that case, it sends a low signal to the relay module, which switches off the solenoid valve and stops the water flow.- The NodeMCU also sends the sensor data to an online platform, such as Blynk, using Wi-Fi. Blynk
 is a mobile app that allows users to create custom dashboards for IoT projects. The user canmonitor and visualize the data in real-time on the Blynk app. The user can also manually control the
 solenoid valve and other devices from the app using buttons or sliders.- The NodeMCU also displays the sensor data and the valve status on an LCD screen. The LCD screen shows the soil moisture percentage, the air temperature and humidity values, and the light
 intensity percentage. It also shows whether the valve is on or off

Hardware used : Esp32,Soil moisture sensor,Dht 11 sensor,Relay,DC water pump,battery.
Platform used : Arduino IDE, Blynk.
