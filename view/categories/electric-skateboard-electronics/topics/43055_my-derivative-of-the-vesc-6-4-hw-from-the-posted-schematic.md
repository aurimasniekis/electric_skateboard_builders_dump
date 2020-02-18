# My derivative of the VESC 6.4 HW from the posted schematic

### Replies: 41 Views: 7368

## \#1 Posted by: chuttney1 Posted at: 2018-01-07T08:08:27.228Z Reads: 429

```
Dimensions are a 70mm x 70mm PCB. I tried for 65mm x 65mm, but I was tight on space. I tried going for a 2-layer design, but ran into issue routing all the traces between the DRV8301, ST32F4 chip, and everything else. So it's 4 layers. I got rid of the NRF24L01P and MPU9150 portions present in the schematic as those were not part of 4.12HW. PCB mounting holes are for M2.5 button head screws.

Bottom of PCB. Ignore the blue capactiors as I didn't figure out how kicad would reder it. I'm missing a few models also.
<img src="/uploads/db1493/original/3X/6/9/6904ac20481bbeb7bb9d23198a8770814d59d5cd.png" width="690" height="350">

Top of PCB
<img src="/uploads/db1493/original/3X/0/7/0782c04cde8172d9d0a5065eee6c5f29b6cc909c.png" width="690" height="350">
```

---
## \#2 Posted by: b264 Posted at: 2018-01-07T08:11:24.341Z Reads: 412

```
Wow, this is awesome!  Have you uploaded the files to github yet?
```

---
## \#3 Posted by: evoheyax Posted at: 2018-01-11T03:04:47.471Z Reads: 384

```
Yes, files would be awesome! Really need someone to modify it so it can be a more reliable 4.12, without extra bits that we don't need for eskate that drive up the price.
```

---
## \#4 Posted by: scepterr Posted at: 2018-01-11T03:07:36.869Z Reads: 383

```
I'm down for beta testing, whenever that is 😁

What's estimated BOM cost btw?
```

---
## \#5 Posted by: notepad Posted at: 2018-01-11T03:35:13.947Z Reads: 374

```
would be interesting to see how this fares against the esc-ape 6.4 thats being tested atm.  got a little armsrace in the making!
```

---
## \#6 Posted by: chuttney1 Posted at: 2018-01-11T04:41:19.462Z Reads: 367

```
I plan to max out the specification of components used such as using as much automotive grade components. It's is not required because the components listed in 4.12 BOM have been proven to work well. I am taking into consideration how to solder the DRV8301 since it was such a pita soldering the DRV8302 when I went the DIY route on VESC 4.7. 

I really want this to be super reliable such as mission-critical, the DRV cannot fail for it's intendend application. I still need to understand why the DRV8302 had such a high failure rate before Vedder increased PCB trace width, made fixes, resulted in the VESC6 version with fewer DRV errors. I'm thinking this relates to the voltage transients between the MOSFET and the DRV itself.
```

---
## \#7 Posted by: jmasta Posted at: 2018-01-11T04:48:53.258Z Reads: 354

```
[quote="chuttney1, post:1, topic:43055"]
I got rid of the NRF24L01P and MPU9150 portions present in the schematic as those were not part of 4.12HW
[/quote]

How does this compare to the VESC v4.12 and v6.4?  I see that you plan to max out the components. I just don't fully understand the point of modifying/downgrading the v6 schematic to be more like v4?

Genuinely curious. I'm an aerospace/mechanical guy, not an EE :face_with_raised_eyebrow:
```

---
## \#8 Posted by: evoheyax Posted at: 2018-01-11T05:56:21.274Z Reads: 342

```
I'm assuming at least part of it is lower the cost to build. Most people don't need all of the features of the vesc 6, like the accelerometer. So by taking the parts that were added that don't impact performance but were just added to give more features, you could lower the cost quite a bit. Just my thoughts at least...
```

---
## \#9 Posted by: chuttney1 Posted at: 2018-01-11T07:08:38.831Z Reads: 340

```
[quote="jmasta, post:7, topic:43055"]
How does this compare to the VESC v4.12 and v6.4?
[/quote]

Not much other than the NRF24L01P adds built-in control for VESC and MPU9150 is the accelerometer. I'm not if Trampa sells the VESC with both of these.I read on the VESC forum that the NRF chip is not included due to certifications with the FCC cause it operates in the 2.4 GHz spectrum for buyers outside the EU. Tramp sells two different version for EU and Non-EU regarding this chip. The other thing, Vedder used the current sense amplifier for the DRV8302 on HW 4.12 and not on the DRV8301. I'm assuming it because the chip only allows for 2 amplifiers and it's not good enough. I just learned TI has the DRV8323R utilizing the SPI interface found in the VESC6.4 and 3 current shunt amplifiers. The buck converter, however, does only 600 mA versus the DRV8301,1.5 amp supply. 

[quote="jmasta, post:7, topic:43055"]
I just don’t fully understand the point of modifying/downgrading the v6 schematic to be more like v4?
[/quote]
Cost wise, the BOM for HW4.12 is ~$75 versus HW6.X  at ~$100. It 50/50 for me; my call if I need to. Price-wise, cheaper wins for the consumer as the general consensus. I'm not cheaping out on my version.




I'm not an EE. I got a chemistry degree. This is all a hobby/education into what the world is moving towards.
```

---
## \#10 Posted by: ThierryGTLTS Posted at: 2018-01-11T08:07:42.964Z Reads: 331

```
[quote="chuttney1, post:6, topic:43055"]
I really want this to be super reliable such as mission-critical, the DRV cannot fail for it’s intendend application. I still need to understand why the DRV8302 had such a high failure rate before Vedder increased PCB trace width, made fixes, resulted in the VESC6 version with fewer DRV errors. I’m thinking this relates to the voltage transients between the MOSFET and the DRV itself.
[/quote]

You are right, most of the problems come from there.
That's why people who use 10S have far less problems.
It's very important to reduce the transients at the DRV and MOSFETs Pins.
Have a Nice Day.
Thierry
```

---
## \#11 Posted by: Pimousse Posted at: 2018-01-11T08:27:15.616Z Reads: 326

```
Is the ability to communicate with the DRV through SPI a feature that helps also to protect the DRV against failure ?
Vedder showed in a video the Overcurrent limit setting of the DRV8301 :
https://youtu.be/bivXOlqooCE?t=6m35s

I was convinced that it definitely helped into get rid of DRV failure.
```

---
## \#12 Posted by: Luuke Posted at: 2018-01-11T08:36:15.711Z Reads: 311

```
Can't wait to see more vesc6 alternatives!
```

---
## \#13 Posted by: jmasta Posted at: 2018-01-11T17:44:36.951Z Reads: 300

```
Gotcha!  I agree with you. The accelerometer and NRF chip aren't needed for most purposes and just add cost.  Good luck on the project! I'll keep an eye out
```

---
## \#14 Posted by: SOICDIP Posted at: 2018-01-11T18:35:02.564Z Reads: 293

```
I'm interested in what Vedder had in mind with the accelerometer. 

Would it take it too much space to have pads for the ICs but leave them unpopulated for those who don't need them?
```

---
## \#15 Posted by: chuttney1 Posted at: 2018-01-11T19:31:01.063Z Reads: 295

```
Nope. A good PCB layout of the components matters more. SPI is just a bus interface. I read as much as fast I can. A mosfet and the motor driving chip can be killed from the flowing current from having too fast of a switch on or off time from the gate. There is a relation of that to a voltage transient I have not figure out how is generated. Think of "water hammer" and explains why you have to put a resistor on the gate.
```

---
## \#16 Posted by: chuttney1 Posted at: 2018-01-11T19:33:04.990Z Reads: 292

```
[quote="SOICDIP, post:14, topic:43055"]
Would it take it too much space to have pads for the ICs but leave them unpopulated for those who don’t need them?
[/quote]

Nope. The version I posted has space for these two chips. It's a copy and paste operation to change the file names so Kicad easily recognizes it.
```

---
## \#17 Posted by: Eboosted Posted at: 2018-01-12T06:31:21.923Z Reads: 284

```
It seems I'm the first with a blown DRV8301 on HW6.4, I wondetwhat would be needed to avoid blowing them
```

---
## \#18 Posted by: chuttney1 Posted at: 2018-01-12T07:06:36.100Z Reads: 282

```
What;s the battery voltage you ran at before blowing it?
```

---
## \#19 Posted by: Eboosted Posted at: 2018-01-12T08:50:33.062Z Reads: 283

```
Between 45v and 47v on a 12s battery
```

---
## \#20 Posted by: chuttney1 Posted at: 2018-01-12T08:55:50.601Z Reads: 291

```
Who is the maker of the VESC you have? I'm comparing the addition of the diode present in the FOCBOX versus the VESC without one.
```

---
## \#21 Posted by: Eboosted Posted at: 2018-01-12T08:57:21.164Z Reads: 275

```
I have @stewii ESC hw6. 4, he calls it ESCape
```

---
## \#22 Posted by: Acido Posted at: 2018-01-12T09:02:46.927Z Reads: 274

```
I was just about to order one of these now Im sceptic
```

---
## \#23 Posted by: notepad Posted at: 2018-01-13T17:17:55.761Z Reads: 273

```
im still waiting for someone to do a proper bench test. I need to see how far the Erpm goes.
```

---
## \#24 Posted by: bimmer Posted at: 2018-01-18T04:38:14.011Z Reads: 272

```
Where is the schematic posted.
```

---
## \#25 Posted by: b264 Posted at: 2018-01-18T04:52:17.692Z Reads: 271

```
https://github.com/b264/bldc-hardware/blob/master/VESC_6.pdf
```

---
## \#26 Posted by: chuttney1 Posted at: 2018-02-05T06:47:44.245Z Reads: 259

```
Just a little update. Changes are the addition of a TVS diodes to the signal line of the servo port, CAN transceiver, and one near the MOSFETs. Added pulldown resistors to the low side MOSFETs. The low-side MOSFETs and the TVS diode can be found in the VESCX design.  Reduced PCB size from 70x70 mm to 68.3x64 mm after rearrangement of components. I also figured out the MPU9150 is mostly used in applications regarding drones and airplanes but not much for eskates, so this stays off. There is space for it on this board should it be used.

The TVS diode near the solder pad for power and the pull-down resistors are not required for operation. The TVS diodes is for protection against transient spikes and low side resistors for negating the shoot-through condition MOSFETs can encounter. 

I'm  planning to run my design at redline such as 58 volts. It's pretty much done and ready to be sent to Oshpark.They are just I just have to fix a few things with the silkscreen layer and slap my own maker's mark. The sad part is I can't buy any of the resistors I chose from Vishay on Mouser or Digikey for the next 6 to 8 months. Apparently it's Vishay's new line of automotive resistors for 2018 so it means waiting. I did make a version for the 0603 resistor since they are in stock but  I still want to try my version at redline. I also have to make a case for this.

As for naming this. I'm not branding it like the ESCape, VESC, VESCX, FOCbox, or any other combination of letters to VESC. It's just going to be the generic term "ESC". Other languages the pass such as tank in German is Panzer today versus  schutzengrabenvernichtungpanzerkraftwagendepending (roughly translates to trench annihilation assault vehicle) depending when it was used. [Source for nameing  tank in German](https://german.stackexchange.com/questions/12193/sch%C3%BCtzengrabenvernichtungspanzerkraftwagen). 

  My version will be my mark with no name. 




![fgfgf|690x350](upload://vBBJQvKL77nRcJJ0wxL8aeEfHas.jpg)
![dgdfg|690x350](upload://3LrUFg0cpDAFqt4UU2PkmwkbLh.jpg)
```

---
## \#27 Posted by: scepterr Posted at: 2018-02-05T07:09:54.090Z Reads: 233

```
Check out allpcb.com, used them a couple times already, super fast, great price, great quality
```

---
## \#28 Posted by: Pimousse Posted at: 2018-02-05T08:11:21.827Z Reads: 232

```
Just my 2 cents : I think the cap are on the wrong side as it will be more difficult to desing a thin case and they will also bother the heatsink for the DirectFet.
BTW, are those SMD cap the same rating as the through-hole model used in the original VESC 6 ?
And, finally, using only "ESC" is not a good approach IMHO. We see a lot of derivatives of VESC 6 now. And for the GPL licence, you need to mention "based on VESC(r)" or something. ;)

What the purpose of TVS on servo port and CAN ?
Do they protect against GND loop as we can see in dual setup using Y-split PPM cable ?

This is a great improvement, congrats for your design !!
```

---
## \#29 Posted by: TarzanHBK Posted at: 2018-02-05T09:54:06.020Z Reads: 229

```
a Chuttney ESC!
```

---
## \#30 Posted by: Lospalaz Posted at: 2018-02-05T12:13:54.816Z Reads: 229

```
[quote="chuttney1, post:26, topic:43055"]
Other languages the pass such as tank in German is Panzer today versus  schutzengrabenvernichtungpanzerkraftwagendepending (roughly translates to trench annihilation assault vehicle) depending when it was used.
[/quote]

I'm going to call it "TAAVESC": The _Trench Annihilation Assault Vehicle ESC!_
```

---
## \#31 Posted by: Lospalaz Posted at: 2018-02-05T12:22:21.831Z Reads: 227

```
Ah!, no VESC allowed, I forgot, OK how about this--

TAA8ESC (Pronounced "TASK"): Trench Annihilation Assault Sk8 ESC!
```

---
## \#32 Posted by: chuttney1 Posted at: 2018-02-05T15:41:18.516Z Reads: 233

```
[quote="Pimousse, post:28, topic:43055"]
I think the cap are on the wrong side as it will be more difficult to desing a thin case and they will also bother the heatsink for the DirectFet.Are those SMD cap the same rating as the through-hole model used in the original VESC 6 ?
[/quote]

I don't know how to get the 3D rendering to show the capacitors the way I want it on KiCAD.It's just a placeholder for now. Capacitors are at the same voltage or greater, the capacitance is the same as listed on the BOM..


[quote="Pimousse, post:28, topic:43055"]
What the purpose of TVS on servo port and CAN ?
Do they protect against GND loop as we can see in dual setup using Y-split PPM cable ?
[/quote]

I thought the transient voltage was the issue. Looks like it's back to the drawing board to prevent the ground loop. There were a few cases the CAN transceiver malfunctioned, I can't do testing on this as I don't have another working VESC controller. I'll just assume the best way to protect it from literature posted on the internet for the best thing to use.
```

---
## \#33 Posted by: secupol Posted at: 2018-02-08T10:28:03.564Z Reads: 220

```
I developed SESC of VESC6 clone. It used a DRV8323 device including three shunt resistor.
https://youtu.be/xZLL47S8EhU
```

---
## \#34 Posted by: akhlut Posted at: 2018-02-08T13:20:29.418Z Reads: 216

```
Nice work!
```

---
## \#35 Posted by: chuttney1 Posted at: 2018-02-08T16:40:05.501Z Reads: 214

```
That was the next thing I was going to do. Use DRV8323RSRGZR chip to get rid of the current sensing amplifiers and make a smaller version more applicable to the drones, airplane, and water RC people, but I couldn't code the stuff.

Do you have any plans to release your version's code for implementing the DRV8323?
```

---
## \#36 Posted by: chuttney1 Posted at: 2018-06-26T21:27:56.810Z Reads: 165

```
Update 6/26/2018
:
These are the files to my version. It's two layers and soldered all components. Firmware and bootloader upload through ST-Link work well, but MCU will not give a green light. I post this to the community here for someone to check what exactly I did wrong. 

https://github.com/YBMat/Speed-Controler/blob/master/VESC6.1.3_0603%20version.zip
```

---
## \#37 Posted by: HappyFridge Posted at: 2018-06-30T21:59:41.467Z Reads: 162

```
Hi Chuttney,
Not a real electro man here (more mechanical), but I got myself interested in VESC pcbs too. I looked at your files and have to say that I couldn't find a hard flaw directly. It was also difficult as not all scheme's are in the zipped folder. I assume you checked for solder balls first and couln't find any abnormalities.

I do think however you designed a very small power supply line to the DRV8301. See picture attached. This line (0.254mm)  feeds 3 SPUPPLY pins, which in turn via the 5V output, and via the LM3671, supplies the power for all IC's on the board. I think it is too small.
![small_supply_line|690x478](upload://6D7s0rsO5J67krAlQ74ACn7KW8H.png)
And then there is a huge VCC track from P7 to U3.

Moreover; there are 4 identical CAPS next to eachother. But I do believe they are more to be placed near each corner of the STM32F045. 
![close_caps|587x500](upload://zhIFTnk9PFQdyFQxemwlhavyuyb.png)

C31 doesn't seem connected?
![not_connected|576x500](upload://3eWpoFZzNYClTeBTzmToLZGcr8P.png)
By the way, my Kicad says there are 16 unconnected nets. Most however look connected, but it might be a good thing to recheck these. And solve them...

Maybe try to get some external / bypased power to the +5V/VCC volt pins of the headers? That way you power the IC's with a bit more power.

Hope you can find the problem! Would be a waist of 'lesson learned' (and money :wink:)
```

---
## \#38 Posted by: chuttney1 Posted at: 2018-07-01T05:55:57.807Z Reads: 153

```
Thanks for the feedback. I should state the design I posted only adds the D9 diode to put an Oring Diode as stated by one of the commenters in a different thread. Never heard of an Oring Diode until it was stated. I had to change the footprint for C32 because I was too small when I got the PCB made which was the reason it was unconnected.

 I increased the track width of the supply line to 0.75mm going to the DRV8301 for the 5V output. It should be enough. 


[quote="HappyFridge, post:37, topic:43055"]
Moreover; there are 4 identical CAPS next to each other. But I do believe they are more to be placed near each corner of the STM32F045.
[/quote]

I fixed the row of capacitors in the schematic and PCB file next to each VDD pin as expected. It really is confusing given Vedder made that note and more experienced people like him know how to interpret it. I believe all the VDD pins can be daisy chained to a bank of capacitors by way of a singlecommon power trace, because of the intended operation of placing individual capacitor next to each VDD pin.I'll probbaly have to add one to the 3.3V/VCC rail.

I fixed C31 by adding traces so it connects to C32.

I fixed the polarity direction of D9 to the correct way after seeing in one of your posted pics. It is the 5V rail for all the connectors and supposedly the "ORing" diode. Sadly, USB power of MCU cannot happen so battery power must be applied when wanting to upload firmware to the MCU.
```

---
## \#39 Posted by: akhlut Posted at: 2018-07-01T10:57:03.042Z Reads: 145

```
[quote="chuttney1, post:38, topic:43055"]
I believe all the VDD pins can be daisy chained to a bank of capacitors by way of a singlecommon power trace,
[/quote]

No.  Those caps need to be as close to the VDD pins as possible.  They are acting as filters to clean up the power entering the MCU.  Look at the 4.12 pcb.

http://vedder.se/wp-content/uploads/2015/01/PCB_Front.png

Google 'decoupling capacitor'
```

---
## \#40 Posted by: HappyFridge Posted at: 2018-11-13T20:40:36.359Z Reads: 96

```
Chuttney,
Were you able to solve it?
I just came across this post and remembered you didn't have power too:
http://vedder.se/forums/viewtopic.php?t=195
Maybe it helps.
On a board I did I had the same problems too. Couldn't find any solderjoints, even after checking all pins next to eachother with an ohm meter. But by luck I did see at 3 pins next to each other that I could move when gently pressing them with the tips of the meter :face_with_raised_eyebrow:. It was a sloppy soldering job but I resoldered them (first created a new solder bridge again :confounded:). Solved my problem.
```

---
## \#41 Posted by: chuttney1 Posted at: 2018-11-13T21:12:19.743Z Reads: 92

```
Nope. I'm currently busy with school and I gave someone my Kicad files to figure out. The 5V and 3V3 rail work as expected. Powering VESC straight from USB works as expected but I'm not sure why. I made sure there were 0 solder bridges in the DRV8301 and STM32F4 chip.
```

---
