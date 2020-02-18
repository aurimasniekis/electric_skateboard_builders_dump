# Wiring of the 6S BMS

### Replies: 39 Views: 1769

## \#1 Posted by: jimmaskell Posted at: 2018-02-20T20:02:50.946Z Reads: 114

```
I'm trying to wire my two 3s batteries to a 6s BMS. I made a wiring diagram, but I'm kinda scared to try it out, so I would like to hear you guys opinions about it first.

Here is a picture of the wiring diagram.
![image|690x388](upload://lVqwGgPYU18i8Ety4LNMuneaJ7p.jpg)

There are a couple a sketches trough above the diagram, but that has nothing to do with it.
```

---
## \#2 Posted by: DevinG Posted at: 2018-02-21T04:15:30.619Z Reads: 94

```
i was advised against this when i asked about this...
```

---
## \#3 Posted by: jimmaskell Posted at: 2018-02-21T06:40:49.808Z Reads: 86

```
Why is that?
```

---
## \#4 Posted by: DevinG Posted at: 2018-02-21T13:07:49.696Z Reads: 80

```
http://www.electric-skateboard.builders/t/looking-to-buy-bms-for-6s-setup-us-preferably/41708/14

check out what @Namasaki told me in my old thread maybe he can clarify
```

---
## \#5 Posted by: krloz Posted at: 2018-02-21T13:24:55.832Z Reads: 74

```
Namasaki makes some good points there but only when using 6s
 In any case @jimmaskell If you still want to use a bms on a 6s only for charging , your diagram looks good to me
```

---
## \#6 Posted by: krloz Posted at: 2018-02-21T13:26:16.234Z Reads: 72

```
[quote="DevinG, post:2, topic:46975"]
against
[/quote]

I wouldn't say against there.  I think he simply stated his opinion.   Adviced against makes it sound like its dangerous.  Or maybe it's just my English
```

---
## \#7 Posted by: DevinG Posted at: 2018-02-21T13:39:30.136Z Reads: 64

```
thats why i shared the thread... so you can see his words first hand,  i dont think he said that cuz of a danger issue idk. also i wasnt trying to imply anything of the sort. i still think his opinion inclines me against using a bms on a 6s build imo.
```

---
## \#8 Posted by: krloz Posted at: 2018-02-21T13:58:08.711Z Reads: 56

```
It makes perfect sense if you have a 6s hobby charger
```

---
## \#9 Posted by: jimmaskell Posted at: 2018-02-21T14:08:44.619Z Reads: 59

```
I understand, but It's just that, with the BMS, you don't have the hassle of taking of your enclosure and charging them separately with a hobby charger.
```

---
## \#10 Posted by: jimmaskell Posted at: 2018-02-21T14:23:39.719Z Reads: 59

```
Here is the link to the BMS and the batteries that I'm using.
https://nl.aliexpress.com/store/product/6S-12A-25-2V-lipo-lithium-Polymer-BMS-PCM-PCB-battery-protection-circuit-board-for-6/2344164_32708935019.html?spm=2114.12010612.0.0.50de25ceQa916o

https://hobbyking.com/nl_nl/zippy-compact-5000mah-3s-25c-lipo-pack.html
```

---
## \#11 Posted by: DevinG Posted at: 2018-02-21T14:24:35.804Z Reads: 55

```
thats what  i thought i understood... at least thats why i made that thread in the first place.
 i wanted on board charging for my board and battery checker and leds from a bms but  i went a different route on account of what nam told me. being the trust level he is i thought it would be best to hold off on a bms until i upgrade to an 8 or 10s build. im not trying to confuse anyone just trying to help
```

---
## \#12 Posted by: b264 Posted at: 2018-02-21T14:25:38.962Z Reads: 54

```
Shouldn't one of the black balance wires go to B- and the other black balance should be left unhooked along with B+

Also charge + typically goes to battery +, in fact all + all get tied together and you put the loop key from batt - to esc -

Please let us know what make and model BMS it is or provide photos
```

---
## \#13 Posted by: jimmaskell Posted at: 2018-02-21T14:38:55.186Z Reads: 52

```
The black balance wire of the lower Battery goes to the B-, I'm trying to make a system the way that I can unplug the batteries when needed, that's why I bought JST-XH 3S extension, of which I will use the female sides to connect to batteries and cut off the male sides so I can solder the wires to the plug which goes into the BMS. This can be seen in the diagram.

To be honest, I don't exactly know if the second black balance wire should be connected or disconnected, but on another persons wiring diagram for two 3s batteries to a 6s BMS I saw the second black balance wire connected.

I don't exactly know what you mean with the lines "Also charge + typically goes to battery +, in fact all + all get tied together and you put the loop key from batt - to esc -"

Here a link to the female balance connectors I bought:
https://hobbyking.com/nl_nl/jst-xh-3s-wire-extension-20cm-10pcs-bag.html
```

---
## \#14 Posted by: b264 Posted at: 2018-02-21T14:45:30.314Z Reads: 51

```
Please let us know what make and model BMS it is or provide photos
```

---
## \#15 Posted by: jimmaskell Posted at: 2018-02-21T15:01:45.282Z Reads: 49

```
I replied with two links to DevinG
```

---
## \#16 Posted by: e.board_solutions Posted at: 2018-02-21T16:14:56.063Z Reads: 47

```
So you want to charge your batteries trough the balance cables? I'm not sure but I think they are not thick enough to take 2A (?) charge current :)
```

---
## \#17 Posted by: b264 Posted at: 2018-02-21T16:23:58.983Z Reads: 46

```
They are thick enough for that.
```

---
## \#18 Posted by: e.board_solutions Posted at: 2018-02-21T16:25:09.826Z Reads: 42

```
Than his wiring is OK I guess?
```

---
## \#19 Posted by: b264 Posted at: 2018-02-21T16:27:38.955Z Reads: 41

```
I definitely did not say that

B3, B4, and B5 look wrong
```

---
## \#20 Posted by: jimmaskell Posted at: 2018-02-21T16:42:26.690Z Reads: 38

```
What would you suggest to improve the wiring diagram?
My diagram is inspired by this diagram that I found:
![image|690x339](upload://204l2Y7Qat8vmu4jZ0hM4g2FRNM.png)
```

---
## \#21 Posted by: b264 Posted at: 2018-02-21T18:19:58.812Z Reads: 35

```
Yeah, for that BMS this diagram looks correct
```

---
## \#22 Posted by: jimmaskell Posted at: 2018-02-21T18:53:27.858Z Reads: 34

```
And why wouldn't that work on mine? Because it is the same right?
```

---
## \#23 Posted by: b264 Posted at: 2018-02-21T18:56:18.813Z Reads: 33

```
That is your BMS
```

---
## \#24 Posted by: jimmaskell Posted at: 2018-02-21T19:29:18.175Z Reads: 33

```
Okay, so my diagram should work?
```

---
## \#25 Posted by: b264 Posted at: 2018-02-21T19:38:16.079Z Reads: 32

```
Your diagram needs a loop key in the fat black cable
```

---
## \#26 Posted by: jimmaskell Posted at: 2018-02-21T19:43:18.720Z Reads: 32

```
Okay thank you. What is its function?
```

---
## \#27 Posted by: b264 Posted at: 2018-02-21T19:43:49.521Z Reads: 31

```
It turns the skateboard on and off.  Make sure it's an antispark XT90 not just an XT90

warning: if you don't plug it **all the way** in **every** time you will burn up the key
```

---
## \#28 Posted by: jimmaskell Posted at: 2018-02-21T19:45:12.072Z Reads: 29

```
Okay but I have an on/off switch so I guess that means I don't need the XT-90 connector right?
```

---
## \#29 Posted by: b264 Posted at: 2018-02-21T19:49:44.070Z Reads: 30

```
If you use an electronic anti-spark switch, you won't need the loopkey but you'll still need an XT60 or XT90 connector internally so the battery can be disconnected if needed.  Make sure it's the kind where you have to hold the button for {number} seconds before it turns off.  That's so if a pebble or stick hits the power button, you don't lose brakes.
```

---
## \#30 Posted by: jimmaskell Posted at: 2018-02-21T20:04:57.710Z Reads: 28

```
Okay thank you
```

---
## \#31 Posted by: jimmaskell Posted at: 2018-02-22T16:01:09.961Z Reads: 26

```
@b264 I was wondering, what batterypercentage is safer, if you charge with the BMS for the first time?
```

---
## \#32 Posted by: b264 Posted at: 2018-02-22T17:19:14.220Z Reads: 27

```
[quote="jimmaskell, post:31, topic:46975"]
I was wondering, what batterypercentage is safer, if you charge with the BMS for the first time?
[/quote]

Maximum of 4.2V per cell, as measured with a multimeter
```

---
## \#34 Posted by: EvanWhy Posted at: 2018-09-12T03:28:59.115Z Reads: 14

```
Hey I'm about to hook up my bms for charging purposes and want to make sure I do it right. I am using two 3s lipos in series. Also would you recommend soldering or just putting the wires into connectors and hot gluing. I also plan on using 10 gauge wire to attach directly to the p- b- and positive charging input. is this correct?

![20180911_123629|281x500](upload://vtGcVSTBaNeLzFj68vdWOr3qAFk.jpg)![20180911_123652|281x500](upload://jFnBzOka61Hswc3sTbH3weObZpq.jpg)
```

---
## \#35 Posted by: TowerCrisis Posted at: 2018-09-12T05:09:20.352Z Reads: 15

```
Okay, first of all lets run through the balance port cables.

Since it is a hobby lipo it probably has a (-) (cell1 pos) (cell2 pos) (cell3 pos) so four cables total. If it does NOT have 4 pins, disregard everything below and let me know.

The BMS has 6 pins total.

For claritys sake, when I refer to the "lower battery" I mean the battery that has it's positive terminal connected to the negative terminal of the "higher battery"

Your lower battery will use 3 of the 4 cables. The (cell1 pos) (cell2 pos) (cell3 pos) terminals will be used. Do NOT use the (-) balance cable on the lower BMS.

Your higher battery will use 3 of the four cables. Like the lower battery, the higher battery will use (cell1 pos) (cell2 pos) (cell3 pos). Again, do not use the (-) terminal on the balance port.

So here's the sequence for the BMS balance port cables

**BATTERY CABLES**   _______ **BMS PORT**
(low batt, cell1 pos)________1 (this pin may be labeled as B1)
(low batt, cell2 pos)________2
(low batt, cell3 pos)________3
(high batt, cell1 pos)_______4
(high batt, cell2 pos)_______5
(high batt, cell3 pos)_______6 (this pin may be labeled as B6)

You may have noticed that there is no (-) pin used in the port. This is because the ground pin is pulled directly from (B-) on the BMS.


Here's what you should do. Lay everything out on a floor. Verify the correct orientation of the plug for the BMS.

Clearly label your high batt and low batt.

Connect low batt + to high batt -. This should use the main battery terminals, not the balance port.

Once that is connected, connect the low batt - to B- on the BMS. Also connect P- to the charge port, and the other charge port pin to the main battery positive terminal. Again, this is using the main battery cables, NOT the balance cables.

After this is done begin working out the balance port. Make sure you have it in the correct orientation, if you connect it backwards to the battery and hook it up to the BMS then you'll release the magic smoke :wind_face:


Here are things you need to keep in mind.

NEVER disconnect low batt from high batt while the balance port is connected. ESPECIALLY when the VESC is still on and connected. This will release the magic smoke. :wind_face:

NEVER connect the balance port when either the P- or B- cables are disconnected. This will release the magic smoke. :wind_face:

Always cover live wires while working. If you have a cable or wire with an exposed plug temporarily tape it up with electrical tape. This includes the balance port plug that goes into the BMS, it has live contacts on one face face. If it touches anything grounded or any other cells voltage it will release the magic smoke :wind_face: and possibly the magic light. :cloud_with_lightning:


BESIDES THAT everything looks good! I just wanted to clarify some pins and let you know the hazards associated with these kinds of batteries and BMS's. Your diagram looks correct enough. It just doesn't look like it has the balance cable connections labeled.

I've personally used that exact model of BMS before and I can vouch for the information I've provided above.
```

---
## \#36 Posted by: EvanWhy Posted at: 2018-09-12T05:22:14.521Z Reads: 14

```
wow thanks a ton for that explanation! It helps a lot! I will update on how it turns out.
```

---
## \#37 Posted by: TowerCrisis Posted at: 2018-09-12T05:23:38.455Z Reads: 13

```
If you have any questions feel free to ask! The community takes care of everyone ;)
```

---
## \#38 Posted by: EvanWhy Posted at: 2018-09-13T03:13:13.179Z Reads: 10

```
Should it look like this?

![15368083595371638581189|281x500](upload://8YPuFzal5kn74PQffUbl1tpa63I.jpg)
```

---
## \#39 Posted by: EvanWhy Posted at: 2018-09-13T03:19:20.305Z Reads: 11

```
I was wondering if this configuration also works since all I need to do is cut off the black balance cable on my series balance connector


![15368085598931640164647|281x500](upload://30BuUJJHmWJN72zuj0neEi2mdkf.jpg)![15368086528901725818346|690x388](upload://t9dF9iTAcIXySoDZ1iyhsTYObsV.jpg)
```

---
## \#40 Posted by: TowerCrisis Posted at: 2018-09-13T04:28:07.780Z Reads: 11

```
Yep, that all works fine :)
```

---
