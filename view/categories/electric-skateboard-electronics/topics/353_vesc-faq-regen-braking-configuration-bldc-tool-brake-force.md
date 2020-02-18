# VESC FAQ &#124; Regen Braking Configuration BLDC tool &amp; Brake Force

### Replies: 56 Views: 23831

## \#1 Posted by: onloop Posted at: 2015-10-24T03:35:25.380Z Reads: 1719

```
**If you didn't already know the VESC has built-in regenerative braking it can charge your battery when braking.** 

*I also thought It would be appropriate to explain exactly what that is & how regen braking works, Then I realised I actually don't fully understand the technical principles of how it actually works, Maybe Someone else can explain in detail how the Back EMF is used as a brake force, how it is created & controlled.*

Anyway, This is my simple explanation as I understand it: The ESC stops outputting power from the battery into the motor, Instead the motor now turns from momentum as it rolls along the ground, it basically turns into a little generator. It starts generating its own current, known as Back EMF (back electromotive force) which is sent back into the battery just like a battery charger does.

> For some interesting analysis on how much this technology can actually charge your battery read [this article][1] written by Justin from Grin Technologies. 


----------



**So now to the actual purpose of this thread**

In this thread I will explain how to set up Regen in the BLDC tool. How to configure the brake to make it perform the way you want it, Stronger or Softer braking force. More charge current less charge current.

**Open the BLDC tool / Motor Configuration TAB / Motor TAB**

<img src="/uploads/db1493/original/1X/0de83856ce50a4aba05110644ad92c131a040819.png" width="690" height="439">

**These are the two parameters you need to change to make changes to the regen. "Motor Min (regen)" & "Batt min (regen)"**
<img src="/uploads/db1493/original/1X/014ba149924b9d9332e3658ca01480d9bc6a325c.png" width="539" height="217">

Displayed above is the default settings, these settings work great! The brake force feels really nice, it's strong but not too strong so you get launched from the esk8.

One thing that confused me a little was the negative values & the wording of the parameters, specifically the "min" part.

For instance if you are using the SPACE Cell and want to maximise the lifespan of the battery and only charge within manufacturer's rated max charge current of 4000ma (per cell) you may want to have a max charging current of just 12 amps (the space cell is 10S3P. 3 parallel groups X 4a Max Charge Current = 12A Charge current). So you would change the "Batt min (regen)" to -12

Motor min (regen) this is how much current you want inside the motor when using regen braking. If your motor has a rating from the manufacturer saying is is good for 40 amps you should then set this parameter to -40.

**So how do these two parameters work together to control the feeling of the brake, the real life braking force you will feel when riding?**

As I said before the default settings are great as they are, progressive controlled braking force that brings you to stop in a safe manner. But if you do change the parameters to meet manufacturer's guidelines what happens?

**Batt min (regen):** If lowered, say to -12 from the default of -20 will reduce the force of the brake (most noticeable at higher speed). If increased above -20 will strengthen the brake force (most noticeable at high speed). Also it will charge your battery more.

**Motor min (regen):** if lowered from the default of -60 will reduce the force of the brake (at low speed brake force will not be changed much) if increased greater than -60 you get stronger brake force, also you might get much hotter motor if you do lots of braking at high speed.


Hopefully now you have a better understanding of how the brake settings work in the VESC and you can tune it to suit your electronics and your riding style.

  [1]: https://endless-sphere.com/forums/viewtopic.php?f=2&t=7891
```

---
## \#2 Posted by: yendi Posted at: 2015-10-24T05:50:30.424Z Reads: 1385

```
If I understand you correclty it would work like this for my batteries:
I have 3x4S 5000mAh 20C
So I should be able to put 20x5 = 100Amps --> -100 in batterie min (charge)
For my motor I have Torque's 2x 5065 170KV 2200W but I can't find any specs for them in terms of Amps.
```

---
## \#3 Posted by: onloop Posted at: 2015-10-24T06:07:07.282Z Reads: 1322

```
20C is your discharge rate. 

Most lipo's however should be charged at 1C 

If you have a 10000mah lipo you can charge safely at 10AH.

Some people say you can charge at 2C without damaging lipo.
```

---
## \#4 Posted by: yendi Posted at: 2015-10-24T06:15:45.814Z Reads: 1249

```
They are rated to charge at 2C and are 3x 4S 5000mAh so it's only -10? Are you sure about that, it looks odd.
```

---
## \#5 Posted by: onloop Posted at: 2015-10-24T06:42:26.333Z Reads: 1184

```
what configuration is the battery?

you have 3 in series or 3 in parallel?
```

---
## \#6 Posted by: yendi Posted at: 2015-10-24T06:52:46.929Z Reads: 1133

```
3 x 4S 5000mAh 20C Tunigy in Series
```

---
## \#7 Posted by: RandV Posted at: 2015-11-04T08:14:44.843Z Reads: 1084

```
When the battery is recharging, does that count towards the battery's cycle limit? In other words, will the life of the battery be reduced from frequent regeneration?
```

---
## \#8 Posted by: Iceni Posted at: 2015-11-04T14:17:34.052Z Reads: 1061

```
Yes, since it's the recharging in and of itself that cause the wear on the batterylife.
It's just that it is the motor that provides the charging current instead of the wall-charger.
```

---
## \#9 Posted by: kampfhahn Posted at: 2016-07-18T12:58:11.146Z Reads: 924

```
Sorry for gravedigging :slight_smile:

If i understand this thread correctly, the only way to generate current to charge the battery is while breaking. This means, pushing the board in neutral mode doesn´t even charge the battery a bit, even if i do this for 10 km. So the only way to charge the battery on the road is to push very hard while braking with the remote or roll down a very long and steep hill breaking?
```

---
## \#10 Posted by: Namasaki Posted at: 2016-07-25T00:12:52.891Z Reads: 900

```
What if your using dual Vesc's?
Would you devide the current and set each Vesc at -6 amps battery regen max?
```

---
## \#11 Posted by: Pablo_702 Posted at: 2016-08-11T07:19:07.024Z Reads: 858

```
if i recall correctly it is not recommended that you push your board with out using the motor since it will fried a componenet in your vesc, i know i read it somewhere here
```

---
## \#12 Posted by: Hummie Posted at: 2016-08-12T18:36:11.342Z Reads: 827

```
If the batteries aren't connected
```

---
## \#13 Posted by: Jinra Posted at: 2016-08-12T18:51:30.367Z Reads: 825

```
The discussion was whether or not your VESC/ESC will be damaged by riding with the board off due to the small amount of electricity created from the spinning motors. We never conclusively found out if it is/isn't harmful for your system, but agreed that you would be fine as long as the board is on. My personal theory was that the current generated would be minuscule enough to not damage components even when the system is off.
```

---
## \#14 Posted by: Hummie Posted at: 2016-08-12T19:15:05.283Z Reads: 799

```
vesc will turn on if connected to motor and they spin.  if there are no batteries connected as well to send the energy too it will generate enough current to slam on the brakes if you're lucky and coasting or ruin components if youre not.  think the capacitors.  read this on vedders forum and I've experienced the brake slam on.

so i guess coasting is regening as well.  using the brakes without a battery attached is bad news though and quick death...although I got lucky there too
```

---
## \#15 Posted by: Namasaki Posted at: 2016-08-18T06:10:56.243Z Reads: 772

```
What if you disconnect the motor wires to push home, say if your battery runs too low. Would it damage the motors to spin if they are disconnected ?
```

---
## \#16 Posted by: Jinra Posted at: 2016-08-18T06:15:07.414Z Reads: 756

```
Pretty sure it won't damage anything, the current has nowhere to go.
```

---
## \#17 Posted by: Hummie Posted at: 2016-08-20T07:51:07.599Z Reads: 750

```
I'm pretty sure as long as you have batteries connected and coasting your fine.  Assuming they aren't fully charged and you don't go down a super steep hill that puts you over the erpm limit
```

---
## \#18 Posted by: chewydinosaurs Posted at: 2017-02-10T01:21:29.929Z Reads: 592

```
If I have 2x4000 3s batteries in series can I charge at 8 amps?
```

---
## \#19 Posted by: DIYer Posted at: 2017-03-04T15:45:46.026Z Reads: 556

```
How does regenerative braking work on a diy board?
```

---
## \#20 Posted by: Hummie Posted at: 2017-03-04T16:41:47.938Z Reads: 558

```
whey you apply the brakes the energy of your momentum gets converted back to electrical by the motor, then chemical energy in the battery with roughly 30 percent efficiency.   you can adjust on the vesc the amount
```

---
## \#21 Posted by: Avalonnw Posted at: 2017-03-08T23:14:25.394Z Reads: 531

```
Does VESC monitor the actual battery charge? If the battery is full and you try to charge it with 4 Amps, it might damage it.
```

---
## \#22 Posted by: Davey Posted at: 2017-03-29T17:04:29.783Z Reads: 511

```
does it charge via the xt60 connectors?
```

---
## \#23 Posted by: tatze Posted at: 2017-11-15T14:14:00.658Z Reads: 336

```
I have the same question. But it would make sense to me to devide it, if you have a dual vesc.
```

---
## \#24 Posted by: L3chef Posted at: 2018-02-26T10:00:00.913Z Reads: 278

```
Did you ever get an answer on your question? I'm wondering the same
```

---
## \#25 Posted by: Namasaki Posted at: 2018-02-26T13:00:08.418Z Reads: 279

```
As long as the connectors on the end of the phase wires don’t touch each other closing the circuit, there will be no resistance between the wire and the magnets. 
I believe it is safe to roll with the phase wires disconnected and secured so they don’t short out.
```

---
## \#26 Posted by: L3chef Posted at: 2018-02-26T13:04:48.206Z Reads: 274

```
Thanks, but I ment your regen question. If -12a is set with single setup. Should it be -6 with dual setup?
```

---
## \#27 Posted by: Pedrodemio Posted at: 2018-02-26T14:21:34.025Z Reads: 271

```
Yes, but this is a personal preference, you have to try a few combinations to see what you like better

The truth is, any charge current that has sufficient braking force is already too much to the small battery’s that most of us use (3P) but since there is currently no alternative we have to live with it, since we brake for only a short period it may have little influence on the cycle life of the battery 

That’s way boards like @Mellow have a integrated braking resistor, the excess energy goes there and is converted to heat
```

---
## \#28 Posted by: Namasaki Posted at: 2018-02-26T16:12:59.641Z Reads: 264

```
My bms and battery are rated for 20a charge so I run -10 per Vesc on dual. 
I could run -20a on single.
```

---
## \#29 Posted by: L3chef Posted at: 2018-02-26T16:55:41.444Z Reads: 257

```
Thanks!
Ten
```

---
## \#30 Posted by: Hummie Posted at: 2018-02-26T18:50:51.666Z Reads: 253

```
I didn't read the whole thread but is it the case u can up the motor regen to whatever,  (maybe 100 amps and maybe hardware r software limited?) And that increases brake power but not true regen And the battery regen to whatever u think your batteries are capable of  and thats the real regen?
Are the two speed dependent similar to motor n battery amp settings?  Or are the two regens interchangeable w same results ?
```

---
## \#31 Posted by: Redfire1 Posted at: 2018-06-15T16:59:32.280Z Reads: 203

```
@Pedrodemio @onloop @Iceni hi good,I finish my skateboard but when going down slopes some time it doesn’t brake,can anyone please tell me why and some time when on it will move without me touching the remote.
```

---
## \#32 Posted by: chinzw Posted at: 2018-06-15T17:17:44.459Z Reads: 201

```
Do you have a BMS? Is your battery fully charged? What battery do you have? Post a picture of your min/max battery vesc settings
```

---
## \#33 Posted by: Redfire1 Posted at: 2018-06-15T17:45:48.491Z Reads: 194

```
I am using Bsm I just plug my chargers in but it’s only showing green,and the battery is showing 28% volts don’t know what’s the problem
```

---
## \#34 Posted by: Redfire1 Posted at: 2018-06-15T17:48:58.944Z Reads: 193

```
That’s how I set I am using 2 vesc ![image|375x500](upload://3vPXdB1Gb6JSjFxzS1ktfmd5Ghx.jpeg)![image|375x500](upload://2lWm4O3CQwEGpd6sxS0ScGu8Ohs.jpeg)
```

---
## \#35 Posted by: Ebisane9 Posted at: 2018-06-15T20:09:09.053Z Reads: 176

```
That battery regen is way too high
```

---
## \#36 Posted by: Jebe Posted at: 2018-06-15T20:46:25.488Z Reads: 182

```
Do you have the app setting for current/watts with brake?
```

---
## \#37 Posted by: Redfire1 Posted at: 2018-06-15T21:15:45.973Z Reads: 184

```
What do you recon it should be ?
```

---
## \#38 Posted by: Redfire1 Posted at: 2018-06-15T21:16:12.450Z Reads: 185

```
@jebe no I don’t have one
```

---
## \#39 Posted by: Redfire1 Posted at: 2018-06-15T21:17:42.534Z Reads: 183

```
I connect my BSM like this https://youtu.be/_yrYG5skwvs
```

---
## \#40 Posted by: Jebe Posted at: 2018-06-15T22:00:53.756Z Reads: 189

```
the control setting I meant, for the ppm control setup in the vesc tool.
```

---
## \#41 Posted by: Redfire1 Posted at: 2018-06-16T09:21:46.749Z Reads: 186

```
[Uploading...]()
```

---
## \#42 Posted by: Redfire1 Posted at: 2018-06-16T09:33:35.392Z Reads: 184

```
![image|374x500](upload://yoqfqHhWq0cjxcfaEt4HJFkOmBx.jpeg)
```

---
## \#43 Posted by: Redfire1 Posted at: 2018-06-16T14:04:53.297Z Reads: 183

```
![image|374x500](upload://k7mRX1FnxffnqecAqon6vYjtLxb.jpeg)![image|374x500](upload://qz5JR3GOW6vkYb6AUtkTA3kZ46I.jpeg)![image|374x500](upload://cSfnoKqQ8A40W2F7eKDOBvqCW8N.jpeg)![image|374x500](upload://bkN5KC5p3gG15Zmw1oi7gkucMDV.jpeg)![image|374x500](upload://yALjug4JYWV94cS23wLCyMHkUMR.jpeg)![image|374x500](upload://toT76L4CJUqein0xSY0jsubE4sj.jpeg)![image|374x500](upload://hbmchWNXXaqE3s9uuAvveGJKSCu.jpeg)![image|374x500](upload://4HzrgU61EgXddaQ9AuCr3go5Vy4.jpeg)[Uploading...]()
```

---
## \#44 Posted by: PiratFPV Posted at: 2018-08-17T10:43:23.940Z Reads: 149

```
I noticed on FLsky VESC 6.6 that to have breaks I have to increase amperage in " Battery current max regan " otherwise breaks are not working , even if I got -60A at " Motor current max Break "
So how can I set breaks without recharging battery ?
```

---
## \#45 Posted by: Koolfarmer Posted at: 2018-09-04T23:17:08.471Z Reads: 146

```
From my humble knowledge, you cannot have break without Regen. Where would the energy go? something would need to get very very hot to absorb this energy. Remember Physics courses: nothing disapear, everything transforms.
```

---
## \#46 Posted by: mishrasubhransu Posted at: 2018-12-05T19:11:54.723Z Reads: 124

```
It would be wasted as heat in the motor and the ESC.
```

---
## \#47 Posted by: b264 Posted at: 2018-12-05T19:30:08.190Z Reads: 124

```
An ESC can be designed with a braking resistor that disspates heat into a heatsink if you didn't want to charge the battery with it or if the battery was full already.  VESC is just not designed with this feature.
```

---
## \#48 Posted by: Cedric Posted at: 2019-02-28T14:26:44.519Z Reads: 99

```
On focbox UI, if I set the PPM mode on fwd/reverse instead of fwd/brake, will it regenarate the battery while braking?
```

---
## \#49 Posted by: sayekim Posted at: 2019-02-28T15:42:19.243Z Reads: 93

```
It should. I run the vesc tool for 3.39 and have it set to Current. 
I brake to a stop and reverse. If not, it’s a kind of magic that’s slowing me down and charging my batts.
```

---
## \#50 Posted by: J95hicks Posted at: 2019-04-21T17:32:36.604Z Reads: 75

```
I have a question that i believe best fits here(as opposed to a new thread lol). When refering to high speed braking, the main contributing setting is battery min, correct? But does motor min still play a partial roll at high speeds? I was riding yesterday, and going down a pretty steep hill i was no longer able to brake! Im 270lbs and my thought was due to my weight, the incline and my speed.... is it possible I was exceeding my Battery min, losing my ability to brake bc the regen setting was being exceeded? This happened twice and as soon as I slowed down I was able to brake again. Oh also, the first time i was able to brake at the top of the hill slightly at first but as I gained speed and the incline increased i completely lost brakes. And I was still able to accelerateXD so it was not a connection issue... bumpXD
```

---
## \#51 Posted by: b264 Posted at: 2019-04-24T04:22:16.777Z Reads: 69

```
[quote="J95hicks, post:50, topic:353, full:true"]
When refering [sic] to high speed braking, the main contributing setting is battery min, correct?
[/quote]

Yes

[quote="J95hicks, post:50, topic:353, full:true"]
But does motor min still play a partial roll [sic] at high speeds?
[/quote]

Not unless it's excessively high, and also higher than Battery Min.  Essentially, no.

So if  
Motor Min -10A  
Battery Min -20A  

then yes, it could override Battery Min but as long as Motor Min is under -20, say like -30A or -40A then it won't matter for high-speed braking.

[quote="J95hicks, post:50, topic:353, full:true"]
I was riding yesterday, and going down a pretty steep hill i was no longer able to brake!
[/quote]

Was your battery fully-charged?  You can't charge a full battery.
```

---
## \#52 Posted by: J95hicks Posted at: 2019-04-24T05:15:29.425Z Reads: 69

```
thx for the reply, it happened twice. One close to full, yes. The other time it was about 75 percent. So i dont think that was it. Motor min was -75, Batt min was -20. I recently switched to Foc too... idk, if thatd play in at all.
```

---
## \#53 Posted by: TSJ Posted at: 2019-05-22T20:01:03.670Z Reads: 52

```
I have a 10S3P battery and have set bat min at -12amps per the 4A/cell recommendation and motor min at -40amp on a single TB 6350 190eV motor.  I find that my brakes are not strong enough on steep hills to keep me from accelerating down.  Is this limited by the battery min?  If so, is there anything I can do in the settings to improve this, or would I need a 4P or 5P battery?  What is the risk if I up the battery min since breaking is infrequent and the duration is typically not too long?
```

---
## \#54 Posted by: jun1208 Posted at: 2019-05-23T00:13:12.917Z Reads: 50

```
If I am not mistaken, none of the VESC has the setting to allow brakes strong enough to make the board stay in place on a slope...
```

---
## \#55 Posted by: Darkie02 Posted at: 2019-06-26T20:17:45.455Z Reads: 40

```
[quote="Hummie, post:20, topic:353"]
then chemical energy in the battery with roughly 30 percent efficiency.
[/quote]

Am I going down the right lines in thinking 100a from the motor back EMF to VESC ends up as 30a charge to the battery.

If so dose the battery min ideally be at least approx 30% of motor min

So in a practical use for calculating you’r battery min spec you wanted -60A motor (Dule set up -30A per motor) you would want a battery regen about -18amps (Dule set up 9A per VESC) min spec of battery charge current?
```

---
## \#56 Posted by: Hummie Posted at: 2019-06-26T20:47:18.315Z Reads: 37

```
I don't know where I heard that and thinking about it...where's the rest of that energy going if not the battery?  or maybe sadly its lost as heat in the motor.
```

---
