# How to balance charge a 12s battery pack

### Replies: 27 Views: 2078

## \#1 Posted by: uigiroux Posted at: 2018-03-10T17:16:07.495Z Reads: 167

```
I'm about to start building on a few battery packs for my new build and I have one issue that I haven't quite figured out yet, so I'm hoping you guys can provide the answers.  So, these packs are going to be 12s4p, and what I am having trouble with is in regards to balance charging these.  From what I understand, the highest number of series that can be balanced is 10.  I've seen they used to offer some chargers that would go above, but they didn't work well, and are no longer offered.  On a YouTube video I saw,  a man solved this by simply making the connection in the center no longer connected, thus giving 2 separate batteries now 6s4p.  One thing I want with my setup is to basically never need to open it again, so any port or connector, all be wired to the enclosure so I can plug everything I need to it.  So is there a way to say, make 2 6s4p packs (or whatever size, mainly anything over 10s) and have 2 charging ports, one for each, yet use only 1 BMS for them?  Or is this something that I'd need 2 BMS's, and to go inside the board each time to deal with balancing....?
```

---
## \#2 Posted by: Colson003 Posted at: 2018-03-10T17:18:10.112Z Reads: 158

```
Why not use a 12s BMS? You’d have just one charging port.
```

---
## \#3 Posted by: uigiroux Posted at: 2018-03-10T17:21:07.815Z Reads: 161

```
Well yes I will most likely do that, but sometimes they aren't very reliable, and balance charging specifically from that type of charger is best.
```

---
## \#4 Posted by: Colson003 Posted at: 2018-03-10T17:24:43.045Z Reads: 158

```
You may get better balancing from a balance charger but then the cells aren’t protected while discharging. 

@mmaner has some coming that would would great with a 4p pack

http://www.electric-skateboard.builders/t/bestech-bmss-10s-12s-charge-discharge-with-e-switch/48611
```

---
## \#5 Posted by: uigiroux Posted at: 2018-03-10T17:27:38.977Z Reads: 145

```
Oh?  I just looked at that post a few min ago.  Those are bestech right?  Is that the best brand for BMS's?
```

---
## \#6 Posted by: onepunchboard Posted at: 2018-03-10T17:27:49.779Z Reads: 140

```
if you make paralle 6s charging lines in addition to 12s line, you can use cheap rc charger. 

which im doing. 
now u have 4 charging port to deal with
```

---
## \#7 Posted by: uigiroux Posted at: 2018-03-10T17:29:34.877Z Reads: 137

```
I didn't really understand what you said... Could you rephrase that please, lol.
```

---
## \#8 Posted by: Colson003 Posted at: 2018-03-10T17:30:08.050Z Reads: 133

```
Yes those are bestech, best brand for bms? I can’t say, but I know a lot of people use them and I haven’t seen any issues. That specific model has an e-switch so there’s no need for an anti-spark switch or loop key.
```

---
## \#9 Posted by: uigiroux Posted at: 2018-03-10T17:33:28.924Z Reads: 127

```
Oh well I really love that, I was reading that thread where all the anti spark units were all failing..
```

---
## \#10 Posted by: deucesdown Posted at: 2018-03-10T17:34:06.388Z Reads: 127

```
There's a few approaches, but BMS will be more convenient.

1. 12s balance charger. there are a small handful.

2. break connection at middle, charge as 6s

3. put 12s bms on charger side

4. find a separate battery balancer

For #1, you can do tricks, like breaking the series connection with a loop key that's panel mounted.
```

---
## \#11 Posted by: Namasaki Posted at: 2018-03-10T17:35:03.376Z Reads: 124

```
[quote="uigiroux, post:9, topic:48705, full:true"]
Oh well I really love that, I was reading that thread where all the anti spark units were all failing…
[/quote]

Stand alone E-switches are notorious for failure but the Bestech built in E-switch is dependable
```

---
## \#12 Posted by: mmaner Posted at: 2018-03-10T17:38:51.052Z Reads: 110

```
Yep, BesTech BMS's.  The best BMS's in my opinion.
```

---
## \#13 Posted by: onepunchboard Posted at: 2018-03-10T17:38:54.319Z Reads: 112

```
So you can make 12s battery and outputs 48v
and if you hi jek between the 6s cell make additional line of balancing cable and charging port, now u have 1+4= 5 power port 

it is a bit complex system hard to describe in words.
I think I can build a switch btween 12s and 2*6s for additional safety

but u can charge quick safe and cheap. and you dont have to open the box ever. 

drawback is now you have 4 ports outside instead of 1.
and if you dont have cover ports can damage and corrode from water.
```

---
## \#14 Posted by: deucesdown Posted at: 2018-03-10T17:42:32.498Z Reads: 105

```
[quote="deucesdown, post:10, topic:48705"]
For #1, you can do tricks, like breaking the series connection with a loop key that’s panel mounted.
[/quote]

I should mention, you don't have to break the connection if you charge 6s at a time. If you try to series or parallel charge two 6s packs that are still connected 12s, you'll probably see fireworks, from the common ground somewhere.

here's a picture of a really well done split 6s trick (might not be 6s) with ebike. Follow the link in the link for more detail

https://endless-sphere.com/forums/viewtopic.php?f=2&t=45009#p677161

http://static.electricbike.com/wp-content/uploads/2012/04/P1000089.jpg

http://static.electricbike.com/wp-content/uploads/2012/04/P1000094.jpg
```

---
## \#15 Posted by: uigiroux Posted at: 2018-03-10T18:16:18.416Z Reads: 96

```
So basically, I shouldn't worry about it as long as I have a proper BMS then?
```

---
## \#16 Posted by: uigiroux Posted at: 2018-03-10T18:20:57.521Z Reads: 93

```
I guess I could build 2 packs each with its own BMS and then connect them with one of those 3 sided series connectors, and each charging port would be able to balance, I'd just need to connect an extra set of sensor wires for each pack to also be hooked up when balancing. So there should be a set going to the BMS and another could be mounted to the enclosure for balance charging.
```

---
## \#17 Posted by: deucesdown Posted at: 2018-03-10T18:22:36.633Z Reads: 92

```
BMS is not magic -- you should always worry. There are many failure modes BMS won't help you with.

And I'll caution once more (I couldn't understand what you were saying). If you try to charge 2 subpacks that are still series at the same time (with 2 chargers, or with parallel charging), it'll most likely blow up due to shared ground.
```

---
## \#18 Posted by: uigiroux Posted at: 2018-03-10T18:24:58.639Z Reads: 91

```
Well yeah, that's why I'm asking about balance charging, without the BMS.  If I thought that then I wouldn't concern myself with this stuff.
```

---
## \#19 Posted by: uigiroux Posted at: 2018-03-10T18:33:28.490Z Reads: 84

```
If I was to have 2 separate packs with 2 separate chargers, I would connect them with a series connector, but disconnect them when charging.  (to avoid the shared grounding)
```

---
## \#20 Posted by: uigiroux Posted at: 2018-03-10T19:22:42.199Z Reads: 82

```
Do any of you guys run a 12s, and if so, how do you charge... or rather, do you charge it any differently than normal?
```

---
## \#21 Posted by: PXSS Posted at: 2018-03-10T19:49:27.460Z Reads: 84

```
My old RC chargers didn't go above 8S. 
Here is what I used to do to charge higher packs:

You need to have 2 independent batteries:

Battery 1: Main negative needs 2 wires, one connected to ESC connector ground and second to charging connector 1 ground. On the positive side, you need a single wire to charging connector 1 positive. 

Battery 2: Main negative needs 1 wire connected to charging connector 2 ground. On the positive side, you need 2 wires, one to ESC connector positive and one to charging connector 2 positive. 

To charge, you connect charging connector one to one charger and charging connector 2 to another charger (or 1 per channel on a dual charger)

To turn on, you need to connect charging connector one positive to charging connector 2 negative. Yes, it doubles as a loopkey. 

You also need one balance connector per battery. 

I'll draw a diagram in a few minutes.

E: Here it is,
![image|666x500](upload://s0TaTmPKzRhtKld9w19OvbWpYn3.jpeg)

So battery 1 is the top row of cells and battery 2 is the bottom. I bought one black and one yellow set of XT60s so I would not confuse them when plugging in the loop key, but it would not matter if you did. The board would simply not turn on.

You also do not need a connector between the ESC and the battery but I had one since it was just a temporary solution
```

---
## \#22 Posted by: deucesdown Posted at: 2018-03-10T20:09:01.013Z Reads: 76

```
Nice artwork :) If you look at the photos I posted above, that block is the loop key, and it blocks the balance ports. It serves as a mechanical lockout so you can't connect both.
```

---
## \#23 Posted by: uigiroux Posted at: 2018-03-11T01:27:48.116Z Reads: 69

```
That's a perfect solution!  I'm gonna do that, thanks!
```

---
## \#24 Posted by: uigiroux Posted at: 2018-03-11T01:30:03.819Z Reads: 68

```
So if I leave the loop key in, it's one pack and I charge from one port, and if I remove it it's two packs and I could just a balance charger on both charge ports. Right?

At least, that's what it looks like to me...  Could I use one 12s BMS or would I need two 6s BMS?
```

---
## \#25 Posted by: ROFEN13 Posted at: 2018-03-11T01:44:07.812Z Reads: 67

```
I did this on my build. I made 2 6s4p and have all connections on the outside. Loop key connects the packs together in series.
```

---
## \#26 Posted by: PXSS Posted at: 2018-03-11T01:46:08.520Z Reads: 68

```
Ish...

[quote="uigiroux, post:24, topic:48705"]
So if I leave the loop key in, it’s one pack and I charge from one port
[/quote]
Yes, you could charge from the ESC port but you would not be able to balance unless you made a harness that joined the two balance plugs. 

[quote="uigiroux, post:24, topic:48705"]
and if I remove it it’s two packs and I could just a balance charger on both charge ports. Right?
[/quote]
Yes. But if you have a harness joining the balance plugs together and try to charge, you would blow up something. 

[quote="uigiroux, post:24, topic:48705"]
At least, that’s what it looks like to me…  Could I use one 12s BMS or would I need two 6s BMS?
[/quote]
As long as you disconnect the BMS harness from the battery to charge the 2 packs individually, you can use a 12S. Having 2 6S BMS would overly complicate things
```

---
## \#27 Posted by: deucesdown Posted at: 2018-03-11T02:17:02.847Z Reads: 65

```
If you do 12s BMS don't bother with all the rest of this -- it takes a surprising amount of room to make all these splices and connections. Just check cell voltages somewhat frequently with a volt meter until you develop some trust. IMO.
```

---
