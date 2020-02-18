# Vesc Max Amperage

### Replies: 46 Views: 8731

## \#1 Posted by: IsTalo Posted at: 2017-01-30T19:34:31.829Z Reads: 648

```
Hi, I bought a Vesc that is Arriving, But Since I bought I questioned my self "My motor can pull 80A and Vesc handle just 50A, Won't It Burn my vesc?" And I read that Vesc can handle 50A from the battery, but how many Amps it can delivery to the Motor?
```

---
## \#2 Posted by: OskarCastrone Posted at: 2017-01-30T19:52:02.114Z Reads: 646

```
I believe that the VESC can actually handle 60a - but I might be wrong.. 
You should definitely limit the current draw (max amperage) to around 40a. Just to be safe. 
How many volts is your battery supplying? What sice motor are you using, at what KV?
```

---
## \#3 Posted by: IsTalo Posted at: 2017-01-30T19:54:20.036Z Reads: 634

```
My Battery is 6s 6300Mah, and motor is a 300kv 1500w from Alien
```

---
## \#4 Posted by: OskarCastrone Posted at: 2017-01-30T19:59:38.065Z Reads: 628

```
Okay. That setup is not ideal for the VESC... It could possibly work out fine, but I think that there's a possibility of frying the VESC due to the low voltage battery (and therefore more amps is needed) and high KV motors. You will probably also lack power going up hill and when accelerating. You will get a high top speed though! 

You will probably need help from some of the experts in here. Just to be sure that you will not fry your ESC.
```

---
## \#5 Posted by: IsTalo Posted at: 2017-01-30T20:01:33.392Z Reads: 591

```
So what do I do now? I already bought it
```

---
## \#6 Posted by: OskarCastrone Posted at: 2017-01-30T20:05:08.282Z Reads: 582

```
You can probably make it work. 
Maybe these two can help you to configure your setting:
@Ackmaniac @laurnts.
It might take some time for them to answer though, so be patient :-)
```

---
## \#7 Posted by: IsTalo Posted at: 2017-01-30T20:18:39.702Z Reads: 569

```
Sure, I'll
```

---
## \#8 Posted by: Vieo Posted at: 2017-01-30T20:52:08.439Z Reads: 553

```
+1 Also interested - Same setup (6S 300KV)

[Alien 4260 Motor 300KV](http://alienpowersystem.com/shop/brushless-motors/alien-4260-outrunner-brushless-motor-300kv-1500w/)

[They also make a 100KV](http://alienpowersystem.com/shop/brushless-motors/alien-4260-outrunner-brushless-motor-100kv-1500w/)

Does VESC need sensored motor? (If not does it make a difference)
```

---
## \#9 Posted by: NickTheDude Posted at: 2017-01-30T21:13:11.511Z Reads: 538

```
Presumably if you use the same amp settings as a board running 10S you'd be fine, however you'd be making less power.
```

---
## \#10 Posted by: OskarCastrone Posted at: 2017-01-30T21:14:24.893Z Reads: 527

```
It is possible to use a sensored motor with the VESC. Many advise not to though... If you buy a motor with sensors then I would recommend to let them be unconnected.
```

---
## \#11 Posted by: OskarCastrone Posted at: 2017-01-30T21:15:30.319Z Reads: 511

```
Dont you think 40a is a good limit for the motor output?
```

---
## \#12 Posted by: NickTheDude Posted at: 2017-01-30T21:17:59.735Z Reads: 505

```
40a should be fine for motor amps but your battery amps is really what you need to worry about. I'd start around 20a and go up from there if you need to.
```

---
## \#13 Posted by: Ackmaniac Posted at: 2017-01-30T21:38:59.706Z Reads: 497

```
If your motor is rated to 80 amps then you can set this value at the VESC. 
If you have a Lipo battery you can also set the max amps to 50A. You could even try 60. 
Only problem with this high kv rating is that the motor will not deliver a lot of torque so it will overheat easily. But the VESC takes care about the temperature by itself. So if you don't loose power than it's fine. Also limit the max ERPM to 60000.
```

---
## \#14 Posted by: Hummie Posted at: 2017-01-30T21:44:54.874Z Reads: 491

```
the motor rating isn't likely legit and not a continuous rating, as that's likely what they're claiming that number is. 

you can set the motor and battery amp limit much higher as long as the motor doesn't overheat or the vesc doesn't shutdown from over temp you'd be fine.  

if you have a lipo it doesn't necessarily mean you can do 50 battery amps but assuming the battery is large enough or has a high enough c rating then the battery will be fine and the vesc will be fine too as long as it's not run forever at that output..otherwise temp shutdown

high kv doesn't  necessarily mean low torque or more heat and you can get the same performance (wattage and torque) from a high kv or low kv if fed the right ratio of amps to volts...higher kv needs more amps but the winding are thicker so makes the same heat...just use less voltage and it balances.
I've had 70/70 motor and bat amps and also ridden with 45/200. bat and motor amps and been fine.   the bat amp limit is what amps are really being pulled and the motor amp limit effects the ramping up of those amps at lower speeds generally and can be put all the way to 200 and it won't be pulling any more amps from the battery than whatever limit you set it to.   the real limit is just temp for the motor and vesc, the vesc will shut down with over temp and your motor will injure its magnets beyond some temp the magnets are rated for.
```

---
## \#15 Posted by: Vieo Posted at: 2017-01-30T21:52:46.155Z Reads: 446

```
I currently use 2x [ZIPPY Flightmax 3000mAh 3S1P 20C](https://hobbyking.com/en_us/zippy-flightmax-3000mah-3s1p-20c.html) to make a 6S pack.Would these be fine?



Does the VESC have a configuration for both Max Battery amps & Max Motor amps?
```

---
## \#16 Posted by: Hummie Posted at: 2017-01-30T21:53:55.862Z Reads: 435

```
ok but not ideal...bit low current ability probably.  and the voltage being low it will draw even more amps. 

there is a bat and motor amp limit yes.
```

---
## \#17 Posted by: Namasaki Posted at: 2017-01-30T22:17:39.555Z Reads: 433

```
300kv at 6s voltage is within the Vesc Erpm limit.
6x4.2=25.2v
25.2v X 300kv=7560 rpm
7560 x 7=52920 Erpm
The Vesc's Erpm limit is 60000
So you don't have to worry about causing a DRV fault in the vesc.
As mentioned, you may not have much torque.
If your not to heavy and your riding mostly on flat ground then you'll prob be ok.
Always give the board a couple push kicks to get it rolling before hitting the throttle.
```

---
## \#18 Posted by: Hummie Posted at: 2017-01-30T22:22:21.662Z Reads: 431

```
you can get as much torque you just need more amps.  especially with 6s this is a good scenario for the motor.  as long as the vesc doesn't get too hot you can up the bat amps and get the same performance as with a lower kv motor and as much torque
```

---
## \#19 Posted by: Namasaki Posted at: 2017-01-30T22:24:15.016Z Reads: 425

```
Your batteries are only capable of 60a 
3ah x 20c = 60a
If you draw 60a from the batteries the voltage will sag a lot.
With a 60a battery, you should prob set your batt max at 30a
```

---
## \#20 Posted by: IsTalo Posted at: 2017-01-30T22:29:24.824Z Reads: 415

```
Ah, okay, I'm 55kg and I live in Brazil, so no mountains
```

---
## \#21 Posted by: IsTalo Posted at: 2017-01-30T22:30:55.490Z Reads: 394

```
And with a 6,3Ah 35C battery?
```

---
## \#22 Posted by: Namasaki Posted at: 2017-01-30T22:37:08.472Z Reads: 390

```
55kg is not very heavy.
6.3 x 35=220a
That battery would be a much better choice.
Basically the higher the C rating, the better.
I personally use 5ah/60C batteries in a dual drive setup. I get very minimal voltage sag even when powering up hills.
I set my motor max at 60a and my battery max at 50a on both Vescs.
```

---
## \#23 Posted by: Vieo Posted at: 2017-01-30T22:41:58.026Z Reads: 381

```
I'm currently rocking a [Hobby King RC ESC](https://hobbyking.com/en_us/hobbykingr-tm-x-car-beast-series-esc-1-8-scale-120a.html) which was alright for prototype. But VESC upgrade sounds worth it.

I've been using 20C batteries for a while now... is this bad for them? I haven't hooked up a meter to the motor yet to see what actual amperage / voltage its runs at.

The motor states max amps of 50A, so I thought I was safe with 60A batteries.
```

---
## \#24 Posted by: Namasaki Posted at: 2017-01-30T22:45:53.666Z Reads: 371

```
a hobby esc works differently than a Vesc.
The hobby esc works in duty cycle mode.
So as you give more throttle the esc gives more voltage to the motors.
The current is determined by the amount of load on the motors.
A Vesc works in current control mode. So it always gives full voltage to the motors and the throttle controls the current flow or amps.
The Vesc is so much smoother in acceleration and braking than any hobby esc.
It is head and shoulders above any other esc out there.
```

---
## \#25 Posted by: Vieo Posted at: 2017-01-30T22:48:48.447Z Reads: 350

```
Ahhh thanks for explaining. Even more excited.

Even when my motor states max amp 50A I should upgrade my current 6S 20C 3000mAh (60A max) batteries. To a higher C rate?
```

---
## \#26 Posted by: Hummie Posted at: 2017-01-30T22:52:42.811Z Reads: 341

```
what the motor says on it is misleading and  It just does what it's fed and doesn't decide the power.   for protecting your batteries without the vesc to tell you whats going on you can feel if the batteries get warm after use or get a watt meter to see the acual amps pulled.  I'd assume half the c rating for lipos.  but if you're not pulling much with the 6s 20c and not getting them warm you're likely fine with those.
```

---
## \#27 Posted by: Vieo Posted at: 2017-01-30T23:15:47.104Z Reads: 339

```
Alright aces makes sense!


About eRPM 

> 300kv at 6s voltage is within the Vesc Erpm limit.
> 6x4.2=25.2v
> 25.2v X 300kv=7560 rpm
> **7560 x 7=52920 Erpm**
> The Vesc's Erpm limit is 60000

**eRPM = pole pairs * RPM**

Where's the **7** from? Do most motors have 7 pole pairs?
```

---
## \#28 Posted by: Hummie Posted at: 2017-01-30T23:22:58.725Z Reads: 323

```
typical out runners yes.  12 stator teeth and with 14 magnets theres the pole pairs.
```

---
## \#29 Posted by: Ackmaniac Posted at: 2017-01-30T23:40:14.607Z Reads: 328

```
[quote="Hummie, post:14, topic:16919"]
higher kv needs more amps but the winding are thicker so makes the same heat...just use less voltage and it balances.
[/quote]
That's not true. More amps result in more heat. And please don't go up to 200 amps. You would disable the Overcurrent protection of the vesc. 
First of all try the values your motor is rated for. If you don't like it you can change it anyway. 
And if you would use the 200 amps then you also need to use the watt control of my firmware mod.  Otherwise the motor will be nearly uncontrollable. (on or off). 
But at the beginning you should try low values to get a feeling for it. Seems that you are a beginner  so don't go creazy.
```

---
## \#30 Posted by: NickTheDude Posted at: 2017-01-31T00:40:53.826Z Reads: 322

```
Isn't it? I thought when you double kV resistance in the motor is halved but amps are doubled creating the same efficiency at % of no load RPM. Vedder wrote a thing about it. http://vedder.se/2014/10/chosing-the-right-bldc-motor-and-battery-setup-for-an-electric-skateboard/
```

---
## \#31 Posted by: devin Posted at: 2017-01-31T00:43:47.612Z Reads: 311

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#32 Posted by: Ackmaniac Posted at: 2017-01-31T01:07:17.522Z Reads: 300

```
@IsTalo thanks to Devin everything should be a no-brainer for you now.
```

---
## \#34 Posted by: PXSS Posted at: 2017-01-31T01:30:35.149Z Reads: 295

```
Take things that @devin says with a grain of salt and DO NOT run your motor at 5000W. It's stupid, you will only get yourself hurt or set your board on fire (not mutually exclusive). 

He posts suggestions about settings that can really hurt a person but has never tried them himself.
```

---
## \#35 Posted by: devin Posted at: 2017-01-31T01:32:04.300Z Reads: 289

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#37 Posted by: TarzanHBK Posted at: 2017-01-31T07:35:00.384Z Reads: 280

```
aaaaand there we go again with devin :D

<img src="/uploads/db1493/original/3X/0/0/008be4e9526d9abe998c3d15ec2646952f661815.jpg" width="400" height="400">

(not that we´re against science and stuff but maaaaaaaaaan!)
```

---
## \#38 Posted by: devin Posted at: 2017-01-31T14:00:28.012Z Reads: 267

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#39 Posted by: lox897 Posted at: 2017-02-01T04:51:07.373Z Reads: 259

```
@devin same calculations, all over the forum. 1/100 of people give a flying fuck. Stop spamming, I beg you. Leave it to your own thread.

No offence, it's just pissing everyone off.
```

---
## \#40 Posted by: JohnnyMeduse Posted at: 2017-02-01T04:53:36.851Z Reads: 261

```
[quote="lox897, post:39, topic:16919"]
flying fuck
[/quote]

<img src="/uploads/db1493/original/3X/1/8/18229e4117017364a896fb3091da5bebe550b516.jpeg" width="251" height="201">
```

---
## \#41 Posted by: lox897 Posted at: 2017-02-01T04:54:15.471Z Reads: 249

```
TRIPLE LIKED
10 characters
```

---
## \#42 Posted by: devin Posted at: 2017-02-01T05:02:45.685Z Reads: 248

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#43 Posted by: JohnnyMeduse Posted at: 2017-02-01T05:04:32.956Z Reads: 242

```
<img src="/uploads/db1493/original/3X/e/f/efb2a8f18b66362a7a23f0ca171a454551f01930.jpeg" width="263" height="192">
```

---
## \#44 Posted by: meesie Posted at: 2018-05-08T21:43:53.561Z Reads: 147

```
Can’t we like.... IP ban devin? He’s killed this thread and many others.

Now i’m also confused about battery amps and motor amps. In the vesc settings i got 80A max amps for the motor and 60A for the battery. Can anyone explain as to why this is? Anyone except Devin that is...
```

---
## \#45 Posted by: Ackmaniac Posted at: 2018-05-08T22:34:12.206Z Reads: 146

```
For motor max you can set the maximum the Motor or the VESC can handle.
Nobody knows how much the motor can handle because you need to stress the motor until it fails to find out. The manufacture rates the motor for maximum constant current. And for him that means you put a propellor on the motor and use it in a rc airplane. So it has like a forced wind cooling.
But we have only the wind from driving which isn't the optimum for the motor. But get rid of the illusion that you pull the motor max amps constantly. If you have a street steup and no extreme steep hills you won't stress the motor with that many amps for more than a couple of seconds. And before you overheat the motor you will overheat the VESC if you have no active cooling.

But as long as you don't go uphill for a couple of minutes at a very steep incline you won't really fry them.
Just simply test that by touching the motors after you think you stressed them really hard. If you still can touch them for a couple of seconds without burning your skin you have nothing to be worried about. If you put a drop of water on them and it boils (> 100°C) you should rethink your setup. If you still can touch them they are below 60°C.

Next problem can be the amps the motor starts to saturate. Means there is a point where the motor can't transfer more amps into more power. That means all the extra amps will be transferred to heat. For motors which are at least 6355 in size that shouldn't happen below 100A. 
Next problem is how much can the VESC handle. For newer versions like FOCBOX, VESC6 a.s.o. 80A for Motor max shouldn't cause any issues. Everything above needs to be tested and depends on the length of the battery and phase wires (shorter is better) and your motor mode (BLDC, FOC).
For VESC of the old age (standard 4.12 like Maytech) that might already be a bit much.
Some go 120A and some even higher but you can get Overcurrent Errors. So it should be tested and i can't recommend it if you are not sure what you are doing.

Battery max is the max the Battery can handle. 
If your Battery can deliver 80A and you have one VESC then you can use 80A Battery max in theory. But practically that is a lot of power for one VESC (e.g. 10S4P at 36V * 80A = 2880W). If you have dual drive the Battery amps need to be split by 2. So 40A each in this case. Which is better handable for the VESC. 
But of course you also need to reduce that if you have fuses, a BMS or a anti spark switch that can't handle that much. So you can take the Amps of the weakest link in your system and devide it by the amount of motors. That is the maximum you should set your battery max.

But that doesn't mean you have to set the value that high. If it is too much power for you can use lower values.
Simple rule is.
If you want to adjust the _power_ at **Low and Mid Speed** you need to adjust the Motor Max
If you want to adjust the _power_ at **High Speed** you need to adjust the Battery Max
If you want to adjust the _brake power_ at **Low and Mid Speed** you need to adjust the Motor Min
If you want to adjust the _brake power_ at **High Speed** you need to adjust the Battery Min

(I used the word _power_ which stands for torque, acceleration, strength, force, momentum or whatever you want to call it that you feel when the motors trys to move your weak flesh)
```

---
## \#46 Posted by: meesie Posted at: 2018-05-09T08:05:14.605Z Reads: 133

```
That last bit you wrote was super informative! Thanks!! 

Though the only thing i still don’t understand is how can the motor current be higher than the battery current. I’m no electrical engineer so my logic would be “the battery outputs 20A so the motor uses 20A”

Here you can see that the motor current is higher than batt current.
![image|690x252](upload://h1WXExFZ9dmLK8Rpd93XM6CopSk.jpeg)

Could you explain why this is?
```

---
## \#47 Posted by: professor_shartsis Posted at: 2018-05-09T13:08:04.697Z Reads: 127

```
[quote="meesie, post:46, topic:16919"]
Though the only thing i still don’t understand is how can the motor current be higher than the battery current. I’m no electrical engineer so my logic would be “the battery outputs 20A so the motor uses 20A”

Here you can see that the motor current is higher than batt current.
[/quote]

[quote="professor_shartsis, post:20, topic:49277"]
an esc works by a similar principle to a dc to dc buck converter in continuous mode which can also lower the effective voltage while increasing the amps. **the battery is periodically connected and then disconnected from the winding at a frequency on the order of 25khz. During the times the winding is disconnected from the battery, the winding is shorted to itself which allows the current generated during the brief on times to continue circulating during the off times.** since the current continues to flow in the winding during the off times, the “motor amps” are numerically higher than the “battery amps.” the battery may see 10a @ 50v, 10% of the time which averages to 1a, while the motor effectively sees 10a @ 5v the entire time. In reality the current rises in the motor from, say, 9.5a to 10.5a during the 10% on times, then decays from 10.5a to 9.5a during the off times.
[/quote]

the motor current is higher than the battery current because the motor current continues to inductively circulate during the very brief duty cycle “off” times while the battery is supplying 0a. (during these duty cycle “off” times, the motor winding forms a continuous circuit through the vesc via a different set of mosfets). this process lowers the “effective voltage” of the battery pack, and this lowered effective voltage is sent to the motor to produce the # of motor amps requested by the user’s throttle.

http://engineeronadisk.com/V2/notes_labs/engineeronadisk-335.gif

http://engineeronadisk.com/V2/notes_labs/engineeronadisk-91.html

https://upload.wikimedia.org/wikipedia/commons/thumb/5/52/Buck_operating.svg/600px-Buck_operating.svg.png

In the following chart, the “motor amps” are labelled “I av” (average current):

https://upload.wikimedia.org/wikipedia/commons/6/63/Buck_chronogram.png

https://en.wikipedia.org/wiki/Buck_converter
```

---
## \#48 Posted by: meesie Posted at: 2018-05-09T14:34:18.682Z Reads: 113

```
I see. It’s still a little bit abracadabra for me but at least i now vaguely understand why it is. Thanks!
```

---
