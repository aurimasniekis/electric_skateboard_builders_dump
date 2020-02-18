# Does Lower KV Really Mean More Torque?

### Replies: 114 Views: 14467

## \#1 Posted by: claudiofiore88 Posted at: 2016-06-10T22:02:16.021Z Reads: 647

```
I feel like this has been disproven in the past, but people still continue to claim a lower kv motor have more torque and a higher kv motor having less torque.  Is this really the case or does motor torque come down to the mass of copper windings and stator size?

@jacobbloy @Hummie @longhairedboy @psychotiller
```

---
## \#2 Posted by: JLabs Posted at: 2016-06-10T22:09:38.949Z Reads: 647

```
I am currently using a tacon bigfoot 295kv, and I can climb hills larger than I ever imagined. I wrote about it here
http://www.electric-skateboard.builders/t/alpha-build-the-torque-misconception-jlabs-open-source-motor-mount-orangatang-spacers/2698
So in my opinion, no lower kv does NOT mean more torque, it is in the gearing. On the other hand hub motors may be different, I have no expirence with them.
```

---
## \#3 Posted by: Hummie Posted at: 2016-06-10T22:20:19.998Z Reads: 635

```
In a motor more than anything to create torque, in a small package especially, you need iron. nothing is as important for torque as iron.  The iron greatly enhances the windings magnetic field and u get a greater magnetic strength. At some point trying to get more and more magnetic strength from the electromagnet, pumping in more amps, the iron enhancer becomes magnetically saturated and the more amps u give it isn't increasing the strength of the iron's magnetic field.  More iron, or more importantly more iron on the end of the stator tooth, where its used, and eventually gets saturated given too many amps. 
  Adding gearing is a huge way to get torque.
Kv doesn't matter as even with a really high kv u can give it more amps and run a low voltage system and get exactly the same power output and the same torque output. Gets just as hot as the low kv in the motor. And the same size battery and watt hours.  Why no one runs on 4s or even 2s..I don't know.  If the controller can do it that's the only limitation. The motor sees either the high voltage or low voltsge systems the same and the volts are converted to amps as far as the motor sees it.  Just as much torque or watts output before overheat in the motor with either system
```

---
## \#4 Posted by: Maxid Posted at: 2016-06-10T22:23:45.743Z Reads: 614

```
That seems like the most unscientific explanation. Gearing obviously changes the characteristics.
You can get any torque or speed output you wamt by adjusting the gearing accordingly.
To answer that question fairly no gearing has to be used and then the output can be compared.
```

---
## \#5 Posted by: NNGG Posted at: 2016-06-10T22:26:05.010Z Reads: 600

```
Don't forget the vesc limitations on 12s. We should only use about <220KV at 12S unless we limit the vesc rpm
```

---
## \#6 Posted by: JLabs Posted at: 2016-06-10T22:36:52.501Z Reads: 596

```
Your right, the gearing does change it. But everyone uses gearing........

I also didn't know this was a science competition. I was just giving my input
```

---
## \#7 Posted by: Maxid Posted at: 2016-06-10T22:43:08.890Z Reads: 580

```
Well this is ultimately physics that we are talking about - and misleading headlines like "torque misconception" should not be used for this type of thing. If you want to do it right you need to get rid of gearing, test the motors and only then tell the differences between high and low kv motors.
```

---
## \#8 Posted by: jacobbloy Posted at: 2016-06-10T23:35:52.625Z Reads: 559

```
As @Hummie said as long as the copper mass, iron and magnets are all the same the output of the motor is the same. Kv is about at what voltage is the motor efficient before drawing To many amps.

Some one correct me if I'm off base!

You need to calculate what speed you want to be riding at 80% of the time and then try and get the motor spinning at about 5-8000rpm at this speed with the highest voltage you can.

Sadly this doesn't work so well for hub motors as you can't gear so you have to reduce your kv.

Boosted use a 1:3.12 gear ratio with a 190kv motor and 43.2v battery. So in turn they have a low top speed but at 20-30km/h they have a really low amp draw and good efficiency, if they used a higher kv motor that efficiency would be at a lower speed and at they would want to use a gear ratio of 1:26 to get the efficiency back up to that speed sweet spot but would loose some low end torque (which they need with such small motors)

Raptor has a bigger motors so can use a 1:26 gear ratio with similar voltage same kv and bigger wheels. So it's efficiency is between 30km/h to 45km/h at its top speed. So for a rider like me who doesn't go faster then 30km/h then the setup is not going to be good for me.

My opinion is we need split gears.

Read more:
http://vedder.se/2014/10/chosing-the-right-bldc-motor-and-battery-setup-for-an-electric-skateboard/
```

---
## \#9 Posted by: psychotiller Posted at: 2016-06-11T01:59:13.844Z Reads: 506

```
The sweet spot is between 190kv and 300kv  Outside of that, your speed will suffer. Too fast  or too slow. 

No groundbreaking tech speak here...just tried and true results.
```

---
## \#10 Posted by: Bobfandango Posted at: 2016-06-11T02:41:46.622Z Reads: 477

```
A lower kv motor does have more torque.....  _per amp!_. This is the thing people always leave off or forget or don't understand.  The lower kv motor will make more torque at a given current than a higher kv motor all else being equal (i.e. You are comparing motors that are identical aside from how they are wound).
```

---
## \#11 Posted by: Bobfandango Posted at: 2016-06-11T02:56:42.078Z Reads: 465

```
People would use 2s or 4s if they could.  But you do know!  Yes, the limitation is the controller. No controller can currently drive the kind of current that would be required to run 2s or 4s.
```

---
## \#12 Posted by: thisrealhuman Posted at: 2016-06-11T03:58:20.765Z Reads: 458

```
Here's my understanding: a 3,000W motor will get me to 30mph without overheating. 3,000W is 4 horsepower, and the scooters here in LV are limited to 2HP (supposedly) and can do 35 with 1/2 mile of runway. 

That's 4 "MECHANICAL HORSEPOWER", so as long as my gearing sets my top speed reasonably, a 30% reduction in KV will equate to 30% reduction in top speed, BUT, 30% increase in motor gear teeth will compensate perfectly.....

IF the motor has the same WATTAGE.
So, 4HP from 245kv is exactly the same as 4HP from 190kv or 149kv.... Right?

No, because the efficiency of the motor depends on the RPMs. 
I changed my 10s, 245kv, 83mm, from 12t to 15t, and although I did get (exactly) 25% increase in speed, my braking torque was almost gone and because of the increase in current required to do 25% more work, my range seemed to decrease also, but I was probably hot-rodding around.
I've ordered a 190kv so I can compare my braking power with electrical torque (low KV) vs mechanical torque (high KV), keeping in mind that I use a K-force that has a drag brake, meaning my brakes are always using exactly the same current.

I think we need to figure out which type of breaking torque kills motors, and gear accordingly.
```

---
## \#13 Posted by: jacobbloy Posted at: 2016-06-11T04:27:35.084Z Reads: 425

```
3,000w is around 4HP but depending on your motor as some suck, and the drive train you might only get 3HP.
```

---
## \#14 Posted by: thisrealhuman Posted at: 2016-06-11T04:57:43.917Z Reads: 425

```
Damn entropy and capitolism, and gravity...

Always gettin me DOWN, man.
```

---
## \#15 Posted by: whitepony Posted at: 2016-06-11T05:09:37.177Z Reads: 426

```
[quote="Bobfandango, post:10, topic:4529"]
A lower kv motor does have more torque.....  per amp!
[/quote]

^this


thats what i wrote a while on ES when contemplating about 190KV 6355 rspecc to 168KV SK6374 switch:

____________________
Im not actually sure what I can expect from a lower KV motor except for a better torque per current ratio. to ride the same speed will cost the same power (naturally, since the same work has to be done). a nice graphic to understand that can also be found here: [mabuchi motor tech](http://www.mabuchi-motor.co.jp/en_US/technic/t_020203.html) --> same speed = horizontal line = same current for identical motors with different winding numbers.

at the same time, for a constant torque you can see that different winding numbers produce the same torque with different currents (vertical line): more windings = lower KV = more torque per current.

when I ride with a constant 35kph, the only difference I will notice coming from my 192KV r-speccs, is the simple copper increase from 6355 -> 6374. the KV change from 192 to 168 wont make a difference, except for my top end power: higher KV = higher power output, since its running at higher speed and power is basically rpm x torque.

so, the only thing Im hoping for with the KV downgrade is less heat in my vesc when I really need just torque and still sufficient speed on the straights, since with 16/36T, the setup can still reach up to 45kph.
```

---
## \#16 Posted by: itsmikeholland Posted at: 2016-06-11T06:12:31.691Z Reads: 388

```
wait wait wait, what about the controller limits 4s from happening? I've never heard anything about this before, I've been browsing this place for about 2 months now and just thought everybody wanted to go super fast. I have 3x 4s batteries, is it not possible to use just one?
```

---
## \#17 Posted by: psychotiller Posted at: 2016-06-11T06:39:54.133Z Reads: 377

```
Lower voltage = Higher amps. The more amps you pull through your esc the greater chance it will say uncle.
```

---
## \#18 Posted by: itsmikeholland Posted at: 2016-06-11T06:41:30.611Z Reads: 369

```
oh no! my set-up is gonna be 12s 6.6ah @ 60C constant. Did I just royally screw up with the massive discharge rate from my 3 4s batteries?
```

---
## \#19 Posted by: Hummie Posted at: 2016-06-11T06:50:44.416Z Reads: 368

```
The reasons to not use one of those batteries...from the battery perspective it would need to be a really high c rating and be able to discharge what's asked of it or it will have few life cycles and also suffer voltage sag in use and keep u slow.   From the perspective of the motor... As long as the kv is increased by 3x it wouldn't notice and you'd go just as fast and just as much torque. From the escs perspective...it now has its power coming from
the battery with a much thicker mix of amps than would be the case with 12s. It will get hotter. Making 1000 watts from 16volts u need to multiply like 70 amps((too many for the vesc but there are escs that will do that)). Or making 1000 watts from 45 volts and multiplying with that you only need like 25 amps and that's no problem for the vesc or a lot of controllers.
```

---
## \#20 Posted by: psychotiller Posted at: 2016-06-11T06:52:23.407Z Reads: 350

```
No. 12s is high voltage. (lower amps) 

Think about it. Most 6s ESCs can handle 120a. Some 6-8s esc can handle 180a-200a.
```

---
## \#21 Posted by: itsmikeholland Posted at: 2016-06-11T06:57:08.108Z Reads: 342

```
Thanks, that reassuring. So the 60C constant and 120C burst is nothing of concern when using a 120A vesc? I didn't think these batteries were gonna be a problem when I bought them, but I lost all the notes I took when picking them out
```

---
## \#22 Posted by: Hummie Posted at: 2016-06-11T07:05:07.011Z Reads: 333

```
12s 6.6ah and 60c
Multiply the 60 times the 6.6 and that's what is said to be the continuous safe amp discharge of ur batteries without them being over drawn.  That's a very high number.  The real battery number is lower than that and it's overrated.  Even at half that c rating ,30, times 6.6...200amps about.  Way way more than ur motor or ur controller will be able to do and way more than you'll need
```

---
## \#23 Posted by: itsmikeholland Posted at: 2016-06-11T07:08:20.103Z Reads: 319

```
ohhhhh okay so this doesn't mean that I _will_ be drawing that much 100% of the time, only that I _can_? That's good to know if so, I bought these specifically to meet the FAA regulations for 100wh with a max of 3 batteries, which happens to give me 12s. I'm very much relieved, the 3 batteries were $197, I'd be pissed if I couldn't actually use them.
```

---
## \#24 Posted by: Hummie Posted at: 2016-06-11T07:23:02.733Z Reads: 312

```
I looked at the faa regulations and I had it wrong before, you can only take 3 lithium batteries total.  The size can be 100 watt hours and if the airline wants it can be up to 160 watt hours. Maybe they aren't enforcing it exactly as I think people are getting through with more. 
(3) 4s 6.6ah packs is a nice number to be legal just under the 100watthours and get 12s
```

---
## \#25 Posted by: itsmikeholland Posted at: 2016-06-11T09:00:35.717Z Reads: 304

```
People are definitely getting through with more, since theres no real way to know the capacity. My concern is that if for whatever reason my batteries decide to explode, the fire should be easier to control and i wont die...hopefully. im really hoping to squeeze this in a 22 inch board to carry on so that it isnt mishandled, but i need all my parts first to see what kind of real estate we're dealing with. I think 12s 6.6a is gonna be pretty great regardless of them meeting the faa regulations, only time will tell with this 149kv motor ive got here waiting
```

---
## \#26 Posted by: Bobfandango Posted at: 2016-06-11T15:04:09.463Z Reads: 294

```
I'm experimenting with a kv "downgrade" as well.  I have a HK 6374-149kv on the way to go in place of my HK 6374-192kv.  Now in theory, these motors are equivalent (same can, same magnets, same iron, same amount of copper). However, if the specs HK posts online is to be believed, the 149kv may be a better choice (hence the experiment).  

That is, I compute the motor constant Km for both motors, and the 149kv should be somewhat better.  Now, I will still be running 12s, so my top speed will suffer.  But I'm okay downgrading from insane, certain death top speed to merely absurd top speed.  

More info about Km here....  http://www.motioncomp.com/pdfs/Motor_Constant_Great_Equalizer.pdf

Anyhow, Km may be a good sanity check when considering motors changes.
```

---
## \#27 Posted by: SimosMCmuffin Posted at: 2016-08-04T11:49:37.885Z Reads: 255

```
Higher battery voltage and lower kV motor will be more efficient, because the current will be lower.
a 300 kV motor and 4S battery is less efficient than
a 100 kV motor and 12S battery just by pure heat losses alone.
Remember heat loss for the current is I^2 * R, so double your current, quadruple your power wasted as heat.

There is a reason why the energy grid is in the magnitudus of kiloVolts and not in the hundreds, because if it were in the hundreds of Volts you would be melting your airlines by heat losses alone.
```

---
## \#28 Posted by: sismeiro Posted at: 2016-08-04T12:03:42.314Z Reads: 256

```
[quote="SimosMCmuffin, post:27, topic:4529"]
Higher battery voltage and lower kV motor will be more efficient, because the current will be lower.a 300 kV motor and 4S battery is less efficient thana 100 kV motor and 12S battery just by pure heat losses alone.Remember heat loss for the current is I^2 * R, so double your current, quadruple your power wasted as heat.
[/quote]

OK, this is true. But which one has more torque for a given wheel RPM? Or when we start from a stand still position?
```

---
## \#29 Posted by: Hummie Posted at: 2016-08-04T15:32:57.500Z Reads: 245

```
not true.  
it takes less amps to get the same torque from a 100kv motor as it does a 300kv motor.  thinner wires but less amps needed.   it all balances out and if your battery is sized correctly you can get the same performance out of any motor if the kv and battery are correctly sized.   It's true that the other wires in the system need to be increased in size if it is a heavy amp system and it can be pushing the limit on some esc but the motor itself will get just as hot.
I dont understand you about airlines.  Yes powerlines benefit from transforming to volts for distances but a motor isnt a power line.
```

---
## \#30 Posted by: SimosMCmuffin Posted at: 2016-08-04T15:35:32.868Z Reads: 251

```
[quote="sismeiro, post:28, topic:4529"]
OK, this is true. But which one has more torque for a given wheel RPM? Or when we start from a stand still position?
[/quote]

Each motor, provided that they are otherwise identical (physical size, pole amount, magnet quality, stator quality), except for different gauge motor windings and turns. As long as they have the same amount of copper on the stator. The torque would be identical, but the higher kV, lower battery voltage motor will run hotter and less efficiently due to heat losses caused by higher currents.

I found a good Vedder's article today, which explains some of the motor characteristics. And he concludes the same thing. "As long as the copper amount is same, the motors have identical power"
 http://vedder.se/2014/10/chosing-the-right-bldc-motor-and-battery-setup-for-an-electric-skateboard/
```

---
## \#31 Posted by: Hummie Posted at: 2016-08-04T15:35:38.078Z Reads: 239

```
either will have the same torque from any position.  If it's a high kv it will take more amps, yes, but the winding is thicker so less heat.  and if the battery is specd right  it will be a low voltage battery with more amps to suit the motor and ultimately be the same energy and performance from battery and motor
```

---
## \#32 Posted by: Hummie Posted at: 2016-08-04T15:37:45.154Z Reads: 236

```
that article is right and says that a low kv and high kv will perform the same.
```

---
## \#33 Posted by: devin Posted at: 2016-08-04T16:39:49.256Z Reads: 231

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#34 Posted by: Hummie Posted at: 2016-08-04T18:04:26.487Z Reads: 224

```
Two motors identical other than the kv will perform the same regardless of the load if the kv and voltage are matched.
```

---
## \#35 Posted by: devin Posted at: 2016-08-04T18:07:33.878Z Reads: 229

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#36 Posted by: Hummie Posted at: 2016-08-04T18:28:19.202Z Reads: 221

```
If the rest of the system is the same between two motors the lower kv will have more torque.  I'm saying it need not be the case though and if both systems are have optimized battery voltage and kv  they'll have the same performance and total watt hours converted to power and torque
```

---
## \#37 Posted by: devin Posted at: 2016-08-04T18:30:15.533Z Reads: 216

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#38 Posted by: Hummie Posted at: 2016-08-04T18:33:11.534Z Reads: 216

```
Maybe so u don't have to use impractical giant gears.    Running a 2000kv motor with a 20:1 gear ratio is impractical but running that motor with only 2s and an esc that can put a lot of amps through will give the same performance.
```

---
## \#39 Posted by: devin Posted at: 2016-08-04T18:34:28.860Z Reads: 213

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#40 Posted by: Hummie Posted at: 2016-08-04T18:38:22.872Z Reads: 209

```
Same range.  Same watt hour battery.  One w lots of amps one w lots of volts
```

---
## \#41 Posted by: devin Posted at: 2016-08-04T18:42:00.671Z Reads: 200

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#42 Posted by: HTownBomber Posted at: 2016-08-04T19:02:19.399Z Reads: 201

```
Yes, inefficiency (waste heat) is current squared times winding resistance. But resistance goes up exponentially in the windings of the lower kv motor, which effectively cancels out the impact of the change in current. From your own link (Mr Vedder):

_Let’s look at an example: Suppose an 8 turn motor has one ohm winding resistance. The winding resistance is proportional to the wire area times wire length. Making the same motor with 4 turns would allow twice as thick wire. Since that wire also is half as long, the resistance is four times lower: 0.25ohm. Further, since current times turns is proportional to torque, we need twice as high current with 4 turns to produce the same torque as with 8 turns. The copper losses are the voltage across the windings times the current: U*I. The voltage across them is R*I, so the losses are R*I*I. This square relation means that doubling the current will produce four times as much losses, however, since we got four times lower resistance the losses are the same for the 4t motor with double the current as for the 8t motor with half the current. Also note that the 4t motor will spin twice as fast as the 8t motor at the same voltage, so it will have double the kv. Putting this together, the 4t motor is equivalent to the 8t motor, but at half the voltage and double the current._
```

---
## \#43 Posted by: SimosMCmuffin Posted at: 2016-08-04T20:16:48.973Z Reads: 195

```
If the motor itself is not a factor in the power efficiency, since the attributes cancel each other out (motor kV), then there are still other parts that don't change to counter the heat losses, the ESC mosfets and wiring.

This is also from Vedder's post.
> From the ESC perspective, we should run on as high voltage and low current as possible. Now, one interesting fact about MOSFETs is that the lower voltage they are designed for, the lower resistance they tend to have. So if I make an ESC for a lower voltage, the FETs will also have lower resistance. However, the PCB traces always have the same resistance and MOSFET resistance does not seem to decrease as fast as their voltage decreases, meaning that an ESC designed for higher voltage tends to be more efficient in general.

I wish I had actual practical test data to test this argument... Now that I've thought about it more, it seems to be as Vedder said. I will continue pondering and researching this topic :confused:...
```

---
## \#44 Posted by: PB1 Posted at: 2016-08-04T21:05:34.447Z Reads: 174

```
@SimosMCmuffin,  every motor has a torque constant, Kt.  Kt= The amount of torque produced per amp.  So in a motor torque is proportional to current.  

Kt = 1 / Kv  these two are linked.  This means that a lower Kv motor will produce more torque per amp or that a higher Kv motor needs more amps to produce the same torque.
```

---
## \#45 Posted by: SimosMCmuffin Posted at: 2016-08-04T21:17:23.134Z Reads: 177

```
Ok, I might have been a bit confused earlier with the statement and I admit I might have had the wrong understanding of the mechanics.

But now I'm really wondering how does efficiency come into play in _real life_ situation? Shouldn't the efficiency and range be the same if you have two same energy capacity batteries?
One with lower voltage, higher capacity (4S 10000 mAh) and the other with higher voltage, lower capacity (8S 5000 mAh).
Two otherwise identical motors, except for the kV, (150 and 300 for example) would be matched to get the same no-load top speed with the proper battery.

Now I really want to do a practical test...
```

---
## \#46 Posted by: ninja Posted at: 2016-08-04T21:25:39.937Z Reads: 164

```
Hey! You are from LATVIA? Me too. If so maybe we can meet up sometime to ride, i'm from RIGA. For now i only know one guy from Riga, who have esk8.
```

---
## \#47 Posted by: Hummie Posted at: 2016-08-04T21:26:56.779Z Reads: 169

```
I forget who it was but someone here did do a test which was similar in which they simply cut their battery voltage from 12s to 6s and did the same steep route at about 15mph and compared the watt hours spent.  It was close but the 12s system was a bit less efficient.  I'd understood that the 6s run would be more efficient as the speed of the climb would be closer to the no load speed at 6s max throttle than 12s max throttle.  I was thinking of the no-load speed being a fixed number solely based on battery and kv, but recently discovered that the no-load is constantly changing as the throttle setting changes.  Ex: half throttle is an effectively  half the max voltage of he battery and so the no-load speed is now half as high!   This was a surprise to me so I don't know why either would be more efficient than the other 
I now understand the difference between the no-load speed and the speed the motor is running in relation to that is purely determined by the load and size of the motor
```

---
## \#48 Posted by: SimosMCmuffin Posted at: 2016-08-04T21:35:01.112Z Reads: 160

```
But they didn't change the motor? So he ran the route at half the battery voltage at half the speed basically?
What I'm wondering is what if they change both battery voltage AND motor kV so that the no-load max speed stays the same. That way the max speed should still be same.

Of course running slower is more efficient on just pure aerodynamics alone, also the mosfets and wiring will have more I^2*R heat losses with higher amps so that also decreases efficiency, but he did use the SAME motor.
```

---
## \#49 Posted by: Hummie Posted at: 2016-08-04T21:37:15.323Z Reads: 159

```
Same speed up hill (he thinks). Same motor and kv.  And the batty variation only.

The mosfets and the current they experience I think is more related to the motor side and would need to apply the same current to get the same torque with the same kv
```

---
## \#50 Posted by: SimosMCmuffin Posted at: 2016-08-04T21:46:23.361Z Reads: 159

```
Just to clarify.

So he felt like he was going uphill at the same speed with the 6S battery, as with the 12S battery?
```

---
## \#51 Posted by: Michaelinvegas Posted at: 2016-08-04T21:48:00.606Z Reads: 156

```
[quote="Hummie, post:47, topic:4529"]
I forget who it was but someone here
[/quote]

Was it @Namasaki?
```

---
## \#52 Posted by: willpark16 Posted at: 2016-08-04T21:48:38.454Z Reads: 155

```
ok so if im running 12s it would be better for me to run 145 vs 245?
```

---
## \#53 Posted by: SimosMCmuffin Posted at: 2016-08-04T21:57:16.136Z Reads: 158

```
[quote="willpark16, post:52, topic:4529, full:true"]
ok so if im running 12s it would be better for me to run 145 vs 245?
[/quote]

What kind of top speed are you wanting? what is your motor/wheel gear teeth ratio and what size are your wheels?
```

---
## \#54 Posted by: willpark16 Posted at: 2016-08-04T22:12:19.089Z Reads: 147

```
83mm and 16 by 36
```

---
## \#55 Posted by: SimosMCmuffin Posted at: 2016-08-04T22:26:15.870Z Reads: 148

```
[quote="willpark16, post:54, topic:4529, full:true"]
83mm and 16 by 36
[/quote]

And the speed you would like to travel at??
```

---
## \#56 Posted by: willpark16 Posted at: 2016-08-04T22:41:22.008Z Reads: 148

```
over 25mph
```

---
## \#57 Posted by: Jinra Posted at: 2016-08-04T22:42:19.655Z Reads: 151

```
You can use this calc to find the speed you'll go

http://calc.esk8.it/

If you're running 12s stay under 170kv to avoid hitting the erpm limit.
```

---
## \#58 Posted by: willpark16 Posted at: 2016-08-04T22:43:30.532Z Reads: 155

```
haha no im saying is it better to run 245 or 145 at 12s im using a tb esc
```

---
## \#59 Posted by: Jinra Posted at: 2016-08-04T22:46:39.337Z Reads: 160

```
Still the same, 145 for the 12S. 245 would be insane
```

---
## \#60 Posted by: makevoid Posted at: 2016-08-04T22:59:39.992Z Reads: 163

```
I switched from 6s to 10s and I noticed that at 6s, with the same settings (with motor max A maxed out because I didn't care about battery life) changing different lipos (6S vs 10S and then 8S), the 6S climbed more than the 10S. I generally had hotter ESC but colder motor at 6S because I didn't make the motor stress under load when doing hills (because I had more torque?)... I decided then to go with a 8s (because I'm using 97mm wheels that's why it can't go uphill with me 200lb+/~95kg with a single 637x motor with a 10S battery)  and I still have a good max speed

Am I right or wrong to think that you should aim to stay near your desired top speed and try to use the highest possible voltage (for the VESC to be efficinent) but that doesn't shift your top speed so that you have a lot that you wouldn't use? Otherwise you lose acceleration and efficiency under load? ...is this right?

(at 6S has a top speed that is too low for me that's why I went with 8S)

basically if I went 10S I had ~11km/h - 6mph of speed more that I wouldn't use, and, even if the ESC would have ran cooler, I would have had less torque, the other way to go at 10S would be to increase my gear ratio like 14T/40T but I'll need a belt idler for that, do you think it's worth it or should I keep running at 8S ? I guess the only thing is to try 10S or 12S on another board before rearranging these cells :)

sorry for hijaking the thread a bit my question is really **Does Lower V** (battery S, number of cell in series) **mean more torque?** (if you can still hit your desired max speed) Yes?
```

---
## \#61 Posted by: willpark16 Posted at: 2016-08-04T23:01:07.827Z Reads: 154

```
insane but doable?
```

---
## \#62 Posted by: Jinra Posted at: 2016-08-04T23:02:08.644Z Reads: 154

```
You'll have crazy heat and amp draw, and probably break something (most likely the ESC), but if you're able to overcome that, then yea do-able on paper.
```

---
## \#63 Posted by: willpark16 Posted at: 2016-08-04T23:12:26.523Z Reads: 153

```
oh nvmd then
```

---
## \#64 Posted by: willpark16 Posted at: 2016-08-04T23:12:57.654Z Reads: 146

```
its cause miami boards runs his on 12s with 250kv
```

---
## \#65 Posted by: Jinra Posted at: 2016-08-04T23:15:13.601Z Reads: 146

```
Link?

10 chars
```

---
## \#66 Posted by: SimosMCmuffin Posted at: 2016-08-04T23:16:48.921Z Reads: 151

```
Lot of text and a lot of points I'm interested in.

[quote="makevoid, post:60, topic:4529"]
the 6S climbed more than the 10S.
[/quote]

So it climbed more hills overall or the same hills on your route faster? Could be just that you were using lower power and speed to go uphill so the heat had time to dissipate?

[quote="makevoid, post:60, topic:4529"]
I generally had hotter ESC but colder motor at 6S
[/quote]

Is the ESC in an airflow or stuffed inside a sealed compartment?

I'm guessing the amperage you were pulling with a 10S going uphill was starting to saturate the stator coils, causing lower efficiency and more heat.

Also, what is your motors kV and the used gearing?
```

---
## \#67 Posted by: willpark16 Posted at: 2016-08-04T23:18:24.596Z Reads: 150

```
http://www.electric-skateboard.builders/t/meb-dirty-dervish-12s-stealth-battery-twin-esc-hub-motor/5104

dual 250kv motors
```

---
## \#68 Posted by: Jinra Posted at: 2016-08-04T23:20:15.049Z Reads: 146

```
those are hubs, no way they're 250kv. More likely 80-90kv.
```

---
## \#69 Posted by: willpark16 Posted at: 2016-08-04T23:21:08.176Z Reads: 145

```
scroll down a bit more
```

---
## \#70 Posted by: Jinra Posted at: 2016-08-04T23:25:10.809Z Reads: 147

```
I see. He mentioned he doesnt hit full throttle on it. Hitting 40mph+ while already insane taxes the controller a lot as well. I imagine if he tried it for an extended period of time that the ESC would end up blowing or melting. Maybe you should order his or TB's esc and be our guinea pig :)
```

---
## \#71 Posted by: willpark16 Posted at: 2016-08-04T23:26:02.506Z Reads: 147

```
haha oh at most id go 26 but i already have the 245kv motor
```

---
## \#72 Posted by: makevoid Posted at: 2016-08-04T23:43:42.585Z Reads: 148

```
I don't know, maybe I'm wrong... is higher voltage be always better? I mean if we could run at 14S or 16S would it be much better than 10S or will we lose torque to get a motor going up a hill for example?
```

---
## \#73 Posted by: SimosMCmuffin Posted at: 2016-08-04T23:50:37.986Z Reads: 150

```
What is your motors kV and the used gearing?

Didn't you say that with the 10S you already had 6 mph on the top end you didn't use? So why use such high series cell battery? On the other hand, what you could do is get a smaller kV motor that would run at the current 8S speed with a 12S? It should feel more punchy/torque
```

---
## \#74 Posted by: Namasaki Posted at: 2016-08-05T00:19:11.227Z Reads: 144

```
It was me. I ran a comparison between 12s and 6s
Going s
And speed up the same hill. 
12s at half throttle 
6s at full throttle 
12s pulled half as much current from battery than 6s
But Esc's got hotter with 12s(just a little hotter)
```

---
## \#75 Posted by: makevoid Posted at: 2016-08-05T00:19:41.911Z Reads: 139

```
I have 192kv 15T/36T, yes I guess I could get a SK3-6374-149 and run @ 10S but I like the 6374 sensored from esk8.de and also the way the current 192kv (enertion) mounts the motor pulley. They have the machined shaft to fit the key that makes pulley installation very easy, with the others I needed grind the shaft to fit the keyway or use green threadlocker, sub-optimal options imho.
```

---
## \#76 Posted by: SimosMCmuffin Posted at: 2016-08-05T10:22:24.910Z Reads: 132

```
Makes sense, as with the 12S battery the ESC experiences higher current pulses which will cause more heat.
```

---
## \#77 Posted by: Bender Posted at: 2016-08-05T13:49:39.855Z Reads: 133

```
[quote="Namasaki, post:74, topic:4529, full:true"]
It was me. I ran a comparison between 12s and 6sGoing sAnd speed up the same hill. 12s at half throttle 6s at full throttle 12s pulled half as much current from battery than 6sBut Esc's got hotter with 12s(just a little hotter)
[/quote]


I'm a little confused by this, or maybe it was just to see the amp draw?
I've switched from 6s to 12s and am able to get up hills that 6s couldn't do
What kv was your motor? 
Maybe it's better matched for 6s
```

---
## \#78 Posted by: Hummie Posted at: 2016-08-05T16:09:40.091Z Reads: 133

```
At least the vesc is said to run cooler with more voltage.  Less amps pulled from batteries but same current will go to motor.   I was recommended to go with more voltage with the vesc by Vedder and Ren.  Good for vesc.  Just as good for motor

I'm hoping someone can explain if there's any difference between the 6s and 12s at half throttle.  

i think escs take a hit on efficiency when at half vs full throttle. But the battery draw is much less on 12s. 

How the motor's efficiency changes if really like to know. I believe it should stay just as warm and inefficient on either system. I used to believe/say the 6s would be more efficient as the no-load speed is further away with 12s but this isn't true and the no-load speed is not static and the voltage changes applied to the motor with the throttle setting.  Half throttle gives half voltage and the no-load speed is half as well.  All the difference between the actual rpm and the no-load is is a reflection on how big that load is compared to what the motor can do.  A bigger motor will always be closer to its no-load
```

---
## \#79 Posted by: Namasaki Posted at: 2016-08-05T16:46:50.019Z Reads: 126

```
The motors where 230kv
```

---
## \#80 Posted by: Namasaki Posted at: 2016-08-05T16:51:48.924Z Reads: 124

```
[quote="Hummie, post:78, topic:4529"]
Less amps pulled from batteries but same current will go to motor.
[/quote]
How could you possibly pull less current form the battery and maintain higher current going to the motors?
That makes no sense.
The motors will pull less amps or current at higher voltage therefore drawing less amps or current from the battery.
```

---
## \#81 Posted by: Hummie Posted at: 2016-08-05T16:56:20.896Z Reads: 121

```
i believe the current to do the work and overcome the load will be the same with either battery and pull as much from the esc (at least the vesc) but at higher voltage the vesc bucks down the voltage effectively turning it to the needed amperage.  The volts don't move the motor just the amps.  The motor will get just as hot with either system...and they are just as efficient!?
Only the vesc and batteries benefit from higher voltage
```

---
## \#82 Posted by: Namasaki Posted at: 2016-08-05T17:02:47.372Z Reads: 120

```
I'm gonna end this argument now before another thread gets hijacked.
```

---
## \#83 Posted by: Hummie Posted at: 2016-08-05T17:17:16.035Z Reads: 123

```
  We can't talk about motors alone in a system.  There are variables relevant to the question.  a high kv motor will give u as much torque as the low kv if the battery can supply the increased amps and not sag. And the esc is important as it needs to be able to pass more amps with a high kv to get that same torque.  I'm just wondering if it's as efficient.  

Higher voltage batteries are more efficient as with less amp draw less sag and therefore more amps to release
Higher voltage for the esc I'm not sure as the vesc is said to be more efficient with higher voltage but when at half duty cycle an esc is less efficient than full duty cycle I believe.
```

---
## \#84 Posted by: SimosMCmuffin Posted at: 2016-08-05T19:10:38.685Z Reads: 121

```
[quote="Hummie, post:78, topic:4529"]
Less amps pulled from batteries but same current will go to motor
[/quote]

This makes no sense. Kirchhoff's current law dictates that the current coming to a point is the sum of currents leaving that node. If you're pulling 10 Amps from the battery it means that the 10 amps will be circulating in the motor. If the ESC pulls 10 amps from the battery, that 10 amps has to go somewhere.

> The total charge flowing into a node must be the same as the the total charge flowing out of the node

https://www.physics.uoguelph.ca/tutorials/ohm/Q.ohm.KCL.html
```

---
## \#85 Posted by: Hummie Posted at: 2016-08-05T19:12:51.288Z Reads: 115

```
There are two settings on vesc and other escs, current from battery and current to motor,  at low speed the voltage can become converted to amperage and u can run huge amps to the motor but have little draw from cells.  So I read on vedder's forum from Ren and Vedder
```

---
## \#86 Posted by: SimosMCmuffin Posted at: 2016-08-05T19:25:05.194Z Reads: 112

```
You need voltage to get amperage.
If volts go down, amps go down.
```

---
## \#87 Posted by: Hummie Posted at: 2016-08-05T19:31:56.608Z Reads: 114

```
Yea but u can have the same wattage at 50v and one amp as 1v and 50amps. 
I have to read the details of how it happens.  The proof is in the motor performance and will perform the same with either mixture into the esc.  Inductance is amps times turns. Volts aren't in the equation.  I'm sure I'm over-simplifying
```

---
## \#88 Posted by: devin Posted at: 2016-08-06T09:06:06.830Z Reads: 113

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#89 Posted by: jrpwit Posted at: 2016-08-06T09:48:12.045Z Reads: 106

```
I always thought that **larger motors, lower kv, gear ratio, and wheel size** gives more torque. For example with all Tacon motor users. We all know that the Tacon 245 and 295 motors have immense amounts of torque even though they have high kv. This was the exact reason why I go the Tacon 245kv. I wanted the speed and a good amount of torque. 

Also from read comparisons of hub motors, I believe the bigger the motor and lower kv equaling more torque factor still applies.

I just hate that the vesc has the 60k erpm limit currently.
```

---
## \#90 Posted by: Jinra Posted at: 2016-08-06T15:25:40.716Z Reads: 104

```
if you're looking for more speed there are other ways of increasing it. Going much higher in erpm is inefficient anyway.
```

---
## \#91 Posted by: Hummie Posted at: 2016-08-06T16:21:28.067Z Reads: 108

```
the size and strength of the magnetic interface between rotor and stator is the true determinant of torque so yea size is the real answer.  not the kv though because you can get the same amount of torque from the same size motor no mater how it's wound, either 245kv or 2450kv.  big motors can be wound to high or low kv. 
If running too small a motor without the needed torque of a larger motor the motor will show it's not up for the job by turning slower and getting hot, both.
```

---
## \#92 Posted by: devin Posted at: 2016-08-06T16:36:42.652Z Reads: 107

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#93 Posted by: Hummie Posted at: 2016-08-06T16:57:44.622Z Reads: 105

```
no just get sick of saying the complete explanation repeatedly.  I'm sure I've said it here 10 times!   the machine is asking me if I reallly want to be in this thread so much.  And if we're being sticklers your statement isnt correct either and you can keep the same cell size and voltage and get as much torque out of a higher kv if you adjust/increase your esc amp limit.
```

---
## \#94 Posted by: devin Posted at: 2016-08-06T17:06:36.339Z Reads: 106

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#95 Posted by: Hummie Posted at: 2016-08-06T17:13:14.533Z Reads: 109

```
i just jumped in and completed your misstatement that you need to change the voltage and size of the cell to compensate.  maybe you're misleading with your half statement and I'm here to correct you

i'm now wondering if there's any reason not to run a higher voltage always.  it seems more efficient across the board
changing only the kv will not change the torque a motor can produce as it's fixed based on size  You can change your torque to amp ratio though.  but now that it's been shown that the voltage effectively can be converted to amps to the motor at lower duty cycle by the esc I'm wondering if there's any reason to bother adjusting the battery voltage or kv ...it all seems to be converted by the esc to whats needed anyway
```

---
## \#96 Posted by: devin Posted at: 2016-08-06T17:25:47.279Z Reads: 109

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#97 Posted by: Hummie Posted at: 2016-08-06T17:39:08.903Z Reads: 112

```
that's a different discussion but have you seen the video overlay done using the vesc by vedder in which the amps from the battery and the amps to the motor is graphed in realtime?  It's pretty fair to say volts get converted to amp at lower speeds as there's simply less amps drawn from the battery and the motor is experiencing the amps to create torque.  This is how it was described to me by Ren and Vedder.  the analogy of a transformer was used.
https://www.youtube.com/watch?v=nGb-zt2Jp9k

I dont want to go into it again.  I'm passing on the info as it was given to me by both the designer and an expert of the vesc.  I've linked their quotes, I've quoted them.  if you want to tell people that it's not fair to view it as a transformer and volts are not being converted to amps when at a low duty cycle then you should tell them as I'm just passing on their words.
```

---
## \#98 Posted by: devin Posted at: 2016-08-06T17:45:46.614Z Reads: 108

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#99 Posted by: Hummie Posted at: 2016-08-06T17:49:33.114Z Reads: 105

```
plagiarizing?  I'm just passing on the words of the maker and expert.  as I said go tell them theyre wrong.
this isn't the place and I already did it for you.   and I keep telling u to go to vedders forum and talk there with them if what they are saying is wrong
```

---
## \#100 Posted by: devin Posted at: 2016-08-06T17:51:00.949Z Reads: 107

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#101 Posted by: Hummie Posted at: 2016-08-06T17:59:57.129Z Reads: 115

```
how bout instead of a long winded explanation we use math:



    Battery side: Power = Battery current * battery voltage
    --------------------------- 3.62 A * 33.2 V = 120.2 W

    Motor side: Power = Motor current * (battery voltage * duty cycle)
    --------------------------- 20.17 A * (33.2 V * 18.2 %) = 121.1 W

is this plagiarizing?  this is simosmcmuffin's simplification.   if you want to keep bringing this up at least do it in the thread.  dont forget chutney1 has added that this is just an explanation of volts converted to amps using duty cycle and there's other phenomena that are happening
```

---
## \#102 Posted by: evoheyax Posted at: 2016-08-06T18:01:24.282Z Reads: 115

```
Ok there's too much to read here to find the answer to this question. So yes or no, does a lower kv mean more torque?

My experience says yes. I have way less torque on my carvons (149kv) than hummies (80kv). Even from hummies 80kv to 90kv, I notice a difference in torque, especially when climbing hills that are steep enough to get them close to stalling.
```

---
## \#103 Posted by: devin Posted at: 2016-08-06T18:02:51.491Z Reads: 112

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#104 Posted by: Hummie Posted at: 2016-08-06T18:04:07.851Z Reads: 112

```
not a yes or no.  No as theres as much torque potential from a motor regardless of kv and size determines real torque.  just need to add more amps to the mix if it's higher kv.  thats it.  thats all there is to it.
```

---
## \#105 Posted by: devin Posted at: 2016-08-06T18:06:03.513Z Reads: 113

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#106 Posted by: Hummie Posted at: 2016-08-06T18:06:41.502Z Reads: 112

```
go jump in a lake!
```

---
## \#107 Posted by: devin Posted at: 2016-08-06T18:08:17.955Z Reads: 119

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#108 Posted by: Hummie Posted at: 2016-08-06T18:13:30.984Z Reads: 131

```
duty cycle equates to how long the voltage is on and then an average is formulated to find the power.
lol all round.  hooo hoo haha.  youre acting like a jerk off
```

---
## \#109 Posted by: devin Posted at: 2016-08-06T18:15:33.273Z Reads: 145

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#110 Posted by: jrpwit Posted at: 2016-08-06T22:42:46.281Z Reads: 150

```
I have though about that and assumed the same thing. High rpm is inefficient and it is avoidable. I played with the e-skate calculator a lot when I first started looking into electric skateboard stuff. Jason uses large 190kv motors, 10s, 83mm wheels, and 15 and 36 teeth pulleys. He gets to get 27mph top speed and all the torque anyone would want with a street skating board. I wanted to make a fast but torquey board  That was the whole reason I decided to go 12s, a large 245kv motor (Tacon 160 similar to Jason's motors) 83mm, and 14 and 36 teeth pulleys. I put a lot of though into it but didnt take into account the high rpm. I did think about it a little but couldn't find anything on the forum regarding high rpm. I am comparing a chain drive to a belt drive too for science and I dont want a belt breaking on me. I plan to just go 8s for normal use. At 8s I will be below 60k erpm, still have a top speed of 27 mph, and have a good amount of torque mainly from the larger motor and 14 tooth pulley. Jason did a very good job balancing the motor, battery, gear ration, and wheel size. At 8s I get the same top speed as Jason but he has more torque and lower erpm but my build can get more speed and the inefficacy high erpm. I live in a flat area tho so torque shouldnt be a problem. Cant wait to finish it! :slight_smile:
```

---
## \#111 Posted by: dan3s2020 Posted at: 2017-06-21T01:49:11.854Z Reads: 116

```
Torque=( I*V*Efficiency of the motor*60)/(rpm*2*3.14) so yes,but not always
```

---
## \#112 Posted by: thetechtrader Posted at: 2017-07-13T04:20:06.920Z Reads: 110

```
Alan, if I have two differet motors 500kv and 330kv, I set VESC amp limit to 50amps, and both motors are on 44.4volt 12S, and I limit the motors rpm to 4400RPM, the torque on both motors from a propeller would max out at 1998 watts for both because of RPM and amp limits, so am I correct in saying technically either motor would have same power here given same motor physical size of 56mm?

downsizing to the 330kv would save some extra wear and tear on bearings but thats about it??? correct?
```

---
## \#113 Posted by: lrdesigns Posted at: 2017-07-13T06:53:49.597Z Reads: 110

```
I recently switched from 5065 270kv motors to the same size 140kv motors with gearing so the top speed is the same. Power and torque feels similar but braking power is much stronger on the lower Kv motors. Not sure what that says but there is some difference. Though they are different brands so the motors are not exactly the same design.
```

---
## \#114 Posted by: pixelsilva Posted at: 2017-11-03T09:37:03.524Z Reads: 80

```
I'm getting 6030 type motors (between the 50XX and 63XX class sizes). Amp: < 50A; Rpm: 5100 (-+)5%; Volt: 36 VDC; Power: > 1600 W.

What is the KV of this motor?
```

---
