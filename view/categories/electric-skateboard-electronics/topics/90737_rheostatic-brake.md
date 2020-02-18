# Rheostatic brake

### Replies: 23 Views: 786

## \#1 Posted by: TOMAS Posted at: 2019-04-16T12:17:40.011Z Reads: 262

```
Hello all,

I have got a rheostatic brake for my electric skateboard project complimentary from the company I work with. I can't find any information about it online, does anyone here know what is it good for and how to connect it (series to the battery or parallel)?

Hope to find some answers here.

That is my first post here so please don't kill me if it is the wrong please the publisher my question...

Thanks.

![15554164847112099016529674869417|666x500](upload://uzf5jVYqL2qU9VhkBKyyLLrjcAG.jpeg)
```

---
## \#2 Posted by: Klaerke91 Posted at: 2019-04-16T12:21:01.913Z Reads: 255

```
[quote="TOMAS, post:1, topic:90737"]
rheostatic brake
[/quote]

heres a video - https://www.youtube.com/watch?v=RA4F01N1ZHY
```

---
## \#3 Posted by: Andy87 Posted at: 2019-04-16T12:33:32.336Z Reads: 245

```
might make sense just to copy the description under the video which is for 12S but looks like on the picture only for 10S:

Maytech MTBR1812 Rheostatic Brake


Battery: max. 12s


Operation voltage: 57V


Startup time: 200ms


Max current: 5A


Function: When regenerative voltage is higher than operation voltage, Rheostatic Brake starts working and reduces the reverse voltage to protect controllers. 
Size 70(L)*47(W)*19(H)mm
Volt 50V
Power Cable 20# AWG Length: 160mm 
Black and Red

If you start a trip from the top of a steep hill with a battery, the regenerative output voltage from the controller during high speed braking could exceed the maximum charging voltage of the battery, and under these circumstances, the battery's BMS to disconnect the charging supply in order to prevent the regenerative braking from overcharging the battery.

When regenerative braking voltage exceeding the maximum charging voltage of the battery, BMS switches off, regenerative braking energy cannot be absorbed by the battery, then the controller of the regenerative braking voltage will continue to rise. After the regenerative braking voltage reached 57V, the electronic switch inside the Rheostatic Brake will start, the energy will be released through special braking resistor, so the braking voltage will be limited. The controller will be protected.

When regenerative braking voltage exceeds maximum charging voltage of the battery, BMS will disconnect.
```

---
## \#4 Posted by: venom121212 Posted at: 2019-04-16T12:56:53.092Z Reads: 212

```
I connect mine parallel with battery and have had no issue. This was recommended by the manufacturer.
```

---
## \#5 Posted by: Andy87 Posted at: 2019-04-16T13:00:31.632Z Reads: 201

```
but did it also help you with something? could you run higher brake currents. if yes, how much compared to what you had before?
```

---
## \#6 Posted by: venom121212 Posted at: 2019-04-16T13:02:10.651Z Reads: 190

```
Theoretically I can run higher brake currents but my brakes are plenty stiff as is
```

---
## \#7 Posted by: rusins Posted at: 2019-04-16T15:11:10.135Z Reads: 168

```
So you just have a box taking up space in your enclosure for no reason? :laughing:
```

---
## \#8 Posted by: Andy87 Posted at: 2019-04-16T15:25:08.514Z Reads: 163

```
Well, if you have space in your box for a box, why not? 💁‍♂️
```

---
## \#9 Posted by: klaus79856 Posted at: 2019-04-16T15:26:03.314Z Reads: 165

```
Are these rheostatic brake modules based on Ultracaps ?
https://www.capcomp.de/en/ultracaps-consultancy-sales.html
```

---
## \#10 Posted by: rusins Posted at: 2019-04-16T15:26:17.411Z Reads: 158

```
As b264 once said: the more parts you have, the higher the chance of something breaking.
```

---
## \#11 Posted by: hyperIon1 Posted at: 2019-04-16T16:07:25.933Z Reads: 145

```
https://youtu.be/Rt0spqQtMKg
```

---
## \#12 Posted by: hyperIon1 Posted at: 2019-04-16T16:08:49.151Z Reads: 138

```
I couldn't help myself........
```

---
## \#13 Posted by: venom121212 Posted at: 2019-04-16T16:11:55.443Z Reads: 132

```
Nah, it's just taking up space for testing and feedback :sweat_smile:
```

---
## \#14 Posted by: hyperIon1 Posted at: 2019-04-16T16:48:45.490Z Reads: 128

```
It's not a critical component, so if it fails it doesn't shut down the system like a switch. As the Battery pack grows in size and power it will be something needed in the future, it will protect your esc and battery from spikes in current, most escs can handle it but your direct discharge battery may not.  Everything has limits
```

---
## \#15 Posted by: hyperIon1 Posted at: 2019-04-16T16:57:20.758Z Reads: 125

```
They do use 2 capacitors in the same principle as the ultra caps regen function but do not manage storage or current out like the ultra caps. the ultra caps can be used in principle, but cost-effective no. It's more for solar, wind and water generated power storage and supply systems that cost $$$$
```

---
## \#16 Posted by: hyperIon1 Posted at: 2019-04-16T17:32:34.716Z Reads: 124

```

that little bit there that says 10s or below, we discovered that for them when they sent out the first batch. Circuit FW limits are not set to accommodate 12s, the 12s will be in production soon. 

![44%20AM|386x222](upload://jM1WJdOfhYuztTnil11fdDty5YT.png) 

As for why? 

A quad hub motor set up or any quad out/in runner will slam the battery pack with a heavy current with all braking at the same time, yes the escs will regulate this, but flawlessly? it's a failsafe that if it fails your still safe, if it does its job your safer. 

case in point: current battery build 12s6p with Sanyo 20700c 35a cells intended to drive 4 TB DD motors with 2 unitys.
```

---
## \#17 Posted by: Vanarian Posted at: 2019-04-16T17:42:34.388Z Reads: 124

```
It's a good thing to have if it can withstand the excessive current, least time I saw this in motion it was a DIY solution from a Nordic guy who modded his pre built EUC. It would prevent brake cutting when battery was full, on top of protecting it from overvoltage AND overcurrent.

I'm waiting for the feedback, these things should have been around earlier.
```

---
## \#18 Posted by: mishrasubhransu Posted at: 2019-04-16T19:41:08.108Z Reads: 113

```
Just a pic.  
![IMG_20190415_225405|666x500](upload://3GVXD7qmXmhQUHsWkoyBlIg1UCE.jpeg)
```

---
## \#19 Posted by: cap7ainclu7ch Posted at: 2019-07-18T02:57:02.765Z Reads: 86

```
Sorry to bring up this older thread, but have there been any developments on this?  I'm really surprised these things aren't in every board already, especially from bigger brands like Boosted seeing as this is a pretty large safety issue for those that live in hilly regions.  

Can you literally just put one of these in parallel with your pack and be good to go?
```

---
## \#20 Posted by: venom121212 Posted at: 2019-07-18T12:08:12.686Z Reads: 75

```
Yes. It's that easy.

Here is why people don't use them regularly. If you hit your throttle for 3 seconds, you've most likely used enough electricity to mitigate the situation. Unless you're starting downhill from a steep hill at 100% battery, you will still have brakes. You will never regen more than you've used unless you're solely downhilling and using regen brake.
```

---
## \#21 Posted by: cap7ainclu7ch Posted at: 2019-07-19T01:19:41.725Z Reads: 62

```
Yeah its definitely an unlikely situation, but honestly even having to worry about it (even if the odds are low) is annoying to me.  Has anyone tested these and seen how well they work?  I assume it only works for a short period before overheating.
```

---
## \#22 Posted by: alexnz Posted at: 2019-07-19T03:18:26.856Z Reads: 54

```
Maybe I don't understand it correctly, but having that device to prevent charging the battery beyond a given voltage is nowhere near as appealing as a device that would dissipate the excess regen current that you can't feed to the battery. 
Such a thing would still give you some strong sustained brakes even on a weak 10S2P battery that can't handle much more than 4A charge.
```

---
## \#23 Posted by: venom121212 Posted at: 2019-07-19T13:13:12.307Z Reads: 47

```
Yes. I have wanted to try this. Theoretically you could set the brake current up to twice as high (parallel regen to battery) and not worry about it.

@cap7ainclu7ch I have been using my maytech one for about 1200 miles. I took it off to save weight when shipping and racing it and haven't put it back on since. I've noticed no difference but am also on a 10s5p 30q pack and my brakes don't draw more than my battery can handle.
```

---
