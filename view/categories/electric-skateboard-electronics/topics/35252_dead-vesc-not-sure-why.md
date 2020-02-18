# Dead VESC not sure why?

### Replies: 31 Views: 1784

## \#1 Posted by: zblad Posted at: 2017-10-10T18:19:46.186Z Reads: 197

```
Went to ride my board today and everything was fine when I put it away last week,  But when I took it out today I noticed only one motor would spin.  So I powered it off and turned it back on and noticed one vesc would blink the red light 3 times and go blue but the other would only be blue no blinking red light.  The vesc that blinked 3 times seemed to work fine.  So I decided to swap motors and hook it to the good vesc and see if the motor was good.  Which it was so I powered it off.  I then went to turn it on again and got a loud pop and now the vesc that was working fine doesn't light up at all.  The other vesc tho atleast has a solid blue light still.  Not sure where to go from here kind of pissed that I basically have $200.00 paper weight.  Does anyone have any components I could check that could be the problem.  I was hoping the vesc had an onboard fuse but I cant find one if it does.
```

---
## \#2 Posted by: Martinsp Posted at: 2017-10-10T18:28:09.381Z Reads: 185

```
Well the one that popped is most probably DRV because if the DRV is faulty (physically damaged->the pop sound) the VESC does not power on.
The one with the blue light only can be more than just one reason. It can happen when there is not enough voltage, firmware problem, faulty component... hard to tell with only this description.
```

---
## \#3 Posted by: L3chef Posted at: 2017-10-10T18:41:09.675Z Reads: 178

```
Canbus or split ppm?
```

---
## \#4 Posted by: zblad Posted at: 2017-10-10T19:03:24.386Z Reads: 167

```
canbus...  Would this have something to do with it?
```

---
## \#5 Posted by: zblad Posted at: 2017-10-10T19:38:19.836Z Reads: 159

```
So the vesc that does get a light it is blue for like 3 seconds then a green led comes on and they both stay illuminated.
```

---
## \#6 Posted by: zblad Posted at: 2017-10-10T20:41:36.274Z Reads: 151

```
I don't get how just powering it on would have caused anything to short out.
```

---
## \#7 Posted by: zblad Posted at: 2017-10-10T21:18:31.429Z Reads: 147

```
http://www.electric-skateboard.builders/t/no-power-to-enertion-vesc/7600/8

so I found this and put my volt meter on that capacitor and I get a beep on both vescs...
```

---
## \#8 Posted by: JohnnyMeduse Posted at: 2017-10-10T21:23:06.575Z Reads: 141

```
If the led light up, it won't be your problem, because the 3,3v is still working. If you just don't see the red led flashing 3 times, it's most likely to be a burn DRV.
```

---
## \#9 Posted by: zblad Posted at: 2017-10-10T21:49:29.006Z Reads: 132

```
ok so what about the vesc with no light think its the drv as well?  I live in thief river falls where digi key is and can get the drv for cost.  I just don't know if I have the skill to replace it myself.  I have a reflow station too.
```

---
## \#10 Posted by: JohnnyMeduse Posted at: 2017-10-10T22:03:41.091Z Reads: 128

```
If there is no light at all, I will suggest to follow the procedure, it might be the can transceiver
```

---
## \#11 Posted by: GrecoMan Posted at: 2017-10-11T01:26:23.062Z Reads: 120

```
ive got DRV_8302.  whenever I press throttle vesc blinks three times then goes back to "normal".  Weird cause it happened while my vesc was sitting in my locker... off
```

---
## \#12 Posted by: Deckoz Posted at: 2017-10-11T01:30:29.135Z Reads: 117

```
That is how my first 4.12 vesc died. I was on lunch came back to the office all was working. Unplugged worked the rest of the day, powered on to leave, motor didn't spin. DRV fault lol... @GrecoMan
```

---
## \#13 Posted by: GrecoMan Posted at: 2017-10-11T01:32:45.248Z Reads: 115

```
weirdest part was that I turned it on before I put it on the ground and it worked beautifully then.  The second it hit the ground, instant drv failure
```

---
## \#14 Posted by: Namasaki Posted at: 2017-10-11T01:52:03.646Z Reads: 111

```
[quote="GrecoMan, post:13, topic:35252, full:true"]
weirdest part was that I turned it on before I put it on the ground and it worked beautifully then.  The second it hit the ground, instant drv failure
[/quote]


did you put it carefully on the ground or let it drop to the ground>?
```

---
## \#15 Posted by: GrecoMan Posted at: 2017-10-11T01:53:56.308Z Reads: 109

```
I dropped the front from about 2 inches off the ground. It’s not the first time I’ve done that
```

---
## \#16 Posted by: Namasaki Posted at: 2017-10-11T01:54:37.923Z Reads: 109

```
I was just thinking that it might have jared something loose
```

---
## \#17 Posted by: GrecoMan Posted at: 2017-10-11T01:56:14.110Z Reads: 106

```
I thought of that too but it’s not like everything wasn’t VERY carefully insulated.  A small drop shouldn’t have cause the drv to just pop out
```

---
## \#18 Posted by: Namasaki Posted at: 2017-10-11T02:02:57.787Z Reads: 104

```
I had one of the my battery packs fail once because of a really rough road. The main pos lead broke loose from the solder tab.
```

---
## \#19 Posted by: GrecoMan Posted at: 2017-10-11T02:03:58.126Z Reads: 103

```
I waaaay overpaid for a torqueboards 6s2p pack ($185) and voltage is good and none of the leads are bad.
```

---
## \#20 Posted by: Namasaki Posted at: 2017-10-11T02:05:36.982Z Reads: 99

```
I was just giving an example of what excessive vibration or shock can do.
These components are not bullet proof.
```

---
## \#21 Posted by: GrecoMan Posted at: 2017-10-11T02:07:09.937Z Reads: 95

```
Oh yea it was probably user error but not sure how.  I was running conservative settings and only at about 40kerpm when flat out.  The weird thing is how long it worked with the exact same setting before
```

---
## \#22 Posted by: JohnnyMeduse Posted at: 2017-10-11T04:01:03.002Z Reads: 85

```
Guys... when are going to understand that the 60K limits is never really a issue if the rest of the setup is alright. @GrecoMan it doesn't take much to kill a DRV (specially on certain kind of vesc, might be bad soldering), just touching two wire for less than a millisecond is enough.
```

---
## \#23 Posted by: Nix Posted at: 2017-10-11T04:17:42.255Z Reads: 85

```
@JohnnyMeduse What do you mean "if the rest of the set up is alright" 😕
```

---
## \#24 Posted by: I82 Posted at: 2017-10-11T06:09:28.505Z Reads: 82

```
Yep. what do you mean? I am about to send back 2 245kv motors and go get 200kv to run "safe" VESCs with 10s li-ion battery.....
```

---
## \#25 Posted by: zblad Posted at: 2017-10-11T17:48:57.087Z Reads: 75

```
replaced the transceiver on the dead one and it WORKED. Super excited right now. But the other vesc still lights up blue and green and I can hook it to the pc and get no fault codes.  But after a minute of being plugged in I felt the transceiver and it was SUPER hot.  So is it possible its like half assed burnt out?  Also I don't know if I'm looking for faults correctly I went to the terminal window and types fault and it says no faults.  Am I doing that wrong.  I tried doing a motor detection and it fails with no fault code still.
```

---
## \#26 Posted by: xxlv Posted at: 2017-10-11T20:07:24.995Z Reads: 68

```
For can Bus, see this: http://www.lp-electronic.com/vesc/connect-two-vesc-via-can-bus/
Especially the electrical part.
```

---
## \#27 Posted by: zblad Posted at: 2017-10-11T20:22:52.094Z Reads: 65

```
im confused my can bus always worked.  I litteraly rode my board and everything was fine.  Put it away went to ride it a week later and my vesc only has a blue and green led that light up.  The red led never blink 3 times and I get no fault codes.  going to try replace the transceiver tonight if that don't work ill order the drv chip and attempt that as well....
```

---
## \#28 Posted by: JohnnyMeduse Posted at: 2017-10-11T21:19:22.184Z Reads: 62

```
What procedure do you use for powering up your board, do you use a simple switch or a lipos and Y connector, so you need to plug back your vesc each time?
```

---
## \#29 Posted by: JohnnyMeduse Posted at: 2017-10-11T21:35:10.174Z Reads: 64

```
If you just started in the eboard I suggest you to follow tye 60k, or else you would have to play with some parameter that can damage your vesc if they are wrong... Also it highly depend on the type of Vesc your using, the motor, and the firmware. On the bench we have been able to push some Focbox over the 100k limits (I don't recommend trying that)...
```

---
## \#30 Posted by: I82 Posted at: 2017-10-11T22:48:29.902Z Reads: 62

```
Not really new to e-sk8, just find innecessary  to burn things. 
I opened a specific thread(poll included) about my matter.
I think I will play safe and get lower kv motors for my new build ;)

Edit: it will be local soldered vescs, ackmaniac firmware, 4.12 hw.
```

---
## \#31 Posted by: zblad Posted at: 2017-10-13T18:13:49.024Z Reads: 54

```
So I replaced the drv and now I actually get the blinking leds but now it says drv fault is there anything else I can test I was extremely careful soldering it on so idk why I'm getting this error.
```

---
