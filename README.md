Winkel Board
=======

**Winkel Board is a Powerful One Stop Arduino Compatible Development and Prototyping Board with ATmega128 at the Core.**


<!-- <table>
          <tr>
           <td>
           <p>For people in India</p>
           </td>
           <td>
           <a href="https://www.instamojo.com/makerville/knit-beta/" rel="im-checkout" data-behaviour="remote" data-style="dark" data-text="Buy" data-token="ed5a4059401167126952178eb636717a"></a>
<script src="https://d2xwmjc4uy2hr5.cloudfront.net/im-embed/im-embed.min.js"></script>
</td>
</tr>
        <tr>
          <td>
        <p>For people outside India</p></td>
        <td>
        <form action="https://www.paypal.com/cgi-bin/webscr" method="post" target="_top">
<input type="hidden" name="cmd" value="_s-xclick">
<input type="hidden" name="hosted_button_id" value="NE6DD2M32CYC8">
<input type="image" src="https://www.paypalobjects.com/en_GB/i/btn/btn_paynowCC_LG.gif" border="0" name="submit" alt="PayPal – The safer, easier way to pay online!">
<img alt="" border="0" src="https://www.paypalobjects.com/en_GB/i/scr/pixel.gif" width="1" height="1">
</form>
       </td>
     </tr>

</table> -->

<iframe src="https://player.vimeo.com/video/193928397" width="720" height="404" frameborder="0" webkitallowfullscreen mozallowfullscreen allowfullscreen></iframe>

Technology
---

The Winkel Board is a microcontroller based board built on [ATmega128](http://www.atmel.com/devices/ATMEGA128.aspx?tab=parameters), an 8-bit microncontroller that has 128KB of Flash memory and 4KB of RAM. It contains everything needed to support the microcontroller; simply connect it to a computer with a USB cable or with a 5v micro USB power adapter.

It houses an Onboard WiFi module in the form of ESP8266 ESP12-E, an Onboard bluetooth in the form HC-05, an Onboard Radio transceiver in the form of NRF24l01 and Onboard Real time clock in the form of DS3231. **All of the Onboard components are built with Smart Opt, which means that they can be powered down if you have no use of that chip in your project.**  

**This board also supports OTA prgramming. This means you can burn your code on ESP8266 and on the microcontroller ATmega128 wirelessy Over The Air. Complete wireless programming** is useful in the sense when a board is already soldered in any project you want to make some changes to the code you burned on the microncontroller, you can easily do it wirelessy.

Features
---

* A powerful core in the form of ATmega128
* On-board Bluetooth Module in the form of HC-05
* On-board WiFi module in the form of ESP8266 ESP12E
* On-board Real Time Clock in the form of DS3231
* On-board Radio Transceiver in the form of NRF24l01
* OTA programming of Atmega128 and ESP12E  (This one is a biggie :) )
* Smart-Opt feature enabling you to use only specific on-board components when needed.
* And all this in a form factor of 5cm x 5cm

| **Specifications**  | **Value**            |
| ------- | ---------------- |
| **Microcontroller**  | ATmega128 |
| **Operating Voltage**  | 5V |
| **Digital I/O Pins** | 38* |
| **PWM Digital I/O Pins**   | 7 |
| **Analog Input Pins**  | 8 |
| **Flash Memory**   | 128KB |
| **SRAM**   | 4KB |
| **EEPROM**   | 4KB |
| **Clock Speed**  | 16MHz |
| **Onboard WiFi**   | ESP8266-ESP12E |
| **Onboard Bluetooth**  | HC-05 |
| **Onboard Radio Transceiver**  | NRF24l01 |
| **Real Time Clock**  | DS3231 |

**\*You get additional IO pins to work with because we have provided access to GPIO pin outs of ESP8266 ESP12E.**

Documentation
====

Pin Map
---

<a href="http://i.imgur.com/ukiZS0f.jpg" target="_blank"><img style="width:720px;height:404px;" src="http://i.imgur.com/ukiZS0f.jpg" title="source: imgur.com" /></a>

Comparison
---

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
|**Onboard WiFi** |Yes |Yes WINC1500 |No |No |No |No |No |
|**Onboard Bluetooth** |Yes |No |No |No |No |No |No |
|**Onboard Radio Transceiver** |Yes |No |No |No |No |No |No |
|**Onboard Real Time Clock** |Yes |No |No |No |No |No |No |
|**OTA Programming** |Yes |No |No |No |No |No |No |
|**Smart Opt**|Yes |No |No |No |No |No |No |


Power
---

### Input sources

You can power up Winkel Board using

- 5V through USB

### LED Indication

Winkel Board has 3 <a style="color:green;">green</a> LED indicators for HC05, NRF24l01 and ATmega128 that light up when these components are powered ON.

### Smart Opt

You can use smart opt feature on the Winkel Board to power ON only required on-board components and not all. There are conducting jumpers on the board, that will allow you to pass power to ESP12E, HC05 and NRF24l01 individually.

Hardware
---

Winkel Board is open source hardware. There are a few definitions of OSHW, but what it means to us is that everything that one would need to make Knit is made available to everyone under a permissive license.

Winkel Board is licensed under the MIT License. You can find text of the license [here](https://github.com/Makerville/knit/blob/master/LICENSE). All the files can be found on our [GitHub](http://github.com/makerville/knit/blob/master/hardware).


### Major components
The Winkel board consists of the following major hardware components -

| Function | Part No | Datasheet
|:-:|:-:|:-:|
| Central Core | ATmega128a-au | <a href="http://www.atmel.com/devices/ATMEGA128.aspx?tab=parameters" target="_blank">Link</a>
| WiFi | ESP8266-12E |<a href="http://www.kloppenborg.net/images/blog/esp8266/esp8266-esp12e-specs.pdf" target="_blank">Link</a>|
| Bluetooth | HC-05 | <a href="http://cdn.makezine.com/uploads/2014/03/hc_hc-05-user-instructions-bluetooth.pdf" target="_blank">Link</a>
| Radio Transceiver | NRF24l01 | <a href="https://www.sparkfun.com/datasheets/Components/SMD/nRF24L01Pluss_Preliminary_Product_Specification_v1_0.pdf" target="_blank">Link</a>
| Real Time Clock | DS3231 | <a href="https://datasheets.maximintegrated.com/en/ds/DS3231.pdf" target="_blank">Link</a>
| Regulator | LM1117 |<a href="http://www.ti.com/lit/ds/symlink/lm1117.pdf" target="_blank">Link</a>

Arduino Support
===
An Arduino Core for the Winkel Boards. A custom bootloader for ATmega128 was needed to provide support for widely used Arduino IDE. A special thanks to MCUdude who wrote an [Arduino Core for ATmega128 and ATmega64](https://github.com/MCUdude/MegaCore) all running a modified version of Optiboot known as **MegaCore.**

### Boards Manager Installation
This installation method requires Arduino IDE version 1.6.4 or greater.

* Open the Arduino IDE.
* Open the **File > Preferences** menu item.
* Enter the following URL in **Additional Boards Manager URLs**: 

`https://raw.githubusercontent.com/mboxtech/WinkelCore/master/package_WinkelCore_index.json`

* Open the **Tools > Board > Boards Manager...** menu item.
* Wait for the platform indexes to finish downloading.
* Scroll down until you see the **WinkelCore** entry and click on it.
  * **Note**: If you are using Arduino IDE 1.6.6 then you may need to close **Boards Manager** and then reopen it before the **WinkelCore** entry will appear.
* Click **Install**.
* After installation is complete close the **Boards Manager** window.
* Go to **Tools > Board >** and you should see **Winkel Board**

### Manual Installation
Click on the "Download ZIP" button in the upper right corner. Exctract the ZIP file, and move the extracted folder to the location "**~/Documents/Arduino/hardware**". Create the "hardware" folder if it doesn't exist.
Open Arduino IDE, and a new category in the boards menu called "WinkelCore" will show up.

OTA Programming
===

### ATmega128 OTA programming
Coming Soon

### ESP12E OTA Programming

<a href="https://github.com/mboxtech/Winkel-Board-Examples/tree/master/ESP12-Winkel-ota-git-example">Instructions</a>

Videos
===

### Wireless Mouse Control Over Radio Network. 

<iframe src="https://player.vimeo.com/video/194135609" width="720" height="404" frameborder="0" webkitallowfullscreen mozallowfullscreen allowfullscreen></iframe>

### Wireless Sensor Network Using the Winkel Board 

<iframe src="https://player.vimeo.com/video/194135878" width="720" height="404" frameborder="0" webkitallowfullscreen mozallowfullscreen allowfullscreen></iframe>

Resources
====
Here are some of the resources for The Winkel Board

Arduino Forum
---
* [Forum Post](http://forum.arduino.cc/index.php?topic=429389.0)

Instructables
---
* [Intro](http://www.instructables.com/id/The-Winkel-Board/)
* [Build Example-1](http://www.instructables.com/id/Wireless-Senor-Network-Using-the-Winkel-Board/)

Hackaday
---
* [Hackaday Page](https://hackaday.io/project/17055-the-winkel-board)

Reddit
---
* [Thread-1](https://redd.it/58fwdf)
* [Thread-2](https://redd.it/5hioau)

FAQs
----
Coming Soon


Get in touch
---
* [Email](info@mintbox.in)
* [Facebook](https://facebook.com/winkelboards)
