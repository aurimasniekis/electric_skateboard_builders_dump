# How to recharge an 8s with one plug?

### Replies: 25 Views: 587

## \#1 Posted by: JamesNothing Posted at: 2018-05-23T21:54:21.316Z Reads: 99

```
soooo... I have 2 4s lipos wired in series that I'm planning to wire to a bms.
I already have the bms (bought a complete setup 190kv, battery, vesc and all that came with a bms).
I don't know what bms it is but I'll figure out the wiring, there's plenty of topics about that.
I found a battery charger on ebay: it's 33,6V for li-po' and li-ion: is this the one I'm looking for? 
I don't want to burn my house down :smiley:
```

---
## \#2 Posted by: mynamesmatt Posted at: 2018-05-23T22:56:19.789Z Reads: 95

```
Yep that's the right charger, Just make sure you've wired the charge and discharge correctly. Then you won't burn your house down. 🤙
```

---
## \#3 Posted by: JamesNothing Posted at: 2018-05-23T23:19:04.758Z Reads: 91

```
Thanks man! luckily the charger has polarity written on it (+in -out). now I'll just read a metric fuckton of threads to be sure to wire the cells correctly to the bms.

Boy, lithium is scary :confounded:
```

---
## \#4 Posted by: mynamesmatt Posted at: 2018-05-28T01:05:23.446Z Reads: 69

```
At first it really is, and don't worry, i'm pretty sure everyone here started with nothing too, just keep reading up my friend!!
```

---
## \#5 Posted by: JamesNothing Posted at: 2018-05-28T08:41:25.608Z Reads: 64

```
I know, right? I've read everything on this forum concerning battery management systems and still fear to fuck up big time :smiley:
When the charger will arrive I'll man up and do the thing triple checking everything so I don't blow up my flat. 
usually I'm ok with mechanics and light electronic jobs, but I've never done anything concerning potential lithium bombs. I'll be prepared for worst scenario while praying that everything goes flawlessly!
```

---
## \#6 Posted by: Cobber Posted at: 2018-05-28T08:57:05.703Z Reads: 51

```
https://www.icharger.co.nz/icharger-308-duo

this is what I use

[quote="JamesNothing, post:5, topic:56531"]
...I’ve never done anything concerning potential lithium bombs...
[/quote]

keep that attitude dude, always triple check every thing...
```

---
## \#7 Posted by: b264 Posted at: 2018-05-28T09:02:57.278Z Reads: 46

```
$275 is about $225 too much for an 8S charger.  That's a balance charger for use with no BMS...
```

---
## \#8 Posted by: JamesNothing Posted at: 2018-05-28T11:08:57.619Z Reads: 44

```
wow that's expensive!


btw I discovered that my bms is one from hobbyking and has an output of 10A max, so I'll have to bypass it in discharge.
is this potentially dangerous? I have vesc cutoff setup to 3.6V so I'm not likely to over discharge but I don't want to damage my batteries
```

---
## \#9 Posted by: b264 Posted at: 2018-05-28T15:55:08.391Z Reads: 33

```
It should be okay if everything is done correctly.
```

---
## \#10 Posted by: JamesNothing Posted at: 2018-05-28T17:31:57.393Z Reads: 31

```
I plan to have two discrete circuits: one with antispark led switch going from the battery to the vesc, with an inline battery meter that switches on with the board.
The second one is the charge circuit: battery and balance leads to the bms.
It's not clear to me if I've to have a switch on the second circuit or  if it's useless to have it.
Am I totally wrong here?
```

---
## \#11 Posted by: b264 Posted at: 2018-05-29T00:02:32.400Z Reads: 27

```
You're correct.  Just hook up the BMS and charger jack with all 22AWG wire

Then directly to the battery, around the BMS, using 10AWG connect either a loop_key OR an antispark switch and the ESC(s)
```

---
## \#12 Posted by: JamesNothing Posted at: 2018-05-29T00:13:59.591Z Reads: 24

```
thank you so much! 

So a switch for the charging circuit is not needed? I wonder if the bms could slowly bleed the battery?
This is the easiest part of the job. 

Now I'll have to get a female dc jack, 22awg wires and a 2 4s to 1 8s adapter, so I can leave the batteries as they are without cutting and resoldering  the balance harnesses.
```

---
## \#13 Posted by: b264 Posted at: 2018-05-29T00:19:11.679Z Reads: 25

```
The BMS will switch the charge jack off automatically.  The charger will switch the charge off automatically.  This is redundant safety so if either one fails hopefully fire is averted.

Make sure the charge jack negative wire goes through the BMS connected to C- (or P- if there is no C-)
```

---
## \#14 Posted by: JamesNothing Posted at: 2018-06-14T16:16:52.313Z Reads: 12

```
so.. I finally received all the parts I needed and the charger for my setup.

I searched the scheme for my bms and I connected the charging jack to p- and to the positive lead for my battery and the negative lead from the battery to b-.
I've now to wire up the balance wires to the adapter that was included with the bms, but the batteries have 10 wires coming out and the adapter only has 9.

to my understanding I have to start counting cells from the negative side of the battery (the one that has the black wire going to the bms's b-) and wire sequentially starting to the black balance wire to b-, b1,2 and so on, and on b4 I've to join the red balance wire from the first battery with the black one from the second battery.
just not to screw up anything I want to be extra sure of what I'm doing here, cause I've not found a suitable example of this searching online :slight_smile: 

![IMG_7610|375x500](upload://gHbmZYBwcQ6xm9M9iufez6hg4sS.JPG)


I'll give all my appreciation to whoever is going to tell me if I'm going to start a big fire or not!
```

---
## \#15 Posted by: b264 Posted at: 2018-06-14T16:21:17.263Z Reads: 9

```
What does it say under the small black wire in the top of the photo?
```

---
## \#16 Posted by: JamesNothing Posted at: 2018-06-14T16:23:07.601Z Reads: 8

```
that's a p-. the board has 2 p- but on the scheme I saw that one was to hook up the charging port
![s-l1600|615x500](upload://dm5eWzCjuOtHAJDnDOQ1tlt2HO9.jpg)
```

---
## \#17 Posted by: b264 Posted at: 2018-06-14T16:30:14.228Z Reads: 9

```
Before you plug the white connector into the BMS you want to check with a multimeter that --

From the big B- wire to

small B- is 0V
small B1 is 4V
small B2 is 8V
small B3 is 12V
...

Of course it may not be exactly 4V, it could be 2.8V to 4.2V but it should go up progressively in that manner.  If that's not the case, don't plug it in yet.

Always only work on one wire at a time to avoid short circuits and fires.  Insulate each connection before starting another one.
```

---
## \#18 Posted by: JamesNothing Posted at: 2018-06-14T16:35:37.996Z Reads: 10

```
yep, that's the plan :) but I've yet to figure out what to do with the 10 cables going to be 9 thing :)
going this way I should encounter one wire from the battery that gives me the same voltage of the one before it.
I don't understand if I have to cut and insulate this wire or if I have to join it with the previous one that should be b4
```

---
## \#19 Posted by: b264 Posted at: 2018-06-14T16:38:11.556Z Reads: 9

```
What battery?  Do you have a photo without the BMS covering the labels?
```

---
## \#20 Posted by: JamesNothing Posted at: 2018-06-14T16:43:31.263Z Reads: 9

```
every battery has 5 wires for balancing, so battery 1(the negative side) goes from b- to b4 and the other one follows from b5 to b8, but having 5 balancing wires each one wire is going to be left out or connected to another.

batteries are multistar 4s 5200 (Bad I know, but these are not definitive)
```

---
## \#21 Posted by: b264 Posted at: 2018-06-14T16:48:33.256Z Reads: 8

```
[quote="JamesNothing, post:20, topic:56531"]
every battery has 5 wires for balancing
[/quote]

This is certainly not true.  I have a 12V lead-acid battery and a AA battery and an 18450 cell and some 5S lipos here and none of those have 5 wires for balancing.  Details matter a lot.  In fact, it's all about the details.  Whether it works or not will be entirely dependent upon details.  Don't overlook things or assume anything.

If they are two 4S lipo batteries, it's likely each one has 7 wires coming out -- 2 large and 5 small.  You may not need to use all of them because some are redundant.  When you connect the cells in series you also make one of the balance wires redundant.  See [another other diagram](https://www.electric-skateboard.builders/t/beautiful-diagrams-no-words-just-pics/3179/117?u=b264) for an example.  (The loop key is wrong in that diagram, but the balance wires are correct --- for those batteries and that BMS, not for yours)

Checking with the multimeter will tell you which one is redundant
```

---
## \#22 Posted by: JamesNothing Posted at: 2018-06-14T17:01:44.731Z Reads: 8

```
I think I'm not explaining things the right way :) 
My two batteries are in series, so let's  treat them as one battery that is 8s1p, has a big black wire, a big red one and 10 little ones connected to the balance plugs.
With a multimeter, starting from the negative side of the battery I have a voltage of 0, 4, 8, 12, 16V on the first 5 little wires.
These little ones I have to wire to the balance cables going to the bms's port, going from b- to b4 (the balance port of the bms is labeled from b- to b8).

On the positive side of the battery (the pack with the big red wire that is my main positive wire) has also 5 little wires: on the multimeter they are 16, 20, 24, 28, 33V.
So now I know that I have two of the little ones that read 16V I know one of them is redundant: my question is which one is the redundant one? what have I to do with it? should I connect the two wires that read 16V on the bms or what else?
```

---
## \#23 Posted by: b264 Posted at: 2018-06-14T17:07:14.897Z Reads: 8

```
You can leave either one unhooked that reads the same voltage -- they are connected together where the big black and red wires meet between the 4S packs.  Essentially, they are the same connection.  One is the top end of the bottom battery and the other is the bottom end of the top battery.
```

---
## \#24 Posted by: JamesNothing Posted at: 2018-06-14T17:16:15.521Z Reads: 7

```
that's the thing I didn't understand! thank you! you were super helpful :smiley:
```

---
## \#25 Posted by: JamesNothing Posted at: 2018-06-14T20:13:45.063Z Reads: 5

```
mostly thanks to @b264 I succeeded to build a bmsed 8s limo without perishing into the flames.
it worked! I guess the list of ppl to thank in my upcoming build thread grows by the day :slight_smile:


edit: also, thanks to @b264 I earned the "firs mention badge" :smiley:
```

---
