# 16s lipo and FVESC 6.6

### Replies: 34 Views: 607

## \#1 Posted by: youseekcota Posted at: 2019-04-21T23:53:11.434Z Reads: 184

```
I'm putting together a 16s graphine lipo battery pack, will be splitting current between four 6.6 FVESC's. Will the FVESC's handle 60v?
```

---
## \#2 Posted by: mynamesmatt Posted at: 2019-04-22T00:34:18.607Z Reads: 184

```
no
10characters
```

---
## \#3 Posted by: mynamesmatt Posted at: 2019-04-22T01:26:23.765Z Reads: 179

```
![Screenshot_20190422-112549_Calculator|243x500](upload://2vIdZsY5a1QgbQPWTg9WdFPiR74.jpeg)

it will barely be able to handle 12s bud. please read
```

---
## \#4 Posted by: Sn4pz Posted at: 2019-04-22T01:29:15.385Z Reads: 174

```
16s is far past esk8s current commonplace technology. I don't even know if we have anything for that.... The ARC200 or whatever might be able to do it. 

Another option,although not out now, is the MotherFOCer by @shaman.
```

---
## \#5 Posted by: AlanZhou Posted at: 2019-04-22T02:24:03.590Z Reads: 161

```
[quote="Sn4pz, post:4, topic:91362"]
The ARC200 or whatever might be able to do it.
[/quote]

I hear this way to much, it does not I only does up to 12s
```

---
## \#6 Posted by: Sn4pz Posted at: 2019-04-22T02:25:00.594Z Reads: 159

```
....wut? :eyes:

E: ah ok the edit makes a little more sense. Nevermind then OP, no arc controller.
```

---
## \#7 Posted by: Dirt_Bag Posted at: 2019-04-22T05:45:26.770Z Reads: 136

```
A vesc 6 is mostly reliable at 12s. 13s is the absolute max. Running thst close to the vescs limit is going to shorten its life i imagine. You might want a cap on the last inch or so of battery wires if you run 13s.
```

---
## \#8 Posted by: sk8l8r Posted at: 2019-04-22T06:34:53.409Z Reads: 125

```
[quote="Dirt_Bag, post:7, topic:91362"]
13s is the absolute max
[/quote]

would 14s (58.8v) not be the absolute max? 

I know @Deckoz said 14s should be possible and after using my 13s I totally agree, in theory with good cooling it should be fine, if I had the space in my 13s I would not been able to stop myself trying it at least for a quick test :)
```

---
## \#9 Posted by: Surfer Posted at: 2019-04-22T07:22:31.823Z Reads: 120

```
It should be fine, just don't brake!!
Anyway I will not try with mine  ;)
```

---
## \#10 Posted by: Arzamenable Posted at: 2019-04-22T08:34:56.677Z Reads: 116

```
What kind of a quest are you on? 

What graphenes are you using? 

The answer is still, “no”. 

If you wanna go fast, just know some of the fastest boards here are 8s but use in runners and high amp escs.
```

---
## \#11 Posted by: Winfly Posted at: 2019-04-22T08:49:07.014Z Reads: 114

```
When I brake on my 13s fully charged it spikes up to 58.x volts 😬. So yeah 14s with no brake is possible.
```

---
## \#12 Posted by: Andy87 Posted at: 2019-04-22T09:05:30.459Z Reads: 110

```
![image|678x499](upload://15GScvMvMZynnx1BkGlptixTaYS.jpeg)
```

---
## \#13 Posted by: Vanarian Posted at: 2019-04-22T09:11:32.677Z Reads: 105

```
14S with a brake chopper is possible, you need a proper load to dump the extra power that's all.

16s on a regular vesc is a no go sorry ! Btw I had two VESC able to take 16s but these are sold so yea ,no.
```

---
## \#14 Posted by: chuttney1 Posted at: 2019-04-22T09:12:31.275Z Reads: 108

```
Maximum voltage is based on the driver chip which is 60V. A 16S pack frys everything unless it was made to handle 16S.
```

---
## \#15 Posted by: sk8l8r Posted at: 2019-04-22T10:01:36.383Z Reads: 104

```
reminded me of a recent post, if we could find a 13s version and used it with a 14s battery (totally assuming here lol) it would apparently release "through special braking resistor, so the braking voltage will be limited" :slight_smile: 

https://www.electric-skateboard.builders/t/rheostatic-brake/90737


Maytech MTBR1812 Rheostatic Brake (12s) 
"When regenerative braking voltage exceeding the maximum charging voltage of the battery, BMS switches off, regenerative braking energy cannot be absorbed by the battery, then the controller of the regenerative braking voltage will continue to rise. After the regenerative braking voltage reached 57V, the electronic switch inside the Rheostatic Brake will start, the energy will be released through special braking resistor, so the braking voltage will be limited. The controller will be protected."

https://www.youtube.com/watch?v=RA4F01N1ZHY


EDIT: @Vanarian is this what you mean?
```

---
## \#16 Posted by: Vanarian Posted at: 2019-04-22T11:33:14.490Z Reads: 95

```
Yea it's the same thing! 

You need something fast enough to contain transient voltage (random spikes) and endurant enough to be used continuously for some time (needed for braking at full battery).

Edit : is the Maytech unit really triggering at 57v? Cause it is rated for 12S so I'd expect it to trigger at 50v for example. Tricky part with brake choppers is you need one tailored to your battery voltage or it will be useless.
```

---
## \#17 Posted by: sk8l8r Posted at: 2019-04-22T12:17:20.755Z Reads: 83

```
I wonder if someone like @Martinsp might be able to make us a variable voltage one :wink:
```

---
## \#20 Posted by: briman05 Posted at: 2019-04-22T13:29:44.503Z Reads: 70

```
You need to contact @shaman as I dont think he has really started developing a vesc for a 60v battery but he is the only one I know that is here that is working on it.  To answer your question in the OP no
```

---
## \#21 Posted by: AlanZhou Posted at: 2019-04-22T13:42:19.145Z Reads: 62

```
I love how at this point, esk8's are tapping into ebike territory.

somebody please create a 100v vesc
```

---
## \#22 Posted by: Vanarian Posted at: 2019-04-22T14:12:26.367Z Reads: 57

```
Go check VESC forum there are 75v versions available 👍🏽
```

---
## \#23 Posted by: Vanarian Posted at: 2019-04-22T14:16:23.298Z Reads: 60

```
Would be great but not cost effective and probably difficult : you'd need multiple  diodes of different trigger voltage and a circuit able to select between diodes too. Which means there will be unused extra components on the board too (if it is doable).

A dedicated one for each voltage means a simpler and more compact layout !
```

---
## \#24 Posted by: AlanZhou Posted at: 2019-04-22T14:42:23.439Z Reads: 53

```
[quote="Vanarian, post:22, topic:91362"]
75v versions available
[/quote]

not good enough...

the euc community already has 100v controllers from focbox
```

---
## \#25 Posted by: Dirt_Bag Posted at: 2019-04-22T15:38:00.706Z Reads: 49

```
Voltage spikes.
```

---
## \#26 Posted by: Sn4pz Posted at: 2019-04-22T16:13:40.090Z Reads: 44

```
source? Some random guy is lecturing for class today and.... :man_shrugging: 

I need something to distract me
```

---
## \#27 Posted by: AlanZhou Posted at: 2019-04-22T16:15:42.632Z Reads: 45

```
gotway ms super 100v, gotway monster 100v/

not standalone controllers but... it intrigues, im really considering EUC's as a option now.
```

---
## \#28 Posted by: Sn4pz Posted at: 2019-04-22T16:19:05.462Z Reads: 45

```
want my ninebot one c+?  its collecting dust in my closet....

no mechanical faults, just scrapes and protective tape residue ( Ill remove that b4 shipping... I want to test out a solvent I found anyways ) 

$200 + shipping? :thinking: ;P
```

---
## \#29 Posted by: Vanarian Posted at: 2019-04-22T16:27:02.261Z Reads: 44

```
These are VESC / FOCBOX based and VESC Tool compatible ? Got a link or more ? If it is available as spare part it is interesting. What max voltage?
```

---
## \#30 Posted by: AlanZhou Posted at: 2019-04-22T16:28:04.431Z Reads: 42

```
no they are not vesc, sorry if i made it sound like it was, my point is, someone please design a 100v vesc
```

---
## \#31 Posted by: AlanZhou Posted at: 2019-04-22T16:28:36.258Z Reads: 41

```
[quote="Sn4pz, post:28, topic:91362"]
$200 + shipping? :thinking: :stuck_out_tongue_winking_eye:
[/quote]

enticing might ride it in the rain, might be too slow for me though
```

---
## \#32 Posted by: Sn4pz Posted at: 2019-04-22T16:30:58.081Z Reads: 42

```
Just trying to get rid of it. Shmonie is 'in the red' and I would like to get this spud build done so I can ride SOMETHING

it was 65 degrees in Utica yesterday. nicest its been in.... a long time o.O
```

---
## \#33 Posted by: AlanZhou Posted at: 2019-04-22T16:31:38.184Z Reads: 41

```
be happy i had nothing to ride and im in spring break
```

---
## \#34 Posted by: Sn4pz Posted at: 2019-04-22T16:32:13.517Z Reads: 41

```
ive had nothing to ride since the end of the previous school year. I think I win the pissing contest x)

not to mention your hummie is probably going to be done before my big build is done... I want that powah :(
```

---
## \#35 Posted by: AlanZhou Posted at: 2019-04-22T17:22:38.820Z Reads: 34

```
[quote="Sn4pz, post:34, topic:91362"]
not to mention your hummie is probably going to be done before my big build is done… I want that powah :frowning:
[/quote]

hehe, :sweat_smile:
```

---
## \#36 Posted by: youseekcota Posted at: 2019-04-22T17:25:39.711Z Reads: 33

```
So glad I didn't go full idiot on this one. Think I'll use my 16s bms with a 12s or 8s2p lipo pack.
```

---
