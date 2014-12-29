---
layout: page
status: publish
published: true
title: BASE-v3i5
author:
  display_name: jcwoltz
  login: jcwoltz
  email: jc@jcwoltz.com
  url: http://www.jcwoltz.com/
author_login: jcwoltz
author_email: jc@jcwoltz.com
author_url: http://www.jcwoltz.com/
wordpress_id: 239
wordpress_url: https://www.jcwoltz.com/?page_id=239
date: '2011-06-03 15:26:54 -0400'
date_gmt: '2011-06-03 19:26:54 -0400'
categories: []
tags: []
comments: []
---
<p>The BASE version 3i5 is an evolution from the BOB and specific customer requests. The goal of the base is to provide the most commonly asked for features:</p>
<ul>
<li>Power/Voltage Regulation</li>
<li>Small Size and Small Power Consumption</li>
<li>Provides an EEPROM for offline storage</li>
<li>Provides a digital Temperature Sensor to read ambient air</li>
<li>Provides a TCXO RTC to wake node up from sleep. This can be used to wake many nodes at the same time.</li>
<li>Provide "Addon" headers. These addon headers can be used to stack the application specific board to the BASE board.</li>
<li>Provides and RS-232 level translation for RF Engine UART0 and UART1</li>
<li>Provides FTDI Headers if you want to use an FTDI Cable to connect to UART1. This is very handy for firmware upgrades.</li>
</ul>
<p>The BASE board was kept generic on purpose. The idea is to allow companies and individuals a quick and proven starting point for application development. Depending on the NODE function, the BASE board can be used by itself with an RF Engine. However if you need to add custom circuitry, that is what the addon headers are for. This will allow the total NODE package to remain small.</p>
<p>There are 3 sets of solder jumpers relating to I2c. These allow you to select RF100, RF200, or RF300 being plugged into the BASE board. The is a solder jumper above the RS-232 IC. When soldered to the left, it makes the RS-232 go into a low power mode when VAUX is turned off. When soldered to the right, it keeps the RS-232 active. There is a solder jumper labeled RTC_INT, this connect the INT pin from the RTC to GPIO_10 of the RF Engine. This solder jumper is provided in case you do not want to use the RTC_INT to wake from sleep and want to recover GPIO_10 for another purpose.</p>
<p>Hardware wise, the I2C address pins are tied to ground. No solder jumpers are provided for changing this.</p>
<p>&nbsp;</p>
<p>More to come....with pictures</p>
