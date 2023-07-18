# Iot-Based_Patient-Health-Monitoring-System-
**Introduction:**

IoT is rapidly revolutionising the Healthcare Industry. In this project, I have designed the IoT
Based Patient Health Monitoring System using **ESP8266 & Arduino**. The IoT platform used
in this project is **ThingSpeak**. This IoT device could read the pulse rate and surrounding
temperature and update them to an IoT platform.
This Health Monitoring System simulates two major aspects of health and wellbeing :
**i) Human Body Temperature, ii) Heart Beat Rate.**
It presents the numerical value of these two aspects and maintains a data logger system
where the patient’s data can be stored and received for medical history and check-up
purpose collectively. Along with that the output values can be viewed through waveform
chart. The circuit output values in the LED represent the current heartbeat, time in second,
heartbeat per minute and body temperature.

**Objectives:**

● To design a portable health monitoring system, which measures the patient’s body
temperature and pulse rate.

● To provide medical assistance according to the data received from the sensors which
stored in cloud server (ThingSpeak).

**Block Diagram:**
![Block Diagram](https://github.com/HackwithArpon/Iot-Based_Patient-Health-Monitoring-System-/assets/116937463/07e15f60-6c7c-4983-8915-264cb5167680)
This is a simple block diagram that explains the IoT Based Patient Health Monitoring System
using ESP8266 & Arduino. Pulse sensor and LM35 temperature sensor measure BPM &
Environmental temperature respectively. The Arduino processes the code and displays it to
16*2 LCD Display. ESP8266 Wi-Fi module connects to Wi-Fi and sends the data to IoT
device server. The IoT server used here is ThingSpeak. Finally, the data can be monitored
from any part of the World by logging into the ThingSpeak channel.


**Requirements:**

Hardware Requirements-

● Arduino Uno

● ESP8266 Wi-Fi Module

● LM35 Temperature Sensor

● Pulse Sensor

● 16*2 LCD Display

● Potentiometer (10K)

● Resistor (1K & 2K)

● Breadboard

Software Requirements-

● Arduino Compiler

● ThingSpeak (Cloud Service)

**Arduino Uno :**

Arduino UNO is based on an **ATmega328P** microcontroller. The Arduino UNO includes 6
analog pin inputs, 14 digital pins, a USB connector, a power jack, and an ICSP (In-Circuit
Serial Programming) header. It is programmed based on IDE, which stands for Integrated
Development Environment. It can run on both online and offline platforms.

The components of Arduino UNO board are shown below:

● **ATmega328 Microcontroller :** It is a single chip Microcontroller of the ATmel family.
The processor code inside it is 8-bit. It combines Memory (SRAM, EEPROM, and
Flash), Analog to Digital Converter, SPI serial ports, I/O lines, registers, timer,
external and internal interrupts, and oscillator.

● **ICSP pin :** The In-Circuit Serial Programming pin allows the user to program using the
firmware of the Arduino board.

● **Power LED Indicator :** The ON status of LED shows the power is activated. When the
power is OFF, the LED will not light up.

● **Digital I/O pins :** The digital pins have the value HIGH or LOW. The pins numbered
from D0 to D13 are digital pins.

● **TX and RX LED's :** The successful flow of data is represented by the lighting of these
LED's.

● **AREF :** The Analog Reference (AREF) pin is used to feed a reference voltage to the
Arduino UNO board from the external power supply.

● **Reset button :** It is used to add a Reset button to the connection.

● **USB :** It allows the board to connect to the computer. It is essential for the
programming of the Arduino UNO board.

● **Crystal Oscillator :** The Crystal oscillator has a frequency of 16MHz, which makes the
Arduino UNO a powerful board.

● **Voltage Regulator :** The voltage regulator converts the input voltage to 5V.

● **GND :** Ground pins. The ground pin acts as a pin with zero voltage.

● **Vin :** It is the input voltage.

● **Analog Pins :** The pins numbered from A0 to A5 are analog pins. The function of
Analog pins is to read the analog sensor used in the connection. It can also act as
GPIO (General Purpose Input Output) pins.

**ESP8266 :**

The ESP8266 is a very user-friendly and low-cost device to provide internet connectivity to
our projects. The module can work both as an Access point (can create hotspot) and as a
station (can connect to Wi-Fi), hence it can easily fetch data and upload it to the internet
making the Internet of Things as easy as possible. It can also fetch data from the internet
using API’s hence our project could access any information that is available on the internet,
thus making it smarter. Another exciting feature of this module is that it can be programmed
using the Arduino IDE which makes it a lot more user-friendly.

The ESP8266 module works with 3.3V only, anything more than 3.7V would kill the module
hence be cautious with our circuits.

Here is its pins description:

**Pin 1: Ground:** Connected to the ground of the circuit

**Pin 2: Tx/GPIO – 1:** Connected to Rx pin of programmer/uC to upload program

**Pin 3: GPIO – 2:** General purpose Input/output pin

**Pin 4 : CH_EN:** Chip Enable/Active high

**Pin 5: Flash/GPIO – 0:** General purpose Input/output pin

**Pin 6 : Reset:** Resets the module

**Pin 7: RX/GPIO – 3:** General purpose Input/output pin

**Pin 8: Vcc:** Connect to +3.3V only

**LM35 Temperature Sensor :**

The LM35 series are precision integrated-circuit temperature devices with an output voltage
linearly-proportional to the Centigrade temperature. The LM35 device has an advantage over
linear temperature sensors calibrated in Kelvin, as the user is not required to subtract a large
constant voltage from the output to obtain convenient Centigrade scaling. The LM35 device
does not require any external calibration or trimming to provide typical accuracies of ±¼°C at
room temperature and ±¾°C over a full −55°C to 150°C temperature range.

**Pulse Sensor :**

The Pulse Sensor is a plug-and-play heart-rate sensor for Arduino. It can be used by
students, artists, athletes, makers, and game & mobile developers who want to easily
incorporate live heart-rate data into their projects. The essence is an integrated optical
amplifying circuit and noise eliminating circuit sensor. Clip the Pulse Sensor to our earlobe or
fingertip and plug it into our Arduino, we can ready to read heart rate. Also, it has an Arduino
demo code that makes it easy to use.

**● Pin-1(GND) :** Black Colour Wire - It is connected to the GND terminal of the system.

**● Pin-2(VCC) :** Red Colour Wire - It is connected to the supply voltage (+5V otherwise
+3.3V) of the system.

**● Pin-3(Signal) :** Purple Colour Wire - It is connected to the pulsating o/p signal.

**16*2 LCD Display :**

The features of this LCD mainly :

● The operating voltage of this LCD is 4.7V-5.3V

● It includes two rows where each row can produce 16-characters

● The utilization of current is 1mA with no backlight

● Every character can be built with a 5×8 pixel box

● The alphanumeric LCDs alphabets & numbers

● Is display can work on two modes like 4-bit & 8-bit

● These are obtainable in Blue & Green Backlight

● It displays a few custom generated characters

**ThingSpeak :**

ThingSpeak allows you to aggregate, visualize and analyze live data streams in the cloud.
Some of the key capabilities of ThingSpeak include the ability to:

● Easily configure devices to send data to ThingSpeak using popular IoT protocols.

● Visualize our sensor data in real-time.

● Aggregate data on-demand from third-party sources.
    
● Use the power of MATLAB to make sense of our IoT data.

● Run our IoT analytics automatically based on schedules or events.

● Prototype and build IoT systems without setting up servers or developing web
software.

● Automatically act on our data and communicate using third-party services like Twilio
or Twitter

To learn how you can collect, analyze and act on our IoT data with ThingSpeak, explore the
topics below:

**Collect :** Send sensor data privately to the cloud

**Analyze :** Analyze and visualize our data with matlab

**Act:** Trigger a reaction

**Circuit Connections :**

**1.** Connect Pulse Sensor output pin to A0 of Arduino and other two pins to VCC and GND.
**2.** Connect LM35 Temperature Sensor output pin to A1 of Arduino and other two pins to VCC
& GND.
**3.** Connect the LED to Digital pin 7 of Arduino via a 220-ohm resistor.
**4.**Connect pin 1,3,5,16 of LCD to GND.
**5.** Connect pin 2,15 of LCD to VCC.
**6.** Connect pin 4,6,11,12,13,14 of LCD to Digital pin 12,11,5,4,3,2 of Arduino.
**7.** The RX pin of ESP8266 works on 3.3V and it will not communicate with the Arduino when
we will connect it directly to the Arduino. So, we will have to make a voltage divider for it
which will convert the 5V into 3.3V. This can be done by connecting the 2.2K & 1K resistor.
Thus the RX pin of the ESP8266 is connected to pin 10 of Arduino through the resistors.
**8.** Connect the TX pin of the ESP8266 to pin 9 of the Arduino.

**Conclusion:**

● Our proposed system aims at simplifying health monitoring.

● This system of ours has been proven effective enough in aiding medical assistance.

● This approach of ours contributes towards Smart India.

**References:**

**❖ Marathe, Sachi, et al. “A Wireless Patient Monitoring System using Integrated ECG
module, Pulse Oximeter, Blood Pressure and Temperature Sensor.” 2019 International
Conference on Vision Towards Emerging Trends in Communication and Networking
(ViTECoN). IEEE, 2019.**

**❖ Mishra, Vaibhav, Durgesh Kumar Mishra and Ass. Prof. Ankit Trivedi. “Health
Monitoring System using IoT using Arduino Uno Microcontroller.” Health 6.08 (2019).**


By **Arpon Kumar Choedhury**, KGEC_CSE'25
