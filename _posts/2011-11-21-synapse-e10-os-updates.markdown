---
layout: post
status: publish
published: false
title: 'Synapse: E10 OS updates'
author:
  display_name: jcwoltz
  login: jcwoltz
  email: jc@jcwoltz.com
  url: http://www.jcwoltz.com/
author_login: jcwoltz
author_email: jc@jcwoltz.com
author_url: http://www.jcwoltz.com/
excerpt: "One of the pieces that Synapse Wireless make is the <a title=\"Snap Connect
  E10\" href=\"http://www.synapse-wireless.com/index.php?mainID=3&amp;subID=10&amp;type=product&amp;prodID=10\">Snap
  Connect E10</a>. I will call this the E10 for short. The E10 is an ARM926 platform
  running Linux. It has an RF Engine in it and runs a piece of software called SNAP
  Connect. Slowly over a couple of months I have been updating the Linux pieces of
  the E10. These updates are primarily to support more USB wifi and cellular data
  modem, but they also update most of the core utilities. This post is meant as a
  point in time documentation of the changes from the factory image to what I have.\r\n\r\nDetails
  below...\r\n\r\n"
wordpress_id: 267
wordpress_url: https://www.jcwoltz.com/?p=267
date: '2011-11-21 19:29:01 -0500'
date_gmt: '2011-11-22 00:29:01 -0500'
categories:
- SynapseWireless
tags: []
comments: []
---
<p>One of the pieces that Synapse Wireless make is the <a title="Snap Connect E10" href="http://www.synapse-wireless.com/index.php?mainID=3&amp;subID=10&amp;type=product&amp;prodID=10">Snap Connect E10</a>. I will call this the E10 for short. The E10 is an ARM926 platform running Linux. It has an RF Engine in it and runs a piece of software called SNAP Connect. Slowly over a couple of months I have been updating the Linux pieces of the E10. These updates are primarily to support more USB wifi and cellular data modem, but they also update most of the core utilities. This post is meant as a point in time documentation of the changes from the factory image to what I have.</p>
<p>Details below...</p>
<p><a id="more"></a><a id="more-267"></a></p>
<p>&nbsp;</p>
<table>
<tbody>
<tr>
<th></th>
<th>Factory</th>
<th>Updated To</th>
</tr>
<tr>
<td>Buildroot Version</td>
<td>2010.02</td>
<td>2011.11-git</td>
</tr>
<tr>
<td>Linux Kernel</td>
<td>2.6.33</td>
<td>3.0.9(3.1.0 soon)</td>
</tr>
<tr>
<td>Target Architecture Variant</td>
<td>generic_arm</td>
<td>arm926t</td>
</tr>
<tr>
<td>Target ABI</td>
<td>OABI</td>
<td>EABI</td>
</tr>
<tr>
<td>uClibc C library Version</td>
<td>0.9.30.2</td>
<td>0.9.31.x</td>
</tr>
<tr>
<td>Binutils Version</td>
<td>2.20</td>
<td>2.21</td>
</tr>
<tr>
<td>GCC Compiler Version</td>
<td>4.3.4</td>
<td>4.3.x</td>
</tr>
<tr>
<td>BusyBox Version</td>
<td>1.13.x</td>
<td>1.19.3</td>
</tr>
<tr>
<td>Python Version</td>
<td>2.6.6</td>
<td>2.7.2</td>
</tr>
</tbody>
</table>
<p>There are many other updates, but those are the highlights. This <a href="http://forums.synapse-wireless.com/showthread.php?t=1796">thread over on the forums</a> has more details about where to download and how to install. One of the HUGE benefits is that I release my entire setup publicly. Using GitHub, this <a title="E10-buildroot" href="https://github.com/jcwoltz/E10-buildroot">repository</a> can be downloaded by anyone. If you are an individual or a company looking to customize your E10, you can download my repository. Then you can customize it and build it. A couple of companies have already picked up my repository to use for their own custom builds. The <strong>one and only</strong> thing that I ask is this: If you find bugs or have issues, please let me know so they can be fixed. It would be nice if you let me know you are using my repo and/or build, but it is not necessary.</p>
<p>If you are looking for more USB wireless support, more USB Cellular modem support, updated applications, or just the ability to customize what you have on the E10, then download the repo and build an image.</p>
