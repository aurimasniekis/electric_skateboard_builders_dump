# Little help with focbox settings

### Replies: 36 Views: 449

## \#1 Posted by: Bobby Posted at: 2019-02-23T02:02:15.181Z Reads: 121

```
What settings would be causing my board to suddenly decelerate when i try to accelerate at high speed? Right now its at 
40 
-40 
30 
-20 
and
 120 total

I also have it im sensored bldc. My biggest concern is that my current battery for this build is a diyeboard battery. I don’t know the specs of it and what i can set my settings to.
```

---
## \#2 Posted by: AlanZhou Posted at: 2019-02-23T02:14:59.744Z Reads: 117

```
it would be helpful it you tell us the rest of your setup... but that -20a seems a bit on the high side, are you bypassing bms for discharge?

[quote="Bobby, post:1, topic:85086"]
diyeboard battery
[/quote]

or you got got a crappy bms
```

---
## \#3 Posted by: briman05 Posted at: 2019-02-23T02:57:59.373Z Reads: 108

```
I was thinking the same do maybe -10
```

---
## \#4 Posted by: Bobby Posted at: 2019-02-23T02:58:03.003Z Reads: 104

```
Dual 6355 tb motors and two vesc x... the recommended was -12 but im pretty much guessing with the numbers
```

---
## \#5 Posted by: briman05 Posted at: 2019-02-23T02:59:13.554Z Reads: 100

```
What is the max amps for motors that is what you would set for motor max like 60a
```

---
## \#6 Posted by: Bobby Posted at: 2019-02-23T03:00:17.566Z Reads: 100

```
I have em at 40 max amps
```

---
## \#7 Posted by: briman05 Posted at: 2019-02-23T03:01:13.458Z Reads: 96

```
That shouldn’t be the motors max though my 5065 have a max of 46a
```

---
## \#8 Posted by: Bobby Posted at: 2019-02-23T03:01:22.747Z Reads: 90

```
The deceleration only happens if i full throttle gun it already going fast... kinda feels like the battery isn’t providing enough juice for that burst. Once i let go of the throttle i can accelerate like normal
```

---
## \#9 Posted by: AlanZhou Posted at: 2019-02-23T03:15:20.735Z Reads: 87

```
Its definitely the bms, diyeboard batts use bms for charge and discharge, too much currect back into the battery can cause cutouts (not related), surpassing the bms ratings for your bursts can also cause cutouts.
```

---
## \#10 Posted by: AlanZhou Posted at: 2019-02-23T03:16:07.860Z Reads: 84

```
mabye take the heatshrink off of the diyeboard pack and bypass the bms for discharge. dont push it though the cells arent that good.
```

---
## \#11 Posted by: Bobby Posted at: 2019-02-23T03:20:27.691Z Reads: 82

```
Im just glad its not my settings. This board is mre for cruising than speed.  I just noticed it on testing it when doing the full speed attempt
```

---
## \#12 Posted by: dareno Posted at: 2019-02-23T09:19:29.682Z Reads: 74

```
What diye battery do you have.  Its all about the battery.  Everything is the battery.  First and foremost the battery.  Life is the battery.
```

---
## \#13 Posted by: SeanHacker Posted at: 2019-02-23T09:21:32.660Z Reads: 71

```
[quote="dareno, post:12, topic:85086"]
Its all about the battery. Everything is the battery. First and foremost the battery. Life is the battery.
[/quote]

You get it. I like that. A lot.
```

---
## \#14 Posted by: Bobby Posted at: 2019-02-23T09:21:49.093Z Reads: 67

```
10s5p but i think its the older Samsung version. Got a 12s4p and 10s5p 30q coming. I honestly figured that was it. Its my only diyeboard part left
```

---
## \#15 Posted by: dareno Posted at: 2019-02-23T09:34:03.292Z Reads: 63

```
Let me tell you a little story.  All those diye batteries with their lovely integrated bms's are rated for the esc's they are supplied with.  Those esc's only draw, note draw, the amps that they can cope with.  You try to pull anything over 20amps per side and the bms will pop.  Trust me on this.  Just because its a 25r 5P battery makes no difference when the esc only draws 18A per motor.  Chinese being the chinese will only supply a bms capable of those draws.  They don't care that you might then go and mate it up to a unity or focboxes capable of ripping amps from them in spades.  The battery will rely on  its shit cheap nasty bms to tell you to fuck off.  I have killed 2p 3p and indeed 5p bms's with after market vesc.  Re wire the thing with a bestech charge only d140 and then you can up the draw to the batteries capacity.

Then it will sag like a witches tit though
```

---
## \#16 Posted by: Jebe Posted at: 2019-02-23T09:40:17.929Z Reads: 59

```
after googling "sagging like a witches tit" I have to agree with this guy. that battery is great for powering your 12 volt radio up the beach.
```

---
## \#17 Posted by: dareno Posted at: 2019-02-23T09:44:34.479Z Reads: 60

```
[quote="Jebe, post:16, topic:85086"]
with this guy.
[/quote]

you fucking sure with this guy????   I will find you at the ettamoga pub

Nice to know you're still about btw
```

---
## \#18 Posted by: Bobby Posted at: 2019-02-23T09:46:30.747Z Reads: 58

```
So with the new bms, how long would it go until voltage sag hits? What should my settings be?  Would a 30 dollar bms even be worth the spend on this battery?
```

---
## \#19 Posted by: Deckoz Posted at: 2019-02-23T19:07:09.403Z Reads: 53

```
[quote="dareno, post:15, topic:85086"]
Then it will sag like a witches tit though
[/quote]

[quote="Jebe, post:16, topic:85086"]
googling “sagging like a witches tit”
[/quote]

Wizard Sleeves.
```

---
## \#20 Posted by: Sn4pz Posted at: 2019-02-23T21:13:16.278Z Reads: 47

```
Is your 120 total the Absolute max?

Ive seen people edit that value and then their vesc behaves irregularly, I usually just keep it at 130A as thats the default

![image|545x159](upload://vB6FGDap1gcnpfNHjpMZk6WCYPG.png)
```

---
## \#21 Posted by: Sn4pz Posted at: 2019-02-23T21:16:06.410Z Reads: 46

```
I used mine to draw its full 50a for a few rides, but used it at 40a for the rest of its existence... I think that sometimes these issues are a little over exaggerated in their quantity, but they speak the truth about the catastrophe that is battery failure.... 

:man_shrugging:
```

---
## \#22 Posted by: Bobby Posted at: 2019-02-23T21:29:41.481Z Reads: 46

```
Changing it back tonight. On a side note, any recommendations for micro usb extensions. Id like to have a little slot so i dint hve to open then enclosure for things like this...
```

---
## \#23 Posted by: b264 Posted at: 2019-02-23T21:51:08.008Z Reads: 45

```
Fill out all the values in the calculator and send us the link so we can see what you have going on

https://calc.3dservisas.eu/
```

---
## \#24 Posted by: b264 Posted at: 2019-02-23T21:53:14.882Z Reads: 45

```
[quote="Bobby, post:14, topic:85086"]
Samsung version
[/quote]

***When a vendor only tells you the brand of the cells and not which cells they are, the vendor is shady as fuck*** and you should not do business with them.

That's like saying I'm selling you a "Ford" vehicle.  Despite Ford making Pintos and Mustangs, but I don't tell you which vehicle.

So, I'm going forward with the assumption that you're talking about Samsung 15L cells unless I find out otherwise.
```

---
## \#25 Posted by: dareno Posted at: 2019-02-23T23:00:14.908Z Reads: 39

```
[quote="Bobby, post:22, topic:85086"]
any recommendations for micro usb extensions.
[/quote]

I use RS pro version with a waterproof cap
https://www.alliedelec.com/rspro-1116750/71038923/
```

---
## \#26 Posted by: Bobby Posted at: 2019-02-23T23:23:36.988Z Reads: 38

```
I got this battery from a shady fuck, who got it from shady fucks.... there is a reason i plan on replacing it lol
```

---
## \#27 Posted by: Sn4pz Posted at: 2019-02-23T23:26:55.689Z Reads: 39

```
Theyre 22p, assuming the pack youre talking about is the 'regular' diyeboard pack
```

---
## \#28 Posted by: Bobby Posted at: 2019-02-24T02:47:07.828Z Reads: 37

```
@b264  this is what i am setting it to? Any suggestions u![image|374x500](upload://96s8aov9EireaBcnpz7wrmIHAHc.jpeg)
```

---
## \#29 Posted by: b264 Posted at: 2019-02-24T03:06:53.397Z Reads: 37

```
It sounds like it could be either max erpm backoff or a saggy battery but I don't have a lot of information.  We don't know your motor kv or gearing ratio or wheel size.  (I didn't see [the calculator filled-out](https://www.electric-skateboard.builders/t/little-help-with-focbox-settings/85086/23?u=b264))

Try starting with

Motor
30
-30
Battery
12
-5

That should be SUPER slow but it should WORK.  If not, start troubleshooting.  If it works, increase the Motor maximums to 50, -50 and see if that works.  Your top end throttle and brakes will be weak but the bottom-end should be good.  If that works try increasing the battery max and see if the problem comes back.  If so, it's a battery issue... lower the battery numbers until the problem goes away, then lower a bit more, then go battery shopping.

And search before you buy from diyeboard.  They are known scammers.
```

---
## \#30 Posted by: dareno Posted at: 2019-02-24T03:12:51.262Z Reads: 37

```
[quote="b264, post:29, topic:85086"]
They are known scammers.
[/quote]

This is very true.  I have 3 batteries from diye and they all are different with regard to workmanship
One was so bad I binned it.  The 2p and 3p are very well built though just crappy cells and cheap bms's.  They work if you don't push them too hard.
```

---
## \#31 Posted by: b264 Posted at: 2019-02-24T03:22:58.527Z Reads: 36

```
Did someone ask what your battery cutoffs were set at yet?
```

---
## \#32 Posted by: Bobby Posted at: 2019-02-24T03:55:44.848Z Reads: 35

```
33 start 31 end. 15/36 with 97mm wheels and 190kv 6355.... im 90% sure its the battery. I actually did not purchase this from diyeboards. Someone sold it to me telling me they had made a custom board only to find out i was scammed and paid double for a diyeboard kit.... lets just say after tons of reading, ill never get scammed again.... im still very new to electricians jargon. Ohms, amps, voltage,watts.... its hard for me to grasp at it at times.... Im actually getting a 12s4p 30q fixed with a new bms and a 10s5p on its way from thisguyhere... I guess what confuses me the most ks what the numbers represent. Is the motor side how much is being taken and returned by the motors to the focbox and the battery max and min how much powere the focbox takes and gives back to the battery?
```

---
## \#33 Posted by: Bobby Posted at: 2019-02-24T04:42:03.112Z Reads: 33

```
So I realized i had a really old firmware installed. I just updated them and redid everything usin ackmaniacs bldc tool... will that make an improvement?
```

---
## \#34 Posted by: b264 Posted at: 2019-02-24T04:57:28.644Z Reads: 34

```
Probably not, but it can't be ruled it out.  I personally have been using the Vedder VESC Tool and haven't tried the 2019 versions yet.
```

---
## \#35 Posted by: Bobby Posted at: 2019-02-25T03:10:56.909Z Reads: 26

```
So i set my motors at 50 -50 and my batt 40 -15.... i used ackmaniacs fw and honestly, everything worked great! No issues at high speed. I still cant go from zero throoto full blast without some sag but i never have want to do that anyways lol. Thanks for your help guys!!  Cant wait to start this next few builds :)
```

---
## \#36 Posted by: b264 Posted at: 2019-02-25T03:19:25.381Z Reads: 27

```
[quote="Bobby, post:35, topic:85086"]
I still cant go from zero throoto full blast without some sag but i never have want to do that anyways lol.
[/quote]

LoLz every time the electric traffic signal turns green and I don't want the cars running me off the road.  They are shocked every time that you can go just as fast as they can.
```

---
