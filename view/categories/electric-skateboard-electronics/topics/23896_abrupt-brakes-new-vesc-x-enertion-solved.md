# Abrupt brakes new vesc x Enertion \[SOLVED\]

### Replies: 17 Views: 865

## \#1 Posted by: Kasper Posted at: 2017-05-25T19:45:54.059Z Reads: 112

```
Hi everyone. here's a question about an issue I have with the new vesc x from Enertion. I've contacted them about it already but they are unable to help... So hopefully someone here does have some expertise about how to solve this.

The problem started ever since I installed the new vesc x. So here's the deal, when I start riding my board (dual raptor, Enertion) and want to brake, they're extremely abrupt. Just one millimeter on the controller and you almost fall off the board. Then after riding it for a bit, say 5-10 minutes, the brakes become very smooth as they should be and you can finally ride the board safely and comfortably.

Does anyone know here what to do? FYI I already tried setting the Batt regen setting a bit lower in BLDC tool. Thanks in advance for your help and time.
```

---
## \#2 Posted by: Blasto Posted at: 2017-05-25T19:47:53.801Z Reads: 109

```
[quote="Kasper, post:1, topic:23896"]
The problem started ever since I installed the new vesc x. So here's the deal, when I start riding my board (dual raptor, Enertion) and want to brake, they're extremely abrupt. Just one millimeter on the controller and you almost fall off the board. Then after riding it for a bit, say 5-10 minutes, the brakes become very smooth as they should be and you can finally ride the board safely and comfortably.
[/quote]

Nano-X remote right?

try this:

-Board off
-Turn remote ON, push and pull throttle to the max both sides. leave idle
-turn ON board
```

---
## \#3 Posted by: evoheyax Posted at: 2017-05-25T19:49:58.077Z Reads: 103

```
What is your batt regen setting?

For example, if it was at 20a and you lowered it to 15a, you might not notice much of a difference, as they are both a very high setting for a dual drive.
```

---
## \#4 Posted by: makevoid Posted at: 2017-05-25T19:56:09.314Z Reads: 99

```
edit: this is not the solution - I had the same problem too lol - blasto solved our issue

----

you could tune down the motor min / batt regen settings as @evoheyax is saying which will get the braking force down overall

or you could charge the battery to ~95% instead of 100% 

also you could try ackmaniac's firmware with watt control mode which is not using current control (amps) but directly Watts (watt control mode) so that the braking force is the same at max and normal voltage
```

---
## \#5 Posted by: Kasper Posted at: 2017-05-25T19:56:15.262Z Reads: 99

```
@Blasto Nano-X indeed. I will try your solution but why should this work? And do I have to do that always?
@evoheyax  My regen setting was 12A (I set it up like this according to the vesc FAQ thread from this site) but now I tried 7A this works but I only notice the difference after riding for about 5-10 min. So this setting does not change my issue.
```

---
## \#6 Posted by: Blasto Posted at: 2017-05-25T19:58:27.759Z Reads: 98

```
[quote="Kasper, post:5, topic:23896"]
Nano-X indeed. I will try your solution but why should this work? And do I have to do that always?
[/quote]

yes everytime you go to ride. Because of the autobind feature, the remote also recalculates it's extreme's every power cycle.
```

---
## \#7 Posted by: evoheyax Posted at: 2017-05-25T20:00:10.116Z Reads: 97

```
That is pretty normal, so yea, you have something else going on...

Just throwing it out there, maybe try like 3a or even less? You might not have brakes though after 10 minutes of riding though...

I would trust @Blasto should be able to help you though, as he understands this stuff to a higher degree than me and most in the community.
```

---
## \#8 Posted by: Kasper Posted at: 2017-05-25T20:02:05.591Z Reads: 93

```
Sounds reasonable to me. Great I'll try it out. The only thing is that I got this issue after installing the new vesc-x. At that point I already had the Nano-X controller. Any thoughts on that?
```

---
## \#9 Posted by: Blasto Posted at: 2017-05-25T20:04:44.621Z Reads: 90

```
[quote="Kasper, post:8, topic:23896, full:true"]
Sounds reasonable to me. Great I'll try it out. The only thing is that I got this issue after installing the new vesc-x. At that point I already had the Nano-X controller. Any thoughts on that?
[/quote]

could your habits have changed? maybe before you were squeezing your throttle and brakes before jumping on it.
```

---
## \#10 Posted by: fraannk Posted at: 2017-05-25T20:06:29.667Z Reads: 84

```
I have to do exactly the same with the Nano-X. Full throttle, full brake and then ready to go :)
```

---
## \#11 Posted by: Kasper Posted at: 2017-05-25T20:07:56.678Z Reads: 83

```
Could be indeed. But now I come to think of it, mostly after 5-10 min I've pushed the controller at least once to full throttle and full brake so your theory should be right. Its only strange that no one else has noticed this then with the Nano-X.
```

---
## \#12 Posted by: Kasper Posted at: 2017-05-25T20:09:00.881Z Reads: 80

```
Oops posted just too early :p so there are more of us having this issue..
```

---
## \#13 Posted by: Tuomalar Posted at: 2017-05-25T20:11:58.063Z Reads: 77

```
It's more like feature than issue with nano-x.
```

---
## \#14 Posted by: Blasto Posted at: 2017-05-25T20:14:09.063Z Reads: 77

```
I have to admit it's a strange feature, but i guess you will always have your range of throttle in the case some obstructs the travel of the trigger? or could be a manufacturing thing, where they are not dependent on the tolerances of the pots

the work around is easy enough to not care

try it, report back
```

---
## \#15 Posted by: Kasper Posted at: 2017-05-25T20:20:13.972Z Reads: 81

```
Will do! Thanks so far for your help :smile:
```

---
## \#16 Posted by: Kasper Posted at: 2017-05-25T21:01:37.683Z Reads: 79

```
So, tried it. And it works!! So much much more fun and comfortable to ride it now. Now I can really hit the road. Thanks again for your help. Too bad only that Enertion couldn't solve it and that this is not in the manual..
```

---
## \#17 Posted by: makevoid Posted at: 2017-05-26T06:50:40.124Z Reads: 57

```
@Blasto @Kasper
  
wow, really? I have the the nano-x too... now that I think about it it happens to me as well and I never thought it was caused by the remote itself! I had to reduce the braking force to prevent too hard  brakes ^^ thanks for spotting it - I'll try this trick for my next ride!

edit: yes that solves my issue as well, many thanks!
```

---
