---
layout: post
status: publish
published: false
title: 'Synapse: PCBs under development'
author:
  display_name: jcwoltz
  login: jcwoltz
  email: jc@jcwoltz.com
  url: http://www.jcwoltz.com/
author_login: jcwoltz
author_email: jc@jcwoltz.com
author_url: http://www.jcwoltz.com/
wordpress_id: 229
wordpress_url: https://www.jcwoltz.com/?p=229
date: '2011-06-02 23:30:39 -0400'
date_gmt: '2011-06-03 03:30:39 -0400'
categories:
- SynapseWireless
tags: []
comments: []
---
<p>Hello again, it has been a long time since I've updated this site. I have been busy working with individual companies and making PCBs to their design requests. This process usually takes a week or two of emails back and forth to get the final design they want. Then it takes about 2-3 weeks for the boards to be fabricated and mailed to me. Then up to a week for me to assemble, test, and ship the finished product to the customer. If this is something you are interested in, please contact me.</p>
<p>One of the requests I get fairly often is a board that charges LIPO/LI-Ion batteries from various power sources. Solar is the most common. Working with Serge taught me a bit with our earlier boards. Serge currently has prototype boards for charging and "fuel guage" of the batteries. They are coming along nicely. I would expect to have a finished product within a month. As these are still in proto-type and will have slight changes, now is the time to get involved if you want something specific.</p>
<p>Personally, I have been focused on two areas. Improving the BASE board and improving/updating the underlying linux on the E10. The Base board is available now for $45 a piece + shipping on total order. The BASE board is intended to provide the basics needed for an RF Engine mesh network (sleepy or otherwise). The BASE board is 2 inches x 2.2 inches. It includes voltage regulation, RTC with interrupt to wake RF Engine, 24LC256 EEPROM for offline storage, LM75A Temp Sensor, and a RS-232 level converter. It also include addon/stacking headers. These headers can be used to put your application specific board on top.  One such addon module is the atmega32u4 microSD Logger. (More details in a future post.)</p>
<p>On the E10. The E10 is great for what it does, but I would like to see it do more. I am working to update its buildroot environment. I would like to be able to package the extra software in .ipk files. This will allow users to run "opkg update &amp;&amp; opkg install socat" or whatever program they need to install. This is more of a personal goal, but if Synapse Wireless decides to pick it up and run with it, that is ok with me.</p>
<p>Serge has been working very hard to create "bridge" devices (for lack of a better term) between diverse SNAP networks over the internet. We are currently able to do this using an E10 and openvpn. He is working to create a solution for Hobbyist/DIY market where they do not need an E10 to accomplish this. There are some exciting software and hardware development in the works.</p>
<p>So, if anything of this interest you, give either one of us a contact through email or comment.</p>
<p>Also, I will get some pictures of completed boards and documentation up soon. If there are an HOWTOs, board development, and anything else you would like to see, just let us know.</p>
