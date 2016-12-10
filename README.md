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

### Hardware

The Knit board has both 5V and 3.3V power rails. Both, 5V and 3.3V, are made available on the dual pin headers, but **please note that the controller pins are all 3.3V logic.** Supplying any of the pins more than 3.3V will likely result in a bricked board.

The 5V is used by

- LM1117 linear regulator IC
- CP2102 USB to serial converter

The 3.3V is used by

- AW-CU300 WiFi module
- W25Q32 Winbond Flash

The above setup allows one to power the board using an external 5V when developing an application, and switch to a 3.3V source, like a lithium ion battery, when deploying the application. The voltage regulator and the USB to serial converter is not necessary for normal operation of the WiFi module and flash memory, as long as you have a stable 3.3V power source.  

If you want to save some more power, you can get rid of the power LED resistor. That'll knock off a few mA. Of course, the nice red LED won't show your powered on status once you do this. **Please note that removing a resistor has the risk of damaging nearby tracks/connections if you are not careful. Please avoid doing this if you are not sure.**

### Input sources

You can power up Winkel Board using

- 5V through USB

### Consumption

Coming soon...

Hardware
---

Knit is open source hardware. There are a few definitions of OSHW, but what it means to us is that everything that one would need to make Knit is made available to everyone under a permissive license.

Knit is licensed under the MIT License. You can find text of the license [here](https://github.com/Makerville/knit/blob/master/LICENSE). All the files can be found on our [GitHub](http://github.com/makerville/knit/blob/master/hardware).


### Major components
The Knit board consists of the following major hardware components -

| Function | Company | Part No| Package|Datasheet
|:-:|:-:|:-:|:-:|:-:|
| WiFi | Azurewave | AW-CU300 | 64 pin LGA|-|
| Flash | Winbond | W25Q32 | SOIC-8| <a href="http://www.elinux.org/images/f/f5/Winbond-w25q32.pdf" target="_blank">Link</a>
| USB to UART | Silicon Labs | CP2102| 28 pin QFN | <a href="https://www.silabs.com/Support%20Documents/TechnicalDocs/CP2102-9.pdf" target="_blank">Link</a>
| Regulator | TI | LM1117| SOT 223|<a href="http://www.ti.com/lit/ds/symlink/lm1117.pdf" target="_blank">Link</a>

### Interfaces
We have the following buttons and LEDs onboard the Knit -

|Interface | Function | Connected to|Silkscreen Identifier|
|:-:|:-:|:-:|:-:|
|Button | Reset | RESET_N| RESET|
|Button | Boot/User | GPIO16/27| BOOT|
|LED | User | GPIO40|Blink!|
|LED | Power | 3V3 rail|pwr|

### Pin Headers
We have the following pin headers onboard the Knit -

| Pin count | Function |Silkscreen Identifier|
|:-:|:-:|:-:|
|16| GPIO breakout | \m/|
|16| GPIO breakout | knit|
|4 | Advanced debugging using [Serial Wire Debug](http://www.arm.com/products/system-ip/debug-trace/coresight-soc-components/serial-wire-debug.php)| SWD|

### Certifications
The Azurewave module that is being used is certified as follows -

- [FCC ID TLZ-CU300](https://fccid.io/TLZ-CU300)
- CE
- IC ID 6100A-CU300
- NCC ID CCAI15LP1350T2

<img src="https://makerville.io/knit/img/knit-module-bottom.jpg" width="470" ></img>


### Antenna

The Azurewave module, and hence the Knit board, has a PCB antenna as the internal antenna, and it also has a uFl connector if you would like to get better range with an external antenna.


Videos
===

### Create AWS IoT thing and certificates
In this screen capture, checkout how to create a new IoT thing by signing in to your AWS account.

&nbsp; <iframe width="470" height="315" src="https://www.youtube.com/embed/hOc-iZcmv9E?list=PLIYfgNqDE8r2XNkXMqbaiF0iBbli7cNYz" frameborder="1" allowfullscreen></iframe>

### Provision and push events to AWS IoT
In this video see how to connect to AWS using the keys that we generated in the previous video and then send a push button event to the AWS IoT device shadow.

&nbsp; <iframe width="470" height="315" src="https://www.youtube.com/embed/CFwY_jNb59s?list=PLIYfgNqDE8r2XNkXMqbaiF0iBbli7cNYz" frameborder="1" allowfullscreen></iframe>

Products w/ 88MW300
===

The Knit is based on the Marvell 88MW300 WiFi microcontroller. This is an industrial grade SoC which is being used to make all sorts of consumer applications, even battery operated ones.

### Teardowns

Some of the commercially available products that have been made using the 88MW300 WiFi microcontroller-
<table style="width:100%">
  <tr>
    <td>Hello Barbie</td>
    <td><a href="http://www.somersetrecon.com/blog/2015/11/20/hello-barbie-security-part-1-teardown" target="_blank">Teardown from Somerset Recon</a></td>
    <td>This one uses the same module as Knit, AW CU300</td>
    <td>See it in action <a href="https://www.youtube.com/watch?v=RJMvmVCwoNM" target="_blank">here</a></td>
  </tr>
  <tr>
    <td>Xiaomi Yeelight</td>
    <td><a href="http://www.miui.com/thread-4260673-1-1.html" target="_blank">Teardown from miui.com (in Chinese)</a></td>
    <td>This one uses a Mi module with 2MB of onboard flash</td>
    <td>See it in action <a href="https://www.youtube.com/watch?v=x0RCSBAH6gE" target="_blank">here</a></td>
  </tr>
</table>

### Software frameworks

The Knit is capable of running the following frameworks. Please note that one needs to contact Marvell/respective framework provider to get access to the source code and documentation.

- Google Weave
  - [88MW300 is the first MCU platform to support Google Weave.](http://www.marvell.com/company/news/pressDetail.do?releaseID=7659)
- Apple's HomeKit.
  - [HomeKit SDK](http://www.marvell.com/microcontrollers/wi-fi-microcontroller-platform/home-kit/)

Misc
====

Mailing List
---

  <form action="//makerville.us12.list-manage.com/subscribe/post?u=064c1b6c971f765e25f2d4c66&amp;id=8d99ecc3e3" method="post" id="mc-embedded-subscribe-form" name="mc-embedded-subscribe-form" class="validate" target="_blank" novalidate>
    <div id="mc_embed_signup_scroll">
      <div class="mc-field-group">

<p> &nbsp; &nbsp; Email:    </p>
   &nbsp; &nbsp; <input type="email" value="" name="EMAIL" class="required email" id="mce-EMAIL"><br/>
      </div>
      <div id="mce-responses" class="clear">
  <div class="response" id="mce-error-response" style="display:none"></div>
  <div class="response" id="mce-success-response" style="display:none"></div>
      </div>   
      <div class = "one-half column" style="position: absolute; left: -5000px;" aria-hidden="true"><input type="text" name="b_064c1b6c971f765e25f2d4c66_8d99ecc3e3" tabindex="-1" value=""></div>
      <div class="clear"> <br/> &nbsp;<input type="submit" value="Subscribe" name="subscribe" id="mc-embedded-subscribe" class="button"></div>
    </div>
  </form>

FAQs
----
- Is Knit OSHW (Open Source Hardware) ?
  - Yes, we have released the schematic and PCB files under the [MIT](https://github.com/Makerville/knit/blob/master/LICENSE) license. You can find the files [here](https://github.com/Makerville/knit/tree/master/hardware).
- When will it be available ?
  - Knit is available now . [Buy Now >][order]
- What will be the price?
  - For early access developers the price will be 999₹ / $14.99
- Where can I get more support ?
  - For SDK related issues, you can join the Gitter [chat](https://gitter.im/marvell-iot/aws_starter_sdk) or raise an [issue](https://github.com/marvell-iot/aws_starter_sdk/issues)


Acknowledgements
------------

- PCB design by [Rohit Gupta](http://rohitg.in/about/)
- Logo by [Cassie McKown](https://thenounproject.com/mckowncr/) under [CC by 3.0 US](http://creativecommons.org/licenses/by/3.0/us/)

Projects we <3 & use
---

- ARM GCC toolchain
- OpenOCD
- KiCad EDA
- Eclipse C/C++ IDE
- Flatdoc site generator by [Rico Sta. Cruz](http://ricostacruz.com/)



[project]: https://github.com/makerville/knit
[order]: https://makerville.io/knit/early-access

Get in touch
---
