# Vesc killed by Swiss slopes?

### Replies: 36 Views: 554

## \#1 Posted by: Balta_6 Posted at: 2019-02-24T21:26:43.980Z Reads: 221

```
Hi guies, I think I killed a vesc 4.12 recently (boohoo), or did I ?
Well I was riding in some slopes next to my house, gently braking (and I'm more your +60kg shrimp that calls itself human) and boom, brakes stopped and nothing responded...
Back home, the vesc couldn't connect to my computer and not light was showing...
Buuuut, after checking closely the vesc, it seems fine, DRV and mostfets looks okay

I don't really not what to look at, or measure with a voltmeter to check if its dead or not, so if some of you could help me with this !
Thanks :cat: (here's a cat)
```

---
## \#2 Posted by: Balta_6 Posted at: 2019-02-24T21:27:30.201Z Reads: 215

```
Well, don't mind me, just posting pictures !
![IMG_20190224_221300|666x500](upload://8TzUUgh5UpvHXqm41uw7puN2BHb.jpeg) ![IMG_20190224_221310|666x500](upload://tsBXRbBiLMtAMREutfvErqkwgIs.jpeg)
```

---
## \#3 Posted by: Mich21050 Posted at: 2019-02-24T21:31:24.603Z Reads: 199

```
Calling the wizard @JohnnyMeduse (sorry for tagging you again :slight_smile:)
```

---
## \#4 Posted by: AlanZhou Posted at: 2019-02-24T21:37:13.404Z Reads: 187

```
some of your soldering looks really freaky with that glue, also im guessing this is a may tech vesc.
```

---
## \#5 Posted by: Mich21050 Posted at: 2019-02-24T21:40:22.142Z Reads: 186

```
![Screenshot_1|690x331](upload://aSz5XNguyPQzI7nyHvRjtL7cx6t.png) 
This looks really sketchy.. Do you remember which settings you used? :slight_smile:
```

---
## \#6 Posted by: Balta_6 Posted at: 2019-02-24T21:45:49.131Z Reads: 175

```
Haha it is, very very bad thing I made for the bluetooth module, but except the hot glue, it's okay, and I've ridden this a lot, no problemo
let me remember this : 
motor current max : 60A
motor current max brake : -12A
battery current max : 60A
Battery regen : -20A (not sure about this)

Need anything else ?
```

---
## \#7 Posted by: Mich21050 Posted at: 2019-02-24T21:46:54.027Z Reads: 163

```
I'm not sure if mt vesc's can handle 60A. Also what battery were you using? (s count) :slight_smile:
```

---
## \#8 Posted by: Balta_6 Posted at: 2019-02-24T21:48:32.163Z Reads: 163

```
Hmm I know they're rated for 50A but I heard 60A is fine for it 
Battery is a 10S4P from 30q, with a 60A bms
```

---
## \#9 Posted by: Mich21050 Posted at: 2019-02-24T21:50:41.292Z Reads: 159

```
I think you smoked it with 60A and 10s. As far as I know, only the focbox is fine with 60A.. :slight_smile: 
But can you measure the output of your battery (just to be sure) :slight_smile:
```

---
## \#10 Posted by: Balta_6 Posted at: 2019-02-24T21:51:18.236Z Reads: 155

```
Yeah maybe... but why did it died when breaking, why a this very moment ? weird
```

---
## \#11 Posted by: Mich21050 Posted at: 2019-02-24T21:52:43.389Z Reads: 147

```
[quote="Mich21050, post:9, topic:85267"]
But can you measure the output of your battery (just to be sure) :slight_smile:
[/quote]
Maybe you smoked your bms. Do you know the rating of it? (charge/discharge)
```

---
## \#12 Posted by: Balta_6 Posted at: 2019-02-24T21:54:20.155Z Reads: 137

```
60A discharge
But no, I check the voltage and it still show a normal amount
Just checked with a 3s lipo lying around, the vesc doesn't light up, so it's the vesc not the battery (thanks god, such a pain in the ass the battery)
```

---
## \#13 Posted by: Mich21050 Posted at: 2019-02-24T21:54:49.738Z Reads: 131

```
I'm pretty sure you smoked your battery.. :slight_smile:
```

---
## \#14 Posted by: Balta_6 Posted at: 2019-02-24T21:56:25.102Z Reads: 129

```
The fact that it still sparks when I plug it without an antispark tells otherwise
```

---
## \#15 Posted by: Mich21050 Posted at: 2019-02-24T21:58:11.366Z Reads: 131

```
That just means that there's a potential difference between both. And some components might still work but I have no idea what exactly is broken... Maybe someone can answer that for you.. :slight_smile:
```

---
## \#16 Posted by: Balta_6 Posted at: 2019-02-24T21:59:48.968Z Reads: 126

```
Well I have other vesc lying on my desk, but I'm too lazy to unscrew my lid off, so I'll probably do it tomorrow or something 
Thanks for your help, I appreciate it
```

---
## \#17 Posted by: JohnnyMeduse Posted at: 2019-02-25T13:53:28.749Z Reads: 96

```
OK... Late to the party.

@Balta_6 Is the Blue light on the vesc still light up (sorry if had been said earlier)?
```

---
## \#18 Posted by: Balta_6 Posted at: 2019-02-25T14:26:17.880Z Reads: 85

```
No no light at all...
```

---
## \#19 Posted by: JohnnyMeduse Posted at: 2019-02-25T14:36:53.581Z Reads: 85

```
I think it might be either a blown Can receiver or a MCU.

The first thing to check is if you have a short on C25. 

https://www.electric-skateboard.builders/t/no-power-to-enertion-vesc/7600/8?u=johnnymeduse
```

---
## \#20 Posted by: Balta_6 Posted at: 2019-02-25T14:37:44.658Z Reads: 80

```
is it possible to have blown a can receiver in single ? Would be surprising but why not
```

---
## \#21 Posted by: JohnnyMeduse Posted at: 2019-02-25T15:10:06.517Z Reads: 70

```
Yes... It would be quite surprising!! 

C25 is on the 3.3V, same line as the CanTransceiver and the MCU. Since you’re running a single motor setup, sadly it is most likely a Blow MCU.
```

---
## \#22 Posted by: Balta_6 Posted at: 2019-02-25T15:40:00.112Z Reads: 66

```
Okay, will try that when I'm home !
I just use the multimeter as an ohmmeter, and look for an abnormal value ( which should be ...?)
```

---
## \#23 Posted by: JohnnyMeduse Posted at: 2019-02-25T16:23:13.391Z Reads: 65

```
What Value did you get? 

I was just thinking about it, but one more thing you could check is the 5V. The easy way is to plug a receiver and check if it light up.
```

---
## \#24 Posted by: AlanZhou Posted at: 2019-02-25T16:36:44.664Z Reads: 63

```
You should not be pushing 60a continuous on any vesc 4.12 without cooling, my TB vesc was suffering at 30a

My focbox couldn't even do 50a without throttle I only managed to push 45a on enertion hubs (basically a 6374)
```

---
## \#25 Posted by: Balta_6 Posted at: 2019-02-25T17:38:44.659Z Reads: 56

```
Yeah, I did that and it was beeping, lightly but it was there (and no light from the receiver)
So it shorted out ?
Any idea why ? Just general wearing out ?
Anything doable for it to save it (non expensive or hugely time consuming)
Well thank you !
```

---
## \#26 Posted by: Balta_6 Posted at: 2019-02-25T17:39:29.924Z Reads: 56

```
I never ridden at those amount of amp, it's just the max setting, most of the time I can't go over 30 amp, even pushing it a lot (I'm light so that helps)
```

---
## \#27 Posted by: JohnnyMeduse Posted at: 2019-02-25T21:44:44.448Z Reads: 49

```
[quote="Balta_6, post:25, topic:85267"]
So it shorted out ?
[/quote]

Resistance need to be 0ohm for a short. 

But If the receiver doesn't light up also, that does mean that the 5V isn't working, which could be a dead DRV.

Maybe you could check with the multi-meter if you have a 5V, if you have nothing it is probably the DRV that is Blown
```

---
## \#28 Posted by: AlanZhou Posted at: 2019-02-26T02:40:59.817Z Reads: 42

```
on startup you will exceed 60a by a wide margin, I pull 85a on startup (on one focbox) for 3 secs and im only 115 pounds

oh and i feel stupid for guessing its a maytech because it is and it says (mt) on the top of the vesc :man_facepalming:
```

---
## \#29 Posted by: Sn4pz Posted at: 2019-02-26T02:46:05.960Z Reads: 43

```
[quote="AlanZhou, post:28, topic:85267"]
I pull 85a on startup (on one focbox) for 3 secs and im only 115 pounds
[/quote]

 What the hell, Ive never pulled max amps unless im starting UP a hill... o.O
```

---
## \#30 Posted by: AlanZhou Posted at: 2019-02-26T02:52:25.104Z Reads: 40

```
mabye?? huh thats what my app says, but my abs is limited at 80a, but mabye its raptor hubs, i measured it and its bigger than a 6374
```

---
## \#31 Posted by: Balta_6 Posted at: 2019-02-26T06:45:50.679Z Reads: 30

```
So weird, but no I've never gone all the way to the max in terms of amp, only got 83 mm wheels for 65kg, 60A would launch in the air :wink:
```

---
## \#32 Posted by: Balta_6 Posted at: 2019-02-26T06:46:58.284Z Reads: 30

```
Will check that tonight too !
Maybe it's that, so it's been due to a bad parameters
```

---
## \#33 Posted by: ARetardedPillow Posted at: 2019-02-26T06:58:58.361Z Reads: 29

```
Here's your issue ![image|665x500](upload://yT5MrYb8HAboGNeEXhru8Sc7lse.jpeg)
```

---
## \#34 Posted by: Balta_6 Posted at: 2019-02-26T09:23:09.145Z Reads: 26

```
the blob of solder is not where it should be ?
Weird how it got here, and weir that it didn't cause problems before, I havent solder the vesc or heat it enough to melt the solder...
```

---
## \#35 Posted by: lrdesigns Posted at: 2019-02-26T09:34:21.816Z Reads: 27

```
I think @ARetardedPillow is saying because its maytech brand its naturally gonna blow up. Which is not true unless you use FOC mode, that will blow them up for sure. They run fine in BLDC.
```

---
## \#36 Posted by: Balta_6 Posted at: 2019-02-26T10:32:58.355Z Reads: 22

```
Yeah I know that, no FOC on this one
I bought it from eskating even, sad it broke like that
```

---
