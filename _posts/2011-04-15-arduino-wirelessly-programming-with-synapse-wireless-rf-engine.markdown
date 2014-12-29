---
layout: post
status: publish
published: true
title: 'Arduino: Wirelessly Programming with Synapse Wireless RF Engine'
author:
  display_name: jcwoltz
  login: jcwoltz
  email: jc@jcwoltz.com
  url: http://www.jcwoltz.com/
author_login: jcwoltz
author_email: jc@jcwoltz.com
author_url: http://www.jcwoltz.com/
wordpress_id: 188
wordpress_url: https://www.jcwoltz.com/?p=188
date: '2011-04-15 12:36:18 -0400'
date_gmt: '2011-04-15 16:36:18 -0400'
categories:
- SynapseWireless
- Arduino
tags: []
comments: []
---
<p>This one took a little longer than normal to do. Before I get to the details, I want to point out a few forum posts that helped. reblli1 had a function to <a href="http://forums.synapse-wireless.com/showpost.php?p=7095&amp;postcount=2">save on the number of writes to nvparams</a>. I'm sorry I forgot which post gave me the NVParameters to use for reliable serial. I am now able to RELIABLY program arduino boards at 57600 through avrdude or the arduino IDE.</p>
<p><strong>Disclaimer: I do not own a SNAP Protoboard. I am using my own breakout boards, but this should be doable through a SNAP Protoboard if that is what you have. </strong></p>
<p>I initially used three nodes to set this up, one being portal. Now that this is working, I only need the two nodes that talk to each other. Short details, Hook up UART1 to your computer with GPIO_10 on the DTR line. Hook up UART1 to your arduino with GPIO_9 on the reset pin.</p>
<p>&nbsp;</p>
<p>Modify these two scripts with your mac addresses:</p>
<p><a href="http://jctc-electronics.googlecode.com/svn/trunk/SNAPpy/datamode1.py">Arduino Node</a></p>
<p><a href="http://jctc-electronics.googlecode.com/svn/trunk/SNAPpy/datamode2.py">Computer Node</a></p>
<p>This will be updated with more details. But if you are looking for a quick way to get up and running, here it is.</p>
<p>Pictures of the Setup:</p>
<p>Computer side is a USB -&gt; 3.3v FTDI Breakout -&gt; BOB. Note The BOB UART jumpers were meant to mate with an Arduino or similar device, So I had to use jumper wires to cross-over the RX and TX singnals.</p>
<p>[gallery link="file"]</p>
<p>Pictures of the Arduino Setup included above. The Green BOB was used for the Arduino. The Blue BOB was used on the computer side with the FTDI Cable.</p>
<p>This has been tested to work with a Sparkfun Arduino Pro(Pictured), Arduino Duemilanove, Seeeduino Stalker, and a boarduino.</p>
<p>&nbsp;</p>
