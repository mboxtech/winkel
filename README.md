# Winkel Board : Unique Arduino Compatible board with m128 at it's core

Video Link : https://vimeo.com/194181201

### Winkel Board is a Powerful One Stop Arduino Compatible Development and Prototyping Board with ATmega128 at the Core. 

A new **Arduino Compatible, Powerful Open Source HardWare Platform**, that'll help accelerate prototyping and will help you put all your time and focus on actually building and completing your project rather than wasting it on the exhaustive non-productive  stuffs that comes as a part and parcel of every electronic project.
The Winkel Board is a unique, advanced & evolved development board. It is Arduino IDE compatible board that is more advanced than many of the popular advanced maker boards in the market. Also built on top of Atmel ATmega128, it goes a step further housing many of the popular known WiFi, Radio and Bluetooth chips on board. Targeted at both entry & advanced level makers, it provides a complete integrated solution for several projects.

## Story behind building The Winkel Board

We were building an IoT product and wanted to experiment with different communication protocols, like radio, wifi, bluetooth and found ourselves in a mess while doing so. Well ofcourse we had an Arduino Board to get started with but had to buy and experiment with different shields everytime and that costed us a lot of time and money. Being from India, such sheilds were really costly to source from outside + it really affected the speed of prototyping. We talked to a lot of makers and electronic hobbyists and found that this was a common problem within the maker community and not just in India but all over the world. Some suggested RPi 3 can be an answer for many projetcs but not every project needs an O.S. And not every project can be housed with an Arduino with all its sheilds, and some projects just require to use many communication protocols at once and need to perform a lot of calculations and I/O operations. To do all these powerfull things with just one small board and to keep it simple and arduino IDE compatible was the idea behind Winkel Board.

Video Link : https://vimeo.com/193928397

There are several other open hardware platforms like an arduino, raspberry pi or say some other controller based boards, but all of them fail to provide a single stop solution.

1. **For example there are times when you would require your Arduino to connect to the internet, but you have to buy an extra ethernet sheild or interface a WiFi chip to it in order to do so.**
2. **You may sometimes want to have accurate times on your controller to fulfil certain tasks at particular intervals, but have to interface an RTC with your controller or read time from the internet for which you will have go to the first point.**
3. **Or maybe you want to create a mesh network using radio nodes but have a hard time figuring out how to get started with NRF24l01 or buy a radio sheild for that reason.**
4. **You may also find a need to use Bluetooth in your projects, or you want to build a drone but you do not have a starting point on how to interface and use MPU6065 with a micro controller.**

Winkel Board provides all you makers with a one stop platform to do everything at once or choose specific onboard components to work with, because winkel board has an onboard powerful microcontroller with an onboard WiFi chip, Radio transceiver, Bluetooth, RTC and Gyroscope+accelerometer.

**You can basically use everything at once or specifically choose which onboard components you want to use in your project.**

# Problems we are trying to solve

_Exhaustive //TODO for a maker while building something awesome_

+ Prepare a list of right electronics components
+ Prepare BOM
+ Search them locally or online to fit the BOM
+ Wait for the components to arrive if sourced online
+ Getting started with prototyping
+ Go online again studying libraries and figuring out how they can be interfaced on breadboard or etch a PCB
+ Finally start building and actually working on your project and then **try not to rage quit**

{no-quit.jpg}


## Not with Winkel Board. You won't!!!

{winkel-board.jpg}

**It houses everything you would require to initiate a project - from basic Blink to advanced builds.**

{specification-top-view.png}

{specification-bottom-view.png}


# Technology

The Winkel Board is a microcontroller based board built on [ATmega128](http://www.atmel.com/devices/ATMEGA128.aspx?tab=parameters), an 8-bit microncontroller that has 128KB of Flash memory and 4KB of RAM. It contains everything needed to support the microcontroller; simply connect it to a computer with a USB cable or with a 5v micro USB power adapter.

It houses an Onboard WiFi module in the form of ESP8266 ESP12-E, an Onboard bluetooth in the form HC-05, an Onboard Radio transceiver in the form of NRF24l01 and Onboard Real time clock in the form of DS3231. **All of the Onboard components are built with Smart Opt, which means that they can be powered down if you have no use of that chip in your project.**  

**This board also supports OTA prgramming. This means you can burn your code on ESP8266 and on the microcontroller ATmega128 wirelessy Over The Air. Complete wireless programming** is useful in the sense when a board is already soldered in any project you want to make some changes to the code you burned on the microncontroller, you can easily do it wirelessy.

# Specifications

{feature.jpg}

| **Specifications**  | **Value**            |
| ------- | ---------------- |
| **Microcontroller**  | ATmega128 |
| **Operating Voltage**	 | 5V |
| **Digital I/O Pins** | 38* |
| **PWM Digital I/O Pins**	 | 7 |
| **Analog Input Pins**	 | 8 |
| **Flash Memory**	 | 128KB |
| **SRAM**	 | 4KB |
| **EEPROM**	 | 4KB |
| **Clock Speed**	 | 16MHz |
| **Onboard WiFi**	 | ESP8266-ESP12E |
| **Onboard Bluetooth**	 | HC-05 |
| **Onboard Radio Transceiver**	 | NRF24l01 |
| **Real Time Clock**	 | DS3231 |

**\*You get additional IO pins to work with because we have provided access to GPIO pin outs of ESP8266 ESP12E.**

# Pinout

{pin-diagram.jpg}

# Comparisons


||Winkel Board|MKR1000|Mega2560|101|Micro|Uno|Zero|
|----|----|----|----|----|----|----|----|----|
|**Processor**|ATmega128|SAMD21 Cortex-MO+|ATmega2560|Intel™ Curie|ATmega32U4|ATmega328P|AT SAMD21G18|
|**Operating Voltage** |5v|3.3v|5v|3.3v|5v|5v|3.3|
|**CPU Speed** |16Mhz|48Mhz|16Mhz|32Mhz|16Mhz|16Mhz|48Mhz|
|**Digital IO** |38|8|54|14|20|14|14|
|**Analog IO** |8|7/1|16|6|12|6|6/1|
|**PWM** |7|4|15|4|7|6|10|
|**EEPROM** |4KB|-|4KB|-|1KB|1KB|-|
|**SRAM** |4KB|4KB|8KB|24KB|2.5KB|1KB|32KB|
|**Flash** |128KB|256KB|256KB|196KB|32KB|32KB|256KB|
|**USB** |Micro|Regular|Regular|Regular|Micro|Regular|2 Micro|
|**UART** |2|1|4|-|1|1|2|
|**Onboard WiFi** |Yes ~success|Yes WINC1500 ~success|No ~danger|No ~danger|No ~danger|No ~danger|No ~danger|
|**Onboard Bluetooth** |Yes ~success|No ~danger|No ~danger|No ~danger|No ~danger|No ~danger|No ~danger|
|**Onboard Radio Transceiver** |Yes ~success|No ~danger|No ~danger|No ~danger|No ~danger|No ~danger|No ~danger|
|**Onboard Real Time Clock** |Yes ~success|No ~danger|No ~danger|No ~danger|No ~danger|No ~danger|No ~danger|
|**OTA Programming** |Yes ~success|No ~danger|No ~danger|No ~danger|No ~danger|No ~danger|No ~danger|
|**Smart Opt**|Yes ~success|No ~danger|No ~danger|No ~danger|No ~danger|No ~danger|No ~danger|


Winkel Board easily stands out as compared to other Arduino boards. While others are really useful to help a beginner learn the basics, they do not offer whats really needed to really get started with a real world project prototype where one can require other on board components. In that case he would have to go looking for such components in local radio shacks or source them online and then interface them.

Winkel board provides all the basic chip components for an intermediate-to-pro maker to really dive into that Super I.O.T project, or get on with that awesome mesh network or start building that co-ordinated drone.

## How it really compares

1. There were some views in the maker community that Atmega128 would be a slow MCU and the huge I/O set of operations would further slow down the board.
But Atmega128 is really isn't slow. Live testing several GPIO's (in projects like connecting huge number of relays in home automation, driving RGB strips using PWM's, gardening systems) have given really good results. Video and tutorials will be out soon.

2. Some compared it to faster 32Bit ARM Cortex where it was said even with the most efficient direct port operations, it takes at least 200ns to do anything on a 16Mhz AVR, where the arm cortex boards take 100 times less to toggle an IO, which means you can reasonably handle more IO pins without having any performance issue.
ARM cortex are really amazing when it comes down to building complex projects where performance and efficiency is needed say for example a robot for doing a complex realtime task where the huge RAM and 32bit architecture is a boon.

3. Winkel has been designed to provide almost everything On Board, that a maker would initially need to kickstart the prototyping of an idea and accelerate build time and not worry initially about nano second comparison. The list of chips and components keeps increasing as the product becomes more complex ofcourse and after prototyping one can easily shift towards powerful chips if necessary.


# Say Hello to OTA Programming

**There are times when you would require to update a sketch on your micro-controller in projects like gardening systems, quadcopter, bots etc. but  you do not want to disconnect everything and wished you could do it all wirelessly.**

### OTA programming of m128 over Bluetooth COM using Arduino IDE
With Winkel Board you have the power to update a skect on your controller Over The Air, completely wireless. You simply pair the onboard HC-05 Bluetooth module to your pc/laptop and use the Bluetooth's serial COM port to upload the sketch.
With Arduino IDE you can perform OTA programming of the **.INO files.** Hit upload and it really works like magic!!!

Video Link : https://vimeo.com/194169532


### OTA programming of m128 over Bluetooth COM using AVRdude
For all AVRDude fans, you can do the same thing using **AVR command line**. A complete wireless solution to update the **HEX file** on the controller. 

Video Link : https://vimeo.com/194171043


### OTA programming of ESP12-E over WiFi
That's not all. Remeber there is an ESP-12E module on-board. What good is OTA programming if you can only program the m128 and not the WiFi module? Winkel Board goes a step ahead and allows you to wirelessly program the ESP12E module over WiFi.
When you power ON the board the WiFi module automatically goes into configuration mode allowing you to bring the ESP module on to your WiFi network. As soon as that is done, your router assigns an IP address to the ESP module and you can upload/update sketches on the ESP12E module over WiFi using the IP address.
It may only sound complex. It is really NOT!!!

Video Link : https://vimeo.com/194170074

**If you have a question that all this might confuse you,we have you covered. You have the power to perform the same old process of uploading code onto the board with those programmers.**

# Build Examples

There are many things you can build with Winkel Board. Below are a couple of examples. We are also coming up with a dedicated page to upload many build examples.

## Wireless Sensor Network

Video Link : https://vimeo.com/194135878

## Remote Control using Joystick

Video Link : https://vimeo.com/194135609

# Who Needs It and Why?
Winkel Board is ideal for makers who work on electronic projects which involve a lot of I/O operations and involves using different communication protocols to fulfill different tasks. Winkel Board is also for engineers and hardware hackers who are looking to build and prototype products of tomorrow, but have to spend time looking for the right components to use and then spend more time figuring out how they can be interfaced together as it requires basic knowledge of various chips and their libraries to get started.

Winkel Board helps you achieve all of the above, so that you don't have to spend time on looking for components and studying their libraries and you can quickly accelerate building and prototyping.

Winkel has almost everything On Board, that any maker would need to kickstart the prototyping of an idea. Be it any product or project, one would primarily need a powerful set of I/O pins to get started with and would need some a simple IDE to embed a code on it. Secondary things would involve using some sort of WiFi controller if the project has something to do with connecting to the internet or providing an adhoc hostspot, or one may require radio controllers if the project has something to do with creating a mesh or building a robot or a drone. The list of chips and components keeps increasing as the product becomes more complex.


# Manufacturing Plan

PCB manufacturing will happen in India or China (or both) depending on the number of pledges we receive. We will start shipping in February. 

{base-board2.jpg}


# Challenges

1. **Everything at once in 5cm x 5cm. The Design.**
  * After deciding on the on-board components for the Winkel board, a major challenge we faced was to keep the form factor of the board small and compact, otherwise we would end up with big bulky board along with some components interfaced together. We finally managed to pull off a 2-sided PCB to fit everything in a form factor of 5cm x 5cm
2. **Design it not just how it looks and feels like.**
  * After getting the design right, we really had to work our way to get everything working together out of the box flawlessly. We had to get features like OTA programming of m128 and ESP-12E working right without any glitches, while also keeping support for conventional wired serial programming. We had to have a fully functional Smart opt feature that would allow a maker to power on only those on-board components that he wishes to work with. We did this by using conducting Jumpers.
3. **Arduino IDE support & AVR support**
  * Another challenge was to get Winkel Board to show up as a standard board under the Boards section of the famous Arduino IDE. While we achieved that and a maker could now perform a standard Boards Manager Installation, we also had to provide support for non IDE users. Hardcore AVR programmers use avrdude and we could successfully keep support for avrdude programming using avr command lines.
4. **Pricing should be maker friendly**
  * Pricing eventually will hugely depend on the response for this board because quantity is what it comes down to when one wants to lower manufacturing costs. We are really trying our best to keep it maker and DIY friendly.

# Current Status

We have been working on this project for quite some time now and we had a successful trial production run for the Winkel Board. As a result of our successful batch run, we would
like to bring Winkel Board to every maker and need your support to build a community around it.

While the work and designs for the actual board are already complete we are now working on a Tiny MPU-6050 Gyro+accelerometer mount for the Winkel Board. The designs and handmade prototypes are ready and we are positive to complete a 
finished batch before the campaign ends. Have a look at the prototype and a working example.

This mount complements the huge IO set of the Winkel Board along with various comm protocols and is ideal if you are planning to build a Balancing Bot, drone, quadcopter or maybe a smart skateboard 

{gyro2.jpg}

{gyro.jpg}

Video Link : https://vimeo.com/194552069

# Community & Resources

1. **[Arduino Forum](http://forum.arduino.cc/index.php?topic=429389.0)**
2. **[Reddit](https://redd.it/58fwdf)**
3. **[Instructables](http://www.instructables.com/id/The-Winkel-Board/)**
4. **[Hackaday](https://hackaday.io/project/17055-the-winkel-board)**
5. **[Github](https://github.com/mboxtech)**

# FAQ's

1. Why choose Atmega128?
  * Many don't know this, but m128 was the original arduino before it was even called arduino. There were some fragments left in the original arduino core but the support for it was dropped years ago. they were replaced by better known mega8(ng). Back then m128 was 20x times expensive and although m8(ng) was 10x times expensive it was affordable and had advantage of dip support. m128 was simply forgotten but has stayed popular among pure AVR programmers and not programming through famous Arduino IDE.
  * They're hand solderable (The TQFP variant have 0.8mm pin pitch)
  * They've been around for more than a decade, and can be found in a lot of different equipment
  * They got 53 IO pins (vs 86 for the ATmega1280/2560)
  * Plus you still have an onboard ESP8266 as well so your Wifi needs have been taken care of. You have the option to power it off if you are not using it.

2. Dual MCU?
  * YES. Atmega128 + ESP8266 ESP12E. ESP is more of a wifi module with a SOC. They are connected via UART (atmega128 has 2 uart) and can communicate with each other at the same time run their own code. You can try it. Like interfacing an ESP8266 with an Arduino Pro Mini.

3. OTA - Gimmick or Magic?
  * You should definitely experience OTA on Winkel Board. Works flawlessly. wireless programming for the main controller m128 using bluetooth and wireless programming esp-12e over wifi. And if at all you start experiencing trouble or wired programming is just what your are more comfortable with, we have retained that feature as well. You can go for wired programming.

4. What is Smart Opt Feature?
  * Smart Opt is a feature through which you can enable or disable the power going to the specific component by use of conducting jumpers. Basically you can control the power to be passed only to specific components and not all.

**A major point behind development of Winkel Board was to bring the famous ATmega128 back on the Arduino IDE platform. So prototyping and development is faster as everything is packaged.**

+ you have support for widely popular Arduino IDE
+ good set of I/O
+ Several communication protocols to work with. No need to search components for interfacing.(wifi,radio,bluetooth,RTC)
+ All programmable onboard components can be programmed wirelessly, so once you use it in a project no need to remove it again to perform wired programming

**If you have more questions, feel free to write to us and we will answer/add them here.**

