# Downhill Assist Board

### Replies: 37 Views: 2040

## \#1 Posted by: Jreamer Posted at: 2017-10-07T04:21:46.639Z Reads: 228

```
So I feel like the best part about esk8 is the brakes. When downhill longboarding breaking is not an option and I had the idea of an esk8 board and it's main purpose is to roll smooth, fast, and provide a break at high speed. 

So that's the idea. A downhill board that provides breaks. Is it possible?

Maybe high KV hub motors with ceramic bearings with vesc?

Is this crazy?
```

---
## \#2 Posted by: willpark16 Posted at: 2017-10-07T04:29:43.719Z Reads: 225

```
Small a123 pack and some decent hubmotors should do the trick, you will need cells that can handle high regen current for stronger braking without damaging the cells
```

---
## \#3 Posted by: Jreamer Posted at: 2017-10-07T04:32:14.063Z Reads: 220

```
What hub motors?
```

---
## \#4 Posted by: willpark16 Posted at: 2017-10-07T04:33:51.726Z Reads: 214

```
I'd say carvon they aren't hub motors but they have nearly the same resistance as hub motors which is to say minimal and they allow swappable wheels
```

---
## \#5 Posted by: Jreamer Posted at: 2017-10-07T04:38:29.016Z Reads: 200

```
So should I get custom carvon hubs? Like high KV hubs so they are within their max speed at like 40-50mph? Do they freewheel well?
```

---
## \#6 Posted by: willpark16 Posted at: 2017-10-07T04:40:15.567Z Reads: 190

```
They can freewheel and 149kv hubs which are their v2s is what you'd want sadly they are no longer made
```

---
## \#7 Posted by: b264 Posted at: 2017-10-07T04:45:55.689Z Reads: 184

```
You won't need cells at all, or even a battery.  It will be a one-of-a-kind build though.  You will need a power resistor on a heatsink instead of a battery.  

Edit: the controller will need a battery
```

---
## \#8 Posted by: onepunchboard Posted at: 2017-10-07T05:16:42.295Z Reads: 181

```
I know a guy who makes a clip on hubmotors at the back of board. it's for going up hill and detach it  put in bag and down heal like normal board. 

I guess it can use as braking system. 

problem with this prototype is, getting enough contact of hub motor, but this resulted too much stress on motor and thane.
```

---
## \#9 Posted by: pat.speed Posted at: 2017-10-07T06:20:39.836Z Reads: 162

```
I think that could work a small remote with one button which connects the phase leads of the hub motor together. This would be very simple and not very expensive. It will free wheel and brake but you won't actually be able to accelerate or anything it will essentially just be a skateboard with a brake
```

---
## \#10 Posted by: Jreamer Posted at: 2017-10-07T06:23:40.474Z Reads: 157

```
This sounds exactly what I am looking to do! Downhill for beginners!
```

---
## \#11 Posted by: b264 Posted at: 2017-10-07T06:47:48.234Z Reads: 151

```
In fact you could even get rid of the controller and esc and all that and just have a wired remote that is one button.  Although you can't just connect the phases together, you need to connect them through a [resistor on a heatsink](https://www.digikey.com/product-detail/en/te-connectivity-passive-product/TJT5003R3J/A123917-ND/5878238), probably under the board or on the truck or something.  That one will dissipate about 392 watts at 11 amps on a 36 volt load and costs $57.63.  
  
The one thing that does not address, is that as soon as you hit the button it'll prob throw you off because it won't be a gradual application of brake... so...

Plus you'd have to see how many volts is coming out of the motor.  You're probably better off using an esc and a regular controller, but you will still need either a battery to store the energy or a power resistor to burn it off as heat
```

---
## \#12 Posted by: Jreamer Posted at: 2017-10-07T06:51:11.467Z Reads: 129

```
I'm thinking a vesc with a super small battery just to take the juice.
```

---
## \#13 Posted by: b264 Posted at: 2017-10-07T06:54:51.662Z Reads: 132

```
That sounds a bit dangerous if the batt gets full.  You could make a really simple circuit that bleeds off extra juice though through a smaller and cheaper resistor at a much slower rate
```

---
## \#14 Posted by: Acido Posted at: 2017-10-07T09:32:06.119Z Reads: 124

```
Why just not mount some discs on the wheels?
```

---
## \#15 Posted by: b264 Posted at: 2017-10-07T10:00:53.983Z Reads: 120

```
Look at the big brain on Acido.  Us in here totally overthinking this :smile:
```

---
## \#16 Posted by: Jreamer Posted at: 2017-10-07T10:36:08.858Z Reads: 122

```
Look at the big brains on this guy disc breaks, genuis
```

---
## \#17 Posted by: BoostedBuilder Posted at: 2017-10-07T10:41:08.384Z Reads: 117

```
Have you not considered this? https://www.kickstarter.com/projects/search?utf8=✓&term=Longboard+brakes
```

---
## \#18 Posted by: Acido Posted at: 2017-10-07T11:15:04.667Z Reads: 119

```
I assume the only problem would be the hydraulic pipes
```

---
## \#19 Posted by: Namasaki Posted at: 2017-10-07T12:48:39.783Z Reads: 123

```
I have run carvons v2 and in my opinion they didn't free roll any better than my current belt drive using 9mm belts. 
The main concern I would have is the erpm limitation of the Vesc. 
If I'm not mistaken, you can exceed the erpm limit while coasting and blow the drv leaving you with no brakes. So you would have to keep your downhill speed within the erpm limit which a 14 pole motor is 8571 rpm
Direct drive would be the best at keeping erpm low. 
According to my speed Calc, this looks doable. 
<img src="/uploads/db1493/original/3X/1/6/16beffec6741bbf0fe636b10ba14f7c7ad6bb95b.PNG" width="281" height="499">
```

---
## \#20 Posted by: chaka Posted at: 2017-10-07T14:19:47.123Z Reads: 112

```
Why not foot brake or coleman slide. I use electric for downhill assist but not for the brakes. 

The question about overrunning the ERPM is a good one, you have to be carefull with that. One thing I do is keep my throttle fully engaged when hitting my top speed while going downhill. With the throttle engaged as you reach your top electrical speed you will feel the motors produce drag to keep the speed from increasing any further. If you let off the throttle the motors will free wheel and you could overrun the ERPM
```

---
## \#21 Posted by: michichopf Posted at: 2017-10-07T16:00:11.358Z Reads: 108

```
Well, I am intrigued by your Idea for science, BUT you are talking about 45mph downhill. (just as a reminder 30mp/h is enough to be lethal). 

I myself tried to mesh the  worlds of esk8 and downhill for years now. Taking my Raptor 1 and DIY builds on trips and mountain passes. 

So I would reccomend against it heavily, here is why.

1;) Wheels. When I go over a certain speed I like to know my wheel, also I prefer 72/73mm for serious riding than anything above 80mm+. So sure mayby carvon speed drives with 72mm wheels could be possible but hard to find.

2.) Trucks. I am a ronin pro rider. I cannot for the life of me change trucks, everything else feels so weird and I am instantly scared (during downhill sessions). This maybe very personal but as a carvon owner, those trucks have nothing to do with Precision RKP trucks. 

3.) Roll resitance. It is minor the resistance one would think with hubmotors or carvons. I actually compared them on my favourite local hill (pretty mellow but amazing ride). Normal set up tucked trough 64km/h, with carvons 51km/h /even though the added weight of the whole set up should actually help on a long donwhill slope).

4.) Cost. Normally during summer a set of wheel lasts me about 2-3weeks (3-4 sessions a week), then its relegated to a "fun" wheel or for freeriding. So hubmotor wheels don't come cheap, and they cannot take much. A few botched slides or an emergency slide and well they are done. With carvons you can ride abecs wich makes it better but still crazy expensive.

5.) Trust. If I were to be going 45mp/h I would never for the life of me trust in brakes, at those speeds I am wearing my leathers, fullface etc. But then trusting for the brakes to make it easier ? hell no.

6.) Logic. If your bottleneck is your ability to stop and you want to circumvent that with an E-brake... I am worried to say the least. At those speeds, stopping should not be your major concern. I mean going into corners you are almost on the pavement anyway, drifting, speed checking and then gripping trough when you can. 

7.) I am nowhere skilled enough to squad or even stand up at those speeds, So I am grabing my board and putting my pucks down, so the remote was allways a hassel. I mean if you stop wearing pucks to hold a remote you aren't locking for a serious ride / challenge anyway. 

8.) I once tried to brake with my carvons at 65+km/h, the sound and how weird it felt was enough for me once. Never again.

My experience was that for one you are so much slower, it is alot more expensive and the set up in which you trust your life into is so much worse. Then the brake only comes in handy on long straights where you exeed your comfortable speed limit, But air braking or a speed check are sufficent. I fried vescs and had some suuper sketchy moments trying to downhill on an esk8. I think that those 2 worlds are too far apart (racing and esk8 has me exited though). 

I my experience invest in a sick DIY buill, go high KV and big gearings if it is the speed you are after. And keep riding downhill like you should, gravity style without any gimmicks. Best for both worlds and alot more joy in the long run,
```

---
## \#22 Posted by: Idle Posted at: 2017-10-07T16:15:38.572Z Reads: 89

```
<img src="/uploads/db1493/original/3X/3/f/3fac9f18442d57a4190851158bb715187ab1b7c5.JPG" width="627" height="500">

https://www.networldsports.com/speed-chute.html?gclid=EAIaIQobChMInqmy9_Pe1gIVxB-GCh2owATAEAQYASABEgI-3vD_BwE
```

---
## \#23 Posted by: Michaelinvegas Posted at: 2017-10-07T16:35:13.618Z Reads: 87

```
[quote="Jreamer, post:1, topic:35005"]
provide a break at high speed.
[/quote]

This almost sounds counter intuitive on Esk8.
```

---
## \#24 Posted by: faithfulpuppy Posted at: 2017-10-07T18:32:30.959Z Reads: 85

```
i'm sorry but i disagree with this.  You should not be launching yourself downhill at speed on a longboard without any idea of how to slow down safely (without external assistance). There is no "downhill for beginners," because that's just an easy way to get hurt. learn how to slide a board and do it the traditional way.

really, even with esk8, you shouldnt be pushing your board to 30+mph if you've never fallen off an unpowered longboard at 20mph or slid a board to a stop safely.  Learn basics before trying to brake the damn land speed record.
```

---
## \#25 Posted by: psychotiller Posted at: 2017-10-07T18:40:38.409Z Reads: 83

```
You could easily mount discs to my sixshooter wheels.
```

---
## \#26 Posted by: Jreamer Posted at: 2017-10-08T02:44:18.769Z Reads: 78

```
how would that work?
```

---
## \#27 Posted by: psychotiller Posted at: 2017-10-08T02:47:50.933Z Reads: 81

```
We would just need to make discs to fit the standoffs 

<img src="/uploads/db1493/original/3X/a/b/abff336c1b8da1a518b5ca1e37a1cac11aa3c869.jpg" width="690" height="331">

<img src="/uploads/db1493/original/3X/3/2/32a6f2236635091aebf00a73198b6c8f4fb855e1.jpg" width="690" height="331">
```

---
## \#28 Posted by: Jreamer Posted at: 2017-10-08T02:48:53.366Z Reads: 79

```
Could you build a whole break system to mount to a longboard?
```

---
## \#29 Posted by: psychotiller Posted at: 2017-10-08T02:50:31.099Z Reads: 76

```
I'm pretty busy as it is...But I't not out of the question.
```

---
## \#30 Posted by: Jreamer Posted at: 2017-10-08T02:52:25.251Z Reads: 74

```
No worries, just a brain teaser atm. Maybe around spring time we can come back to this :)
```

---
## \#31 Posted by: psychotiller Posted at: 2017-10-08T02:54:27.346Z Reads: 77

```
MBS uses a reverse V brake. It could be done the same way with my hubs too being that the wheel beads are aluminum. One would just need to figure out how to mount v brake calipers or reversed single sided hydraulic calipers and pads to the hanger.

Instant brakes.
```

---
## \#32 Posted by: Schulerbible Posted at: 2017-10-08T04:53:49.593Z Reads: 66

```
<img src="/uploads/db1493/original/3X/6/0/603a58d7b62c91ca1052b6cd50678beaed4f3274.png" width="630" height="420">
```

---
## \#33 Posted by: b264 Posted at: 2017-10-08T05:04:55.570Z Reads: 64

```
Why not just have a little anchor you can toss off the side of the deck
```

---
## \#34 Posted by: Jreamer Posted at: 2017-10-08T05:24:50.654Z Reads: 60

```
wish they where bigger trucks. 150mm.
```

---
## \#35 Posted by: psychotiller Posted at: 2017-10-08T05:26:59.370Z Reads: 63

```
Skateboardstabilizor sells those I'm guessing!
```

---
## \#36 Posted by: GrecoMan Posted at: 2017-10-08T12:06:38.914Z Reads: 60

```
Yea man you’ve gotta slow down somehow.  His hubs will push 1,200mph!
```

---
## \#37 Posted by: b264 Posted at: 2017-10-10T16:34:17.800Z Reads: 46

```
Look at this; it has [disc brakes](https://brakeboard.com/)
```

---
