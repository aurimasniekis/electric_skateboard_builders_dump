# Running a alternator as a brushless motor in a kids hummer limiting rpm

### Replies: 23 Views: 892

## \#1 Posted by: fixitmoditbreakit Posted at: 2018-08-02T04:42:53.683Z Reads: 149

```
Hi i need some help,  I've upgraded my sons 12v hummer using a alternator and a gokart rear axle. the thing is too fast!! running a alternator as a brushless motor is inefficient i know i just wanted to see if i could do it. the acceleration is good does wheelys i can limit that with max amps but if i bring the erpm limit max down i loose acceleration too is there away to limit the rpm and not loose the acceleration?

**Settings i am using and battery ect**

ERPM MAX 12000.0 seems a good top end 
8s lipo drone racing batteries x2 4s in series  
hall sensor foot pedal ADC app 
playing around with motor amps but set to 80amps
battery max is 100amps lol
braking max is -35amp
regen is 7amps
ABS is 150amps
duty cycle reverse button which is on a switch

I know all these settings are wrong and could harm the vesc.   It seems to just go in to over temp and slows down but thats only with me in it, its fine with him so could bring all these settings down.

I know its a bit off topic but any help would be much appreciated!!
Cheers
Adam
```

---
## \#2 Posted by: AutoItKing Posted at: 2018-08-02T04:55:50.184Z Reads: 142

```
ERPM limit shouldn't affect the acceleration, that's odd. Are you sure no other settings change when you lower the ERPM limit?
Something that may be happening is what's known as slip. Basically the rotor can't keep up with the rotating magnetic field and it "slips". Modern automotive alternators have no permanent magnets and rely on a separate field winding to provide a counter rotating magnetic field.
Can you do some data logging? It would give insight into what's going on. If you hit the ERPM limit because of slip that would explain it.

Edit: a note on your settings, battery amps will always be less than motor amps (at 95% duty it'll be ~95%). Setting your battery max higher than motor max does nothing.

Edit 2: last one I promise. When you convert an alternator to a motor you are effectively turning it into a squirrel cage motor which definitely have slip.
```

---
## \#3 Posted by: fixitmoditbreakit Posted at: 2018-08-02T05:05:50.867Z Reads: 122

```
nice cheers will have to look in to how to data log!!

I have played around with the field voltage a little but not after bringing the erpm down.  I have the voltage at around 8v maybe giving it a stronger magnetic field would help with slip?

when hes pulls away and the wheels spin alittle add some slip too it will hit the erpm limit and slows down thats what you are saying right.

Thanks for your info dude
```

---
## \#4 Posted by: AutoItKing Posted at: 2018-08-02T05:16:30.547Z Reads: 116

```
Ah okay, you do have a field current. The voltage isn't so important, it's the current that creates a magnetic field: current * # of turns (plus some constants). But of course you can't have current without voltage... you can turn up the voltage to get a higher field. That might help.

Although now that I think about it, the VESC programming monitors the back EMF from the unfed phase to track the rotor position. Dunno what that would do but I would think it wouldn't allow for slip and throw an error, but I could be wrong.

And lastly motor (machine) slip has nothing to do with what's outside of the machine (motor). It is between the stator and rotor. Not to dumb it down too much, but think of turning a heavy load with just your hands. Your hands may slip a bit when turning so your hands (stator field) are turning faster than the load (rotor field).
Your wheels loosing traction is just fun, nothing to with what I'm talking about.

I should note that you need some amount of slip to generate torque. Induction machines may have up to 5% slip under load and these things create a huge torque.
```

---
## \#5 Posted by: fixitmoditbreakit Posted at: 2018-08-02T05:21:58.856Z Reads: 102

```

[quote="AutoItKing, post:4, topic:63571"]
And lastly motor (machine) slip has nothing to do with what’s outside of the machine (motor). It is between the stator and rotor. Not to dumb it down too much, but think of turning a heavy load with just your hands. Your hands may slip a bit when turning so your hands (stator field) are turning faster than the load (rotor field).
Your wheels loosing traction is just fun, nothing to with what I’m talking about.
[/quote]

I understood that bit you explained it very well my wording isn't great!! i just thought the 2 thing together would increase the chances of it hitting the erpm limit.
```

---
## \#6 Posted by: AutoItKing Posted at: 2018-08-02T05:23:50.202Z Reads: 94

```
Gotcha, yeah it would cause it somewhat but I don't think it's the issue here.
```

---
## \#7 Posted by: fixitmoditbreakit Posted at: 2018-08-02T05:27:41.534Z Reads: 92

```
here's a little video of the car.  i put plastic wheels over the rubber ones to make more sliding fun
this was limited to 10000.0 ERPM it wont wheely,  wheels spin abit 

https://youtu.be/_7cto5myJeA

might do a video of it unlimited but i don't have anything quick enough to keep up lol
```

---
## \#8 Posted by: AutoItKing Posted at: 2018-08-02T05:36:30.726Z Reads: 90

```
Looks like fun! I'll defer to those more experienced with the VESC control scheme, I haven't really dug into the code much. For data logging, you should be able to plug in your laptop with VESC-tool open and log that way.

For reference: with a field current you've effectively created a synchronous motor. If you simply shorted (or grounded) the field winding it would be an induction motor (or squirrel cage). I know I said earlier you created a squirrel cage as that's what a lot of people do, but with the field current it's more accurately a synchronous motor. Just FYI.
```

---
## \#9 Posted by: fixitmoditbreakit Posted at: 2018-08-02T05:44:04.318Z Reads: 82

```
Thanks for your help!! i ve learnt more which is the aim thank you!! I will look it to squirrel cage and synchronous motor for its advantages and disadvantages
```

---
## \#10 Posted by: Skunk Posted at: 2018-08-02T10:14:43.446Z Reads: 70

```
 that's pretty cool.  Can't wait to build crap like this for my kid.
```

---
## \#11 Posted by: fixitmoditbreakit Posted at: 2018-08-02T11:23:34.678Z Reads: 66

```
Thats it slap it together find some room and let them go!!
```

---
## \#12 Posted by: fixitmoditbreakit Posted at: 2018-08-05T11:34:57.218Z Reads: 52

```
This is at 20000 erpm limit to fast I think. Need a way of turning it off with a remote when he goes to fast or changing the erpm limit with a remote would be good 

https://youtu.be/ZL7xPY9uckw
```

---
## \#13 Posted by: Skunk Posted at: 2018-08-05T11:46:56.593Z Reads: 52

```
Damn i wanna ride that thing
```

---
## \#14 Posted by: Mobutusan Posted at: 2018-08-05T15:55:33.639Z Reads: 49

```
Nice build! That thing's a beast. I modded my son's 12v Mini Cooper to 6s Lipo, then 4s with faster brushed motors and he loves it. Goes 10mph instead of 5mph. I think Charlie is going a wee bit faster and might need to slow down just a tad (heard that somewhere). Lol. That wide, slick wheelbase seems to be serving him well though. Thought he was going to roll it a time or two there.

What kind of throttle/brake controls are you using? My Mini has just the standard on/off pedal throttle, with Slow & Fast modes on a hand shifter. Right now, I have him start Low then shift to High to practice shifting and reduce the NSF (neck snapping factor), whiplashery, etc., but proportional control is next.
```

---
## \#15 Posted by: fixitmoditbreakit Posted at: 2018-08-05T21:11:01.682Z Reads: 43

```
Yeah he was driving slow all day until I said right let's pack up lol.  I ve been trying different erpm settings this is too fast at 20000 Max erpm and I thought he was going to roll it scary to watch!! I did the same I will find the video with 30000 rpm motors/gearboxs.  With the brake,  it's setup with the vesc and using about 25amps braking and 8amps Regen so when he releases throttle they come on.  I had to put a huge throttle curve on the throttle as the thing wouldn't stop wheeling seemed to work OK.

https://youtu.be/nHYvLP9rhF0
```

---
## \#16 Posted by: Skunk Posted at: 2018-08-05T22:01:50.072Z Reads: 37

```
I wanna build one with Luke Skywalker's Landspeeder bigwheel I keep seeing. 
So cool.
```

---
## \#17 Posted by: fixitmoditbreakit Posted at: 2018-08-05T23:05:22.486Z Reads: 32

```
[quote="Skunk, post:13, topic:63571, full:true"]
Damn i wanna ride that thing
[/quote]

Man it's twitchy as when I get on it,  still fast but the vesc over heats after about 30sec of full throttle.  You should make one it's easy the pricey bit for me was the vesc the rest was free
```

---
## \#18 Posted by: Skunk Posted at: 2018-08-05T23:11:13.390Z Reads: 30

```
It will be a few years.  She's not even 1. Lol
```

---
## \#19 Posted by: fixitmoditbreakit Posted at: 2018-08-05T23:19:51.075Z Reads: 28

```
He's just turned 3!! Get her one of them balance bikes when she get abit older.   I found that really helped with steering.
```

---
## \#20 Posted by: aidsbmx Posted at: 2018-08-05T23:33:45.730Z Reads: 28

```
Aahaha if you where in AUS you're car would be impounded under HOON legislation for that little outburst there my friend =P
```

---
## \#21 Posted by: fixitmoditbreakit Posted at: 2018-08-06T00:29:44.671Z Reads: 28

```
[quote="aidsbmx, post:20, topic:63571, full:true"]
Aahaha if you where in AUS you’re car would be impounded under HOON legislation for that little outburst there my friend =P
[/quote]

Ahaha I am in Australia Sydney lol
```

---
## \#22 Posted by: K5_guy Posted at: 2018-08-06T01:22:50.545Z Reads: 26

```
Just put a roll bar on it.  :rofl:
```

---
## \#23 Posted by: fixitmoditbreakit Posted at: 2019-05-17T20:16:14.151Z Reads: 10

```
Hey thought I'd put this video up of my sons drift trike just a test build to see if hes likes it ect.  

https://youtu.be/JyXdNNLsUhU

Going to completely remake it next week if i have time
```

---
