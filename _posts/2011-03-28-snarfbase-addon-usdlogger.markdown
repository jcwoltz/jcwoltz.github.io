---
layout: post
status: publish
published: true
title: 'Synapse: SNARF-BASE Add-on'
author:
  display_name: jcwoltz
  login: jcwoltz
  email: jc@jcwoltz.com
  url: http://www.jcwoltz.com/
author_login: jcwoltz
author_email: jc@jcwoltz.com
author_url: http://www.jcwoltz.com/
wordpress_id: 141
wordpress_url: http://www.jcwoltz.com/?p=141
date: '2011-03-28 00:00:30 -0400'
date_gmt: '2011-03-28 04:00:30 -0400'
categories:
- Electronics
- SynapseWireless
tags: []
comments: []
---
<p>The previous post highlighted the features of the SNARF-BASE v3h. The first add-on board that I have created for the base is a microSD data logger.</p>
<p>[gallery link="file"]</p>
<p>First, you'll have to forgive the sloppy hand assembly as this is a first prototype. Enough talk, lets get to the hardware features:</p>
<ul>
<li>ATMega32u4 MCU</li>
<li>microSD Socket</li>
<li>Mini-B USB Socket</li>
<li>Standard Add-on headers for BASE and other boards.</li>
<li>The chips SDA/SCL lines have a solder jumper to connect them to the SDA/SCL lines of the BASE board.</li>
<li>UART1 of the RFE is connected to the UART1 of the ATMega32u4</li>
<li>RGB LED to indicate various status</li>
</ul>
<p>Now to the software. This thing can have various bootloaders on it so you do not need an AVRISP programmer. My personal preference is the DFU bootloader, but there is a CDC bootloader, and maybe soon a HID bootloader. Dean Camera at <a title="LUFA" href="http://www.fourwalledcubicle.com/LUFA.php">http://www.fourwalledcubicle.com/LUFA.php</a> has done an excellect job with LUFA. The Board currently uses a slightly modified DFU Bootloader from LUFA to light a LED to let you know you are in bootloader mode.</p>
<p>The LUFA stack provides great usb projects and demos, but I also want to make this board compatible with <a title="Arduino" href="http://arduino.cc/en/Main/HomePage">Arduino</a>. Thankfully Paul Stoffregen at <a href="http://www.pjrc.com/">pjrc.com</a> has done some excellent work with arduino and the USB series of Atmel Chips. He has written <a href="http://www.pjrc.com/teensy/teensyduino.html">teensyduino</a>, which is an addon to the arduino environment. This allows you to use most of the arduino libraries available on this board. There are some moral/ethical/(legal?) problems using the teensyduino on a non teensy board. You have to rely on the drivers written by Paul when using teensyduino to connect to a computer.</p>
<p>Anyhow, This is just the first alpha of this board. Only 3 people will have a copy to beta test. The second alpha has already been sent off to the fab to fix some of the problems of this board.</p>
<p>If this board is something that interests you, and/or you would like to see changes please let me know. For starters the 5mm RGB led has been removed and replaced with surface mount LEDS. Also The second revision has solder jumpers to select RFE UART0 or UART1.</p>
<p><a href="https://www.jcwoltz.com/wp-content/uploads/2011/03/AtMEGA32u4-uSD-AddON-v01-brd.png"><img class="alignnone size-medium wp-image-163" title="AtMEGA32u4-uSD-AddON-v01-brd" src="https://www.jcwoltz.com/wp-content/uploads/2011/03/AtMEGA32u4-uSD-AddON-v01-brd-e1301257806606-285x300.png" alt="" width="285" height="300" /></a><a href="https://www.jcwoltz.com/wp-content/uploads/2011/03/AtMEGA32u4-uSD-AddON-v01-brd-pour.png"><img class="alignnone size-medium wp-image-164" title="AtMEGA32u4-uSD-AddON-v01-brd-pour" src="https://www.jcwoltz.com/wp-content/uploads/2011/03/AtMEGA32u4-uSD-AddON-v01-brd-pour-e1301257882178-300x229.png" alt="" width="300" height="229" /></a></p>
<p>&nbsp;</p>
