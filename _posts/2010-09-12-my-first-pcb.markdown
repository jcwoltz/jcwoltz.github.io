---
layout: post
status: publish
published: false
title: My first PCB
author:
  display_name: jcwoltz
  login: jcwoltz
  email: jc@jcwoltz.com
  url: http://www.jcwoltz.com/
author_login: jcwoltz
author_email: jc@jcwoltz.com
author_url: http://www.jcwoltz.com/
wordpress_id: 5
wordpress_url: http://www.jcwoltz.com/?p=5
date: '2010-09-12 17:26:34 -0400'
date_gmt: '2010-09-12 21:26:34 -0400'
categories:
- Electronics
- SynapseWireless
tags: []
comments:
- id: 2
  author: Hello world! | Tech and Electronics
  author_email: ''
  author_url: http://www.jcwoltz.com/?p=1
  date: '2010-09-12 16:20:17 -0400'
  date_gmt: '2010-09-12 20:20:17 -0400'
  content: "[...] This will also be a place about various electronics. To get the
    ball rolling here is a post about a Synapse Wireless Breakout Board.   This entry
    was posted in Uncategorized. Bookmark the [...]"
- id: 3
  author: Eric
  author_email: gericrogers@yahoo.com
  author_url: http://majolsurf.net/wordpress
  date: '2010-09-13 15:40:04 -0400'
  date_gmt: '2010-09-13 19:40:04 -0400'
  content: Nice!  "3 miles LOS" that's incredible!  Who are you using for your PCB
    manufacturing?
- id: 4
  author: jcwoltz
  author_email: jc@jcwoltz.com
  author_url: http://www.jcwoltz.com/
  date: '2010-09-13 15:43:15 -0400'
  date_gmt: '2010-09-13 19:43:15 -0400'
  content: "My first set is from http://www.dorkbotpdx.org/wiki/pcb_order\r\n\r\nIf
    everything turn out right, I plan on sending my next batch to <a href=\"http://www.seeedstudio.com/wiki/index.php?title=Opensourcepcb\"
    rel=\"nofollow\">seeedstudio</a> after some small modification. There is nothing
    wrong with the group pcb order, but at this size seeedstudio is cheaper. \r\n\r\n-J.C."
- id: 205
  author: Attu
  author_email: controlcraft@alaska.net
  author_url: ''
  date: '2011-02-08 03:45:28 -0500'
  date_gmt: '2011-02-08 08:45:28 -0500'
  content: "I like your battery charge SNAP with twin headers. How about a rs232 DTE
    configuration. I see the XBee version in Droids something like that? Give me some
    cost estimates i presume your not a tek charity.\r\nThanks"
---
<p>I've been working with these <a title="Synapse RF Engine" href="http://www.synapse-wireless.com/index.php?mainID=3&amp;subID=3&amp;type=product&amp;prodID=3">Synapse RF Engines</a>. The advantage over an XBee (<a title="Xbee Series 1" href="http://www.digi.com/products/wireless/point-multipoint/xbee-series1-module.jsp#overview">Series 1</a> and <a title="Xbee Series 2" href="http://www.digi.com/products/wireless/zigbee-mesh/xbee-zb-module.jsp#overview">Series 2</a>) is they are able to run python code. This allows the wireless modules to do more than pass serial data and pin status. The XBee modules have their place. I am a strong believer of using the right tool for the job and there is more than one correct way to do something. Both Synapse and XBee modules have 2mm pin spacing instead of the prototyping friendly 2.54mm spacing.</p>
<p>There is no shortage of breakout boards for XBee modules. Adafruit has their <a title="XBee adapter kit v1.1" href="http://www.adafruit.com/index.php?main_page=product_info&amp;cPath=29&amp;products_id=126">XBee Adapter kit</a>. Sparkfun has their <a title="XBee Explorer Regulated" href="http://www.sparkfun.com/commerce/product_info.php?products_id=9132">XBee Explorer Regulated</a>. Seeed Studio has their <a title="UartSB v2.2" href="http://www.seeedstudio.com/depot/uartsb-v22-a-much-more-powerful-usb-to-serial-converter-p-495.html?cPath=104_109">UartSB</a> which is my favorite FTDI replacement.<strong>UPDATE: <a href="http://www.seeedstudio.com/depot/uartsbee-v31-p-688.html?cPath=104_109">New UartSB released</a>. </strong> But there isn't a breakout board for the Synapse Wireless RF Engine close to $10.</p>
<p>So I decided to make a PCB.  My requirement for a breakout board were to be able to use it in a breadboard or plug an ftdi cable into them. I wanted to be able to select the uart and power source.</p>
<p>[gallery link="file"]</p>
<p>I added jumpers to be able to select which uart the FTDI will connect to. This also allows you to be able to reverse transmit and receive if you needed to. There is a jumper to power the wireless module from the ftdi or from a 3.3V LDO Regulator. The board has places for four 3 mm LEDs and a resistor network. These can be left off if the user has no need for them.</p>
<p>The next revision will have the ability to plug a 5V FTDI in and safely communicate with the wireless module.</p>
