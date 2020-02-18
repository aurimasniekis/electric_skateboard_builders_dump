# Does anyone ever build / use EV Controller to replace ESC?

### Replies: 13 Views: 2520

## \#1 Posted by: laurnts Posted at: 2016-02-11T10:11:53.391Z Reads: 98

```
So I've been wondering alot why we are not building electric longboard with serious EV controller similar to the one used on ebike for instance. I believe they are more ready product, made for the abuse and distance while price wise they're quite the same with VESC. Okay the size might be larger, but I believe it's all just about the case.

- How complicated it's to swap ESC with EV controller?
- How much part / components would be required to complete a running longboard?
- Can it still be controlled with standard G2TB / RC remote?
- How difficult? or what are the reasons why we're not doing it?

---

I've seen one nice company in US at least offering also FOC sensored ev controller with similar featured to VESC. They also offer sensorless one without FOC yet, but small enough to be fitted under longboard. They are also waterproof with configurable options.

Currently there is Alienpowersystem.com who already sells ev controller and there is also Kellycontroller.com that sells really wide variety range of EV controller. This doesn't include many more shady chinese ev controller manufacturer.

---

I'am asking because I would like to find another option for VESC replacement. I still consider VESC the best among other ESC, but for many reason it just simply doesn't feel robust / reliable enough yet. Repair is also really hard with components that are quite expensive and difficult with SMT method.
```

---
## \#2 Posted by: lowGuido Posted at: 2016-02-11T10:23:15.080Z Reads: 94

```
Because VESC 
--------------
```

---
## \#3 Posted by: Sebastiaan Posted at: 2016-02-11T10:40:19.297Z Reads: 94

```
There should be a case like the one often used in all varities for the raspberry pi.
Imagine that for the VESC, it would improve the durability.

I have no idea what an EV controller does in comparison with the ESCs used for eboards. Following this thread.
```

---
## \#4 Posted by: laurnts Posted at: 2016-02-11T11:14:21.913Z Reads: 92

```
I've seen some people convert RC PWM signal into EV controller using a servo and locked them together with EV Throttle input. Cheap working solution, but not elegant. Some uses Arduino to convert PWM input to output 0 - 5V to the EV controller which is quite nice.

I mean look at this EV Controller
http://kellycontroller.com/kbs48051x25a24-48v-mini-brushless-dc-controller-p-357.html

The spec are quite similar to VESC BLDC mode, even advance at some points.
Cost wise 79 USD, way cheaper than VESC.

---

For FOC sensored motor, can use this EV Controller
http://kellycontroller.com/kls4812s24v-48v120asinusoidal-brushless-motor-controller-p-1347.html
I mean look at the spec it offers, also dense with features VESC don't have, yet very robust.
Cost 149 USD, slightly more expensive than VESC.

---

At some point I don't mind having cable hanging around from my board if I need to go several days for several km. Reliability is my main concern. I just simply hate to stop in the middle of no where having no replacement parts / toolbox to fix my dead board.
```

---
## \#5 Posted by: lowGuido Posted at: 2016-02-11T11:29:49.913Z Reads: 86

```
so your issue is reliability? 
I have traveled close to 800km on my board and I have only ever had one break down. and that was from a PWM cable that vibrated loose.
```

---
## \#6 Posted by: laurnts Posted at: 2016-02-11T12:19:45.049Z Reads: 86

```
Not entirely because of reliability, but at least one of the aspect.

Well you could be a master builder that has great knowledge and abilities in making highly reliable electric longboard. You might be one from hundreds / thousands people who have only 1 problem over 800km. Experience does count as well, but trust me, there is a reason why this forum exist. Many questions, many issues in building an ideal yet reliable board.

I am not the only one who experience breaking a VESC, there are many others who are also experience builder who apparently broke them too by chance. In my perspective, at the moment VESC is the most fragile part within the build. In my perspective, the reason I go DIY is because of the swappability and ease of repair in case things gets broken. At the moment this is not entirely the case, especially in EU where VESC is not being produced / distributed here. Ordering new one took weeks - months, repair is not getting easier.
```

---
## \#7 Posted by: chaka Posted at: 2016-02-11T16:49:52.728Z Reads: 76

```
The VESC is actually very robust when built with quality control. I personally have never had one fail on me while riding. More often than not, failures are due to poor installation or manufacturing. 

Before I began manufacturing the VESC people had their doubts about the vesc due to an extremely high failure rate and virtually no quality control or support.  Some time has now passed and I think I have made it clear that with quality manufacturing and quality control the VESC was undeserving of it's unreliable reputation.

The simple fact is, with open source HW, if a distributor chooses to maximize profits by nickel and diming a manufacturer you are going to see a high failure rate with a circuit as complex as the VESC. This is something we should all consider when talking about open source hardware, we are going to see something similar to cheap knock-offs, etc....
```

---
## \#8 Posted by: elkick Posted at: 2016-02-11T17:06:09.009Z Reads: 69

```
I absolutely agree with that! No single failure here either and we have built a large number of VESCs recently. They even work well in non-esk8 related environments and setups. 

It's vital that the manufacturing process goes with the exact specifications and details of the BOM and this of course adds to the costs. But at the end youre buying a piece of HW which can be very relevant for your safety.
```

---
## \#9 Posted by: lowGuido Posted at: 2016-02-11T23:54:10.998Z Reads: 65

```
[quote="laurnts, post:6, topic:1318"]
Well you could be a master builder that has great knowledge and abilities in making highly reliable electric longboard. You might be one from hundreds / thousands people who have only 1 problem over 800km. Experience does count as well, but trust me, there is a reason why this forum exist. Many questions, many issues in building an ideal yet reliable board.
[/quote]

totally! this is true I believe that at least 90% of the problems brought up on this forum fall back to user error.
but what I don't understand is how will a different ESC stop user error? it can't
```

---
## \#10 Posted by: laurnts Posted at: 2016-02-12T02:44:09.059Z Reads: 64

```
Well I have my VESC from enertion and I only being able to ride on it for 7 minutes of 5 degree hill grade. It shut off when I was riding on it, so indeed it's very very uncommon scenario for many of you. When I look at the build quality, I was actually pretty impressed with the neatness and cleaness.

<img src="/uploads/db1493/original/2X/5/5a8ca0267b9afe84602d588dd2a589654ed9ee48.png" width="640" height="480">

Simply no signs of shorts / burn / not even a slight scratch on it. Well again this is might be one of a case scenario and this topic is not meant into discussing about VESC quality but more into another option of ESC to be installed. I'm curious if anyone think / would / already use it wether it's for longboard application or for other. However you guys definitely change my perspective into replacing VESC :smiley:
```

---
## \#11 Posted by: lowGuido Posted at: 2016-02-12T03:54:24.435Z Reads: 60

```
There are plenty of RC hobby  ESC available too if you dont want the VESC.
```

---
## \#12 Posted by: laurnts Posted at: 2016-02-12T04:08:22.902Z Reads: 61

```
Yes I am using one one HV ESC at the moment and simply sucked when there is no gradual brake. There are some which are quite good from castle creations / alienpower / etc, but theres no doubt that VESC is the best on this league. Vedder really put his words on it, trying to make the best ESC at this moment.
```

---
## \#13 Posted by: lowGuido Posted at: 2016-02-12T08:38:39.392Z Reads: 62

```
I have used the HK 150A car ESCs on a lot of my builds, and while I admit that quality was hit and miss (one or 2 just failed for no reason) the majority of the them have been going strong for over a year. the VESC is a better product no doubt. but I have built many boards with the hobby ESC with good results.
```

---
