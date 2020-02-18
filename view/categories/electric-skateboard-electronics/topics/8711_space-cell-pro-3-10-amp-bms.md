# Space Cell Pro 3 - 10 amp BMS?

### Replies: 38 Views: 3072

## \#1 Posted by: themegak Posted at: 2016-08-31T16:46:50.843Z Reads: 252

```
I have a space cell pro 3 (10S3P).  I opened it up to reorganize the components to maximize my wheelbase for dual vescs and peripherals.  Once i opened it up I noticed that the BMS was pretty small.  Upon further investigation i noticed that the BMS label says "36V" on one line and "10a" on the next line.  There is a bunch of Asian text inbetween and I haven't had any luck finding this BMS online to see what the details are.  Lastly I also noticed that the negative discharge cable from the battery pack is going directly to the power switch (anti spark?) board, which is connected to the bms and out to my xt60 discharge cable which came with a 40amp inline fuse.  I'm a little confused as the other teardowns of the Space cell I've seen on this forum all have bigger BMS's, I'm not sure what to make of my findings.  Do the pictures indicate that the BMS is being bypassed for discharging ?  Did Enertion use a 10amp BMS on my Space Cell strictly for charging and balancing the cells only ?  If anyone can share some insight on what is going on here I would appreciate it. 

BMS :
<img src="/uploads/db1493/original/2X/2/2b075736b1a00dd7ca855e4a60a1a747a8d97920.JPG" width="690" height="450">

Discharge Cables and Power Switch Board
<img src="/uploads/db1493/original/2X/d/d7a852b51bdf427266746ec210e925a30ffbbf0a.JPG" width="690" height="400">
```

---
## \#2 Posted by: barajabali Posted at: 2016-08-31T16:49:23.222Z Reads: 238

```
the BMS has to be bypassed. I cant tell by the pictures provided but that is the only way a 10 amp bms will work.  its only used for charging.  (brings cost down)
```

---
## \#3 Posted by: themegak Posted at: 2016-08-31T16:58:08.979Z Reads: 236

```
That's what i was thinking too but have only seen talk about a 30amp and 50amp BMS when it concerns the Space Cell.  I also saw the posts where @evoheyax actual bypassed the BMS on discharge on his Space Cell and I think Enertion was not fond of the idea.
```

---
## \#4 Posted by: t1m0007 Posted at: 2016-08-31T17:01:36.753Z Reads: 232

```
interesting. wonder what @onloop has to say on this. I'll check mine when I get home. Aside from balancing, isn't the low voltage cutoff another reason we'd want the BMS wired for discharge?
```

---
## \#5 Posted by: barajabali Posted at: 2016-08-31T17:08:02.751Z Reads: 225

```
Yes if you want to take advantage of low voltage protection you would need to go thru the BMS. 

Hmmm that being said I wonder if this space cell will allow you over discharge and ruin it.
```

---
## \#6 Posted by: t1m0007 Posted at: 2016-08-31T17:20:11.461Z Reads: 217

```
yeah this is definitely a curiousity of mine as well.

Now of course, I'm using a VESC and I have low-voltage protection in there as well but coming from an engineering background it's hardwired in my brain that more at least 2 fail-safes are a good measure of quality. I'm a little concerned at the prospect of this corner being cut, especially after a much higher AMP BMS was advertised on this forum in batches previous. Not jumping to conclusions yet-- I haven't looked at mine yet. But mine is from this latest batch. so it would not surprise me if I find the same thing. the BMS was definitely smaller than i anticipated
```

---
## \#7 Posted by: Hillso Posted at: 2016-08-31T17:23:31.711Z Reads: 206

```
There is an improvised way to do specific cell low voltage cutoff while bypassing the BMS, you use an arduino to check if the BMS has done cutoff, and use the arduino to do the cutoff, for example you connect the receiver to the VESC thru the arduino, and than the arduino can send 50% PWM when he detecs cutoff from BMS
```

---
## \#8 Posted by: themegak Posted at: 2016-08-31T17:52:45.135Z Reads: 199

```
I'm curious on what you find.  If we are bypassing the BMS for discharge then why only a 40 amp fuse ?  The pack should be able to do 60 amps and I think we could conservatively discharge 50 amps and get more power to our motors.   I would just like some clarity so that i know for sure what is going on and what the intention was/is.
```

---
## \#9 Posted by: Jinra Posted at: 2016-08-31T17:56:27.925Z Reads: 204

```
Semi related

http://www.electric-skateboard.builders/t/honey-driver-honey-velocity-v3-deck-caliber-iis-83mm-evolve-gt-wheels-dual-om5065-200kv-space-cell-pro4-diy-pulleys-enertion-pulley-bones-super-reds-enertion-mounts-winning-remote-chaka-vescs-build-complete/5760/77?u=jinra

I spoke with enertion support and they said the bms handles up to 80a discharge current, though i suspect that it's really just bypassing the bms.
```

---
## \#10 Posted by: t1m0007 Posted at: 2016-08-31T18:22:46.983Z Reads: 194

```
yeah I'd say that's probably marketing speak. If @themegak popped open the case and there's a BMS with 10a written on it Plus TWO positive leads from the battery then that could be the smoking gun. I' used google translate to analyze the photo. The 2 characters in front of 10A say "Charge" and the partial unobstructed characters after 36v say "Lithium Ion"
```

---
## \#11 Posted by: themegak Posted at: 2016-08-31T18:32:00.396Z Reads: 189

```
Are you able to physically see what kind of BMS you have in your Space Cell Pro 4
```

---
## \#12 Posted by: Jinra Posted at: 2016-08-31T18:32:30.953Z Reads: 188

```
Pretty sure it's the same as SCP3
```

---
## \#13 Posted by: themegak Posted at: 2016-08-31T18:39:37.748Z Reads: 184

```
I have a Space Cell Pro 3.  If your BMS is like mine then you too would have a 10 amp BMS.  You may want to take a look.  Up to you, but it is always good to know what you are working with.
```

---
## \#14 Posted by: Jinra Posted at: 2016-08-31T18:42:05.256Z Reads: 182

```
I took a look and it's physically the same, but I didn't read too much into it. I can pretty much guarantee yours and mine are not 10A discharge BMS's. As @t1m0007 pointed out it's probably 10A max charge current. Enertion claimed it's 80A discharge, though I'm a bit skeptical on that.
```

---
## \#15 Posted by: mccloed Posted at: 2016-08-31T18:43:54.724Z Reads: 173

```
Looking at the two pictures, I believe the BMS is for charging only. No amp limit on discharge. Correct me if I'm wrong but, the main negative lead should be going into the BMS and going out of the BMS for amp limiting.
```

---
## \#16 Posted by: themegak Posted at: 2016-08-31T18:50:29.801Z Reads: 170

```
It's just hard to believe a BMS that small can output that many amps.  I am skeptical that we are discharging via the BMS.  Then again I am no BMS expert.
```

---
## \#17 Posted by: themegak Posted at: 2016-08-31T18:53:45.876Z Reads: 173

```
Sorry but can you take a picture of yours as I want to be sure we have the same BMS so that i can assume i can change my fuse holder and fuse and bump my Batt Max up to 50 amps safely across two vescs (25 amps for each vesc).  I would appreciate this greatly.
```

---
## \#18 Posted by: Jinra Posted at: 2016-08-31T18:54:36.201Z Reads: 172

```
Yea, I think it's just bypassing the BMS for discharge and they said 80A to me because thats the output rating of 4 parallel cells. Either way I would replace the fuse holder or remove it altogether as 40A is a bit small for this pack.
```

---
## \#19 Posted by: longhairedboy Posted at: 2016-08-31T18:55:53.314Z Reads: 176

```
most BMSs interrupt the negative lead. That's to say all the ones i've ever seen or used did. this is interesting. I don't think i've seen any like this yet, they must be lasting longer. 

I also noticed that the VESCs you get from Enertion are now coming automatically set to a 42 volt limit and though i didn't pay enough attention to remember, i'm willing to bet that the cutoff is also 10S friendly. So the VESCs are actually protecting the pack from over discharge now? Seems odd to me. 

in a complete this would work fine. I'm not sure how long it would last in a DIY build though. HMMMMMM.
```

---
## \#20 Posted by: Jinra Posted at: 2016-08-31T18:58:40.189Z Reads: 174

```
VESCs voltage cut offs tend to be higher than BMS's anyway. Supower has a 2.9v over discharge cut off by default. I don't see a problem with using the VESC for that. However, if you mean over current, I think the Space Cell is bypassing BMS discharge and relying on the 40A fuse to not bust your components in case of battery mutiny.
```

---
## \#21 Posted by: longhairedboy Posted at: 2016-08-31T19:05:22.611Z Reads: 166

```
ahhh. That makes much more sense now.
```

---
## \#22 Posted by: themegak Posted at: 2016-08-31T20:44:06.500Z Reads: 161

```
I found [this](http://www.aliexpress.com/item/Free-Shipping-36V-10ah-battery-BMS-3-7V-18650-li-ion-cell-10S-BMS-PCB-PCM/32283661813.html) on AliExpress.com.  It isn't the exact same "BMS" i have but it is pretty close.  It says it has "Over-Current Discharging Protection:50A (Max.)" .  I guess this is a 50amp BMS after all.  I think i am still going to bypass it as i don't trust it to do anything but balance the cells and I could use those extra amps i would gain.  Thanks everyone for the help, thoughts and conversation.  Kudos.
```

---
## \#23 Posted by: Jinra Posted at: 2016-08-31T20:46:09.785Z Reads: 159

```
I'd like to reiterate that I think the Space cell Pros bypass the BMS by default. The BMS you linked will not handle 50A continuous and is meant for burst output.

Here's a response from @EnertionSupport

<img src="/uploads/db1493/original/2X/7/77fe0e39e4ecbfca81328ff969762a0ffc9fef3f.png" width="690" height="198">
```

---
## \#24 Posted by: themegak Posted at: 2016-08-31T21:12:25.804Z Reads: 157

```
I hear you and i wouldn't trust the BMS for any kind of discharge protection as I stated above, but there is evidence (if you look at the wiring diagram in the link, it is exactly how my/your BMS is wired) that there is some kind of protection again over-current discharging and being that neither of us are BMS experts, i wouldn't totally discount that evidence.  Take a look at @evoheyax thread about bypassing the BMS if you are interested in bypassing it, he has detailed the process pretty well.   Lastly, your battery and mine are different Space Cell 4 vs Space Cell 3, you have more batteries in parallel (probably different BMS too) so you can achieve a 80a continuous discharge "safely" while i can only hope to achieve 60a best case "safely".   Don't always trust the guy manning the support emails.  I'm not saying he is wrong but he could be and if he is, you would be the one out $ 400.  Thanks for the insights, appreciate it.
```

---
## \#25 Posted by: Jinra Posted at: 2016-08-31T21:34:52.602Z Reads: 148

```
yea i know how to bypass a bms. I've helped a bunch of users on here with bms wiring including evoheyax. I said i was skeptical of enertion support and was merely showing you what they said to me. I could take a look at my bms again but I'm pretty comfortable with my assumption that it's bypassed.
```

---
## \#26 Posted by: themegak Posted at: 2016-08-31T21:43:47.072Z Reads: 148

```
No worries, i hope you didn't take what i said personally.  I'm just basing my views on the facts that i've uncovered so we don't need to assume.  Historically the Spacecell has come with a 30 amp and 50 amp BMS.  That is why my BMS was so surprising. I do see that there is some kind of 50 amp protection, but i don't speak Ali Express english so i can't verify that for sure, but wouldn't discount that completely either.  Your battery pack is more than likely not bypassing the BMS by default, Jason has historically not been fond of that idea according to this forum and according to the wiring diagram that shows that.  Just don't want you to hurt your battery as i know how expensive it is.  Either way i sincerely appreciate your thoughts and input and are very kind.
```

---
## \#27 Posted by: makevoid Posted at: 2016-08-31T21:54:36.618Z Reads: 138

```
Using a bms for always balancing the cells (to get balanced discharging) should help maintaining the life of the cells long and 40USD (for a [url=http://www.ebay.com/itm/36V-37V-42V-10S-60A-Lithium-ion-Li-ion-Li-Po-LiPo-Polymer-Battery-BMS-PCB-System-/221769582503?hash=item33a27f47a7:g:VV0AAOxywCJRa-m2]60A BMS[/url]) isn't a big expense If you have the charge-only one. Maybe you can think of upgrading it later when the warranty expires if you didn't put many cycles through the battery yet.
```

---
## \#28 Posted by: themegak Posted at: 2016-08-31T22:03:32.398Z Reads: 137

```
that sounds like a good plan.  Are there any you recommend or suggest in particular ?
```

---
## \#29 Posted by: makevoid Posted at: 2016-08-31T22:14:10.987Z Reads: 142

```
I use that specific one on 8S, I never tried other BMSes, on 8S I am not plugging in the last two balance leads, it seems to do the job up until now, it took 3 weeks to arrive and I paid 5$ shipment to the UK. I tested the short-circuit protection (by mistake) and it seems to work as well (tried to charge for a second with reverse polarity lol). I have set 50A as battery max on the VESC and I have an 8S5P configuration. The bms fits [url=http://www.electric-skateboard.builders/uploads/db1493/original/2X/7/7717b441cb2bb06835777cec3eb3c6edb8a7dd3a.jpg]horizontally[/url] in the space cell enclosure.
```

---
## \#30 Posted by: onloop Posted at: 2016-08-31T22:47:32.795Z Reads: 144

```
The space cell battery don't use a BMS to control discharge.

The two mechanism to prevent overy discharge are the fuse and the settings in the vesc which control current draw.

Inside the space cell is a charge / balance circuit and a mosfet switch for turning the circuit off.

Technically speaking the space cell pro 4 can output peaks of 80a and there won't be a problem..

However i always suggest a fuse.
```

---
## \#31 Posted by: racidon Posted at: 2016-08-31T22:57:22.725Z Reads: 142

```
[quote="themegak, post:8, topic:8711, full:true"]
I'm curious on what you find.  If we are bypassing the BMS for discharge then why only a 40 amp fuse ?  The pack should be able to do 60 amps and I think we could conservatively discharge 50 amps and get more power to our motors.   I would just like some clarity so that i know for sure what is going on and what the intention was/is.
[/quote]

This could be because that style of inline fuse holder fuses are quite common in 40 and below amperage for the use of Vehicle fuses. However when you start looking at 50+amp in a vehicle they tend to use the square fuses which are much more expensive and also bulkier.
```

---
## \#32 Posted by: themegak Posted at: 2016-08-31T23:04:50.610Z Reads: 137

```
can u send me a link to where u purchased or point me in the right direction.  just want to read up on it.
```

---
## \#33 Posted by: themegak Posted at: 2016-08-31T23:13:44.780Z Reads: 134

```
got it.  that's great news.  is this something fairly new ?  I was confused by the other posts on the forum especially the one where someone bypassed the BMS.  Theoretically I could get a 60amp inline fuse and rock my batt max at 50 amps if I wanted to right?
```

---
## \#34 Posted by: Jinra Posted at: 2016-08-31T23:16:08.603Z Reads: 132

```
yes, you can. you will need a new fuse holder though
```

---
## \#35 Posted by: onloop Posted at: 2016-08-31T23:17:46.042Z Reads: 134

```
We are always innovating and being reiterative with our products.

After months of testing with vesc we realise that it can control current better than most BMS. Plus with a fuse you can protect your cells easily.

Also due to the rise of popularity of hub motors we needed a solution that can allow people to draw more current from battery if needed.

Until there are specific custom made BMS for esk8 no BMS is better.
```

---
## \#36 Posted by: makevoid Posted at: 2016-09-01T05:23:16.574Z Reads: 127

```
There's an ebay link in my post above and [url=http://www.batterysupports.com/36v-37v-42v-10s-60a-10x-36v-lithium-ion-lipolymer-battery-bms-p-267.html]this[/url] is from their site (supower).
```

---
## \#37 Posted by: evoheyax Posted at: 2016-09-02T00:52:44.555Z Reads: 116

```
[quote="onloop, post:35, topic:8711"]
Until there are specific custom made BMS for esk8 no BMS is better.
[/quote]

I feel the same way. I wish there was an easier way to balance cells than a bms, like something you plug into the balance connector (and leave permanently, like a bms) that it shifts volts around to cells until they are all the same.
```

---
## \#38 Posted by: longhairedboy Posted at: 2016-09-02T13:15:23.059Z Reads: 108

```
[quote="onloop, post:30, topic:8711"]
The space cell battery don't use a BMS to control discharge.
[/quote]

Well there you have it. I was wondering WTF was going on inside these raptor cells as well, the last few i cracked open sure had a lot of space left over. 

This is at least the third iteration i've seen of the regular raptor packs.
```

---
