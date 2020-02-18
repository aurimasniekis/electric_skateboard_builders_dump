# 1st time build for heavy rider

### Replies: 11 Views: 1054

## \#1 Posted by: Weirdboards Posted at: 2017-09-23T16:50:30.848Z Reads: 166

```
Wanted to get some additional thoughts on my first build. My side hustle is building custom longboards, and i wanted to try my hand at an eBoard for myself. But right now I am riding at a heavier cruising weight (265lbs) than normal, and I live in a development with 20-30% grade hills. I have done a lot of research and come up with the components that i think should give me the best balance of speed, torque and weight capacity, but I would love some feedback from those with a little more experience to reinforce my choices. Everything is on order, but parts can be returned and exchanged if needed. 

here is what I am building. I call it the "Fat Jesus":

- DRD (dual rear diagonal mounted) Turnigy SK3 168kv 6374 Aerodrive motors
- 10s Turnigy Graphene 10,000mah 15c battery (matching spec 4S+6S)
- 15mm belt with 15/36 tooth ratio
- Dual VESC
- wireless remote 2.4ghz
- 97mm bigfoots
- caliber 10" trucks 

Still designing the board, but will likely be 38-42". 

The online calculators factor for motor efficiency when calculating top speed, so at 80% I should be looking at 21-ish mph. Which is fine for me. 

My first question is how much does weight diminish overall top speed? Is there a way to calc rider capacity for a given speed range using these numbers?

Second is of course, can I expect a decent ride (carving/cruising flat land, some hills in and out of my neighborhood)?

Third, what is the best charger to use in a set up like this? & how do you display battery life remaining?

Lastly, Would love opinions on what has worked for battery cases on the deck. Worst case, I am going to get some sheet aluminum and make a box. Thoughts?

Thanks All!
```

---
## \#2 Posted by: Okami Posted at: 2017-09-24T17:33:02.492Z Reads: 135

```
Looks like u have good choice of components.

Not sure about hills as i live in non hilly place but i assume u should still get up.to.them.

As about range, there was this one extra calc
www.esk8.today
But u should lower the capacity as u.dont want to drain your pack competely empty. Also calculating range including going uphills might be.a bit.hard, i suspect going.up hill might take 2.5-3x times more energy at least, compared.to flats, depends on how steep and long are these hills.

As about batt indicator - most handy ive come up is percentage display, if u got some extra.money / space i would suggest to look into "energy meters" / power analyzers. They can also be found as coulometers, these will show more precisely how much energy is being consumed and how much is left but might be a bit.more difficult to set them up (requires main power wires.going.through them)

Hope this helps, looks like uve researched quite enough so far on your own ;)

If possible. I would.maybe go with focboxes instead of regular vesc, since they seem to be more durable / robust

Charging is another story dont wanna go into that too deep here, your best bet might be to.get dual charger, since u cant really parallel charge, if u choose 6s and 4s batt. One more option is buy standalone 10s charger or install bms and then find suitable psu for that (though bms install and good functioning might be problematic)'
```

---
## \#3 Posted by: bigben Posted at: 2017-09-24T18:01:45.051Z Reads: 124

```
How are you thinking of mounting the motors to the trucks? I have gullwing sidewinder 2s and use evolve hangers and mounts.
I've made a few fibreglass enclosures and sell them if you're in the eu. If not there are a lot of 3d printable designs or abs enclosures available. I used a rosti mepal sandwich box at first.
For the batteries I think 15c batteries are a little under spec for the demands of e skate. I've recently got the parts together for a 10s pack by buying 5 of the 2s graphene packs which are rated to 90c.
```

---
## \#4 Posted by: BigBoyToys Posted at: 2017-09-25T21:59:29.633Z Reads: 97

```
Id steer away from dual diagonal if you dont want your board steering away from you. The amount of torque required to accelerate guys our weight  will steer the trucks in the direction opposite to the side the motor is mounted. I think you do need dual 6374's or atleast dual 6364's  but how about mointing them on Torqueboards 218mm extended caliber clones as a dual rear drive? You pretty sure you could at least fit dual 6364 on those trucks they are plenty long.

I think the 10AH 15C Graphene batts will do. Those should be good for 150A, your dual Vescs would probably overheat before the battrry does.

I would also recommend you go with 10 or 12 S. Youll can draw draw less amps with the higher voltage battery and acheive the same topspeed wiith a lower KV motor which will provide you with more torque as well.

Just my thoughts as a 280lb rider.
```

---
## \#5 Posted by: Namasaki Posted at: 2017-09-25T22:35:29.127Z Reads: 93

```
[quote="Weirdboards, post:1, topic:33787"]
DD (dual diagonal mounted) Turnigy SK3 168kv 6374 Aerodrive motors w/sensors
10s Turnigy Graphene 10,000mah 15c battery (matching spec 4S+6S)
15mm belt with 15/36 tooth ratio
Dual VESC
wireless remote 2.4ghz
97mm bigfoots
gulwing 10" trucks
[/quote]

what I would recommend 
Torqueboards 218mm caliber clone trucks
dual rear mounted 6374 motors
90mm Abec11 75a flywheels with 40T wheel pulleys or
83mm Abec11 75a flywheels with 36T wheel pulleys.
15t motor pulleys
60C or 90C Lipos
at least 10s, preferably 12s 
Still 30% grades are not gonna be easy.
```

---
## \#6 Posted by: Weirdboards Posted at: 2017-09-26T03:39:51.239Z Reads: 83

```
Thanks for the suggestions Okami! Quick question - the build would still require two focboxes? they do see sturdier than regular VESC. Have you used them?

Cheers.
```

---
## \#7 Posted by: Weirdboards Posted at: 2017-09-26T03:44:20.979Z Reads: 79

```
bigben, I have switched the trucks to 10" Caliber and ordered the mounts for my motors. Was concerned with the way the generic mounts looked when I got them in. 

Interesting thought on the batteries. I didn't think it was safe (for the motor) to go above 15c, but that seems like a learning curve thing now. I would say that seems like an expensive way to build a battery. I couldn't find any 2s LiPo batteries with 10k mah less than $65 ea. 

Thanks!
```

---
## \#8 Posted by: Weirdboards Posted at: 2017-09-26T03:48:19.416Z Reads: 76

```
So you and Namasaki are both suggesting the DR set up. Seems like there are a lot of fans of both ways. The new trucks I switched to will support dual rear, just wondering if there are any downsides to DR from your experience?

Thanks!
```

---
## \#9 Posted by: BigBoyToys Posted at: 2017-09-26T07:23:19.178Z Reads: 72

```
The only disadvantages to the DR set up I can think of are:
1. Both motors will be using the same truck hanger as a heat sink.
2. If you are pressed for space along the hanger you'd have to use narrow belts and pulleys which will limit the torque you can put down.
3. The board will not be balanced weight wise from front to rear which probably makes no difference other than when carrying it. (Putting the battery at the front could help offset this bit I wouldn't recommend it).

Advantages to the DR setup.
1. No torque related steering issues during acceleration or braking or during the transition between the two (biggest issue by far that I had).
2. Shorter power leads since they dont have to stretch from one side of the board to the other which is safer for your speed controllers.
3. No front wheel burnout issues during hard acceleration as your weight shifts to the rear.
4. Looks cleaner to me to have the whole drivetrain in one area rather than having them stretched from one end to the other.
```

---
## \#10 Posted by: bigben Posted at: 2017-09-26T07:30:56.736Z Reads: 68

```
https://hobbyking.com/en_us/graphene-5000mah-2s2p-hardcase-w-5mm-female-bullet-connector.html?wrh_pdp=7
I bought these last weeks when they were less than half price. At full price it'd be an expensive pack. There are some with comparable specs at a keener price.
```

---
## \#11 Posted by: Okami Posted at: 2017-09-27T08:13:41.839Z Reads: 58

```
There are lots of info about them. So far what ive heard is u should check out whenever u can use the new vesc tool for configuring.nicely as some people got errors i, think. (U can still use the old program tool and it will work nicely)

Hardware / look wise they stand on higher shelf. At least that is what seems to be the experience with them in community. Less errors / faults with.them.

Otherwise u can order vescs from chaka but i think they are similarly prices (not sure if thisnis.still a thing as he.might have moved.onto.other.things?)
```

---
