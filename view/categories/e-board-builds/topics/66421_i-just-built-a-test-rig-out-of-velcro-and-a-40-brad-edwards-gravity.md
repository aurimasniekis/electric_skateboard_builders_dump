# I just built a test rig out of velcro and a 40&rdquo; brad edwards gravity

### Replies: 36 Views: 926

## \#1 Posted by: longhairedboy Posted at: 2018-08-28T23:26:41.544Z Reads: 233

```
![14|667x499](upload://8HEMXez3li2I4JWzPmqRRcMVKn0.jpg)

I got tired of not having an easy way to just attach things and test them. I remembered a long time ago @lowGuido did this to one or more of the boards in his giant pile of esk8s  so i did the same. 

The only thing that's semi permanent here is the drive train, though swapping belts and pulleys and wheels is as easy as always.

The important thing here is i can test any pack with any ESC and any receiver, and even try different eswitches or bluetooth units or whatever else i want just by plugging it in and sticking it on and strapping velcro over it. So now FlipSky and the like will get all of my opinions a little faster. 

The picture above doesn't have the blanket of velcro covering everything so you can see what's up, but after i strapped it all down i picked the board up several times to shoulder height and just dropped it.  Nothing came loose. However, this is by no means weather proof so dry days only. 

At the moment I have a pair of 10Ah Tattu 25C 6S lipos in series with a Y connector going straight into a FlipSky FSESC4.20 dual ESC that they sent me, running 3.40. Used VESC-Tool to set it up, no issues at all. Running sensored FOC. 

No eswitch, no volt meter, not even an antispark plug. 

Its fucking raining right now. I'm so pissed. I know this monster will move like a motherfucker. If anything can dump enough current to melt this flipsky its these Tattus, and i want the pcb on fire before i start sending opinions.
```

---
## \#2 Posted by: longhairedboy Posted at: 2018-08-28T23:29:56.967Z Reads: 210

```
Oh yeah: for wire management on the back i have one of those RipTide channel risers. They're 1/2" height. On the front i have a 1/4" Indy riser.
```

---
## \#3 Posted by: Saturn_Corp Posted at: 2018-08-28T23:35:31.011Z Reads: 205

```
I have velcro holding my focboxes to my board and even had a 10s2p attached the same way. It's stronger stuff than you'd think.
```

---
## \#4 Posted by: longhairedboy Posted at: 2018-08-28T23:38:14.631Z Reads: 194

```
Its serious shit for sure. None of this shit is moving at all.
```

---
## \#5 Posted by: PatRocks Posted at: 2018-08-28T23:39:35.636Z Reads: 187

```
Love to see the tattu lipos! Mine have been KILLIN it for a year and a half, no signs of aging
```

---
## \#6 Posted by: goldrabe Posted at: 2018-08-28T23:40:54.862Z Reads: 179

```
I really want to see that Flipsky burning! 👹👹👹👹
That shit spread around quick here without a lot of proper testing.
```

---
## \#7 Posted by: longhairedboy Posted at: 2018-08-28T23:44:34.242Z Reads: 176

```
is this dual ESC even out yet? I don't see it on thier site. The single is. 

Also they have an eswitch coming. I've been trying to talk them into making one with a lot of fets and a midi fuse holder, the bolt in style. They just keep telling me about their 8 fet switch that looks like it could turn on the starter for my truck.
```

---
## \#8 Posted by: goldrabe Posted at: 2018-08-28T23:46:59.446Z Reads: 172

```
Yeah it's on their website now. The dual 6.6 was delayed, but the dual 4.20 there are already group buys for it.
```

---
## \#9 Posted by: longhairedboy Posted at: 2018-08-28T23:52:07.344Z Reads: 166

```
i should try and burn up that single too. 

i need a BT logger for this rig.
```

---
## \#10 Posted by: moon Posted at: 2018-08-28T23:53:56.109Z Reads: 169

```
This is your best build yet
```

---
## \#11 Posted by: danielz Posted at: 2018-08-29T00:08:19.507Z Reads: 162

```
I use heavy duty Velcro on lots of my projects, its an underrated tool and seriously tough. It held my enclosure to my mountain board with ease and as a bonus isolates vibration.
```

---
## \#12 Posted by: longhairedboy Posted at: 2018-08-29T18:00:06.511Z Reads: 152

```
It should be dry enough when i get home to run this board down the road. Setup was really easy using VESC tool with this ESC. I was expecting it to complain about firmware or some stupid shit, but it just worked. We were trying to do burnouts on the dusty garage floor yesterday while it was raining.
```

---
## \#13 Posted by: brenternet Posted at: 2018-08-29T18:22:40.920Z Reads: 156

```
Bookmarked, I will be back hourly until either that flipsky vesc is immolated or you are.
```

---
## \#14 Posted by: longhairedboy Posted at: 2018-08-31T01:20:34.254Z Reads: 148

```
My report on the FlipSky is as follows:

THE GOOD:

* its running the latest firmware, 3.40, which is excellent. 
* Works with VESC-Tool right out of the box with no issues.
* can be flashed back to 2.18 easily to work with BLDC-Tool if you prefer the older stuff
* integrated can bus connection is really nice and saves time
* works well in both FOC and BLDC mode when it does work
* supports multiple control schemes and has all the needed ports to take advantage of them 
* small, almost perfect form factor. I really, really like the size. 

THE BAD:

* there is a hardware issue that leads to complete power loss during hard acceleration and hard braking. There is little that can be done in the settings to mitigate this.
```

---
## \#15 Posted by: longhairedboy Posted at: 2018-08-31T01:24:34.100Z Reads: 148

```
on the other hand.. we have the Unity which is what i'm testing now. Its kind of fucking amazing. Everything is.. well.. dreamy and perfect. I don't know how else to describe it. 

For example, i ran motor detection on a shorted fucked up motor:
https://www.instagram.com/p/BnH5fGgAcIE/?taken-by=longhairedboy

The Unity is perfectly fine, in fact i ran it around the block a half dozen times, hitting the accelerator hard and braking hard too. Then for more fun, i unplugged one phase lead and rode it some more. Sounded like shit and went all quirky but nothing bad happened. 

Next we're going to light it on fire and beat it with hammers.
```

---
## \#16 Posted by: Winfly Posted at: 2018-08-31T01:26:42.281Z Reads: 136

```
Which flipsky vesc r you talking about? 6.6 or the 4.20
```

---
## \#17 Posted by: longhairedboy Posted at: 2018-08-31T01:27:29.229Z Reads: 137

```
Sorry, i should have been specific. Its the one i mentioned earlier in the thread, the FSESC4.20 Dual 100A
```

---
## \#18 Posted by: Wraith Posted at: 2018-08-31T01:28:20.046Z Reads: 138

```
Hoping these won’t be happening with the 6.6 flipskys. I read that @mmaner was also testing these fsescs but not sure which of them he’s testing on
```

---
## \#19 Posted by: longhairedboy Posted at: 2018-08-31T01:28:57.104Z Reads: 141

```
This one. He's noticing the same problems. 

We also tested the 6.6 and found it to have a shitty power switch.
```

---
## \#20 Posted by: Jc06505n Posted at: 2018-08-31T01:28:58.921Z Reads: 141

```
[quote="longhairedboy, post:15, topic:66421"]
Next we’re going to light it on fire and beat it with hammers.
[/quote]

Ah the old lightitonfireandbeatitwithhammers Test
```

---
## \#21 Posted by: Wraith Posted at: 2018-08-31T01:30:36.545Z Reads: 132

```
Does it run into the sudden shut offs as well on the 6.6? I plan on using the DieBieMS with them and power switch connected to the BMS shouldn’t be a an issue I hope
```

---
## \#22 Posted by: Wraith Posted at: 2018-08-31T01:31:43.969Z Reads: 131

```
Id like to see a video of this :rofl:
```

---
## \#23 Posted by: longhairedboy Posted at: 2018-08-31T01:32:00.304Z Reads: 129

```
no not at all. The only issues were with the power switches themselves. Jakes' running the 6.6s right now at 12S and they're fine. We lack a 13S pack at the moment or they would be on that.
```

---
## \#24 Posted by: Wraith Posted at: 2018-08-31T01:33:44.915Z Reads: 131

```
Awesome. Thanks @longhairedboy! Good to know they’ve been thoroughly torture tested. Gives me some peace of mind.

Have you done said, lightonfirebeatwithhammers test? Id be afraid to try that with my dual 6.6s lol
```

---
## \#25 Posted by: longhairedboy Posted at: 2018-08-31T13:42:22.408Z Reads: 114

```
I sent FlipSky a full report on the FSESC4.20 100Amp and after telling them everything they got right i told them about the cutouts. 

I let them know that i'm pretty sure the issue is the hardware and even when using much lower settings than we do on focboxes and other VESCs we were still getting cutouts. they immediately blamed my battery pack and said it was probably too weak. I LOLed so hard and sent them a pick of the test rig AGAIN. 

weak batteries my ass.. These Tattus ain't whistlin' Dixie, motherfuckers. I don't have anything at all between them and the ESC either because the whole point is to know what the ESC is doing, not the eswitch or BMS or whatever.
```

---
## \#26 Posted by: Skunk Posted at: 2018-08-31T13:51:06.251Z Reads: 108

```
[quote="longhairedboy, post:15, topic:66421"]
Unity which is what i’m testing now. Its kind of fucking amazing.
[/quote]

So unity > focboxes ?
```

---
## \#27 Posted by: brenternet Posted at: 2018-08-31T13:54:21.485Z Reads: 110

```
Keep in mind that while you're semi sound of mind and reasonably smart (I'm working hard here) they do deal with a whole whack of really stupid people on a daily basis, not helped further by the Xenophobia, which is similar to how we feel about them.

They probably have canned responses for people and 80% of the time the end user is actually trying to run these things on 102 watch batteries in series.
```

---
## \#28 Posted by: Jc06505n Posted at: 2018-08-31T14:05:29.404Z Reads: 101

```
[quote="brenternet, post:27, topic:66421"]
which is similar to how we feel about them.
[/quote]

Some******
```

---
## \#29 Posted by: longhairedboy Posted at: 2018-08-31T14:18:50.365Z Reads: 104

```
[quote="brenternet, post:27, topic:66421"]
you’re semi sound of mind and reasonably smart
[/quote]

I'm mentally unstable, clinically depressed with periodic manic mood swings, and a tortured artistic genius. 

but i'll accept your assessment.
```

---
## \#30 Posted by: brenternet Posted at: 2018-08-31T14:36:37.200Z Reads: 101

```
Where are we on things catching on fire though?
```

---
## \#31 Posted by: longhairedboy Posted at: 2018-08-31T14:47:47.361Z Reads: 99

```
I ran out of fire, used the my last shred of plasma burning my for arms so that i would feel more alive. 

 I have a Prime account though, so should have some more here Sunday.
```

---
## \#32 Posted by: brenternet Posted at: 2018-08-31T15:49:29.169Z Reads: 97

```
I'm out, this got too real
```

---
## \#33 Posted by: brenternet Posted at: 2018-09-03T20:17:21.725Z Reads: 79

```
Damon what's your final verdict on this dual fesc please? The form factor is really great and would solve a logistical problem for me in a tight enclosure. For an everyday rider who doesn't throttle around like a nutcase would you call this a good buy or is the cut out problem simply a no go in your opinion?
```

---
## \#34 Posted by: pat.speed Posted at: 2018-09-03T21:18:05.486Z Reads: 75

```
I saw a thread a while ago about a maytech that would cut out just like this when set higher than 30a batt. Maybe you have it higher? Try lowering it and see what happens
```

---
## \#35 Posted by: longhairedboy Posted at: 2018-09-03T23:15:39.370Z Reads: 73

```
In my opinion they can't be trusted. 

Not yet, anyway. They'll figure out the problem I'm sure. Eventually.
```

---
## \#36 Posted by: brenternet Posted at: 2018-09-04T05:29:42.143Z Reads: 58

```
Thank you, will exercise some patience
```

---
