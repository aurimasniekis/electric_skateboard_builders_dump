# SOLVED- Wiring BMS, bypass discharge 10S, anti spark- help please

### Replies: 31 Views: 4481

## \#1 Posted by: MontPierre Posted at: 2017-07-17T20:15:06.118Z Reads: 455

```
Hi!

I have read 10's of posts about wiring BMS to bypass discharge and I'm still confused. I'm sorry to bother but conflicting posts have confused me ( red wire in balancing cable being last cell or that it doesn't matter ... etc). 

I would be grateful for help with finishing of below drawing.

I have 2x3S Zippy 8000mah and 2x2S Zippy 8000mah to make 10S ( same C rating, capacity and make) , I also have colour coded cables from each battery as they are on my Zippy's. Am I right that black wires have to be cut out apart of the one in first battery? or is it the reds? ehhh

My BMS is a cheap one from eBay - below is wiring diagram from the manufacturer. 

As I'm adding Vedder anti spark switch it all got too much for me in terms of wiring.

Below is my drawing so far, please feel free to change it.

Thank you in advance! 


<img src="/uploads/db1493/original/3X/5/5/5592343f751e9c3362d24fa2ed2c8af95be50375.png" width="449" height="500"><img src="/uploads/db1493/original/3X/3/7/37847227d4d5a88a340936189674f020c750d23c.jpg" width="649" height="500">

I've got this so far but not sure at all it this is going to work.

<img src="/uploads/db1493/original/3X/0/5/059a97d986e4793a3ec100c841b3dad7d9627aca.png" width="402" height="500">
```

---
## \#2 Posted by: cricrithezar Posted at: 2017-07-17T22:00:11.950Z Reads: 394

```
At a glance, looks right to me. Just make sure your cells are the same (like same capacity and C rating at least) so they don't get too unbalanced since you're using a cheap BMS. Using 5 2s batteries would have been easier to make sure of that but if you already have them and they have the same specs go for it.
```

---
## \#3 Posted by: darkkevind Posted at: 2017-07-17T22:08:38.643Z Reads: 388

```
Best thing to do is wire your battery up like you don't have a BMS. Then wire up the BMS's balance leads to the relevant cells. In this diagram, there's no need to connect the B- to the BMS with the same wire you're using as output. It need only be a thin balance wire like the others.
```

---
## \#4 Posted by: MontPierre Posted at: 2017-07-17T22:15:28.356Z Reads: 382

```
@darkkevind - just like that? Can I use the thin balance wire from last battery?It is connected with negative wire right?
 
<img src="/uploads/db1493/original/3X/e/9/e9e0a51ba8a26304328436c9afb78d589a41ae50.png" width="412" height="500">
```

---
## \#5 Posted by: MontPierre Posted at: 2017-07-17T22:16:30.826Z Reads: 357

```
@cricrithezar They all are same C rating, capacity, make and same supplier. I even checked voltage with multimeter and all looks good - same values, almost.
```

---
## \#6 Posted by: darkkevind Posted at: 2017-07-17T22:17:42.179Z Reads: 356

```
Yes, that's fine. You can do the same with the plus as well on the other end. No need to connect to the output plus wire. Use separate lower gauge wires for the charge port.
```

---
## \#7 Posted by: MontPierre Posted at: 2017-07-17T22:22:08.844Z Reads: 351

```
True, it will be only small current, 2A max - my charge won't give more. But the two main wires going to anti spark  from switch and battery I'll leave at 12AWG.

Thank you for your help @darkkevind ! I can finally go to bed after working this out for HOURS :)
```

---
## \#8 Posted by: darkkevind Posted at: 2017-07-17T22:28:13.936Z Reads: 339

```
Yes, definitely leave them at 12awg :slight_smile:
```

---
## \#9 Posted by: Moav Posted at: 2017-07-31T09:59:29.318Z Reads: 314

```
If I have battery system with 2 10S sets of batteries in parallel for higher Ah, can I plug them to a 20S BMS even though they are not in series?
```

---
## \#10 Posted by: krloz Posted at: 2017-07-31T10:06:06.112Z Reads: 324

```
No.
If you have a series of 10s you wire a 10s bms. What you want is that all connections are parallel between both sets
@Moav
```

---
## \#11 Posted by: krloz Posted at: 2017-07-31T10:08:05.306Z Reads: 319

```
Be careful.  Some bms require you to wire both the first balance cable to the balance connector AND the thick black cable to B-. I would wire both to be sure although they do carry the same connection to the battery
```

---
## \#12 Posted by: MontPierre Posted at: 2017-07-31T10:12:11.271Z Reads: 311

```
Otherwise you'll fry it like I did ;) make sure you connect balancing cables at the end !!! First all other connections
```

---
## \#13 Posted by: krloz Posted at: 2017-07-31T10:24:47.103Z Reads: 303

```
Omg. Did you actually fry if for that? I didn't notice the dates.  Sorry for piling up on your accident :joy:
```

---
## \#14 Posted by: Moav Posted at: 2017-07-31T10:48:42.935Z Reads: 294

```
I'm sorry I don't understand which connection should be parallel, 2 BMS's for both battery sets, then the batteries in parallel, and one power supply. Correct?
```

---
## \#15 Posted by: krloz Posted at: 2017-07-31T12:51:08.169Z Reads: 279

```
 You can wire 2 packs of 10s lipo together in parallel to a single bms. Ill try and make a diagram later.  Did you search the forum to see if there already is a diagram?
```

---
## \#16 Posted by: Moav Posted at: 2017-07-31T18:04:13.971Z Reads: 292

```
Yes, a dozen times, but I as well can't believe I'm the only one trying that.
This is as far as I know. I don't know how to pass the BMS for discharge though I think I can get one that discharge at 100A or more.
<img src="/uploads/db1493/original/3X/3/c/3c53ee4848bd776beb028b1c556c76d110971373.JPG" width="353" height="500">
```

---
## \#17 Posted by: krloz Posted at: 2017-07-31T21:53:52.724Z Reads: 275

```
You got the balancing part right there.  Not quite sure about that power switch you have.  Do you have a link for your bms so I can correct and add the output to vesc. 
Also what are you planning on using to turn on the board? Xt90s Loopkey? Antispark switch? If that is a normal switch in the diagram it is wrongly wired, and not the best option
You are not the only one.  I have nearly the same setup.  The problem is my diagrams usually stay in my head.  And you don't want to go there and check.  Trust me
```

---
## \#18 Posted by: Moav Posted at: 2017-08-01T10:18:01.020Z Reads: 262

```
LOL! that's fine I love twisted minds..

So my power switch is an vedder anti spark with a power switch, and I've seen one of those BMS's here somewhere but if you can suggest one with how to wire them to the batts that would be great!

Thanks dude
```

---
## \#19 Posted by: krloz Posted at: 2017-08-01T10:39:49.470Z Reads: 260

```
<img src="/uploads/db1493/original/3X/5/c/5c2bdcb0b1f3282ac60e01cb322e0fef6af047b7.jpg" width="666" height="500">
There you go.  Choose either bypassing discharge or not.  Only use discharge protection if your bms can handle the amps.
  I moved your vmeter after the switch.  You can wire it where you had it but it would be on 24/7. I wouldn't

Btw. If your bms is not marked b- p- and c- post a picture or a link and I'll clear up
```

---
## \#20 Posted by: krloz Posted at: 2017-08-01T10:46:59.613Z Reads: 241

```
Oh. And your balance connector in the bms should have 11 wires.  Tell me if it has less
```

---
## \#21 Posted by: Moav Posted at: 2017-08-01T11:31:37.588Z Reads: 230

```
Thanks buddy, appreciated!!
I think I'll go with the low discharge BMS as my VESCs are protecting my batts from unwanted discharge effects.
```

---
## \#22 Posted by: Moav Posted at: 2017-08-03T10:05:21.135Z Reads: 231

```
<img src="/uploads/db1493/original/3X/d/6/d6e1dc6dee17f57d700e601643fa2e7a6dad4ec3.jpg" width="353" height="500">

This is the BMS I've chosen although Lucy from BesTech recommended getting the same BMS only with 20S Balance lids. Is that seems logical?
```

---
## \#23 Posted by: krloz Posted at: 2017-08-03T10:22:37.415Z Reads: 218

```
[quote="Moav, post:22, topic:27876"]
getting the same BMS only with 20S Balance lids. Is that seems logical?
[/quote]

Do you mean she recomended a bms for a pack of 20s? Or a bms with 20 pins?  Maybe they are extra pins for other things.  Did you explain it was meant for a 10s2p and not for a pack of 20 cells? This are the only reasons i can imagine for the confusion.  If you have 20 cells in series you WILL get up to 84V and blow the vesc. 

Any way the bms you post is perfectly fine.  You can even use discharge protection depending on your does power draw and vesc configuration
```

---
## \#24 Posted by: Moav Posted at: 2017-08-03T11:20:06.029Z Reads: 211

```
I've tried to explain that I've 2 10SP1 packs in parallel, but as I understand you cannot balance 20 cells in which 10 are in parallel though I don't understand why. I trust you that it is safe to parallel balance the two packs in pairs, so I'll get one of those and hope for the best. Maybe I could plug them in series just for charging, but that seems complicated.
```

---
## \#25 Posted by: Wilsonliang777 Posted at: 2017-11-01T18:57:23.051Z Reads: 178

```
I am also trying to use a cheap bms for my 10s lipo pack.  I want to use your wiring diagram to bypass the discharge.  Before I start working on it could you tell how this battery bms set up work out.  

Thank you.
```

---
## \#26 Posted by: MontPierre Posted at: 2017-11-01T18:59:16.143Z Reads: 174

```
I have ended up not bypassing BMS. Try to search forum for bypassing, you’ll find a lot of diagrams which will help. 

Mine Worked out fine, with bms on discharge ;)
```

---
## \#27 Posted by: MontPierre Posted at: 2017-11-01T19:00:48.513Z Reads: 173

```
I made an error and didn’t pay attention to balancing wires and didn’t connect them in order and burned my bms. So that’s important
```

---
## \#28 Posted by: MannyM0E Posted at: 2018-03-25T18:29:22.412Z Reads: 145

```
Need help. Using only for charging. I believe I did everything correct but once I plugged the charger into the port, a spark happened on the charging port socket and the charger socket. I have the negative of the battery connected to the B- also with the last balance cable.Also advoiding the red wire on my negative battery. CH- connect to the negative charging port and the positive battery connected to the positive charging port. I didn't connected anything to the P- because I believe that's only for discharging What could had happened ? I notice my charging port  has 2 negative and 2 positive as well 

![IMG_3927|660x496](upload://6eF1JY2Z4A9xhqAVpkKIAKJkO1P.PNG)![IMG_3928|375x499](upload://4yF5ZlNKFIXcGhh5b7gBtEgIGcf.PNG)![IMG_3929|369x500](upload://1hG2CUXuW9ynOrLJ93B1I26rCRO.PNG)
```

---
## \#29 Posted by: Lambjr088 Posted at: 2018-03-25T20:05:57.408Z Reads: 138

```
If we wire it using the alternative you have provided will the bms drain the battery? If i have a esc that has a on/off button and wire it to bypass the discharge will it also drian the battery?
```

---
## \#30 Posted by: krloz Posted at: 2018-03-26T16:25:41.082Z Reads: 134

```
Theoretically a decent bms shouldn't discharge the battery faster than the battery's own self discharge.
 If you bypass discharge that means you are connecting your esc directly to battery.  In that case you need some sort of disconnect or your esc WILL dangerously discharge the battery
```

---
## \#31 Posted by: krloz Posted at: 2018-03-26T20:40:05.736Z Reads: 131

```
Just to be clear.  I'm not saying the on/off on an esc won't do. I'm saying it will do only if it fully cuts off power instead off putting it in a stand by mode. 


I however will always recommend prying a xt90s loop key somewhere even if you never use it. Just in case the rest fails and you have to quickly turn it off
```

---
