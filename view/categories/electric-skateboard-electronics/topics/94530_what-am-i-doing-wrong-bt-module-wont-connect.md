# What am I doing Wrong?(BT Module won&rsquo;t connect)

### Replies: 40 Views: 502

## \#1 Posted by: J_Dizzle Posted at: 2019-05-21T14:13:17.651Z Reads: 102

```
My build is 100% done, I just can't get my bluetooth module to connect. I'm using the HM-10 module with the Xmatic ios app by @twan however I cannot get my phone to find it. I'm using an iphone SE and have the latest update to his app. Yesterday I noticed the wires connecting it to the UART port on Vesc were all out of order, so I rewired it to how it should be wired according to the settings displayed on the app. The wiring is now

Bluetooth Module-UART            

RXD-TX

TX-RX

GND-ADC

VCC-5V

I still can't even get an LED to flash on the module, is it me or is it a faulty pcb?

Edit: I'll tag @b264 because I'm confident he can help me solve this
```

---
## \#2 Posted by: AlanZhou Posted at: 2019-05-21T14:28:58.391Z Reads: 87

```
[quote="J_Dizzle, post:1, topic:94530"]
I’m using the HM-10 module
[/quote]

Gotta change your buadrate

If there is no light the module might be dead or you wired it incorrectly
```

---
## \#3 Posted by: J_Dizzle Posted at: 2019-05-21T14:29:52.716Z Reads: 84

```
 I already had it changed to 9600 and had the app set to PPM and UART

When I recieved the module I noticed it was wired incorrectly so I rewired it to how it was shown in the app
```

---
## \#4 Posted by: Jumpman Posted at: 2019-05-21T15:14:28.666Z Reads: 76

```
GND-ADC?  Maybe try GND-GND?
```

---
## \#5 Posted by: J_Dizzle Posted at: 2019-05-21T15:37:47.672Z Reads: 71

```
There is no pin labeled GND on any jst connector on the Vesc, so I assumed ADC was ground
```

---
## \#6 Posted by: Wilsonliang777 Posted at: 2019-05-21T15:48:01.656Z Reads: 69

```
I am having the same problem.  I am running fsesc 4.12.   bt mod would not connect or transmit any data but everything was working b4 I upgraded to the new vesc firmware.    But if I use the bt mod by flipsky things work
```

---
## \#7 Posted by: J_Dizzle Posted at: 2019-05-21T15:55:14.535Z Reads: 66

```
Do you use the flipsky bt module with the Xmatic app?
```

---
## \#8 Posted by: Wilsonliang777 Posted at: 2019-05-21T16:00:58.394Z Reads: 65

```
No. I have an Android phone
```

---
## \#9 Posted by: Jumpman Posted at: 2019-05-21T16:02:40.081Z Reads: 64

```
Is there a pin between 3.3V and ADC?  Maybe try that one.
```

---
## \#10 Posted by: J_Dizzle Posted at: 2019-05-21T16:17:08.206Z Reads: 61

```
Yeah I’m thinking of trying that one. It is labeled —  and idk if that means ground or the pin isn’t used
```

---
## \#11 Posted by: skelstar Posted at: 2019-05-21T18:51:34.335Z Reads: 56

```
It's definitely not ADC.

![image|690x403](upload://vg4XnhfiBNqc7uLh6Bfq4iH8O9l.png) 

(I Googled VESC 4.12 pinout)
```

---
## \#12 Posted by: J_Dizzle Posted at: 2019-05-21T19:19:47.783Z Reads: 51

```
I was going off of the pinout shown by flipsky, however GND wasn’t labeled like it is here
```

---
## \#13 Posted by: Santino Posted at: 2019-05-21T22:15:10.110Z Reads: 50

```
You could check with a cheap voltmeter and a 1,5 volt battery, just remove the pins from the jet and close the circuit through the batt, you should be able to find ground... hope it helps
```

---
## \#14 Posted by: J_Dizzle Posted at: 2019-05-21T23:21:24.908Z Reads: 50

```
Ok so I’ve made progress. My phone is able to connect to the Bluetooth module after some rewiring, however it just keeps saying connecting to Vesc. I am positive that I have set the Vesc to ppm and uart and baud rate to 9600. Are there any other settings  that need to be changed?
```

---
## \#15 Posted by: 1337 Posted at: 2019-05-21T23:22:16.894Z Reads: 50

```
Are you using lightblue app or similar to find the hm10? I have to do that for mine to see it in the settings on my phone.
```

---
## \#16 Posted by: J_Dizzle Posted at: 2019-05-21T23:22:45.120Z Reads: 46

```
I can see it in my regular phone settings now
```

---
## \#17 Posted by: 1337 Posted at: 2019-05-21T23:32:39.496Z Reads: 47

```
Ah I missed your last post
```

---
## \#18 Posted by: J_Dizzle Posted at: 2019-05-21T23:33:35.948Z Reads: 47

```
Yeah it says connected in my phone settings however in the app while the Bluetooth is connected it can’t connect to my Vesc
```

---
## \#19 Posted by: 1337 Posted at: 2019-05-21T23:33:58.044Z Reads: 45

```
Were in the same boat now, my phone is connected by the app says trying to connect to vesc.
```

---
## \#20 Posted by: 1337 Posted at: 2019-05-21T23:36:04.165Z Reads: 45

```
Under the stats screen when you click the Bluetooth icon flashing below what does it say on the next screen?
```

---
## \#21 Posted by: J_Dizzle Posted at: 2019-05-21T23:36:11.291Z Reads: 43

```
I think I may have figured it out, I just don’t know how to solve it. 
Xmatic app supports Ack firmware 3.102, but if you use the Ack tool to download the newest firmware then it downloads 3.013, which I don’t think Xmatic app supports
```

---
## \#22 Posted by: 1337 Posted at: 2019-05-21T23:41:32.182Z Reads: 39

```
Oh I must have a different problem then, I haven’t used Ack firmware
```

---
## \#23 Posted by: 1337 Posted at: 2019-05-21T23:42:52.496Z Reads: 39

```
Or the ack tool I should say
```

---
## \#24 Posted by: 1337 Posted at: 2019-05-22T02:00:09.883Z Reads: 37

```
Fixed my problem, poor wire connection.
```

---
## \#25 Posted by: J_Dizzle Posted at: 2019-05-22T02:01:18.635Z Reads: 38

```
Where was the poor connection? In the connector of just a bad solder? Maybe I will try replacing all the wires since I have nothing to lose
```

---
## \#26 Posted by: 1337 Posted at: 2019-05-22T02:03:07.655Z Reads: 35

```
Mine was the plastic connector on the end of the cables, I cut it off and soldered the wire to the pins just for shits and giggles and it connected right away.
```

---
## \#27 Posted by: J_Dizzle Posted at: 2019-05-22T02:03:52.036Z Reads: 35

```
Was this the jst connector that plugs into the vesc or the black connector on the Hm-10 module?
```

---
## \#28 Posted by: 1337 Posted at: 2019-05-22T02:05:17.296Z Reads: 35

```
Vesc side, the pins on the hm10 were larger so they were snug. If your connector seems tight it’s prob not your solution though I could feel mine was not the best
```

---
## \#29 Posted by: J_Dizzle Posted at: 2019-05-22T02:05:56.382Z Reads: 32

```
Yeah on the vesc side I can feel the wires almost pull out of the connector
```

---
## \#30 Posted by: 1337 Posted at: 2019-05-22T02:06:03.586Z Reads: 34

```
Do you have a multimeter? Maybe try to check the continuity of the wires for a fault
```

---
## \#31 Posted by: 1337 Posted at: 2019-05-22T02:08:29.324Z Reads: 34

```
It’s worth a shot if you have exhausted all else, Need a small tip for the soldering iron to get to the vesc pins.
```

---
## \#32 Posted by: 1337 Posted at: 2019-05-22T13:05:10.085Z Reads: 30

```
I guess I have a firmware issue as well, I can not write modes, I sent a log and a question about it to thuan and he said the app does not support my firmware.
```

---
## \#33 Posted by: J_Dizzle Posted at: 2019-05-22T17:00:30.355Z Reads: 22

```
I’ve just about troubleshot every option, I’m pretty sure I have a bad module. So far I’ve replaced all wires and connectors, upgraded and downgraded my Vesc firmware, tried the module on multiple vescs but to no avail. It just keeps saying connecting to Vesc. I have been sending pms to @twan over the last two weeks but he has not been answering them. Any final suggestions before I buy a new hm-10?
```

---
## \#34 Posted by: 1337 Posted at: 2019-05-23T17:40:45.020Z Reads: 22

```
Hmm are you sure you have the rx to tx? Your hm10 is on and sending signal since you were above to connect to it. Just not sending and recovering data.
```

---
## \#35 Posted by: J_Dizzle Posted at: 2019-05-23T19:52:37.233Z Reads: 19

```
Positive. I have checked them 10+ times
```

---
## \#36 Posted by: RealaPolarBear Posted at: 2019-05-23T20:16:57.072Z Reads: 18

```
Where did you get the HM-10? Cause a while back I was having the same problem with my HM-10 from BKB and I tried all the troubleshooting and it didn’t work. Did the wires soldering it direct to the Vesc work?
```

---
## \#37 Posted by: J_Dizzle Posted at: 2019-05-23T20:49:53.157Z Reads: 19

```
Yeah I too got mine from bkb. I purchased mine in November of last year but it has sat untouched since then. Maybe ours are from the same batch? I didnt directly solder the wires to the vesc, instead I just ripped the wires out of the jst and they still had those small metal prongs on the end of them and I pushed them over the vesc pins in the uart port and they fit really snug.
```

---
## \#38 Posted by: RealaPolarBear Posted at: 2019-05-23T22:35:06.575Z Reads: 19

```
Yeah I got mine in November too, part of the Black Friday sale. Is that when you got yours? Haven’t had it working since I got it.
```

---
## \#39 Posted by: J_Dizzle Posted at: 2019-05-23T22:42:13.226Z Reads: 19

```
Yup, got it for Black Friday too lol
@JLabs do you have any in stock, I need to pick up a new one
```

---
## \#40 Posted by: JLabs Posted at: 2019-05-23T22:52:12.015Z Reads: 18

```
If your having issues, shoot me an email. Jared at buildkitboards dot com. 

The app is sometimes (but not all times) at fault. If you have an android tablet or phone try the ackmaniac app. That has been rock solid for me. The twan app is hit or miss sometimes. One update it works fine, the next update there is an issue.

Either way, I’ll sort out any issues.
```

---
