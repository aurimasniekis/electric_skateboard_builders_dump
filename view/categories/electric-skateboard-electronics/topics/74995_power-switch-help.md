# Power switch help!

### Replies: 13 Views: 179

## \#1 Posted by: KrisKraanen Posted at: 2018-11-17T14:33:36.499Z Reads: 65

```
![IMG_20181117_152937|666x499](upload://NPvT4Vs9YETmXbfq5U0eACsxgI.jpeg) 
I had a switch and it broke, now i want solder up a new one but i need a resister but i can't figure out what resister this is company told me 1k but when i went to buy it it didn't look the same
```

---
## \#2 Posted by: KrisKraanen Posted at: 2018-11-17T14:39:01.344Z Reads: 63

```
![IMG_20181117_153834|375x499](upload://eLNyLPcqEuQWaKVJaKIxIbKvx81.jpeg)
```

---
## \#3 Posted by: goldenHusky Posted at: 2018-11-17T14:40:19.489Z Reads: 59

```
What voltage has your battery? Do you also know the rated voltage of the led or maybe even the rated current?
```

---
## \#4 Posted by: KrisKraanen Posted at: 2018-11-17T14:43:46.226Z Reads: 60

```
im running 8s but its the switch you get with the flipsky vesc but im changing the switch to a diffrent 5pin latching switch 
http://www.onpow.com/en/product/product1824.html
```

---
## \#5 Posted by: KrisKraanen Posted at: 2018-11-17T14:44:48.376Z Reads: 58

```
changing to this one https://electricboardsolutions.com/collections/switches/products/led-switch
```

---
## \#6 Posted by: goldenHusky Posted at: 2018-11-17T14:54:18.511Z Reads: 47

```
You are good with any resistor from 1100 Ohm to 2200 ohm, rated dissipation power of at least half a watt.
That values are only valid for a 8s battery with a 12V led.
```

---
## \#7 Posted by: KrisKraanen Posted at: 2018-11-17T15:23:28.698Z Reads: 43

```
You sure? Do you perhaps know why its there?
```

---
## \#8 Posted by: amazingdave Posted at: 2018-11-17T16:44:17.319Z Reads: 41

```
It’s there to drop the voltage for and limit the current through the indicator LED.
```

---
## \#9 Posted by: KrisKraanen Posted at: 2018-11-17T18:18:17.225Z Reads: 36

```
I don't know anything about resistors ![IMG_20181117_191503|666x500](upload://ewsOPWemt541FUmc4Sx52cG9AIb.jpeg) Is this one usable?
```

---
## \#10 Posted by: swimmydude Posted at: 2018-11-17T19:55:33.435Z Reads: 25

```
Blue resistors are slightly annoying to decode because it's harder for me to tell which colors are which. I'm not 100% certain but I believe the colors are as followed: red, yellow, black, black, gold. That means it's 240 ohms. I'm not sure if that color combo is a valid one in a resistor or not, but regardless it is not quite the 1.1k - 2.2k range goldenHusky stated. If you mean usable as in if it still works, then idk. The only way you can be certain if a resistor is still viable is using a multimeter.
```

---
## \#11 Posted by: KrisKraanen Posted at: 2018-11-17T20:13:25.774Z Reads: 19

```
![46480031_2329915880628529_4159249052455665664_n|690x469](upload://8nKKM1ysPiq5x04i6kvihEooIv1.png) i got this from the manufacture of the original, but the resistor in the first picture isn't a 1k am i right?
```

---
## \#12 Posted by: ElectricCoast Posted at: 2018-11-17T20:20:47.419Z Reads: 17

```
There is a resistor color code that you can look up to determine what the resistor is.
```

---
## \#13 Posted by: KrisKraanen Posted at: 2018-11-17T20:24:40.040Z Reads: 18

```
then it tells me 10 ohm.... so that cant be right
```

---
