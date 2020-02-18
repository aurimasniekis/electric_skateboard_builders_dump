# Newbie, input is greatly appreciated!

### Replies: 20 Views: 1164

## \#1 Posted by: marcmt88 Posted at: 2017-08-03T03:03:06.377Z Reads: 122

```
Hi, did some research on how to wire a dual motors for my first build longboard.  I want to connect 2 packs in parallel of 6S2P to give me 6S4P.  Want to know what you all think of my wiring diagram.  Not sure how I am going to wire two 6S2P in parallel, I plan to use JST-HX connection.   Did I miss anything?  Thanks in advance!


<img src="/uploads/db1493/original/3X/1/a/1a54aec2e3edeb4f381f7b2d64e37bcabb793270.gif" width="690" height="388">
```

---
## \#2 Posted by: MrHappy Posted at: 2017-08-03T03:28:36.270Z Reads: 112

```
All "newbies" need to pay attention to this guy! 

I'm not exactly sure how those batteries are going to react to charging/discharging with that setup. Yes, it should work, I would just double check the voltages of your batteries after the first 1-5ish full discharge&charges. You want to make sure both of the pairs of cells are at the same voltage. (1&1, 2&2, etc.) Also, you don't need a XT90 key with an e-switch BMS but it won't hurt your board.

Thank you for doing your research, it keeps me from the sarcastic comment of "I don't know, google it"
```

---
## \#3 Posted by: marcmt88 Posted at: 2017-08-03T15:16:19.179Z Reads: 99

```
Thanks for the head-up.  Contemplating if I should up my batteries to 8S4P or 10S4P, pros: more power and longer ride time, cons: $ and extra weight.  Which 16850 battery should I use?  LG HE2 (20A cont. 2500mAh) or LG HG2 (20A cont. 3000mAh), does 500mAh difference justify the cost/benefit?  
Anyone has experience with Bestech BMS HCX-D223V1 with E switch?  How do you go about connecting those leads? 
http://www.bestechpower.com/256v8spcmbmspcbforlifepo4batterypack/HCX-D223V1.html
```

---
## \#4 Posted by: Schirmi Posted at: 2017-08-04T03:57:44.382Z Reads: 73

```
As a fellow esk8 noob, here are my 2 cents on the topic:
The connection between the lowest cells of your packs should also be a thick one.
Are you using LiFePO4 Packs ?, as that BMS will only work well with those kind of cells.
Other than that no problems.
As of charging or discharging your setup, there won't be any trouble, just keep in mind that there will now flow compensation currents in your balancing leads during operation. The magnitude of these depend on the difference in capacity of the connected cells, so make sure that this difference is small.
Also make sure that your two packs are balanced, when first connecting the cells, as there might flow huge currents if not done.

As for the 18650s, i personally would go for the HE2s because the HG2s are more than twice as expensive at my supplier and only deliver 20% more capacity.
```

---
## \#5 Posted by: marcmt88 Posted at: 2017-08-04T04:22:40.611Z Reads: 63

```
Thanks for the response.  I am planning on wiring my battery pack using 18650s.  I came across the mentioned BMS because it came with the e-switch feature.  Do you have a particular BMS that you recommend?
```

---
## \#6 Posted by: Namasaki Posted at: 2017-08-04T04:44:51.512Z Reads: 59

```
[quote="MrHappy, post:2, topic:29532"]
Yes, it should work,
[/quote]

No, it wont work because the balance wiring is incorrect.
```

---
## \#7 Posted by: Namasaki Posted at: 2017-08-04T04:55:48.532Z Reads: 59

```
Your diagram is very nice looking but the balance wiring is incorrect.
The bms will only have 6 balance wires, not 7
You can't run a balance wire for the negative side of cell 1 to pin 1 of the bms. If you connect the balance wires incorrectly the bms will either not turn on or it will smoke.
The bms you listed is for Lifepo4 cells.
The same version of bms is available for Li-ion/Lipo cells
http://bestechpower.com/222v6spcmbmspcbforli-ionli-polymerbatterypack/PCM-D223V1.html
The Bestech bms is a very good choice, I've been using them for about a year now with good performance and dependability.

If you are using Li-ion 16850 cells for a 6s4p then you should assemble  six 1s4p groups and wire those in series to make a 6s4p. This is the best and most simple way to build said battery.
```

---
## \#8 Posted by: michaelcpg Posted at: 2017-08-04T04:57:21.077Z Reads: 55

```
Samsung 30Q seem to be the go to around here for cost effective cells atm
```

---
## \#9 Posted by: Jinra Posted at: 2017-08-04T05:04:27.884Z Reads: 59

```
Some BMS's have an extra pin on the balance header for B-. At least my two bestech ones do.
```

---
## \#10 Posted by: Namasaki Posted at: 2017-08-04T05:07:54.931Z Reads: 60

```
the bms that was listed does not have a ground pin in the balance connector.
what model are you using?
```

---
## \#11 Posted by: Jinra Posted at: 2017-08-04T05:09:23.788Z Reads: 55

```
http://www.electric-skateboard.builders/t/small-bestech-bmss/25819
```

---
## \#12 Posted by: Bloop Posted at: 2017-08-04T05:11:09.396Z Reads: 54

```
The 30Q only give 15A so if you have 4 paralel you will have 60A that batttery can offer right ? let.s assume your mottor also cand use up to 60A.

Isnt it a bit at limit ?
```

---
## \#13 Posted by: Namasaki Posted at: 2017-08-04T05:16:20.871Z Reads: 54

```
@marcmt88 has a Bestech HCX-D223V1 in his diagram.<img src="/uploads/db1493/original/3X/8/f/8ff982da588b6b7b451262bcdda6892c3d823057.png" width="430" height="430">
```

---
## \#14 Posted by: Jinra Posted at: 2017-08-04T05:16:31.108Z Reads: 53

```
Rated for 15A, but real world testing that 20A is suitable as well. Cells can draw however much you want to draw from it, problems arise when heat is too high. 30Q's have proven to maintain a good temperature at up to 20A current. Even with 60A, you won't be drawing that much continuous often anyway.

It actually makes me wish the VESC had an option for burst current as well.
```

---
## \#15 Posted by: marcmt88 Posted at: 2017-08-04T16:40:20.836Z Reads: 46

```
Yes, your are absolutely correct!  see new diagram. <img src="/uploads/db1493/original/3X/2/e/2e5883227c7605dafdbdf3d895cca78ab7355dd4.gif" width="690" height="388">
```

---
## \#16 Posted by: Jinra Posted at: 2017-08-04T16:44:27.286Z Reads: 43

```
your B- is not in parallel.
```

---
## \#17 Posted by: marcmt88 Posted at: 2017-08-04T17:09:58.565Z Reads: 42

```
Thanks for pointing that out!
```

---
## \#18 Posted by: Namasaki Posted at: 2017-08-04T18:02:53.945Z Reads: 41

```
I still don't get why your assembling the cells like that
```

---
## \#19 Posted by: marcmt88 Posted at: 2017-08-04T18:07:43.733Z Reads: 39

```
Just for the sake of correcting wiring.  I definitely consider your suggestion of six 1s4p groups and wire those in series to make a 6s4p.
Thanks.
```

---
## \#20 Posted by: marcmt88 Posted at: 2017-08-05T00:21:29.811Z Reads: 37

```
Namasaki, 
Thanks for the advice.  Here is my corrected wiring as suggested by you<img src="/uploads/db1493/original/3X/5/6/5667a26e9063338ea026636fd4f8bcf27b2e960f.gif" width="690" height="388">.
```

---
