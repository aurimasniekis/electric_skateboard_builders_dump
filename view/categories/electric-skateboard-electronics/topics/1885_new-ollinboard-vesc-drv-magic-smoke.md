# New ollinboard VESC DRV magic smoke

### Replies: 29 Views: 5062

## \#1 Posted by: unicycleking Posted at: 2016-03-20T18:51:53.188Z Reads: 333

```
I just received a new VESC from Ollinboard.  I adjusted the settings using a current limiting power supply at 12V and 10A. After successfully running the auto detection, and adjusting the voltage cutoff settings, I tested it with full 12s voltage.  The motor would spin up with no load, but had  no torque when a load was applied.  The motor would just cog.  Even when allowing the motor to reach a higher RPM before applying a load, the motor would cog.  I tried increasing the startup boost to 0.1, but that didn't help too much.  I did a little more bench testing, trying different startup boost settings.  The last time I tested it with the full 12s voltage, I saw smoke coming from the DRV chip.  Any help with this issue is greatly appreciated.  It's pretty frustrating since I just received the VESC.

 - New Ollinboard VESC
 - new Enertion r-spec 190kv 6355 motor.
 - 4 3s 5000mah SMC batteries in series (12s)
 - GT2B radio

<img src="/uploads/db1493/original/2X/8/837c15f54f3b890f4d42754e7c6313bbe2e35216.PNG" width="690" height="394"><img src="/uploads/db1493/original/2X/c/cea70ae6f8821ed3aa15268523ed7c629032777b.PNG" width="690" height="394"><img src="/uploads/db1493/original/2X/e/e3da651dfa9a0bc9af82af341d170eefe7da20cf.PNG" width="690" height="392"><img src="/uploads/db1493/original/2X/6/61c95d3cedca4a067adb5371f9469640c361b49e.PNG" width="690" height="395"><img src="/uploads/db1493/original/2X/f/f80dbae999e2ed9e471dfb3d3ae2c22c98600f1b.PNG" width="690" height="393"><img src="/uploads/db1493/original/2X/7/7efba37de1a515e9591f2252de3a325560d89750.jpg" width="690" height="388"><img src="/uploads/db1493/original/2X/5/5f3ec6009f0d76206f5014806365782959707267.jpg" width="690" height="388">
```

---
## \#2 Posted by: claudiofiore88 Posted at: 2016-03-20T21:16:58.163Z Reads: 294

```
Your DRV chip is probably toast. I suggest contacting @Chaka about the matter.
```

---
## \#3 Posted by: treenutter Posted at: 2016-03-20T22:10:39.832Z Reads: 293

```
Sorry to hear it @unicycleking. The images of your BLDC Tool screens are really helpful.I took a look at them and nothing seems out of place to me. You've got the voltages right AFAIK, and you did the right thing by using a low current power supply when you configured your VESC.

It seems clear, as @claudiofiore88 notes, that your DRV chip probably needs to be replace. 

As to why... the only thing that comes to mind is whether you attempted to flash the firmware and perhaps selected the wrong file to flash. If you don't use the right firmware for your HW version of VESC, you can toast it.

In either case, you're in luck because @chaka is responsive and will get you up and running in no time!
```

---
## \#4 Posted by: unicycleking Posted at: 2016-03-20T23:25:39.690Z Reads: 279

```
Thanks for the replies.  The DRV chip is definitely toast, as there is a big burn mark on it.  I am just curious about why it fried.  I have not flashed any new firmware on it, and I am using the latest version of BLDC tool.  It is getting frustrating trying to get the VESC working correctly.  I had many problems with my last VESC from Enertion, and eventually the DRV chip blew on that one too.  I bought a new VESC from Ollinboard because I have read the quality is better (it does look much better).  But at least I could get the Enertion one to work intermittently.  If anyone can find a problem with my settings, or has any ideas on how to prevent the DRV chip from blowing, it would be helpful so I don't blow another one.
```

---
## \#5 Posted by: chaka Posted at: 2016-03-21T03:33:37.104Z Reads: 267

```
Go ahead and send that vesc back to me and I will replace the drv chip. There is a good chance you have a short in your phase wires. Do you mind posting some pictures of your connections?

I will run the vesc through its paces before sending it back to rule out anything else.
```

---
## \#6 Posted by: unicycleking Posted at: 2016-03-21T05:19:07.775Z Reads: 267

```
Thank you very much @chaka.  I will send it back.  I don't see how my phase wires could have a short.  All my connections are shrink-wrapped 5.5mm bullets with electrical tape.  Maybe the motor could have an internal short?<img src="/uploads/db1493/original/2X/c/c24840bdd97c667d3fe5e91e7774815f99240205.jpg" width="690" height="388"><img src="/uploads/db1493/original/2X/7/7e9c6d01052e7b3878910e4659c042ca72cb2e94.jpg" width="690" height="388">
```

---
## \#7 Posted by: BigAl Posted at: 2016-03-21T16:25:12.693Z Reads: 251

```
Thats how it's done!  Customer service, it's really not difficult!
```

---
## \#8 Posted by: Iceni Posted at: 2016-03-21T17:59:10.065Z Reads: 253

```
Worst case it could be the motor, it has happened to me recently.
Though it was the way i oriented the motor, had the wires facing toward the center of the deck instead of toward the trucks.
Doing so made the wires rub off the insulation inside the motor, causing a short. I was lucky to not burn out my vesc.

Not sure how you have your motor mounted.
But if you have a multimeter, check for shorts between your phasewries and the motor housing.
```

---
## \#9 Posted by: chaka Posted at: 2016-04-14T16:41:26.196Z Reads: 238

```
Well I repaired your VESC and promptly fried it during load testing! I wish you had told me you messed with the max current ramp settings. I am going to have to send you a completely rebuilt VESC but you are on notice for being click happy with the settings. ;) If you blow another one I am going to have to charge you little for the repair service.

Please take some care with this next unit, you may have a motor with a small short in the phase wires. Those r-spec's don't have shrink wrap deep enough into the housing and the wires can rub on the machined aluminum. How many miles have you ridden that motor?
```

---
## \#10 Posted by: longhairedboy Posted at: 2016-04-14T17:19:39.097Z Reads: 239

```
[quote="chaka, post:9, topic:1885"]
Those r-spec's don't have shrink wrap deep enough into the housing and the wires can rub on the machined aluminum.
[/quote]

I have seen evidence of this as well, pretty recently in fact.
```

---
## \#11 Posted by: CSN Posted at: 2016-04-14T20:02:12.381Z Reads: 228

```
How would people go about modifying the R-spec so it doesn't cause a short? or what is the best 63xx motor to upgrade to? 

With long enough shaft to run 12 or 15 mm belt?
```

---
## \#12 Posted by: chaka Posted at: 2016-04-15T03:41:37.488Z Reads: 230

```
I ran a tacon 160 on your board when I was testing the  VESC. I had it geared a little tall but it would probably be perfect with the gear ratio you have now.  

Board would top out around 25-28mph so it will be a little fast compared to your current setup. I want to say it will still climb ok but I honestly don't know how it will compare since it is a larger motor. 

For anyone wondering here are the systems specs on the board we are talking about:  8s lion, 16/44 tooth on 97mm wheels
```

---
## \#13 Posted by: unicycleking Posted at: 2016-04-15T06:01:04.249Z Reads: 228

```
Thank you for doing all that!  I'm not sure how the max current ramp setting was changed.  I am not aware of changing any settings in the advanced tab other than the startup boost.  I did try to rule out any problems with my settings by posting screenshots of all the settings in the original post.  

It does seem likely that I have a short in the phase wires.  The shrink wrap did look a little short.  The motor has been ridden about 100 miles. I will make sure to keep those wires insulated when testing the new VESC.
```

---
## \#14 Posted by: chaka Posted at: 2016-04-15T12:49:38.030Z Reads: 227

```
I had checked your screen shots. They were set to default when the screen shots where taken but it was set 10X higher when I had received it. Luckily I build these gems so it isn't a big deal to rebuild on a fresh PCB.
```

---
## \#15 Posted by: Skitzor Posted at: 2016-06-20T16:10:05.887Z Reads: 206

```
Sorry to fall in in your topic but I got advised by @HH1 to take a look here.

<img src="/uploads/db1493/original/2X/c/c09868d07088603db5880e9f3bbd25a4978425bc.jpeg" width="666" height="500"> 

Take a look at the windings, all 3 in contact with each other and the aluminum of the motor. If I compare this to my good one it's exactly the same. Should I worry about my vesc drv chip beeing blown up as well? I've ordered 2 new spare motors already, but the Vesc would set me back months... I can still do motor detection trough the BDLC tool though... It just shuts down my battery (thank god for safety circuits)
```

---
## \#16 Posted by: Hummie Posted at: 2016-06-20T17:07:13.480Z Reads: 199

```
That's a lot of wire that's doing nothing on top of the stator. Weird to see so much. About it shorting though..best way to tell is use an LC meter to measure the inductance as a multimeter isn't accurate enough.  20$
```

---
## \#17 Posted by: Skitzor Posted at: 2016-06-20T17:55:47.065Z Reads: 197

```
I should probably have access to a one at work. Thanks for the tip.

But just for clarity. Sorry for the most logical question ever btw: But given my 2 motors are exactly the same... The 3 wires should not touch at all right? (Even if they would be treated with a isolation product, it's still stranded wire which could make contact easily)
```

---
## \#18 Posted by: Hummie Posted at: 2016-06-20T18:09:25.772Z Reads: 190

```
They can touch. They're converted in a thin enamel.
```

---
## \#19 Posted by: HH1 Posted at: 2016-06-20T18:31:31.648Z Reads: 188

```
maybe @longhairedboy can shed a bit more light on this as he is also working with this motors
where you should heatshring the wires or  where it is not necessary.
```

---
## \#20 Posted by: longhairedboy Posted at: 2016-06-20T18:53:09.985Z Reads: 191

```
That's typical. @Hummie is right about the windings being enamel coated, they can touch inside the can like that, they're designed to do that. 

What does end up happening though is the heat shrink at the end of the windings that is near the hole in the motor can ends up coming loose, and if your phase leads are moving around too much because they aren't bunched correctly to allow movement, the part of the lead that is in the can which becomes the windings (the part clearly shown in the image above) will start to rub together. once they start rubbing, the enamel will start to rub off and chip, then you have shorts. 

So when you're done rewinding, or even just replacing your phase leads like i do on occasion with colored ones, make sure you do what you can with the heat shrink to keep those phase leads from moving around inside the can. and when you run the leads to the ESC, make sure you have slack so that when you carve there isn't any tension on the leads. I like to curl mine in such a way that they don't stress. Enertion does something similar on the raptors.
```

---
## \#21 Posted by: Skitzor Posted at: 2016-06-20T19:58:35.134Z Reads: 178

```
I'm not sure what I've done. Which makes this still a problem...

I played with the heatshrink and put the wires as nice as possible without disconnecting anything. I put the remote on my second vesc and tested again. It's working again !!!
Next thing I did is soldered the two vesc's together again ( master/ slave connection) alligned everything as it should. Both motors up and running again. Just did a small test-drive of a kilometer. Like nothing ever happened...

So what's the cause of this short exactly (as a hit on my wheels, obviously not motor, could trigger it) 
Should I try to put some extra glue/heatshrink on the part where the wires enter the motor so they absolutely don't move anymore? Your thoughts on this please !
```

---
## \#22 Posted by: longhairedboy Posted at: 2016-06-20T20:00:12.524Z Reads: 174

```
@hummie might have a better idea on what kinds of adhesives you can use to lock down wires inside a motor. But in general, it sounds like a good idea.
```

---
## \#23 Posted by: Skitzor Posted at: 2016-06-20T20:03:06.160Z Reads: 176

```
Well, I'm good in electromechanics. These are my first steps in DC-motors though. But if I would make those motors, the wires coming in should have a little more heatshrink on them and at least some form of strain relief, with these kind of applications with a lot of stress and movement on them.

Edit: btw, @longhairedboy, @HH1 and @Hummie. Thanks for pointing me in the right direction ! Hence the power of this forum!
```

---
## \#24 Posted by: Hummie Posted at: 2016-06-21T01:22:35.130Z Reads: 174

```
Hi. I don't remember or know if u ever wrote what makes u think u have a short. And now u don't?  Humm. Maybe u did jiggle something away from something. Does the motor behave just as well as it had and does it get just as hot?  

U can use a multimeter and check for a circuit between the motor housing or the stator and the leads.  But shorts in the windings u need the LC meter


.there's spray on enamel that's intended for windings I think
https://www.zoro.com/sprayon-red-insulating-varnish-20-oz-s00601000/i/G1811056/?gclid=CjwKEAjwqJ67BRCzzJ7Hy-LYlFYSJABwp9PGwJPlGpKe9W4281qzty2FW9OJNlFIwT0hu06I1ZHaURoC1K7w_wcB&gclsrc=aw.ds
I've put a lot of epoxy on motors to secure windings and other reasons but u want a thin coating and to have nothing rubbing coming through the housing. But maybe u don't have a short to begin with and I forget ur what happened
```

---
## \#25 Posted by: flatsp0t Posted at: 2016-06-21T07:06:30.064Z Reads: 170

```
http://www.electric-skateboard.builders/t/raptor-dual-motor-breakdown-any-help-for-quick-shipping-appreciated/4868

This came from there.
```

---
## \#26 Posted by: Skitzor Posted at: 2016-06-21T07:41:19.560Z Reads: 169

```
I'm still not 100% sure, but the heat shrink (3 wires together going in motor) was wiggly. I've put the wires nicely. There were actually 3 small wires (stranded wire) broken and touching the aluminum. which I've cut off as well. So it makes sense if it's only coated on the outside. So this was the temp solution.

I'm now going to look into some product to insulate them better. I've got plastic spray laying around (used for PCB's), a heated glue gun and some liquid isolation spray. (has a more rubber texture) I'm thinking of spraying that over the excess wire below the coils to keep them nice and tight + insulated and glue the incoming heatshrink as tight as possible
```

---
## \#27 Posted by: chaka Posted at: 2016-06-21T14:04:03.918Z Reads: 172

```
I use Glyptal 1201 when rewinding motors. They have several different products but 1201 works well for coils etc. Hot glue will melt at operating temps so it may not be a good idea.
```

---
## \#28 Posted by: Hummie Posted at: 2016-06-22T04:12:56.158Z Reads: 168

```
The vesc u can use to find shorts with its induce  and resistance measurements
```

---
## \#29 Posted by: charliek Posted at: 2016-12-19T10:05:16.849Z Reads: 92

```
Hey guys I have the same problem here. Motor wouldn't spin under load and it makes weird noise. I've disassembled the motor to have a look if there is any short. Seems like none of the wires are touching each other and heat shrink is in place. Is there anything that I'm missing here?<img src="/uploads/db1493/original/3X/2/9/29b7c2cc773191f47835610ce17af00436c861b2.jpg" width="281" height="500"><img src="/uploads/db1493/original/3X/0/9/09aa98a5cf39572b30df56895a3218351845580b.jpg" width="281" height="500">
```

---
