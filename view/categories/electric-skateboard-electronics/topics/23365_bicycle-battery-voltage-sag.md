# Bicycle battery voltage sag

### Replies: 13 Views: 999

## \#1 Posted by: Vaulter92 Posted at: 2017-05-18T08:48:36.727Z Reads: 104

```
Hi
Recently I found a bicycle battery on the junkyard, disassembled it and found out that just one of the protection circuits was damaged. After a short research I found out that it is a 10 cell Lithium Ion battery with 12Ah capacity. I took 6 of those cells and built them into my eboard. Yesterday I was doing the first "long range" test (about 12.5 km in total) and experienced a very high voltage sag on the last few kilometers. I was driving on flat streets only and I am using a single drive SK3 6355 260 Kv motor and the X-Car beast 150A ESC. At the end I was left with 18 Volts /0% which recovered to 10% after some time of rest.
After recharging the charger stated that only about 7 Ah where required to get back to 100 %
So what about the other 5 Ah?
Did I draw too much current? maybe bisycle batteries are rated for low current draw?
Sadly I have thrown away the old housing so I am not able to check the continuous current draw for this battery.
Do you have any suggestions?
I am thinking about using the whole 10 cells to make a 5S2P batery?!
thanks in advance for your help.
```

---
## \#2 Posted by: TarzanHBK Posted at: 2017-05-18T09:10:36.449Z Reads: 100

```
There are only a few Liion Cells which are capable of our high current draw we use in eboards. So have you checked what cells these are? You can´t use only 6 cells or even 10 cells to build an eboard. We´re usually using min. 30 cells, better 40 cells to build a battery that is capable of our demand. You definitely damaged them.
Read a bit more into this before you make moves like this and have damaged components afterwards.
You can also tell us your plans here and people going to help you or tell you if it´s a good idea or not.
```

---
## \#3 Posted by: Vaulter92 Posted at: 2017-05-18T09:35:36.298Z Reads: 91

```
I am not talking about single round cells. the dimennsions of a single cell is 7 by 14 cm and looks as follows:
<img src="/uploads/db1493/original/3X/0/2/02033d02bb765da809b96cd3e6040fb6a3c2e80f.jpg" width="375" height="500"><img src="/uploads/db1493/original/3X/c/b/cbd63e1b94cc04d9a860c63544c9f2724c1c937b.jpg" width="666" height="500"><img src="/uploads/db1493/original/3X/5/3/533f2abda8149f8839bb2b361c3619de9ac7b4c3.jpg" width="666" height="500">
In the pictures you can see the remaining unused 4 cells and the assembled 6 cell battery. I thought that there might be round cells connected in parallel in one of the aluminium compartment.
Dimensionwise 5 of the samsung 18650 cells would fit into one of these cells.
Furthermore I limited my current draw to 40A max. Have a 40A fuse installed and never fried it unless there was a short or something. Has anyone ever seen such an alu case for batteries and is it likely that it is one cell or there are several cells inside in parallel?
```

---
## \#4 Posted by: TarzanHBK Posted at: 2017-05-18T09:40:09.265Z Reads: 87

```
hmm I´m not sure what kind of battery that is. There is no number or name on it, so you could google it and find out about the specs?
```

---
## \#5 Posted by: Vaulter92 Posted at: 2017-05-18T09:55:05.133Z Reads: 80

```
<img src="/uploads/db1493/original/3X/5/a/5a7e36a068bd52dffaed023bc62341cb2d29490e.png" width="690" height="388">
I guess I found it (at least from the picture it seems very similar. it says 6 cells in parallel and 10 cells in series which would fit the dimensions quite well. and rated curent is 15A.
so when I do 5s and then in parallel I would have a rated current of 30A right?
And since I do not even reach 40A since my fuse does not fry I should be fine with that?
And sorry for the german language in the picture...
```

---
## \#6 Posted by: DeathCookies Posted at: 2017-05-18T10:50:42.315Z Reads: 70

```
Just because it Looks similiar it does not have to be similar.... 
Your fuse can porbably handle more than 40A for a short amount of time not continously.
```

---
## \#7 Posted by: Okami Posted at: 2017-05-18T12:43:58.905Z Reads: 68

```
The batteries do look very interesting..

I wouldnt suggest drawing much more power below 10% anyways.. so leaving at least 15-20% in battery is probably wise (especially if power demand is high).

How did you manage to get 6s out of them anyways?

They are somewhat 10s right when connected together?

And yeh, ebikes unfortunately very often use lower power batteries in terms of amps, as you can see, a common power limit for them is 250 - 500w and usually higher powered setups just build their own batteries, I think.

At 36v that is below 10A or 20A at most I think, being 15A in the middle, since low grade chinese controllers also output only max 20A I think and usually for ebike with human power assist that might be enough already.
```

---
## \#8 Posted by: Vaulter92 Posted at: 2017-05-19T09:58:14.916Z Reads: 53

```
Ok, I will make a 5s2P setup out of it tomorrow I guess. Will keep you updated and also show the process.
```

---
## \#9 Posted by: Vaulter92 Posted at: 2017-05-21T15:04:14.053Z Reads: 48

```
Here is what I have done with the batteries.
<img src="/uploads/db1493/original/3X/3/c/3c7cd4f87c1b9335c73e1837e06992570135c3b0.JPG" width="690" height="460">
<img src="/uploads/db1493/original/3X/1/6/1680e289218b82e5fe69a01fe100997f0b970a2f.JPG" width="690" height="460">
Unwrapped the battery and started to disconnect all the wires.
<img src="/uploads/db1493/original/3X/b/8/b85f7eb4176b26b0626cd0fa89e857d5022a1093.JPG" width="690" height="460">
Thats what a single cell looks like.
<img src="/uploads/db1493/original/3X/3/6/36e9701218b33e91f32f0a267e2a671645158fe3.JPG" width="690" height="460">
<img src="/uploads/db1493/original/3X/0/b/0b5f616b64a0e5d90b1e8abcc2c148579834c62b.JPG" width="690" height="460">
Then I had to isolate the remaining four cells that I have not used before.
<img src="/uploads/db1493/original/3X/a/a/aac86450661978e25923b6d191bad59a86843c8b.JPG" width="690" height="460">
<img src="/uploads/db1493/original/3X/d/7/d711a5b429e78bcab9b904cdb8af01d1dc7372e0.JPG" width="690" height="460">
<img src="/uploads/db1493/original/3X/3/8/387bed240bff611eb242e45812ad58c6988e5495.JPG" width="690" height="460">
Cut off the circuit board...its garbage

<img src="/uploads/db1493/original/3X/7/f/7ff6c6d028eadac0bd2a7e5b9f525a37e9848c5d.JPG" width="690" height="460">
And cut and unsoldered all the wires.
<img src="/uploads/db1493/original/3X/c/4/c41cd01df41fe0cf3b5ef2c64433370a9e1fc396.JPG" width="690" height="460">
You can see that there are those little metal sheets that connected some poles. These came out really handy since I could just solder on those. I do not have access to one of those battery weld thingies (right now I don´t recall the name of that device).
<img src="/uploads/db1493/original/3X/0/c/0ce36a13885548220e25705476d2712d8422b2a1.JPG" width="690" height="460">
Cut off everything that hold the cells together.
<img src="/uploads/db1493/original/3X/5/c/5cc5abbadafe93e298e3f88061786c3effe9548e.JPG" width="690" height="460">
And finally four recycled cells.
I wrapped all of them in Tape individually and then sorted for same voltage:
<img src="/uploads/db1493/original/3X/d/0/d0916fe2615dd445254ad9f9b76c2cd2fe1ddc07.JPG" width="690" height="460">
<img src="/uploads/db1493/original/3X/b/5/b5bf2a3f7cf84a82490d268fd724f1058eee0dcf.JPG" width="690" height="460">
And wrapped them:
<img src="/uploads/db1493/original/3X/d/5/d5eb7ae4980ab79bd9a8b1184b6efea079dcedc1.JPG" width="690" height="460">
Then some soldering:
Connecting the parallel cells:
<img src="/uploads/db1493/original/3X/f/8/f8985f811bb27c9fd59b949b9f6b16913228fa38.JPG" width="690" height="460">
<img src="/uploads/db1493/original/3X/8/a/8add1cac315b3accb37a01bf430ac073d228fb4a.JPG" width="690" height="460">
Then the serial connections:
<img src="/uploads/db1493/original/3X/a/f/affb989f19d7c7d9381feb0335f63a6116cd50df.JPG" width="690" height="460">
And it worked out quiet fine.
Then soldering the balance leads and the discharge negative and positive with an xt_60 connector.
<img src="/uploads/db1493/original/3X/4/7/47fcaabf8eb3e1c987991d5c67a32a1adc852ea3.JPG" width="690" height="460">
<img src="/uploads/db1493/original/3X/c/f/cf67355e5c7258099ba970d6f5a9b0c85de60295.JPG" width="690" height="460">
The connector looks really ugly though since I ran out of shrink tubes when I soldered this one a few months ago and I was too lazy to redo it. Since it is in the housing you do not see it anyways :smiley:. 
Finally wrapping everything:
<img src="/uploads/db1493/original/3X/a/6/a6b0d6fddc14cda28149cd624aa2a99c09bc621d.JPG" width="690" height="460">
<img src="/uploads/db1493/original/3X/6/3/63e185e09d799090710dac5d1611e6c4d8ccdeff.JPG" width="690" height="460">
And here is the 5S2P battery. Should now have 24Ah with 30A continuous current.
I am charging it right now and testing it over the next week.
```

---
## \#10 Posted by: Okami Posted at: 2017-05-21T16:08:17.597Z Reads: 38

```
Nice pictures. Yeh report the results later. Should give you a lot of range. 
Im curious how much capacity you are really going to get out of these batteries / pack.
```

---
## \#11 Posted by: Vaulter92 Posted at: 2017-05-30T12:35:57.319Z Reads: 30

```
It turned out that I get a range of maybe 12-15 km out of this battery pack. I could b not charge it up to 100% since it took ages to get to 92% (like five hours). The voltage sag was really high so I decided to go for my lipo packs again. Nevertheless it was a really great project and I learned a lot about batteries. Since I found the battery on the junk yard it only cost me some tape, solder and a lot of time.
```

---
## \#12 Posted by: ugothakd Posted at: 2017-05-30T15:50:17.094Z Reads: 22

```
Isn't that circuit board a balancer? I definitely think the cells will not charge and discharge evenly like that
```

---
## \#13 Posted by: Vaulter92 Posted at: 2017-05-30T15:53:47.391Z Reads: 21

```
Well, they definately charge evenly since I am using an Imax B6 for charging. With discharging you are right but there are a lot of boards out there using for example lipos without bms for discharge and it works fine. I through the circuit board away since it was an unknown to me especially with the changed number of cells in series.
```

---
