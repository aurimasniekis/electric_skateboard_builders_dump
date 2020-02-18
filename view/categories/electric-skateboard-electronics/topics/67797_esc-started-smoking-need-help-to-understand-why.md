# ESC started smoking, need help to understand why!

### Replies: 34 Views: 891

## \#1 Posted by: Mau Posted at: 2018-09-12T10:52:01.330Z Reads: 171

```
I have this ESC (https://m.banggood.com/it/FVT-CBWI120A-ESC-Brushless-Speed-Controller-For-110-and-18Series-RC-Cars-Skateboard-ESC-p-985970.html?cur_warehouse=CN) that did an annoying and loud beeping sound on startup. Because the sound is made by the motor my idea was to disconnect the motor for the first few seconds of the startup and then connect it again.

So I disconnect the first cable from the motor and then switch the board on, but the motor still beeps. So I disconnect another cable from the motor and this time I hear a spark from the point where one of the power cable is connected to the switch. To avoid other problems I reconnect the two cables and switch the board on (this is now the usual setup) but, even if the ESC turns on, when it should starts beeping it somehow "restarts" (there was maybe a short circuit). 

Now I think that maybe the switch has been damaged, so I remove it and switch the board on directly connecting one of the power cables to the battery (something I did also when my previous switch was broken), and at this point the ESC starts smoking from the inside. 

I later opened the ESC and noticed that one of the internal capacitors (there's also an external one) was disconnected (not welded anymore), as well as some burning marks. 

My questions:
-what the heck happened to the ESC? It has worked just fine so far
-is it possible that the main cause is giving power to the ESC without it being completely connected to the motor? 
-is any of my actions the cause of the failure? 
-the capacitor disconnected because of the heat that caused the smoke or its disconnection is the cause of the failure?
-should I buy the same esc again? (I don't think so)

Any suggestion will be greatly appreciated; thank you in advance! :upside_down_face:
```

---
## \#2 Posted by: Taquel Posted at: 2018-09-12T11:15:19.497Z Reads: 153

```
Well, probably the power button was broken, but now you fried the esc by connecting it to the battery directly.
```

---
## \#3 Posted by: Mau Posted at: 2018-09-12T11:34:41.417Z Reads: 144

```
Actually the switch still works, and I don't think I've fried the esc by connecting it directly to the battery as it's something I had done previously (and there's no difference in connecting the esc to the battery with a switch or with a connector). 
Do you think the problem was powering the esc with it being only partially connected to the motor? Or the fault is only of a crappy esc?
```

---
## \#4 Posted by: ElectricCoast Posted at: 2018-09-12T11:44:34.776Z Reads: 128

```
A spark from plugging it in could have fried it.  That's why I always use Xt90S connectors with the antispark capability.
```

---
## \#5 Posted by: slick Posted at: 2018-09-12T13:04:59.638Z Reads: 117

```
[quote="Mau, post:1, topic:67797"]
So I disconnect another cable from the motor and this time I hear a spark
[/quote]
 could it be that the two disconnected leads accidentally touched each other causing the spark while you turned your ESC on? 

[quote="Mau, post:1, topic:67797"]
the ESC starts smoking from the inside
[/quote]
...mhhhh magic smoke. probably the aftermath of the big spark?

sounds like you accidentally shorted the disconnected leads when powering up. i´m no engineer so i cannot give you any other explanations. The ESC vibrates the motor to produce the accoustic signal you described - thats "normal" - i used a car ESC on my first build...it used to annoy me too...

Capacitors are also sensitive to over-voltage...mabe the voltage was more than the capacitors could handle? (could be an underrated capacitor that finally quit)

[quote="Mau, post:1, topic:67797"]
should I buy the same esc again? (I don’t think so)
[/quote]
nope. save a few more bucks and get a VESC.  (no, I´m not affiliated to any seller :smile:)
```

---
## \#6 Posted by: Mau Posted at: 2018-09-12T14:32:11.717Z Reads: 88

```
[quote="slick, post:5, topic:67797"]
could it be that the two disconnected leads accidentally touched each other causing the spark while you turned your ESC on?
[/quote]

Don't think so, but can't be sure about that.

[quote="slick, post:5, topic:67797"]
Capacitors are also sensitive to over-voltage…mabe the voltage was more than the capacitors could handle? 
[/quote]

The voltage should have been normal; my ipothesis is that the capacitor disconnected for some reason and that caused the esc to fail. 

[quote="slick, post:5, topic:67797"]
nope. save a few more bucks and get a VESC
[/quote]

Thank you for your suggestion. What is the main difference between an esc and a vesc? Do you suggest any specific one?
```

---
## \#7 Posted by: Mau Posted at: 2018-09-12T14:32:45.415Z Reads: 75

```
Thank you, I'll consider using thos connectors in the future.
```

---
## \#8 Posted by: Sn4pz Posted at: 2018-09-12T14:35:39.565Z Reads: 78

```
if youre looking for a good cheap vesc ive been seeing good reviews for the flipsky 50a ones, or even the dual if you have 2 motors

otherwise you could get a pair of focboxes, get a thermal case for them and youll probably have more power than you will ever want
```

---
## \#9 Posted by: slick Posted at: 2018-09-12T18:41:53.200Z Reads: 70

```
i can only recommend the hobbyking VESC since its the only one i used so far. so far it has been doing its job well until a capacitor failed (pins broke off) due to occuring vibrations. easy repair...no problem

a VESC has good acceleration curves , good brakes and regenerative braking. its really the better option compared to a car ESC. another plus is if you want to increase voltage,you can go up to 10S - 12S (though 12S is maybe hard at the limits and you risk frying your VESC).
```

---
## \#10 Posted by: Mau Posted at: 2018-09-12T19:02:08.712Z Reads: 69

```
Thank you very much!
Are you talking about this one? https://hobbyking.com/it_it/turnigy-sk8-esc-v4-12-for-electric-skateboard-conversion-w-bec.html
```

---
## \#11 Posted by: slick Posted at: 2018-09-13T12:31:00.639Z Reads: 60

```
yes that one.
```

---
## \#12 Posted by: PXSS Posted at: 2018-09-13T16:22:19.045Z Reads: 58

```
[quote="ElectricCoast, post:4, topic:67797"]
A spark from plugging it in could have fried it.
[/quote]
Nope. The biggest danger with that spark is wearing out the connector. This will never burn out an ESC. 

@Mau 
Reasons it may have blown:
Faulty ESC. You could have had a faulty capacitor in your ESC that just went out as you plugged it directly into the battery. 

Shorting motor. The more likely scenario is that you somehow shorted the motor wires when you turned the ESC on without the motor plugged in. 
You should have never done this. Most ESCs need to see the motor to go through their proper boot up and syncing. Taking one or two leads out essentially tells the esc theres a faulty motor and it can fail catastrophically if the ESC doesn't expect it or know what to do with the condition. 

The issue definitely did not come from connecting the battery directly to the esc. Not how things work
```

---
## \#13 Posted by: dareno Posted at: 2018-09-14T03:52:01.960Z Reads: 50

```
[quote="Mau, post:1, topic:67797"]
that did an annoying and loud beeping sound on startup.
[/quote]

Not sure that the beeping is the motor dude.  Car esc's beep on boot up to let you know they're on.  
They all do it.  Its normal.  The beeps usually let you know if there is an issue.  It beeps to tell you the amount of cells connected.  If it doesn't beep properly you have a problem. Read the manual.
```

---
## \#14 Posted by: Mau Posted at: 2018-09-14T19:02:23.722Z Reads: 45

```
Thank you. I'm gonna buy a better esc and, most importantly, never try this again!
```

---
## \#15 Posted by: Mau Posted at: 2018-09-14T19:03:47.982Z Reads: 44

```
The beeping was absolutely normal, and I could feel it was made by the motor (because of the signals sent from the esc) by touching it. I just didn't want it to beep.
```

---
## \#16 Posted by: evoheyax Posted at: 2018-09-14T20:17:24.806Z Reads: 46

```
@Mau Yes, please just buy a vesc 6.x. The biggest issue I had with this esc in particular (I've used multiple of them, the 150a one is much better) is the settings are terrible. Instead of being able to limit current to a finite number, you have settings like low, medium, and high, with no way of knowing what real world numbers those correlate to. So it's easy to over work these little guys and blow them up. I also had these 120a guys smoke and blow up. The second one I used made my motor smoke and overheat too. It's nightmare not being able to do some simple math to set it up correctly and instead, rely on trial and error, with error meaning time to buy another esc.
```

---
## \#17 Posted by: b264 Posted at: 2018-09-14T20:20:23.739Z Reads: 47

```
[quote="Sn4pz, post:8, topic:67797"]
if youre looking for a good cheap vesc
[/quote]

"good" and "cheap" are mutually-exclusive.  You pick one or the other.  Your choice.
```

---
## \#18 Posted by: b264 Posted at: 2018-09-14T20:21:55.783Z Reads: 50

```
[quote="dareno, post:13, topic:67797"]
Not sure that the beeping is the motor dude
[/quote]

I've never used this ESC before but my suspicion is that the beeping is coming from the motor, because it might be doing some sort of motor autodetection on bootup, and the rotor might be making that noise as the ESC is probing the windings to measure resistance, inductance, et cetera
```

---
## \#19 Posted by: Mau Posted at: 2018-09-14T20:31:53.879Z Reads: 46

```
Thanks for your reply, do you think that the hobbyking vesc is a good choice? (https://hobbyking.com/it_it/turnigy-sk8-esc-v4-12-for-electric-skateboard-conversion-w-bec.html)
```

---
## \#20 Posted by: Sn4pz Posted at: 2018-09-14T20:34:38.464Z Reads: 48

```
fine fine, "good, for being cheap" would have been a better way to phrase it
```

---
## \#21 Posted by: evoheyax Posted at: 2018-09-14T20:58:04.413Z Reads: 45

```
Just get in on hummies group but for the 6.6 fesc. It’s a little over $100 and will do much better. It’s basically the vesc 6.6. The 4.12 have design flaws and I don’t know why people still buy them. They will likely break over and over and over again. Some people get lucky or don’t run foc with these 4.12s and they work. But foc, and more power than you know what to do with is what you’ll gain. More power than you need means your not running everything to it’s edge of breaking, which should mean longer life also.
```

---
## \#22 Posted by: dareno Posted at: 2018-09-15T02:02:51.440Z Reads: 42

```
This has never happened to me in esk8 or rc applications.  So not like an audible alarm sound but a high frequency vibration noise?  What i do know though is most car esc's have an alarm sounder on boot and to indicate the  programming settings.Thanks for that info because when it inevitably happens to me I will now know.
```

---
## \#23 Posted by: Mau Posted at: 2018-09-15T07:42:13.499Z Reads: 50

```
Do you suggest any specific ones (providing link if possible)?
```

---
## \#24 Posted by: evoheyax Posted at: 2018-09-15T16:13:00.992Z Reads: 43

```
If you want a bullet proof ESC, buy the official VESC 6 from Trampa for an arm and a leg:
http://www.trampaboards.com/1x-vesc-6-in-cnc-t6-silicone-sealed-aluminium-box-with-genuine-xt90-connectors--vedder-electronic-speed-controller-trampa-special-p-24333.html

If you want a cheaper alternative, the fesc 6.6 (based on the vesc 6) can be purchased from Flipsky (the manufacturer) here:
https://flipsky.net/collections/electronic-products/products/fsesc6-6-simplify-version-with-aluminum-heatsink

Or there's this group buy which saves you a bit more (not sure if it's too late though):
https://www.electric-skateboard.builders/t/flipsky-groupbuy-again-120-including-usa-shipping-with-tracking/65563

Other wise, there's the focbox at a bit higher price:
https://www.enertionboards.com/electric-skateboard-parts/FOCBOX-programmable-brushless-motor-controller/

Any of these options are much better than any hobby grade ESC or VESC 4.12 (besides chaka's VESC 4.12's because he figured out how to fix the flaws, but he doesn't sell them to the public anymore).

Flipsky also offers them in a full alum case with a nice led power switch and another with out the case and an led power switch. If you buy one any of the other ones, you should use an xt-90 anti spark switch to turn it off and on.
```

---
## \#25 Posted by: Mau Posted at: 2018-09-15T16:30:16.939Z Reads: 34

```
Thank you! I really appreciate it!
```

---
## \#26 Posted by: b264 Posted at: 2018-09-15T19:47:37.317Z Reads: 34

```
[quote="dareno, post:22, topic:67797, full:true"]
This has never happened to me in esk8 or rc applications. So not like an audible alarm sound but a high frequency vibration noise? What i do know though is most car esc’s have an alarm sounder on boot and to indicate the programming settings.Thanks for that info because when it inevitably happens to me I will now know.
[/quote]

I don't know, I'm guessing
```

---
## \#27 Posted by: dareno Posted at: 2018-09-15T19:52:31.409Z Reads: 32

```
You guess?!?!  Never?!  now I'm not sure if the suns going come up.:thinking:
```

---
## \#28 Posted by: Multi Posted at: 2018-09-15T20:19:24.186Z Reads: 30

```
there are good and cheap things, like japanese cars. cheaper and definetely more reliable than a ferrari.
```

---
## \#29 Posted by: dareno Posted at: 2018-09-15T20:26:05.459Z Reads: 28

```
[quote="evoheyax, post:24, topic:67797"]
If you want a bullet proof ESC, buy the official VESC 6 from Trampa for an arm and a leg:
[/quote]

thats both arms and both legs and your first born child.
```

---
## \#30 Posted by: dareno Posted at: 2018-09-15T20:31:34.500Z Reads: 27

```
Sadly that is generally not the case in esk8.
```

---
## \#31 Posted by: evoheyax Posted at: 2018-09-15T21:00:15.356Z Reads: 28

```
Here’s the problem. We are not 4 lb drones, we are 100-300lb people. We put huge strains for long periods of time and the esc tech for us is very new. Can you make the fvt esc wok? Yes you can. I used the fvt 150 for months every day without issue. But the performance with a a vesc is night and day. Not just more powerful but smoother. And you can protect other components like your motor and battery from damage. With the fvt and other hobby grade escs, you can’t protect anything and you will break something else in time. The vesc allows to you protect your motor from overheating and the battery from under discharging. It protects the esc from pulling too much current and blows it up. A lot can go wrong on electric skateboards. Ride a diy board for 3 years and you’ll see, even with 4.12 vescs. Buy quiality or buy twice the choice is really yours. But you will buy it twice, I promise.
```

---
## \#32 Posted by: evoheyax Posted at: 2018-09-15T21:01:32.859Z Reads: 27

```
[quote="dareno, post:29, topic:67797"]
thats both arms and both legs and your first born child.
[/quote]

Which is why I don’t own any haha. But Derek was a big dude that used them and he told me they were the first ones he wasn’t able to break, so that says a lot to me about their quality (assembly and design).
```

---
## \#33 Posted by: b264 Posted at: 2018-09-16T03:09:17.170Z Reads: 19

```
[quote="evoheyax, post:31, topic:67797"]
A lot can go wrong on electric skateboards.
[/quote]

Biggest understatement of the year award goes to ... @evoheyax 

You will soon realize reliability is the only thing that matters in the end ;-)

... because an electric skateboard of any kind is better than a broken electric skateboard.
```

---
## \#34 Posted by: Bobby Posted at: 2018-09-16T03:18:03.570Z Reads: 19

```
“Esc started smoking, need help to understand why”

Honestly i think its stress. Focbox unity is coming for its job, The motors just wont give it a break and not to mention how it gets all hot headed. Just needed something to take the ease off maaaaannnn ✌🏼
```

---
