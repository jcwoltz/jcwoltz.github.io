---
layout: post
status: publish
published: false
title: PCBs back and next steps
author:
  display_name: jcwoltz
  login: jcwoltz
  email: jc@jcwoltz.com
  url: http://www.jcwoltz.com/
author_login: jcwoltz
author_email: jc@jcwoltz.com
author_url: http://www.jcwoltz.com/
excerpt: "The PCBs for LiPoly charging, LiPoly protection, RTC, and low power ADC
  are back. They have been assembled and testing has begun. The code has been written
  for arduino. SnapPy code written too...\r\n\r\n[gallery link=\"file\" columns=\"4\"]\r\n\r\n"
wordpress_id: 68
wordpress_url: http://www.jcwoltz.com/?p=68
date: '2010-11-25 10:36:02 -0500'
date_gmt: '2010-11-25 15:36:02 -0500'
categories:
- Uncategorized
tags: []
comments:
- id: 72
  author: jack
  author_email: jack_menchin@verizon.net
  author_url: ''
  date: '2010-12-03 20:58:48 -0500'
  date_gmt: '2010-12-04 01:58:48 -0500'
  content: "In a similar application with a regulator with a sense lead, I tied the
    lead to the voltage from the solar pannel.  \r\nAfter many months of using solar
    chargers and sleeping nodes, the 2 batteries which went low were due to other
    factors.  One had a bad cell in a pack of 3 cells in parallel (cheap Lipos are
    like any other cheap battery).  The other had dropped out of sleep cycle (snafu).\r\nJack"
- id: 201
  author: Tom
  author_email: tsand8444@gmail.com
  author_url: ''
  date: '2011-01-21 17:41:24 -0500'
  date_gmt: '2011-01-21 22:41:24 -0500'
  content: "I'm interested in becoming a beta tester for your PCBs and would ultimately
    like to purchase the \"finished product\".  Contact me at the email address submitted
    with this comment.\r\n\r\nTom"
- id: 202
  author: Tim
  author_email: tim@themarzs.com
  author_url: http://n/a
  date: '2011-01-24 09:33:36 -0500'
  date_gmt: '2011-01-24 14:33:36 -0500'
  content: "Hi,\r\n\r\nI'm interested in your project.  I like the look of this board,
    but also interested in your breakout board if you're willing to ship to Australia.\r\n\r\nTim"
- id: 203
  author: Matt
  author_email: skerbitz@yahoo.com
  author_url: ''
  date: '2011-01-27 00:38:34 -0500'
  date_gmt: '2011-01-27 05:38:34 -0500'
  content: Hi - interested in all that your doing - just wondering if you have any
    more of the plain BOBs for sale ?  Thx
---
<p>The PCBs for LiPoly charging, LiPoly protection, RTC, and low power ADC are back. They have been assembled and testing has begun. The code has been written for arduino. SnapPy code written too...</p>
<p>[gallery link="file" columns="4"]</p>
<p><a id="more"></a><a id="more-68"></a>These boards are being tested, then merged into one board. The next board is designed to fit into a case that can be used indoors or outdoors. If this is something that interests you, let me know. We would love to have more feed back or beta testers.</p>
<p>At this point, I can't take all of the credit. Serge Sozonoff as been a huge help in all of this. He initially started by providing ideas and use cases. Later he helped in board design and components. Now he is helping with all of it plus code. So I want to share credit where credit is due.</p>
<p>Let's start with an interesting board. The DS2764 whose pcb layout I owe a thank you to Serge Sozonoff. This IC tells you all kinds of information. Voltage, Current, Accumulated Current, charging, discharging, and more. It will also protect the battery from being discharged or charged too much. This is a good thing so that you do not need to constantly watch the battery level. Arduino code available at <a title="Arduino DS2764 Example" href="http://code.google.com/p/jctc-electronics/source/browse/trunk/Arduino/ds2764Test/ds2764Test.pde">Google Code site</a>. Snappy code also available at <a href="http://code.google.com/p/jctc-electronics/source/browse/#svn/trunk/SNAPpy">Google Code</a>.</p>
<p>Next is the PCF2129A, a low power TCXO RTC. This Temperature Compensated Crystal (Xtal) Oscillator Real Time Clock and Calendar support I2C-Bus or SPI-Bus interface. This IC was selected for low power usage and the integrated TXCO. We provide Snappy code to talk to this IC and also set the time from Portal.</p>
<p>The main board being tested ("Solar Base"), has the charging IC MCP73861 from MicroChip. The idea is to charge a LiPo battery from a solar panel. We included to voltage regulators. The main one is always one powering the rf engine or other components. The second regulator has its shutdown line connected to a GPIO on the rf engine. This could be used to power down sensors when not being read.  This board also holds the Synapse RF Engine. We are trying to keep this board generic and have provided headers for application specific add-on boards to stack on it.</p>
<p>Alright, that is a brief description of each board. We have been testing these boards over the past week. There are a couple of problems to fix on the next revision. The biggest problem of all is when the DS2764 hits an under voltage condition. Its response is to disable discharge and <strong>charge</strong>, then enter sleep mode. This is a problem as it is unable to self-recover. We apply power to the charger, but charging never starts. Even if the DS2764 did not disable charging, the MCP73861 still would not begin charging. At this point the MCP73861 sees the battery at 0 volts.</p>
<p>Another issue comes is when charging by a solar panel. With the MCP73861 we can set the fast charge rate. Let's assume a 100ma fast charge rate. When the sun is coming up in the morning, the solar panel does not have very much power available. The MCP73861 will try to pull more power than is available. As the MCP73861 increases its current pull above what the panel can handle, the voltage drops. Once the voltage dips around 4.7 volts, the Under Voltage Lockout kicks in on the MCP73861. This stops the chip from charging, and starts a cycle all over again. The other disadvantage of pre-setting the fast charge rate, is when the sun is all the way up. The charger is not using all of the available power. Due to this and other problems we are testing out two other chips, the LT3652 and the MCP73861.</p>
<p>The LT3652 is a multi composition battery charger designed to be powered from solar. Currently laying out the schematic to have a test batch made. The advantage it offers is the voltage regulation loop which automatically adjusts to use the power optimally. The MCP73871 also as its own advantages to offer. More on that later...</p>
<p>Here is a chart show the battery status and current consumption. This is a 900 mAh battery that started at full charge over 48 hours ago. The rf engine consumes around 65 ma while awake. It is configured to run for 10 seconds, then sleep for 3 minutes.</p>
<p><a href="http://www.jcwoltz.com/wp-content/uploads/2010/11/battchargemon-201011261327.png"><img class="size-medium wp-image-87 alignnone" title="battchargemon-201011261327" src="http://www.jcwoltz.com/wp-content/uploads/2010/11/battchargemon-201011261327-300x112.png" alt="" width="300" height="112" /></a></p>
