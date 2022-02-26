---
layout: post
status: publish
published: false
title: 'QuickRef: Synapse Wireless Pin Mappings'
author:
  display_name: jcwoltz
  login: jcwoltz
  email: jc@jcwoltz.com
  url: http://www.jcwoltz.com/
author_login: jcwoltz
author_email: jc@jcwoltz.com
author_url: http://www.jcwoltz.com/
wordpress_id: 97
wordpress_url: http://www.jcwoltz.com/?p=97
date: '2011-02-02 09:59:21 -0500'
date_gmt: '2011-02-02 14:59:21 -0500'
categories:
- SynapseWireless
tags: []
comments: []
---
<p>Mainly A quick Reference for myself. This information was gathered from the "SNAP Hardware Technical Manual" version 1.3 DOC# 600-101.01D. Unfortunately It now turns out this document disagrees with the "SNAP Reference Manual" version 2.4 DOC# 600-0007G.</p>
<p><span style="color: #ff6600;">Public Message to Synapse Wireless: If you would provide this, I would not need to.</span></p>
<p>But, in the meantime, here is the side-by-side comparison of RF Engine pin outs. If it helps you, please leave a comment.</p>
<table border="0" cellspacing="0" cellpadding="0" width="759">
<col width="64"></col>
<col width="124"></col>
<col width="198"></col>
<col width="172"></col>
<col width="64"></col>
<col width="73"></col>
<col width="64"></col>
<tbody>
<tr height="20">
<td width="64" height="20">pin num</td>
<td width="124">rf100</td>
<td width="198">rf200</td>
<td width="172">rf300</td>
<td width="64">I2C</td>
<td width="73">SPI</td>
<td width="64"></td>
</tr>
<tr height="20">
<td height="20" align="right">1</td>
<td>GND</td>
<td>GND</td>
<td>GND</td>
<td></td>
<td></td>
<td></td>
</tr>
<tr height="20">
<td height="20" align="right">2</td>
<td>GPIO0_TPM1CH2</td>
<td>GPIO0 OC0A OC1C PCINT7 PB7</td>
<td>GPIO0 ADC17 P2.1 SDA</td>
<td>rf300-sda</td>
<td></td>
<td></td>
</tr>
<tr height="20">
<td height="20" align="right">3</td>
<td>GPIO1_KBI0</td>
<td>GPIO1 OC1B PCINT6 PB6</td>
<td>GPIO1 ADC18 P2.2 SCL</td>
<td>rf300-scl</td>
<td></td>
<td></td>
</tr>
<tr height="20">
<td height="20" align="right">4</td>
<td>GPIO2_KBI1</td>
<td>GPIO2 OC1A PCINT5 PB5</td>
<td>GPIO2 ADC19 P2.3</td>
<td></td>
<td></td>
<td></td>
</tr>
<tr height="20">
<td height="20" align="right">5</td>
<td>GPIO3_RX_UART0</td>
<td>GPIO3 RXD0 PCINT8 PE0</td>
<td>GPIO3 ADC20 P2.4</td>
<td></td>
<td></td>
<td></td>
</tr>
<tr height="20">
<td height="20" align="right">6</td>
<td>GPIO4_TX_UART0</td>
<td>GPIO4 TXD0 PE1</td>
<td>GPIO4 ADC21 P2.5</td>
<td></td>
<td></td>
<td></td>
</tr>
<tr height="20">
<td height="20" align="right">7</td>
<td>GPIO5_KBI4_CTS0</td>
<td>GPIO5 OC3B INT4 PE4</td>
<td>GPIO5 ADC22 P2.6</td>
<td></td>
<td></td>
<td></td>
</tr>
<tr height="20">
<td height="20" align="right">8</td>
<td>GPIO6_KBI5_RTS0</td>
<td>GPIO6 OC3C INT5 PE5</td>
<td>GPIO6 ADC0 P0.0 VREF</td>
<td></td>
<td></td>
<td></td>
</tr>
<tr height="20">
<td height="20" align="right">9</td>
<td>GPIO7_RX_UART1</td>
<td>GPIO7 RXD1 INT2 PD2</td>
<td>GPIO7 ADC5 P0.5 UARTRX</td>
<td></td>
<td></td>
<td></td>
</tr>
<tr height="20">
<td height="20" align="right">10</td>
<td>GPIO8_TX_UART1</td>
<td>GPIO8 TXD1 INT3 PD3</td>
<td>GPIO8 ADC4 P0.4 UARTTX</td>
<td></td>
<td></td>
<td></td>
</tr>
<tr height="20">
<td height="20" align="right">11</td>
<td>GPIO9_KBI6_CTS1</td>
<td>GPIO9 CTS1 ICP1 PD4</td>
<td>GPIO9 ADC3 P0.3 CTS</td>
<td></td>
<td></td>
<td></td>
</tr>
<tr height="20">
<td height="20" align="right">12</td>
<td>GPIO10_KBI7_RTS1</td>
<td>GPIO10 RTS1 ICP3 INT7 CLKO</td>
<td>GPIO10 ADC2 P0.2 RTS</td>
<td></td>
<td></td>
<td></td>
</tr>
<tr height="20">
<td height="20" align="right">13</td>
<td>GPIO11_AD7</td>
<td>GPIO11 ADC0 SCL PF0</td>
<td>GPIO11 ADC16 P2.0</td>
<td>rf200-scl</td>
<td></td>
<td></td>
</tr>
<tr height="20">
<td height="20" align="right">14</td>
<td>GPIO12_AD6</td>
<td>GPIO12 ADC1 SDA PF1</td>
<td>GPIO12 ADC15 P1.7</td>
<td>rf200-sda</td>
<td>rf300-mosi</td>
<td>rf100-mosi</td>
</tr>
<tr height="20">
<td height="20" align="right">15</td>
<td>GPIO13_AD5</td>
<td>GPIO13 ADC2 DIG2 PF2</td>
<td>GPIO13 ADC13 P1.5</td>
<td></td>
<td>rf300-sclk</td>
<td>rf100-sclk</td>
</tr>
<tr height="20">
<td height="20" align="right">16</td>
<td>GPIO14_AD4</td>
<td>GPIO14 XCK0 AIN0 PE2</td>
<td>GPIO14 ADC14 P1.6</td>
<td></td>
<td>rf300-miso</td>
<td>rf100-miso</td>
</tr>
<tr height="20">
<td height="20" align="right">17</td>
<td>GPIO15_AD3</td>
<td>GPIO15 ADC4 TCK MISO PF4</td>
<td>GPIO15 ADC6 P0.6 CNVSTR</td>
<td></td>
<td>rf200-miso</td>
<td></td>
</tr>
<tr height="20">
<td height="20" align="right">18</td>
<td>GPIO16_AD2</td>
<td>GPIO16 ADC5 TMS SCLK PF5</td>
<td>GPIO16 P2.7</td>
<td></td>
<td>rf200-sclk</td>
<td></td>
</tr>
<tr height="20">
<td height="20" align="right">19</td>
<td>GPIO17_AD1</td>
<td>GPIO17 ADC6 TDO MOSI PF6</td>
<td>GPIO17 (GPIO_0)</td>
<td>rf100-sda</td>
<td>rf200-mosi</td>
<td></td>
</tr>
<tr height="20">
<td height="20" align="right">20</td>
<td>GPIO18_AD0</td>
<td>GPIO18 ADC7 TDI PF7</td>
<td>ANT_A</td>
<td>rf100-scl</td>
<td></td>
<td></td>
</tr>
<tr height="20">
<td height="20" align="right">21</td>
<td>VCC</td>
<td>VCC</td>
<td>VCC</td>
<td></td>
<td></td>
<td></td>
</tr>
<tr height="20">
<td height="20" align="right">22</td>
<td>PTG0/BKDG</td>
<td>GPIO19 OC3A AIN1 PE3</td>
<td>C2D</td>
<td></td>
<td></td>
<td></td>
</tr>
<tr height="20">
<td height="20" align="right">23</td>
<td>RESET</td>
<td>RESET</td>
<td>RESET</td>
<td></td>
<td></td>
<td></td>
</tr>
<tr height="20">
<td height="20" align="right">24</td>
<td>GND</td>
<td>GND</td>
<td>GND</td>
<td></td>
<td></td>
<td></td>
</tr>
</tbody>
</table>
