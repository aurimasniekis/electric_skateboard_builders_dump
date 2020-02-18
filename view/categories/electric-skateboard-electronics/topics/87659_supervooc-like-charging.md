# SuperVOOC like charging

### Replies: 21 Views: 211

## \#1 Posted by: directC Posted at: 2019-03-19T18:53:51.231Z Reads: 70

```
Hi all

I recently found out about oppo's supervooc charging (for smartphones)

The company puts 2 batteries in the device, so it can load them simultaneously, thus needing only half the time (actually even less)  
The charger outputs 10V/5A which get pushed in 2x 5V batteries

I'm not the best in electric circuits, so sorry i'll write complete BS

I thought, we could do that for our eskates too

Let's say we have 2 12S batteries and a 24S bms in the board

Connect it like this:  
![IMG_20190319_200459|281x500](upload://oFXaSQS5bb2NmTK0IpwwcGocWrp.jpeg)       

So AC to charger  
charger to bms  
bms to batteries in serial     

the batteries have the connection for the bms to charge, but also a connection to the vesc which you use like a loop-key  
Instead of just looping one wire out and back in, you need 1 (let's say male) plug for the 2 + wires and 1 (male) plug for the 2 - wires  
you build an 1 (female) to 2 (male) plugs adapter (a bit bulkier than a normal loop key) and that's it  
you still only need 1 antispark plug, the female one

What do you guys think?  
Did I make any mistake?
```

---
## \#2 Posted by: Sn4pz Posted at: 2019-03-19T18:55:47.713Z Reads: 66

```
I think you should take the time to draw these diagrams out in paint or a similar software. My electronically challenged eyes and brain assumes there is some sort of formatting issue, or at least the pictures would make it more clear
```

---
## \#3 Posted by: directC Posted at: 2019-03-19T19:07:38.116Z Reads: 57

```
updated
10ch
edit: damn, can i turn a picture somehow?
```

---
## \#4 Posted by: Pedrodemio Posted at: 2019-03-19T19:12:59.285Z Reads: 56

```
I saw some videos about SuperVOOC, my impression is that they are just taking advantage for the lack of knowledge of most people to pass it as something new

The thing is, the limitation is the battery itself, it doesn't matter if the series parallel arrangement, the speed will be the same

That being said, in a phone environment, where the cables wouldn't be capable of handling 10A/5V, it helps

But the main innovation here is not the charging scheme, but the battery being able to take that much current, supposedly without much degradation, only time will tell 

Now bringing this to our use case, it doesn't make much sense, if you have a 24S battery, is way easier to get a 24S charger than make all the switching for 24 cells

How much current we can pass through a charge cable it's not limited like on mini/micro USB cables
```

---
## \#5 Posted by: b264 Posted at: 2019-03-19T19:13:21.734Z Reads: 41

```
As soon as you plug in the ESC you will short the batteries and they will burn using that wiring.

For faster charging, just use a higher current charging system.  Most builds aren't charging at their battery's rated charge current.  It does reduce battery lifetime a bit to push charging rates to the limits.
```

---
## \#6 Posted by: Andy87 Posted at: 2019-03-19T19:14:12.112Z Reads: 42

```
I would say it makes a big boom when you connect it like that.
![image|522x500](upload://oojHJgiwzcLD5YUbG5Pu51YeJWH.jpeg)
```

---
## \#7 Posted by: directC Posted at: 2019-03-19T19:16:39.564Z Reads: 37

```
does the bms connect it? even when not loading?
else you need a loopkey for charging :rofl:

Edit: or did you think i connect the 2 battery leads before the xt90?
```

---
## \#8 Posted by: directC Posted at: 2019-03-19T19:19:43.604Z Reads: 36

```
but you can't use a 24S battery without stepping it down (or at least i don't know the components for it, but you get what i mean)
```

---
## \#9 Posted by: Andy87 Posted at: 2019-03-19T19:21:51.343Z Reads: 36

```
I took out my Picasso skills and made a small redrawing of your drawing.
Hope like this it’s more understandable.
Maybe I got your drawing wrong, but if you first put the packs in series and than in parallel you short out your pack. Doesn’t matter how much loopkeys you use.
![image|375x500](upload://hbEUNvpjWTPRxCR24dvl1RGBBXn.jpeg)
```

---
## \#10 Posted by: directC Posted at: 2019-03-19T19:22:50.996Z Reads: 34

```
so the bms is always connecting?
```

---
## \#11 Posted by: directC Posted at: 2019-03-19T19:26:22.101Z Reads: 33

```
So a charging loopkey

![51|375x500](upload://fnATsSzeZnseJ7qjrcY5VJVIfA7.jpeg)
```

---
## \#12 Posted by: Andy87 Posted at: 2019-03-19T19:28:15.198Z Reads: 27

```
I don’t look at the bms at all.
Just your main power leads.
If you wire it up like you was drawing it the + of the first 12s pack is on the same connection like the - of the first pack. It’s a direct short of plus and minus.
```

---
## \#13 Posted by: Sn4pz Posted at: 2019-03-19T19:29:44.046Z Reads: 24

```
Keep trying Andy youll get through eventually :disappointed_relieved::joy_cat:
```

---
## \#14 Posted by: directC Posted at: 2019-03-19T19:33:35.861Z Reads: 26

```
Whoops...
Why does elecricity never do what I want it to. 
Is smart electricity already invented? 😁
```

---
## \#15 Posted by: Andy87 Posted at: 2019-03-19T19:33:42.157Z Reads: 27

```
Looks a bit like a moonface ... sorry @moon no connection to you 😅
But look the blue marked connection
![image|387x500](upload://yJh7RY0Mw8CcuZkdOldPDC611vy.jpeg) 

It’s the same potential.
If you solder there a wire which than goes to the plus xt90 you short the first pack
```

---
## \#16 Posted by: Andy87 Posted at: 2019-03-19T19:36:30.851Z Reads: 24

```
I in general don’t see a reason for all that troubles.
Why not to get 2x12s packs, wire them in parallel and just double the charger amps.
🤔 easy peasy and takes half the time charging as well.
```

---
## \#17 Posted by: directC Posted at: 2019-03-19T19:39:22.562Z Reads: 25

```
The meaning is to have a 12s pack, not a 24s, which charges at half the time without using to much amps to preserve the batteries
```

---
## \#18 Posted by: b264 Posted at: 2019-03-19T19:41:53.763Z Reads: 25

```
It's not going to save you anything that way.  You'll be charging at half the amperage, but also charging half the cells -- so the per-cell charge current will be exactly the same.
```

---
## \#19 Posted by: Andy87 Posted at: 2019-03-19T19:42:43.753Z Reads: 25

```
😅 ok ähm ja...so lets come back to the basics.
If you wire up 2x 12s in parallel it’s still 12s.
I think that’s clear right?
If you have a 12s2p the charging current is going to be half half for each parallel pack.
So 8a Charger would mean 4a for one pack, 4a for the other pack. 
I don’t see any problem with that.🤔
```

---
## \#20 Posted by: directC Posted at: 2019-03-19T19:49:36.174Z Reads: 24

```
Damn, you're right
So oppo just does it bc of the heat and little battery
So for eskates is useless

And I thought I have a good idea 😩
```

---
## \#21 Posted by: directC Posted at: 2019-03-19T19:52:25.340Z Reads: 24

```
But i'm still curious how oppo connects everything
```

---
