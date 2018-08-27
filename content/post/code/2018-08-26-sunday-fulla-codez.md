---
day: '134'
title: Smart Greenhouse
date: '2018-08-26T11:38:09-07:00'
tags:
  - 100daysofcode
  - python
categories: 'circuits, hardware, arduino'
weight: 0
---
# Progress
- Mounted a light inside a chest
- Built a smart outlet with Arduino 

# Thoughts
I drew the schematic wrong and let some of the smoke out of the wires lol. I switched the hot instead of the neutral...but it was drawn like that in my schematic. So at least I built it accurately. After I fixed that, I was able to get it working. Only one outlet is connected to the relay now too. I'll work on that later. 

## Design
### Relay
<hr>

I'm using 4-port relay
- Port 1 - Lights (Normally closed)
- Port 2 - Pump (Normally open)
- Port 3 - Fan (Normally open)
- Port 4 - Not used

### Timer
<hr>
The timer to control lights will be set in code

### Pump
<hr>
Repurposed an old paper shredder for the water reservoir. I put a small water pump in it, and will control it with a YL-69 soil moisture sensor. If it gets too dry, pump some water into the pot.

### Fan
<hr>
Using an old computer fan. The DHT-11 sensor will turn the fan on if it gets too hot. 

# Links
- [Understanding Python's "with" statement](http://effbot.org/zone/python-with-statement.htm)
