---
layout: post
status: publish
published: true
title: 'Synapse: Users of RFEs, Why Re-invent the wheel?'
author:
  display_name: jcwoltz
  login: jcwoltz
  email: jc@jcwoltz.com
  url: http://www.jcwoltz.com/
author_login: jcwoltz
author_email: jc@jcwoltz.com
author_url: http://www.jcwoltz.com/
wordpress_id: 118
wordpress_url: http://www.jcwoltz.com/?p=118
date: '2011-03-21 16:56:05 -0400'
date_gmt: '2011-03-21 20:56:05 -0400'
categories:
- Electronics
- SynapseWireless
tags: []
comments:
- id: 349
  author: cbowen12345
  author_email: cbowen12345@yahoo.com
  author_url: ''
  date: '2011-03-27 15:59:33 -0400'
  date_gmt: '2011-03-27 19:59:33 -0400'
  content: "JC,\r\nI have been using your first version BOB.  It has worked well (even
    with my soldering technique).  What is the cost of the new BOB assembled?\r\n
    \ \r\nCbowen12345@yahoo.com"
- id: 350
  author: jcwoltz
  author_email: jc@jcwoltz.com
  author_url: http://www.jcwoltz.com/
  date: '2011-03-27 16:03:23 -0400'
  date_gmt: '2011-03-27 20:03:23 -0400'
  content: "Charles, This board is a BASE and not a BOB like you have. The new BASE
    board starts at $50 and goes down depending on quantity.\r\n-JC"
- id: 351
  author: jbaird
  author_email: joe@bus-informatics.com
  author_url: ''
  date: '2011-03-28 12:18:56 -0400'
  date_gmt: '2011-03-28 16:18:56 -0400'
  content: "How many do you have available?  plese let me know when you have the pricing!\r\n\r\nJoe"
- id: 352
  author: jcwoltz
  author_email: jc@jcwoltz.com
  author_url: http://www.jcwoltz.com/
  date: '2011-03-28 12:42:46 -0400'
  date_gmt: '2011-03-28 16:42:46 -0400'
  content: "Joe, \r\n\r\nI think cbowen12345 was asking about the Break Out Board
    in the previous post. Not this board. I am emailing you with details. But I guess
    I should have made this clear in the post, On this board was a test run for a
    company. On April 4th, I'll get more PCBs made. Pricing on this board really depends
    on how many people want them. Also what changes they would like to see.\r\n\r\n-JC"
---
<p>If you are a company or individual who uses Synapse Wireless RF Engines, how many times do you design a board with the same basic components? With the help and co-operation from some people around the world, here is the SNARF-BASE:</p>
<p style="text-align: center;"><a href="http://www.jcwoltz.com/wp-content/uploads/2011/03/IMG-20110315-00147.jpg">[gallery link="file" columns="2"]</p>
<p></a></p>
<p><a href="http://www.jcwoltz.com/wp-content/uploads/2011/03/IMG-20110315-00147.jpg"> </a></p>
<p><a href="http://www.jcwoltz.com/wp-content/uploads/2011/03/IMG-20110315-00147.jpg"></a></p>
<p><a href="http://www.jcwoltz.com/wp-content/uploads/2011/03/IMG-20110315-00147.jpg"> </a></p>
<p><a href="http://www.jcwoltz.com/wp-content/uploads/2011/03/IMG-20110315-00147.jpg"></a></p>
<p><a href="http://www.jcwoltz.com/wp-content/uploads/2011/03/IMG-20110315-00147.jpg"> </a></p>
<p><a href="http://www.jcwoltz.com/wp-content/uploads/2011/03/IMG-20110315-00147.jpg"></a></p>
<p><a href="http://www.jcwoltz.com/wp-content/uploads/2011/03/IMG-20110315-00147.jpg"> </a></p>
<p><a href="http://www.jcwoltz.com/wp-content/uploads/2011/03/IMG-20110315-00147.jpg"></a></p>
<p><a href="http://www.jcwoltz.com/wp-content/uploads/2011/03/IMG-20110315-00147.jpg"> </a></p>
<p><a href="http://www.jcwoltz.com/wp-content/uploads/2011/03/IMG-20110315-00147.jpg"></a></p>
<p><a href="http://www.jcwoltz.com/wp-content/uploads/2011/03/IMG-20110315-00147.jpg"> </a></p>
<p><a href="http://www.jcwoltz.com/wp-content/uploads/2011/03/IMG-20110315-00147.jpg"></a></p>
<p><a href="http://www.jcwoltz.com/wp-content/uploads/2011/03/IMG-20110315-00147.jpg"> </a></p>
<p><a href="http://www.jcwoltz.com/wp-content/uploads/2011/03/IMG-20110315-00147.jpg"></a></p>
<p>The SNARF-BASE v3h has these features:</p>
<ul>
<li>Voltage Regulation to 3.3 volts for the RF Engine with a protection diode</li>
<li>Has solder jumpers to select between RF100 or RF200 (even RF300)</li>
<li>Has 3 very useful I2C devices for almost any project onboard:
<ul>
<li>PCF2129A Realtime Clock with Interrupt to wake RFE from sleeep</li>
<li>LM75A Temperature Sensor</li>
<li>24LC256 EEPROM to store data. (Mainly used when out of range, but has other purposes)</li>
</ul>
</li>
<li>Has a RS232 driver on both UART0 and UART1</li>
<li>Has an Axillary voltage regulator used to shutdown sensors on demand</li>
<li>Uses standard spaced headers  for application specific addon boards that could be stacked</li>
</ul>
<p>The goal is to provide this board fully assembled and tested. This should allow companies/users to get started on their application faster. By including the headers, you only have to develop a small pcb for your project. (You could even use protoboard if you wanted).</p>
<p>&nbsp;</p>
<p>More projects and boards to come shortly. Although I have been quiet on the blog, I have been developing and testing boards and parts. Stay tuned.....</p>
<h2>UPDATE: 2011/03/28</h2>
<p>This board was done for a company. I am sold out, but will have more at the end of April. The newest design is not finalized yet. Now is the time to talk to me If you would like some of these boards, or see changes to these boards. I will order 40 updated PCBs. Again, If you are interested in this board and/or changes, contact me before April 4th. Changes so far:</p>
<ul>
<li>Changed RS232 driver to ICL3223EIVZ in order to save power in sleep modes</li>
<li>Move Temperature sensor out from under RF Engine</li>
<li>R4 (Addon Header Reserved Pin 4) connected to VIN after the diode, but before the voltage regulator. This is to provide application specific addon boards access to the VIN in case the addon board needs more than 3.3 volts.</li>
</ul>
