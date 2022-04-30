---
title: "Door activated halloween lights"
last_modified_at: 2022-04-30T11:50:00-08:00
categories:
  - Personal Project
tags:
  - Software
  - Hardware
  - 
---

# Problem

While hosting a halloween party, I wanted to make our bathroom an experience. A few hours before the party, I realized that I had everything needed to make our bathroom turn blood red when the door was closed. 

# Solution

Using wiz wifi activated lights, a python API for said wiz lights, an arduino, and a button circuit; I cobbled together a solution. Since it was only a few hours before the party, I didn't have time to buy a proper contact switch. So rigged together a circuit with a large button and connected it to an arduino, which I wedged above the door frame in the bathroom. I ran a long usb to a laptop running a python script which communicated to the arduino via serial communication and connected to the wiz lights using their API. 


# Result
This resulted in a room that appeared to have normal lighting when walking in and turned very red when the door was closed. Further in the bathroom, the bath tub appeared to be filled with blood, with candles and pentagram above the bathtub. We were going for a creepy ritual look. 

Additionally to this, I wish I had time to also trigger a speaker to play something cheery and cheesy like the monster mash when the door was open, and something creepy like ritual chanting when the door closed. But I unfortunately didn't have enough time with this being a last minute project.