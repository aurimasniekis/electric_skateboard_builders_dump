# BMS Not charging and cant figure out why (help needed)

### Replies: 41 Views: 666

## \#1 Posted by: AdamE3399 Posted at: 2018-12-20T10:33:01.450Z Reads: 61

```
So I recently finished building my third board (so I like to think I know what im doing at this point) and everything was going fine until my dad shoved the loop key into the charging port (there both xt 90 ports). Anyway it was lucky in that it only short for a mili second and seemed to have caused minimum damage as the board kept working so I resoldered a new xt 90 and plugged it in but it would not charge. So I checked the cells and one was at 1.5v, so Im assuming this cell took the current of the short circuit. I recharged the cell individually slowly to match that of the other cells and left it overnight to see if it would self discharge and in three days it only lost 0.01 volts so I think the internal resistance is still ok. So I assumed the BMS wouldn't charge as the cells weren't balanced properly and now that the cell matched the others I tried again but it still wouldn't charge. So I though maybe the short circuit broke the bms and luckily I had a spare of the same type so I replaced it and again It wouldn't charge. B- is the battery negative C- is charge port negative battery positive is positive charge port and balance wires are all correct so I have no idea what is wrong, any ideas?
@Winfly @dareno
```

---
## \#2 Posted by: b264 Posted at: 2018-12-20T10:37:08.515Z Reads: 56

```
@Andy87 has a little bit of experience with a more severe form of this
```

---
## \#3 Posted by: b264 Posted at: 2018-12-20T10:38:00.727Z Reads: 56

```
What failed when it was shorted?  Which wire melted?  It's not likely a human hand could have gotten it disconnected in a millisecond, so I'm confused.
```

---
## \#4 Posted by: AdamE3399 Posted at: 2018-12-20T10:38:55.259Z Reads: 51

```
Sorry I mean the xt90 melted and broke the connection almost instantly so I don't think any wires melted
```

---
## \#5 Posted by: AdamE3399 Posted at: 2018-12-20T10:39:50.863Z Reads: 54

```
Sorry not melted but the metal connection broke from the heat
```

---
## \#6 Posted by: b264 Posted at: 2018-12-20T10:41:45.924Z Reads: 53

```
Just a public service announcement for future readers: don't use an XT90 for a charge port.  But no matter what you use for a charge port, put a fuse on it.  A 5A automotive fuse if you have to.
```

---
## \#7 Posted by: AdamE3399 Posted at: 2018-12-20T10:42:33.353Z Reads: 53

```
Note taken
```

---
## \#8 Posted by: Andy87 Posted at: 2018-12-20T10:43:03.389Z Reads: 52

```
What every you plan for the future,
First thing you should do,
Change the damn charging port and loopkey.
You was very lucky with it. Very very lucky.
And believe me, it can always happen again that you plug the loopkey into the charging port.
As min switch the xt90 one to male the other to female. Better make an xt60 for the charge port.
```

---
## \#9 Posted by: AdamE3399 Posted at: 2018-12-20T10:43:52.107Z Reads: 50

```
Will do, but does anyone know what is happening with the bms?
```

---
## \#10 Posted by: b264 Posted at: 2018-12-20T10:45:02.862Z Reads: 49

```
[quote="AdamE3399, post:1, topic:78511"]
So I checked the cells and one was at 1.5v
[/quote]

This is very concerning.  Is this lithium-ion?  The cells will probably be damaged after dropping that low.

Are you certain all of the other P-packs are correct?  Have you verified (CAREFULLY) that the battery voltage is present on the pins of the charge jack -- i.e. there are no breaks between the BMS and charge port?  (Warning: do not short it out again by accident)
```

---
## \#11 Posted by: AdamE3399 Posted at: 2018-12-20T10:46:09.434Z Reads: 45

```
Yes I used the multimeter and all looks good
```

---
## \#12 Posted by: AdamE3399 Posted at: 2018-12-20T10:46:53.640Z Reads: 43

```
Though for some reason the c- is 1v lower than the b-, is that normal?
```

---
## \#13 Posted by: b264 Posted at: 2018-12-20T10:47:20.501Z Reads: 40

```
That is an indication of a BMS safety shutdown

You'd be reading the battery voltage via the voltage drop of the MOSFET body diode and not through the actual activated FET junction itself.  Meaning "it's turned off" intentionally because there is a problem
```

---
## \#14 Posted by: AdamE3399 Posted at: 2018-12-20T10:47:39.688Z Reads: 38

```
But I put a new bms in and still didn't work
```

---
## \#15 Posted by: AdamE3399 Posted at: 2018-12-20T10:49:03.635Z Reads: 37

```
ill recheck voltage
```

---
## \#16 Posted by: b264 Posted at: 2018-12-20T10:49:11.337Z Reads: 39

```
Yes but this one senses a problem and is shut down.  I would verifiy all the cell voltages again and make sure they are all connected to the BMS with no loose connection.  Without accidentally shorting anything.
```

---
## \#17 Posted by: b264 Posted at: 2018-12-20T10:50:33.260Z Reads: 37

```
Also check for an "off-by-one" problem where all the balance leads are in the wrong place
```

---
## \#18 Posted by: AdamE3399 Posted at: 2018-12-20T10:52:43.612Z Reads: 36

```
b- is 39.0 and c- is 38.6, charging wires are: 3.90 3.90 3.90 3.90 3.90 3.90 3.90 3.91 3.91 3.90
```

---
## \#19 Posted by: AdamE3399 Posted at: 2018-12-20T10:55:47.056Z Reads: 36

```
@b264 any ideas?
```

---
## \#20 Posted by: Winfly Posted at: 2018-12-20T10:58:47.601Z Reads: 37

```
are you checking voltage from the balance wire?
```

---
## \#21 Posted by: AdamE3399 Posted at: 2018-12-20T10:59:13.811Z Reads: 38

```
yes, what I called the charging wires are the balance wires
```

---
## \#22 Posted by: Winfly Posted at: 2018-12-20T11:03:05.713Z Reads: 37

```
what bms are you using and by soldering P I'm assuming you are using discharge protection.
```

---
## \#23 Posted by: AdamE3399 Posted at: 2018-12-20T11:04:24.942Z Reads: 38

```
im bypassing for charging only so I don't use p- and it is one of these: https://www.amazon.com.au/Li-ion-Battery-Protection-Ternary-Balancing/dp/B07GPQFSFM/ref=sr_1_1?ie=UTF8&qid=1545303840&sr=8-1&keywords=10s+bms
```

---
## \#24 Posted by: Winfly Posted at: 2018-12-20T11:06:08.848Z Reads: 38

```
on this diagram it says Charge+ so did you wire +ve or -ve of your charge port to that.
![image|500x500](upload://AdRfx9YhdKHy5jcZTQ0sgGgLMEs.jpeg)
```

---
## \#25 Posted by: AdamE3399 Posted at: 2018-12-20T11:07:47.723Z Reads: 35

```
I wired the negative because you always wire the negative to the c- or at least I thought you were supposed to
```

---
## \#26 Posted by: Winfly Posted at: 2018-12-20T11:10:59.496Z Reads: 35

```
yeah you are right. had to think about it for a bit. can you draw a diagram of your wiring?
```

---
## \#27 Posted by: AdamE3399 Posted at: 2018-12-20T11:11:30.895Z Reads: 32

```
ok give me a minute
```

---
## \#28 Posted by: AdamE3399 Posted at: 2018-12-20T11:32:27.209Z Reads: 35

```
@Winfly here you go:![Chart|690x388](upload://4wkVIhNiqpYsxYWz9s34Iip4Ks5.png)
```

---
## \#29 Posted by: Winfly Posted at: 2018-12-20T11:37:29.859Z Reads: 38

```
unless you soldered your xt90 wrong I dont see a problem in this diagram. voltage reading is measured by probing adjacent balance wire right? 

it could also be that you broke your charger as well. try another charger.
```

---
## \#30 Posted by: Noob-at-building Posted at: 2018-12-20T11:38:10.340Z Reads: 36

```
He replaced the charger so that's not the issue
```

---
## \#31 Posted by: Winfly Posted at: 2018-12-20T11:40:11.497Z Reads: 33

```
are you with him irl or did I miss that part that he said he replaced the charger?
```

---
## \#32 Posted by: Noob-at-building Posted at: 2018-12-20T11:40:41.141Z Reads: 33

```
With him, where friends
```

---
## \#33 Posted by: AdamE3399 Posted at: 2018-12-20T11:43:56.801Z Reads: 33

```
Sorry im back, I have a throbbing headache so Ima go to bed, but the charger is giving out 42 volts and everything is wired correctly so that's why I don't understand what's happening
```

---
## \#34 Posted by: Winfly Posted at: 2018-12-20T11:51:59.116Z Reads: 35

```
Honestly I have no clue atm. when you have time add the balance wire on your diagram.

just realized the +ve, -ve of those individual Bat on this diagram is flipped.

[quote="Winfly, post:24, topic:78511"]
![image|500x500](https://www.electric-skateboard.builders/uploads/db1493/optimized/3X/f/d/fddf50aec76529e7aab8579e64969cffa21cebd4_1_500x500.jpeg)

image.jpg1001x1001 226 KB
[/quote]
```

---
## \#35 Posted by: b264 Posted at: 2018-12-20T19:56:21.242Z Reads: 30

```
That diagram is 100% wrong and should never be used for anything.
```

---
## \#36 Posted by: Winfly Posted at: 2018-12-20T20:47:55.880Z Reads: 29

```
I pulled that from his link.
```

---
## \#37 Posted by: b264 Posted at: 2018-12-20T22:02:28.809Z Reads: 28

```
Amazon is giving you a wiring diagram that's all but guaranteed to cause a fire or failure if followed.
```

---
## \#38 Posted by: b264 Posted at: 2018-12-20T22:09:55.069Z Reads: 28

```
At this point I recommend you return both BMS to the seller and demand a full refund (or file a chargeback if they refuse) because their wiring diagram is not only wrong, but extremely dangerous.  Only after that I would work on fixing the battery with a BMS from a different seller, preferably not on Amazon.

I have reported this to Amazon as well.  This is the second time I've seen this image on the forum.

Effectively, they are scamming you in a roundabout way and endangering the safety of people.
```

---
## \#39 Posted by: AdamE3399 Posted at: 2018-12-20T23:23:40.150Z Reads: 25

```
I know that the diagram is wrong and I have wired many bms's before and know the correct way to wire them and I did not follow this diagram and it did work, but then after a small short circuit I replaced the bms with a new one and still nothing, so I don't know what's wrong?
```

---
## \#40 Posted by: AdamE3399 Posted at: 2018-12-20T23:26:12.014Z Reads: 26

```
What about this one: https://www.ebay.com.au/itm/10S-45A-37V-42V-Li-ion-Lithium-Battery-Cell-BMS-PCB-Protection-Balance-Board/302924070488?hash=item4687ae7e58:g:IC8AAOSwmoVaqOK0:rk:3:pf:1 seems to be higher quality and has a correct wiring diagram
```

---
## \#41 Posted by: b264 Posted at: 2018-12-31T22:44:52.918Z Reads: 15

```
@AdamE3399 @Winfly I reported the fire hazard wiring diagram to Amazon and it looks like they finally took it offline

https://www.electric-skateboard.builders/t/bms-not-charging-and-cant-figure-out-why-help-needed/78511/23?u=b264
```

---
