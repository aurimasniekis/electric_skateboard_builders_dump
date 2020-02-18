# Is 12s a waste if you don&rsquo;t plan on going fast?

### Replies: 16 Views: 1591

## \#1 Posted by: Atimu Posted at: 2017-02-07T05:13:30.464Z Reads: 246

```
I built a 12s5p battery that im gonna use with a 190kv 2500watt torqueboard motor (and by summer dual motor) and vesc, with a 2:1 gear ratio for now to be able to hit 35-40mph. I live in NYC, the hills arent more than 10-15 degrees and I would typically stay around 20-25mph for the most part, if not less. 

I told my friend about this and he said if I'm not going top speed, the extra voltage is wasted and dissipated as heat through resisters and such on the vesc, so it would be better if I had made a lower voltage battery and perhaps higher capacity. Though that can't be completely true right seeing that going 10mph on my current  6s board vs going 22mph saves a looot of power, and it doesnt seem to heat up at all. And I always hear high voltage is great because you don't need as much amps, thus reducing heat. 

Also some say this setup runs beyond the 60k erpm limit (only when fully charged though), but wouldnt that not be an issue as long as you dont ride full throttle while the battery is at full voltage?
```

---
## \#2 Posted by: evoheyax Posted at: 2017-02-07T05:40:07.138Z Reads: 241

```
Some of this has been debated in the community for a while. Some argue that it's all converted to watts anyways, so the efficiency of a 6s and 12s should be the same, as long as the ESC your using can handle the amps. Some argue higher voltage means less amps and thus less heat. I have noticed way less amps at 12s than even 10s per say with the same setup. Also, my tests showed the same motor getting 20 degrees cooler and the vesc got hotter at 12s, than at 10s. So a trade off maybe. I'll let some better experts dive into this one.

*grabs popcorn*
```

---
## \#3 Posted by: DilatedPupils Posted at: 2017-02-07T05:50:37.323Z Reads: 234

```
it's like saying why do you need a turbo on your car if you're not hitting top speed anyway?
would it be better to be flooring it all the time and only go so fast, or half throttle and go the same speed, and still have more power when you need it(e.i. when a dog chases you on your esk8)? [quote="evoheyax, post:2, topic:17324"]
I'll let some better experts dive into this one.

grabs popcorn
[/quote]
```

---
## \#4 Posted by: evoheyax Posted at: 2017-02-07T06:47:59.402Z Reads: 209

```
[quote="DilatedPupils, post:3, topic:17324"]
(e.i. when a dog chases you on your esk8)?
[/quote]


Funny you say this, when I literally outran getting picked off by a Prius who decided to not look up hill in the direction they were going while I was going downhill. He pulled a left into a driveway as I was passing him on my  side of the street. Having high speed can help you get out of the way of bad drivers.
```

---
## \#5 Posted by: SeanHacker Posted at: 2017-02-07T07:08:54.038Z Reads: 206

```
I'm watching this only because I don't know any better. ;)

<img src="/uploads/db1493/original/3X/b/d/bd1871ae8fe9706b4b0e18a77b2f5533d75bb778.jpg" width="499" height="499">
```

---
## \#6 Posted by: RogerD Posted at: 2017-02-07T11:20:53.616Z Reads: 196

```
You don't need lots of voltage to go fast. It's all about gearing, and the right motor KV (and size) for the job.

Given a "standard board" - to increase speed you do one of these:

- Increase physical gearing (a larger motor pulley or a smaller wheel pulley) - though don't "over gear" your setup - if you gear too high you'll heat up the motor and ESC.
- Increase voltage - i.e. go up from 6s to 8s. This is a very easy way to increase speed, Make sure your ESC can take the voltage increase (the motor probably will)
- use bigger wheels (same as increasing gearing)

It is best when choosing motor, esc, battery voltage to try and have your board running at max efficiency at full (or near to full) throttle. So, using one of the many speed calculating spreadsheets on the internet, put in the motor KV, battery voltage, gearing, and wheel size and see what top speed it gives. Then knock a bit off. So if it tells you you will max at 25Mph, it will be around 21 ish in the real world.

Now you can change the motor KV, or the battery voltage, or the gearing to get the max top speed you actually want, and build your board around this.

When doing this, if you want to keep things cheap, don't go above 6s (cheap batteries and chargers).
If you want to use a VESC then you want to head towards 8s or more as the VESC doesn't run much above 75Amps, and more voltage = lower amps. But now you need more expensive batteries.
If you climb a lot of hills, keep your gearing and KV down and increase voltage. Saying that, I climb steep hills on 6S with car escs.

I recently built a new board with two motor choices. The calcs told me that the high KV motors would theoritically give me 42 mph - this is WAY more than I want. The second motor, the lower KV one, would give 24mph. The supplier of the motors said "don't worry, get the faster ones and then don't use full throttle".

He's right, and very wrong too. I would be running a very fast setup at less than half throttle all the time. It's not right to compare it to a turbo car with spare power (a car engine runs just as efficiently at medium and higher revs) . Because my setup would have been running at less than half throttle nearly all the time, it would be hard work on the ESC, and I'd be running less than optimal gearing. To have all that spare speed at hand, but hardly ever used, is akin to driving everywhere in 5th gear - really inefficient. It would be crap up hills too (lacking in torque as the setup is geared for a speed you hardly ever do).

Gear your setup correctly and everything runs cool and happy. I've built a few boards now and a change of 1 tooth on a motor pulley can be the difference between overheating and running cool.

When your friend refers to wasted voltage in esc heat he's mostly right. At part throttle, an esc has to dump the excess - some of this is heat. Hence it's best to set your board up to run at your normal cruising speed at a point beyond 60% throttle.

I have two 6s boards, and both are geared to run a top speed of around 24 mph. Throttle is around 50% for cruising and I use around 75% going up steep hills, and only 100% when I am wearing a helmet, and that's not often (not often max speed!). I'm 48 and coming off over 20mph is reasonably likely to break somthing (on me!). My board was previously geared for 35 mph but I geared it down to keep it cool and avoid a traumatic brain injury! :slight_smile:
```

---
## \#7 Posted by: mountainboardlover69 Posted at: 2017-02-07T12:06:52.696Z Reads: 165

```
<img src="/uploads/db1493/original/3X/8/6/86f55f462da13098ebebf9eb8947263bcad58182.png" width="500" height="350">
```

---
## \#8 Posted by: Namasaki Posted at: 2017-02-08T03:36:38.721Z Reads: 144

```
I agree with @evoheyax.
Higher voltage does not necessarily mean less heat.
It does however mean more top speed.
I have run compared 12s with 6s on the same setup. 
12s at half throttle and 6s at full throttle equaled the same speed.
A motor's KV stands for rpm per volt.  So, 190kv at 52v = 9880 rpm
190kv at 25v = 4750rpm
Of course higher voltage yields more speed.
unfortunately, as my experience has been with 12s, it is rather hard on the electronics.
I burned up a HV switch and a 12s 120a ESC running 12s.
on the other hand, I have never overheated running 6s or 10s.
Bottom line, I would not recommend 12s if your trying to build a dependable board for transportation.
```

---
## \#9 Posted by: jmasta Posted at: 2017-02-08T05:23:29.193Z Reads: 131

```
It's really a matter of power, and how that power is distributed based on your gearing.  Speed is proportional to voltage.  Torque is proportional to current.  Power is the product of voltage and current.... aka, speed and torque

50V at 10A is 500W.  Just like 25V at 20A is 500W.  But this does not take into account the fact that the heat generated is directly related to amount of current flowing.  As electrical components heat up, their resistance also increases.  Higher resistance equals lower efficiency.  

TLDR; 12S would be more efficient than 6S with equivalent gearing
```

---
## \#10 Posted by: jmasta Posted at: 2017-02-08T06:14:06.914Z Reads: 125

```
Side note[quote="Atimu, post:1, topic:17324"]
I built a 12s5p battery that im gonna use with a 190kv 2500watt torqueboard motor (and by summer dual motor) and vesc, with a 2:1 gear ratio for now to be able to hit 35-40mph. I live in NYC, the hills arent more than 10-15 degrees and I would typically stay around 20-25mph for the most part, if not less.
[/quote]

Keep in mind that BLDC motors are most efficient at around 80-85% max RPMs. So ideally you'd want to design your board's gearing accordingly. If you were traveling at 25mph, a board designed for a weighted topspeed of 30mph would be more efficient than one geared for 40mph
```

---
## \#11 Posted by: Ackmaniac Posted at: 2017-02-08T09:11:54.852Z Reads: 109

```
I think 12S is more efficient because of the lower current. But on the other side a 20% more speed results in 72,8% more energy consumption at top speed (20% more = factor 1.2 and 1.2³ = 1.728). So that would be the explanation why the system can overheat then. 
So if you would compare the same gearing setups at the same speed with 10S and 12S then the 12S should perform better.
```

---
## \#12 Posted by: RogerD Posted at: 2017-02-08T10:50:45.060Z Reads: 97

```
My brief experimenting with a 12s board (for a friend) works fine, but the extra efficiency you theoretically get from running higher voltage didn't result in a measurable real world difference. I'm 6s, he's 12s. His packs are half the capacity of mine (twice the voltage) and we both run about the same distance.
```

---
## \#13 Posted by: okp Posted at: 2017-02-08T11:57:59.864Z Reads: 93

```
maybe the weight gain?
```

---
## \#14 Posted by: RogerD Posted at: 2017-02-08T14:53:17.133Z Reads: 87

```
I'm around 90kg, he is around 90 kg, so we are both the same.

His batteries are a similar weight to mine, and to be honest, they weight of the batteries, and the board, for that matter, are fairly insignificant compared to what they have to haul around (us!)

I reckon the differences in efficiency are trivial when compared to how much energy is going into propelling us about.
```

---
## \#15 Posted by: jmasta Posted at: 2017-02-08T16:37:47.103Z Reads: 82

```
That's because you have confounding factors that are negating the efficiency gain from 12S.  If you run 6S at 80% load and compare it to 12S at 40% load... you are pulling less current at 12S (higher efficiency) but also running your motor at a less optimal RPM (lower efficiency)

You need to account for gearing by using different sized pulleys
```

---
## \#16 Posted by: RogerD Posted at: 2017-02-08T18:48:30.492Z Reads: 78

```
Nope - I built both boards and they are both geared correctly - his is geared for 12s, mine for 6. I toothed down his gearing to bring his top speed down from 40mph to the mid 20's. Both motors are running as they should.

Incidentally, running a 10s "rated" motor on 6s doesn't mean it runs less efficiently. With brushless motors, the max voltage is a limit, not a recommendation. 

The 10/12s efficiency thing is way overrated. Expensive batteries and chargers for little gain.
```

---
