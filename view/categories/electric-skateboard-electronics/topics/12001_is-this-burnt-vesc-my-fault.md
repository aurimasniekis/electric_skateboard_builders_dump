# Is this burnt VESC my fault?

### Replies: 20 Views: 1717

## \#1 Posted by: Cjnutts Posted at: 2016-10-27T15:35:51.038Z Reads: 209

```
 So Monday morning I took my mountain board for a very quick spin.( not extensive, very quick) I brought it into the shop, hooked it up to the laptop and switched everything into FOC because it works very well on my single motor longboard (Sk3 149kv-9s). When I was done I shut the board off turned it back on, turned on the remote and one wheels spun and the other VESC started to smoke. I just want to know if it's my phone but I don't care either way I just need to know. I can handle it . If so what did I do? 
Thanks guys, hope I did this right if not just kick me off and  i'm going to try to download some pictures 
2-Tb VESC & 2-Tb 6374 230kv  sensored but running on sensorless .12 lipo
<img src="/uploads/db1493/original/3X/d/9/d96da11e71b2766e8683fb2a5b4d927d086f9f62.jpeg" width="669" height="499"><img src="/uploads/db1493/original/3X/b/b/bba09033f8f07a0e34d32eb8fda78a0377fe532b.jpeg" width="373" height="500">
```

---
## \#2 Posted by: treenutter Posted at: 2016-10-27T16:06:31.151Z Reads: 199

```
@Cjnutts It looks like the positive power lead is not soldered to the cap board. It may have disconnected and shorted; frying your DRV chip. You'll need to replace the chip.

Is it your fault? Hard for us to say I think. In general, when you switch from BLDC mode to FOC mode I'd suggest doing a firmware update/reset to make sure there are no lingering settings that impact the new config. That's what I've done and it seems to work.
```

---
## \#3 Posted by: zmoney Posted at: 2016-10-27T16:10:29.408Z Reads: 197

```
From what i've heard, TB has been using the 4.10 HW, which means that C26 is missing. This might have been the cause for this. I'd replace the DRV and at the missing caps.
```

---
## \#4 Posted by: Blasto Posted at: 2016-10-27T16:11:51.513Z Reads: 192

```
The capacitor board seems to have cold solders, even on the wires still connected.
```

---
## \#5 Posted by: JohnnyMeduse Posted at: 2016-10-27T16:21:53.539Z Reads: 182

```
Well, It won't burn the drv like that !
```

---
## \#6 Posted by: Pantologist Posted at: 2016-10-27T16:31:10.448Z Reads: 172

```
What would? A short?
```

---
## \#7 Posted by: Pantologist Posted at: 2016-10-27T16:38:51.683Z Reads: 166

```
Yeah, that capacitor was added for FOC stability.

It seems that everyone with a TB vesc running FOC has an issue.
```

---
## \#8 Posted by: JohnnyMeduse Posted at: 2016-10-27T16:55:26.386Z Reads: 157

```
These kind of damage require a massive amount of energy, so yeah probably a short over the motor lead or on the power (witch look like the case in this situation)
```

---
## \#9 Posted by: Cjnutts Posted at: 2016-10-27T17:20:13.595Z Reads: 149

```
 It's kind of what I was thinking,  I think. I suppose I'll just order two new Ollin VESC  this time around. Seems to be what everybody's talking about. 
          _ thanks you guys rock
```

---
## \#10 Posted by: lox897 Posted at: 2016-10-27T21:20:41.780Z Reads: 126

```
VESC + Mountain Boards isn't a good mix anyway. Ask @barajabali
```

---
## \#11 Posted by: Cjnutts Posted at: 2016-10-27T21:26:50.885Z Reads: 124

```
 For real?  Why is this the first time I'm hearing this?  Do others concur ?
```

---
## \#12 Posted by: lox897 Posted at: 2016-10-27T21:27:32.374Z Reads: 122

```
They tend to break a lot more due to higher amps I believe.
```

---
## \#13 Posted by: barajabali Posted at: 2016-10-27T22:44:04.414Z Reads: 115

```
I would reccomend the TB esc. I have 2 spare used ones if you want. 

Maybe 150 miles on them running strong
```

---
## \#14 Posted by: caustin Posted at: 2016-10-28T03:04:07.267Z Reads: 110

```
Emtb and vesc not a good match. @kaly just opined a sec ago on separate thread coincidentally lol
```

---
## \#15 Posted by: onloop Posted at: 2016-10-28T09:01:10.259Z Reads: 97

```
VESCX should resolve these concerns. Improved thermal dynamics and upgraded components to handle the voltage spikes.

Of course an efficient drive train is always important. Plenty of reduction and geared for a top speed that won't be impacted heavily by wind resistance.
```

---
## \#16 Posted by: TarzanHBK Posted at: 2016-10-28T09:19:43.781Z Reads: 95

```
because noone mentioned it before: 12s plus 230kv on a vesc is much to high!

also like others said - go for a 12s esc.
```

---
## \#17 Posted by: Zama Posted at: 2017-08-05T22:56:09.813Z Reads: 61

```
Hello there! We have the same problem. We're testing 2 VESC's. Our prototype was powered by two sets 6S (LiPO 22.2 V 5200 mAh 35c 6S) each. But on an experimental basis without BMS. Only the batteries connected directly at VESCS.

We use too two motors with the following specifications:

KV: 170
Idle Current: 0.8A
Max. Current: 65A
Input Volt.: 2-12s Lipo Max. Output Watt: 2000W Max. Pull: 9700g
Rated Current: 60A
Motor Weight: 765g
Shaft: 8mm
Internal Resistance: 0.0402 With black closed cover

Everything was going very well and in three weeks of tests we obtained excellent results, but in the fourth week this happened with the VESC’s:

<img src="/uploads/db1493/original/3X/7/3/730fd8c3ff36dc5f91e81c55ac00f8a91a2ec579.jpg" width="280" height="500">
```

---
## \#18 Posted by: Jinra Posted at: 2017-08-05T23:01:00.925Z Reads: 56

```
wow that's a huge hole. I'm guessing Maytech VESC? Were you using BLDC or FOC?
```

---
## \#19 Posted by: Zama Posted at: 2017-08-05T23:51:05.910Z Reads: 50

```
BLDC @Jinra
```

---
## \#20 Posted by: TarzanHBK Posted at: 2017-08-07T06:57:44.495Z Reads: 35

```
that´s another dead maytech there, you can see that on the internal certification sticker they use.
What are you doing with all 4 Canbus cables connected?
```

---
