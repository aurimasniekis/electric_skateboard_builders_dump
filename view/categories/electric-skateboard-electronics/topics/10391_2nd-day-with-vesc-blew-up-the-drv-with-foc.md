# 2nd day with VESC, Blew up the DRV with FOC

### Replies: 21 Views: 2226

## \#1 Posted by: covert Posted at: 2016-09-30T00:04:15.410Z Reads: 246

```
Title says it. I blew up the DRV on my VESC. Yesterday I set it up on my board, been sitting on the shelf for months. It ran well in BLDC on my 12S setup. It was great to have breaks that worked as well. Last ESC was a 90A boat ESC and had close to no breaks.

I had a  6364 190kv on it and changed it out to a 6374 149kv today. I also decided to try FOC out. I followed a tutorial on youtube by the man himself on how to detect the FOC values. All went well and I took it for a few KM ride. All was well. Put it back on the bench and did a few unloaded motor spin ups. I noticed if I started softly it would run in reverse for a little before running forward. It just didn't seem right. I ran it a few more times to try to understand what was wrong and in my head I said "I should stop and check settings" No sooner had I thought this i pressed the trigger one last time and nothing.

Ordered a few DRV chips from mouser. It will be running again early next week.

I've been reading about FOC a lot more and I can't seem to find a reason for it blowing up. Best answer I can find is "They blow the DRV up when they have the wrong settings ..."
```

---
## \#2 Posted by: Jinra Posted at: 2016-09-30T02:33:55.932Z Reads: 232

```
Tons of theories on why it blows up, but no one has concrete evidence.
```

---
## \#3 Posted by: Namasaki Posted at: 2016-09-30T02:52:04.450Z Reads: 226

```
I have made up my mind, I an never ever gonna try FOC.
BLDC is just fine and its really not that loud either.
```

---
## \#4 Posted by: NNGG Posted at: 2016-09-30T02:57:38.608Z Reads: 214

```
My old ti83 could be salvaged for the drv chip :blush:
```

---
## \#5 Posted by: covert Posted at: 2016-09-30T03:00:14.404Z Reads: 210

```
Yeah BLDC seems fine. My inquisitive mind got the better of me again. If I can find a bit more info I might give it another shot but two replaced DRV will be my limit.. 

@NNGG what is a TI83 ? I only know it as a graphics calculator.
```

---
## \#6 Posted by: Jinra Posted at: 2016-09-30T03:09:04.602Z Reads: 205

```
I think that's what he means since Texas instruments is the creator of the drv :stuck_out_tongue:

Also if you try again, try reflashing the firmware before your switch over to FOC.
```

---
## \#7 Posted by: covert Posted at: 2016-09-30T03:15:32.505Z Reads: 200

```
@Jinra are you saying re-flash every time between switching from the two modes ?
```

---
## \#8 Posted by: Jinra Posted at: 2016-09-30T03:19:13.143Z Reads: 195

```
yea, sure way to reset all settings
```

---
## \#9 Posted by: VladPomogaev Posted at: 2016-09-30T03:36:51.084Z Reads: 189

```
Just out of curiosity, what are the symptoms of a dead DRV chip? Like lights, voltage, anything?
```

---
## \#10 Posted by: Jinra Posted at: 2016-09-30T03:49:00.688Z Reads: 186

```
drv fault in bldc tool
```

---
## \#11 Posted by: VladPomogaev Posted at: 2016-09-30T03:49:41.037Z Reads: 181

```
Ah makes sense haha
```

---
## \#12 Posted by: CRABOLSKY Posted at: 2016-09-30T04:04:55.822Z Reads: 177

```
I've run about 30km so far on FOC and it is working really well. The difference between this time and the first time I blew the drv chip is that I flashed new firmware and very carefully went through the setup process. The first time I also had the buggy version of BLDC tool running (the multiply bug). 

Although (arguably) marginal difference between the two modes I am still really happy with my choice. 

FOC is like running the same turbocharged 911, only with fresh spark plugs, new oil and repaired muffler😁
```

---
## \#13 Posted by: evoheyax Posted at: 2016-09-30T05:50:16.182Z Reads: 170

```
The reverse/stuttering on the bench is normal. In FOC, motors struggle at low speeds unless they are sensored using the sensor/foc hybrid mode. I have never had an issue with FOC yet and I'd ridden a over a thousand miles in FOC. It's not perfect, but mathematically, it's a better mode than BDLC.
```

---
## \#14 Posted by: covert Posted at: 2016-10-01T10:49:21.718Z Reads: 143

```
I loaned another VESC today. I'll run this one is BLDC mode only till I give it back just to make sure I'm not repairing two.

I just realized I blew up my VESC the same day I donated to Vedder. Hope it was not a coincidence :) Sure it was not.
```

---
## \#15 Posted by: covert Posted at: 2016-10-03T04:38:20.661Z Reads: 137

```
This morning my Mouser order arrived (wow there quick). Didn't need to use the loaned VESC. Instead I fitted the new DRV with my 852D+ reflow station.It took more heat than expected but I forgot it has the heatsink pad at the bottom. Make sure you pre-warm the board well before trying this.

Plugged it up on the bench and ran motor detection in BLDC mode and it worked ! Happy days. Weather out is not so good with 40km winds. Will give it a shot anyway :)

Only a $6USD lesson. I'm lucky.
```

---
## \#16 Posted by: kyo Posted at: 2016-10-03T04:54:17.492Z Reads: 137

```
@covert i'm ab to replace my drv chip too this weekend. Any tip for me beside the preheat the board. Ive been practising smd on my old RAM. Thanks in advance
```

---
## \#17 Posted by: covert Posted at: 2016-10-05T01:53:41.303Z Reads: 122

```
@kyo plenty of youtube video's on reflowing that explain it better than me.

Heat control is king. Don't rush it. Most of all don't over cook the board. Use a temperature gun if you have it. 

I removed the main power wires to make it easy to work on. I should of placed it in a vice to make it easier to work with.

Remember when the solder is upto reflow temperate all the parts around it are also at reflow temperature and if you knock anything else it will move.

Once the DVR chip was reflow-ing I moved it a little left and right to get the soldier flow to the legs better. My first attempt of just placing it showed what looked like bad soldier joints with under my Andonstar USB microscope. Good flux would help, I couldn't find mine :( 

Take your time with it. Don't rush it.

Good luck
```

---
## \#18 Posted by: psychotiller Posted at: 2016-10-05T03:35:43.780Z Reads: 117

```
Your motor spinning backwards on the bench is normal if your are running sensorless. you just need to push off to get them moving in the right direction. 

Sensored foc is another story! It is crazy quiet  and has huge amounts of torque. Taking off fro a standstill, no cogging/searching. It just goes.
```

---
## \#19 Posted by: kyo Posted at: 2016-10-06T09:10:22.007Z Reads: 99

```
Thanks appriciate it. I see  contact point on the bottom of the chip, do we need to solder this as well?
```

---
## \#20 Posted by: covert Posted at: 2016-10-14T01:11:46.138Z Reads: 92

```
[quote="kyo, post:19, topic:10391"]
act point on the bottom of the chip, do we need to sol
[/quote]

Yes the contact point at the bottom of the chip needs to be soldiered. It should reflow with the rest of the pins. If not sure get it done by someone with experience, even ask them to teach you. VESC is a little expensive to be learning on. Anyone who does Xbox 360 BGA reballing will find this a breeze to fix.
```

---
## \#21 Posted by: Goombaacez84 Posted at: 2016-10-14T01:19:26.021Z Reads: 88

```
This same scenario is what happened to me over this past weekend except I was running a 6374 190kv rspec. I had the same twitchy symptoms but went for a ride anyways... it rode beautifully for 3 miles, then DRV went.

If you find out why FOC breaks VESCs other than "wrong settings", spread the word. I'd like to know since I'm kind of sad that once I get my VESC back from chaka I'll have to ride it out in BLDC :sob:
```

---
