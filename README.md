# lwrf-pylink
Python script to listen for LightwaveRF energy monitor values and input into Emoncms.

This is a simple Python script that I put together to help input energy usage data from a LightwaveRF energy monitor into Emoncms (http://emoncms.org) where I can create dashboards and run reports on power usage, etc.  In order to use this you will need both a LightwaveRF WiFiLink and energy monitor devices (http://lightwaverf.com).

This script listens on UDP port 9761 for the output of the energy monitor device and then parses the data and using the Emoncms API inputs it as a feed.  You will need to create an Emoncms API key to be able to write into a feed.  I run this then from using a screen session in Linux, but there's now reason it could not be run in Windows.

By the way to code for inputting feeds was based off of the emoncms pylink script here: https://github.com/emoncms/development/blob/master/Tutorials/Python/PyLink/pylink.py

The Python may not be that great as this is my first foray into it, so I do apologise...  I'll update this over time if needed.
