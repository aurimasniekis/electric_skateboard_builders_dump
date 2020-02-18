# Guide to choosing a fuse?

### Replies: 43 Views: 1014

## \#1 Posted by: beherit Posted at: 2019-02-12T18:07:59.039Z Reads: 245

```
I'm almost done my personal build, but I've noticed one part that goes fairly undocumented in most builds despite being almost vital: The fuse. I've seen suggestions to use a 60V 10A fuse, 60A fuse, fuse on the negative charge wire, fuse on the positive battery wire, and everything inbetween. Could any experienced builders explain why they chose the fuses they did on their builds, where they placed them, and why?
```

---
## \#2 Posted by: venom121212 Posted at: 2019-02-12T18:41:59.028Z Reads: 241

```
There are 2 main commonly talked about fuse locations:

1) fuse between esc and battery. 

2) fuse between the board's charge port and battery.

Fuse 1 is to protect your speed controller from pulling too much power (whether or not the controller can actually handle it) from the battery in a tough situation (steep incline from low speed). Some people here, myself included, prefer to run unfused because I know that the speed controller can handle a higher amp spike for a few seconds and don't want the fuse to blow and throw me on my face. Others really want the protection of blowing a fuse, not a controller.

Fuse 2 is a requirement. If protects your battery from something bad happening with the charger or charge port. If the charger starts freaking out for whatever reason and doesn't stop sending current to your batteries, it will start a fire. The fuse in this case will blow, saving your battery/house/family/life.

In each case the fuse should be rated dependent on the system. Fuse 1 rating depends on battery/bms setup and esc. Fuse 2 rating should be a bit higher than your chargers charging Amps.
```

---
## \#3 Posted by: Creavenger Posted at: 2019-05-06T10:39:24.033Z Reads: 187

```
@venom121212 I have a charge/discharge bms so does a fuse between the battery and esc still matter?
```

---
## \#4 Posted by: Andy87 Posted at: 2019-05-06T11:35:52.907Z Reads: 181

```
@Creavenger you don’t need a fuse between the battery and the vesc, but a 8-10a fuse on the negative of the charge port is never bad.
```

---
## \#5 Posted by: Rustedbucket Posted at: 2019-05-06T11:46:46.278Z Reads: 179

```
yes it is still better safe than sorry.
```

---
## \#6 Posted by: venom121212 Posted at: 2019-05-06T12:41:12.387Z Reads: 176

```
I agree with both of the above answers. You don't need one as the bms should do its job and cut off current in overload situations. Fuses are also dirt cheap and offer more protection.

Then again.. I run unfused (except negative side charge port) with a charge only bms and rely on my unity vesc to be able to shut and and take it. No issues so far.
```

---
## \#7 Posted by: MD84 Posted at: 2019-05-06T12:57:41.473Z Reads: 171

```
My reasoning and specification for fuse #1 would not be an overload situation but a short circuit or thermal runaway. Protecting a battery from faulting into a short circuit. 

#2 fuse, why place on negative lead? Edit to add, I don't think fuse 2 will protect from a charger malfunction in all cases. The charger could pass 4A and overcharge the batteries all day. Again I see it as a short circuit protection on accidental short at the charge port or also an overload in the smaller charge wires.
```

---
## \#8 Posted by: venom121212 Posted at: 2019-05-06T13:46:59.044Z Reads: 166

```
If fuse #1 lies between the battery and the vesc, how would a blown fuse protect any more than a blown BMS in a short circuit scenario? If your battery shorts itself, you're in trouble already.

Current is flowing from battery to BMS (set to cut off at over current) to Fuse #1 to VESC to motors.

Nothing is back flowing to the battery in this case except regenerative braking which we aren't talking about. 

This is where fuse #2 comes in. It won't protect against all malfunctions. His job is to make sure that if your charger flips its shit and starts outputting 30A somehow, your battery doesn't get charged at the incorrect rate. It blows the fuse and your board is no longer charging. Your BMS can also F up and start charging cells at the wrong rate. Nothing is perfect, just aim for the safest you can.

Negative side charge port is @b264's recommendation that I just regurgitate from time to time.

What part of Ohio are you out of?
```

---
## \#9 Posted by: MD84 Posted at: 2019-05-06T15:43:04.851Z Reads: 152

```
I'm northeast Ohio east of Akron. Are you around here?

I'm saying I'm not worried about protecting my esc. I'm sizing my fuse based on a shorted fet, melted connector at the esc, etc. Something that would cause the batteries to dump current into a short circuit resulting in venting batteries and flaming balls of plasma. I would spec this fuse well over the overload range of the esc. I would spec it somewhere below my batteries short circuit current ability but we'll above my esc current capability Like 200A time delay.  

Just because a bms or esc is set to cutoff at certain current levels, does not mean that during a fault or component failure it will reliably do so.

I still see #2 as protection from shorting your charge jack. Is it known in our community for a charger to fail in such a way as to over current to the battery? I think it is more common that the jack gets shorted. 

I think it is important to understand what faults or equipment we are planning on protecting before we prescribe a fuse. This comes down to user preference and best practice. I agree, no reason not to fuse charge port at slightly above charge current. Fuse 1 we must decide what we are protecting against. Is it equipment overload or short circuit. 

I like a fuse on pos and on neg, this way if your battery is in a good mood you protect the happy and loving electrons, or if it is angry you protect the little deviant bastard electrons. Conventionally speaking anyways...
```

---
## \#10 Posted by: venom121212 Posted at: 2019-05-06T15:55:52.072Z Reads: 139

```
Cinci area so direct opposite :confused: 

Ok we can agree on many things here. I am using the fuse rating of the wire to attempt to accomplish the same task. I am running case #1 without a traditional fuse to allow equipment overload momentarily but still able to hopefully prevent a short from occurring. I personally like to have a fuse built in to the battery positive charge circuit as well for extra protection but not all battery makers are implementing this.
```

---
## \#11 Posted by: MD84 Posted at: 2019-05-06T16:08:08.167Z Reads: 129

```
I have hesitation about using wire as fuse such as in the cell level fusing. What gauge wire are you using? And what would be the expected melting current. Maybe I could try a real world test.

I am having a little fun with the pos vs neg side fuse, I would be content with one. 

I actually put my loop key in the middle of my battery, so it is like two 5s packs series'd together by loop key. I was thinking of using a fuse there. I am trying to think if there would be any benefit there if there was an internal battery short.
```

---
## \#12 Posted by: venom121212 Posted at: 2019-05-06T16:23:02.771Z Reads: 128

```
10 gauge but very high quality wire. Silicone wrapped so it doesn't melt even when a soldering iron touches it. Inside stand count is in the thousands. Loopkey in the middle is an interesting concept. I need to think about that one for a minute. So when you plug it in, you have the end opposite the loop double paralleled out to your packs? Assuming yes for a moment, would that really do any difference to in rush current? 18650 packs of multiple p groups are doing this on a smaller scale to the bms but with a board between. I'm approaching the limits of my knowledge and re-entering the learning field.

Hyper drive, engaged
```

---
## \#13 Posted by: Fatglottis Posted at: 2019-05-06T17:07:27.243Z Reads: 121

```
Fuses help to protect stuff when you decide to connect your battery with opposite polarity... @Creavenger :wink:

Within my 7 years of working with the high voltage system in electric cars, I have seen countless of times where a fuse is a good thing when working with prototype parts. I take all that knowledge with me home. 

For me the loop key is the fuse and it is placed in the middle of the pack (It just felt better having the pack divided in two when not used). I pretty much agree on everything @MD84 has said :)
```

---
## \#14 Posted by: Creavenger Posted at: 2019-05-06T17:39:11.030Z Reads: 119

```
Guess im installing 2 fuses 🤔 🤣
```

---
## \#15 Posted by: sharky Posted at: 2019-05-06T17:47:19.653Z Reads: 118

```
so when i want to use a charger for my upcomming 12s5p pack with 4amps and 50.4V
would be a 5a or 6a fuse like those are ok or do i need to take smthg else?
![grafik|690x381](upload://xWj85jzdJtOqyg1Q7c9nS3vDX0q.jpeg)
```

---
## \#16 Posted by: MD84 Posted at: 2019-05-06T17:59:42.870Z Reads: 117

```
If you look at the silver end caps of those fuses you should see the voltage rating. I'm guessing those are not rated for 50v. One thing to consider is that even though the fuse element may melt, this will draw an arc. The fuse needs to be able to quench that arc. Many fuses employ a spring or otherwise mechanical means of separating the electrodes sufficiently to create an air gap for the voltage if the system. Some fuses are filled with sand for example. If the fuse cannot extinguish the arc, it is possible arc could persist and lead to further faults and damage. 

Long story, size a fuse based on the nominal system voltage and desired current threshold. Also it is good to consider reactance and short circuit ratings. For example motor loads or capacitors exhibit reactance in which a large current initially flows for a very short time. In this case you would want a time delay fuse. The time vs current curves can be referenced for more details. For a constant linear load a fast blow fuse can be used. Available short circuit current is also a consideration. If the battery is able to deliver thousands of amps it is possible the fuse cannot break that amount of current and will fail allowing fault current to persist. 

These considerations are partly why I question using wires as fuses. If we have a silicon encasement around our melting conductor, how does the current break if the molten copper is contained?
```

---
## \#17 Posted by: sharky Posted at: 2019-05-06T18:03:13.441Z Reads: 113

```
yes youre right theyre not rated for 50v but there are some rated for 8a and 60v
what are other people using here? im talking about the chrging fuse
kr
```

---
## \#18 Posted by: MD84 Posted at: 2019-05-06T18:08:28.556Z Reads: 116

```
This should work

https://www.amazon.com/Baosity-Overload-Protector-Resettable-Waterproof/dp/B07H3V23J7 

![_AC_SY400_|446x400](upload://t7JrBAiYCxIFfeUMExeSMyoOZsQ.jpeg) 
![_AC_SY400_|365x400](upload://6nb49P2QRThriPcG0MFzft3jeol.jpeg)
```

---
## \#19 Posted by: sharky Posted at: 2019-05-06T18:15:32.585Z Reads: 113

```
thx very much man gonna build this into my new integrated deck
```

---
## \#20 Posted by: MD84 Posted at: 2019-05-06T19:13:09.507Z Reads: 113

```
For Science 

https://youtu.be/NKtK6IAEaMc
```

---
## \#21 Posted by: Creavenger Posted at: 2019-05-07T09:31:14.925Z Reads: 109

```
What fuses should i get? I have a bms with a continuous dischage current of 40A, the esc can handle 60A continuous and max 240 for a few seconds, I'm running a single motor setup so i was thinking about a 80A fuse between the battery and esc. And I was thinking about a 7.5A fuse for the charge port (on the negative wire?).
```

---
## \#22 Posted by: MD84 Posted at: 2019-05-07T11:31:22.812Z Reads: 104

```
Could you tell us from what faults you are trying to protect which equipment? Are you trying to protect your esc and or bms?

Do you know how much time your esc can handle 240A?

I don't see a problem with 7.5A fuse on charger port. Negative wire? Sure. I can only share my theory on why the negative wire is a popular choice. Perhaps @b264 can shed some light on a technical reason for fusing the negative wire on the charge port. 

To reiterate I think there is a decision about what our main protection strategy is:

1. Fuse nothing accept charge port and cross our fingers. Assure the ultimate chances of maintaining brakes in emergency situations. Esc bms and wiring are our fuse now and very possibly will catch on fire if there is an accidental short, reverse polarity, fault etc. 

2. Fuse based on protecting for only short circuit knowing the fuse should not blow even during demanding overloads. The bms and esc will not have any additional protection and very well could be destroyed and burn down during a fault. There is protection here should a fault turn into a short circuit such that the batteries should not deliver insane amounts of power into a fault which could lead to the batteries themselves burning down. There is still very much assurance that emergency braking functions will work and not be hindered by your fuse. 

3. Fuse is sized to protect equipment such as esc. If the esc, bms, Regen is overloaded, the fuse would open hopefully protecting this equipment. There is the possibility that during demanding situations the fuse would open and you would lose brakes and or acceleration.
```

---
## \#23 Posted by: Creavenger Posted at: 2019-05-07T12:09:23.690Z Reads: 101

```
Im mainly trying to protect my esc since I reversed the battery polarity and fried a focbox last week. But that was due to applying the connector to the battery in the wrong way. Now I just want to make sure the esc is protected from getting fried. I have 10s2p battery with a bestech charge and discharge bms and im not going to open up the battery any time soon. I think I just need to place a fuse between the battery and the esc. If the chance of loosing power is too high I'd rather avoid using a fuse however. I fried my esc due to my own error afterall so im not sure the probability to fry components while riding is without a fuse is high enough to outweigh a potential loss of power while going downhill. (my first build hasn't had any shorts or breakdowns in almost a year untill i shorted the esc by my own mistake. I ordered a esk8.de vesc, they mention "a few seconds of max 240A" on their website.

Thanks for your help so far! very interesting topic aswell! :slight_smile:
```

---
## \#24 Posted by: MD84 Posted at: 2019-05-07T14:01:17.709Z Reads: 98

```
Let me do a little more research but here is a quick starting point

https://www.digikey.com/product-detail/en/littelfuse-inc/142.5631.6102/F6794-ND/2515912 

![6101_sml|200x200](upload://1mfBLR6JKwFFjzMETR7mD6VGPLL.jpeg) 

https://www.littelfuse.com/~/media/automotive/datasheets/fuses/passenger-car-and-commercial-vehicle/bolt-down-fuses/littelfuse_bf1_58v_datasheet.pdf
```

---
## \#25 Posted by: MD84 Posted at: 2019-05-07T15:54:17.229Z Reads: 99

```
Could you tell me what type and configuration of batteries you are using. Also what size wire and approximate length from the battery to the fuse.
```

---
## \#26 Posted by: Creavenger Posted at: 2019-05-07T16:06:33.105Z Reads: 100

```
Samsung 30q cells, wire is turnigy 12awg battery to fuse would be between around 10cm
```

---
## \#27 Posted by: b264 Posted at: 2019-05-07T17:23:19.851Z Reads: 98

```
[quote="MD84, post:22, topic:84027"]
Perhaps @b264 can shed some light on a technical reason for fusing the negative wire on the charge port.
[/quote]

Yes, either side will work but I think it's slightly better to fuse the negative side for a few reasons.

First, it's easier.  BMS already all work with a common positive and the negative sides are all switched.  Making "all" positives just connect together, including the battery positive, is easy and leads to less wiring errors.

Second, if you fuse the negative wire, it gives you access to BAT+ for troubleshooting.  If you also use a loopkey with a bypassed BMS, that gives you access to BAT- for troubleshooting.

So, for example, if I need to check battery voltage or if I need to test an ESC using my board as a power source, it's easy:

![20190505_212656|230x129](upload://gXxvbBWZAcH43j40R04EDBKZtfP.jpeg) 

Plug these into the charge and loopkey ports and you can test an ESC on the bench or measure the battery or whatever.
```

---
## \#28 Posted by: MD84 Posted at: 2019-05-08T01:32:58.598Z Reads: 95

```
Based on a 30q internal impedance of 26 milliohms we can determine the available short circuit current of 3.6/0.026=138A. This is confirmed by the Samsung factory short circuit test of around 135A with a 10 milliohm load.

Series connected groups do not increase short circuit current. The connection resistance of each series connection would actually decrease the SCC but we will assume 0 ohms. 

Parallel groups would multiply the SCC for each P group. 

The wiring from the battery we will consider although in this case it will be somewhat negligible. Let's say 10 milliohm for your 12 awg wiring. 

Putting it another way to calculate SCC of the pack is:
36v nominal / (10S*0.026ohm/2P+0.01ohm) = 
 257A available Short Circuit Current

The fuse I linked above is rated to interrupt 1000A at 58V

That said, you originally suggested an 80A fuse. The Littlefuse BF1 series 80A fuse would be a good choice. The 100A would be fine as well. If you're concerned with more sensitive protection for your esc, I would pick the 80. If you are concerned with losing control of your board during demanding loading but still want some protection to your esc I would pick the 100A.

I will add this BF1 fuse with a 58V 1000A interrupting rating would be good for 30q packs up to 12S7P. Although I would add in some safety factor as a rule of thumb and say each 30q P group has 150A SCC. This would limit it to a 12S6P. 

I noticed Littlefuse has a MEGA 70V fuse with a interrupting rating of 2500A. This would be good for a 16S16P 30q. Very nice how much
```

---
## \#29 Posted by: Hannes Posted at: 2019-05-09T15:46:42.952Z Reads: 84

```
Is it ok if they are rated  for 230v ? 3,15a
```

---
## \#30 Posted by: MD84 Posted at: 2019-05-09T16:15:17.364Z Reads: 85

```
I need to know more about your setup to give an accurate answer. 

As long as DC voltage rating of fuse is greater then voltage if battery. Amperage rating depends on your protection strategy. 

230v rating sounds like an AC rating. DC is more difficult to extinguish arc because there is no zero voltage crossing like in AC. 

My gut would say a fuse rated for 230vac would be sufficient for 50vdc though. 

I don't know what you mean by 3,15A but it does not look promising. 

Tell me what your battery is and provide a link to the fuse and I will tell you if it is good.
```

---
## \#31 Posted by: Hannes Posted at: 2019-05-09T16:18:50.026Z Reads: 82

```
the fuse is for the charge wire, i got a 10s4p 30q, using a 2A charger.

The fuse is 230v, 3,15A [this is the fuse](https://www.biltema.se/bil---mc/elsystem/sakringar/glassakringar-5-st-2000016473)

They don't specify ac or dc, but i guess AC
```

---
## \#32 Posted by: MD84 Posted at: 2019-05-09T16:29:05.330Z Reads: 82

```
I would not recommend it unless it has a DC voltage rating. 

That said it is better than no fuse and will likely work for you. The 3,15A is good for a 2A charger. 

You could consider getting a fuse greater than 4A should you ever wish to use a faster charger. A 5A fuse would still be fine for a 2A charger in my opinion.
```

---
## \#34 Posted by: Mich21050 Posted at: 2019-05-09T17:02:45.810Z Reads: 80

```
I could send you an DC 3A fuse with your prints... :slight_smile:
```

---
## \#35 Posted by: Hannes Posted at: 2019-05-09T17:11:48.192Z Reads: 78

```
I'll PM u
10char
```

---
## \#36 Posted by: deucesdown Posted at: 2019-05-11T19:03:24.522Z Reads: 75

```
This is the way I've started doing it. The bananas allow bypassing the fuse if it blows.

https://www.thingiverse.com/thing:3623953
```

---
## \#37 Posted by: nirurin Posted at: 2019-05-12T22:38:23.528Z Reads: 72

```
Figured I'd ask this here, as @b264 seems to be the guru for anything battery related on here haha. 

So I'm likely to be getting a 2A charger, so what rating of fuse would be best to put on the negative line? I'm guessing either 5A or 7.5A? Only reason I'm considering 7.5A is in case I end up upgrading to a 5A charger in future, but if that means its not going to do me any good with the 2A charger I'm starting with then I'll just change fuses when the time comes. 

Actually will probably use a circuit breaker instead of a fuse, something like [this](https://www.ebay.co.uk/itm/5-Amp-Reset-Circuit-Breaker-Fuse-125-250v-AC-32v-DC-w-Rubber-Cap-Boot-Cover/254072351452?hash=item3b27e46adc:g:Gc0AAOSwzqBcsDex)

Also, I did consider putting a high-amperage fuse in between the vesc and the bms as another line of protection, but it seems people are saying it's not worth it as if it goes wrong or trips unexpectedly you can lose braking (which could be worse than damaging the board). This sound about right? I'd been considering something like a 100A fuse but no point if it's not doing anything helpful.
```

---
## \#38 Posted by: b264 Posted at: 2019-05-13T03:20:28.274Z Reads: 73

```
For 1A, 2A, or 4A charging I think this fuse (7.5A, 58V) works great and it's physically very small and easy to solder to.


https://www.mouser.com/ProductDetail/576-099707.5WXN

I JB Weld one to the inside of the enclosure and then solder to it.
```

---
## \#39 Posted by: briman05 Posted at: 2019-05-13T18:02:57.039Z Reads: 66

```
What do you solder to it.  I have bullet connectors on my plug and the females coming off the battery.  I feel like I could just put bullet connectors on each end and and on the other ends leave the wire bear to solder to the fuse then heat shrink everything.
```

---
## \#40 Posted by: b264 Posted at: 2019-05-13T18:50:44.451Z Reads: 64

```
[quote="briman05, post:39, topic:84027"]
What do you solder to it.
[/quote]

You can see one here

https://forum./t/the-blue-one-12s-lifepo4-170kv-6374-caliber-2-30-43-powell-peralta-focbox/75/1
```

---
## \#41 Posted by: briman05 Posted at: 2019-05-13T20:57:12.188Z Reads: 62

```
That isn't a barrel connector right?
```

---
## \#42 Posted by: b264 Posted at: 2019-05-13T21:53:45.508Z Reads: 61

```
Not on that board but I use these

https://smile.amazon.com/gp/product/B06XRT5C2Q/ref=ppx_yo_dt_b_asin_title_o04_s00?ie=UTF8&amp;psc=1

the same way on 10S li-ion boards

![20190411_214906%20(copy)|682x500](upload://u5HN1qq8vtJ8LpDer4sPvjAZf07.jpeg)
```

---
## \#43 Posted by: briman05 Posted at: 2019-05-13T23:46:29.291Z Reads: 59

```
Would it be bad to make them adapted to the bullet connectors and so I don’t have to cut the leads to the battery
```

---
## \#44 Posted by: Creavenger Posted at: 2019-05-25T13:16:25.752Z Reads: 48

```
![20190523_212748|375x500](upload://mb7TdyPtqubClM860E4Do3hFqyI.jpeg) ![20190523_212846|375x500](upload://506zXDL86ew33JUsQpHr6vdew9w.jpeg) 

Charge port is fused up 👌
```

---
