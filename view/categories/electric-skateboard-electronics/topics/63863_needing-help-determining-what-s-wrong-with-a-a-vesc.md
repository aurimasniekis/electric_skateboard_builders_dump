# Needing help determining what’s wrong with a a VESC

### Replies: 13 Views: 240

## \#1 Posted by: erod998 Posted at: 2018-08-05T00:10:39.772Z Reads: 79

```
Hey everyone. I got a TorqueBoards 4.12 VESC. Worked great, until one day I accidentally shorted a motor wire and boom blew up a mosfet. No big deal, got ready to order a new one. However, the VESC Tool said I had a DRV error. So, added a DRV ago my cart. I now can’t get the VESC to connect to the PC at all after removing the bad MOSFET. The CPU and DRV get very warm. I was getting 5v and 3.3v out of the P3 jumper. The board itself is drawing .116 amps off my lab power supply at 30 volts. Anyone have any ideas on which parts to check for functionality or error? Keep in mind that the MOSFET actually caught fire, it was out of my board luckily.
```

---
## \#2 Posted by: ThermalM16 Posted at: 2018-08-05T03:50:12.518Z Reads: 66

```
Hi @erod998 it sounds like you have a short somewhere. Is the blue light turning on on your VESC? Also, did you replace the DRV yet?
```

---
## \#3 Posted by: erod998 Posted at: 2018-08-05T04:28:04.290Z Reads: 62

```
I have the blue light, and have not replaced the DRV. Waiting on Mouser. I do not have the light that turns on when USB is attached. I have removed the DRV, should I try turning the VESC on without it or will that make it worse.
```

---
## \#4 Posted by: strattos Posted at: 2018-08-05T04:40:29.081Z Reads: 60

```
Typically when motor wires are shorted it blows the DRV. Replace it.
```

---
## \#5 Posted by: ThermalM16 Posted at: 2018-08-05T04:42:50.159Z Reads: 57

```
Don’t turn it on without it. The DRV powers the MCU and all of the logic on your VESC, it would be pointless to turn it on while that’s missing, and also I’m not entirely sure if anything bad would happen
```

---
## \#6 Posted by: ThermalM16 Posted at: 2018-08-05T04:45:29.207Z Reads: 51

```
Also there isn’t a light that turns on when the USB is attached. The MCU turns on the green light once it boots up, and the red light is for faults. It’s possible you killed the MCU, but that’s not a very common scenario unless you shorted something while probing your VESC
```

---
## \#7 Posted by: erod998 Posted at: 2018-08-05T04:47:28.060Z Reads: 48

```
What would cause the CPU to get warm and not communicate over USB after shorting the motor?

I am going through and checking all resistor values, and if need be I have a capacitor tester. However I doubt the capacitors have anything to do with it, maybe some resistors especially on the Mosfet circuit blew too?
```

---
## \#8 Posted by: strattos Posted at: 2018-08-05T05:06:46.202Z Reads: 47

```
It's not a cap and define what you mean by CPU and warm?
```

---
## \#9 Posted by: erod998 Posted at: 2018-08-05T05:09:42.436Z Reads: 45

```
The ARM STM32F4. I guess I should have called it a MCU. Before I removed the DRV, when I plugged the VESC the MCU was very warm, I'd say 180 degrees. Didn't measure it. Is it fried since it was powered by a fried DRV or just shorted at the time it was powered? I will probably order one anyways, since I haven't placed it yet.
```

---
## \#10 Posted by: strattos Posted at: 2018-08-05T05:13:02.158Z Reads: 43

```
Well if it's 180 Fahrenheit it's not that out of the normal Imo if it's Celsius welp idk.

It seems everytime someone shorts a motor wire they have to replace the DRV, at least that my experience reading this forum for the last couple years. I'd replace the DRV first and see if it works.
```

---
## \#11 Posted by: erod998 Posted at: 2018-08-05T05:17:01.185Z Reads: 43

```
Awesome, thanks so much. I'll get the DRV switched and update this topic if it fixes it. 

Thanks guys!
```

---
## \#12 Posted by: erod998 Posted at: 2018-08-11T18:00:40.962Z Reads: 34

```
Ok, Update:
Replaced DRV. After, found that MCU was dead. Replaced and Flashed new .hex with STLink.
New issue:
USB not connecting. Traced the 3rd and 4th connection on the USB port to R104 and R103 and then to the MCU. Continuity across all, but the VESC isn't connecting in Vesc Tool. Blue light is all I've got right now.

Could the crystal (X2) be bad?
Can the VESC be used with VESC Tool through an STLink?

99% sure the DRV is soldered properly, I have 3.3 volts on pin 32 of the MCU with comes from the DRV, so if the ground pad did not solder I do not think I would have the 3.3 volts.

![capture2|685x500](upload://3apTwMelnlZsQfGmC7UGnqXvRNd.PNG)

Does the USB connector supply 5v to the board?

![48%20PM|640x426](upload://sobw5YnZeVN2ZVCxVz7NCc5Gdpt.jpg)!

![49%20PM|640x426](upload://bjMo0RRlByfR6T0vD1M7En6UK1t.jpg)
I checked continuity on all pins, and while some kay not look pretty, like pin 49, but all have continuity to the board and none to each other.
```

---
## \#13 Posted by: erod998 Posted at: 2018-08-15T00:42:46.918Z Reads: 14

```
This things for sale 😂 give me an offer someone and its yours I bought a new one.
```

---
