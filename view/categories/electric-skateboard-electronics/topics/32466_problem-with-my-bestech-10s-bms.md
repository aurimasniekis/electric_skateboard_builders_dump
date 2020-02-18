# Problem with my bestech 10s BMS

### Replies: 23 Views: 1599

## \#1 Posted by: Silverline Posted at: 2017-09-06T20:12:34.955Z Reads: 181

```
Hallo
I have a problem with my bestech 10s BMS.
I can't get it to power up my vesc's. When i turn on the switch nothing happens. Funny thing is, no matter if the switch are on or off, when i connect my Charger to the port , it turns on my vesc. If i then disconnect the Charger , while the E-switch is On, the VESC keeps being turned on. I can now turn off the switch, and the light goes out in the VESC. But i can't turn them on again by pushing the switch again. 

I have connected the BMS according to this diagram , and using the BMS as discharge. 
<img src="/uploads/db1493/original/3X/e/b/ebc40e7f4ee3e825907c2e72ce60703702a49ddd.png" width="392" height="500">
```

---
## \#2 Posted by: psychotiller Posted at: 2017-09-06T20:18:27.836Z Reads: 167

```
We had the same thing happen to a 10s bms the other day. Except ours would turn on then not turn off. We would disconnect the switch, plug it back in and then the switch would turn it on, but not off again. We tried 3 different swtches. Thing is, when we touched the white switch wires together, then separated them, it would turn the system on and off like normal.
```

---
## \#3 Posted by: scepterr Posted at: 2017-09-06T20:24:18.319Z Reads: 162

```
@psychotiller try replacing the white wires?
There's been quite a few switch issues with the bestech BMSs lately
@Silverline try jumping the solder points on the BMS for the switch, see if it works
```

---
## \#4 Posted by: Silverline Posted at: 2017-09-06T20:35:08.298Z Reads: 155

```
Okay i Wil try that thanks...
```

---
## \#5 Posted by: psychotiller Posted at: 2017-09-06T21:10:17.166Z Reads: 145

```
I'll give that a shot as well. Thanks
```

---
## \#6 Posted by: Silverline Posted at: 2017-09-06T21:13:32.218Z Reads: 144

```
But i have a feeling that this is not my problem, since when i can turn it on by using my charger, and then the button works when i power it off.
```

---
## \#7 Posted by: Namasaki Posted at: 2017-09-06T21:39:12.685Z Reads: 140

```
[quote="Silverline, post:6, topic:32466, full:true"]
But i have a feeling that this is not my problem, since when i can turn it on by using my charger, and then the button works when i power it off.
[/quote]


anytime you connect and turn your charger on, power will go to the vesc when the bms is on or off. This is normal.

someone recently had the same problem where their bms would not turn on and it turned out to be a break in one of the white wires.

First remove the switch and try touching the wires together to turn it on.
If that doesn't work then try jumping the solder points where the wires are soldered to the circuit board.
```

---
## \#8 Posted by: Silverline Posted at: 2017-09-07T04:45:55.711Z Reads: 122

```
But even if the switch is Off, the vescs lights Up when i connect the Charger. But i have look at the switch again.
```

---
## \#9 Posted by: Namasaki Posted at: 2017-09-07T05:18:41.705Z Reads: 123

```
It is normal for the vescs to light up when you plug in and turn on the charger even if the switch is off.
You want the switch to be on while charging though per the manufacture's instructions.

You have me thinking now that there may be some issue other that the switch wires.
What type of battery are you using and have you checked the output voltage of the battery.
Have you checked individual cell or cell group voltages.
One cell or cell group with voltage of 3v or less will cause the bms to not turn on.
If one or more of the bms balance wires is not connected or has a poor connection it will cause the bms to not turn on.
```

---
## \#10 Posted by: Silverline Posted at: 2017-09-07T05:47:31.655Z Reads: 106

```
I Can measure All the cells via the ballancing wires from the battery. And they are all spot on 3,68X volt.  But i have no change measure if the BMS is actually getting that voltage. Lets assume that the ballancing plug that comes with the BMS is defective, that could do that the BMS wont turn on ? Thanks... You give me something to Work with there.

It makes sense
```

---
## \#11 Posted by: MontPierre Posted at: 2017-09-07T07:00:00.810Z Reads: 98

```
Yes, bms won't turn on when balancing cable is not connected. I guess it is the same when it is defective.
```

---
## \#12 Posted by: Silverline Posted at: 2017-09-07T15:07:00.055Z Reads: 94

```
@Namasaki When is measure the cells on the backside off the BMS, it all look fine. But i noticed that the two solder tabs saying "Fuse" is where the two E-switch wires is soldered on, and the two "SW" tabs, is where the little white thing setting on the side on the heatsinks is soldered to. Shouldn't it be the opposite way ?
```

---
## \#13 Posted by: Namasaki Posted at: 2017-09-07T15:31:48.733Z Reads: 92

```
Can you post a close up pic of it
```

---
## \#14 Posted by: Silverline Posted at: 2017-09-07T15:34:51.195Z Reads: 91

```
<img src="/uploads/db1493/original/3X/0/5/05e323cfd5bf8fa0abe159bb02e70d0f6d8562a8.jpg" width="690" height="388">
```

---
## \#15 Posted by: Namasaki Posted at: 2017-09-07T15:35:46.337Z Reads: 89

```
Need better pics too and bottom. 
Can't tell anything from that pic
```

---
## \#16 Posted by: Silverline Posted at: 2017-09-07T15:36:13.392Z Reads: 93

```
@Namasaki Not so easy. But the two saying "Fuse" is where the E-switch wires is soldered on. And the other two saying SW is where the "thermostat" i assume it is, is soldered on
```

---
## \#17 Posted by: Namasaki Posted at: 2017-09-07T15:37:12.363Z Reads: 94

```
Try shorting the solder points from the thermostat and see if it turns on

Leave the 2 wires for the switch disconnected
```

---
## \#18 Posted by: Silverline Posted at: 2017-09-07T15:41:26.510Z Reads: 93

```
The thermostat is a NC contact, so it`s always "shorted" so long the heatsinks is not to hot. But my logic says, that SW must be for the ESwitch and Fuse must be the thermostat, and not the other way around. So now when the E-switch is playing the "fuse" when its turn off, it`s like if the BMS is overheating, and you can`t turn i on. The only way to reset the BMS is to turn off and on the E-switch, but since the thermostat is soldered to the SW, it`s newer ever going to get a Off signal. Does that make sense ?
```

---
## \#19 Posted by: Namasaki Posted at: 2017-09-07T17:42:10.465Z Reads: 89

```
That does make sense so try desoldering the wires and switch them. 
It's seems unlikely that they would come from the factory with the wires soldered incorrectly and they are supposedly inspected and tested before shipped. 
Did you buy directly from Bestech?
```

---
## \#20 Posted by: Silverline Posted at: 2017-09-07T17:45:20.630Z Reads: 89

```
Im on it 😃
```

---
## \#21 Posted by: Silverline Posted at: 2017-09-07T18:39:01.505Z Reads: 84

```
Same damn thing....:-(

Only way to turn the vesc's on is if i connect my charger, and disconnect it again, then the VESC stays on, until i turn off the e switch

Or if i turn on the e switch, pull the loop key (in line between P- and the vescs) and put the loopkey back in, that makes the well knowen spark , and that turns on my vescs , and they stay on, until i turn off the E-switch
```

---
## \#22 Posted by: Silverline Posted at: 2017-09-07T19:10:28.879Z Reads: 84

```
I have a bat. meter display. If i  disconnect My two focboxes, so the bat. meter is the only thing connected to the P- and plus, i can turn on and off without any Problems via the E-switch. The moment i connect my two focboxes, i can't turn on and off anymore
```

---
## \#23 Posted by: pjotr47 Posted at: 2018-01-04T16:50:48.106Z Reads: 62

```
Is the problem solved? I have the same issue
```

---
