# Space cell 3 problem

### Replies: 19 Views: 871

## \#1 Posted by: Battosaii Posted at: 2017-07-18T01:18:46.961Z Reads: 98

```
I have a space cell 3 with a broken power button, i replaced the power button and it switches on and powers my raptor but when i go to charge it, it gets to about 70% ish and the power starts jumping to 100% and back down to 70% also the charger turns on and off when this happens. could my cells be damaged? i havnt taken the battery apart but i do want to fix it if its worth it.
```

---
## \#2 Posted by: Jinra Posted at: 2017-07-18T01:26:06.290Z Reads: 95

```
Could be a broken BMS, have you tried prodding with a multimeter to see what voltage it's at?
```

---
## \#3 Posted by: Battosaii Posted at: 2017-07-18T01:31:29.488Z Reads: 95

```
not yet i didnt want to rip into the heat shrink if i didnt have to
```

---
## \#4 Posted by: Jinra Posted at: 2017-07-18T01:32:42.576Z Reads: 92

```
You don't need to, just measure the voltage from the power header.
```

---
## \#5 Posted by: Battosaii Posted at: 2017-07-18T01:33:28.807Z Reads: 88

```
ohhhhh, im going to go search for my multimeter right now and test it.
```

---
## \#6 Posted by: Eboosted Posted at: 2017-07-18T01:46:28.877Z Reads: 81

```
It has to be definitely a broken nickel strip inside the pack
```

---
## \#7 Posted by: Battosaii Posted at: 2017-07-18T01:54:42.282Z Reads: 81

```
If a nickel strip was broken could it be repaired with solder?

also ive been going crazy trying to find my Multimeter im pretty sure i lent it to my buddy and he "forgot" to return it.... Ill call him tomorrow
```

---
## \#8 Posted by: Jinra Posted at: 2017-07-18T01:55:58.405Z Reads: 79

```
you could technically solder it, but you might damage the cell if you mess up or have a low power iron. Otherwise, spot welding it again is the way to go
```

---
## \#9 Posted by: sl33py Posted at: 2017-07-18T03:01:25.384Z Reads: 81

```
Agree with @Jinra here.  I'm helping a buddy here repair a Space Cell 3 now, and by the time you dig into the battery - fix it right w/ spot welder.
```

---
## \#10 Posted by: Battosaii Posted at: 2017-08-08T03:09:09.029Z Reads: 63

```
So I had time to dig into the battery today, I still havnt found my multimeter but I found all Nickel strips to be in tact all my balance wires also in tact, I'm inclined to believe it's the BMS that failed. Another weird thing is does that I probably would never catch with out having another good space cell is that the Bad space cell turns on the display while charging no matter the switch position  and the good space cell only turns on the display when it's powered on whether it's charging or not.

<img src="/uploads/db1493/original/3X/b/a/baa9f09abb018d8c263060b18aa710b7a0515de2.jpg" width="666" height="500"><img src="/uploads/db1493/original/3X/f/3/f3648248bd8f323880309cb8acd311e8104dd688.jpg" width="666" height="500"><img src="/uploads/db1493/original/3X/d/9/d998f8227507b7f56607df259980613039ed6ab2.jpg" width="666" height="500"><img src="/uploads/db1493/original/3X/5/a/5a12affd96c2b72697dc8abe6cf4ab0974deaf55.jpg" width="666" height="500"><img src="/uploads/db1493/original/3X/8/e/8e858f403848c48cc6b1be5cad508a374bbabfe4.jpg" width="666" height="500">
```

---
## \#11 Posted by: Battosaii Posted at: 2017-08-08T23:39:49.141Z Reads: 53

```
im looking for a BMS would any cheap 10s lithium BMS work? i was looking at this one http://www.ebay.com/itm/36V-37V-42V-10S-45A-Lithium-ion-Li-ion-Li-Po-LiPo-Polymer-Battery-BMS-PCB-System-/322445471781?hash=item4b133f7025:g:VJcAAOSwTuJYvS8E

ideally id like to not have to rewire a BMS it would be cool to get a BMS that i can just plug in my balance leads into, i dont mind soldering but if i dont have to soldier the battery pack i wont.
```

---
## \#12 Posted by: adrianenertion Posted at: 2017-08-09T00:36:09.197Z Reads: 54

```
Hi /u/Battosaii,

I've spoken with Charles, our lead engineer, and he recommends using this BMS to replace the one in your Space Cell:

http://www.batterysupports.com/36v-37v-42v-10s-60a-10x-36v-lithium-ion-lipolymer-battery-bms-p-267.html

Hope that helps, and sorry for the delay in getting you this information.

Kind regards,
```

---
## \#13 Posted by: Battosaii Posted at: 2017-08-09T00:44:20.325Z Reads: 51

```
[quote="adrianenertion, post:12, topic:27902"]
http://www.batterysupports.com/36v-37v-42v-10s-60a-10x-36v-lithium-ion-lipolymer-battery-bms-p-267.html
[/quote]

Sweet! im going to order it now, thanks for pointing me in the right direction.
```

---
## \#14 Posted by: adrianenertion Posted at: 2017-08-09T00:58:32.426Z Reads: 50

```
No problems at all; wish i'd had the information sooner for you!
```

---
## \#15 Posted by: Battosaii Posted at: 2017-10-04T00:41:42.449Z Reads: 43

```
hmm after all this time i get the BMS in the mail and i realize the bms has 10 balance wires and the space cell has 11 balance wires, is this the wrong bms? or can this be wired differently?

also i dont think this BMS has any switches? i understand how a diy battery works but i asked for a replacement part not something i have to modify..... i feel like i wasted my money.
```

---
## \#16 Posted by: Jinra Posted at: 2017-10-04T01:16:46.398Z Reads: 43

```
space cell has a B- as one of the balance leads, your new BMS uses the B- terminal on the BMS for this.
```

---
## \#17 Posted by: Beck0934 Posted at: 2018-01-28T13:13:59.255Z Reads: 36

```
i was having similar issues and if anyone else has, I found it was the plug for the charge cable it has two tabs with wires soldered on to them and one of the tabs was  almost ripped in half, it was hard to notice but it was and I solder it and fixed it right up.
```

---
## \#18 Posted by: Schulerbible Posted at: 2018-01-29T00:04:26.121Z Reads: 26

```
If you guys ever experience that the spacecell won't charge up to 100% anymore then you've got most likely the same issue. I was a bit shocked seeing how messy and unprofessional the spacecell was put together. Also, some of the BMS cables were really short which I extended where necessary.

![image|635x356](upload://FS5NLE5gSUbsJSYOLTS37z19LA.jpg)
```

---
## \#19 Posted by: dAeM0N1K3 Posted at: 2018-01-29T00:27:10.507Z Reads: 25

```
@Schulerbible I noticed the exact same issue with mine as well
```

---
