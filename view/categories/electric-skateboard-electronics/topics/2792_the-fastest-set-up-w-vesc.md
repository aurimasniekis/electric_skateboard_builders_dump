# The fastest set-up w/ VESC

### Replies: 20 Views: 3939

## \#1 Posted by: wallaboo Posted at: 2016-05-01T23:37:32.585Z Reads: 423

```
I am curious what the best configuration is with the technology we have. I am not concerned with which motor or battery will be cheap/have longevity. I know its possible to build a 60mph+ board, but that is not what we are about. We want boards that are reliable and safe.

What I envision is to have a board that can accelerate up hills or have enough torque to maintain the speed on a 10% hill grade. Say, you reach max top speed and enter a hill that has a higher grade than 10%. Can the speed be maintained? How much torque is needed to reach top speed on a hill? What is the top speed for hills? The speed and torque should have a nice equilibrium. You don't need enough torque to throw you from the board, but there needs to be enough to make it up any hill at a decent speed. For people like me, it would be good to know whats the best configuration to make it up hills because once you hit the top, there is no need for a motor.


So my question is what is the best configuration with the VESC? Highest top speed vs. torque to climb the steepest hills

From my research a 12S battery with a 198kv motor might be our max output with the VESC( I heard that the VESC won't handle 12S with 200kv+). Is this best for top speed or torque? Would 11S with say, 250kv be better? Also, there is the factor of having one vs. two motors. Will two motors and two VESC allow us to build an insane 24S set-up? 

 I would also like to see what the best configuration is for the pre-built 10S3P or 10S4P batterys, since its lower than 12S. This is probably just an issue of higher and lower kv. What is the max/min for a reliable kv? Should we ever go above 300kv or lower than 150kv?

All this information will change when we test this in the real world. I personally live in a area with lots of hills, so torque should be a bit higher for people like me. Flat areas will need relatively little torque. This tool is great for calculating the max output for setups, but it doesn't calculate torque or hills. [Calculator Link:](http://toddy616.blogspot.com/2013/07/electric-skateboard-calculator.html)
```

---
## \#2 Posted by: BoardAdmin Posted at: 2016-05-01T23:42:06.489Z Reads: 399

```
http://www.elektro-skateboard.de/wiki/wissenswertes/strom-spannung-reichweite-vii
```

---
## \#3 Posted by: Adam0311 Posted at: 2016-05-01T23:59:06.494Z Reads: 389

```
I can't tell you what the BEST setup is, but the dual 6355 motors (194kv...?) and 10s3p battery on the raptor dual can accelerate from a kick push to 20mph up the 15% grade next to my house. Gearing and wheel size also play a big factor. As does rider weight.
```

---
## \#4 Posted by: psychotiller Posted at: 2016-05-02T00:15:15.876Z Reads: 382

```
Rider weight, temperature, durometer, abec rating, voltage sag...find a way to average those variables.
```

---
## \#5 Posted by: Michaelinvegas Posted at: 2016-05-02T04:22:46.749Z Reads: 351

```
Lol are you spec in'  this shit to sent to China ?
```

---
## \#6 Posted by: wallaboo Posted at: 2016-05-02T05:26:33.161Z Reads: 348

```
[quote="psychotiller, post:4, topic:2792, full:true"]
Rider weight, temperature, durometer, abec rating, voltage sag...find a way to average those variables.
[/quote]


It's a work in progress :grin:

[quote="Michaelinvegas, post:5, topic:2792, full:true"]
Lol are you spec in'  this shit to sent to China ?
[/quote]

Hahaha no I'm just asking questions with my insufficient knowledge. I mostly just browse this forum, but I can see a reoccurring trend revolving around the question of kv and voltage. The only way to find these bits of information is to read every build thread and get each piece of information at a time. It would be nice to have a single thread so we can fully understand what all this is.

Standard knowledge: lower kv, higher torque. 
So I have no idea what would be a kv that is too low. I am intending to build a quiver(multiple EBoards - I am also a skier so I have a different ski set-up for different snow conditions.) one for flat ground, one for hills, one for night rides etc...
```

---
## \#7 Posted by: Michaelinvegas Posted at: 2016-05-02T05:32:00.405Z Reads: 315

```
Hahah .... What you should do...is just get it done...not once...not twice ... Not anything.... Just do it...then break it ...then build it ....and when that settles in...build a new one...then break that shit....and build it....so on so fourth ....

Get your base ride built ...then you can build around it ...Plus you'll have some rides for your friends 🤘🏻
```

---
## \#8 Posted by: trbt555 Posted at: 2016-05-02T05:39:39.728Z Reads: 307

```
The question you're asking is the one all DIY'ers are trying to answer.
12S with 190kv motor seems to be the sweet spot. Check Vedder's blog for a tutorial on how to select a motor for optimum performance.
Need more torque ? Go dual or go for a longer motor.
```

---
## \#9 Posted by: Michaelinvegas Posted at: 2016-05-02T05:51:15.756Z Reads: 298

```
How MUCH larger???? HUMMM? 👀

Kinda wonder what the can size limit is🤔
```

---
## \#10 Posted by: wallaboo Posted at: 2016-05-04T04:12:36.734Z Reads: 286

```
Alright, my intro into electricity 101 has officially begun. I have done some research just to double check the claims. I trust you guys, but my curiosity got the best of me :slight_smile: I am taking the specs and breaking them down into bite sized chunks. I just got done looking at amps and volts.

VESC specs:
Voltage: 8V – 60V (Safe for 3S to 12S LiPo).
Current: Up to 240A for a couple of seconds or about 50A continuous depending on the temperature and air circulation around the PCB.

1S is what we all know as a lipo cell. Each cell contains (on average) 3.7Volts OR 4.2 Max Volts. 12S would be 3.7 x 12 = 44.4  OR 4.2 x 12 = 50.4 This shows that 12S is withing the safe range of 60V. Looking at the other ESC's on the market showed me that they will only specify the safe number of cells. As in "Input Voltage: 4-14 cells li-XX or 12-42 Ni-MH/Ni-Cd battery" or "Power Supply: 2s~6s LiPo Battery"

The batteries then have the "C"  and mAh ratings. You multiply these together to get your Amps. There are 1,000 mAh in a Ah. So a 5000mAh with a 10C rating is calculated like so: 5000mAh/1000 = 5Ah then, 5Ah x 10C = 50Ah. So by this it looks like a 5000mAh battery with 10C rating is the one to get.

Basics:
S (voltage) is (power) how fast you can go
A (amps) is (time) how far you can travel
```

---
## \#11 Posted by: Michaelinvegas Posted at: 2016-05-04T04:33:13.949Z Reads: 254

```
Lol looks good....

Ok now go build lol

6s esc common
8s and higher is not 

Batteries keep above 10c ( but I keep above 25c)
Also stay with a 5000mah or higher...or else your ride will be a short one
```

---
## \#12 Posted by: wallaboo Posted at: 2016-05-04T04:43:41.897Z Reads: 256

```
[quote="Michaelinvegas, post:11, topic:2792, full:true"]
Lol looks good....

Ok now go build lol

6s esc common
8s and higher is not 

Batteries keep above 10c ( but I keep above 25c)
Also stay with a 5000mah or higher...or else your ride will be a short one
[/quote]

I'm still waiting for a VESC haha so I have been slowly crafting my deck. I just got some acrylic paint for my design. It should be finished in the next few days. I'll post it in my thread.

5000mAh is pretty low, but running a few of these batteries in series should double or triple the ride time? Increasing voltage should increase the power required, which might effect this claim...

 Running batteries in series increases the voltage, while keeping the mAh the same. Running in parallel makes the inverse true.
```

---
## \#13 Posted by: Michaelinvegas Posted at: 2016-05-04T04:47:07.659Z Reads: 253

```
Sure the more MAH the bigger the battery...

It's a balance between looks and utility ... 

Trust me you don't want board that looks pregnant cause you have 10,000 mah battery under ur feet ... Unless you split the pack to make it flat
```

---
## \#14 Posted by: onloop Posted at: 2016-05-04T04:53:47.879Z Reads: 264

```
I know this is going to sound like a sales pitch... but it's just from my experience...

This is the best setup I have found.
10S | 190Kv | 83-90mm Wheels | 15-36 Motor/Wheel Pulley | Dual 6355 Motors | Max 50A Current limit

In terms of top speed, this configuration is 52km/h theoretical at full charge (~ 45km/h in reality) 

In terms of hill climbing, this config eats hills... if you are a really heavy rider 100kg+ you might need dual diagonal 6374 motors..

What would I do to make it better?
1. Bigger (or more) motors, this is the answer to all questions about performance.
2. Bigger Battery, Bigger battery can output higher current for longer. Increase max current output up to approx 80A
3. Heat management systems, water or air. For motors, esc & maybe battery.
4. Wider Belts, Improved Torque transfer, to get all this power to the wheels!
5. Have your motor spinning up to max of around 8000-9000rpm for optimal performance.

What I wouldn't do.
1. Higher voltage... Going 12S might (not enough info yet) introduce problems, especially with higher KV motors.... For now, I am staying clear of that. ALSO: 11S is not a good number for battery assembly even numbers are better. So 10S is good.
2. Less gearing reduction, Never reduce reduction to increase speed. It will just increase current draw & overwork the motors. This is why HUB motors are difficult to perfect. Maximise Reduction & Custom KV motors is the best choice for your drive train.. If you want more torque use a smaller wheel.
3. Ride faster than approx 45km/h.. Any faster than this & wind resistance becomes a major problem & you get diminishing returns, basically you start converting energy to heat with minimal thrust. ALSO, any faster in urban environments is dangerous. Faster is ok on track day in controlled env.

How do i know all this.....

TESTING TESTING TESTING TESTING TESTING TESTING....

The best thing you can do is build a few boards & ride em.
```

---
## \#15 Posted by: jack_pate Posted at: 2016-05-18T07:19:49.581Z Reads: 238

```
How far and fast would I go with a 2 x 6s 5000mah (in series)
with a vesc? Would this break the vesc?
```

---
## \#16 Posted by: willpark16 Posted at: 2016-05-18T08:26:36.170Z Reads: 241

```
depends on your motor kv
```

---
## \#17 Posted by: jack_pate Posted at: 2016-05-18T09:37:12.657Z Reads: 246

```
My motor is a enertion 190kv motor
```

---
## \#18 Posted by: BOBimusREX Posted at: 2016-09-24T04:10:43.098Z Reads: 180

```
Have you ever actually blown a VESC? I'm modifying a chinese device that came with a 60v lithium ion battery pack, and the VESC is rated for 60v in some descriptions, and 50v in others.
```

---
## \#19 Posted by: Jinra Posted at: 2016-09-24T04:13:05.092Z Reads: 178

```
the VESC is rated for 12s which is 50.4v, but the VESC can handle 60v. You want to leave headroom for voltage spikes.
```

---
## \#20 Posted by: StormTrooperBert Posted at: 2017-09-16T00:57:28.463Z Reads: 88

```
This is my gas station run setup. 190kv, 16:36, 90mm wheels, I weigh 220lbs, it goes 6.1-6.2 miles on a full charge consistently. 👍🏽
```

---
