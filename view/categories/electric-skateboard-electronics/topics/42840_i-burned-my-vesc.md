# I burned my Vesc

### Replies: 38 Views: 1861

## \#1 Posted by: Benja_man Posted at: 2018-01-05T10:43:21.347Z Reads: 285

```
Okaj, a couple months ago I replaced the cables (connecing the batteries with the vesc and a switch) with some thick silicone ones,. But I messed up the polarity of the connector on the vesc. When I connected the "new" cable and turned on the switch, some magic smoke came out of the vesc! I immediately dissconected everything.  Wires were hot, I touched the mosfets they were hot as well. I'm guessing i made a some sort of a short circut...

I want to know if I destroyed the whole Vesc or just the DVR chip? It would be cheaper just to replace he drv chip, but im worried other parts (on the vesc) are destroyed as well. If anyone knows what should I do, please tell. 
Also I'm broke as hell right now, iIcan't afford the new vesc...
```

---
## \#2 Posted by: pat.speed Posted at: 2018-01-05T10:50:43.936Z Reads: 276

```
Post some pics so we can see
```

---
## \#3 Posted by: CarlCollins Posted at: 2018-01-05T10:50:54.117Z Reads: 276

```
Hi Benja 

From where did you get that VESC from?
```

---
## \#4 Posted by: SimosMCmuffin Posted at: 2018-01-05T10:56:51.078Z Reads: 264

```
If you connected the negative and positive wires the wrong way, then the VESC is toast. You will have most likely blown the DRV and Mosfets at least.
```

---
## \#5 Posted by: Kug3lis Posted at: 2018-01-05T12:54:04.400Z Reads: 247

```
mcu too, as high voltage went thought ground pins and negative throughout resistors into adc pins
```

---
## \#6 Posted by: JohnnyMeduse Posted at: 2018-01-05T15:13:55.662Z Reads: 225

```
@Benja_man do you mind posting some pictures, I think there might be more than just the DRV that is burned. But If didn't blow any of the Trace, It could be repaired.
```

---
## \#7 Posted by: Benja_man Posted at: 2018-01-05T18:09:13.326Z Reads: 209

```
I bought my vesc from ebay, and it is Maytech brand.
```

---
## \#8 Posted by: Benja_man Posted at: 2018-01-05T18:45:04.582Z Reads: 203

```
<img src="/uploads/db1493/original/3X/5/e/5e9f45700932480c24c300334b18ac18873a1875.jpg" width="690" height="386"><img src="/uploads/db1493/original/3X/1/1/11a8d2a8a18d3570e585a519ba297454c1b131c0.jpg" width="690" height="386"><img src="/uploads/db1493/original/3X/f/6/f6493d946034f1cfc837c00f11533944e0c7f7c8.jpg" width="690" height="386"><img src="/uploads/db1493/original/3X/3/e/3eef2abc37c59f4c16b1c81055efcfde2a11cf0d.jpg" width="690" height="386"><img src="/uploads/db1493/original/3X/1/6/16b9421ee8a3bf145f414426596092ea424ff8d0.jpg" width="690" height="386"><img src="/uploads/db1493/original/3X/e/b/eba6f3cb0261e23d5ed555c6af7d626d1a9ac7e5.jpg" width="690" height="386"><img src="/uploads/db1493/original/3X/0/e/0e73f12173fc1850bbb3b1e0ba01d75d2ec709d4.jpg" width="690" height="386"><img src="/uploads/db1493/original/3X/a/7/a7b1658527bfaa02be569ca5378943c92a7d2a0a.jpg" width="690" height="386">
```

---
## \#9 Posted by: Benja_man Posted at: 2018-01-05T18:54:18.455Z Reads: 186

```
I closely checked every tiny part and I can't see any burned spots on the board or even drv chip. (I have no idea where the smoke came from if even it did at all, i dont remember clearly)

Also you should know that in the incident a cell in one of the 3S batteries died.. (the voltage on that cell is 0 and the battery   therfore doesn't provide any voltage at all (shorted maybe??) I seriously don't want any lipo fire trying to fix it cuz that shit is toxic af.
```

---
## \#10 Posted by: JohnnyMeduse Posted at: 2018-01-05T18:56:52.451Z Reads: 183

```
You could always try it, to see if it still power up, with a small 12V power pack.
```

---
## \#11 Posted by: Benja_man Posted at: 2018-01-05T18:57:30.443Z Reads: 184

```
I know that and it is the reason im so worried.. VESC's definitely weren't made for dumb mistakes like this.
```

---
## \#12 Posted by: Benja_man Posted at: 2018-01-05T19:02:12.561Z Reads: 173

```
I did that, but the motor didn't spin and i think that messed up the battery. I have set up the lower voltage limit, so it shouldn't spin anyway i think.
I also plugged it in my computer but no response, the computer didn't recognise it and leds didn't light up.
```

---
## \#13 Posted by: JohnnyMeduse Posted at: 2018-01-05T19:04:33.835Z Reads: 164

```
[quote="Benja_man, post:12, topic:42840"]
leds didn't light up.
[/quote]

So you did burn something...
```

---
## \#14 Posted by: Benja_man Posted at: 2018-01-05T19:45:06.620Z Reads: 149

```
I'm quite sure i burned sth but the question is if it is only drv chip that is burned or the whole VESC...
```

---
## \#15 Posted by: JohnnyMeduse Posted at: 2018-01-05T20:29:07.031Z Reads: 146

```
All the Voltage are controlled by the DRV, so if no light is powering up, there is probably some chance that they DRV is blown. 

It could also be a short-circuit over the 3.3V. 

Maybe you could start by probing with a Multimeter to see if any of the Voltages are shorted to the ground.
```

---
## \#16 Posted by: LAVAMAN Posted at: 2018-01-05T21:38:30.036Z Reads: 136

```
I just sent my non-working VESC to the board tech (user name thermalm16) and he fixed it for me in 1 day for $45.00. Worth every penny. If he can't fix it, it only costs you the shipping to find out.
```

---
## \#17 Posted by: JohnnyMeduse Posted at: 2018-01-05T21:59:33.601Z Reads: 135

```
Nice same price as I do ... :wink:
```

---
## \#18 Posted by: Benja_man Posted at: 2018-01-06T15:47:45.164Z Reads: 127

```
I need to know if my vesc is completely wasted, or can be repaired by replacing the drv chip. Because I can't afford to pay for repair if it won't work even then. I rather buy new one.
```

---
## \#19 Posted by: JohnnyMeduse Posted at: 2018-01-06T15:55:10.442Z Reads: 124

```
The problem is it could be more than just the DRV or something else other than the DRV. If you have a multi-meter on hand we could check out, the root cause of your problem. 

Or if you don't have any, you could still send it for repair.
```

---
## \#20 Posted by: Benja_man Posted at: 2018-01-06T16:02:47.617Z Reads: 118

```
I have a mulitmeter on me, but I'm not sure what to check. (where to put the "wires")
```

---
## \#21 Posted by: GrecoMan Posted at: 2018-01-06T16:03:23.830Z Reads: 107

```
they’re called probes.
```

---
## \#22 Posted by: Benja_man Posted at: 2018-01-06T16:11:57.555Z Reads: 109

```
I would appreciate if someone who is an expert, marks the pins where i need to check with my probes if anything is shorted. (where it has to conduct and where it doesn't)
If you need any closer images please tell me. (you can also show me a "blueprint" or electrical scheme of the VESC and tell me what to check)
```

---
## \#23 Posted by: JohnnyMeduse Posted at: 2018-01-06T16:22:45.383Z Reads: 106

```
First you can check if the Can Transceive is still good ?

https://www.electric-skateboard.builders/t/no-power-to-enertion-vesc/7600/11?u=johnnymeduse
```

---
## \#24 Posted by: JohnnyMeduse Posted at: 2018-01-06T16:25:04.632Z Reads: 105

```
And you can also check if you have 5v over the 5v pin, on one of the connector.

If you don’t have 5V, it is probably because the Drv is dead (since it is the one giving the 5V)

<img src="/uploads/db1493/original/3X/3/8/38c55011bd0e07c31b6b795d8ce8889b386a83f3.jpeg" width="666" height="500">
```

---
## \#25 Posted by: Benja_man Posted at: 2018-01-06T16:34:35.155Z Reads: 100

```
Ground and 5V pins are shorted
```

---
## \#26 Posted by: JohnnyMeduse Posted at: 2018-01-06T16:35:40.406Z Reads: 99

```
GND and 5V or GND and 3.3V... If it is GND and 5V YES the DRV is Dead
```

---
## \#27 Posted by: Benja_man Posted at: 2018-01-06T16:38:16.682Z Reads: 101

```
Yes obiously I know that the drv is dead, but do you know how to check other parts if they're shorted?
```

---
## \#28 Posted by: JohnnyMeduse Posted at: 2018-01-06T16:40:49.540Z Reads: 102

```
The DRV is the heart of it... you have to remove it and check the other because if it is not removed, it will only give you wrong data when you will probe other things.
```

---
## \#29 Posted by: Benja_man Posted at: 2018-01-06T16:44:20.559Z Reads: 101

```
Okay, I understand.
```

---
## \#30 Posted by: Benja_man Posted at: 2018-05-24T13:48:32.652Z Reads: 80

```
Hello people. I recieved a new drv chip and removed the old one. Someone sugested, i should check if other componetns are damaged, when the drv chip is not present on the pcb. So I'm asking you guys, if you can tell me, how to check if mcu (ARMwhatewer) is still working
```

---
## \#31 Posted by: ThermalM16 Posted at: 2018-05-24T16:33:00.586Z Reads: 77

```
So the main things you want to check for is a short on the 5v and 3.3v rails. Also, you don't have to go in the order I listed these in. You can test in any order.

Once you've verified those aren't shorted go ahead and test each gate resistor for the MOSFETs. Their values should be 4.7 and 39k Ohms, it's okay if they're off by a tiny bit. For example, I get 5.5 and 38.87k Ohms on my multimeter. 

Now you can test R40 through R51. These should all be 100 Ohms.

Next, go ahead and test R23, 24 and 32. These should be 39k Ohms.

Now that you've verified all of those are the correct values, go ahead and test your MOSFETs. You'll want to test source to drain, so pins to tab. Set your multimeter in diode test mode and put your red probe on the pins, pick one of the two middle ones to avoid confusion, and then place the black probe on the tab. You should get a reading somewhere around 0.4-0.6 since some multimeters will give different readings. If you have a short or 0.005 or something like that, you'll need to replace the MOSFET

And that's how you repair a VESC... more or less
```

---
## \#32 Posted by: Benja_man Posted at: 2018-05-24T18:16:22.131Z Reads: 72

```
Okay thanks for the quick anwser. I will test these tomorrow, because i dont have the burned vesc on me. I did some testing with my friend and first connected 12V on the V_SOURCE. But nothing happend. We figured out there is no 5V , so we decided to manually connect a power supply on 5v pins and the leds lit up. We also connected the whole thing to the computer and it did detect it! (so im guessing ARM is not damaged??)
Now im still not sure why there is no 5V... (do i need to solder the DRV chip back on or sth?)

I hope all the components you mentined are okay. :) I hope we can save this VESC
```

---
## \#33 Posted by: JohnnyMeduse Posted at: 2018-05-24T18:25:18.208Z Reads: 72

```
yeah the DRV as a internal regulator that provide the 5v, and as @ThermalM16 check the resistor specialy the 100ohms from r48 to r51 the are the one that usully got damage.
```

---
## \#34 Posted by: Benja_man Posted at: 2018-05-24T18:27:30.412Z Reads: 68

```
thanks for the info. will check em
```

---
## \#35 Posted by: ThermalM16 Posted at: 2018-05-25T03:56:49.963Z Reads: 67

```
Also I would never recommend artificially powering the 5V or 3.3V rail. If it’s done correctly you won’t have any issues, but out of the tons of VESCs I’ve repaired, I’ve never needed to do that. Also make sure the VESC is not powered during testing!!
```

---
## \#36 Posted by: Benja_man Posted at: 2018-05-25T07:30:52.495Z Reads: 61

```
turns out 2 middle mosfets are fried...
```

---
## \#37 Posted by: Benja_man Posted at: 2018-05-27T09:45:19.213Z Reads: 50

```
Does anybody know where can I order IRFS7530-7PPBF MOSFETS, from an european warehouse? I don't want to pay ridicilous shipping just to order them from America (I live in europe).
I checked farnell and many other websites, but they mostly don't have them in stock. Any recomendations where to get them from?
```

---
## \#38 Posted by: banjaxxed Posted at: 2018-05-29T23:35:15.881Z Reads: 41

```
Farnell does free shipping, tried mouser?
```

---
