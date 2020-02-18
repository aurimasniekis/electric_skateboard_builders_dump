# Torqueboards 12s4p

### Replies: 30 Views: 2400

## \#1 Posted by: Battosaii Posted at: 2017-12-06T19:02:50.114Z Reads: 306

```
I purchased a 12s4p 30q battery pack from Torqueboards but the BMS says 30 continuous amps and 80amp spikes this seems to be a bit underwhelming considering the battery size. Is this normal or should I change the bms?
```

---
## \#2 Posted by: Skitzor Posted at: 2017-12-06T19:15:45.994Z Reads: 297

```
Not familiar with TB's battery model, but if the BMS is used for charging only. Your limits are the specs of the battery type used and not the BMS. Will check it out now.

Edit: it clearly states on his website "BMS is rated for 30A Continuous Amp Output and 80A Peak Amp Output."

Given they are 30 Q that's quite up to spec and the BMS is rated for this, so nothing to be gained by bypassing it.
```

---
## \#3 Posted by: Battosaii Posted at: 2017-12-06T19:23:22.987Z Reads: 278

```
Well I'm going from the specs on the website and I'm assuming it uses the bms for charge and discharge.
```

---
## \#4 Posted by: kyletrainy Posted at: 2017-12-06T19:28:37.429Z Reads: 265

```
30q cells are rated for 15A continuous so isn't the bms a bottleneck here?
```

---
## \#5 Posted by: jrpwit Posted at: 2017-12-06T19:43:18.378Z Reads: 258

```
Its probably only used for charging similar to enertion packs.
```

---
## \#6 Posted by: Battosaii Posted at: 2017-12-06T19:54:13.169Z Reads: 245

```
What do you guys recommend for battery vesc settings with this battery set up. I had 30 battery amps with my old 10s3p space cell set up maybe I can push 40-50 battery amps?
```

---
## \#7 Posted by: myreala Posted at: 2017-12-06T19:58:56.162Z Reads: 236

```
Its a 30Q 15A draw in 4P so total spec should be 60A draw. That means you can bypass the BMS for discharge rate of up to 60A draw. I am not sure how battery max per vesc works but If you have two vesc's you can set 30A per vesc and If you are using single VESC you should be able to set it up to 60A Also long as you bypass the BMS.
```

---
## \#8 Posted by: willpark16 Posted at: 2017-12-06T20:28:40.609Z Reads: 218

```
Are you sure it's the 30q one and not Panasonic
```

---
## \#9 Posted by: Exiledd_Top Posted at: 2017-12-06T20:30:03.081Z Reads: 213

```
They were some 12s4p 30q for sale on TB site for 300$ for cyber Monday
```

---
## \#10 Posted by: myreala Posted at: 2017-12-06T20:31:50.992Z Reads: 207

```
Those $300 were PanasonicPF ones, 30Q were $350 each.
```

---
## \#11 Posted by: Battosaii Posted at: 2017-12-06T20:32:46.162Z Reads: 198

```
Yep I spoke with Dexter and payed extra for the 30q cells
```

---
## \#12 Posted by: Exiledd_Top Posted at: 2017-12-06T20:36:14.503Z Reads: 198

```
<img src="/uploads/db1493/original/3X/a/2/a224d0ebc6329d10a80b0a7e26f29f7f1c51ab94.png" width="281" height="500">
I asked there support team and they said it was only balance not sure if they know or not
```

---
## \#13 Posted by: Battosaii Posted at: 2017-12-06T20:40:31.725Z Reads: 185

```
I'm not sure they know very technical stuff like that. I hope it's just charging
```

---
## \#14 Posted by: myreala Posted at: 2017-12-06T20:57:08.306Z Reads: 182

```
I wouldn't take them very seriously. They told once told me the BMS was 60A but the pack itself was 30A which made no sense as they confirmed it was a 30Q 12s4p pack.
Confirm it on your own, if it is not wired to be charging only then you can make the change. Its actually quite simple. I ordered this pack from them on Black friday I think. Still hasn't shipped. I have no idea what they are doing.
```

---
## \#15 Posted by: Battosaii Posted at: 2017-12-06T21:19:08.527Z Reads: 176

```
I got my tracking number last night so yours will probably ship soon, I think I was one of the first to buy it on Black Friday.
```

---
## \#16 Posted by: Namasaki Posted at: 2017-12-06T22:55:04.559Z Reads: 172

```
[quote="Battosaii, post:1, topic:40303, full:true"]
I purchased a 12s4p 30q battery pack from Torqueboards but the BMS says 30 continuous amps and 80amp spikes this seems to be a bit underwhelming considering the battery size. Is this normal or should I change the bms?
[/quote]


@torqueboards is the man with answers to technical questions.
```

---
## \#17 Posted by: myreala Posted at: 2017-12-06T22:58:19.632Z Reads: 170

```
That's good to know. Now just gotta wait for those Chinese parts that will take forever to arrive.
```

---
## \#18 Posted by: torqueboards Posted at: 2017-12-06T23:13:19.157Z Reads: 170

```
@Battosaii It's normal.  Ride it with the current BMS you should be able to hit 30mph+ if you want it faster you'll need to swap out the BMS. The current BMS is 30amp cont/80amp peak. Typically, you won't need much higher then that but you can.

@myreala 30Q packs are 30A Cont/80A Peak BMS. Cells are capable of more but the BMS is the limiting factor. Unfortunately, we're a bit delayed at this time as we are also moving into a new warehouse. We will be expanding our team very shortly to help ship out orders on a daily basis sometime in January. Doesn't fix the delays that are present now but they will for the future. Sorry :cry:
```

---
## \#19 Posted by: Battosaii Posted at: 2017-12-06T23:22:43.084Z Reads: 154

```
So I should run 15 battery amps each vesc? Seems a bit low honestly, but I'll mess with the settings worst case I'll use the bms for only charging like other have said but I'll use as is for now.
```

---
## \#20 Posted by: GrecoMan Posted at: 2017-12-06T23:38:33.101Z Reads: 160

```
on my 6s2p pack I was told by their support to run 50a batt. max
```

---
## \#21 Posted by: torqueboards Posted at: 2017-12-07T01:03:33.720Z Reads: 150

```
@Battosaii Yeah, I'd still run 40amp per VESC (Dual) and just let the BMS take care of it. VESC is just an extra pre-caution to limit amp output or if your battery didn't have a BMS and you wanted to limit output.
```

---
## \#22 Posted by: Battosaii Posted at: 2017-12-07T01:16:01.974Z Reads: 152

```
Nice I will try that, all my parts are ordered and most are already on the way now I just need to wait before I can build
```

---
## \#23 Posted by: BigBoyToys Posted at: 2017-12-07T01:21:03.083Z Reads: 151

```
@torqueboards

Hmm, how do your BMS's limit max current on your current battery models? On your 12S3P pack, exceeding the current max for thr BMS (which I did regularly lol) would completely turn off the battery and it would require a hard reset by cycling the power switch off then back on. A hard cut like that might be ok if it was hit during a hill climb but if it occured due to heavy acceleration at high speed it would create a pretty dangous sitiation of jarring decelartion and no brakes until it was reset. Considering such, max battery current of 40A or less per VESC might be the safer option.
```

---
## \#24 Posted by: torqueboards Posted at: 2017-12-07T02:06:23.381Z Reads: 145

```
@BigBoyToys - Yeah, correct. Thanks. I would retract what I said as far as 40-60amp and to stay safe keep it at 40amp. Single 80amp, Dual 40amp. I don't full throttle but if you plan on it 40amp is better. The battery will shut off if it hits pass 80amps.
```

---
## \#25 Posted by: Battosaii Posted at: 2017-12-07T02:21:53.871Z Reads: 144

```
I full throttle alot with my current set up  with 90mm wheels so I imagine the 107 set up with bigger motors and a12s battery will have about the same or similar torque as my 10s 90mm set up so I'll still be full throttling alot.
```

---
## \#26 Posted by: torqueboards Posted at: 2017-12-07T02:33:43.709Z Reads: 137

```
For 12S4P we'll be upgrading them to a 60A/150A BMS soon.
```

---
## \#27 Posted by: Battosaii Posted at: 2017-12-07T02:45:17.010Z Reads: 135

```
can i buy the BMS from you guys to upgrade my pack?

i have installed BMS's before i understand not everyone can install them but i can so is it an option for me or do i have to go somewhere else?

@torqueboards
```

---
## \#28 Posted by: BigBoyToys Posted at: 2017-12-07T02:48:22.486Z Reads: 130

```
Usually bms's rated for higher current will be larger so its unlikely to fit in the same battrry wrap/enclousure.
```

---
## \#29 Posted by: Battosaii Posted at: 2017-12-16T23:22:52.935Z Reads: 116

```
i tried out the battery today and i ended my ride early, either the display is not reading correctly or the BMS is not cutting power cause i ran the battery to 42v with what felt like no sag. whats a safe voltage i can run a 12s Li-ion battery to with out causing damage just incase the BMS is not doing its job?
```

---
## \#30 Posted by: Battosaii Posted at: 2017-12-16T23:30:03.176Z Reads: 116

```
nvm found my answer i could have ridden alot more holy crap.
http://www.electric-skateboard.builders/t/critique-my-vesc-settings-12s4p-dual-6355-190/32110/3?u=battosaii
```

---
