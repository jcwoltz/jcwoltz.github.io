---
layout: post
status: publish
published: true
title: 'My First PCB: The verdict'
author:
  display_name: jcwoltz
  login: jcwoltz
  email: jc@jcwoltz.com
  url: http://www.jcwoltz.com/
author_login: jcwoltz
author_email: jc@jcwoltz.com
author_url: http://www.jcwoltz.com/
excerpt: My first PCB came in the mail. It looks good. Some things sure look different
  in real life than when zoomed in on the screen.
wordpress_id: 33
wordpress_url: http://www.jcwoltz.com/?p=33
date: '2010-09-27 19:53:26 -0400'
date_gmt: '2010-09-27 23:53:26 -0400'
categories:
- Electronics
- SynapseWireless
tags: []
comments: []
---
<p>My first PCB came in the mail. It looks good. Some things sure look different in real life than when zoomed in on the screen.<a id="more"></a><a id="more-33"></a></p>
<p><a href="http://www.jcwoltz.com/wp-content/uploads/2010/09/Synapse-BOB-1c-Bottom.jpg"><img class="alignnone size-medium wp-image-39" title="Synapse-BOB-1c-Bottom" src="http://www.jcwoltz.com/wp-content/uploads/2010/09/Synapse-BOB-1c-Bottom-300x225.jpg" alt="" width="300" height="225" /></a><a href="http://www.jcwoltz.com/wp-content/uploads/2010/09/Synapse-BOB-1c-topRFEngine.jpg"><img class="alignnone size-medium wp-image-40" title="Synapse-BOB-1c-topRFEngine" src="http://www.jcwoltz.com/wp-content/uploads/2010/09/Synapse-BOB-1c-topRFEngine-300x225.jpg" alt="" width="300" height="225" /></a></p>
<p>Things to change:</p>
<ul>
<li>The 2mm headers should have a little bit more copper. The drill size and placement is good.</li>
<li>Add a place for a smaller voltage regulator</li>
<li><span style="text-decoration: line-through;">Add a diode or something to drop the 5 volt tx down to 3.3 for the rx on the rf engine.</span> Strictly 3.3V, no logic level translation yet.</li>
<li>Removed all the leds except one. Put a 0603 pad for resistor. Put a solder jumper to select None/GPIO0/GPIO1.</li>
<li>Re-arranged components.</li>
<li>Added extra breadboard holes to allow 900 mil, 600 mil, 400 mil, and 100 mil spacing. Sensors or components could also be soldered directly to the board.</li>
</ul>
<p>Here is the layout for the new board. I have sent this off for manufacture. I will receive 10 blue and 10 green of this board. I would expect these at the end of October. If anyone needs these sooner, I can have a batch run, but will cost more.</p>
<p><a href="http://www.jcwoltz.com/wp-content/uploads/2010/09/synapse-BOB-1f.png"><img class="alignnone size-medium wp-image-36" title="synapse-BOB-1f" src="http://www.jcwoltz.com/wp-content/uploads/2010/09/synapse-BOB-1f-274x300.png" alt="" width="274" height="300" /></a></p>
<p>Here are the ordering options I am offering:</p>
<ol>
<li>Bare PCB Only $3 Green, $4 Blue</li>
<li>PCB + 2 samtec headers $6 Green, $7 Blue</li>
<li>PCB + following components: $9 Green, $10 Blue
<ul>
<li>2 Samtec MMS-112-01-T-SV headers</li>
<li>1 MC33269T-3.3G Low Drop Out Voltage Regulator</li>
<li>1 0603 Green LED</li>
<li>1 0603 Resistor</li>
<li>3 Shut/Jumper blocks (used to select uart and power source)</li>
<li>2 100uF Capacitors</li>
<li>2 100nF (0.1uF) Capacitors</li>
<li>2 Diodes</li>
<li>1 40 pin male breakaway header</li>
</ul>
</li>
</ol>
