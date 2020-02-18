# Does Mellow Boards Have the Quietest Longboard?

### Replies: 8 Views: 2155

## \#1 Posted by: stuxtruth Posted at: 2016-09-08T00:17:11.992Z Reads: 244

```
Seems awfully quiet. 

http://youtu.be/jExeJhXHVgg
```

---
## \#2 Posted by: Grosso Posted at: 2016-09-08T05:05:08.919Z Reads: 218

```
When can you buy this thing?

Even when you can buy it, isn't it like $1800? That's a crazy price.
```

---
## \#3 Posted by: Nate Posted at: 2016-09-08T05:07:02.241Z Reads: 221

```
All that research and testing ain't gonna pay for itself :joy:
```

---
## \#5 Posted by: Nismo Posted at: 2016-09-14T08:24:10.332Z Reads: 183

```
Their 4x4 (dual units) drive looks amazing.  The possibility for me to make two electric rides from one so that I can go for a ride with the girlfriend/a buddy is a great way to share the sport with others.  Also seems like one of the safest way to trust the brakes as it doesn't cut out when over charged, and you always have a back up, not just the rear unit to count on.  I need to see this in action.
```

---
## \#6 Posted by: Mellow Posted at: 2016-09-27T15:33:59.022Z Reads: 149

```
Mellow here. Yes, research and testing...but development, materials and manufacturing as well. "Made in Germany" translates loosely by "performance before profit". Our Drive has features you literally won't find anywhere else, not even in DIY (yet).

- Why does our stator have nearly 1,000 pieces instead of 100?
- Why do we use brand name microprocessors under the hood where no one will see? (Good on Vedder with the STM32F4 in VESC's specs btw)
- How did we make our braking available 100% of the time without hurting the battery? 
- How did we fly through 4 airports with 4 Mellows with 0 problems?
- Why don't we play the word game using "water proof", "water resistant", "weather proof" at the same time? 

@Nismo The configuration you describe would technically have 3 backup brakes. Talk about redundancy. If you guys have further questions, fire away.
```

---
## \#7 Posted by: SimosMCmuffin Posted at: 2016-09-27T18:26:21.854Z Reads: 138

```
* More pieces on stator, because all the stator teeth are separate (a lot of laminations in total) and then assembled into a complete set. This gives better winding density with easier winding itself.
* Why use brand name microcontrollers? Much better benchmarking done by manufacturer and simply quality of component and documentation. (I'm using Atmel's ARM M0+ MCU on my own controller).
* If it's just to protect the battery at full capacity, then it means you're pumping all that regen current somewhere else... Can't think where off the top of my head, maybe some kind of novel solution :D?**Figured it out by reading your kickstarter updates: " By adding the thermal breaking resistor we ensured the breaks of the Mellow Drive will never have to shut off due to a full battery or in order to not harm the Mellow Drives electronics."**
* Small enough capacity (< 99 KWh) per unit to allow carry-on with most airlines. Maybe units were distributed between multiple people?
* I'm guessing you're laughing at the marketing people who use the "water proof" word to market their product, even though it's only water resistant. I'm guessing, seeing how you guys are going for quality that the unit is truly water proof.

Any one of these even close?

I'm a student at the Finnish polytechnic university of Tampere, specializing in embedded systems and have gathered a team to develop an esk8. Not sure at this point if we're going commercial with it, but time will tell.

I wish the best to you guys at Mellow and I will keep my eye on your future updates!
```

---
## \#8 Posted by: Mellow Posted at: 2016-09-28T23:04:19.709Z Reads: 101

```
Nice work @SimosMCmuffin:

* Exactly
* Nice. A brand name isn't obligatory but Texas Instruments is an established value in BDLCs, and our manufacturing partner has a long history and proven expertise with them. Our MP is the Piccolo (TMS320F28069F).
* Great find. Our bad: brakes not breaks. Can you imagine buying a car, and the salesman tells you: the brakes "almost always" work!
* Oops, just the opposite: as external power packs (there's a USB port) a single passenger can even carry on up to three Mellow drives. The rest was just put into checked-in baggage. 
* Yes. Our entire system + remote is IP65. Others say "weatherproof" but only for a few drops on the battery/ESC. while the remote and motor windings are hugely vulnerable to water damage.

Sounds lnteresting. What's your setup and use scenarios?
```

---
## \#9 Posted by: SimosMCmuffin Posted at: 2016-09-29T08:47:05.821Z Reads: 88

```
The easiest way to see the current setup, is check out this Imgur album that I made couple months back: http://imgur.com/a/Mjodj

I have already a lot of improvements planned for it in the motor controller, powertrain and battery departments.
I also held a presentation at my local university for students about the board and asked if any of them were interested in coming with me to develop it. I presented 3 bachelor's degree eligible works for it: BMS, remote controller and smartphone app. 
Out of ~14 students (from embedded systems specialization) 5 were interested and I then interviewed them and picked 3 to the specific bachelor works. Yesterday I held them a short tutorial on how to use Cadsoft's EAGLE PCB design software.



----------

**Brakes!** I went last week to the biggest local hill to do some testing on the board's performance and suffice to say, I learned a lot of the limitations of the current build! I started the test from the top, going down and went with pretty much max braking. It's 12 degree hill, but that feels surprisingly steep. Talked with a local and he said bicycles hit about 80 km/h at the bottom and there has been a death, caused by two bicycles colliding at a junction at the bottom of the hill. 
I got about 2/3 of the way down when I suddenly lost braking. Thankfully to my ninja reflexes I just stepped of the board and stopped it with my foot. Luckily I was going so slow with the max brake. Walked to the bottom of the hill and opened the board and felt the battery (was pretty cool) and the already quite cooled motor controller, but I then suspected that something must have went into over temperature protection. Looked for the Texas Instruments' DRV8302 mosfet driver IC datasheet and it indeed had an over temperature protection at 150 degree Celsius, at which it cuts all driving signals to MOSFETs, so I was pretty much cooking the controller.
The fact that the board worked again no problem also lead me to the over temperature protection conclusion, so I then rode another way back home. A way that didn't have big hills.

I have two remedies planned to help the situation: 
_Higher battery voltage_, current battery is 4S (14.4V) so I'm thinking of going to 12S just to lower the currents, especially on the high side FET, which causes most of the heating in regen braking, due to the current going through the MOSFETs body diode. So that should lower to 1/3 if I triple my battery voltage. 
_Dual motors_, which means dual power stages on the controller, which means double the surface area to dissipate heat + lower current per motor when compared to single motor current. This also helps to reduce the waste heat caused by regen braking.

I'm planning to conquer that hill one day... going both ways...

**The most important thing to take away is:** The rider has to always feel like he/she is in control of the board, if this trust is broken, the ride will turn from fun and good times to dread and bad time.



----------
**Texas instruments, BMS and BLDC'**

I accidentally, when browsing DigiKey for BMS components, noticed this:

<img src="/uploads/db1493/original/3X/c/a/ca952e8d6269ffd082bc1537859817ee3dc15e67.png" width="689" height="299">

"Interesting" I thought, because I had earlier read your kickstarter update where you talked about your BMS and using impedance tracking to figure out the capacity. Turns out "Impedance Track™" is a _Texas instruments_ trademark. and then based on your reply above this one:
[quote="Mellow, post:8, topic:9175"]
Nice. A brand name isn't obligatory but **Texas Instruments is an established value in BLDCs, and our manufacturing partner has a long history and proven expertise with them. Our MP is the Piccolo (TMS320F28069F).**
[/quote]

This lead me to conclude that you were also using TI components in your BMS, as the "Impedance Tracking" is only found on TI products and you are also using the Piccolo with "InstaSPIN-FOC" (1 for each motor, based on looking at the kickstarter update pictures) and the above quote.



----------
The current motor controller's MCU is Atmel's AVR Xmega256A3, but after discovering I had butchered the ADC design on the board to be so noisy that I didn't use any of it. I decided to improve it on the next iteration and also went for a upgrade on the MCU side to an ARM platform, also from Atmel. 
The next controller will have SAMD21J M0+ MCU, which is a new platform to me, but I decided to start learning it, because I thought it would help in any future employment searches when I can say I have experience in the ARM platform.

**Whoo, that was a bit longer reply than I expected :innocent:**
```

---
