# Did I ruin my focboxs

### Replies: 22 Views: 927

## \#1 Posted by: Hummie Posted at: 2018-03-08T21:20:34.876Z Reads: 160

```
I plugged them both into the battery backwards!  spark...and then had to do it again to make sure and a big spark.   both of them have just the blue light going and seem ok except when I do foc testing the resistance number and the inductance are fluctuating and not passing the bldc test either.  how do you check for faults?
```

---
## \#2 Posted by: RedEagle Posted at: 2018-03-08T21:21:33.329Z Reads: 155

```
Do they connect to bldc tool?
```

---
## \#3 Posted by: Hummie Posted at: 2018-03-08T21:22:00.704Z Reads: 152

```
yes they seem good and normal except those two things
```

---
## \#4 Posted by: RedEagle Posted at: 2018-03-08T21:22:34.286Z Reads: 151

```
Did you type faults in the terminal tab?
```

---
## \#5 Posted by: Hummie Posted at: 2018-03-08T21:22:54.593Z Reads: 147

```
that's what I need to do.  wheres the terminal tab? found it
```

---
## \#6 Posted by: Hummie Posted at: 2018-03-08T21:23:30.528Z Reads: 145

```
none.  no faults
```

---
## \#7 Posted by: RedEagle Posted at: 2018-03-08T21:23:36.224Z Reads: 144

```
Right next to the firmware tab if I'm correct.
```

---
## \#8 Posted by: Hummie Posted at: 2018-03-08T21:24:17.719Z Reads: 144

```
makes no sense that resistance could double between testing
```

---
## \#9 Posted by: RedEagle Posted at: 2018-03-08T21:25:04.773Z Reads: 143

```
1. Connect them to pc.
2. Check ppm tab for ppm signal input (does it move when you push throttle?)
3. Do a few bench tests with remote
4. Check again for faults
```

---
## \#10 Posted by: Blasto Posted at: 2018-03-08T21:28:49.947Z Reads: 140

```
everyone was so flabbergasted by this (myself included, i see it now)

![image|586x441](upload://8bqDqiqfX0CYtX6mp6BJKTM0xIV.jpg)

didn't even notice that the polarity was reversed

small chance that the TVS diodes saved you... but they are probably busted
```

---
## \#11 Posted by: Hummie Posted at: 2018-03-08T21:31:14.529Z Reads: 134

```
yup that was it!.  

strangely I get different resistance doing the foc test when I hold the rotor fixed or let it move. 3x differences.  maybe that's just how it works and my real problem is the bell is slightly held back from hard epoxy on the rotor and a tiny airgap...or no airgap in place.  So  I have other things that could be the cause other than the focboxs.  they seem fine otherwise.
```

---
## \#12 Posted by: Hummie Posted at: 2018-03-08T21:32:00.766Z Reads: 132

```
@Blasto so what you think.  even if the diodes are shot am I ok
```

---
## \#13 Posted by: RedEagle Posted at: 2018-03-08T21:32:58.362Z Reads: 129

```
You should be fine.
```

---
## \#14 Posted by: Blasto Posted at: 2018-03-08T21:33:34.172Z Reads: 124

```
[quote="Hummie, post:12, topic:48524"]
the diodes are shot am I ok
[/quote]

maybe not shot... depends how long you held the power in place. but the size of the spark probably scared the shit out you lol (it's a dead short)
```

---
## \#15 Posted by: RedEagle Posted at: 2018-03-08T21:35:15.867Z Reads: 120

```
Check battery cells for voltage. You have a very real chance of cells being under 1v.
```

---
## \#16 Posted by: Hummie Posted at: 2018-03-08T21:35:27.071Z Reads: 120

```
does the changing resistance while doing the foc set-up make sense?  connections are all pretty solid and it will fluctuate all over...but if I hold the rotor still vs let it rotate a bit while doing the resistance test it makes a big difference.  I wouldn't think the rotor would be at all involved in the resistance test
```

---
## \#17 Posted by: Hummie Posted at: 2018-03-08T21:35:46.804Z Reads: 119

```
they're good.  17 v on the realtime data with 4s....actually that's higher than it really is.  hummm
```

---
## \#18 Posted by: RedEagle Posted at: 2018-03-08T21:38:07.017Z Reads: 115

```
The test should be done with motor spinning freely. As far as resistance goes. I don't know if it's good or bad. It makes sense that you get different readings under different load. With load the focbox has to work harder to get the motor spinning.
```

---
## \#19 Posted by: Hummie Posted at: 2018-03-08T21:39:21.844Z Reads: 114

```
but resistance being electrical resistance of just two or one phase (I think it does one)...the rotor isn't important.  I'll test with rotor off.   

strange how it shows my battery like a volt and a half high
```

---
## \#20 Posted by: RedEagle Posted at: 2018-03-08T21:42:30.241Z Reads: 104

```
Hmm.. very bad sign it is.. doing extensive testing before risking your life on that plank of death you must..
```

---
## \#21 Posted by: RedEagle Posted at: 2018-03-10T20:31:13.566Z Reads: 67

```
Did you solve the problem? If so, it may be a good idea to mark the reply that solved it as a solution.
```

---
## \#22 Posted by: Hummie Posted at: 2018-03-14T20:33:15.414Z Reads: 46

```
send them to @JohnnyMeduse to look at them.  one was getting hot just doing testing on the table.  surprised they didn't explode really

ears are ringing!
```

---
