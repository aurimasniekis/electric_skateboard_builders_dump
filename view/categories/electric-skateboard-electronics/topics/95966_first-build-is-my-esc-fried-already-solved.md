# First build, is my ESC fried already? \[Solved\]

### Replies: 9 Views: 414

## \#1 Posted by: plurf Posted at: 2019-06-05T20:55:27.155Z Reads: 114

```
Hello all!

So after monthes of wandering and reading (as a guest tho), days of parts harvesting and hours of soldiering my board is (almost) finished. 
But obviously it doesn't turn on...
Well i have a led flashing once on the esc and the power switch, and then back to nothing.

Well let's start from the beggining : i got a cheap board from internet something cold Helvei Smartmove (for like 250$).
It's basically a rebranded Liftboard dual motor, as far as i could tell, which is pretty similar to benchweel but the esc and bms seems different.
Out of the box everything worked just fine, even though i tryed it like five min in my kitchen.

Because i had to travel by plane, i could not take the battery (nor all the big things) so i dismounted it and let behind the battery, the deck and the metal enclosure.

i don't really now what motor it is but they are tagged as 2*900W belt driven
The battery was a 6s4p (22v 8.8Ah), i made up a new one from an electric bycicle one, so i now have a 6s2p (22v 13Ah) with big flat cells instead of classic samsung accus.
The BMS was a bit weird to me because the negative battery wire was a small red wire among the whites balance ones and not a big and sturdy one. Plus it seems like a custom thing with two spareted board one over another, and it has in addition a specific 5v (i guess because when i test it, the voltmetre stay blank when the esc is off) out for the controller.

The motor and mechanical parts looks good quality as much as i could tell, the blets are tight and everything seems good and new.

The ESC seems a lot better than most of the chinese or RCcars one i saw on the net (big and clean) you can see it on the pictures bellow. I didn't find any similar one on the net so far, and i've been trying a lot.

So basically i did all the mecanic, i did all the battery and soldiering thing (even if the esc was looking weird i got a good 24.4v out of the battery and a stable 21.6v out of the BMS), plugged everything...
When i press the button, one led on the ESC (see the pictures) and the button itself flash red (like really quick, a third of a second) and then back to nothing. 
I thought it could have been the "5v" input which didn't seems to work, but i tested it while clicking the button: it seems to get alive for the flashing time but not long enough to get an actual reading.

I spent the day plugging/unplugging, resoldiering stuff and looking for ints over the internet, but still the same.

I don"t know if the ESC is fried, but the flashing thing makes me hope it's not. It could be the battery also, but i don't know how. 
(i tried pluging it to the charger, it says green and nothing happens, but i'm pretty sure the cells were all fully charged before i made it so it doen't mean anything) I doesn't have an other one to test.

I hope one of you could have a int of what is the problem or how to test it up...
And if you think that the ESC is definitely fried, which one could i get on a budget ? (already went to more expenses than i thought buying decks and batteries...)

Thank you!!

![closeUp|375x500](upload://37CUy38uxxbImit9gI9RtubDsUN.jpeg) ![total|375x500](upload://kJDmbEgmkA0QnQBosGgDhKBSCIF.jpeg)
```

---
## \#2 Posted by: briman05 Posted at: 2019-06-06T03:11:23.945Z Reads: 82

```
Well first what gauge are the wires for the motor. As they look way to small. I would say you have gotten your money’s worth out of the parts. To get a reliable board you have to spend the money for it. Get a vesc look at the flipsky vesc if you want one on a budget.
```

---
## \#3 Posted by: plurf Posted at: 2019-06-06T11:02:41.265Z Reads: 71

```
@briman05 
Well they seem to me more or less as big as the power input ones, they are rated 250°C
![esc|281x500](upload://4oq1JALpOBmtEuspTjSvxsEm0js.jpeg) 

Is there a way to test if it's really dead?
What do you think about the ownboard ones that are not as fancy but half the price ?
thanks
```

---
## \#4 Posted by: briman05 Posted at: 2019-06-06T12:05:20.589Z Reads: 60

```
Ownboard is like all the other low price boards just good luck getting any customer service. If it was a vesc you would connect it to the vesc tool and type fault in the terminal. I have never seen that esc.
```

---
## \#5 Posted by: plurf Posted at: 2019-06-09T18:54:40.241Z Reads: 51

```
Update : it was definitely the BMS, i finally found the (b-) wire totaly riped away, changing it and rearanging the order of the balance wires did the trick. I ordered for a new ESC anyway, so i could do some tests. Thanks.
```

---
## \#6 Posted by: DeathByBacon Posted at: 2019-06-09T19:41:58.282Z Reads: 42

```
What ESC is this? Do you have a link?
```

---
## \#7 Posted by: plurf Posted at: 2019-06-09T19:54:57.907Z Reads: 42

```
I have no idea, the board was this one : http://helvei.com/product/smartmove-longboard/ . i can't tell if it's the same hardware as the Liftboard but the design seems the same from the outside
```

---
## \#8 Posted by: hyprlite Posted at: 2019-07-20T00:11:10.020Z Reads: 27

```
Had to search around but I knew I've seen that ESC somewhere.. 
https://www.electric-skateboard.builders/t/various-used-and-unused-esk8-parts-for-sale/48198

On another note, if I may hijack the thread for a moment, it's my first post so I thank you for your knowledge and help. I've been lurking and reading for weeks now regarding this same issue and I'm still a little lost. I'm running the Liftboard Dual but mine isnt like the other ones which I find is common practice with these cheap completes. Everything has worked great on mine, no cut out issues, no power sag, no motor mount problems so I want to keep it and am willing to spend a few bucks repairing it.
My power ring flashes red rapidly until I turn it back off, I can hear the motors turn on when the power button is pressed and the motors move freely.

Total noob here so go easy on me, apologies for the hijack. Just unsure what went wrong here and what my next move is or which part needs replacing. I'm not in love with the metal housing and may make a custom one so size isnt too much an issue with replacement parts.

Thanks in advance!

I'm new so I can only add one photo at a time, this is my ESC ![20190716_190510|375x500](upload://km56y2Fv3b9wAOhAETKSH72d4uq.jpeg)
```

---
## \#9 Posted by: Money Posted at: 2020-01-11T00:47:35.943Z Reads: 11

```
Hey Plurf,

Sorry for not seeing this sooner. 

Hopefully you found a solution by now. But, I have a bunch of these ESC’s. They are indeed Liftboard ESC’s.

Honestly, i’d suggest using a vesc over these any day. 

But that means you’d also need to order a remote and receiver that work with the vesc. And costs can add up fast. But if a project is worth doing, it’s worth doing right. Especially if you’re going to be trusting the technology with your safety. 

That being said, if you are at all interested in a replacement ESC, i got you. It does require a willingness to DIY and a healthy dose of determination. 

During the time I worked for them, Liftboard made lots of changes to their protocols, code, hardware and more, which resulted in numerous versions of the Liftboard. Unfortunately, these changes made the various parts incompatible across different versions. To make things worse, they weren’t labeling or marking the boards to indicate which version each board was. 

The reason i’m saying this is cuz I honestly do not know which version ESC you would need. The LB ESC’s all look fairly similar. But some LB remotes may not be compatible with some LB ESC’s. So you’ll need to do some trial and error.

I’m not certain how many LB ESC’s I have. I’d guess about 8-10. Maybe more. 

If you want them, their yours.

Again, i’d Suggest a VESC over these if you can afford it. If not maybe these will help. 

If you want them send me a DM and i’ll take care of it. 

I’ll even pay the shipping for the esc’s. 

If you need other parts let me know. Again, not selling you anything. Just would like to help.
```

---
