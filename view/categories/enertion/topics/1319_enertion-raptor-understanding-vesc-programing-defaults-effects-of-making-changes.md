# Enertion Raptor &#124; Understanding VESC Programing Defaults &#124; Effects of Making Changes

### Replies: 67 Views: 8142

## \#1 Posted by: thomwithah Posted at: 2016-02-11T13:48:50.703Z Reads: 396

```
Continuing the discussion from [Enertion Raptor | First Batch Problems &amp; Solutions](http://www.electric-skateboard.builders/t/enertion-raptor-first-batch-problems-solutions/1296/51):

[quote="onloop, post:51, topic:1296, full:true"]

The Low Voltage Cut off (LVC) of S.P.A.C.E Cell is 28v
This is roughly how the LCD is programmed.
42v = 100%
40v = 80%
37v = 50%
35v = 30%
33v = 10%
32v = 0%

Once the battery reaches 0% **under load** you will probably be hitting the LVC - which means **OFF**

From now on I'll program a soft voltage cut-off at 33V and hard cutoff at 28v, this way if you approach a hill the board won't shut off rapidly. It will slow down.

**I highly recommend that everyone considers making this change or not riding up hills with low % battery**


<img src="/uploads/db1493/original/2X/7/7832a20b4c603e3e4acd637ee80bb0041fcd9145.png" width="539" height="380">

ALSO, you guys might want to get something like this to help with accessing the USB port on the VESC.

search something like this: **"Mini USB Male to Female Right Angle 90 Degree Adapter"**


<img src="/uploads/db1493/original/2X/9/9067058f1348b5af0d45e60e0e328e865b2f333a.png" width="501" height="500">
[/quote]


----------


----------


----------


Do these new recommended numbers leave no room for a situation (even with a heavy rider and hills) in which the board would lose function? I mean it has a battery, right, it can't go forever... So, what happens as the battery capacity is reduced and eventually is depleted to the low voltage cutoff? Do these new recommended numbers mean the board will reduce performance for a period to give the rider a "heads-up" that they are approaching a point of no power? If so, can that period of time be extended by adjusting these numbers? If not with these number fields, is that an option some other way? I would think the potential for sag would be greater for the Raptor Dual. So, are these recommended numbers good for both the Raptor Mono, and Raptor Dual?  With the new numbers what would be the relationship between the boards performance and the LCD readout. Is it simply 10% = full performance, 0% = nothing? 



If the battery cutoff end is at 28v and cutoff start is at 33v I take it to mean that the Raptor will slow down when the display is at 0 (33v) and kill the motors (and everything else) at 28v the LVC. Is that correct?  Doesn't that still mean that under load it *could* cut out going up hill, due to battery sag? Would it be better then to make the cutoff end 29v (or 28.Xv) to ensure that the board always had battery power, and therefore, reasonably, brakes if it has momentum? Would setting the cutoff start at, say, 34v give the result of more lead time till cutoff simply at the cost of time at max performance? If not, what would the results be? 

I've tried reading a bit in different areas about the VESC programming and battery voltage sag. I couldn't find the direct information I was looking for. I was confused about the different battery chemistry's voltages and susceptibility to sag, along with the exact function of these parameters in the VESC. I'm certain there is some level of flexibility here, and would like to completely understand the effects of modifying these numbers.



Basically, I don't have an understanding of the effects of this programming.  I would like to. I want to make sure nothing like what @Xusia experienced ever happens to me. I'm a heavier guy, about 205+ lbs with a pack and gear.. I suppose this means the board will experience more load than typical. I also live in a hilly area, at the top of a very long steep hill, so I'm guessing this will make the problem these numbers intend to correct an even more likely problem for me if I didn't change to them, or something else, from the currently shipping default numbers.

I'm not trying to be a lazy ass, and be spoon feed all the answers. I would just as well like to see links to were I can study and figure all this out. That said, I wouldn't mind having it all laid out here and perhaps other Raptor owners can benefit too. I'll break this off, so it doesn't distract from more pressing matters, as well. 

Maybe we can share all our **Raptor specific** VESC findings here for the time being.
```

---
## \#2 Posted by: treenutter Posted at: 2016-02-11T21:30:36.921Z Reads: 341

```
@thomwithah it's good that you're thinking about this; I use a VESC and before I set these parameters properly I would get knocked off during a voltage sag; either through rapid acceleration or low battery power. Since I corrected the parameters, it hasn't happened.

There should be a thread about how to avoid "tripping" VESC and what to do to make sure it doesn't happen. It can be ugly.
```

---
## \#3 Posted by: onloop Posted at: 2016-02-11T21:49:03.592Z Reads: 337

```
- The idea of a soft cut off is to bring the board to a slow stop, instead of an instant OFF state.
- The numbers I gave won't be good for everyone, some people might want the soft cut to begin earlier, some people might not need a soft cut as they will simply learn what percentage hard cut occurs for them.
- Increased rider weight & high current draw from hill climbing will make voltage much sag more, especially near the end.
- Increasing the cutoff start voltage above the cutoff end may need to be customized to each environment & the individuals expectations.


**Batteries are not linear in their discharge curve, they quickly drop from 4.2 to reasonably steady voltage range of between 4 & 3.3 - after 3.3 they can drop off very quickly under high load.**

<img src='/uploads/db1493/original/2X/2/244bba1fdc99d82eb112cad6e68983edb0940dae.jpg'>


At the end of the day, once a battery is depleted the board won't work anymore as an electric board. It becomes a normal skateboard which won't roll up hill and won't stop when rolling downhill, try to keep this in the back of your mind. 

From one perspective tweaking these settings becomes nearly redundant. It's an ongoing debate I keep having with myself... Should I have de-tuned the raptors to make them less powerful? (more safe) In the end, I said no! leave them at max settings.... maybe that was a mistake.

If there is enough demand from raptor owners ill spend the next week trialing a whole bunch of new settings that make the raptor more, um... how do I say this without sounding like a complete dick and offending everyone... *"Fool Proof"*

I could do a number of things.
1. RPM limit & soft cuts
2. Lower Motor Current (make startup much slower & safer) This will also make the remote less sensitive because it is in current control mode.
3. Set soft voltage cuts
4. Maybe lower battery current to reduce voltage sag. This will also make the remote less sensitive and likely increase range.

In fact I could try to emulate a "boosted boards" style profile... I test rode one for 3 hours yesterday.... it's much more beginner friendly, but boring after about 5 minutes.
```

---
## \#4 Posted by: Blasto Posted at: 2016-02-11T22:11:52.652Z Reads: 277

```
Shouldn't the "batt cutoff end" on the VESC be a little higher than the BMS cutoff to avoid the power being suddenly cutoff?
```

---
## \#5 Posted by: onloop Posted at: 2016-02-11T22:21:40.562Z Reads: 270

```
it's the same thing. once the battery is empty there are no settings that can make the board keep working
```

---
## \#6 Posted by: Tarzan Posted at: 2016-02-11T22:28:25.451Z Reads: 275

```
I don´t think that those drastic changes are necessary. I love the pure unfiltered power of the Raptor!
You  become used to it after 20 min of riding. Okay the first minutes are scary but it comes predicable quick.
The solution from Bossted it superb because you can use an app to make the change.
Personally I think it is some kind of over engineered because you use the App just once while owning a Boosted Board. Sure a really nice gadget but imo not necessary. 
For the Raptor you should use some electrical tape to limit the travel of the joystick :D I know it sounds ridicules but it would be a hardware beginner mode. Easy and without this VESC magic to get the full power.
Edit: The soft cutout makes sense of course!
```

---
## \#7 Posted by: onloop Posted at: 2016-02-11T22:29:23.057Z Reads: 264

```
ATTENTION ALL RAPTOR OWNERS
---------------------------



I am now offering you all a **FREE 2 HOURS VESC** programming support package

See here: http://vesc.net.au/support/


Please use this time to get some help re-programming your vesc with your own custom settings. He has a raptor so can help you de-tune it.

I'll pay @jacobbloy for the service he offers you. If you need more time with Jacob you can arrange to pay for that.
```

---
## \#8 Posted by: Tarzan Posted at: 2016-02-11T22:30:59.892Z Reads: 259

```
That is awesome customer service. Thank you very much! :smiley:
```

---
## \#9 Posted by: Blasto Posted at: 2016-02-11T22:35:53.518Z Reads: 254

```
[quote="onloop, post:5, topic:1319, full:true"]
it's the same thing. once the battery is empty there are no settings that can make the board keep working
[/quote]

yes i know, what i mean it would be preferable to have the VESC gradually cuting off the power than the BMS kicking in and suddenly cutting everything off
```

---
## \#10 Posted by: Adam0311 Posted at: 2016-02-11T22:41:02.414Z Reads: 246

```
Haven't experienced the Raptor yet (order #1935), so take my comments with a grain of salt, but I would rather find my own limits over time than have a board set limits for me (caveat, changing LV cutoff seems to make sense). I bought the raptor because it was more powerful and had more range. My only ask is that you ensure the Raptor and remote deliver a consistent experience, so I know what to expect and have the thrill of finding my limits.
```

---
## \#11 Posted by: onloop Posted at: 2016-02-11T22:51:13.725Z Reads: 240

```
I think you meant to say have the battery **cutoff start** set higher. Yes this make sense.

I simply never bothered to do it because I never road up hill when its near empty.... Like I said **STUPID MISTAKE.**

If the battery cuts out because of the BMS LVC when you are riding on flats or slight downhill there really is no problem, you no longer have power, you just start coasting...
```

---
## \#12 Posted by: thomwithah Posted at: 2016-02-11T22:56:16.339Z Reads: 243

```
@onloop Thank you for sharing the technical infomation. I hope to see more of that in this thread!! :stuck_out_tongue_winking_eye:


 [quote="onloop, post:7, topic:1319, full:true"]
ATTENTION ALL RAPTOR OWNERS

I am now offering you all a FREE 2 HOURS VESC programming support package

See here: http://vesc.net.au/support/

Please use this time to get some help re-programming your vesc with your own custom settings. He has a raptor so can help you de-tune it.

I'll pay @jacobbloy for the service he offers you. If you need more time with Jacob you can arrange to pay for that.
[/quote]

**This is truly amazing service!!!** It solidifies the positive feeling I have about your commitment to customer service, and my choice to give you my business. 

I hope users that taking advantage of this service share their results, settings, and general experience here.
------------------------------------------------------------------------
```

---
## \#13 Posted by: Adam0311 Posted at: 2016-02-11T22:57:52.208Z Reads: 230

```
Yes, thank you. Anyway, as a future Raptor owner I appreciate the efforts to make these boards great. I'll stop high jacking the thread now.
```

---
## \#14 Posted by: onloop Posted at: 2016-02-11T23:04:12.095Z Reads: 230

```
[quote="Adam0311, post:10, topic:1319"]
My only ask is that you ensure the Raptor and remote deliver a consistent experience
[/quote]

i have not had any issues with it.... i also ride with the lid on.
```

---
## \#15 Posted by: treenutter Posted at: 2016-02-12T01:12:39.881Z Reads: 251

```
This graph is interesting because it highlights one major difference between 18650's and Lipo... when the voltage sag begins! Below is a graph that @trbt555 posted in [this thread.][1]  Here it looks like the drop starts at 3.6v for Lipos.

<img src="/uploads/db1493/original/2X/4/4ae1a5aeb29650010294fff8d1c4b33989766883.PNG" width="690" height="449">

  [1]: http://www.electric-skateboard.builders/t/loaded-dervish-dual-r-spec-6355-dual-vesc-nunchuck-paris-195-90mm-flywheels/524/62
```

---
## \#16 Posted by: thomwithah Posted at: 2016-02-13T11:22:05.641Z Reads: 253

```
Well, I'm having issues making this appear as a quote from onloop, (I'm on my phone at the moment) perhaps a mod can fix it...

http://www.electric-skateboard.builders/t/enertion-raptor-first-batch-problems-solutions/1296/166?u=thomwithah

My instructions to reduce the aggressive low-speed power of the raptor.
=======================================================================

NOTE: please test with lid off first! This is to make sure your problem is not related to poor signal, if nothing changes with the lid off & the signal seems responsive its fair to assume you can get some results with the below instructions.

**1. Reduce motor current**. - See "Motor Max" change this to 40- To reduce the brake force, change "Motor min (regen)" - this is also rider weight dependent. Maybe try -10 or -20 to get it perfect you will need to use trial & error.
http://www.electric-skateboard.builders/uploads/db1493/original/2X/7/79fa0d046d167ac9416a6b3c198e9f3c895b7068.png



**2. Re-tune or customize the PPM settings**.- Adjust the "Soft RPM Limit" settings- Increase the Deadband

Watch this video too:

https://www.youtube.com/watch?v=OtuofrQr3F8
http://www.electric-skateboard.builders/uploads/db1493/optimized/2X/a/a43794d97445b47f38d09e5e17eb430128358b53_1_690x327.png

**3. Limit Top Speed using RPM limits**
You might also try setting the ERPM Limit Start at **20000** This will start limiting the Speed at around 10km... Could be a good idea until you get your bearings.
Otherwise maybe try these settings below... 
Its really up to you. You can tune this to meet your expectations.
```

---
## \#17 Posted by: thomwithah Posted at: 2016-02-13T11:36:04.533Z Reads: 237

```
http://www.electric-skateboard.builders/t/enertion-raptor-first-batch-problems-solutions/1296/167?u=thomwithah
```

---
## \#18 Posted by: thomwithah Posted at: 2016-02-13T11:38:30.960Z Reads: 227

```
http://www.electric-skateboard.builders/t/enertion-raptor-first-batch-problems-solutions/1296/168?u=thomwithah
```

---
## \#19 Posted by: thomwithah Posted at: 2016-02-13T11:39:50.071Z Reads: 229

```
http://www.electric-skateboard.builders/t/enertion-raptor-first-batch-problems-solutions/1296/170?u=thomwithah
```

---
## \#20 Posted by: thomwithah Posted at: 2016-02-13T11:40:09.890Z Reads: 231

```
http://www.electric-skateboard.builders/t/enertion-raptor-first-batch-problems-solutions/1296/171?u=thomwithah
```

---
## \#21 Posted by: Howser Posted at: 2016-02-13T18:43:32.464Z Reads: 219

```
i managed to get the drivers running and started bldc. i even managed to connect but it won't let me read out the configuration. also in the corner it says "connected, limited". someone seen this before?
```

---
## \#22 Posted by: Blasto Posted at: 2016-02-13T18:59:50.984Z Reads: 218

```
You need v1.14 of the bldc tool, it will match the fw version of your vesc



http://vesc.net.au/BLDC-TOOL/Windows/OLD%20Versions/

I don't recommend updating your fw for now, you can end up damaging your vesc or bricking it.
```

---
## \#23 Posted by: Howser Posted at: 2016-02-13T19:14:26.850Z Reads: 222

```
perfect, thank you it worked!
```

---
## \#24 Posted by: thomwithah Posted at: 2016-02-14T10:35:59.195Z Reads: 222

```
@Xusia have you gained any remote specific knowledge beyond the channel switching information posted by @onloop? I'm wondering in buttons A or B may be used for cruise control or if that function is limited to the C button (throttle).
```

---
## \#25 Posted by: Xusia Posted at: 2016-02-14T18:09:54.551Z Reads: 209

```
Hi Thom,

I would say I have gained some knowledge - about the VESC settings (and this definitely beyond the channel changing).  The settings you are referring to are remote specific and therefore *if* they are available would likely be found in the remote receiver firmware/software.

In my humble opinion, however, the buttons are good as is.  It's actually quite natural to just press down the stick when you get it where you want it.  Having to press "B" would mean holding the remote differently (for me, awkwardly), and what if you accidentally also pressed "A"?  Or just had your finger up there and pressed "A" long enough to turn it off?  Not a good idea as far as I'm concerned.

I posted my results in the First Batch Problems & Solutions thread, along with a couple videos.  I definitely recommend that anyone not 100% happy with the remote check out these settings and make appropriate adjustments.  Just changing the settings by .1 made a HUGE difference!

I'm happy to help you if you want.
```

---
## \#26 Posted by: Howser Posted at: 2016-02-15T00:00:55.028Z Reads: 197

```
i'm not sure what i'm talking about, i just watch a lot of videos. so if this is stupid please ignore it :)

has anyone tried fiddling around with FOC? like his: https://www.youtube.com/watch?v=bYYNbxPXNEU

it seem's it was the key to okayplayer's (esk8fr) "problems". he tried all sorts of setup's until he finally got the desired results with FOC: https://www.youtube.com/watch?v=HGdswPPROWs

here's another example how smooth it can be: https://www.youtube.com/watch?v=Uvelb52XICU

is this possible for the raptor dual or was there some info about this that i missed?
```

---
## \#27 Posted by: Howser Posted at: 2016-02-15T16:12:58.175Z Reads: 194

```
because of non stop rain i went to the close by tunnel to give the new settings a quick run.
i can now accelerate really smoothly! but now the motors turn off as soon as i'm over 1/4 throttle: https://drive.google.com/file/d/0BybdY5w-PsmIRFlscmlkNGNiOXM/view?usp=sharing (10 sec mark, battery above 90% charge)

i did not change the battery settings as suggested above.
i did however apply the settings @onloop posted about lowering aggressive low speed.

any idea which of the settings could have caused this? is it motor max which i changed from 80 to 40?

cheers
```

---
## \#28 Posted by: thomwithah Posted at: 2016-02-15T19:09:25.067Z Reads: 188

```
It looked like your LCD display died too, not just your motors. This seems like the low voltage cutoff is being hit, but I'm not sure. Were you going uphill at all? I'd think the new setting should make thisnless likely, not more. Have you tried it during a bench test and if so what's the result. I think you said your battery (like mine) wouldn't turn on. You had to charge it first, right? Maybe someone can tell if this is an after effect of that. Maybe the battery is week from a prolonged period of low, or under, charge. Maybe the weakness makes it morenpron to voltage sag, I don't know? Just a thought. Can anyone tell me if I'm a complete idiot for thinking any of this?
```

---
## \#29 Posted by: Howser Posted at: 2016-02-15T19:19:15.159Z Reads: 182

```
this was on a straight. same happens on the bench: https://drive.google.com/file/d/0BybdY5w-PsmIR3I1REtYZ1BDTkE/view?usp=sharing (on the bench i can't accelerate slowly, so it instantly cut off as soon as i hit the throttle)

battery has a funky switch which i have to press just right in order to hold, that is the problem. i don't think the cut off it battery related. i have to toggle the power off and on, kinda reboot, to start it again opposed to just turning on.
```

---
## \#30 Posted by: Xusia Posted at: 2016-02-15T19:22:22.660Z Reads: 171

```
I can't say for sure, because I just don't know enough about the battery electronics, but that sure looked like the LVC kicking in.  How charged was the battery?  Also, what was it flat or were you going uphill?
```

---
## \#31 Posted by: Howser Posted at: 2016-02-15T19:23:02.385Z Reads: 168

```
above 90% charge, flat, see my last post for video on bench please :blush: 
edit: i did charge he battery. until the green light appeared on the charger as suggested in onloops video.
also keep in mind that i didn't have this before i changed the settings. so the battery seems ok.
```

---
## \#32 Posted by: Xusia Posted at: 2016-02-15T19:27:47.170Z Reads: 164

```
Sorry - your post came in as I was typing mine.  I didn't see it.

Based on that, you have a defect somewhere.  My guess is the battery.  Do you have another ~37v battery lying around to test with?  Or another Raptor owner close by?
```

---
## \#33 Posted by: Howser Posted at: 2016-02-15T19:35:54.003Z Reads: 167

```
i will hopefully when thom is back and he still want's to do so :smile:

before i changed the values in the BLDC tool, i was one of those who reported he couldn't maintain lower speeds. i could however drive it without cut offs and it had the full torque.

now that i made the suggested changes, i have the problem with the cut offs.
do you think these two problems could be linked? or does this just show i'ts not the battery?
```

---
## \#34 Posted by: Xusia Posted at: 2016-02-15T19:50:26.114Z Reads: 167

```
Hmmm.  Not really sure, but based on that I think it's worth looking into.  If you care to hook it up to the BLDC tool again, can you tell me:
1.  The values of remote at full backward, neutral, and full forward (should be 3 values, each higher than the last)?
2.  The Min & Max Pulsewidth values, and the Deadband value?

Did you make any other changes?  Also, did you visit the the motor config page, and if so did you first READ the config, before clicking Write?  If not, you might have written some incorrect values.  Maybe take a screen shot of that page so I can compare to mine?
```

---
## \#35 Posted by: Howser Posted at: 2016-02-15T19:52:39.161Z Reads: 161

```
thank you i will provide these values (and screenshot) as soon as i have the board again tomorrow.
i did not make any other changes and i did read the config first before i changed anything
```

---
## \#36 Posted by: thomwithah Posted at: 2016-02-15T21:18:17.622Z Reads: 175

```
I'm definitely willing to do whatever I can. I've made arrangements to have my next Enertion package delivered (after I return from Sweden) Wednesday. I will only be in Switzerland 2 days before heading out to Dubai. I'll return on the 25th. You are welcome to my battery or anything else before then, but you'd need to come down. I won't have time to come up to you. Also, keep in mind my battery seems to have issues itself. 

On to the issue at hand though. I suppose it'd be easy enough for you to change back to your default "out of the box" settings, right? If so, give it a try and see if the apparent battery issue is still present. Had you ever opererated the board with the battery at 90%, or less, on the old settings? If not, it'd seem even more likely, to me, this is a battery issue that simply hadn't had the opportunity to show up until now. I don't see from what you mention how those settings should allow you to draw enough power quickly enough to hit the low voltage cutoff and not blow a fuse or something. I may be wrong, of course, I'm very far from an expert on the matter.

Maybe try seeing what it says the percentage is before it cuts off. Does it jump from 90% to 0% or does it hit levels in between. If levels in between maybe there is enough time to test something else. I'm curious if your able to "slam on the brakes" and send voltage back to the battery quickly and prevent the shutdown. Not sure what it would reveal if that was the case, but it's possible it might help diagnose the issue with someone more knowledgeable. In any case I don't understand how the motors could request enough energy on the bench to hit the low voltage cutoff of the battery when it's showing 90% charge on the LCD, regardless of the settings, without blowing a fuse. I mean, if a fuse serves a purpose it seem it should blow before then, right? Maybe the amps needed to blow the fuse aren't enough, but I thought pulling amps quickly during load is what caused the low voltage cutoff in the battery to hit. This of course was when th battery was low. At 90%, it's not low, right, so more amps drawn (quickly) before hitting the low voltage cutoff, no? 

Anyhow, it seems clear the issue is in the battery, to me. I just can't seen a 90% voltage reporting battery hitting the low voltage cutoff otherwise. I mean the VESC can't shut down the battery, right? Only the BMS can do that automatically, correct? Is there an instance where the BMS will shut down the battery while voltage shows capacity at nearly 90% other than hitting the low voltage cutoff? If not, are there any settings you could (incorrectly) put into the VESC to demand enough from the battery that it would hit the low voltage cutoff while reporting nearly 90% charged according to voltage? 

Hopefully someone knowledgeable comes in here and can clear it up for you soon. I'm really anxious to learn about this.
```

---
## \#37 Posted by: jacobbloy Posted at: 2016-02-16T08:33:42.893Z Reads: 171

```
If your LCD is turning off it this is wire into the battery before the vesc. this could mean a few things,
 your pulling more amps then the BMS is set for, or the voltage is to low and the LVC as kicked in and also if there are to high charging amps and the bms is trying to discharge the battery but can't do it fast enough so it will cut off the bms. 
If your BMS reaches its amp limit you have to charge your battery for 20mins to rest your BMS.
but you will know if this has happened because the lcd will not turn on at all.

i have found that the exertion 4A charger will continue to charge your board well after the lcd says 100%.
the 2a charger light will turn green but if i plug in the 4a charger it will continue to charge.

so you might want to keep the charger charging longer maybe 1 hour after the green light turns on.
the 2a charger should take 4 hours to charge your battery.

as for battery you can also damage or the bms if you bomb a hill and apply brakes while on a full charge.
```

---
## \#38 Posted by: Howser Posted at: 2016-02-16T09:42:56.005Z Reads: 170

```
Center stick: 1.554 - 1.560
Full Brake: 1.183 - 1.189
Full Throttle: 2.007 is the last number shown before the board turns off again

screenshot: https://drive.google.com/file/d/0BybdY5w-PsmIUnhkS0w0TXViUzg/view?usp=sharing
(i had motor max on 40 before i tried different values)

i will fully charge the battery once more now to see if the cut off still happens then
```

---
## \#39 Posted by: Howser Posted at: 2016-02-16T12:35:44.372Z Reads: 182

```
so i charged it up again to 100%. now the battery is not cutting off as early as before, but still does. it seems like it hits a certain threshold and shuts off. i made another video: https://drive.google.com/file/d/0BybdY5w-PsmIdERCUkplRnZTNWc/view?usp=sharing

you can see that i'm accelerating slowly, all of a sudden it cuts off, the battery counts down to 0%.
But right as i hit the brake it was booting again (normally i have to power off / on)
```

---
## \#40 Posted by: thomwithah Posted at: 2016-02-16T15:27:42.490Z Reads: 184

```
@Howser So it's cutting off now at 100% full even with the old settings, yet it didn't before making the changes?
```

---
## \#41 Posted by: Howser Posted at: 2016-02-16T15:36:02.806Z Reads: 176

```
yes battery is at 100% now.
original settings was 80 (only full speed), changed down to 40 (battery cuts off) i have since changed it to 60 (battery still cuts off)
will make another test with the original 80 but i don't think it matters.
```

---
## \#42 Posted by: Howser Posted at: 2016-02-16T15:55:55.790Z Reads: 178

```
just switched "motor max" back from 60 to 80 and it's not shutting off anymore on the desk at least. i will go for a test drive quick to see if i can still accelerate slowly

edit: test ride is over. still cuts off even with the default settings :( what's really weird is that the board now is completely controllable even with the default 80 settings opposed to always going full throttle like my first ride. i don't know what to think anymore.. it seems it cuts off when LCD shows a bit under 90%.. not sure though..

here is a video of todays attempt:

accelerate - power cut - brake - power gain - accelerate - power cut - dead
https://drive.google.com/file/d/0BybdY5w-PsmIMHZtMjdqeXEyZ1U/view?usp=sharing
```

---
## \#43 Posted by: thomwithah Posted at: 2016-02-16T16:12:37.505Z Reads: 169

```
So you're mnow back to default and it doesn't cutoff? What is your battery voltage or % now <90% or full? Let us know what happens at 90% with 80 motor max.

I have no idea what's happening.  Maybe @onloop can chime in now that more information is available.
```

---
## \#44 Posted by: Howser Posted at: 2016-02-16T16:22:10.461Z Reads: 162

```
check my edit please, my problem seems weirder then ever...
```

---
## \#45 Posted by: Xusia Posted at: 2016-02-17T03:13:54.588Z Reads: 171

```
@Howser, I have some suggested settings for you.

For the braking,I would change the Batt Regen Min from -20 to -40 or possibly -45.  Personally I found that -20 was just not enough.  Your experience may be different though.

As for the VESC settings, try these (not sure what your current values are, but I would save them).

Min Pulsewidth: 1.02
Max Pulsewidth:   2.1
Deadband:  0.15

Please let me know what you find.  I'm still learning.  :smile:
```

---
## \#46 Posted by: onloop Posted at: 2016-02-17T04:14:10.907Z Reads: 174

```
[quote="Xusia, post:45, topic:1319"]
Min Pulsewidth: 1.02
Max Pulsewidth:   2.1
Deadband:  0.15
[/quote]

Those settings are a bit different to what i got when doing more testing yesterday, on the particular remote i was testing Min 1.19 &  max 2.01 was working best, maybe everyones will be a little different. **Please, everyone! tune the settings if you haven't already done it.**

ALSO, Contacted the factory about the hand controller firmware to see if there is anything that needs tweaking there.

I spent a few hours yesterday doing more testing, also made some video, just not had time to upload. Tomorrow.

Was also getting inconsistent result using cruise control. Have notified Factory, maybe firmware can fix it.

But was easily able to do sustained, very slow speed laps around carp park 5mph or 10mph easily.. The throttle control feels really good. Brake seemed same as normal, strong & responsive.

Also, the GF lids are ordered. maybe dispatch in around 10days.still need confirmation.


**PLEASE EVERYONE > UPDATE THE SHEET WITH ANY PROBLEMS OTHERWISE YOU MAY GET MISSED> [HERE][1]**


  [1]: https://docs.google.com/spreadsheets/d/19Jd2938Xb_zMbXhBkOocz24FOrxj0mx5bQEV-HLOhw0/edit#gid=0
```

---
## \#47 Posted by: onloop Posted at: 2016-02-17T04:16:29.497Z Reads: 165

```
Hey,

Currently in talks now with battery factory discussing all these various issues. It was the first time we used the upgraded 50ABMS in space cell. Some of the weird issues may be related to that.

**PLEASE BE SURE TO LINK TO YOUR VIDEOS FROM THE FAULT SHEET.**
```

---
## \#48 Posted by: Xusia Posted at: 2016-02-17T04:24:31.610Z Reads: 165

```
Hey Jason, just curious (I'm working on a theory here):  On the remote where those settings worked well, was the "neutral" value approximately 1.6?  If not, what was it?
```

---
## \#49 Posted by: onloop Posted at: 2016-02-17T04:34:04.450Z Reads: 164

```
Not sure, will have to check later, 

what is the theory?
```

---
## \#50 Posted by: Xusia Posted at: 2016-02-17T05:21:50.290Z Reads: 160

```
I'm trying to develop a mathematical understanding of the relationship of the values that produce good results with the remote.  The theory is that the neutral value needs to be close to the 50% mark of the overall range.  With the numbers you provided, that would mean a neutral value of about 1.6.
```

---
## \#51 Posted by: trbt555 Posted at: 2016-02-17T06:57:07.563Z Reads: 166

```
The standard pulsewidths for all RC controlled gear using pwm or ppm is a pulse range from 1ms at full reverse to 2ms at full throttle forward.
1.5ms is regarded neutral, which is halfway. Always. Default setting on every hobby esc for car control.

Apparently, due to Chinese quality, the output of each controller varies slightly without possibility of trimming the signal like on a GT2B or other hobby transmitters.

By entering the lower and upper pulse widths measured from your controller into the VESC, you're allowing it to calculate what the halfway mark (ie neutral) should be.

But if your controller doesn't send the corresponding "halfway pulse" when the stick is in neutral, you need to start playing around with the high and low pulsewidth settings to find neutral, which will then affect you brakes and acceleration.
You cannot change how linear or non-linear the pulses correspond to the joystick input nor which response curve the VESC applies to that input.
That can only be changed in the controller and/or VESC firmware.

I've plotted the pulsewidth output from the controller against joystick position if anybody's interesed.
```

---
## \#52 Posted by: pierres Posted at: 2016-02-17T23:09:07.591Z Reads: 160

```
are you sure you do not loose the signal ? It may give random cut offs
does the weird cut offs happen when removing the lid or keeping the remote close to the receiver ?
For example when the remote is in my left hand (on the front) I observe random cut offs which i do not have when the remote is in my right hand, ie closer to the receiver ...
Just in case, you may already tried ?
```

---
## \#53 Posted by: Howser Posted at: 2016-02-17T23:38:29.394Z Reads: 155

```
i have considered that. but i also had signal losses, they are different. when the power cut happens you can actually see the LCD display of the battery counting down from 100% (or whatever the charge is) to 0% and stays at 0% until i off / on the battery again.
```

---
## \#54 Posted by: Xusia Posted at: 2016-02-18T00:21:48.817Z Reads: 153

```
I still say that sounds like voltage sag hitting the LVC, which would mean a battery problem.
```

---
## \#55 Posted by: thomwithah Posted at: 2016-02-19T00:24:21.074Z Reads: 160

```

My settings after calibration are very close to those that you by @onloop. 

Full Brake: 1.19 - 1.20
Full Throttle: 2.01

Center Stick seems to be about 46-47%, not 50%, does this effect me negatively in some way? I haven't noticed it if it has. On thing I notice is the display kinda sticks for a split second on ramp up to 100% there a few brief pauses with the most aggressive one being at about 71%. Anyone else notice such a thing?

@Xusia have you seen anything about what we might need to with a Raptor Dual and applying changes to the VESCs that might differ from a Raptor mono? Specifically, I'm wondering about the CAN Fwd options. Do all the recommended changes the the main VESC effect the slave too, so that nothing need be changed in regards to the slave alone?

My battery is dying under load when indicating 83% charge, or less. It seems to start to shut off when battery sag drops the displayed charge to about 73%. I can prevent shutdown of the battery by hitting the brakes and sending some current back into the battery. My battery also only shows 90% charge immediately after being removed from a charger with green LED. The battery's LCD goes out and the battery shuts off even without any load (other than the electronics) when simply left turned on and nothing else. Onloop has assured me I will be taken care of and this bad battery issue will be resolved in a way that I am VERY happy with. That said, can anyone tell me what I might try via the VESC to prevent hitting the apparently bad BMS and triggered LVC, or bad or disconnected cells, of my battery? It's only 7% or something, but I'd like to try and maximize the use of that 7% to get to know my Raptor better so for the time when I have a properly functioning battery. I don't mind the Raptor slowing (way) down (even always being slow) as long as I have brakes for as long as possible. I'm sure this could be managed via the VESC by someone knowledgeable. That's not me, yet. 

I'm only getting a about 3 fast, or 5-6 slow minutes of ridding before my battery dies due to an issue. In those brief moments, while testing throttle control after calibration I've been happier than I expected after reading through the forum here. I can ride quite slow if needed with small tweaks. My cruise will set at a slow speed and VERY slowly ramp up. I think with more research and VESC settings trials I will be completely happy with the control of the Raptor. I'm still tweaking the braking while getting used to it. Now it seems I need more time on the board to learn how to shift my weight to maintain traction and not lock and slide the wheels. I want to find the right settings to stop ASAP, sliding isn't doing that. It's nice to know I can lock it up, but that's not the fastest. At this point I think it's more about my lack of skill and experience on the Raptor than the settings needing tweaks. That said,  I'll share my settings when I find something I'm happy with. 

Unrelated, but I have to say I love the rush of jamming the throttle on the Raptor dual. It's a genuine thrill.  It's very nice to ride my Raptor even if it's for brief moments *for the time being*. It's tough not enjoying to it's full potential, but I know that will time come.  **@onloop, you've really made something special.** I don't know if anyone has had more problems than me, but I'd be surprised if they had from what I've seen. Still, with all that, I really *really* like this thing, and the way you've supported your customers. What I like most is the feeling that you will do your very best to make things right in the end. So far, I couldn't ask for more from you than you've already offered to meet those ends. **Thank You!**
```

---
## \#56 Posted by: onloop Posted at: 2016-02-19T01:38:23.381Z Reads: 151

```
[quote="thomwithah, post:55, topic:1319"]
I'm wondering about the CAN Fwd options. Do all the recommended changes the the main VESC effect the slave too, so that nothing need be changed in regards to the slave alone?
[/quote]

For now, I recommend mirroring all settings across both vesc. Even the PPM settings.

I am pretty sure that Dual VESC with CANBUS connection **doesn't** require the PPM settings to be changed on the slave, as the master is sending the same signal it is receiving, but it won't hurt so just do it.

ALSO, your battery is failing because its faulty, changing settings in the vesc won't resolve that.

I suppose if i had that battery here I would test the output voltage, that will tell you a lot. 
I am guess that one of the sense wires is not connected or one of the cells in a group has a problem, therefore the BMS is detecting a lower pack voltage and cutting off. 

If you feel like doing some battery surgery cut the black plastic off & remove all the parts so we can better see inside the battery, there is a chance it is one loose wire. You could be riding in a matter of minutes without a battery fault.
```

---
## \#57 Posted by: Xusia Posted at: 2016-02-19T06:26:07.703Z Reads: 149

```
[quote="thomwithah, post:55, topic:1319"]
Center Stick seems to be about 46-47%, not 50%, does this effect me negatively in some way? I haven't noticed it if it has. 
[/quote]

The thing I noticed when the neutral position was below about 48% is that the brake would sometimes activate when in the neutral position.  I had to lower the minimum pulsewidth value until the neutral position was at least 49% (I got better results on the braking when neutral was 50%).

[quote="thomwithah, post:55, topic:1319"]
@Xusia have you seen anything about what we might need to with a Raptor Dual and applying changes to the VESCs that might differ from a Raptor mono? Specifically, I'm wondering about the CAN Fwd options. Do all the recommended changes the the main VESC effect the slave too, so that nothing need be changed in regards to the slave alone?
[/quote]

From what I understand, you do not need to program the slave.
```

---
## \#58 Posted by: thomwithah Posted at: 2016-02-19T07:18:24.179Z Reads: 153

```
[quote="onloop, post:56, topic:1319"]
I recommend mirroring all settings across both vesc. Even the PPM settings.
[/quote]

Done, just for good measure, even though it isn't required. 

[quote="onloop, post:56, topic:1319"]
I would test the output voltage
[/quote]

I have a couple of multi-meters, can I test this effectively at the XT 60 connection or need it be done before the BMS, so to speak?

[quote="onloop, post:56, topic:1319"]
If you feel like doing some battery surgery
[/quote]

I'm happy to tear things apart to diagnose the issue. I'd like to know what's wrong so you may work with your factory to prevent future S.P.A.C.E cells from having the same issue. If I'm riding in a "matter of minutes without a faulty battery" that'd just be a bonus. That said, I'm not positive I'd have the tools or skill set to resolve the issue. If that's OK with you it's more than fine by me. I'd like a chance to try provided it doesn't limit my options, in terms of support, should I fail to resolve the problem. I'm guessing it wouldn't from your thus far outstanding  commitment to my satisfaction, but, as you know, I like to be clear.


----------


EDIIT: I just read:

[quote="thomwithah, post:58, topic:1319"]
future S.P.A.C.E cells
[/quote]

It sound's like a blurb from a science fiction book.... thought it was funny.
```

---
## \#59 Posted by: thomwithah Posted at: 2016-02-19T07:18:34.606Z Reads: 147

```
[quote="Xusia, post:57, topic:1319"]
I got better results on the braking when neutral was 50%
[/quote]

[quote="Xusia, post:57, topic:1319"]
From what I understand, you do not need to program the slave.
[/quote]

Good to know on both accounts. Thanks!
```

---
## \#60 Posted by: Dedbny Posted at: 2016-02-19T12:16:10.105Z Reads: 151

```
@onloop. Ive looked through your list of problems from users and it doesnt look that bad. Most items you can address which you are. With your permission I would like to try and adjust the Vesc for better speed control from what @xusia has tested. The next batch should run smoother.
```

---
## \#61 Posted by: onloop Posted at: 2016-02-19T22:42:03.856Z Reads: 148

```
I recommend changing the settings.
```

---
## \#62 Posted by: Dedbny Posted at: 2016-02-20T08:42:40.122Z Reads: 155

```
New settings dialed. On second run now second motor doesnt work properly it chatters,and doesnt spin properly at all, and Mini usb cant go back in vesc( tried @xusias mod usb) As the vesc is glued its very difficult to connect mini usb. The board is now only running on 1 motor. 

https://youtu.be/IW87K00qY3g

Hoping it can be rectified easily as its a tad frustrating. Both motors were working properly on bench and after an initial road test. But after second road test other motor not working properly now. 

Update. Working, but further testing required.
```

---
## \#63 Posted by: Khayman Posted at: 2016-06-12T20:44:36.643Z Reads: 127

```
Is the new and better settings already there when the raptor get shipped now or is it still the old settings?
Im a little bit worried that when im getting my board in a couple of months i wont be able to do it myself unless learning this stuff.
I feel like i dont have the time to do it but guessing i have to to get it working good?
```

---
## \#65 Posted by: Khayman Posted at: 2016-06-12T20:50:30.363Z Reads: 129

```
[quote="onloop, post:3, topic:1319"]
In fact I could try to emulate a "boosted boards" style profile... I test rode one for 3 hours yesterday.... it's much more beginner friendly, but boring after about 5 minutes.
[/quote]

Is probably good! if you are a pro you can change the settings and a beginner dont know how.
```

---
## \#66 Posted by: Dedbny Posted at: 2016-06-12T22:11:35.338Z Reads: 132

```
[quote="Khayman, post:63, topic:1319"]
r get shipped now or is it still the old settings?Im a little bit worried that when im getting my board in a couple of months i wont be able to do it myself unless learning this stuff.I feel like i dont have the time to do it but guessing i have to to get it working good?
[/quote]

Its likely you will need to make some Vesc changes just to get the controller adjusted with right limiter and any fine tuning you may want for personal preferences. Its my understanding the new settings should be fine now.

You have to remember this is a high performance board. It doesnt have settings to adjust from beginner to stig mode. Its controllable, so just take it to the speeds your comfortable with and take it slow from the start. You will be rewarded.
```

---
## \#67 Posted by: Khayman Posted at: 2016-06-12T23:20:26.938Z Reads: 136

```
Sounds great, thanks.
That gets my adrenaline running already! whant it now!!!
The kids can have my Blink board.
```

---
## \#68 Posted by: y.k Posted at: 2018-10-24T02:10:04.220Z Reads: 29

```
Hi.i have a 220kv 2200w alien power motor with a 8s lit ion battery pack and a Vesc. i wan to programmate my vesc. could you help me to fill in the parametrs in bldc tool program?
```

---
