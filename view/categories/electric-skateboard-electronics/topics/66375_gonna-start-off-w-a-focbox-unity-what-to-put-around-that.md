# Gonna start off /w a FOCBOX UNITY – what to put around that?

### Replies: 10 Views: 467

## \#1 Posted by: dalausb Posted at: 2018-08-28T17:54:42.782Z Reads: 182

```
Howdy fellas! In a weird twist of events I just ordered a FOCBOX UNITY that's supposed to act as a starting point for my very first DIY Esk8 project. Yeah, I know... Probably overkill for a rookie. But now that I'll get it (whenever that's gonna be..) I wanna make good use of it.

Plus, I'm eyeing a cheap stop-gap solution to carry me through the time until the Unity ships – possibly an ONAN X2 4WD. Nothing's set in stone yet, though. Ideally, my stop-gap solution would accommodate the Unity and noticeably profit just from replacing its VESC already. But I have a hunch that I'll probably get a better result by keeping these two things completely separate, no?!?

My Esk8 is gonna be used for casual fun rides predominantly at first but since the regulatory landscape in Germany is about to change in October *fingers-crossed* I wouldn't wanna rule out a more frequent commute usage either. Thus, the option to change out wheels in order to add some limited offroad-capabilities later on would make a ton of sense. Afaict, that means I'll have to go with a belt drive or direct drive solution. But I'm looking to build something BoostedBoard-esque, anyway. So that doesn't bother me.

Adhoc-budget is a concern, overall-budget not so much. Which is to say that I'm willing to sink a good chunk of money into this project in order to create a fun, solid, and well-performing build. But I'd wanna build and extend it over time, rather than spending one big lump sum. 

So, right now, my very vague game plan looks like this:

- stop-gap solution: ONAN X2 AWD on a Vanguard
- real deal: FOCBOX UNITY + 10s5p battery pack from diyeboards + single TB 6374 190kv motor + mechanical kit
- later on: extend that to a dual TB 6374 setup 
OR switch to a CarvonV4TorqueDrive

+++ Questions:

1) Does this game plan make any sense to you, more experienced DIY-builders?
2) Are those components even gonna play nice with the UNITY?
3) Are those components making good use of UNITY's capabilities?
4) Do you know of any cheap-ish ONAN-X2-like complete set that would have it's shortcomings drastically improved just by adding the UNITY?

Cheers and thanks from Berlin – David
```

---
## \#2 Posted by: Jc06505n Posted at: 2018-08-28T18:08:12.980Z Reads: 172

```
I would recommend taking the time to research and see what components best suite your needs. 

[quote="dalausb, post:1, topic:66375"]
ONAN X2 4WD.
[/quote]

Onan's are Terrible. 

[quote="dalausb, post:1, topic:66375"]
10s5p battery pack from diyeboards
[/quote]

Why waste a "premium" ESC on subpar batteries? Look around and get your self a battery pack made from 30Qs or a battery builder willing to experiment with those new 30T's.

[quote="dalausb, post:1, topic:66375"]
later on: extend that to a dual TB 6374 setup
OR switch to a CarvonV4TorqueDrive
[/quote]

Make sure you understand the strength and limitations between a Torque Drive and Speed Drive, one may be better for you preferences than the other. 

[quote="dalausb, post:1, topic:66375"]
Are those components even gonna play nice with the UNITY?
[/quote]


Anything can play nice if you make it so. 

[quote="dalausb, post:1, topic:66375"]
Are those components making good use of UNITY’s capabilities?
[/quote]


No imho

[quote="dalausb, post:1, topic:66375"]
Do you know of any cheap-ish ONAN-X2-like complete set that would have it’s shortcomings drastically improved just by adding the UNITY?
[/quote]

Sounds like alot of work for just getting regular motors.
```

---
## \#3 Posted by: dalausb Posted at: 2018-08-28T18:19:50.719Z Reads: 140

```
Thanks man! I'm kinda torn about the torque vs direct drive question. Silent driving is great, thus the idea of getting a cheap stop-gap hub motor solution at first. As soon as sane regulation kicks in around here, though, I wouldn't mind the torque drives' loudness anymore and rather enjoy the better responsiveness. Then again, from what I'm hearing those CarvonV4 come pretty darn close to what a torque drive offers, no?!

Also, never heard of 30T's - gonna look into that. Are those an option that UNITY should be best/well equipped to handle?

And Re:Onan'sSuck – What would be your suggestion for a better alternative within the same price range?
```

---
## \#4 Posted by: topcloud Posted at: 2018-08-28T18:33:27.164Z Reads: 136

```
http://skatemetric.com/index.php/2018/07/03/ultimate-accessible-foosted-build-tutorial/

Easy to build, easy to sell to fund your next build.  Good hunting.
```

---
## \#5 Posted by: dalausb Posted at: 2018-08-28T20:28:23.913Z Reads: 119

```
Yes, thanks man! I knew about that one, already. I guess I'll stick rather close to that build, after all. Then again my question would be: (How) does the UNITY allow me to one-up that Foosted-build? 

And I guess I can answer that myself, already: The UNITY allows for 60A (or 30A per motor) to run through that thing - continuously - but I'll have a hard time (and/or very expensive one) finding a battery pack that would allow for that high of a continuous discharge. 

18650/20700's cap out at 20A/30A continuous and those 30A-cells are terribly expensive and/or near-impossible to get your hands on. 

So, in order to get the _most_ out of the UNITY, I'd basically _have_ to run with LiPo packs that are rated at 60-C, right? That, in turn, makes the BMS and stuff more expensive/complicated/bulky, though. 

Then again, I guess I shouldn't worry too much about getting the most out of the UNITY but rather focus on a good overall build balance for my needs and just be happy to have plenty of head room in terms of ESC temperature and throughput.

Still curious to see if someone has an idea on question number 4:

[quote="dalausb, post:1, topic:66375"]
Do you know of any cheap-ish ONAN-X2-like complete set or board that would have it’s shortcomings drastically improved just by adding the UNITY?
[/quote]
```

---
## \#6 Posted by: Blitz Posted at: 2018-08-28T20:31:16.444Z Reads: 104

```
Unity should be able to handle (60a- x1 motor) constant easily (120a- x2 motors )

Samsung Q30's are the most popular choice here, 15a constant (running cool) and they can pull up to 20a.

But again 80a is a lot off current and if you would constantly pull that much energy your battrey would drain very fast.
I've heard @b264 talk about how pulling less that the max is a safety feature.
So no need to worry about not Utilising 100% off the power the esc can handle.
```

---
## \#7 Posted by: b264 Posted at: 2018-08-28T20:40:50.088Z Reads: 97

```
Yes; using any electronic devices under their maximum rating will prolong both its lifespan and safety
```

---
## \#8 Posted by: dalausb Posted at: 2018-08-28T20:52:35.155Z Reads: 95

```
[quote="Blitz, post:6, topic:66375"]
Unity should be able to handle (60a- x1 motor) constant easily (120a- x2 motors )
[/quote]


Holy cr** --- the max load is indeed even higher than what I thought it was:
160A Continuous System Current
80A Continuous Motor Current
300A Max Current

There's no way I'm gonna get close to that on my first build, indeed. Nor should I. Thanks for your feedback!
```

---
## \#9 Posted by: 12meterkuk Posted at: 2018-08-28T20:55:42.994Z Reads: 88

```
When you add cells in parallel eg a 4p pack of 15a cells you’ll get a total of 4 x 15 = 60 amps continuous output.
```

---
## \#10 Posted by: dalausb Posted at: 2018-08-28T21:04:37.024Z Reads: 90

```
Dang! Of course!!! Thanks a lot! You wouldn't believe just how much this helped me out here, really. With all those factors in play I'm still very early in the process of wrapping my head around each and every one of them – and this, well, is quite an essential one to grasp.
```

---
