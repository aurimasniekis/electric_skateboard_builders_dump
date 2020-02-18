# VESC - is pushing the board good or bad?

### Replies: 40 Views: 2825

## \#1 Posted by: yaca Posted at: 2016-10-10T15:34:50.177Z Reads: 314

```
I like to know if pushing the board for longer distances is ok or not. I think it should not be a problem if the VESC can regenerate to the battery, isn't it? But what will be happen if I turn off the board and the VESC can not feed the battery?
```

---
## \#2 Posted by: IDVert3X Posted at: 2016-10-10T15:47:05.852Z Reads: 311

```
Nothing. There will be only small mechanical resistance. That's all.

Just be aware: that the faster you go - the higher the voltage on the motor will be.
If it reaches certain ( high ) voltage, it can blow up your ESC. That's not very likely tho.
I don't know how VESC works, that's just my general knowledge of motors.
```

---
## \#3 Posted by: Hummie Posted at: 2016-10-10T16:00:34.197Z Reads: 295

```
The motors will turn on the vesc if they are connected.  If the batteries aren't connected and u ride that's very dangerous as the motor energy will either ruin the vesc or slam on ur brakes.   Keep batteries connected if pushing.
```

---
## \#4 Posted by: yaca Posted at: 2016-10-10T16:05:14.872Z Reads: 282

```
Thank you, that's what I thought. So I will have my batteries connected if pushing.
```

---
## \#5 Posted by: treenutter Posted at: 2016-10-10T16:56:19.095Z Reads: 266

```
[quote="Hummie, post:3, topic:10912"]
If the batteries aren't connected and u ride that's very dangerous as the motor energy will either ruin the vesc or slam on ur brakes
[/quote]

@Hummie Do you have a sense of how much speed (and for how long) this would require? My impression (and it could  be totally wrong) is that the energy generated and delivered from the motor is pretty small.
```

---
## \#6 Posted by: IDVert3X Posted at: 2016-10-10T17:02:41.889Z Reads: 259

```
Everybody should learn at least Ohm's law...
Guys, there is no energy that "has to go somewhere".
```

---
## \#7 Posted by: Hummie Posted at: 2016-10-10T18:25:33.258Z Reads: 243

```
The motor will generate enough going even over 5mph it can slam on it brakes.  That's if ur lucky and it doesn't blow up ur stuff. Or maybe in my case it was better.  Happened a couple times to me before I found out what was up.  The energy has to go to the battery or else it's forced to dissipate in the esc and poof
```

---
## \#8 Posted by: Jinra Posted at: 2016-10-10T18:44:31.839Z Reads: 234

```
I'm not convinced on the large danger of this. While I agree it can create some electrical activity in the motor. I don't think it creates enough to damage anything and will most likely dissipate that energy as heat. 

I suppose someone could disconnect the phase wires and hook them up to a meter to measure current and voltage through them when traveling.
```

---
## \#9 Posted by: IDVert3X Posted at: 2016-10-10T18:49:49.991Z Reads: 226

```
There is a voltage on the motor, no magic energy flowing out of it.
If there will be any current ( energy flow ) depends only on the ESC itself.
There don't have to be any current ( open circuit ) and motor can spin freely.
Or there can be very small current just to keep the VESC running ( unnoticable for you as a driver ).
Energy is produced only if the motor is converting kinetic enegy to electron flow - it don't have to do it.
Once it does, you can feel it ( you loose your momentum ) - it can be really small so you won't notice it.
If it breaks - then there is problem. Breaking means most of your energy is transfered to the flow of the electrons and if that happens, there is a huge current flowing through the ESC that can burn it.
That's it. 
It's not like water or anything that has to go somewhere and get stored. You CAN'T store electricity.
You can transfer it to chemical energy ( battery ) and than the other way around once needed.
Electricy is movement of electrons inside the wire in a loop. Those are the basics of electricy.

So, will it blow your ESC? Really depends on how it's designed.
I don't know how VESC circuitry works, but what causes damage is the current flowing through something.

I won't recommend doing that anyway.
```

---
## \#10 Posted by: Hummie Posted at: 2016-10-10T19:13:31.949Z Reads: 207

```
Check vedders site on the details of how much energy is produced when coasting and no batteries and when it will ruin the vesc.  I had brakes slam on at 6mph
```

---
## \#11 Posted by: Spek Posted at: 2016-10-10T19:45:49.028Z Reads: 194

```
Is all of this discussion referring to riding with a dead or turned off battery, then? When the system is on there should be no issue at all, and it's totally fine to coast at high speeds, right?
```

---
## \#12 Posted by: Hummie Posted at: 2016-10-10T19:53:34.935Z Reads: 187

```
Referring to having a battery connected.  If the motor is connected to the vesc  it will power up regardless of if there are batteries attached.  If there are no batteries attached it's dangerous
```

---
## \#13 Posted by: yaca Posted at: 2016-10-10T19:55:03.657Z Reads: 182

```
The only problem I see with connected battery is if the battery is completely charged and you additionally generate energy into the battery while pushing for longer distances, so you can overload it.
```

---
## \#14 Posted by: Hummie Posted at: 2016-10-10T19:56:24.964Z Reads: 177

```
You don't charge by pushing only braking. Going down a hill and braking with full charge u can overcharge the battery
```

---
## \#15 Posted by: Spek Posted at: 2016-10-10T19:57:32.869Z Reads: 175

```
Ok cool. Who's gonna push with a full battery, anyway? :p
```

---
## \#16 Posted by: IDVert3X Posted at: 2016-10-10T20:00:06.824Z Reads: 171

```
@Hummie:
Exactly. Actually, you do transfer little bit of your momentum to electricy so the VESC has some power to operate, but that's unnoticable. The moment when the ESC allows electrons to flow and convert mechanical energy ( your kinetic energy transfered to motor shaft ) to the electrical energy is when you break. And this electron flow can either go to the battery / capacitors or short something out in the ESC ( if it's badly designed ).

@Spek:
Yup. Even if you went the hill up and then back down, you would still generate much less energy than you used to get up.
```

---
## \#17 Posted by: yaca Posted at: 2016-10-10T20:05:33.365Z Reads: 163

```
That's good! So I can push my board with unconnected battery but I'm not allowed to use the break, right? Oh, I forgot it is not possible to break with unconnected battery.
```

---
## \#18 Posted by: Hummie Posted at: 2016-10-10T20:09:34.986Z Reads: 158

```
No.  must have connected battery if ur vesc is connected to spinning motor and ur pushing
```

---
## \#19 Posted by: yaca Posted at: 2016-10-10T20:11:32.903Z Reads: 155

```
OK I understand. I can not push it without battery because it's still dangerous for the vesc, right?
```

---
## \#20 Posted by: IDVert3X Posted at: 2016-10-10T20:14:48.389Z Reads: 152

```
Nobody actually knows how the VESC works in a detail ( well, Vedder does ).
You should be fine just pushing it ( not using breaks ), but noone is gonna guarantee that.
Neither me.

Do it at your own risk, in theory, you should be fine, but in reality? You will have to find it out!
```

---
## \#21 Posted by: Hummie Posted at: 2016-10-10T20:19:21.123Z Reads: 146

```
It's been said specifically that the energy produced when just pushing and not having batteries attached will ruin ur stuff quickly.  Check vedders site
```

---
## \#22 Posted by: IDVert3X Posted at: 2016-10-10T20:42:36.216Z Reads: 142

```
You said many times "check vedder's site" - post the link, please. I can't find it.
I'm really interested to see what's the problem that causes that.

My theory ( again, THEORY, I don't know how it works, that's why am I asking you for the link ):
Motor is spinning => You get voltage on it's terminals => there is no ( or very small ) current => Voltage can rise easily => Voltage reaches cricital level ( at certain speed ) => something on the board can't stand ( no longer works as an insulator, voltage barrier is broken ) => high current flows ( short circuit ? ) => component(s) get damaged
```

---
## \#23 Posted by: Hummie Posted at: 2016-10-10T21:03:36.772Z Reads: 131

```
http://vedder.se/forums/viewtopic.php?f=6&t=277&p=1732&hilit=braking+disconnected+battery#p1732
```

---
## \#24 Posted by: IDVert3X Posted at: 2016-10-10T21:11:15.334Z Reads: 126

```
Thank you!

So the general advice then sounds: unless you break or go crazy fast, you should be fine.
```

---
## \#25 Posted by: Hummie Posted at: 2016-10-10T21:11:46.385Z Reads: 124

```
no.  if you push the board without a battery attached you will blow it up!

braking without the battery should set off the high voltage limit and nothing will happen, hopefully.   no brakes will happen for sure.  but pushing without brakes is still enough to ruin the vesc.  In my experience it slams on the brakes.
```

---
## \#26 Posted by: IDVert3X Posted at: 2016-10-10T21:15:30.825Z Reads: 123

```
> With no battery is bad: if you brake, the voltage on the bus-line will rise very quickly, possibly causing over-voltage-damage before the VESC notices that something is wrong. 

> So without a battery, the accidental brake command will quickly fry the VESC (as long as you're moving). When going down a hill faster than the unloaded speed, the NO brake commanded situation is the worst.....

> Turning the VESC off isn't going to last long: The motor will power up the VESC. Then if you somehow activate the brake... you're toast.

There is no reason why it should get blown up when breaking is not applied. There is just no current that coud damage something unless you allow it to flow ( using breaks ).

If the VESC starts to break itself without a battery, then you have a big problem.
```

---
## \#27 Posted by: Hummie Posted at: 2016-10-10T21:15:53.969Z Reads: 115

```
read the link i linked.  o wait it's not there.  let me find it
```

---
## \#28 Posted by: IDVert3X Posted at: 2016-10-10T21:21:15.572Z Reads: 119

```
I read it and pasted few quotes there already.
Basically what they said is that if you break or go crazy fast, you can damage it.

Also:
> So, with a bad reciever connection to the vesc I have gotten extreme unwanted brakes with no battery connected

So if your receiver tells the VESC to break ( by a mistake ), it will break and you know what happens.
```

---
## \#29 Posted by: Hummie Posted at: 2016-10-10T21:27:28.462Z Reads: 114

```
maybe you're right.  i thought i'd read somewhere on there otherwise.  how much current does flow with coasting and no batteries?  is it limited?  there's some current flowing to get it to light up..but too much would be too much no?
the quote you put in is me.  maybe thats why I assume it's bad because it's thrown me a couple times with the bad receiver
```

---
## \#30 Posted by: IDVert3X Posted at: 2016-10-10T21:31:22.937Z Reads: 109

```
I = U/R.
If battery is disconnected, there is infinite R.
But there is a microcontroller and other things that require some small amount of power ( a lot of R ).
Remember, the higher the R, the lower the current.
So if no breaking is applied, you got maybe 30mA ( I don't know, I'm guessing! ) of current that is used by the board itself.

Once you break, you probably get short circuit somewhere due to too high voltage and that means a lot of current is transfered directly to the heat = bye bye your VESC.

I can't really tell you anything more, I don't know how the VESC works.
```

---
## \#31 Posted by: Hummie Posted at: 2016-10-10T21:46:29.618Z Reads: 108

```
i understand you with the ohms law but with the motor increasing in speed and building a greater voltage...at some point the resistance of the esc maybe isn't enough and too much current will run though?  you say you don't know the vesc in particular but i imagine at some point this will happen.  but the more I read the more I'm not finding what I said before and the vesc will not die being pushed without a battery.  just braking
```

---
## \#32 Posted by: IDVert3X Posted at: 2016-10-10T21:49:14.765Z Reads: 105

```
Well, if you go crazy fast ( like really crazy ), the motor can generate higher voltage than the semiconductors on VESC can handle and they will became conductors. In that moment, your VESC is dead. But the same can happen even if the battery is connected ( just smaller chance as the voltage will be smaller thanks to the load - the battery ). So this is a different story.

Its almost midnight where I live, better gonna sleep.
Take care.
```

---
## \#33 Posted by: Hummie Posted at: 2016-10-11T00:10:49.463Z Reads: 100

```
Thanks for breaking it down.   

With the fets, the transistors, they open or close the current, ..when the board is coasting it lights up, so there is a current coming through and u say it's very small, is it through programming that the current will be limited to maybe 30 mah and it will stay at that current until the fets voltage limit is broken, or does ohms law dictate the current increases with the voltage? A fixed resistance. 

Which brings me back a step, what decides how much current is let through?
```

---
## \#34 Posted by: im-done Posted at: 2016-10-11T00:16:40.170Z Reads: 101

```
Hummie is correct! i used to push with the esc off and it would pop on and throw me off. when magnets pass over windings like in a motor it creates electricity. that can power on the esc. you can test this by taking the 3 phase wites from your motor and grounding them all together. than spin the wheel by hand and you can feel the power stall the motor. make sure you have the motor disconnected from the esc and any other electronics.
```

---
## \#35 Posted by: IDVert3X Posted at: 2016-10-11T06:57:56.130Z Reads: 98

```
There is only as much current as is needed, unless there is a short circuit. When you break, the current goes thourgh the battery and it charges it. When there is no battery, VESC somehow redirects the current through itself ( I dont know, just guessing ) which probably ends up in a short circuit ( very small resistance, high current flows ) which destroys your VESC.
```

---
## \#36 Posted by: danyCRO Posted at: 2019-05-24T19:45:52.953Z Reads: 37

```
Hi. I am pushing with connected batterys, but when my battery was near to empty - only 4% left, on pushing my motor blocking and I almost crash. I was repeated 2-3 times to test.. Is that means that 4% left of baterry means that battery are empty (in that moment) and lose contact?
```

---
## \#37 Posted by: Hummie Posted at: 2019-05-24T20:31:23.016Z Reads: 35

```
xxxxxxxx. No idea
```

---
## \#38 Posted by: danyCRO Posted at: 2019-05-24T22:10:51.376Z Reads: 31

```
I have now dual FS vescs and FS motors with 6S batterys. But similar thing was happened before with my single chinesse motor and chiping vesc..
```

---
## \#39 Posted by: Schulerbible Posted at: 2019-05-24T22:31:37.986Z Reads: 29

```
I am running a Raptor 1 DIY build since many years and I regular push with the battery switched off (longest was 3 miles). Never had any problem and I am running Enertion Vescs (not the focbox).
```

---
## \#40 Posted by: Hummie Posted at: 2019-05-25T01:49:37.797Z Reads: 20

```
as long as you have a battery connected youre supposed to be fine.
```

---
