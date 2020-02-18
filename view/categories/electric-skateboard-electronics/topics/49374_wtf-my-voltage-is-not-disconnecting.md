# WTF&hellip;My voltage is not disconnecting!

### Replies: 25 Views: 579

## \#1 Posted by: mmaner Posted at: 2018-03-18T00:06:01.285Z Reads: 161

```
Let me start by saying I've disassembled all the major components and can't figure this out. My voltage meter is going down to 23v when I hit the E-Switch, up to a normal 40v when I turn it on.

I've removed the switch and resoldered the leads.  I resoldered the led power leads on the switch. Neither made any difference. I'm thinking I may have a BMS issue. Can anyone confirm this for me?

![IMG_20180317_190525|375x500](upload://cUY79i8IIeJGBmG7XjuZZs9yy6J.jpg)
![IMG_20180317_190517|375x500](upload://g5An6vLjZeUVp0tyz9saTpdwlCz.jpg)
```

---
## \#2 Posted by: Martinsp Posted at: 2018-03-18T00:11:40.560Z Reads: 150

```
I had a similar problem when the BMS would power on and off which created something similar to PWM and made my voltage roughly double. in my case it was poor connection of the balance leads which caused the bms to turn on and off constantly i guess that it turned on checked if the problem is present then shut down and back to start
```

---
## \#3 Posted by: mmaner Posted at: 2018-03-18T00:13:42.163Z Reads: 148

```
I don't think it's a balance leads issue, I didn't pull them and resoldered but I checked the voltage on each block, it was normal.  Thanks for the info though. 

I'm guessing it's a BMS issue, but maybe the switch circuit. I'm gonna replace the switch tomorrow to rule that out.
```

---
## \#4 Posted by: abenny Posted at: 2018-03-18T00:16:58.186Z Reads: 140

```
might be obvious but the voltage meter isnt wired between the switch and batteries right? its after the switch?
```

---
## \#5 Posted by: mmaner Posted at: 2018-03-18T00:18:14.522Z Reads: 135

```
Yes, it's wires to the same leads the power the VESC's. In fact it's been running fine for months. 

Here's the original build thread. 

http://www.electric-skateboard.builders/t/dropped-glorrrrrrryyyyyyyy/
```

---
## \#6 Posted by: abenny Posted at: 2018-03-18T00:19:47.462Z Reads: 128

```
i mean in what order is it wired, 
i think it should be
batteries>switch>bms>voltmeter>vescs


but if it was working fine until now its probably like you suspect and a bms issue
```

---
## \#7 Posted by: Deckoz Posted at: 2018-03-18T00:22:22.081Z Reads: 121

```
Mosfets failed open...
```

---
## \#8 Posted by: mmaner Posted at: 2018-03-18T00:24:17.971Z Reads: 115

```
The E-Switch is in the BMS. Nit an anti-spark. Thanks for trying though 😀
```

---
## \#9 Posted by: mmaner Posted at: 2018-03-18T00:25:31.139Z Reads: 115

```
It's litterally just before the VESC's. Another odd thing...the multimeter shows less than a bolt at the charge port when it's off.
```

---
## \#10 Posted by: Deckoz Posted at: 2018-03-18T00:27:04.556Z Reads: 115

```
Those BMS use mosfets to limit output turn on and off...

I would be surprised if you have a fetless bms
```

---
## \#11 Posted by: mmaner Posted at: 2018-03-18T00:30:40.194Z Reads: 115

```
I did not know that. I've never heard if a BMS E-Switch failing, I would have assumed it would be as common as anti-spark switch failures. 

If it's not the switch itself and the BMS still.operates correctly I'll prolly put an anti-spark loop key in and call it a day. I mostly use discharge only these days so is loop keys a lot anyways.
```

---
## \#12 Posted by: Deckoz Posted at: 2018-03-18T00:55:12.737Z Reads: 111

```
See the reason a bms eswitch likely doesn't fail as it has all these voltages and gates in series with one another. So it can take the lowvoltage of a 1cell or a group of 2 or 3 cells at a time and increase the voltage across the gate... Trying to step down high voltage to control a gate is hard..but when you have 12 cells and 12 different voltages to work with...

Where a typical antispark has 1...

Likely one of the fets in the BMS is failed open.. likely the one connected to your 6th cell based on the voltage your seeing...
```

---
## \#13 Posted by: fedestanco Posted at: 2018-03-18T01:08:12.278Z Reads: 102

```
I believe most BMS' have a bunch of high voltage mosfets in parallel, directly placed to limit the LOAD (12s). Why do you think each series has its own mosfet? EDIT: I understood what you meant now.

@mmaner if you want to get serious with the tests you could desolder the on-off button. Then you could observe the behaviour keeping  2 switch wires shorted, and then insulating each of them.
If in both cases the lcd doesnt turn off, the bms cannot be used for discharging anymore.
```

---
## \#14 Posted by: mmaner Posted at: 2018-03-18T01:12:03.110Z Reads: 95

```
Good info, thanks brother.
```

---
## \#15 Posted by: mmaner Posted at: 2018-03-18T01:13:11.688Z Reads: 91

```
I will give that a try, thanks for the info.
```

---
## \#16 Posted by: fedestanco Posted at: 2018-03-18T01:26:13.029Z Reads: 87

```
@Deckoz do you say that bmss take the low voltage of a couple series because you have seen this in an existing design? 
I am curious because cheap chinese mosfets draw quite some power for operating and having 10 of them being powered just from 1 series all the time could cause some balancing issues.

Also to the possible problem list there would be that if the balancing cable that powers the fets came off, the bms would loose power. So all of  safety function would depend upon that particular cable.
```

---
## \#17 Posted by: JohnnyMeduse Posted at: 2018-03-18T01:41:45.474Z Reads: 82

```
[quote="mmaner, post:1, topic:49374"]
Let me start by saying I’ve disassembled all the major components and can’t figure this out. My voltage meter is going down to 23v when I hit the E-Switch, up to a normal 40v when I turn it on.
[/quote]

I don't see an issue there.... but an opportunity to get a beginner mode. :crazy_face:
```

---
## \#18 Posted by: mmaner Posted at: 2018-03-18T01:52:23.836Z Reads: 75

```
Yeah, when standing on top of a lightning powered murder board, I want my shit right 😀
```

---
## \#19 Posted by: scepterr Posted at: 2018-03-18T01:59:33.114Z Reads: 77

```
[quote="mmaner, post:18, topic:49374"]
murder board
[/quote]
Hahaha 😂🤣😂🤣
```

---
## \#20 Posted by: JLabs Posted at: 2018-03-18T02:07:49.338Z Reads: 78

```
I didn’t read through everything here so forgive me if this has all ready been said. 

I have a few different BMS’s with an eSwitch and the voltage in the off position is around 24v but it isint try voltage from what I understand. It will power the voltage meter because it dosnt draw very many amps but my VESC is still off. Is that what is happening?
```

---
## \#21 Posted by: mmaner Posted at: 2018-03-18T02:53:34.811Z Reads: 70

```
Essentially, the only other thing is I can still make a BT connection. Just figures that one out.
```

---
## \#22 Posted by: JLabs Posted at: 2018-03-18T03:07:38.379Z Reads: 69

```
Is it one of the packs I sent you?
```

---
## \#23 Posted by: mmaner Posted at: 2018-03-18T03:09:40.337Z Reads: 70

```
No, it's a pack I had made specifically for a sound 39 and ended up using in the Evo and I supplied the BMS.  Its not an issue with construction, it's  either a bad BMS or bad switch  if I was  home id find out, but alas it cannot be so 😀.
```

---
## \#24 Posted by: LiquidSkater Posted at: 2019-04-30T18:57:45.561Z Reads: 34

```
Hi, I bought an anti spark switch on ebay, I had the non - latching button and put another button on the NC wire and it worked perfectly fine. So I set up the board and went for a ride and 800 meters in power started to cit out, then it came back and I continued to ride, but on my way home (2nd km) power completely cut off and something started to smell. When I rushed home and opened the  enclosure I saw that the mosfets had melted a hole in shrink wrap...
I don't know what should I do now. If I had done something wrong or if I should cool it somehow...![15566504592414279644416883785934|374x500](upload://x6wPjx44n3iAxT1ByffDgT305nu.jpeg) ![15566504847895978260481251717062|375x500](upload://pMbvUX0r742SH0qRQDrnY42ELCJ.jpeg) 
I had the wires soldered correctly but it just melted...

The button i got (model 6)
https://www.ebay.com/itm/Anti-Spark-Power-On-Off-Switch-for-VESC-or-ESC-electric-skateboard-longboard-LED/163610874953?_trkparms=aid%3D111001%26algo%3DREC.SEED%26ao%3D1%26asc%3D56949%26meid%3D607a686075f5439c9d2f2223b46b5922%26pid%3D100675%26rk%3D1%26rkt%3D15%26sd%3D163610874953%26itm%3D163610874953&_trksid=p2481888.c100675.m4236&_trkparms=pageci%3Ac2cc312f-6b78-11e9-9fab-74dbd180dd14%7Cparentrq%3A6f950d4f16a0aadc417ffeaaffeea806%7Ciid%3A1
```

---
## \#25 Posted by: linsus Posted at: 2019-04-30T19:16:00.834Z Reads: 28

```
Dsnt rly specify but if its the original schematic, you need a latching switch. Else youll pull current thru semi open FETs resulting in what probably happened to you. Replace the FETs get a latching button.
```

---
