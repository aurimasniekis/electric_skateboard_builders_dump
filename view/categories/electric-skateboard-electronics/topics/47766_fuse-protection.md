# Fuse protection

### Replies: 39 Views: 2592

## \#1 Posted by: Ingvarjedi Posted at: 2018-02-28T17:00:24.948Z Reads: 367

```
You'll probably laugh for me, for my insanity or not knowing.

I would like to use a fuse, put it between batteries and VESC.

I used Li-Po 12s 5000mAh 25C and motor 192kv 80A and VESC 4.

1. Which fuse to choose?
2. How many amperes = 80A or more?
3. On which wire should I put a plus(red) or minus(black)?

![25|690x488](upload://qvqfnN5bz6OIGI3b3Aw2xRvOWll.png)![19|616x500](upload://1wDZ79zPaehSlupegqKldwxuuHM.png)

And now madness.
Can I use it?
There is a single-pole and two-pole??
![42|315x499](upload://ev4rOhBOeuU5ehGcQNmkJ3CN0UK.jpg)
```

---
## \#2 Posted by: Acido Posted at: 2018-02-28T17:07:12.623Z Reads: 353

```
Polarity on the first one does not matter since only one pole is going thru, I reccomend the first option.
The amp rating depends on how many amps you will pull from your battery if you put it betweeen battery and bms/esc
```

---
## \#3 Posted by: laurnts Posted at: 2018-02-28T17:30:50.261Z Reads: 349

```
I have the first on exact same with 80A. Its abit too much I think, the smaller 30A also does the job well. I mean you dont get really to draw continuous 60 - 70A, so 80A is just wayyyyy ovver the top.
```

---
## \#4 Posted by: Sebike Posted at: 2018-02-28T17:44:15.703Z Reads: 337

```
There are a few threads going through these exact topics already...
```

---
## \#5 Posted by: krloz Posted at: 2018-03-01T11:14:24.349Z Reads: 308

```
https://www.electric-skateboard.builders/t/wiring-up-an-in-line-fuse/35304/5?u=krloz
```

---
## \#6 Posted by: Acidfie Posted at: 2018-03-01T11:52:13.187Z Reads: 297

```
as far as i can say, i would never use a fuse.

simple as that, if the fuse blows because you drain too much amps (mostly going downhill/uphill) and the connection between VESC and Batterys is lost, your VESC will blow up because it cant forward the electric energy that is produced by the motors. so if your fuse blows, you will probably lose your VESC(s) and maybe your battery. Also you can be injured because no brakes!
```

---
## \#7 Posted by: Bataleon Posted at: 2018-03-01T12:12:47.893Z Reads: 274

```
[quote="Acidfie, post:6, topic:47766"]
the connection between VESC and Batterys is lost, your VESC will blow up because it cant forward the electric energy that is produced by the motors.
[/quote]

Wow, is this really true? I always thought I was lowering chances of a damaged VESC by using an inline fuse.
```

---
## \#8 Posted by: Nordle Posted at: 2018-03-01T12:29:36.512Z Reads: 253

```
Thats true but you probably never ever will produce that many amps while braking, and in the reverse case you will notice a 100% loss of power, you just don't have to hit your brakes then.. simple as that.
The fuse however is very usefull as it protects your battery from short circuit, doesn't do much to protect your vesc.
```

---
## \#9 Posted by: Stevemk14ebr Posted at: 2018-03-01T13:56:43.179Z Reads: 247

```
If your fuse didn't blow all the hardware would blow up anyways, since you know, your fuse just stopped a huge in-rush of current.
```

---
## \#10 Posted by: krloz Posted at: 2018-03-01T15:44:40.329Z Reads: 242

```
In our aplications fuse should be rated high enough for their main use to be to prevent a short to the batteries that could make your full board go up in flames with you on top. So screw the vesc
```

---
## \#11 Posted by: Acidfie Posted at: 2018-03-01T16:18:12.866Z Reads: 241

```
It can happen, @Nordle you can create very powerful currents while braking downhill e.g.

Also, if the VESC loses connection to the battery, the motor can induce voltage and the vesc could be powered on just "half" and some application configurations or programm configurations can be lost. if powering on without checking it could blow up your VESC
```

---
## \#12 Posted by: Nordle Posted at: 2018-03-01T17:14:23.034Z Reads: 237

```
Sure it can happen but you will recognize first and you can react accordingly.
And no you can't create more current than you set in your settings, if you could your vesc already would be faulty.
```

---
## \#13 Posted by: cosmicc89 Posted at: 2018-03-01T18:06:03.756Z Reads: 235

```
If you have no fuse and aren't discharging off a BMS and you get a short circuit, your battery probably catches fire and destroys the entire board, so you're probably losing the expensive battery at the very least. What if it shorts while its in your house and causes serious fire damage? If your battery is actively shorting, your VESC probably won't respond at all anyway since power isn't getting to it and it can't activate braking. If you're going downhill, power is being dumped into the battery which is short circuiting which makes everything worse anyway.

If you do have a fuse, the fuse blows and you lose a <$200 VESC and a $5 fuse at the most. No fires, no property damage. If you're wearing appropriate safety gear, you bail and roll and come away with no injuries. 

Seems pretty clear to me...
```

---
## \#14 Posted by: cosmicc89 Posted at: 2018-03-01T18:07:49.903Z Reads: 226

```
P.S. I juse a 60A JCase fuse:
http://www.littelfuse.com/~/media/images/products/fuses/passenger-car-and-commercial-vehicle/cartridge-fuses/littelfuse_cartridge_jcase.jpg

with 2 spade connectors. The fuses are quite small, encased in plastic and available from any store that carries auto parts since they're commonly used in GM vehicles.
```

---
## \#15 Posted by: Ingvarjedi Posted at: 2018-03-01T23:13:24.601Z Reads: 214

```
If the fuse explodes, how can I lose VESC? When the fuse blows, the current flowing from the battery to the VESC is cut off.
```

---
## \#16 Posted by: ZackoryCramer Posted at: 2018-03-01T23:36:49.591Z Reads: 209

```
I think he means that the vesc will blow before the fuse blows since it shouldn't suck in so much amperage.
```

---
## \#17 Posted by: cosmicc89 Posted at: 2018-03-01T23:37:10.460Z Reads: 208

```
It was mentioned above that this would only happen if you were going downhill. I'm pretty sure you're only generating enough current to do anything if you're actively braking, which you couldn't do because the VESC would be off, so I don't see how the VESC would be destroyed anyway, but I also have no evidence to the contrary.

Either way, the fuse is there to stop short circuits that would otherwise cause a fire. Generally speaking you should use a fuse that is the same amperage or a bit higher than what you intend to put your motor maximum at.
```

---
## \#18 Posted by: Pedrodemio Posted at: 2018-03-01T23:43:30.435Z Reads: 202

```
The thing is, the fuse of sized correctly will never blow during extreme operation, be it an abnormal brake current or whatever 

A 60A fuse does not blow when you reach 60,1A or 70A or 100A, each current will make it blow earlier, but never immediate, if I’m not mistaken there is an standard about how the fuses should blow, maybe not every cheap fuse follow, perhaps some one with E.E. can chime in

The scenario that a fuse does protect is if there is a short on the main power circuit that can actually reache a very high current, the rest it does nothing, you charging wiring will probably melt first than a 30A fuse, the balances wires even less, the fets inside the controller the same
```

---
## \#19 Posted by: laurnts Posted at: 2018-03-02T04:40:29.596Z Reads: 192

```
Ok this discussion I have to say is rather absurd. Fuse is fuse and fuse made to protect. It works and its implemented everywhere in our lives. The fuse main job here is to prevent shorts and flame in batteries. Vesc broke, thats no problem. Board goes on flame, thats hell expensive roasted brick. Btw, have you ever tested how much amp does regen brake does? The energy saved is not alot, maybe around 5% equivalent usage. Unless you spin ur motor like a generator, how much amp really does a 4000 rpm does? You're breaking btw, so it gets less and less during the breaking period. I couldn't imagine someone burning down their fuse due to braking 😀. I think 30A - 50A fuse is more than sufficient. If your board constant draw is 60A per second, mate you got something wrong.

Note: motor amp is measured in burst mode and vesc can handle 100A - 150A constant with decent cooling (according to vedder). Check ur vesc log and ride the board, then tell me how much the amp draw really is. I have to say 30A burst with 1-3A constant 80% of the time.
```

---
## \#20 Posted by: Deckoz Posted at: 2018-03-02T04:45:53.382Z Reads: 192

```
[quote="cosmicc89, post:14, topic:47766"]
60A JCase fuse:
[/quote]

You know that shit is rated for 12v right?.... Ie 720w
```

---
## \#21 Posted by: chuttney1 Posted at: 2018-03-02T04:54:25.065Z Reads: 182

```
Actually according to Littelfuse's Specs. For that particular fuse, it's rated for a max of 32V

https://www.mouser.com/ds/2/240/Littelfuse_JCASE_Datasheet-523198.pdf
```

---
## \#22 Posted by: chuttney1 Posted at: 2018-03-02T04:55:50.260Z Reads: 176

```
Just use the smallest 40 amp fuse rated for ~60V and you are fine.
```

---
## \#23 Posted by: laurnts Posted at: 2018-03-02T05:02:47.190Z Reads: 177

```
Technically fuse is made to blow based on amps and not voltage. It's more the current or even more accurate, the wattage that blows off the fuse. Off course those specification on 12v is meant for precise 12v 30A = 360 watt. Say you run 36v, it will blow when you do 10A draw as they are equivalent of 360 watt.
```

---
## \#24 Posted by: PXSS Posted at: 2018-03-02T05:23:55.015Z Reads: 184

```
This is wrong. ^^^
Fuses blow at a current in x amount of time. It has nothing to do with the wattage going through it. They are essentially a resistor with a low melting point. So when a high current goes through, it generates heat (I^2*R) and the fuse melts, opening the circuit. 

For example, the little fuses posted above,
![image|281x499](upload://66XxteWGjMwxV5UVNs2yfeAvogU.png)
A 20A fuse will blow in 10secs at ~45A or in 1sec at ~88A. 

The voltage rating determines the ability of the fuse to suppress the internal arcing that occurs after a fuse link melts and an arc is produced. If a fuse is used with a voltage rating lower than the circuit voltage, arc suppression will be impaired and, under some overcurrent conditions, the fuse may not clear the overcurrent safely.
```

---
## \#25 Posted by: Nordle Posted at: 2018-03-02T07:26:37.177Z Reads: 170

```
Most fuses voltage is overrated however 36v car fuses should be fine up to 12s

@pxss just make sure people get that the big "S" stands for "seconds" here, not "series cells" :)
```

---
## \#26 Posted by: michaelcpg Posted at: 2018-03-02T07:54:31.640Z Reads: 164

```
I really hope you don't give this as advice to people...
```

---
## \#27 Posted by: Acidfie Posted at: 2018-03-02T09:02:20.309Z Reads: 160

```
well, this is personal experience, many people just make a rough guess about the fuse, this can lead to serious injuries at high speeds.
```

---
## \#28 Posted by: michaelcpg Posted at: 2018-03-02T09:16:46.381Z Reads: 158

```
Those are two separate issues. Making a rough guess obviously isn't good either but saying that not having a fuse all together is just spreading bad information. 

A properly specced fuse won't blow under any normal operating conditions but could potentially stop someone's entire board from going up in flames, or worse, their entire house, particularly when battery fires are much harder to put out than most house fires or normal electrical fires.
```

---
## \#29 Posted by: Acidfie Posted at: 2018-03-02T09:22:28.867Z Reads: 156

```
true that, that is what a fuse is for.

but i see a lot of people taking "some" fuse - even asking about microfuses in some cases.

you should always know the short circuit current of your batteries, then you can search for a fuse.

not like, uuh my VESC has 50A * and my other one has 50A so this would be 100 but it is too big for me so i take 70A

i do not encourage people to not make their boards safer
```

---
## \#30 Posted by: krloz Posted at: 2018-03-02T09:46:07.627Z Reads: 154

```
I have the feeling people could have a look at what hag already been posted, explained, linked.  I see people asking and explaining over and over again the same stuff
```

---
## \#31 Posted by: PXSS Posted at: 2018-03-02T10:01:35.956Z Reads: 163

```
[quote="Acidfie, post:29, topic:47766"]
not like, uuh my VESC has 50A * and my other one has 50A so this would be 100 but it is too big for me so i take 70A
[/quote]
I'll humor you, and take this scenario. 
Lets say joe has a 10S4P battery pack that can do 60A, driving dual ESCs. Yes, the ESCs are capable of 100A but the battery isn't. So joe goes to radioshack and buys a fuse with a current rating of 60A. He then proceeds to forget to set his max current setting on the ESC to 30A each and instead puts it at 60 each. 

While not having a fuse could have very damaging effects on his battery and overall build if said batteries were to go into thermal runaway. Having a fuse could save his build. 

Based on the chart below...:
![image|281x499](upload://66XxteWGjMwxV5UVNs2yfeAvogU.png)
A 60A fuse can handle 80A for 1000secs and 100A for 80secs. 

So joe's fuse blew and he now has a chance to review his settings and catch his mistake for a whole $5 instead of spending $500+ on a new battery and escs. That is, if his whole setup didn't burn. 

Using a fuse even an underrated (60A) one isn't something that is going to make shit catch on fire. If a fuse goes, it means your battery was being damaged anyway as there are very few of us that have anything higher than 10S4P 30Q packs or Lipos capable of 60+A continuous. 

100A fuses for most, if not all of us is plenty and there is no good reason to not use one other than laziness.
```

---
## \#32 Posted by: scrapheap Posted at: 2018-03-02T12:40:16.361Z Reads: 142

```
I have the low profile ones, 60A 58V rating. Pretty compact.

[https://www.amazon.com/Profile-J-Case-Yellow-Cartridge-Littelfuse/dp/B00MEJ5UB4/ref=sr_1_fkmr2_3?s=industrial&ie=UTF8&qid=1501904015&sr=1-3-fkmr2&keywords=jcase+58v+60a](https://www.amazon.com/Profile-J-Case-Yellow-Cartridge-Littelfuse/dp/B00MEJ5UB4/ref=sr_1_fkmr2_3?s=industrial&ie=UTF8&qid=1501904015&sr=1-3-fkmr2&keywords=jcase+58v+60a)
```

---
## \#33 Posted by: Hatman30 Posted at: 2018-03-11T02:51:19.563Z Reads: 143

```
Just came across this whilst researching on the web. Very interesting.

Fuse ratings

    Continuous rating 
Fuse are marked with the current that they will continuously pass (at a standard temperature) without blowing, known as the continuous rating. It is good practice not to allow the continuous current to exceed 75% of the fuse's rated value to accommodate momentary current surges that might cause the fuse to fatigue over time or blow unnecessarily (nuisance blow).

    Blow rating

In simplified terms this is the current rating at which the fuse will blow. Most fuses have a blow rating around twice that of the marked continuous rating. So a 5A continuously rated fuse will have a blow rating of 10A.
```

---
## \#34 Posted by: edgar.s Posted at: 2019-01-27T01:23:29.077Z Reads: 93

```
Has anyone tried a fuse of this type?

https://www.ebay.com/itm/DC12V-42V-Sicherungsautomat-Manual-Reset-Stereo-Audio-Circuit-Breaker-70A/132901829830?hash=item1ef190fcc6:g:VCYAAOSwdgxcJhW4:rk:1:pf:1&frcectupt=true

I just have antispark xt90-s in my build 
I would like to protect my build more
i have dual vesc and lipo in serie 10s 20c 5000mah
```

---
## \#35 Posted by: b264 Posted at: 2019-01-27T01:30:15.537Z Reads: 91

```
That's not a fuse, it's a circuit-breaker
```

---
## \#36 Posted by: edgar.s Posted at: 2019-01-27T01:44:39.992Z Reads: 91

```
the function is not the same ?
```

---
## \#37 Posted by: Winfly Posted at: 2019-01-27T05:10:24.767Z Reads: 89

```
Yes they do the same thing and can be easily switch back on. But the form factor is too big to up in a board. It's big and tall.
```

---
## \#38 Posted by: edgar.s Posted at: 2019-01-27T11:04:35.302Z Reads: 81

```
hmmm what do you recommend? maxi blade fuse is for 24v, and my 42v batteries is a problem?
```

---
## \#39 Posted by: deucesdown Posted at: 2019-01-27T15:17:33.713Z Reads: 73

```
https://m.littelfuse.com/products/fuses/automotive-passenger-car/high-current-fuses/bf1-58v.aspx

Try to use the proper voltage and current rating. You don't want to go through the trouble of installing the fuse only to have it not function.
```

---
