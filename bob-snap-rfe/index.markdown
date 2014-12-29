---
layout: page
status: publish
published: true
title: Breakout Board for Synapse Wireless RF Engine
author:
  display_name: jcwoltz
  login: jcwoltz
  email: jc@jcwoltz.com
  url: http://www.jcwoltz.com/
author_login: jcwoltz
author_email: jc@jcwoltz.com
author_url: http://www.jcwoltz.com/
wordpress_id: 175
wordpress_url: https://www.jcwoltz.com/?page_id=175
date: '2011-03-28 21:38:42 -0400'
date_gmt: '2011-03-29 01:38:42 -0400'
categories: []
tags: []
comments: []
---
<p>Hello,</p>
<p>I have been making various circuit boards for <a href="http://www.synapse-wireless.com/">Synapse Wireless</a> <a href="http://www.synapse-wireless.com/index.php?mainID=3&amp;subID=3&amp;type=product&amp;prodID=3">RF Engines</a>. If you are unfamiliar with Synapse or their RF Engines, they have an <a href="http://www.synapse-wireless.com/index.php?mainID=3&amp;subID=30&amp;type=default">overview video</a>. Lately I have stopped assembling PCBs, but I still design boards. If you are interested in boards I have or customs boards, go ahead and contact me. Since I do this as a hobby, I am not charging commercial prices. All of my boards designs are released under the Open Source license <a title="CC BY-SA 3.0" href="http://creativecommons.org/licenses/by-sa/3.0/">CC BY-SA 3.0</a>.</p>
<p><a href="http://creativecommons.org/licenses/by-sa/3.0/"><img class="alignnone" title="CC BY-SA 3.0" src="http://i.creativecommons.org/l/by-sa/3.0/88x31.png" alt="CC BY-SA 3.0" width="88" height="31" /></a></p>
<div><a href="http://www.solarbotics.com/products/39255/"><img class="alignright" title="Solarbotics breakout board" src="http://content.solarbotics.com/products/photos/2a0d0834b93c9c26eb76c035d5d0a2bd/med/39255-img_0153.JPG" alt="" width="192" height="144" /></a><br />
Solarbotics now makes an affordable<a href="http://www.solarbotics.com/products/39255/"> breakout board</a>. This board breaks out the 2.0 mm RF Engine Headers into hobbyist friendly 2.54mm (0.1 inch) headers. Picture in red.Please check them out and support them.</div>
<h2>Breakout Board:</h2>
<p><a href="https://www.jcwoltz.com/wp-content/uploads/2011/02/IMG-20110315-00143-e1300975930465.jpg"><img class="size-thumbnail wp-image-119 alignleft" title="SNAP-BOB-11g-top" src="https://www.jcwoltz.com/wp-content/uploads/2011/02/IMG-20110315-00143-e1300975930465-150x150.jpg" alt="" width="150" height="150" /></a>The details and status of the current Breakout board can be found <a href="https://www.jcwoltz.com/2011/02/synapse-breakout-boards-updated/">on this page</a>. The Breakout Board (BOB for short) is designed to be flexible and have multiple purposes. The main purpose is to put an RF Engine (RF100/RF200/RF300) on it. The BOB then breaks out the RF Engine pins to 2 rows of headers per set of RF Engine pins. RF Engine pins 1-12 have two rows of pin headers, pins 13-24 have two rows of pin headers. This board can be used as a simple breakout board for the RF Engine and plug into a breadboard, plug into a custom boards, or have sensors soldered directly into the pin headers. The BOB can have a 3.3 volt regulator populated. It can have 3.5 mm screw terminal to supply power to the voltage regulator. The BOB also include a place to plug in a <a title="FTDI Basic Breakout - 3.3V" href="http://www.sparkfun.com/products/9873">3.3v FTDI Basic</a> <a title="Older FTDI Basic Breakout - 3.3V" href="http://www.sparkfun.com/products/8772">breakout</a> or <a title="Modern Device USB BUB II" href="http://shop.moderndevice.com/products/bub_ii">compatible</a>. This board has been used by many people as their gateway node, Wireless Arduino Programmer, and simple sensor nodes. For other options, please check out SolarBotics line of products: <a href="http://www.solarbotics.com/search/?query=synapse&amp;x=0&amp;y=0">http://www.solarbotics.com/search/?query=synapse&amp;x=0&amp;y=0</a></p>
<h2>BASE Board:</h2>
<p><a href="https://www.jcwoltz.com/wp-content/uploads/2011/03/IMG-20110315-00147-e1300740913949.jpg"><img class="alignleft size-thumbnail wp-image-125" title="SNARF-BASE-v3h-top" src="https://www.jcwoltz.com/wp-content/uploads/2011/03/IMG-20110315-00147-e1300740913949-150x150.jpg" alt="" width="150" height="150" /></a>The details and status of the current BASE Board can be found <a href="https://www.jcwoltz.com/2011/03/synapse-users-of-rfes-why-re-invent-the-wheel/">on this page</a>.</p>
<p>The goal of the BASE board is to handle some standard functions that most application built on RF Engines need. Outside of the RF Engine area are pins for add-on or stacking headers. These add-on headers allow you to use the same BASE board for all of you needs, then create application specific add-on boards. The headers are a standard 0.1 inch (2.54 mm) pitch. This allows you to use proto board if you wanted.</p>
<h2>E10 OS Updates:</h2>
<p>Over the past few months, I have been updated the core OS for the Synapse Wireless E10. The primary purpose is to add more USB WiFi and USB Cellular modem support. As part of the process, everything has been updated. The linux kernel has been upgraded from 2.6.33 to 3.0.12 which adds quite a few drivers. The core biuldroot has been updated. This brings many updates to busybox, python, utilities, and too many others to list. If interested, please email me or contact me in this <a href="http://forums.synapse-wireless.com/showthread.php?t=1796">forum</a>.</p>
