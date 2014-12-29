---
layout: post
status: publish
published: true
title: 'Synapse: Breakout Boards available for sale'
author:
  display_name: jcwoltz
  login: jcwoltz
  email: jc@jcwoltz.com
  url: http://www.jcwoltz.com/
author_login: jcwoltz
author_email: jc@jcwoltz.com
author_url: http://www.jcwoltz.com/
excerpt: 'The boards have now arrived for the Synapse Wireless RF Engine Brakout Boards.
  If anyone is interested in them, please contact me. '
wordpress_id: 54
wordpress_url: http://www.jcwoltz.com/?p=54
date: '2010-10-25 15:23:18 -0400'
date_gmt: '2010-10-25 19:23:18 -0400'
categories:
- Electronics
- SynapseWireless
tags: []
comments:
- id: 24
  author: 'majolsurf.net &raquo; ByteMaster: JTAG ISP Is Now Even More Affordable'
  author_email: ''
  author_url: http://majolsurf.net/wordpress/?p=1250
  date: '2010-11-07 04:25:26 -0500'
  date_gmt: '2010-11-07 09:25:26 -0500'
  content: "[...] I would be remiss if I didn&#8217;t mention JC Woltz, who is doing
    excellent work with the Synapse RF Engine breakout boards.  Synapse RF Engines
    are a Python-compatible alternative to the XBee.  Not only [...]"
- id: 206
  author: andy
  author_email: la.hinkle@sbcglobal.net
  author_url: ''
  date: '2011-02-08 12:40:20 -0500'
  date_gmt: '2011-02-08 17:40:20 -0500'
  content: "Could you add the following additions to your RF Engine protoboard.\r\n\r\n#1.
    4 evenly spaced mounting holes in all four corners of the board. (0.125 holes)\r\nReason:
    To mount the protoboard in an enclosure.\r\n\r\n#2. Have 0.01 sp headers on both
    sides of the RF engine instead of below the rf engine.\r\nThese headers would
    connect to the RF I/O.\r\nReason: You can add stacking headers or just put wires
    in the holes. (0.040 holes)\r\n\r\n#3. Places for current limiting resistors on
    all I/O pins. Since this RF engine I/O is programmable and if the\r\nuser connects
    this to another programmable device eg microcontroller then by having two outputs
    connected together (by accident) with a high on one and a low on the other will
    destroy the I/O pin. \r\nThese current limit resistors will prevent destruction
    of a $35 rf engine and or microcontroller."
- id: 208
  author: jcwoltz
  author_email: jc@jcwoltz.com
  author_url: http://www.jcwoltz.com/
  date: '2011-02-08 13:00:18 -0500'
  date_gmt: '2011-02-08 18:00:18 -0500'
  content: "Andy,\n\nThank you for your comments. This Breakout Board was essentially
    the first PCB I have even made. I agree with mounting holes and have added them
    to all recent boards.\n\n#2 Since the BOB(Breakout Board) I have included a 30
    pin header (16 pins on the left, 14 pins on the right side of the rfe) for the
    purpose of adding application specific add-on boards. It is sort of like the arduino
    shield idea, but I want anyone to be able to make their own add-on or even use
    proto board to do it. \n\n#3 I am trying to provide a cheap generic BOB. Yes,
    resistors do not cost that much, but does reduce the generic purpose. If you use
    a RF200 based on the ATMega128RFA1, it has 5v tolerant IO and uses less current.
    I will put a new post up soon on the new boards and direction.\n\nAgain, Thank
    you for your comment and suggestions."
- id: 209
  author: Peter Gorbounov
  author_email: pgo11@orange.fr
  author_url: ''
  date: '2011-02-14 11:57:54 -0500'
  date_gmt: '2011-02-14 16:57:54 -0500'
  content: "Hello Jack,\r\n1) I would be very glad to get a couple of boards for evaluation,
    but I am located in Europe...\r\n2) In your design, the F-antenna is obscured
    by the board from below. Did you remove the copper entirely from that area?"
- id: 210
  author: Andy
  author_email: la.hinkle@sbcglobal.net
  author_url: http://nowebsite
  date: '2011-02-14 16:48:33 -0500'
  date_gmt: '2011-02-14 21:48:33 -0500'
  content: Jack, what is the date / time frame on your new boards?
---
<p>The boards have now arrived for the Synapse Wireless RF Engine Brakout Boards. If anyone is interested in them, please contact me. <a id="more"></a><a id="more-54"></a></p>
<p><a href="http://www.jcwoltz.com/wp-content/uploads/2010/10/IMG00030-20101023-1624.jpg"><img class="alignnone size-medium wp-image-60" title="BOB-1f-top" src="http://www.jcwoltz.com/wp-content/uploads/2010/10/IMG00030-20101023-1624-300x225.jpg" alt="" width="300" height="225" /></a><a href="http://www.jcwoltz.com/wp-content/uploads/2010/10/IMG00029-20101023-1624.jpg"><img class="alignnone size-medium wp-image-59" title="BOB-1f-bottom" src="http://www.jcwoltz.com/wp-content/uploads/2010/10/IMG00029-20101023-1624-300x225.jpg" alt="" width="300" height="225" /></a></p>
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
<p>Here is a picture with a different voltage regulator:</p>
<p><a href="http://www.jcwoltz.com/wp-content/uploads/2010/10/IMG00031-20101024-1339.jpg"><img class="alignnone size-medium wp-image-61" title="IMG00031-20101024-1339" src="http://www.jcwoltz.com/wp-content/uploads/2010/10/IMG00031-20101024-1339-e1288035363230-260x300.jpg" alt="" width="260" height="300" /></a></p>
