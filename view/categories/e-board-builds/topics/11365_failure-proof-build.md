# Failure proof Build

### Replies: 31 Views: 2184

## \#1 Posted by: willpark16 Posted at: 2016-10-18T18:10:00.461Z Reads: 269

```
So I am looking to make a final build Ive been doing a few for other and my personal I managed to fix up and get running again which was 6s 10000mah 245kv. I've been learning and building electric skateboards for about 1.5 years nowand Now I'm ready to build one of the best that can be made. A few questions though for the community about the most efficient and durable parts. dual or single? Im thinking single since it consumes less current and increases battery life, however there is also hub motors but are they currently efficient? From what I am able to deduce they are less efficient than a pulley driven system. Then for the esc Im thinking about either the vesc or fvt 12s however the vesc has not been known for long life, but I also know that @chaka  has made some that have lasted people years. Finally the battery, is 12s truly more efficient than 10s? I know increased voltage means more efficiency but is that truly the case if you're putting more stress on the components at that voltage? Im willing to put in around 2000 maybe more if necessary, what I truly want is something that can just function as well as a boosted but as powerful as a DIY build.

Edit: Its not that I don't know what to do, its more so everyone has their own viewpoint and id like to learn from everyone mistakes, and you can never truly know it all.
```

---
## \#2 Posted by: ajaynagra Posted at: 2016-10-18T18:32:20.752Z Reads: 260

```
Best batteries @barajabali
```

---
## \#3 Posted by: sl33py Posted at: 2016-10-18T18:44:03.151Z Reads: 252

```
Sounds like a fun project/build.  I'm mostly on the same page as you myself w/ a few projects in progress.

I would start like a newbie with requirements based on your weight and riding style/area.  Heavy/light rider, hills/flats, and type of ride (commute/cruise/race), etc.

I like the stealth and simplicity of hubs in theory, but mostly i don't trust the bearings and wear/life of a hub for a big guy like me.  So currently sticking with satellite motors w/ belts like most.

For this monumental build - i would build on the best i could find - Ollin's VESC, or wait for v6.  Heatsinks and warranty just make it a no-brainer.  Especially if you stick to BLDC and <60k ERPM.  If you want to push the envelope and run FOC i might wait for v6.

10s vs 12s - depends on motor kv.  if you can get your ERPM below 60k i'd go as high voltage as possible.

batteries - barajabali, miami electric, DIYes, SPACE cell - li ion sounds like a great way to go.  I'm in the process of building a 10s or 12s3p...  fun project, but not saving any $ when you factor in spot welder and materials/tools!  Going to do a removable pack w/o BMS and balance on my existing chargers.

Will definitely follow - GL!
```

---
## \#4 Posted by: willpark16 Posted at: 2016-10-18T19:03:48.353Z Reads: 224

```
thanks! I weigh only 120 and 10 percent is hills the rest downhill and flat So assuming single motor 10s with what kv
```

---
## \#5 Posted by: willpark16 Posted at: 2016-10-18T19:04:53.683Z Reads: 217

```
he was going to fix up my 6s pack
```

---
## \#6 Posted by: barajabali Posted at: 2016-10-18T19:08:54.283Z Reads: 212

```
Do you still need that done? 
Waiting for your response
```

---
## \#7 Posted by: sl33py Posted at: 2016-10-18T19:09:20.431Z Reads: 206

```
for a build that should last you i would go past 6s and look at 10/12s.  depending on motor kv you want/have.

for your weight a single will make a ton of sense.
```

---
## \#8 Posted by: Pantologist Posted at: 2016-10-18T19:20:57.692Z Reads: 204

```
Switch to 10S get a Vesc. For your weight and limited hills, you can make a great board with $1000. Either dual hubs or a single 63mm. 

If you want something like a Boosted at that price. You can always buy one ;)

If you want more of a Boosted experience, you'll need a set of high end components like a smart BMS, Bluetooth module and functional smartphone app. That's my goal atleast.
```

---
## \#9 Posted by: NickTheDude Posted at: 2016-10-18T19:38:31.687Z Reads: 195

```
I'd go with VESCs and Dual 190kV 6355s at 12S. 

It's important to keep the amps low in the VESC since that's where most of your losses come from. Using 12S will allow you to use a lower kV motor, therefor pulling less amperage for a given RPM, this is what makes it more efficient. 

You're aiming for 60k ERPM and I'm pretty sure the VESC's max voltage is 12S, so 190kV gets you really close to that 60k limit. That's right where you want to be since these motors are more efficient in higher RPMs.

I also think dual motors would put less stress on each motor, and the VESCs since you'd only be using half the amps.
```

---
## \#10 Posted by: longhairedboy Posted at: 2016-10-18T20:00:20.826Z Reads: 187

```
yep. What @NickTheDude said. 

and do everything possible to prevent shorts. if you have pins poking wires, file them down, etc. Use a silicone sealer or silicone foam gasket on your enclosure and you'll never have to worry about crud in your box, and if you run your phase leads Raptor style then do your best to wrap up those connections. plug up your charge port if possible and if you go with a push button on your eswitch get a heavier one with a satisfying click. You can tell the ones that won't hold up just by holding them in your hand and feeling the "thickness" of the click. Try to use a P count in your pack that gives you higher continuous current draw than you'll ever need, and go with a BMS that slightly lower than that but still delivers more than you'll need. I use 80amp continuous packs and 60amp continuous BMSs for example so the pack never even gets warm. Belt drives will probably hold up better on shitty sidewalks and crap pavement.
```

---
## \#11 Posted by: Hummie Posted at: 2016-10-18T20:48:11.839Z Reads: 174

```
not that it's necessarily the case but a hub motor should be more failure proof as it has less parts to break, less parts to maintain.  Many other parts that will deteriorate while a hub motor should only have to have the bearings replaced.  Using a belt the first thing to go will likely be the belt, then maybe the mount when it bottoms out, ..pulley wheels in aluminum maybe next.  then the grub screw gets lost or stuck.
```

---
## \#12 Posted by: willpark16 Posted at: 2016-10-18T21:11:53.464Z Reads: 166

```
still deciding weather I want you to just make me a new one or not
```

---
## \#13 Posted by: barajabali Posted at: 2016-10-18T21:18:40.443Z Reads: 159

```
You could take the opportunity to upgrade
```

---
## \#14 Posted by: willpark16 Posted at: 2016-10-18T21:19:24.015Z Reads: 154

```
can u salvage the cells from the 6s 4p or should i just have u do an entirely new one
```

---
## \#15 Posted by: willpark16 Posted at: 2016-10-18T21:29:48.687Z Reads: 153

```
Hey @Namasaki how do you feel safe wise charging lipos, do u feel comfortable doing it at work with a bms?
```

---
## \#16 Posted by: willpark16 Posted at: 2016-10-18T21:39:18.592Z Reads: 152

```
any issues running 12s and 190kv?
```

---
## \#17 Posted by: barajabali Posted at: 2016-10-18T21:39:51.957Z Reads: 146

```
How used are they
```

---
## \#18 Posted by: willpark16 Posted at: 2016-10-18T21:40:09.068Z Reads: 147

```
4 full recharges
```

---
## \#19 Posted by: Namasaki Posted at: 2016-10-18T21:58:14.184Z Reads: 141

```
I always charge mine at home. 
I don't charge them overnight while sleeping. 
I keep an eye on them while charging.
```

---
## \#20 Posted by: barajabali Posted at: 2016-10-18T22:20:42.676Z Reads: 142

```
Ehhhh I mean. I suppose you could if you want to save some money... what cells are they? Lg he2? Or he4?
```

---
## \#21 Posted by: willpark16 Posted at: 2016-10-18T23:44:27.432Z Reads: 128

```
Lg he2 but if u don't think it will work just tell me
```

---
## \#22 Posted by: barajabali Posted at: 2016-10-19T01:07:48.141Z Reads: 129

```
It will work. 

Its just the cheaper way of going. out with the old in with the new
```

---
## \#23 Posted by: longhairedboy Posted at: 2016-10-19T14:45:36.682Z Reads: 127

```
you're probably right about the hubs at this point, in the past though they didn't seem to hold up as well against the constant clack clack clack clack of the sidewalks according to things i've read.
```

---
## \#24 Posted by: Hummie Posted at: 2016-10-20T03:28:11.235Z Reads: 118

```
I feared a magnet coming loose but haven't heard of any in the 140 I sold. They haven't been out there that long but a relief.  The windings and leads breaking has happened to me and at least one other person and the rubber...especially the rubber.  I wonder what other hub motors are selling as their rubber.   A bigger motor that will keep cooler like lever's have really nice rubber and they stay cool enough, because they're so big, but all those little motors out there.  I just saw 70mm wheels on Acton or whatever they're called'S site.  But I did also see their new four wheel vehicle has what look like nitrile tires 
Nitrile is really nice.  Really nice. But greater rolling resistance.  Since ur not pushing much and there's still a bit of resistance with the motor then it's hard to notice but it's there on paper and probably in miles to watt hours.   I'm syched to soon be pouring "hot pour " polyurethane thats also intended for high heat.  Really excited to see how it does.  Polyurethane and nitrile have a lot of the same wear characterisitcs, they're both tough, but the rebound of a good hot pour polyurethane skate wheel is so nice.
```

---
## \#25 Posted by: willpark16 Posted at: 2016-10-25T15:58:13.225Z Reads: 116

```
Update: vesc has been ordered, and will be selling a few intresting parts to raise a few more funds for the board. The deck is either going to be custom or I will use my bustin deck. Caliber 50's for trucks, I have 83mm wheels and 97mm so Ill decide between the two later on which to use. Black Enerion mount!!! (will post pictures). Motor, and battery are still being determined however!!!!!! Would anyone be intrested in a black tacon 245kv motor(yes it is just painted black the coated with polyestrylene but it can be removed if wanted...
```

---
## \#26 Posted by: willpark16 Posted at: 2016-11-03T06:49:05.496Z Reads: 111

```
@torqueboards @ajaynagra @Pantologist @barajabali @Namasaki @sl33py @oriol360 so i now have $350 to spend on a new battery and esc, and apologies if I am a bother, just let me know and I'll stop tagging u. But after extensive research and talking to different sellers my original 12s 2p oriol pack with a tb esc won't work. I now have to find an alternative, I wanted to use the tb esc due to it being basically bullet proof, however reviews with running this esc and li ion packs haven't been too good. So I have two options for escape thanks to @barajabali I can get the tb esc for 80 or my friend will give me his unused ollin vesc for 80. That leaves me with 270 ish dollars to spend on my battery which has to be li ion due to safety. Almost forget to mention I need the parts by Wednesday!!!! Any help u guys can offer or insight is much appreciated. I just cannot have this setup fail like my 6s4p
```

---
## \#27 Posted by: sl33py Posted at: 2016-11-03T14:55:29.574Z Reads: 94

```
Personally if you have an option for an Ollin VESC for that cheap - get it.  Assuming it wasn't thrashed and is working well.

Wednesday?!  Dude - you are going to be lucky to get this by then.  Your best bet is DIYes (@Torqueboards), or MEB (@oriol360) - talk w/ them and see if they can expedite to you.  BUT being batteries they're usually limited to ground shipping (not allowed on planes afaik).  So even getting that going right away it might not be doable.   Your profile doesn't note your location (and i'm not fully awake (no coffee yet) and didn't read above again) - so it might make more sense to order from whichever is located closest to you.  DIYes is West coast SF/CA, MEB is Miami/FL i believe.  Shouldn't forget @barajabali who is in Chicago (love that town, just not this time of year!).  As he builds custom i'm not sure he's in your budget though...

Failure proof and "can't have this setup fail" - a word of warning.  Electronics fail.  Mechanics fail.  You cannot build anything that will be 100%.  You can minimize likelihood of failure, but everything has wear/tear/friction and will break at some point.  Good maintenance, good quality components to start, and frequent checking will all help.  but it'll still break.  If you want to go super anal you can log miles and replace wear items at a certain interval (like airlines do on airplanes), before they are likely to break... but they can still fail before then.

HTH - GL!
```

---
## \#28 Posted by: Namasaki Posted at: 2016-11-04T01:51:18.723Z Reads: 72

```
An Ollin Vesc for $80. Better jump on that.
And don't even think about trying FOC mode.
Stick with BLDC for Bullet Proof operation.
Also, when deciding on voltage and motor KV, stay bellow Vesc 60K ERPM limit for bullet proof operation.
I've been running 10s with 190KV on BLDC mode and its been flawless.
Even when jamming up hills, my motors barely get warm. And there is plenty of power and speed.
```

---
## \#29 Posted by: willpark16 Posted at: 2016-11-04T01:54:28.632Z Reads: 68

```
Tacon 245kv spacecell pro 3 and tb esc or vesc?
```

---
## \#30 Posted by: TarzanHBK Posted at: 2016-11-04T10:58:40.550Z Reads: 66

```
245kv is too high for a 10s spacecell.
190kv 10s is optimal.
```

---
## \#31 Posted by: evoheyax Posted at: 2016-11-05T22:14:19.467Z Reads: 63

```
[quote="Namasaki, post:28, topic:11365"]
And don't even think about trying FOC mode
[/quote]

It's an ollin vesc, so FOC is not an issue. I have 8 in FOC, and have switched back and forth with no issues.

Plus if something breaks, chaka will take care of you.
```

---
