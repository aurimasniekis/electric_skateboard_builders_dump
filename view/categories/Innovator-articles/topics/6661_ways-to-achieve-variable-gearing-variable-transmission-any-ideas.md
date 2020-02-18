# Ways to achieve variable gearing (variable transmission). Any ideas?

### Replies: 23 Views: 3689

## \#1 Posted by: Okami Posted at: 2016-07-26T22:07:04.923Z Reads: 232

```
Hi there! 

So I got this idea in my head how well would it work, if one motor had let's say 3:1 gearing ratio, and the second one has, 2:1. Ideally, it could be implemented on a mountainboard - more room for different gearing ratios!

The scenario would be like this - there would be a control switch to just control one esc - one motor, once the ''first motor'' has reached its maximum usage, you switch to the second esc and fire up the second motor, which has more speed.. 

There might be some ''lag'' in between the first motor stopping and the second firing up.. but perhaps, with some advanced electronics this could be made to work..

Just an idea.. let's discuss this.. :slight_smile:

---
Since bicycles can get away with wider space for sprockets, there should be a way for eboards, too! 

Aim of this would be to just gear it, so the board can be started from a standstill.. then once optimum speed has been reached, the second motor would kick in / be started.

----

Would not suit most of the people.. probably totally useless for the ones who only goes 20kph / 15mph.. but still.. perhaps there are some mad ones, who would like to have 2 different gearings.  

<img src="/uploads/db1493/original/2X/0/0d92b6c6dd6fe96441a6be7a0995ed95bed55f80.png" width="250" height="250">
```

---
## \#2 Posted by: Jinra Posted at: 2016-07-26T22:12:13.186Z Reads: 223

```
@lowGuido Did something similar, though not exactly, with varying kv motors. The idea is to have one lower kv motor for torque and as speed picks up, the higher kv motor propels you faster. Not sure how it ended up working out.
```

---
## \#3 Posted by: torqueboards Posted at: 2016-07-26T22:14:35.809Z Reads: 224

```
Typically, your always as slow as your weakest link. So IMO it wouldn't work in the traditional sense.

Just like a 1:4 won't ever be as fast as a 1:1 ratio. Even if one is pulling the other and/or vice versa.

Unless, we can change gears like a bike then it's a bit difficult. We're always limited on the space we have available.
```

---
## \#4 Posted by: quanze Posted at: 2016-07-26T22:15:44.926Z Reads: 219

```
Dual rear pulley drive and dual front hubs omg lol think about it :3
```

---
## \#5 Posted by: Jinra Posted at: 2016-07-26T22:16:04.894Z Reads: 214

```
Carvon is doing this :)
```

---
## \#6 Posted by: torqueboards Posted at: 2016-07-26T22:19:16.560Z Reads: 209

```
[quote="quanze, post:4, topic:6661, full:true"]
Dual rear pulley drive and dual front hubs omg lol think about it :3
[/quote]

That would be doable as far as hill climb.

But I think top speed is still only limited to as fast as your "belt drive" can sustain.

Unless you can completely remove the belts and stop power to the belt motors.

Would be interesting though if someone knew how to make it work :)
```

---
## \#7 Posted by: Jinra Posted at: 2016-07-26T22:20:31.427Z Reads: 198

```
Why would it not work? You can go downhill faster than what your motor can provide on flats, so why wouldn't a separate motor be able to propel you faster than what your other motor can provide?
```

---
## \#8 Posted by: torqueboards Posted at: 2016-07-26T22:21:37.169Z Reads: 200

```
In a sense that would work. But you wouldn't be able to max out on your hub motor because the belt system is providing extra resistance.

Unless they are both capable of the same max speed but then what's the benefit? Just the 4WD aspect?
```

---
## \#9 Posted by: CSN Posted at: 2016-07-26T22:22:51.920Z Reads: 198

```
A CVT - continuous variable transmission allows for many ratios which could decrease the need for as large of motors.

It's been done in larger vehicles. Might work for E boards also.

http://www.forix.com/8w/altpower/daf55-transmission.jpg
```

---
## \#10 Posted by: maxchilton Posted at: 2016-07-26T22:34:44.073Z Reads: 188

```
[quote="Okami, post:1, topic:6661"]
The scenario would be like this - there would be a control switch to just control one esc - one motor, once the ''first motor'' has reached its maximum usage, you switch to the second esc and fire up the second motor, which has more speed.. 

There might be some ''lag'' in between the first motor stopping and the second firing up.. but perhaps, with some advanced electronics this could be made to work..

Just an idea.. let's discuss this.. :slight_smile:
[/quote]


umm... why?  Basically you have one motor working at a time while carrying two motors, two drivetains, two esc etc. 

Surely having two motors working in sync is faster in all aspects than one motor "geared for torque"  then switching to one motor "geared for high speed"
```

---
## \#11 Posted by: torqueboards Posted at: 2016-07-26T22:35:51.978Z Reads: 176

```
We can go all out in the $5k range lol

Could literally build a mini car for your feet.
```

---
## \#12 Posted by: Jinra Posted at: 2016-07-26T22:36:01.041Z Reads: 172

```
I think we're talking about different setups. I was referring to the design lowguido did with 2 varying kv motors, not carvons dual hub dual satellite config.

The main benefit would be achieving higher speeds while preserving low end torque. Since I have a dual diag config on my board, I might try this out sometime..
```

---
## \#13 Posted by: torqueboards Posted at: 2016-07-26T22:51:10.508Z Reads: 167

```
You'll get slightly better top speed and you'll have torque but it's never equal to the top speed KV and the high torque alone. It's more like in between. So IMO I don't think you'd get the best of both worlds. I tried it.. didn't work out that well. But don't let that stop anyone to try. More information is better then less.
```

---
## \#14 Posted by: Okami Posted at: 2016-07-26T23:18:12.963Z Reads: 165

```
[quote="CSN, post:9, topic:6661, full:true"]
A CVT - continuous variable transmission allows for many ratios which could decrease the need for as large of motors.

It's been done in larger vehicles. Might work for E boards also.
[/quote]


I suppose something similar happens in scooter (50cc) gearboxes, im not that technically / mechanically smart yet, but basically that is just what is called ''automatic transmission''. Is that correct?

Gears change when certain rpm/ speed has been reached.. 

So.. know the question would be - is it feasible to do it on such a small scale vehicle / construction size as an eboard? 

It would already work great if there were just 2 speeds.. It's actually why I started this thread - was wondering is it possible to make a ''gearbox'' for e-boards.. (again mountainboards might be better suited for this application because of their clearance / wider space for various parts.)
```

---
## \#15 Posted by: Okami Posted at: 2016-07-26T23:26:47.026Z Reads: 164

```
[quote="maxchilton, post:10, topic:6661"]
umm... why?  Basically you have one motor working at a time while carrying two motors, two drivetains, two esc etc. 

Surely having two motors working in sync is faster in all aspects than one motor "geared for torque"  then switching to one motor "geared for high speed"
[/quote]

I was imagining a situation where only one motor is working to sustain the needed power. I assume it could be better if 2 motors were working in sync with each other but it just seems that there will be times (high torque vs high speed) where both motors won't be able to work as efficiently, so that's why I came to idea to just using each motor for its best suited application, once the motor no longer is able to keep up, the second one takes the lead.. 

----
Plus, it seems tricky for me to make both motors to work in sync.. I am not quit sure how well it would work out if one motor was putting out more torque / more speed while the second one would put out less.. 

Perhaps someone with faulty motors / escs in dual drive system can comment on this.. always wondered do they really work 100% the same all the time.

---

3rd idea of mine - there is some sort of ''clutch''
---

 You engage this clutch when you need to change the gears, so there should be some sort of locking mechanism, which engages and disengages the ''extra gear'' from the motor (and also the main gear!)

This could work with just one dual shaft motor. There would be a need to extend the shaft probably but someone mechanically savy could perhaps figure this out.. there are people who spend countless hours fiddling with their gas/diesel cars all the time ;) .. actually same goes for eboards.. 

Not entirely sure how this might look from the benefit / financial side.. but there are different concepts in this world.. some work, some don't .. some are just in the middle.. not sure where this one goes ;)

-
```

---
## \#16 Posted by: Okami Posted at: 2016-07-26T23:59:53.874Z Reads: 162

```
Update:

Some good info here:


https://en.wikipedia.org/wiki/Transmission_(mechanics)#Electric_variable
>  Each driven wheel is equipped with its own electric motor, which can be fed varying electrical power to provide any required torque or power output for each wheel independently. This produces a much simpler solution for multiple driven wheels in very large vehicles.[...] 
--
It also improves the ability to allow different wheels to run at different speeds, which is useful for steered wheels in large construction vehicles.

That sort of suggests it could help with steering if the ''software'' would be optimized, to allow to choose a direction while holding the remote. 

This has already been implemented in one electic sports car (could be Mercedes, saw it on Top Gear). It was called ''power steering'' or something similar, car was turning more because the outside motor was spinning faster/stronger than the inside wheel

-------
Some more good info for ideas here:
https://en.wikipedia.org/wiki/Continuously_variable_transmission

---

Sorry for the very long replies.. I assume I just got enthusiastic about this concept / idea.
```

---
## \#17 Posted by: Okami Posted at: 2016-08-04T19:57:25.768Z Reads: 140

```
Found someone else has theorized about similar idea (on e-bike):

https://www.facebook.com/groups/684227311714643/permalink/823447191125987/

<img src="/uploads/db1493/original/2X/f/f3b68f96ebcf60dc1f79838c6390ab39ee0a0541.png" width="403" height="500">

<img src="/uploads/db1493/original/2X/c/c4578e0a64b7acb2f245117041e1774c6eb67798.png" width="478" height="445">
```

---
## \#18 Posted by: bill_f Posted at: 2016-08-06T00:26:15.744Z Reads: 131

```
I think this type of centrigugal transmission could be practical if you are working on a larger build like an e-mtb using a two stage gearing approach. https://www.sram.com/sram/urban/products/automatix
It will probably need to be adjusted so that it shifts at the right time since smaller skateboard wheels will have higher rpms compared to a bike wheel.
```

---
## \#19 Posted by: devin Posted at: 2016-08-06T01:05:08.362Z Reads: 126

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#20 Posted by: Okami Posted at: 2016-08-07T20:10:55.619Z Reads: 110

```
Yeah, gearing is more suitable for emtbs.. (off road, city, hard packed trails, standstill start and so on.. ) .. hard to implement on a small longboard.
```

---
## \#21 Posted by: Okami Posted at: 2016-08-07T20:12:02.893Z Reads: 112

```
Someone could try.. although have you seen those 100W buck converters? These things are huge.. (are used for driving 100w led chips).. not sure how big converter would look like for 1000w of power.. if you find anything, through it here.. [for fun]
```

---
## \#22 Posted by: Okami Posted at: 2016-11-27T21:11:35.977Z Reads: 85

```
Someone made a 2 speed chain transmission on his e-scooter:

https://youtu.be/Vr6SIEmcQsE?t=3m23s

I think this guy is quite smart.. he's only like 15yrs old or something.

Though, as can be seen in the video, the chain is relatively long.. would probably still be cumbersome to mount it on an emtb.. (also the thing that chain has to be positioned a little bit sideways is not that great.
```

---
## \#23 Posted by: Lutxipi Posted at: 2017-09-04T06:20:20.135Z Reads: 47

```
Hi there!; I have thought so long in all that issue you are talking about... and I thing I have "the answer"; but still haven't tried it:
"poket bike cvt gear box"
;-)
```

---
