# Ever get an Over Current fault? Check your motor for shorts!

### Replies: 12 Views: 789

## \#1 Posted by: Jinra Posted at: 2017-10-11T05:56:36.136Z Reads: 134

```
TL;DR Over current faults might be causing your motor to short. Check your motor for shorts by moving the phase wires around in different positions before riding (see video below)

Most of you have heard of my recent FOC failure and crash at 30mph~. This crash left me with a ER visit and minor concussion as well as another $260 bill for a new TSG Pass.

Initially, I believed this to be a failure in FOC made (and possibly DRV failure). However my findings today made me second guess that analysis.

**Some background**
When I initially setup foc, I was getting overcurrent faults left and right ending up with 300~ amp current and 140~ filtered on each VESC. This happened a bunch as I was testing on the bench and while riding. I setup higher limts, and eventually found a solution via doubling the observer gain in FOC. While most of the faults in testing were **over current** faults, one of them did pop up as **drv8302** error. This led me to believe the DRV completely failed recently due to my testing.

**New findings**
Today one of my motors completely seized and died while riding in **BLDC** mode. The seizing occured at a similar time as when it would error in FOC, which was when I throttled up from any given point too fast. I was sure the DRV was toast at this point. Now, the motor doesn't spin right when throttling and only cogs

However, when I got home and tested throttling, I only got over current errors and **not**  DRV8302 error. I thought this was weird since I was sure it was a dead DRV chip. I then tested detection and, as expected, the detection failed. However, when I tested it on my other motor (same vesc) it ran fine! This led me to investigate if it was a short within the VESC itself. However, when I disconnected the motor completely, I noticed the motor still span like there was a short.

**Motor shorts**
At this point I concluded there was definitely a minor motor short (not complete short like touching 2 phase wires together). Shockingly, I found that this was present on **both** motors if the wires were in a certain position.

I don't know how to take the stator off the baseplate to investigate more closely, but I might've noticed some strands of copper that were broken. This is possibly causing the short. See the video below as evidence of the short **in certain positions**.

**Questioned unanswered**

Assuming the overcurrent faults caused some copper strands to break leading to motor shorts, why did the problem only really prevent itself when throttling quickly from any given point? 

* My overcurrent failures were a result of throttling too quickly, which was remedied by doubling my observer gain
* After the OC fix, the motor would perma short until restart every so often when throttle to maximum speed
* My crash was caused by the short at maximum speed, after which I tested the throttle and motors responded normally.
* My motor shorted again in BLDC mode (previous notes were all FOC) when throttling from mid to high speed quickly

https://youtu.be/ehIsZj6UYE8

Now I'm still not 100% what may have caused the short, but I believe it's likely either a manufacturing quality issue or a consequence of my over current faults. It's also possible the shorted wires were causing the over current faults in the first place, but unsure why doubling the observer gain would resolve the issue in that case.
```

---
## \#2 Posted by: scepterr Posted at: 2017-10-11T06:34:00.849Z Reads: 113

```
Did you ever run this test?
   [quote="scepterr, post:46, topic:33203"]
Mine can go overcurrent on the bench too without movement, but not consistently, I can force a fault if I shake 1 phase wire. Jiggle and twist it at every connection including on the vesc. 
I can replicate on 2 vescs
[/quote]
Most oc faults ive handled if not caused by an obvious component failure on the vesc ended up being a connection/short issue
```

---
## \#3 Posted by: Jinra Posted at: 2017-10-11T06:42:21.221Z Reads: 108

```
The video shows the issue, which I believe is caused by the over current faults to begin with. It wouldn't explain why doubling observer gain fixed my OC issues though.
```

---
## \#4 Posted by: scepterr Posted at: 2017-10-11T06:43:17.762Z Reads: 104

```
It was still happening just didn't register as an error and fault

Getting the motor apart isn't that difficult and at this point can't make it any more broke
```

---
## \#5 Posted by: Jinra Posted at: 2017-10-11T06:48:24.001Z Reads: 101

```
If it was happening why wouldn't it register as a fault? I'm fairly confident at this point that doubling the observer gain is indeed what is causing the OC issues, which may have led to the short, not the other way around.

Like I mentioned, I did open up the motor to look for signs of damage, but can't figure out how to separate the stator from the base plate.
```

---
## \#6 Posted by: scepterr Posted at: 2017-10-11T06:50:33.235Z Reads: 97

```
Whoops misread that, got an LCR meter to check the phases?

Unless the fets are shorted I don't know how the vesc could the damage the motors
```

---
## \#7 Posted by: Jinra Posted at: 2017-10-11T06:51:52.491Z Reads: 95

```
Well sending 150 amps of filtered current to the motor might've caused the copper strands to blow leading to a short. Unfortunately, I don't have a meter to test LCR with.
```

---
## \#9 Posted by: BigBoyToys Posted at: 2017-10-11T21:46:27.600Z Reads: 78

```
Cheapest one I know of thats available that would arrrive by Friday. Not sure if the shipping is Prime in your area though.

Digital Multimeter Resistance Capacitance Inductance LCR Multi Meter Tester with LCD Backlight Transistor hFE Display: 1-1999 UA6243L https://www.amazon.com/dp/B0114KNPV0/ref=cm_sw_r_cp_apa_EcP3zb0AZ8P07
```

---
## \#10 Posted by: racidon Posted at: 2017-10-11T23:12:54.015Z Reads: 65

```
Completely agree with you here @Jinra as I've had a very similar thing happen to me twice. I've now decided to consider the motor responsible as dead (not fixing it anymore). As the first time it threw at about 30km/h (something like that) was bad, but I got back up pretty easy, it however fried the VESC I was using at the time. The next time it happened the VESC survived (something be said about @chaka's great work - his was not the one that died previously).
Both times caused by the phase wires shorting whilst underload, which essentially slams the breaks on 100%  makes you realise just how strong your belt is though :slight_smile:

My second time left me with a really nasty bruise and still allowed the motor to spin freely without weight on it, but once there was some load it produce the same result.

You can also produce the same error if you have bad connections between the VESC and the motor.
```

---
## \#11 Posted by: faithfulpuppy Posted at: 2017-10-11T23:32:17.500Z Reads: 63

```
maybe a stupid question, but what exactly is "going wrong" in the video? is it the clicking noises?
```

---
## \#12 Posted by: Jinra Posted at: 2017-10-12T00:32:33.690Z Reads: 64

```
it spins much more initially, then when i press on the phase wires just a bit, stops nearly instantly when spun.
```

---
## \#13 Posted by: faithfulpuppy Posted at: 2017-10-12T00:58:29.972Z Reads: 62

```
gotcha, i didn't see the phase wires
```

---
