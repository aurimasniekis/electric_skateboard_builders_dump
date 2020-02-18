# Antispark from eskating.eu help

### Replies: 24 Views: 465

## \#1 Posted by: AgileCow Posted at: 2018-07-09T16:58:29.642Z Reads: 173

```
Hi guys!

Managed to screw up my antispark switch from eskating.eu. 
Does anyone know where the red thin wire should be soldered? 
![IMG_0684|375x500](upload://9e0M1v0bali7YvahEIQp1bbl36u.jpg)

It doesn't look like other switches I found references to in the forum.
```

---
## \#2 Posted by: goldenHusky Posted at: 2018-07-09T17:19:03.447Z Reads: 158

```
@fottaz 
10 chars
```

---
## \#3 Posted by: b264 Posted at: 2018-07-09T17:51:22.602Z Reads: 149

```
Ask the vendor
```

---
## \#4 Posted by: AgileCow Posted at: 2018-07-09T17:56:55.434Z Reads: 145

```
@b264 I already did, however I also know that Alberto is swamped after the accident he had, so I thought I'd shoot out the question here on the forum as well. 

Thanks for the tip though
```

---
## \#5 Posted by: willpark16 Posted at: 2018-07-09T17:59:28.904Z Reads: 145

```
Positive discharge would be my assumption
```

---
## \#6 Posted by: ARetardedPillow Posted at: 2018-07-09T19:15:15.847Z Reads: 127

```
Positive discharge as @willpark16 said, but the light is a 12v light which requires a 12v rail though. If you connect it straight to the positive discharge it might blow the light.
```

---
## \#7 Posted by: AgileCow Posted at: 2018-07-09T19:31:59.202Z Reads: 117

```
Yo, mr Pillow.

Thx for the help, I also noticed the 12v rating, hence the question. I don’t understand how to give the LED 12v, given the available components. Maybe it’s just connected to positive discharge and “hope it works”.

What do you think @ARetardedPillow @willpark16?
```

---
## \#8 Posted by: Hannes Posted at: 2018-07-09T20:01:40.667Z Reads: 108

```
You can't see any "residue" at any of the solder on the board where it might have been connected?
```

---
## \#9 Posted by: ARetardedPillow Posted at: 2018-07-09T20:02:29.597Z Reads: 103

```
Hmm can you find a resistor anywhere that the wire might be connected to?
```

---
## \#10 Posted by: Hannes Posted at: 2018-07-09T20:03:12.063Z Reads: 103

```
Actually, might not connect to the board? might be a connection like a loop on the switch since the heatshrink. or as @ARetardedPillow wrote, a resistor, but it's inside the heatshrink and it should be soldered to the power
```

---
## \#11 Posted by: ARetardedPillow Posted at: 2018-07-09T20:06:23.650Z Reads: 102

```
The switch will work fine as it is right now just that you have no LED, but just find a way to supply 12v to that wire and youre good to go
```

---
## \#12 Posted by: ARetardedPillow Posted at: 2018-07-09T20:07:05.485Z Reads: 97

```
Hmmm, I think there's a resistor inside the heatshrink aswell
```

---
## \#13 Posted by: AgileCow Posted at: 2018-07-10T05:20:12.879Z Reads: 87

```
@Hannes @ARetardedPillow thanks for all the feedback. 
I do have some residue on the positive discharge so I'm not too worried about that. Haven't found a resistor in the shrink wrap though. 

I think I might have some suitable resistor at home but I'm leaning more towards "bleep it, let's just solder it and go" :slight_smile:
```

---
## \#14 Posted by: ElskerShadow Posted at: 2018-07-10T05:54:11.614Z Reads: 82

```
I had the same problem with the antispark at eskating
I don't know why but you pay 50 € and you get the shittiest cables Alberto could find. My advice change every cable for stronger one because they will break All the time.
Do what other have said it's positive discharge!
```

---
## \#15 Posted by: fottaz Posted at: 2018-07-10T09:10:21.311Z Reads: 74

```
Hey man! The red wire goes on out positive. So the led will go on just when you push it.
```

---
## \#16 Posted by: AgileCow Posted at: 2018-07-10T09:15:44.554Z Reads: 73

```
Aah, ok, thx Alberto. 

So the risk to the LED is acceptable? It will receive a much higher voltage than the rated 12v.
```

---
## \#17 Posted by: koralle Posted at: 2018-07-10T09:38:50.778Z Reads: 73

```
Are you sure it's a 12v connection for the led? Some switches are rated for 48v and have different resistors inside. If it really is a 12v switch, use 2x16.5kohm resistors in parallel!
```

---
## \#18 Posted by: apollo383 Posted at: 2018-07-10T09:46:44.800Z Reads: 72

```
![image|665x500](upload://kyAjo4gIgdyThR6Og7blO4xS4TC.jpg) this is how I light up my led on the switch
```

---
## \#19 Posted by: apollo383 Posted at: 2018-07-10T09:48:29.484Z Reads: 72

```
![image|375x500](upload://1fwTJitiBnoj0omWq9hyyRurJzi.jpeg) you gonna need one of these to transfer the lower voltage
```

---
## \#20 Posted by: apollo383 Posted at: 2018-07-10T09:55:23.595Z Reads: 69

```
https://m.ebay.com/itm/100PCs-1-4W-1-5K-1500-OHM-Through-Hole-RESISTOR-Carbon-Film-250mW-5-250V-Axial/152058080074?epid=1866163783&hash=item23675e2b4a:g:ePgAAOSw~oFXE6Y1:sc:USPSFirstClass!60630!US!-1
```

---
## \#21 Posted by: apollo383 Posted at: 2018-07-10T10:00:54.340Z Reads: 66

```
![image|666x500](upload://hS3digMakNcHg4hbsWrjozoWkD3.jpeg)
```

---
## \#22 Posted by: AgileCow Posted at: 2018-07-11T05:36:15.401Z Reads: 47

```
Just FYI for everyone. 

The resistor was hidden under the shrinkwrap, and I managed to hook it all up again. I didn't have any spare resistors at home, so, lucky me :slight_smile:

Thanks for all the help!


/Ronny
```

---
## \#23 Posted by: koralle Posted at: 2018-07-11T06:34:14.051Z Reads: 46

```
Glue the resistors and heat shrink to the pcb! I think it wasn't your cable that broke but the leg of the resistor, which is incredibly frail. You don't want it to come loose again and short some random stuff it shouldn't.
```

---
## \#24 Posted by: fottaz Posted at: 2018-07-15T19:49:20.552Z Reads: 37

```
I see a side of the resistor it's not usable (it still be under the black heatshrink), you'd need another resistor of 1.5k or more (I'm soldering 2k to be safe with highest voltages) as other guys said! Sorry for the delay
```

---
