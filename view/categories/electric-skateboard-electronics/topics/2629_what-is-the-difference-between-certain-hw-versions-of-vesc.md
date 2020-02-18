# What is the difference between certain HW versions of VESC?

### Replies: 2 Views: 1197

## \#1 Posted by: Chewy Posted at: 2016-04-26T19:26:32.256Z Reads: 134

```
Just out of interest, because I'm currently trying to build a dual powered skateboard. What is the difference between 4.7 HW and 4.10 + HW versions?

Thanks very much!
```

---
## \#2 Posted by: Blasto Posted at: 2016-04-26T21:27:43.229Z Reads: 115

```
http://vedder.se/forums/viewtopic.php?f=6&t=124

[quote=" Benjamin Vedder, post:0, topic:0"]
4.0 to 4.5
* Redesign, added CAN bus, moved things around, added i2c temp sensor

4.5 to 4.6
* Changed i2c temp sensor to ntc resistor

4.6 to 4.7
* Changed FETs and voltage divider resistors to measure up to 60V

4.7 to 4.8
* Moved traces and capacitors around to make it more robust.
* Changed some pins (hall 3 I think)

4.8 to 4.10
* Moved some traces around
* Added hardware SPI to the comm connector and added an extra pin
* Changed ADC pins for the SPI support. This is why loading the wrong firmware is dangerous here - the current snese ADC lines have moved and the wrong firmware won't provide any feedback for the current control loop.

4.10 - 4.12 are very similar and use the same firmware. The difference from 4.10 to 4.11 is that I made a trace thicker, and the difference from 4.11 - 4.12 is that I added a capacitor to GVDD on the DRV8302
[/quote]
```

---
