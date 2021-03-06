# TLV493D-A1B6-3DMagnetic-Sensor
<img src="https://github.com/Infineon/Assets/blob/master/Pictures/3D%20Magnetic%20Sensor%202Go.jpg" width=250> <img src="https://github.com/Infineon/Assets/blob/master/Pictures/TLV493D-Sense-Shield2Go_Top_plain.jpg_2045671804.jpg?raw=true" width=300>

Library of Infineon's [TLV493D-A1B6 3D magnetic sensor](https://www.infineon.com/cms/de/product/sensor/magnetic-position-sensor/3d-magnetic-sensor/tlv493d-a1b6/) for Arduino. 

## Summary
The 3D magnetic sensor TLV493D-A1B6 offers accurate three-dimensional sensing with extremely low power consumption in a small 6-pin package. With its magnetic field detection in x, y, and z-direction the sensor reliably measures three-dimensional, linear and rotation movements. Applications include joysticks, control elements (white goods, multifunction knops), or electric meters (anti tampering) and any other application that requires accurate angular measurements or low power consumptions.
The integrated temperature sensor can furthermore be used for plausibility checks.

Key features are 3D magnetic sensing with a very low power consumption during operations. The sensor has a digital output via 2-wire based standard I2C interface up to 1 MBit/sec and 12 bit data resolution for each measurement direction (Bx, By and Bz linear field measurement up to +-130mT).

## Key Features and Benefits
* Integrated temperature sensing
* Low current consumption of 0.007 µA in power down mode and 10 µA in ultra low power mode
* 2.7 to 3.5 V operating supply voltage
* Digital output via 2-wire standard I2C interface
* Bx, By and Bz linear field measurement up to ±130 mT
* 12-bit data resolution for each measurement direction
* Resolution 98 µT/LSB
* Operating temperature range from -40 °C to 125 °C
* [GUI](https://www.infineon.com/cms/en/product/sensor/magnetic-position-sensor/3d-magnetic-sensor/TLV493D-A1B6+2+GO+KIT/productType.html?productType=5546d4624e24005f014e6775d0177011#ispnTab12) for free download as well as integration in Arduino IDE with this repository

## Installation

### Integration of Library
Please download this repository from GitHub by clicking on the following field in the [releases](https://github.com/Infineon/3D-Magnetic-Sensor-2GO/releases) of this repository or directly [here](https://github.com/Infineon/3D-Magnetic-Sensor-2GO/releases/download/V1.0.0/IFX-3D-Magnetic-Sensor-2GO.zip):

![Download Library](https://raw.githubusercontent.com/infineon/assets/master/Pictures/Releases_Generic.jpg)

To install the 3D magnetic sensor 2GO library in the Arduino IDE, please go now to **Sketch** > **Include Library** > **Add .ZIP Library...** in the Arduino IDE and navigate to the downloaded .ZIP file of this repository. The library will be installed in your Arduino sketch folder in libraries and you can select as well as include this one to your project under **Sketch** > **Include Library** > **TLV493D-A1B6**. 

![Install Library](https://raw.githubusercontent.com/infineon/assets/master/Pictures/Library_Install_ZIP.png)

## Usage
Please see the example sketches in the `/examples` directory in this library to learn more about the usage of the library.

Currently, there exist two separate evaluation boards:

* [TLV493D-A1B6 MS2GO](https://www.infineon.com/cms/en/product/sensor/magnetic-position-sensor/3d-magnetic-sensor/tlv493d-a1b6-ms2go/)
* [TLV493D-A1B6 3DMagnetic Shield2Go](https://www.infineon.com/cms/en/product/evaluation-boards/s2go_3d-sense_tlv493d/)

### Usage with TLV493D-A1B6 MS2GO
The 3D Magnetic Sensor 2GO is an evaluation board equipped with the magnetic sensor [TLV493D-A1B6](https://www.infineon.com/cms/de/product/sensor/magnetic-position-sensor/3d-magnetic-sensor/TLV493D-A1B6/productType.html?productType=5546d462525dbac401529cebc74f07b7) for three dimensional measurement combined with an ARM® Cortex™-M0 CPU. The 3D Magnetic Sensor 2GO has a complete set of on-board devices, including an on-board debugger. A PDF summarizing the features and layout of the 3D magnetic sensor 2GO board is stored on the Infineon homepage [here](https://www.infineon.com/dgdl/Infineon-3D-Magnetic-Sensor_EvalKit_UM-UM-v01_01-EN.pdf?fileId=5546d462525dbac40152ac4ca1d318c2).

Please note that base of the Sensors 2GO is the XMC 2Go from Infineon. Therefore, please install (if not already done) also the [XMC-for-Arduino](https://github.com/Infineon/XMC-for-Arduino) implementation and choose afterwards **XMC1100 XMC2Go** from the **Tools**>**Board** menu in the Arduino IDE if working with this evaluation board.

### TLV493D-A1B6 3DSense Shield2Go
The TLV493D-A1B6 3DMagnetic Shield2Go is a standalone break out board with Infineon's Shield2Go formfactor and pin out. You can connect it easily to any microcontroller of your choice which is Arduino compatible and has 3.3V logic level (please note that the Arduino UNO has 5V logic level and cannot be used without level shifting).

* [Link](https://github.com/Infineon/TLV493D-A1B6-3DMagnetic-Sensor/wiki) to the wiki with more information

However, every Shield2Go is directly compatible with Infineon's XMC2Go and the recommended quick start is to use an XMC2Go for evaluation. Therefore, please install (if not already done) also the [XMC-for-Arduino](https://github.com/Infineon/XMC-for-Arduino) implementation and choose afterwards **XMC1100 XMC2Go** from the **Tools**>**Board** menu in the Arduino IDE if working with this evaluation board. To use it, please plug the TLV493D-A1B6 3DMagnetic Shield2Go onto the XMC2Go as shown below.

<img src="https://github.com/Infineon/Assets/blob/master/Pictures/TLV493D-A1B6_S2Go_w_XMC2Go.png" width=250>

## Processing
This library supports the open-source software [Processing](https://processing.org/) for creating GUIs. It allows you to connect your evaluation board to a PC over serial communication and visualisation of the embedded system. Find out more on the Arduino homepage [here](http://playground.arduino.cc/Interfacing/Processing). The respective files are stored in the /processing folder of this repository. 

## Board Information, Datasheet and Additional Information

The datasheet for the TLV493D-A1B6 can be found here [TLV493D-A1B6 Datasheet](https://www.infineon.com/dgdl/Infineon-TLV493D-A1B6-DS-v01_00-EN.pdf?fileId=5546d462525dbac40152a6b85c760e80) while respective application notes are located here [Application Notes](https://www.infineon.com/cms/de/product/sensor/magnetic-position-sensor/3d-magnetic-sensor/TLV493D-A1B6+2+GO+KIT/productType.html?productType=5546d4624e24005f014e6775d0177011#ispnTab4).

Please check the [wiki](https://github.com/Infineon/TLV493D-A1B6-3DMagnetic-Sensor/wiki) with more information for the TLV493D-A1B6 3D Sense Shield2Go as well.

