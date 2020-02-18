# &ldquo;Death Trap&rdquo; Build: Blank customskateboards.com deck, Dual 10s2p 30Q batteries, Two Flipsky FSESC 4.12, Dual 6374, dickyho mounts

### Replies: 14 Views: 856

## \#1 Posted by: ChicagoSkater Posted at: 2018-09-27T21:33:36.073Z Reads: 287

```
First build! This was after I realized it would be nice to have a way to get to the gym that didn't involve driving, and sort of escalated from there. 

As a first build, it was definitely improvised as things failed along the way. I first started by attempting to build something like the Skatemetric Foosted board, except on a budget. I was able to find cheap 6374's and went with those on caliber II trucks and ownboard enclosures and battery. I did give it a ride, and had a tough time fitting the enclosures to the curve, and found the standard bushings to be fairly unstable. 

I then ordered some riptide bushings, a second battery, and use 3 Seahorse enclosures mounted on the bottom. Wheels are Abec 11 97 mm, with aluminum mounts, pulleys, motors, and belts from Dickyho. The wheel pulleys needed to be drilled out to 1 in (25.4 mm) to clear the trucks, but come with 22 mm bore to add a bearing if necessary. 

The vescs are running Ackmaniac firmware, I've only ridden it in sensorless BLDC, and there was some cogging at the start, and overall not very smooth. I just set up FOC, and changed the ramp settings to hopefully smooth things out. I also adjusted the throttle curve.

I'm using two mini receivers paired to one remote for now, it's pretty straightforward and bulletproof.  

I have a larger 3d printer on order to make custom enclosures, along with TB trucks so I can mount both motors inboard; having one on the back is just annoying for standing the board up. The deck was cheap, so I don't feel bad drilling into it. I did attempt to form kydex with a foodsaver, but that didn't pull vacuum fast enough, and I was itching to get on the board, hence the seahorse enclosures. 

A few things I'd do differently:

Order smaller motors, 6374's are not necessary for a first board, but they were cheap, and I won't be running them nearly to their limits. 

Use black grip tape; it gets dirty fast. 

Use one larger enclosure mounted up top instead of 3 on bottom; clearance is fine with the big wheels and riser/6 degree dewedge in the back, but the look of the 3 enclosures isn't the cleanest. Great for prototyping and setup of electronics though.

For now, I'm still not comfortable on the board, so I'll probably spend some time practicing on paved trails before taking it on city streets. 

And here's the pictures: 

![IMG_2427|375x500](upload://fXWcr8qAz41MfPMoDAUfmdCEkIf.jpeg) ![IMG_2431|375x500](upload://gDy5dlejZ0vp3dYj29urVwJi149.jpeg) ![IMG_2432|375x500](upload://dfPqlZyLueMX4VquNpvI8SlphJq.jpeg) ![IMG_2428|375x500](upload://nbX8qe8qcH6lXxzXLv1OM0j3R6r.jpeg) ![IMG_2429|375x500](upload://gIoIbCxmTLXJXUa3vc8NVBeLl77.jpeg)
```

---
## \#2 Posted by: Jake2k17 Posted at: 2018-09-27T21:46:51.628Z Reads: 247

```
What batteries did you use?
```

---
## \#3 Posted by: ChicagoSkater Posted at: 2018-09-27T22:05:56.968Z Reads: 245

```
The batteries are two, 10s2p packs from ownboard, wired in parallel. Parallel discharge, but they need to be charged independently. It was a good cost/power ratio, but it looks like jackzoom has the packs for less.
```

---
## \#4 Posted by: Saturn_Corp Posted at: 2018-09-27T22:51:49.167Z Reads: 231

```
Looks good man! What range are you getting with those 10s2p x2's?
```

---
## \#5 Posted by: ChicagoSkater Posted at: 2018-09-28T02:23:39.408Z Reads: 208

```
Thanks! I'm still personally trying to get over how sketchy it looks. As far as range goes, I haven't run it down yet; I've only gone maybe 4 miles and it's at roughly 85%, I'd expect a range of at least 20 miles with 432 watt/hr batteries.
```

---
## \#6 Posted by: TheFluffiest Posted at: 2018-09-28T02:42:08.877Z Reads: 197

```
Be VERY careful with those red lights. I did the same exact thing, and I lost one immediately on the first ride. The second one died super quickly.

The other thing is try Dual Diagonal. Put one motor in back, and one motor in front on the opposite side. It is one of the best ways to transfer torque evenly, because there is more traction in front. 

You will be glad you ordered dual 6374 in the future! It's cheaper in the long run to go all out in the beginning 😂

Keep your weight low, and above the front truck. It will help you be more stable. It's usually called "tucking"
```

---
## \#7 Posted by: chrischo1996 Posted at: 2018-09-28T12:43:05.209Z Reads: 172

```
Hey so my build is pretty similar to yours, do you have any tips for mounting the wheel pulleys centered on the wheels? Once I lathed mine out to 1", it's hard to make it sit centers on the wheel
```

---
## \#8 Posted by: ChicagoSkater Posted at: 2018-09-28T13:42:40.145Z Reads: 159

```
Thanks for the heads up on the lights! I'll probably just stick them on my belt or bag or something; they'd be more visible that way anyways. 

I thought about dual diagonal, but I was concerned about running really long phase wires. Once I wire in sensors, I'll probably mix up the setup. 

Thanks for the riding tips! I'll give that a try this weekend.
```

---
## \#9 Posted by: ChicagoSkater Posted at: 2018-09-28T13:45:11.223Z Reads: 157

```
I had that same issue actually; what I did was tighten the screws so they're just _barely_ holding the pulley on the wheel with no slop, and then put it on the axle and give it a spin; if it wobbles, I'd tighten/loosen one pair of screws, put some tape on them to mark them, and spin it again. If it was better, I'd switch to a different set of screws; if it was worse, I'd do the opposite. 

It took some trial and error. Next time, I'd only drill out a portion of it, but not the whole thing. Just enough to get it over the hanger. I'll most likely 3d print some pulleys however, just to have a cleaner look.
```

---
## \#10 Posted by: chrischo1996 Posted at: 2018-09-28T13:53:00.497Z Reads: 147

```
Huh ok, that's basically the process I went through, was just wondering if there was a better way. It seems to work at the moment for me. 
I also noticed that even with the motors as far forward as possible the mount doesn't extend much further (maybe a 1/16" at the right angle) which becomes a problem when your trying to stand the board up. I'm thinking about utilizing the pulley cover mount holes to mount a bar or something over the motors, any ideas?
```

---
## \#11 Posted by: TheFluffiest Posted at: 2018-09-28T19:16:57.311Z Reads: 135

```
True. Be super careful with it if you are riding at night. Mine went out on my backpack and I almost got hit by a car going pretty fast. I had to bail at 32mph, and the car destroyed the board
```

---
## \#12 Posted by: Blitz Posted at: 2018-10-18T19:29:49.706Z Reads: 105

```
How are those flipsky 4.12 vesc's holding up?

Do you run them In BLDC or FOC?
```

---
## \#13 Posted by: Igor Posted at: 2018-10-19T17:39:32.625Z Reads: 88

```
@ChicagoSkater, any updates on this project? I want to convert my vanguard to something similar, so I would appreciate your insight!
```

---
## \#14 Posted by: ChicagoSkater Posted at: 2018-10-19T21:17:10.537Z Reads: 92

```
Unfortunately I haven't had much time to work on it lately. Ride wise, it's actually pretty good when tuned in. I mostly run it in BLDC, I did run it in sensorless FOC for one ride, but had some motor cogging on startup and at low speeds. Otherwise, those ESC's are great. 

I'm currently trying to swap it to a stiffer deck with a new 3d printed enclosure once I find one that fits the batteries. 

Additionally, I'm going to switch to TB 218 trucks to fit both motors inboard. I really don't like having any outboard motors, they make it difficult to stand the board up or roll it by the back wheels. I'm also connecting the sensor wires now that my JST plugs came in. 

I go back and forth between using canbus and two receivers; at the moment I'm using two receivers just because that's how I last set it up. I didn't notice any difference in performance or reliability between the two.
```

---
