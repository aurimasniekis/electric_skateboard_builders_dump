# Fried multiple Vescs :( could someone double check my settings?

### Replies: 50 Views: 531

## \#1 Posted by: slade Posted at: 2018-12-29T04:48:51.993Z Reads: 166

```
As the title says, I've burned through multiple vescs so far; two from my own personal stupidity of accidentally causing a reverse polarity, and a third and most recent one for reasons currently unknown.

I've gotten a total of about 10 mins of use out of my first build before the board shut itself off and came to a stop. when I took it home and undid the enclosure, the master vesc was unresponsive, while the slave vesc was fine. When plugged in, the master vesc has no lights that come on, no audible whine from failing parts, and it is not recognized by the bldc-tool. There is some heat being generated from what feels like either the large 220 uH inductor, or the DRV chip next to it. It feels like the inductor is hotter, but I know more people have issues with the DRV chip than anything so I don't want to rule that out :/ Not able to load faults, the vesc is completely unresponsive. 

Here is a compiled screenshot of my motor settings:
![settings|245x499](upload://juusmOuXKuVn7nT7TAoY0lQffbM.png) 

Does anything stand out as a red flag? I've destroyed ~$300 bucks worth of these and I really don't want to do this again.
```

---
## \#2 Posted by: pat.speed Posted at: 2018-12-29T05:24:52.585Z Reads: 152

```
Looks pretty normal to me. What battery/ motor you got. And what brand of vesc.

Pics of the vesc pcb might help to diagnose what went wrong as well
```

---
## \#3 Posted by: slade Posted at: 2018-12-29T05:58:48.075Z Reads: 143

```
They are Maytech vescs bought from them on Aliexpress. The battery is a 12s4p battery I made with Samsung 30Qs, and the motors are dual Turnigy SK3 6374s.

Front:
![vescfront|283x500](upload://zAXeVl4tBVXBonpw8cOy7LmjIsW.png) 
Back:
![vescback|280x499](upload://9p3v2SuhSjs9e52C644PmrZhUzt.png)
```

---
## \#4 Posted by: slade Posted at: 2018-12-29T06:01:57.120Z Reads: 133

```
I can't find anything that talks about the difference between BR ERPM and just ERPM. I have my ERPM set to 60k, and the BR ERPM set to 80k (default value).
```

---
## \#5 Posted by: Andy87 Posted at: 2018-12-29T06:13:57.861Z Reads: 136

```
I would start with 30A as bat max.
I never had one of this hw4.12 VESCs, but I read that the max is about 35A if not in an extra heat sink case installed.
```

---
## \#6 Posted by: goldrabe Posted at: 2018-12-29T07:42:29.846Z Reads: 137

```
Did Maytech supplied you the can connector cable?
Can you show a picture of it?
```

---
## \#7 Posted by: Gamer43 Posted at: 2018-12-29T08:06:16.888Z Reads: 131

```
EDIT: There is nothing wrong with your settings; the motor controller you received is a lemon. The big electrolytic caps in the plastic shroud are not even connected to the PCB. You should ask for your money back on all three controllers.

Reliable alternatives, the $99 FOCBOX is the best option, Flipsky also offers decent ESCs, but you'll have to pay for shipping. I can't recommend TB ESCs because I literally watched my friend's TB ESC die at 12S on FOC; it needed a DRV8302 replacement.
Also, if you get the FSESC 4.20, be warned that it will throw DRV faults if you try to put too much current  through it (above 50A) or try to change the current too quickly, such as by quickly reversing the throttle.

In order to repair the motor controller, two things need to be replaced, the DRV8302 and the 5V TVS diode. A soldering iron and a heat gun can accomplish this. Additionally, the plastic shroud needs to be opened up and the board of electrolytic caps needs to be soldered (with wires) to the power rails of the motor controller; make sure they have the correct polarity.

Arrow.com offers free overnight shipping and they have DRV8302s in stock. Any 5V TVS diode will work.
```

---
## \#8 Posted by: pat.speed Posted at: 2018-12-29T08:12:34.788Z Reads: 120

```
I think the problem is the vesc in general. The main issue with these particular vescs is the fry the drv easy. Hence the name “drv cookers” if possible I would get some more reliable vescs especially with 12s. 

Personally I have run Tb 4.12 vescs at 12s just fine although I also added extra capacitors to be safer from voltage spikes.

Focboxs are a great option atm as they are $99 or turnigy vescs from Hobbyking are too as they come with a 12month warranty. Flipsky are another good alternative just stay away from the 4.20 version
```

---
## \#10 Posted by: pat.speed Posted at: 2018-12-29T08:51:48.272Z Reads: 119

```
What you mean the caps aren’t connected? They are attached to the wires
```

---
## \#11 Posted by: Gamer43 Posted at: 2018-12-29T08:58:11.947Z Reads: 118

```
Yes, but they aren't electrically connected, the electrolytic capacitors are basically floating in the plastic. The metal leads of the capacitors are soldered to a small board, but that board is not connected to anything else. Those capacitors may as well not exist for all the motor controller cares, which is very bad for the motor controller.
```

---
## \#12 Posted by: trampa Posted at: 2018-12-29T09:14:43.720Z Reads: 112

```
The titel should be changed to: Fried multiple VESC clones. 

All those ESC are not VESCs! VESC refers to the original, solid hardware. 
Failing, non genuine hardware, branded VESC, has a negative impact on the projects reputation. 
The hardware you show is obviously non genuine, 3rd party Hardware. 

If you open a thread called "failing VESC", uninformed users get the impression that VESCs fail easily. It's the VESC clones that fail, not VESCs. VESC is a registered Trademark!

Please change the titel to assure that people know exactly which Hardware failed. If it was a M-tech ESC, call it by its name. Always try to be as precise as possible.
```

---
## \#13 Posted by: Gamer43 Posted at: 2018-12-29T09:21:35.260Z Reads: 104

```
[quote="trampa, post:12, topic:79289, full:true"]
The titel should be changed to: Fried multiple VESC clones.

All those ESC are not VESCs! VESC refers to the original, solid hardware.
Failing, non genuine hardware, branded VESC, has a negative impact on the projects reputation.
The hardware you show is obviously non genuine, 3rd party Hardware.

If you open a thread called “failing VESC”, uninformed users get the impression that VESCs fail easily. It’s the VESC clones that fail, not VESCs. VESC is a registered Trademark!

Please change the titel to assure that people know exactly which Hardware failed. If it was a M-tech ESC, call it by its name. Always try to be as precise as possible.
[/quote]

This post is not pertinent to the thread or the OP's problem. 

If you feel the OP incorrectly titled this thread, you should resolve the matter through private messaging.
```

---
## \#14 Posted by: pat.speed Posted at: 2018-12-29T09:29:25.117Z Reads: 102

```
The caps are connected to the leads. Have you disassembled a vesc before? The caps are soldered to the pcb board which is then connected to the power wires. The pcb has some prongs that protrude a little wider with solder pads to attach to the wires.

[quote="trampa, post:12, topic:79289"]
All those ESC are not VESCs! VESC refers to the original, solid hardware.
Failing, non genuine hardware, branded VESC, has a negative impact on the projects reputation.
The hardware you show is obviously non genuine, 3rd party Hardware.
[/quote]

@trampa WTF! How can something open source be original. Does that mean that every single vesc 4.12 is not genuine? Because it’s not made by Ben himself? In that case your own vesc 6 is also a “clone”. This is just dumb, if the files were not released for others to use then they would be clones (ie. the focbox, those files aren’t released as far as I know) however the 4.12 and 6 file have been released so I would not call it copying.
```

---
## \#15 Posted by: Gamer43 Posted at: 2018-12-29T09:31:47.831Z Reads: 95

```
[quote="pat.speed, post:14, topic:79289"]
The caps are connected to the leads. Have you disassembled a vesc before? The caps are soldered to the pcb board which is then connected to the power wires. The pcb has some prongs that protrude a little wider with solder pads to attach to the wires.
[/quote]
In a properly assembled VESC, yes this is the case.

However, in the ESC that the OP has, this is NOT the case; he does NOT have a properly assembled VESC, and that is why all three of them failed quickly. They are lemon controllers, he did not receive a correctly assembled product and should demand a full refund from the seller of the ESCs he purchased.
```

---
## \#16 Posted by: pat.speed Posted at: 2018-12-29T09:33:53.347Z Reads: 90

```
How can you tell just from those pics? You can’t even see the connection point from these pictures. You would need to remove the heatshrink and angle the vesc differently to have a chance of seeing the connection point
```

---
## \#17 Posted by: Gamer43 Posted at: 2018-12-29T09:38:38.849Z Reads: 89

```
Well, since the capacitor board and main PCB are not physically connected, as can be seen in the pictures, in order for the two to be electrically connected, there must be a pair of wires running between the two.
In the picture. There are two sets of wires, a pair of black and red wires that are power positive and power negative, and a set of three wires that I can safely assume to be for the receiver. 

The black and red power wires run along the length of the capacitors, and across the capacitor board. The two wires appear to be completely insulated along their entire length in the picture, aside from the solder joints on the main PCB. Thus I can safely assume those wires are not electrically connected to the capacitors or capacitor board.

Since there are no more wires present in both pictures, I can assume that the capacitor board and main PCB are not electrically connected.
```

---
## \#18 Posted by: pat.speed Posted at: 2018-12-29T09:42:45.724Z Reads: 89

```
The wire insulation is only partially removed, it is removed from one side of the wire but not the other. Just think about it why put caps there and not solder them to the wire, like what’s the point
```

---
## \#19 Posted by: Friskies Posted at: 2018-12-29T09:43:36.175Z Reads: 89

```
Those maytechs run well in bldc @ 10s and 30A max. Anything else and you will fry them. 

If you want to run your board and the specs you want. I would get some ollins or focbox and enjoy the quality hardware.
```

---
## \#20 Posted by: Gamer43 Posted at: 2018-12-29T09:43:40.517Z Reads: 89

```
[quote="pat.speed, post:18, topic:79289, full:true"]
The wire insulation is only partially removed, it is removed from one side of the wire but not the other. Just think about it why put caps there and not solder them to the wire, like what’s the point
[/quote]

Ask Maytech, they clearly do not know what they are doing.
I saw some reviews on Banggood explaining the same situation where the capacitors were not electrically connected.
Basically, the makers of whatever ESC the OP purchased blindly copied the design files of the VESC 4.12. The additional connection between the capacitors and main PCB are not present in the PCB design files.
```

---
## \#21 Posted by: Friskies Posted at: 2018-12-29T09:46:10.933Z Reads: 81

```
They are stripped on one side and then soldered to the wire. Nothing wrong with the caps.
```

---
## \#22 Posted by: Gamer43 Posted at: 2018-12-29T09:47:14.136Z Reads: 83

```
That may be the case, if so, I think the OP should open up the heatshrink to verify.
```

---
## \#23 Posted by: pat.speed Posted at: 2018-12-29T09:47:32.852Z Reads: 82

```
They know exactly what they are doing, they make a lot of money. I know what they are doing too, they make the cheapest vescs and don’t care about Qc. However they do know how to solder some caps to a wire, as do I considering I did it a few weeks back and can tell you rn that those caps are more than likely connected and that the whole wire insulation does not need to be removed nor is it
```

---
## \#24 Posted by: J0ker3366 Posted at: 2018-12-29T09:49:44.634Z Reads: 82

```
![Screenshot_2018-12-29-02-44-29|281x500](upload://hsRhHOAIlRHrqCNwm0e6jsUrMm.png)
```

---
## \#25 Posted by: pat.speed Posted at: 2018-12-29T09:50:13.124Z Reads: 82

```
[quote="Gamer43, post:20, topic:79289"]
The additional connection between the capacitors and main PCB are not present in the PCB design files
[/quote]

What? Do you think maytech are really that dumb, they make some of the best motors and other electronics we have. They also have their own designs for escs, I’m pretty sure whoever their engineer is would realise they are connected
```

---
## \#26 Posted by: pat.speed Posted at: 2018-12-29T09:51:19.520Z Reads: 79

```
Idk what that was meant to show but it does show the protruding pcb legs I was talking about that the wires are soldered to
```

---
## \#27 Posted by: Friskies Posted at: 2018-12-29T09:53:24.974Z Reads: 79

```
I have a few at home. They are just like the cheap flipskys. They work well within their limits but they do not like being pushed outside of them at all.
```

---
## \#28 Posted by: sayekim Posted at: 2018-12-29T09:53:50.651Z Reads: 77

```
I am no expert but they seem to be just floating capacitors without a connection to the pcb or wires. 😂🤪😱

Since these esc are faulty anyway please open up the heat shrink and pull the wires from the capacitors to judge.
```

---
## \#29 Posted by: sayekim Posted at: 2018-12-29T09:55:50.027Z Reads: 75

```
Well spotted. Luckily they seem to be connected after all.
```

---
## \#30 Posted by: Gamer43 Posted at: 2018-12-29T09:56:11.640Z Reads: 80

```
My apologies. From what I could tell, it looked to me that the capacitors were not connected. You know more than I do about the construction of this brand of VESC.
TB ESCs do it differently, that is why I made such a mistake in judgment.

But I still think the connection should be verified, the solder joint could still be faulty (it happens, especially with the lead-free rubbish that everyone is forced to use these days, cold joints are not uncommon, even under proper reflow conditions). The vibration from riding would only exacerbate such a fault if it were to occur.

If the connection is good, then my best guess would be OP was running a BMS and had a tad too much regen and an overvoltage condition occurred.
What would've happened there was overvoltage caused the buck converter to fail, which in turn overloaded the 5V TVS diode. 
He should change the overvoltage cutoff setting to 52V if this is indeed the case. I've had BMSes cut off my ESCs during regen, but since this happened in unloaded conditions, the ESCs survived. Since the OP had some momentum and I'm guessing attempted to regen, the VESC didn't cut off from overvoltage soon enough.

@slade try setting the maximum input voltage to 52V, batt regen current to -20A, and undercharge your battery pack a little bit, something like 0.1 or 0.2V per cell.
```

---
## \#31 Posted by: jadatmag Posted at: 2018-12-29T12:02:09.182Z Reads: 71

```
Battery current max regen at -30 is pretty high. What kind of battery you running?
```

---
## \#32 Posted by: slade Posted at: 2018-12-29T22:54:07.970Z Reads: 66

```
Just to confirm, 30A for each one? It's a dual setup.
```

---
## \#33 Posted by: slade Posted at: 2018-12-29T22:56:08.838Z Reads: 68

```
The DC input wires out of shot are 10 or 12 gauge wire, with exposed and tinned leads. I added 5mm male bullet connectors to them.
```

---
## \#34 Posted by: slade Posted at: 2018-12-29T23:03:24.716Z Reads: 69

```
I am using the can connector cable that was given to me by the user on the forums that I bought the first two from.
![20181229_145807|281x500](upload://9usfkCxI3nd3jpY2oYb161vJSaF.jpeg) 

I did continuity checks on the wires, and haven't seen an issue with them.
```

---
## \#35 Posted by: slade Posted at: 2018-12-29T23:11:02.386Z Reads: 67

```
It's incredibly hard to tell, but there is a slice of insulation missing from the DC input wires, and the exposed part of the wire is soldered to the electrolytic cap's PCB.

IF all that I have to do is replace the DRV chips I can definitely do that myself, but I'm not even fully sure if that is the real issue :/

[Any of these](https://www.arrow.com/en/products/search?cat=&q=drv8302&r=true) would be fine replacement DRVs?
```

---
## \#36 Posted by: goldrabe Posted at: 2018-12-29T23:11:28.920Z Reads: 62

```
Okay, the can connector is fine. Maytech supllied me the can connector with all 4 wires in it which killed my Canbus chip.
```

---
## \#37 Posted by: slade Posted at: 2018-12-29T23:13:31.149Z Reads: 62

```
It's a custom battery pack I made with Samsung 30Qs in a 12s4p configuration.
```

---
## \#38 Posted by: pat.speed Posted at: 2018-12-29T23:15:58.091Z Reads: 60

```
Jeezus lower that battery current right away. You could be pumping upto 60a into that battery at some points. This is not safe for the battery nor the esc. I missed this setting, this could be what is cooking your vesc. It should be set to 8a each esc or 16a if it’s only 1. The max charge rate on the 30q is 4a and you’ve got it in a 4p so 16a.
```

---
## \#39 Posted by: Gamer43 Posted at: 2018-12-29T23:33:18.256Z Reads: 63

```
Could you do a light strain/stress test to ensure the solder joint is good? I've had bad solder joints on my ESCs before, but the worst thing it did for them was make the motor cog a bit.

In order to verify that the DRV8302 does indeed need to be replaced, check if batt positive and batt negative are short-circuited to each other (use both continuity and ohms mode, ohms mode won't beep, but anything less than a few kilo ohms is a short. On both tests HOLD IT FOR A FEW SECONDS since the caps need to charge up to get an accurate reading).
If there is a short, DRV8302 needs to be replaced.
If there is not a short, replace the 5V TVS diode with a new one, make sure the polarity is the same as the original.
If the DRV8302 is still good, lights will come on, and hopefully the ESC will work.
If not, the new 5V TVS diode will die (and need to replaced again) and nothing will light up.
If the latter happens, both the DRV8302 and the new 5V TVS diode you soldered on will need to be replaced. 

The 5V TVS diode can be found here 
![TVS%20Diode|666x500](upload://n4jaxF7cbFh5Qhq1K4rfzYA3YDX.jpeg) 
(btw, those MOSFETS are the IPB014N06NATMA1 and not the IRFS7530 rubbish :D).

MAKE SURE a functioning 5V TVS diode is ALWAYS present when electrically testing with power.

Once the DRV8302 and 5V TVS Diode are removed, check for shorts between batt positive and batt negative and shorts to ground on the 5V and 3.3V rails. If no shorts are present, those *should* be the only two components you need to replace and I think you can then solder on the new components.

Remember that the DRV8302 has an exposed ground pad underneath it; you will need hot air to remove it and to solder on a new one. I didn't realize this when I was repairing my friend's VESC and knocked a couple of caps off.

And yes, Arrow.com sells genuine electronic components, they are the second largest electronics distributor for OEMs. Digikey is just the most well known among hobbyists since they started as a hobby distributor and now have the widest selection of online catalog parts in stock (and ready to ship same day) than any other distributor.
```

---
## \#40 Posted by: slade Posted at: 2018-12-30T00:17:38.495Z Reads: 61

```
Would you happen to know the name of the TVS diode? I'm about to buy the DRV chips on Arrow and it would be nice to get the diode as well.
```

---
## \#41 Posted by: Andy87 Posted at: 2018-12-30T00:20:52.473Z Reads: 61

```
Yes for each only 30a battery max
```

---
## \#42 Posted by: Gamer43 Posted at: 2018-12-30T00:20:52.895Z Reads: 61

```
any 5V TVS diode will work, 
The ones I got were https://www.arrow.com/en/products/smaj5.0a-e361/vishay

I would highly recommend ordering an extra DRV8302 and like five 5V TVS diodes.
Something as trivial as a (SINGLE) bent pin can really ruin your day, had to throw out a DRV8302 because of that DXXX.

I would also recommend removing the DRV8302 and 5V TVS diode and performing electrical checks to make sure there aren't any other components that need to be replaced.
```

---
## \#44 Posted by: slade Posted at: 2018-12-30T01:07:48.246Z Reads: 58

```
So using the remaining vesc reprogrammed to be master with the recommendations from you guys above, I did a no-load throttle test, and got several blinks of the red light that triggered a motor cutoff when punching the acceleration (didn't happen when slowly increasing acceleration). It didn't fry the vesc, so I was able to read faults off the DRV and it gave these: 
    The following faults were registered since start:

Fault            : FAULT_CODE_ABS_OVER_CURRENT
Current          : 19.6
Current filtered : 33.3
Voltage          : 48.20
Duty             : 0.671
RPM              : 39680.3
Tacho            : 20488
Cycles running   : 3768
TIM duty         : 4051
TIM val samp     : 2025
TIM current samp : 5044
TIM top          : 6037
Comm step        : 2
Temperature      : 29.02
 
Fault            : FAULT_CODE_ABS_OVER_CURRENT
Current          : 22.6
Current filtered : 30.3
Voltage          : 48.50
Duty             : 0.579
RPM              : 34449.4
Tacho            : 26527
Cycles running   : 3203
TIM duty         : 3983
TIM val samp     : 1991
TIM current samp : 5428
TIM top          : 6874
Comm step        : 5
Temperature      : 29.02
 
Fault            : FAULT_CODE_ABS_OVER_CURRENT
Current          : 27.0
Current filtered : 31.8
Voltage          : 48.52
Duty             : 0.463
RPM              : 25979.0
Tacho            : 28358
Cycles running   : 1924
TIM duty         : 3863
TIM val samp     : 1931
TIM current samp : 6102
TIM top          : 8342
Comm step        : 6
Temperature      : 29.18
 
Fault            : FAULT_CODE_ABS_OVER_CURRENT
Current          : 25.0
Current filtered : 32.2
Voltage          : 48.47
Duty             : 0.458
RPM              : 25895.3
Tacho            : 29660
Cycles running   : 1913
TIM duty         : 3857
TIM val samp     : 1928
TIM current samp : 6141
TIM top          : 8425
Comm step        : 6
Temperature      : 29.07
```

---
## \#45 Posted by: Andy87 Posted at: 2018-12-30T01:26:59.872Z Reads: 53

```
Looks like something lose.
Check all connections and have a look if there bad solder joins on the pcb etc.
People had this issues when the caps where lose etc.
I had this fault for a while and than the drv popped...
```

---
## \#46 Posted by: slade Posted at: 2018-12-30T01:35:38.850Z Reads: 52

```
This happened only once per hard acceleration, if that makes any difference
```

---
## \#47 Posted by: Andy87 Posted at: 2018-12-30T02:37:28.814Z Reads: 49

```
That makes sense as it is an over current fault.
So it appears only when the vesc sees too high values for the current, what could be while accelerating (but shouldn’t happen on the bench how it is in your case...)
```

---
## \#48 Posted by: slade Posted at: 2018-12-30T02:52:03.051Z Reads: 46

```
Why does the vesc shutdown at 30A, instead of making that the artifical ceiling of current draw? If I want to floor it/do the hardest acceleration possible while staying under or at 30A, I'm confused why it shuts off vs holding a 30A ceiling.
```

---
## \#49 Posted by: deucesdown Posted at: 2018-12-30T03:14:49.668Z Reads: 49

```
It looks like yew set ABS CURRENT MAX to 30a. You should leave this value at the default whick I believe is 130a.

The advice was to set battery max current to 30a.
```

---
## \#50 Posted by: Turboboard Posted at: 2018-12-30T19:37:36.259Z Reads: 37

```
Can anyone help me with my vesc settings? I have dual 6374 190KV 3300w motors with a 10s battery. The vesc is rated for 150A continuous and 300A surge. I'm getting almost no torque at all with the default settings, (I can stop them in mid spin with my hand)
```

---
## \#51 Posted by: Andy87 Posted at: 2018-12-30T19:43:42.073Z Reads: 34

```
Maybe you want to split this up and create a new topic. Post your setup, which battery exactly, which vescs, which motors, which gearing and wheel size.
```

---
## \#52 Posted by: Turboboard Posted at: 2018-12-30T19:53:23.718Z Reads: 32

```
Thanks, will do
```

---
