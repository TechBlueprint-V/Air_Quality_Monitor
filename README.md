# Air_Quality_Monitor

This is an open-source, modular air quality monitoring system designed for both urban and remote deployments. It uses a combination of ESP32 and STM32 microcontrollers to collect and process real-time environmental data from various sensors measuring PM2.5, PM10, CO₂, VOCs, O₃, SO₂, and NO₂. The system features LoRa communication for long-range data transmission, GPS for location tagging, and a solar panel and charger for long-term usage. The hardware is custom-designed and includes power management for battery operation, while the firmware is optimized for low-power performance. All PCB designs, firmware code, and 3D-printed enclosure files are provided in this repository.

# Block Diagram

![Block Diagram](https://github.com/TechBlueprint-V/Air_Quality_Monitor/blob/main/Air%20Quality%20Monitor/Images/Block%20Diagram.png)


## Real View

![Real View](https://github.com/TechBlueprint-V/Air_Quality_Monitor/blob/main/Air%20Quality%20Monitor/Images/Air%20Quality%20Monitoring%20Device.jpg)

*Note: The device shown above is an early prototype and not the final version. Development is still ongoing, and once the fully assembled version is complete, updated images and design details will be added here.* 

# Contents
- [Used Tools](#Used-Tools)
- [Features and Specifications](#Features-and-Specifications)
- [Schematic](#Schematic)
- [Layout](#Layout)
- [3D Views](#3D-Views)
- [Enclosure](#Enclosure)
- [Future Work](#Future-Work)
- [References](#References)

## Used Tools

**Altium Designer**

![Altium Logo](https://github.com/TechBlueprint-V/Air_Quality_Monitor/blob/main/Air%20Quality%20Monitor/Images/Altium_Designer_Logo.png)

   - Altium Designer (AD) is a software package for printed circuit board (PCB) design and electronic design automation. It is developed by the American software company Altium Limited. Altium Designer was formerly known under the brand Protel.

  **Saturn PCB Toolkit**

![Saturn PCB Toolkit Logo](https://github.com/TechBlueprint-V/Air_Quality_Monitor/blob/main/Air%20Quality%20Monitor/Images/logo-saturn-pcb.png)

  - The Saturn PCB Toolkit is the best freeware resource for PCB-related calculations. It incorporates many features that PCB designers and engineers regularly need, like the current capacity of a PCB trace, via current, differential pairs, and much more.

  **SolidWorks**

![SolidWorks Logo](https://github.com/TechBlueprint-V/Air_Quality_Monitor/blob/main/Air%20Quality%20Monitor/Images/SolidWorksNewLogo.jpg)

  - SolidWorks (stylized as SOLIDWORKS ) is a computer-aided 3D solid modeling and design (3D CAD) software. SolidWorks Corporation was founded in 1993 by Jon Hirschtick in Concord, Massachusetts. It was acquired by Dassault Systèmes in 1997 after releasing the first version of the software in 1995. It was the first 3D solid modeling (3D CAD) software integrated into Windows.


## Features and Specifications

| Feature                  | Description                                                                 |
|--------------------------|-----------------------------------------------------------------------------|
| Microcontrollers         | ESP32 and STM32F103C8T6 (dual MCU architecture for efficient task handling)|
| Particulate Matter Sensor | PMS5003 - Measures PM2.5 and PM10                                           |
| Gas Sensors              | MQ-136 (SO₂), MQ-131 (O₃), MICS-2714 (NO₂), BME680 (VOC)                    |
| CO₂ Sensor               | SCD30 - Measures CO₂, humidity, and temperature                             |
| UV Sensor                | GUVA-S12SD - Detects UV light intensity                                     |
| Environmental Sensor     | BME680 - Measures temperature, pressure, humidity, VOC                      |
| Communication            | LoRa SX1276 - 868 MHz long-range wireless data transmission                 |
| GPS Module               | NEO-6M - Provides geolocation tagging                                       |
| Display                  | 1.54-inch TFT LCD - Displays live sensor readings                           |
| Power Supply             | 1100mAh Li-ion Battery + USB-C charging                                     |
| Power Management         | MCP73831, MP2182GTL-Z, MIC2250, BQ24210 for voltage regulation and charging |
| Enclosure                | 3D-printed custom case for outdoor use                                     |
| Use Case Examples        | Urban pollution monitoring, smart agriculture, remote environmental sensing |

## Schematic

**MCU**

![MCU](https://github.com/TechBlueprint-V/Air_Quality_Monitor/blob/main/Air%20Quality%20Monitor/Images/MCU.png)

**Sensors**

![Sensors](https://github.com/TechBlueprint-V/Air_Quality_Monitor/blob/main/Air%20Quality%20Monitor/Images/Sensors.png)

**Lora**

![GPS](https://github.com/TechBlueprint-V/Air_Quality_Monitor/blob/main/Air%20Quality%20Monitor/Images/Lora.png)

**GPS**

![GPS](https://github.com/TechBlueprint-V/Air_Quality_Monitor/blob/main/Air%20Quality%20Monitor/Images/GPS.png)

**Power**

![Power](https://github.com/TechBlueprint-V/Air_Quality_Monitor/blob/main/Air%20Quality%20Monitor/Images/Power.png)

## Layout

**Layer-1**

![Layer-1](https://github.com/TechBlueprint-V/Air_Quality_Monitor/blob/main/Air%20Quality%20Monitor/Images/L1.png)

**Layer-2**

![Layer-2](https://github.com/TechBlueprint-V/Air_Quality_Monitor/blob/main/Air%20Quality%20Monitor/Images/L2.png)

**Layer-3**

![Layer-3](https://github.com/TechBlueprint-V/Air_Quality_Monitor/blob/main/Air%20Quality%20Monitor/Images/L3.png)

**Layer-4**

![Layer-4](https://github.com/TechBlueprint-V/Air_Quality_Monitor/blob/main/Air%20Quality%20Monitor/Images/L4.png)

## 3D Views

**3D-Top**

![3D Top](https://github.com/TechBlueprint-V/Air_Quality_Monitor/blob/main/Air%20Quality%20Monitor/Images/3D%20Top.jpeg)


**3D-Bottom**

![3D Bottom](https://github.com/TechBlueprint-V/Air_Quality_Monitor/blob/main/Air%20Quality%20Monitor/Images/3D%20Bottom.jpeg)

## Enclosure

**Enclosure view 1**

![Enclosure-1](https://github.com/TechBlueprint-V/Air_Quality_Monitor/blob/main/Air%20Quality%20Monitor/Images/Enclosure-1.png)

**Enclosure view 2**

![Enclosure-2](https://github.com/TechBlueprint-V/Air_Quality_Monitor/blob/main/Air%20Quality%20Monitor/Images/Enclosure-2.png)

**Enclosure view 3**

![Enclosure-3](https://github.com/TechBlueprint-V/Air_Quality_Monitor/blob/main/Air%20Quality%20Monitor/Images/Enclosure-3.png)


**Enclosure view 4**

![Enclosure-4](https://github.com/TechBlueprint-V/Air_Quality_Monitor/blob/main/Air%20Quality%20Monitor/Images/Enclosure-4.png)

**Enclosure view 5**

![Enclosure-5](https://github.com/TechBlueprint-V/Air_Quality_Monitor/blob/main/Air%20Quality%20Monitor/Images/Enclosure-5.png)


## Future Works

- **Cloud Integration and Dashboard**: Develop a cloud-based data logging and visualization dashboard to store historical air quality data and present trends using interactive charts and maps.
- **Mobile Application**: Create a companion Android/iOS app for real-time monitoring, GPS-based pollution alerts, and historical data access.
- **OTA (Over-the-Air) Firmware Updates**: Implement OTA functionality for ESP32 to allow remote firmware upgrades without physical access.
- **Machine Learning for Pollution Prediction**: Integrate lightweight ML models to analyze collected data and predict air quality trends based on environmental factors.
- **Solar Power Option**: Design and test a solar-powered charging module to support long-term outdoor deployment without manual charging.
- **Additional Sensors**: Expand sensor support for detecting carbon monoxide (CO), lead (Pb), or other industrial pollutants.
- **LoRaWAN Gateway Support**: Enable compatibility with public or private LoRaWAN gateways to support broader communication networks.

## References

1. Plantower PMS5003 Datasheet – [https://files.particle.io](https://www.aqmd.gov/docs/default-source/aq-spec/resources-page/plantower-pms5003-manual_v2-3.pdf)
2. Sensirion SCD30 CO2 Sensor Datasheet – [https://www.sensirion.com](https://sensirion.com/media/documents/4EAF6AF8/61652C3C/Sensirion_CO2_Sensors_SCD30_Datasheet.pdf)
3. Bosch BME680 Sensor Datasheet – [https://www.bosch-sensortec.com](https://www.bosch-sensortec.com/media/boschsensortec/downloads/datasheets/bst-bme680-ds001.pdf)
4. MQ Sensor Series Overview – [https://www.winsen-sensor.com](https://www.pololu.com/file/0j309/mq2.pdf)
5. NEO-6M GPS Module Datasheet – [https://cdn.sparkfun.com](https://content.u-blox.com/sites/default/files/products/documents/NEO-6_DataSheet_%28GPS.G6-HW-09005%29.pdf)
6. Semtech SX1276 LoRa Transceiver Datasheet – [https://www.semtech.com](https://semtech.my.salesforce.com/sfc/p/E0000000JelG/a/2R0000001Rbr/6EfVZUorrpoKFfvaF_Fkpgp5kzjiNyiAbqcpqh9qSjE?__hstc=212684107.5cd8f4b223e4b582dc3641df41a9f0a5.1751280448539.1751280448539.1751280448539.1&__hssc=212684107.1.1751280448539&__hsfp=2742738040)
7. STM32F103C8T6 Reference Manual – [https://www.st.com]([https://www.st.com/resource/en/reference_manual/CD00171190.pdf](https://www.st.com/resource/en/reference_manual/rm0008-stm32f101xx-stm32f102xx-stm32f103xx-stm32f105xx-and-stm32f107xx-advanced-armbased-32bit-mcus-stmicroelectronics.pdf))
8. ESP32 Technical Reference Manual – [https://www.espressif.com](https://www.espressif.com/sites/default/files/documentation/esp32_technical_reference_manual_en.pdf)
9. [PlatformIO](https://platformio.org/) – Cross-platform development environment
10. [STM32CubeIDE](https://www.st.com/en/development-tools/stm32cubeide.html) – Integrated development tool for STM32 microcontrollers
