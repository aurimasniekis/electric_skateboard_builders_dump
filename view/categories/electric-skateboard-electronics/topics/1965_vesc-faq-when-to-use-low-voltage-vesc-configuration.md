# VESC FAQ &#124; When to use low voltage - VESC Configuration

### Replies: 40 Views: 9888

## \#1 Posted by: chaka Posted at: 2016-03-24T22:53:38.825Z Reads: 788

```
I see many people fret about using a low voltage power supply to configure their VESC. This is a good idea but it is not always necessary. 

The only time I would say it is absolutely necessary is when powering up a VESC for the very first time, if you buy them from me you can count on this already being done. Sometimes a solder bridge will not be seen on the first visual inspection and you can fry a vesc if you attempt to spool up at higher voltages. Also if you are attempting to power an unusual motor that is not normally used, better to use caution and use low voltage. 

Well sir.... what low voltage supply should I use?

Lab power supplies will often have trouble or induce unknown variables so I recommend a basic 12v lead acid battery. Nothing fancy, you can get one delivered for less than $10.  Again, if you buy one of my VESC's this is not necessary unless you are using unorthodox motors.

 I have run motor detection at 12s without issue on a 192kv motor. This brings up another point... motor KV and system voltage. Before running config divide 8600rpm by your system voltage. If the resulting number is lower than the KV of the motor you are going to use than your KV is to high and you need to get another motor or lower your voltage.

A 192kv motor is the absolute max you should use at 12s.   

 8600rpm/44.4v = 193.69KV

If you attempted to spool up a higher kv motor at 12s it could cause faults and return a bad detection. Same goes for lower voltages but with higher KV motors. Take 10s for instance. 8600rpm/37v = 232.43kv    So we can see 230kv is the max kv we should use at 10s.
```

---
## \#2 Posted by: mohammedex Posted at: 2016-03-24T23:35:16.304Z Reads: 681

```
Useful thread!
It should also be possible to power up the VESC for the first time with a 3s lipo battery right?
I would happily get myself a 12v lead acid battery if needed, but I do have quite a few 3s lipos at hand. This probably goes for quite a few people.
```

---
## \#3 Posted by: chaka Posted at: 2016-03-25T00:22:29.785Z Reads: 627

```
Thats a tricky question. Chances are those lipos are capable of some really high amps in comparison to a little 12v lead acid battery. Small lead acid batteries are not capable of high discharge currents while a lipo might give a fault all the current it needs to do some damage. Maybe I worry too much?

Edit: After giving this some thought I came to the realization that i have never breached 5 amps on my power supply when running detection at 12v.. even with a faulty VESC. A 3s lipo should be fine.
```

---
## \#4 Posted by: claudiofiore88 Posted at: 2016-03-25T00:46:17.117Z Reads: 573

```
I have a 12 volt 4 amp brick power supply that I got from a credit card terminal. I'm think of using it, or would that be problematic?
```

---
## \#5 Posted by: NNGG Posted at: 2016-03-25T02:33:13.537Z Reads: 543

```
How about a 7 volt nimh ?
```

---
## \#6 Posted by: claudiofiore88 Posted at: 2016-03-25T02:42:45.293Z Reads: 519

```
I have a few nimh packs as well.
```

---
## \#7 Posted by: chaka Posted at: 2016-03-25T04:40:45.666Z Reads: 509

```
@claudiofiore88  That should work but you will probably pop it if you try to reverse rotation at max rpm. Most of the time you can reset it by unplugging/plugging the power supply with the vesc disconnected. Using a SLA eliminates this nuisance when calibrating transmitters etc... again this is only necessary on a fresh untested VESC or when running an experimental or questionable motor. 

@NNGG The VESC version 4.12 and under currently has a minimum voltage requirement of 8v. 

Honestly, if you have an untested VESC your best bet is to look over the drv8302 legs in detail with a 10x jewelers loupe before running motor detection. I never test without first going over the entire board with 5x and legs with 10x magnification. 

Most failures are actually due to uninsulated phase wires and bad connections. I personally have never killed a vesc. It is not for lack of trying but I mind my wires and I always look for things that might be wearing through cables or coming loose. I also use a bms so no more battery connection mishaps. 

Don't rush it, take your time and inspect everything before making your final connections and make sure everything will not come loose when you go for that first ride. Haste has killed more VESC's than we will ever know.
```

---
## \#8 Posted by: Hummie Posted at: 2016-03-25T05:05:09.582Z Reads: 457

```
   

So if I have an 80kv motor I can run the vesc at 100 volts comfortably since 8600/100= 86!!!!

That's insane. I mean that's awesome.

But I'm too afraid something will arc 


In your math you just can go with the nominal voltage?  12s fully charged is 50 volts and 8600/50 = 172kv max
```

---
## \#9 Posted by: onloop Posted at: 2016-03-25T06:44:38.043Z Reads: 442

```
[quote="Hummie, post:8, topic:1965"]
I can run the vesc at 100 volts
[/quote]

No you can't, the components on board are rated up to max 60V. Staying at 50V or less is the recommendation.
```

---
## \#10 Posted by: onloop Posted at: 2016-03-25T06:47:28.935Z Reads: 424

```
@chaka its great to see you contributing with an informative VESC article! the community appreciates it.

NOTE: I added FAQ to the title so it appears for that search query
```

---
## \#11 Posted by: akira Posted at: 2016-03-25T07:51:25.980Z Reads: 414

```
Thanks for this informative post !

Isn't it safer to use a lab power supply with current limitation for the first times you power up your VESC ?
An battery of 12V has no current limitation and can deliver quite a big load in comparison.

Can you also elaborate a bit more on this statement ?
"Lab power supplies will often have trouble or induce unknown variables"
```

---
## \#12 Posted by: chaka Posted at: 2016-03-25T13:52:53.964Z Reads: 407

```
@akira You are correct but.... three of my customers have killed vesc's using lab power supplies. I don't know if they reversed polarity, uploaded the wrong firmware or some other cause. It leaves a lot of questions and not many people have lab power supplies or know how to use them either. A thorough inspection paired with a low voltage power source has given me 100% success rate when testing fresh VESC's. The main saving grace of using low voltage is that the motor will spool up softly compared to higher voltage. It is much less aggressive.

One little detail I did not mention earlier. Use the arrow keys to check the VESC before running detection. Just give it a quick tap. If everything sounds fine give it another longer burst and make sure it spools up before detecting parameters. If something is wrong it will let you know with either a drv8302 fault or jerky operation.

@Hummie using a nominal cell voltage for the max kv calculation is fine. In real world use, the pack will be under considerable load at max rpm and have considerable voltage sag unless it is an extremely large pack. 192kv @ 12s has proven to work without faults. 

There really isn't many reasons to go higher than 12s on a skateboard. 12s at 80 amps will give you 3500 watts. 80 amps being the limit "for me" when using 10awg cable. 3500 watts should propel a person to about 45 to 50 mph on a skateboard. If you use higher voltage you also need to use special cables and take some extra precautions like warning labels etc. Everything gets a lot more expensive too. Maybe someday when we have a fully fledged racing circuit will see systems like this in the open class but I would still caution against it for the average street rider.
```

---
## \#13 Posted by: treenutter Posted at: 2016-05-08T03:19:02.618Z Reads: 357

```
[quote="chaka, post:1, topic:1965"]
Before running config divide 8600rpm by your system voltage. If the resulting number is lower than the KV of the motor you are going to use than your KV is to high and you need to get another motor or lower your voltage.
[/quote]


@chaka is there any margin of error in this calculation? I was going to run a 245KV motor at 10s but the calc suggests that 232KV would be the max KV recommended.
```

---
## \#14 Posted by: Bender Posted at: 2016-05-08T10:14:46.843Z Reads: 357

```
[quote="chaka, post:1, topic:1965"]
I have run motor detection at 12s without issue on a 192kv motor. This brings up another point... motor KV and system voltage. Before running config divide 8600rpm by your system voltage. If the resulting number is lower than the KV of the motor you are going to use than your KV is to high and you need to get another motor or lower your voltage.

A 192kv motor is the absolute max you should use at 12s.   

 8600rpm/44.4v = 193.69KV

If you attempted to spool up a higher kv motor at 12s it could cause faults and return a bad detection. Same goes for lower voltages but with higher KV motors. Take 10s for instance. 8600rpm/37v = 232.43kv    So we can see 230kv is the max kv we should use at 10s.
[/quote]

My understanding is that the VESC can limit the voltage and rotation
So would it be possible to use a 12s pack with a 230kv
If you limited one or both?
```

---
## \#15 Posted by: chaka Posted at: 2016-05-08T14:05:46.148Z Reads: 332

```
You could but it may throw some fault codes if you spool up the motor on the bench.

@treenutter 245kv works on 10s. 

The 8600 rpm is the point when our motors start to loss efficiency.

The vesc has a max erpm of 100000. If you breach that you will throw a fault and maybe cause some damage so you should be limiting your erpm.
```

---
## \#16 Posted by: treenutter Posted at: 2016-05-08T14:32:56.547Z Reads: 331

```
Many thanks @chaka! It's really helpful for me to understand the rationale behind the calculation.  I always limit erpm to around 40-50k, just to keep top speed aligned with my personal speed tolerance (this gets me to about 24mph top).
```

---
## \#17 Posted by: Hummie Posted at: 2016-05-08T14:56:13.925Z Reads: 322

```
Am I wrong but I remember someone saying that you may run a voltage and kv motor that keeps you under the 8600 limit on the bench, but if you get outside going down a hill/mountain and were to brake you'll end up beyond the rpm limit and have a fault?  That sounds like disaster.
```

---
## \#18 Posted by: 3sly Posted at: 2016-05-23T14:47:05.355Z Reads: 310

```
I have a question though: does the voltage used for your config and motor detection have to reflect the voltage that will later be used.

e.g.: I'm using a 149kV motor with a 12s lipo. But I'd like to run the config from 8s lipo (esk8.de recommends 16V 5A minimul for motor detection), will it still do a correct motor detection at 8s?

Thanks in advance, Dries
```

---
## \#19 Posted by: fraannk Posted at: 2016-05-24T16:46:50.132Z Reads: 302

```
I would like to know if a 20 (maybe 24) volt 2A lab supply would be sufficient for a SK3 168kv motor detection run? :)
```

---
## \#20 Posted by: NNGG Posted at: 2016-05-24T21:07:48.409Z Reads: 295

```
its more than enough. I use a 3S lipo
```

---
## \#21 Posted by: chaka Posted at: 2016-05-24T21:08:48.472Z Reads: 272

```
Yeah, anything over 8 volts should be fine.
```

---
## \#22 Posted by: fraannk Posted at: 2016-05-24T22:44:57.610Z Reads: 264

```
So the VESC will detect the motor fine with only 2A? :) Doesn't the motor pull more than that
```

---
## \#23 Posted by: chaka Posted at: 2016-05-24T22:46:57.019Z Reads: 265

```
Not usually. You want to be sure the motor is not under any load during detection.
```

---
## \#24 Posted by: fraannk Posted at: 2016-05-24T22:48:10.919Z Reads: 260

```
Okay, thanks a lot guys
```

---
## \#25 Posted by: chaka Posted at: 2016-05-24T23:00:30.688Z Reads: 255

```
The power supply might shut off if you hit the brakes during transmitter configuration so keep that in mind if you lose power during setup. Usually you will need to unplug the PS from the wall and plug it back in to get it to reset if this happens.
```

---
## \#26 Posted by: zmoney Posted at: 2016-05-29T21:23:29.240Z Reads: 249

```
okay so im reading all about VESC's and how to config them. Im buying mine from [Diy's](product/vesc-the-best-electric-skateboard-esc/) with pre installed software. Do i need to power it up with a lower voltage? or can i just wire everything and just plug in the usb to my pc? thanks
```

---
## \#27 Posted by: chaka Posted at: 2016-05-29T23:00:37.288Z Reads: 249

```
I would ask dexter about that. I am not sure what kind of testing he does on his units. Always a good idea to run low voltage for testing anyway. Much less aggressive than running detection at higher voltage.
```

---
## \#28 Posted by: ThinkChink Posted at: 2016-09-05T10:54:05.698Z Reads: 209

```
@chaka Hi, I'm new to this thing. Was wondering for the first time when powering up my VESC, you recommended a 12v basic lead acid battery. I currently have a 12v 45ah lead acid battery and I was wondering if it's too much to do a first-time power up? The box writes 45A continuous discharge, and if any further info helps, it's a Sebang SMF NX100-S6S. Also, would a 4s 8000mah 15c lipo stick do the trick as well?
```

---
## \#29 Posted by: chaka Posted at: 2016-09-05T15:09:21.687Z Reads: 212

```
I have actually been rethinking this. If your VESC is questionable you can use a pair of 9v alkaline cells in series and you will be much safer. 
<img src="/uploads/db1493/original/2X/6/6ec562c6f32683bead3a67af4a360fe1dadfbb72.jpg" width="690" height="388">
```

---
## \#30 Posted by: nmagz3 Posted at: 2016-12-09T08:28:49.133Z Reads: 156

```
@chaka thanks for taking the time to spell this out for everyone.  I've really walked away with a wealth of knowledge that will save me some pain when detecting my motor for the first time.  Anyhow, I'll be building receiving my VESC in the next coming weeks and I wanted to confirm with you that the 9v in series would be safe for first power up of the VESC.   Thanks again for the awesome post :sunglasses:
```

---
## \#31 Posted by: chaka Posted at: 2016-12-09T13:56:54.477Z Reads: 154

```
It is enough to power it but they dont push enough amps to run motor detection. 

If you purchase a vesc from us you don't need to worry about using full system voltage on the first go. We load test every VESC we build.
```

---
## \#32 Posted by: nmagz3 Posted at: 2016-12-09T14:51:13.408Z Reads: 156

```
Thank you sir!
```

---
## \#33 Posted by: laikiux Posted at: 2016-12-23T15:30:09.905Z Reads: 146

```
Hello,
I bought 4.12 Vesc from enertion. I have 10s battery. Can I connect my battery with Vesc for the first time?
```

---
## \#34 Posted by: zmoney Posted at: 2016-12-23T15:33:27.696Z Reads: 143

```
If you don't have any other low voltage supply, you might be able to get away with it. Just make sure you visually inspect you VESC for any solder bridges and anything of the like. Also, make sure you double and triple check you BLDC tool configurations before running anything..
```

---
## \#35 Posted by: themegak Posted at: 2016-12-23T17:12:52.742Z Reads: 144

```
yes, that low voltage thing doesn't apply to any modern vesc that already has firmware installed.  This is a very popular misconception.  You will be fine.  Just make sure you have right VESC settings when setting up your particular motor and run the detections required prior to riding.
```

---
## \#36 Posted by: DevinG Posted at: 2018-04-16T21:06:21.231Z Reads: 53

```
hey guys just got my foc in the mail today, im intending on running 6s lipos in series to power a 260kv motor. i dont want to kill this thing, im reading the walk through thread now but could use some help and advice in getting to my first ride thanks ! also  would like to run foc mode :smiley:
```

---
## \#37 Posted by: zepton Posted at: 2018-04-27T16:39:34.857Z Reads: 52

```
I have been riding my board on 6S with my Enertion Vesc for a long time. I recently upgraded my batteries to 9S and when I plugged in the batteries on the bench the vesc blinked red and I got a DRV8302 fault. 

When I rebooted and plugged in my 6S batteries the vesc performed fine as if nothing happened. Can anyone help with this? Are there any specific settings I need to change to support 9S? I don’t want to break my $100 Vesc.
```

---
## \#38 Posted by: TarzanHBK Posted at: 2018-05-14T18:51:31.559Z Reads: 42

```
If you put your Input Voltage too low, you wont be able to use higher batteries with the old settings.
Pls post Screenshots
```

---
## \#40 Posted by: zepton Posted at: 2018-05-15T14:40:38.786Z Reads: 37

```
On a different forum:

https://www.electric-skateboard.builders/t/vesc-drv8302-failures-and-repair-options/4201/168?u=zepton
```

---
## \#41 Posted by: TarzanHBK Posted at: 2018-05-17T10:40:20.531Z Reads: 33

```
Did you upload fresh Firmware and tried again?
```

---
