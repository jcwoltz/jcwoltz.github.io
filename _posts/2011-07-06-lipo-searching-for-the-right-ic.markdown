---
layout: post
status: publish
published: true
title: 'LiPo: Searching for the right IC'
author:
  display_name: jcwoltz
  login: jcwoltz
  email: jc@jcwoltz.com
  url: http://www.jcwoltz.com/
author_login: jcwoltz
author_email: jc@jcwoltz.com
author_url: http://www.jcwoltz.com/
wordpress_id: 251
wordpress_url: https://www.jcwoltz.com/?p=251
date: '2011-07-06 17:19:39 -0400'
date_gmt: '2011-07-06 21:19:39 -0400'
categories:
- Electronics
tags: []
comments: []
---
<p>I have pretty much given up on all things Lithium Polymer (LiPo) related development. However, Serge Sozonoff has continued the development of a LiPo charger that can work from solar. He has continued to use the DS2764 as the fuel guage. Back in December Serge and I collaborated on a PCB that combined the MCP73871, DS2764, an RF Engine, and a few other ICs. I was never able to get mine assebled correctly, but he got his assembled and working. Here's a picture of it in the case it was designed for:</p>
<p><a href="https://www.jcwoltz.com/wp-content/uploads/2011/04/IMG_1576.jpg"><img class="size-thumbnail wp-image-194 alignnone" title="MCP73871 in case" src="https://www.jcwoltz.com/wp-content/uploads/2011/04/IMG_1576-150x150.jpg" alt="" width="150" height="150" /></a></p>
<p>It is with great pleasure to say that Adafruit has now <a title="Adafruit MCP73871 LiPo Charger" href="http://www.adafruit.com/products/390">released a LiPo charger based on the MCP73871</a>. I really think many people who charge LiPo batteries from a solar panel will enjoy this IC for two reasons. The first reason is the MCP73871 separates the system load from the charging of the battery.  That means you can run you system load without a battery if you need to. The second reason is the MCP73871 monitors the incoming voltage from the power source. The reason it does this is as it tried to draw too much current, the voltage will drop. When the voltage drops to a certain point, the MCP73871 will not try to pull more current than that. Without this feature, The solar panel, charging IC, and battery go into this endless loop of charging, then not charging. This is a big bonus for people wanting to use solar panels. There is one downside of the MCP73871 when compared to the MCP73861 and that is the MCP73871 is limited to a 6 volt maximum input. However the advantages that the MCP73871 offers outweigh this single disadvantage.</p>
<p>For those interested, the eagle files for the PCB in the picture are available at:</p>
<p><a href="http://jctc-electronics.googlecode.com/svn/trunk/Synapse/SolarPower/archive/SolarBase731-v02.brd">http://jctc-electronics.googlecode.com/svn/trunk/Synapse/SolarPower/archive/SolarBase731-v02.brd</a></p>
<p><a href="http://jctc-electronics.googlecode.com/svn/trunk/Synapse/SolarPower/archive/SolarBase731-v02.sch">http://jctc-electronics.googlecode.com/svn/trunk/Synapse/SolarPower/archive/SolarBase731-v02.sch</a></p>
<p>&nbsp;</p>
<p>Now to the real point of this post. Something has spark my interest/curiosity in LiPo charging and Fuel Guage monitoring. There are plenty of ICs for multicell LiPo or Li-Ion battery packs. I cant find a single IC for charging and monitoring of a single cell Lithium Polymer battery. If you know of any, please let me know.</p>
<p>The reason for this: I assume an integrated solution would know more about the state of the battery, the charge, the discharge rate, etc. Ideally, I would like something that seperates the battery pack charging from the system load. I would also like it to monitor the incoming voltage so it know when to back off the current draw. So If you know of anything like this, please let me know.</p>
<p>&nbsp;</p>
