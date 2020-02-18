# Understanding current limits on VESC motor settings

### Replies: 23 Views: 7379

## \#1 Posted by: Eboosted Posted at: 2017-09-30T23:36:10.237Z Reads: 616

```
I have a dual 6374 190KV runing on 12S, the board is a real beast, it's my favorite board out of my 4 builds, I'd like to understand more about these current limits, so I'm shotting a couple of questions for you experts.

Why does increasing motor max from 60A to 70A yields to better performance even though I left battery max at 40A?

If 40A is the maximum current output my battery I wonder how I felt such a huge increase in torque?

If I increase motor max to 80A or even 100A I heard the motor might not hold it, why would that happen if the current is still being restricted by the battery limit?
```

---
## \#2 Posted by: rich Posted at: 2017-10-01T03:35:44.419Z Reads: 604

```
That topic was confusing me for months, too :joy:
I've read a proper explanation for this by an electrician but due lack of knowledge I can't repat it (post a link if I find it again). But the amps pulled by the motor are always higher than the amps pulled by battery. You can see that in many ride logs which people post. Often the battery amps are 50%-60% of the motor amps. That's the reason why you get more power with higher motor max settings even with battery max at 40A. But you should not exceed the max amp rating of your motors, otherwise they get too hot or gonna die.
```

---
## \#3 Posted by: chewydinosaurs Posted at: 2017-10-01T04:40:22.339Z Reads: 596

```
How far does one thing a motor can exceed the amp limit set for it? Just wondering since my amp limit is 60A and I need a little more torque haha. And since it's getting rather cold where I live, I'm sure the outside air will keep the motor fairly cooled off
```

---
## \#4 Posted by: Eboosted Posted at: 2017-10-01T04:48:06.116Z Reads: 577

```
The @torqueboards 6374 motors are rated for 3150w, if I make the math on 12S at a nominal voltage of 3.7*12=44.4V, the maximum current should be 3150/44.7=70.94A so my setting at 70A for motor max should be perfect.

Now I wonder what happens inside a motor when too much current is flowing through it? What is the part that fails when  it starts to get hot?

I had some 6355s magnets falling apart, could that be something a high current breaks?
```

---
## \#5 Posted by: Namasaki Posted at: 2017-10-01T04:58:52.621Z Reads: 561

```
TB motors are rated for 80a so set your Motor max amps to 80a and you should  be fine.
I run my AP motors at 80a with batt max at 50a on 10s voltage.
I tried turning them up to 90a but noticed they where running higher temp at that setting.
You should check your motors after running them to make sure they are not overheating.

<img src="/uploads/db1493/original/3X/7/8/78e48f91eb7eb1121d042d43af61600c669599db.png" width="576" height="500">
```

---
## \#6 Posted by: Namasaki Posted at: 2017-10-01T05:02:28.798Z Reads: 511

```
[quote="Eboosted, post:4, topic:34425"]
I had some 6355s magnets falling apart, could that be something a high current breaks?
[/quote]


excessive heat might cause that or rocks getting in your motors and getting stuck between the magnets and stator.
could have been defective glue maybe.
```

---
## \#7 Posted by: rich Posted at: 2017-10-01T05:05:45.702Z Reads: 501

```
[quote="Eboosted, post:4, topic:34425"]
Now I wonder what happens inside a motor when too much current is flowing through it? What is the part that fails when  it starts to get hot?
[/quote]


I don't know but also waiting for someone to explain it :grin:
```

---
## \#8 Posted by: Namasaki Posted at: 2017-10-01T05:10:31.803Z Reads: 489

```
I had a discussion with @Hummie a while ago about this. Maybe he can chime in and give you a better explanation.
He convinced me to try running higher motor max and it has worked out very well for me.
```

---
## \#9 Posted by: Jebe Posted at: 2017-10-01T05:13:41.797Z Reads: 483

```
info on the vedder forums
http://vedder.se/forums/viewtopic.php?t=883
```

---
## \#10 Posted by: BigBoyToys Posted at: 2017-10-01T05:19:23.956Z Reads: 482

```
Not recommending you surpass manufactures ratings, but since you are asking about limits I figured Id share that I do on all my builds. Below are my current settings. I suppose some of my setups could overheat if they were pushed uphill for long periods of time but I keep their limitations in mind and havent damaged any of them due to overheating. The Maytech, TB's and Carvon v3's have temp sensors though so I dont worry about them much. 

Raising current too high can saturate the motor amd cause rapid heating and other issues including vesc failure if the vesc loses sync due to the breakdown of the magnetic fields at high currents. Also, magnets fall off/ potentially demagnetize, stator coil lamination burns off causing a short and bearings seem to lose all their lube once overheated.
Per each motor and esc:
1. Maytech 6364's at 50A battery/100A motor.  
2. Carvon 2wd V2's 40A battery 100A motor
3. Carvon 4wd V2's 37.5A battery/110A motor
4. TB V2 hubs 37.5A battery/130A motor
4. Carvon V3's 30A battery/80A motor.
```

---
## \#11 Posted by: Eboosted Posted at: 2017-10-01T07:18:01.805Z Reads: 452

```
When should you consider it is in fact overheating? Hot to the touch, not being able to hold the motor for more than 2 seconds or wait for the VESC temperature limit to kick in? 

100A seems to be pretty high for a 6374 with 3150W, but if the difference is substantial, I'm willing to risk my motors, on the other side, if the increase on torque is barely noticeable as the motor limit keeps on being exceeded, then I'll stay within the limits of the motor rating. I guess this is something I'll have to test myself. Can't wait for the VESC tool update to be able to communicate through the hm-10 Bluetooth module to change VESC settings on the fly. 

I'm still wondering how can more current be produced while the battery limit is set to 40A, yes I know motor current always read higher on any datalog. I guess it's stored on some kind of buffer between the battery and motor and it just flows as soon as the throttle is pressed. Does it make any sense?
```

---
## \#12 Posted by: Eboosted Posted at: 2017-10-01T07:21:13.780Z Reads: 427

```
[quote="Namasaki, post:5, topic:34425"]
I run my AP motors at 80a with batt max at 50a on 10s voltage.
[/quote]

What cells do you have on your build? Can your battery produce more than 80A constant, 40A for each VESC? Are you feeling a noticeable performance difference between runing battery max 40A vs 50A?
```

---
## \#13 Posted by: BigBoyToys Posted at: 2017-10-01T08:23:52.142Z Reads: 417

```
I left the vesc motor temp settings at 80C I think its a pretty safe max temp. For the most part, torque and power equal heat. After riding and hitting the back off a few times Ive gotton a pretty good idea of how hard I push my various set ups begore they will hit the nack off temp. Before the vesc tool I had to roll around with a IR temp gun to accomish this.

To be honest, if you are running the motor temp control on the vesc tool I dont think you have to worry about the motors as much as u do your VESC's. 

Increases in motor amp settings are very noticeable. Try and see 😉
```

---
## \#14 Posted by: Namasaki Posted at: 2017-10-01T09:36:38.598Z Reads: 399

```
I'm using Lipos five 2s 5ah 60C packs in series
My bms is rated for 80a continuous but can handle up to 200a peaks
I have run my battery max at 60a per vesc without any problems.
I turned it back down to 50a just to be conservative.
I'm pretty sure though that my battery never sees 80a or 100a draw even going up hills.
My gearing is pretty low 15/40 with 90mm wheels. Lower gearing seems to be most efficient.
But turning up the batt max seems to improve the power band even though I'm not reaching the max.
Just as turning up the motor max improves torque even though I'm not reaching that max either
```

---
## \#15 Posted by: trampa Posted at: 2017-10-01T10:50:31.491Z Reads: 377

```
Hi Eboosted, any VESC based ESC can alter the current and voltage. If your battery has 44.4V and you set battery max to 10A that equals 440W output from the battery. 

At 50% duty cycle the VESC would run your motor at 22.2V and could push 20A which equals 440W again. Still the current flowing out of the battery would only be 10A.

Setting higher motor amps than battery amps only helps in situation where the throttle is lower than 100%. At max throttle the lowest of both values (motor max/battery max) is the limiting factor.

Going slow up a hill would be a situation where a higher motor amp setting helps. Downside is a non linear power along the throttle range.

Frank
```

---
## \#16 Posted by: PXSS Posted at: 2017-10-01T12:10:31.805Z Reads: 357

```
@Eboosted look up any of the threads @devin had created. He has the math in there. Essentially, ESCs are constantly switching on and off. The faster you go the more on time you get. So at full speed you power is dictated by your battery, 43.2v x 40a = 1728W. At 10% of full speed you get the ESC switching on 10% of the time. This means to get the same power output than at full speed, you would need: 4.32v x 400a = 1728W. Thats where the motor limit comes in, your battery can provide the power but you'd more than likely burn your motor fast. If your motor limit is 80A then you will get:
4.32v x 80A = 345.6W from motor
43.2v x 8A = 345.5W from your battery

The torque produced is close to 1/kv * current, so you can see how the motor limit really is what matters at low speeds when talking about torque. 

---
 The issue you run into with pushing too much current is in this order:

Demagnetized motor: the component with the lowest temp rating in a motor are usually the magnets. A demagnetized motor will have a different kv value. 

Magnets falling: if the epoxy holding the magnets in place gets too hot, it can fail. This is more of an issue with cheaper motors. I've never seen it happen. 

Enamel coating on copper wires burning off: if you even get close to this point, toss the motor. Its gone. The enamel coating doesn't burn until 300c so if your motor got this hot. You probably have a board on fire.
```

---
## \#17 Posted by: pshaw Posted at: 2017-10-05T03:15:22.582Z Reads: 328

```
[quote="BigBoyToys, post:10, topic:34425, full:true"]
Not recommending you surpass manufactures ratings, but since you are asking about limits I figured Id share that I do on all my builds. Below are my current settings. I suppose some of my setups could overheat if they were pushed uphill for long periods of time but I keep their limitations in mind and havent damaged any of them due to overheating. The Maytech, TB's and Carvon v3's have temp sensors though so I dont worry about them much. 

Raising current too high can saturate the motor amd cause rapid heating and other issues including vesc failure if the vesc loses sync due to the breakdown of the magnetic fields at high currents. Also, magnets fall off/ potentially demagnetize, stator coil lamination burns off causing a short and bearings seem to lose all their lube once overheated.
Per each motor and esc:
1. Maytech 6364's at 50A battery/100A motor.  
2. Carvon 2wd V2's 40A battery 100A motor
3. Carvon 4wd V2's 37.5A battery/110A motor
4. TB V2 hubs 37.5A battery/130A motor
4. Carvon V3's 30A battery/80A motor.
[/quote]

Wow 100A motor on the dual 6374!?! What battery are you running on this board? Also wheelsize and gearing?
```

---
## \#18 Posted by: BigBoyToys Posted at: 2017-10-05T03:20:43.738Z Reads: 317

```
Its actually a dual 6364 so even smaller. I have had these settiing on my trampa with 200mm pneumatics 15-66 gearing and a 10S8P battery for months now. This thing eats belt teeth for breakfast lol.  I run 100-130A motor on most of my builds haha.
```

---
## \#19 Posted by: pshaw Posted at: 2017-10-05T03:21:49.878Z Reads: 315

```
[quote="BigBoyToys, post:18, topic:34425, full:true"]
Its actually a dual 6364 so even smaller. I have had these settiing on my trampa with 200mm pneumatics 15-66 gearing and a 10S8P battery for months now. This thing eats belt teeth for breakfast lol.  I run 100-130A motor on most of my builds haha.
[/quote]

ah there we go. I'm running 97mm w/ 16t/40t street config. Think I would kill the motors instantly? :p
```

---
## \#20 Posted by: BigBoyToys Posted at: 2017-10-05T03:37:31.858Z Reads: 313

```
How about my 1:1 ratio 90mm hubs pushing 130A motor?
```

---
## \#21 Posted by: pshaw Posted at: 2017-10-05T03:48:23.083Z Reads: 302

```
[quote="BigBoyToys, post:20, topic:34425, full:true"]
How about my 1:1 ratio 90mm hubs pushing 130A motor?
[/quote]

heh yeah i'd assume that's a bit taxing lol
```

---
## \#22 Posted by: BigBoyToys Posted at: 2017-10-05T03:57:00.027Z Reads: 303

```
High amps are much more likely to kill Vescs  than motors from my experience. 6374 motors are great heatsinks ;).  Give it a try?
```

---
## \#23 Posted by: Deckoz Posted at: 2017-10-05T04:12:44.482Z Reads: 303

```
The answer to your question is duty cycle.

On my build I have 1300watts per motor.

Let's say I have a charged battery 42v and starting from a stand still the duty ramps to 35%

35% duty of 42v is 14.7volts. So at 42v & 35% duty the motor is operating at 14.7v. Well 14.7v in order to produce 1300 watts, it would take 88 motor amps.

That 1300 watts at 100% duty(42v) is only 30 battery amps...

The answer to your question is duty cycle.

In case that didn't make sense these two produce the same power/torque
100% duty
1300w/(42v * 1)= 30.95A

35% duty
1300w/(42 * .35)= 88.43A

What's that mean? It means your motor needs more amps with lower duty during the duty ramp to produce a linear amount(relative/same) of torque throughout the powerband/throttle.

Another thing motors rated for amps and voltage need to be calculated for watts. 12s 80 amps is 4032watts. Let's take this as its certainly outside of the vescs capabilities. But to get the full watts at 35% duty would require a max motor amp of 232amps... Vesc can't do this. So by setting 80 as the max motor amps when it reaches 80 amps it forces the duty to step up(V) reducing the ampers until duty cannot ramp any further.
```

---
