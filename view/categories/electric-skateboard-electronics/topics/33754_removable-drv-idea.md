# Removable drv idea

### Replies: 24 Views: 794

## \#1 Posted by: pat.speed Posted at: 2017-09-23T03:54:33.916Z Reads: 159

```
Ok, so I keep seeing people blowing the drv chips and I've heard they are annoying to replace so would it be possible to somehow use an Ic chip holder to hold the drv chip. That way if you blow it you can just pop it out and put in a new one. I think others have probably thought of this and there will be some sort of reason why it won't work
```

---
## \#2 Posted by: scepterr Posted at: 2017-09-23T03:58:51.786Z Reads: 160

```
I've lost count how many times this has been brought up lol...the way the chip works, it's not feasible for it to be removable. It's already plagued by distance and noise and would only be exponentially worse. Also for the people making and selling vescs there's no incentive...for them it's not an issue
```

---
## \#3 Posted by: pat.speed Posted at: 2017-09-23T04:13:15.646Z Reads: 155

```
Ahhh ok 

10 chars
```

---
## \#4 Posted by: Pantologist Posted at: 2017-09-23T04:41:18.880Z Reads: 145

```
I think the biggest issue is that the chip holder would not be reliable with the amount of vibrations in an esk8 application. Failure rates would end up being higher than they are now.
```

---
## \#5 Posted by: scepterr Posted at: 2017-09-23T04:44:32.747Z Reads: 141

```
If that was the only issue it could be solved with a levered plate and locking pin holes like cpus have in desktops
```

---
## \#6 Posted by: Pantologist Posted at: 2017-09-23T04:54:19.908Z Reads: 135

```
Good point. But yeah the effort to do all that takes up lots of space and it will still not perform as well as directly being soldered.
```

---
## \#7 Posted by: pat.speed Posted at: 2017-09-23T06:18:09.223Z Reads: 127

```
Hmm ok so that's a no go then
```

---
## \#8 Posted by: chuttney1 Posted at: 2017-09-23T06:21:45.021Z Reads: 119

```
Even if it is possible, Texas Instrument would not spend a single cent to produce a DRV830X chip in the QIP format if the big buyers don't shell out dollars for it.
```

---
## \#9 Posted by: pat.speed Posted at: 2017-09-23T06:23:55.378Z Reads: 115

```
um I'm not sure what QIP means
```

---
## \#10 Posted by: chuttney1 Posted at: 2017-09-23T06:26:00.714Z Reads: 114

```
Sorry, it's Quad In-Line Package. 

Wiki page as a reference. https://en.wikipedia.org/wiki/Dual_in-line_package

 I'm sure this is what you meant with removable chips
```

---
## \#11 Posted by: pat.speed Posted at: 2017-09-23T06:28:25.197Z Reads: 107

```
Yes it was. I though we might be able to just bend the pins but probably not. I looked up QIP on google and it came up with 'quality improvement plan'😂 I thought you were nuts
```

---
## \#12 Posted by: scepterr Posted at: 2017-09-23T08:57:48.448Z Reads: 96

```
Well lol I think you're the first to think of trying to bend the pins on the existing chip...that's unique 🤣
```

---
## \#13 Posted by: pat.speed Posted at: 2017-09-23T11:15:54.132Z Reads: 82

```
😂 Yeah most of the stuff I build is 'unique' because I haven't a lot of money for specialised parts so I modify lots of random bits and bobs
```

---
## \#14 Posted by: ThierryGTLTS Posted at: 2017-09-23T15:44:40.505Z Reads: 66

```
Hi ,

You forgot to say where and how you'll attach the PowerPad that is used to spread the heat!!!

Thierry
```

---
## \#15 Posted by: pat.speed Posted at: 2017-09-23T23:18:01.153Z Reads: 49

```
I am not sure what a power pad is but I'm guessing kinda like a heat sink. Yes that is another problem so this will definitely not work😂
```

---
## \#16 Posted by: scepterr Posted at: 2017-09-23T23:19:43.673Z Reads: 49

```
The pad on the underside of the chip that gets soldered, not just the pins, thus the whole bendy pin idea is rather silly 😉
```

---
## \#17 Posted by: pat.speed Posted at: 2017-09-23T23:24:14.943Z Reads: 49

```
So that's what the bottom soldered pad thing is. I have heard people saying that it is almost impossible to solder with a normal iron.
```

---
## \#18 Posted by: scepterr Posted at: 2017-09-23T23:25:24.010Z Reads: 51

```
Uhm without damaging the chip I would say it is impossible with a soldering iron. A fat chunky soldering iron sitting on the chip would eventually solder the ground pad but after killing the chip, you could do it with a blow torch...it'll also solder the ground pad but destroy everything else 🤣 The right tool for the job is best.
```

---
## \#19 Posted by: pat.speed Posted at: 2017-09-23T23:27:19.184Z Reads: 49

```
Ok, well this idea was really bad and I now know why nobody as made this happen😂
```

---
## \#20 Posted by: chuttney1 Posted at: 2017-09-24T01:53:19.187Z Reads: 45

```
I would at least thing soldering the ground pad of the DRV with being made easier if the ground pad was extended outward, so heat from the solder conducts to the ground pad.
```

---
## \#21 Posted by: FredSaberhagen Posted at: 2017-09-24T02:39:47.604Z Reads: 39

```
This is not a bad idea.  A daughter board holding the drv and MCU would get it out of the current path.  Heat could be managed, height might be an issue?
```

---
## \#22 Posted by: pat.speed Posted at: 2017-09-24T04:21:41.199Z Reads: 33

```
Hmmm, yes maybe something like an arduino board with the chip and anything else it needs, then we wouldn't have the pins problem. It wouldn't need the heat spreader and you could even solder the pins to make sure they don't come out. The only problem left is the noise and distance @scepterr was talking about
```

---
## \#23 Posted by: scepterr Posted at: 2017-09-24T04:42:25.609Z Reads: 31

```
The daughter board idea has been discussed as well...
```

---
## \#24 Posted by: scepterr Posted at: 2017-09-24T04:49:45.866Z Reads: 32

```
There's nothing stopping anybody from redesigning the vesc with more than enough capacitance, diodes and filters to never ever fry a drv, itll just cost twice as much and take up twice the space atleast.
**AKA VESC6** 

If cost isn't a factor a military grade vesc is possible.
```

---
