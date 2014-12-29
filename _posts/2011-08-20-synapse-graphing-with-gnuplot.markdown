---
layout: post
status: publish
published: true
title: 'Synapse: Graphing with Gnuplot'
author:
  display_name: jcwoltz
  login: jcwoltz
  email: jc@jcwoltz.com
  url: http://www.jcwoltz.com/
author_login: jcwoltz
author_email: jc@jcwoltz.com
author_url: http://www.jcwoltz.com/
excerpt: I've been playing around with graphing and plotting of various sensor data.
  I also have been testing how batteries, my PCBs, and the Synapse Wireless RF Engines
  handle freezing temperatures. This post will focus on <a title="GNUplot" href="http://www.gnuplot.info/"
  target="_blank">http://www.gnuplot.info/</a>. I am currently using SNAP Connect
  to receive the RPC calls, but Portal can be used just as well.
wordpress_id: 259
wordpress_url: https://www.jcwoltz.com/?p=259
date: '2011-08-20 15:56:44 -0400'
date_gmt: '2011-08-20 19:56:44 -0400'
categories:
- Electronics
- SynapseWireless
tags: []
comments: []
---
<p>I've been playing around with graphing and plotting of various sensor data. I also have been testing how batteries, my PCBs, and the Synapse Wireless RF Engines handle freezing temperatures. This post will focus on <a title="GNUplot" href="http://www.gnuplot.info/" target="_blank">http://www.gnuplot.info/</a>. I am currently using SNAP Connect to receive the RPC calls, but Portal can be used just as well.<a id="more"></a><a id="more-259"></a></p>
<p>I have to thank the "Using Gnuplot" section of this <a href="http://www.ladyada.net/make/logshield/lighttemp.html" target="_blank">article on adafruit</a>. This helped me get going quickly. Jumping straight to the code:</p>
<h2>This is the SNAP Connect Code:</h2>
<pre>def loglm75aRawCalc(name, raw):
    """ Converts the raw reading from a LM75A Temp Sensor """
    if name == None:
        name = convertAddr(com.rpc_source_addr())
    intraw = int(raw)
    intC = intraw &gt;&gt; 5
    tC = intC / 8.0
    tF = calcCtoF(tC)
    eventString = str(tC) + "," + str(tF) + "," + name
    formattedString = time.strftime("%s") + "," + convertAddr(com.rpc_source_addr()) + "," + eventString
    print formattedString
    f = open('/root/jcCSVlm75.txt', 'a')
    f.write(formattedString + '\n')
    f.close()
    return tC
def calcCtoF(raw):
    fraw = float(raw)
    tempF = (fraw * 9)/5 + 32
    #print tempF
    return tempF
def convertAddr(addr):
    return binascii.hexlify(addr)</pre>
<h2> This is the gnuplot config file:</h2>
<pre>set term png size 1024, 768
set output "jccsvlm75a.png"
set datafile separator ","

set xlabel "Time"              # set the lower X-axis label to 'time'
set xtics rotate by -270       # have the time-marks on their side

set ylabel "Temp in F"
set ytics nomirror             # tics only on left side

set y2label "Temp in C"   # set the right Y-axis label
set y2tics border              # put tics no right side

set key box top left           # legend box
set key box linestyle 0

set xdata time                 # the x-axis is time
set format x "%H:%M:%S"        # display as time
set timefmt "%s"               # but read in as 'unix timestamp'

plot "jcCSVlm75.txt" using 1:4 with lines title "FTemp", \
 "jcCSVlm75.txt" using 1:3 axes x1y2 with lines title "CTemp"</pre>
<h2> To Create the Graph:</h2>
<pre> gnuplot plotlm75a.cfg</pre>
<p>This create the jccsvlm75a.png as defined in the gnuplot config file. Now the code used in snap connect can easily be modified to run in Portal. It can also be modified to log other type of data. For right now, take a look at this graph: <img class="alignnone" src="http://jcu.homelinux.org/rrd/jccsvlm75a.png" alt="" width="1024" height="768" /></p>
<p>I will update and post links to code for Portal, the nodes sending this data, and more. If any one has suggestions to improve the graphs, please send them in.</p>
