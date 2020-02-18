# BMS Group Buy: Who&rsquo;s in and for how many?

### Replies: 99 Views: 6624

## \#1 Posted by: longhairedboy Posted at: 2016-04-05T11:20:54.441Z Reads: 368

```
While i was getting my payment issue resolved with liion wholesale, i happened to ask them for their opinion on who has the best BMSs and they mentioned they get all of theirs directly from China. So i asked them about the possibiliy of a group buy and they said they would probably need 10-15 units ordered to make it happen but it might be possible and that lead time wouldn't be too bad, just a couple of weeks most likely. 

Then they asked me for some specs so they could see what they could get. I told them 10S, 60Amp ish with an 80 ish burst, a soft switch, solder points for the fuel gauge, and the charge circuit set up so that the fuel gauge would light up but the mains wouldn't energize while the unit was powered off and charging. I've had enough of the VESC-Wifi twitching. lol

So now i'm waiting to hear back from them about what they can do. If they can do this, who's in and for how many?
```

---
## \#2 Posted by: akira Posted at: 2016-04-05T11:26:39.368Z Reads: 337

```
Hi longhairedboy,
Nice initiative !
What about max voltage ?
I guess it is small enough for an easy Europe shipping, right ?
```

---
## \#3 Posted by: Ulfberht Posted at: 2016-04-05T11:31:39.738Z Reads: 330

```
I'm in if the price is right. Not sure how many yet...
More info should get me there...
Ummm...Please excuse my ignorance, but what is a "softswitch"?
```

---
## \#4 Posted by: longhairedboy Posted at: 2016-04-05T12:34:37.897Z Reads: 324

```
That's when it has a built in switch so you don't have to buy one seperately. All you have to do is attach your favorite push button.
```

---
## \#5 Posted by: longhairedboy Posted at: 2016-04-05T12:36:15.764Z Reads: 309

```
I'm sure they can ship to europe, but when they get back with me i'll ask to be sure.  

This is for a 10S BMS. A bunch of us just did a group buy on cells and are making 10S packs.
```

---
## \#6 Posted by: DeathCookies Posted at: 2016-04-05T13:31:30.530Z Reads: 303

```
I want to buy somewhere a bis, too. But i have some different specs:

- 12S Li-Ion Batteries
- Different ports for charging and discharging
- Continous Discharging: >= 60A
- Continous Charging: 60A
- Chargeable with a 12-18V DC power supply
- Power switch (ON / OFF) (you called it soft switch) 

But now i have a question. Is it possible to charge a 12S battery pack through a BMS  with a 12-18V DC power supply?
```

---
## \#7 Posted by: longhairedboy Posted at: 2016-04-05T18:38:11.330Z Reads: 293

```
Li-ion just got back with me and said thier suppliers don't offer anything like this, which is weird to me, since i've seen them elsewhere, but ok. 

So i guess if we want to do a group buy from bestech or somebody i'd still be down. Otherwise i'm just going to get some for me. 

poop.
```

---
## \#8 Posted by: lox897 Posted at: 2016-04-05T20:12:28.832Z Reads: 297

```
I'm pretty sure you can't. But ask @chaka , he would know.
```

---
## \#9 Posted by: paragon Posted at: 2016-04-05T21:58:46.669Z Reads: 300

```
I'd buy one. 

*20 characters :wink:
```

---
## \#10 Posted by: Ulfberht Posted at: 2016-04-05T23:12:43.335Z Reads: 307

```
I'm in for at least one. Depends on the deal. If we are close to an attractive volume price/shipping break I would easily go 2. 
Anybody else?
```

---
## \#11 Posted by: treenutter Posted at: 2016-04-06T02:15:00.171Z Reads: 310

```
@longhairedboy moving this detail to the group-buy thread...

I got a quote today from Bestech for this BMS. Price is $49.50. Minimum order is two. I'd love it if someone here who has experience selecting BMS's could take a look at the specs and help me to understand whether this is a good choice for 10s3p. It seems to be aligned with what we've been looking for. It's even more robust with 80a continuous discharge and 20a charging. Also is wired for a power switch.

I've got a note in to Bestech about group pricing, shipping costs, and whether they have a model that provides charging leads that are separate from the power leads (I think this might be the way to accomplish a fuel-guage when the power is off). 

Also, is it strange that to charge 10s on this model, you have one 8-port JST connector for most of the balance leads and then a dual in another place on the PCB?

<img src="/uploads/db1493/original/2X/b/be4f62195a6a98d23aeb5fecf884996a73bde5c8.jpg" width="450" height="338">
http://www.bestechpower.com/37v10spcmbmspcbforli-ionli-polymerbatterypack/PCM-D223V1.html

<img src="/uploads/db1493/original/2X/6/62643e0c283dc282cac620972d7df5aa1082cc5d.png" width="351" height="499">
```

---
## \#12 Posted by: lox897 Posted at: 2016-04-06T03:13:20.806Z Reads: 275

```
What cells are you using? If they are 20 amp continuous cells you should get a 60 amp continuous bms if you are doing 3p.
```

---
## \#13 Posted by: longhairedboy Posted at: 2016-04-06T11:36:12.153Z Reads: 273

```
its kind of big but it will definitely get the job done. And it looks pretty tough. 

I've been scrolling up and down bestech's list and couldn't decide, but kept coming back to this one too. 

I'm in for this one. What about you, @cmatson ?

@lox897 i think some or most of us are going 10S4P on this one.
```

---
## \#14 Posted by: paragon Posted at: 2016-04-06T12:08:47.511Z Reads: 267

```
I'm going 10s4s so I'd be in
```

---
## \#16 Posted by: lox897 Posted at: 2016-04-06T12:51:38.666Z Reads: 260

```
@treenutter Sounded like he was doing 3P though.
```

---
## \#17 Posted by: longhairedboy Posted at: 2016-04-06T13:15:27.868Z Reads: 254

```
You could still use this BMS on a 10S3P you'd just need to mind your VESC's power draw settings and stick to a reasonable charge amperage.
```

---
## \#18 Posted by: treenutter Posted at: 2016-04-06T14:33:31.342Z Reads: 256

```
@longhairedboy @lox897 Yes, I'm planning 10S3P.. but I think the idea is that I wanted a BMS that was robust enough to handle any hi-amps pulls that might occur; so a little bit of  overhead with 80A. I think that I'd keep VESC set at 60A continuous draw, although I don't think I've ever pulled that much. I'll adjust the voltage cutoffs accordingly. As @longhairedboy notes, adjust the charging rate and voltage to match. Does that sound right?

Come to think of it, though, How would I limit charging voltage if the charger doesn't have any setting? If this BMS can only deliver 42V, I might need to reconsider. I guess I would just get a charger that tops out at 37V? I'm not sure that makes sense...
```

---
## \#19 Posted by: cmatson Posted at: 2016-04-06T14:44:58.131Z Reads: 257

```
[quote="longhairedboy, post:13, topic:2172"]
I'm in for this one. What about you?
[/quote]

Yep, I'm good with that one.
```

---
## \#20 Posted by: longhairedboy Posted at: 2016-04-06T14:52:51.231Z Reads: 291

```
ok so for this buy we have....
@cmatson
@treenutter
@paragon
@Ulfberht

Anyone else? Also, how many do you guys want? I'm getting two and i think i saw @Ulfberht say he wanted two as well.      

I don't think we'll get any kind for price break for our volume but $50 isn't bad for this guy i think.
```

---
## \#21 Posted by: akira Posted at: 2016-04-06T14:57:15.719Z Reads: 289

```
Do you think a shipping to France would kill the deal (because of the shipping costs) ?
If not, I am in for two !!
```

---
## \#22 Posted by: barajabali Posted at: 2016-04-06T15:05:02.496Z Reads: 270

```
I also still want one Fam
```

---
## \#23 Posted by: paragon Posted at: 2016-04-06T15:06:37.527Z Reads: 268

```
I'm in for one. $50 isn't bad at all.
```

---
## \#24 Posted by: treenutter Posted at: 2016-04-06T15:22:17.391Z Reads: 269

```
@longhairedboy I got some responses from Bestech today, here are my questions and their answers:

*Do you carry a BMS that has a separate charge port, so that it is not required to turn on the BMS while charging?*
For this item,it can do 60A charging current and 60A discharging current in same port. And also can do 20A charging current and 80A discharging current in different port. 

*For the model below, what is the expected shipping cost to the US? Is the minimum order 2 units?*
For 2pcs samples,it need 27.50USD shipping cost to USA. MOQ is 2pcs.

*Is there a bulk discount for ordering a larger volume? 10-20 perhaps?*
For 10-20pcs,usually it is same as samples. We can talk later once you want 10-20pcs.

*If I can arrange a group-purchase of 10-20, could they be sent to multiple addresses?*
It can send to different address,but the shipping cost would not be same.
```

---
## \#25 Posted by: treenutter Posted at: 2016-04-06T15:24:47.622Z Reads: 238

```
@longhairedboy Yup, I'm in for one as long as I can figure out how to limit charging voltage to not exceed 10S3P.
```

---
## \#26 Posted by: longhairedboy Posted at: 2016-04-06T16:19:06.269Z Reads: 239

```
wouldn't the charging voltage be the same for 3P as 4P? this is something i'm fuzzy on. All i know is that charging voltage is higher than the packs output voltage, and the pack voltage is the same no matter how many you have in parallel.
```

---
## \#27 Posted by: paragon Posted at: 2016-04-06T17:11:43.737Z Reads: 234

```
It would be the same.
```

---
## \#28 Posted by: evoheyax Posted at: 2016-04-06T20:48:00.037Z Reads: 225

```
I might be in for one. If it would work as a replacement for the space cells bms, then I'm down.
```

---
## \#29 Posted by: Ulfberht Posted at: 2016-04-06T20:56:25.293Z Reads: 232

```
I got a quote and datasheet this morning from Bestech as well. It is unclear if they would be willing to do a group buy. They didn't actually give me all the info I requested. I wanted a volume price breakdown before I negotiated price and shipping terms. I couldn't post the PDFs on here, but I have a $49.50 MOQ:2 quote.
```

---
## \#30 Posted by: cmatson Posted at: 2016-04-06T20:56:36.364Z Reads: 229

```
[quote="evoheyax, post:28, topic:2172"]
If it would work as a replacement for the space cells bms, then I'm down.
[/quote]

it would, and I believe it supports a higher continuous amperage aswell!
```

---
## \#31 Posted by: Ulfberht Posted at: 2016-04-06T21:04:03.897Z Reads: 230

```
That is correct, sir. Here's info from the data sheet.
For 37V 10S Li-ion/Li-Polymer Battery Packs
Data Sheet
Model: HCX-D223V1 
**10S--80A working current**
2 Voltage Charging voltage 42V
9 Resistance Inner resistance ≤20mΩ
**Maximal continuous charging current 20A**
**Maximal continuous discharging current 80A**
Current consumption ≤20μA
Over charge detection voltage 4.28V±0.025V
Over charge detection delay time 0.5~2S
Over charge release voltage 4.08V±0.05V
Over discharge detection voltage 2.80V±0.05V
Over discharge detection delay time 50~200mS
Over discharge release voltage 2.80V±0.1V
Over current detection voltage 0.1V~0.2V
Over current detection current 240A±40A
Detection delay time 5~20mS
Release condition Cut load,automatically recover
Detection condition Exterior shot circuit
Detection delay time 200~500uS
Release condition Cut load,automatically recover
Balance voltage for single cell 4.2V±0.025V
Balance current for single cell 126mA±15mA
Operating temperature range -40 ~ +85°C
Storage temperature range -20~ +125°C
11 Size (L*W*T) L120mm * W80mm * T25mm

Enjoy...
```

---
## \#32 Posted by: evoheyax Posted at: 2016-04-06T21:56:44.386Z Reads: 212

```
Ok I'm down for one then. Any idea when these guys would arrive?
```

---
## \#33 Posted by: Ulfberht Posted at: 2016-04-06T22:14:24.382Z Reads: 209

```
[quote="treenutter, post:11, topic:2172"]
I'd love it if someone here who has experience selecting BMS's could take a look at the specs and help me to understand whether this is a good choice for 10s3p. It seems to be aligned with what we've been looking for. It's even more robust with 80a continuous discharge and 20a charging.
[/quote]

@chaka You are the man when it comes to this stuff!! I'm wondering about a 10s5p pack. Do you foresee any possibly issues/pitfalls to watch out for?
```

---
## \#34 Posted by: Krudte Posted at: 2016-04-06T22:22:56.442Z Reads: 194

```
Going of @akira's comment: Do you think a shipping to Denmark would kill the deal (because of the shipping costs) ? If not, I am in for one as well.
```

---
## \#35 Posted by: akira Posted at: 2016-04-07T05:30:25.317Z Reads: 199

```
If we do not get an good shipping cost, we could set up another group buy for Europe.
I am sure I can get some people from okp s forum onboard.
```

---
## \#36 Posted by: Ismon Posted at: 2016-04-07T09:35:58.234Z Reads: 195

```
Im looking for a 10s4p bms, so im in for one. Depending on shippingcosts to Sweden.
```

---
## \#37 Posted by: akira Posted at: 2016-04-07T11:47:15.506Z Reads: 198

```
Already three possible order in Europe.
I have posted a message on the French forum.
Let's see how it goes.

@longhairedboy : I hope you do not see it as a hijacking of your order.
I am just trying to get the best deal for us in Europe :-)
```

---
## \#38 Posted by: longhairedboy Posted at: 2016-04-07T11:52:52.458Z Reads: 197

```
its all good man. living in different places means ordering from different places a lot of the times. My original thing fell through anyway.
```

---
## \#39 Posted by: longhairedboy Posted at: 2016-04-07T17:49:51.750Z Reads: 201

```
@treenutter so how should we proceed? They mentioned that they'd be willing to ship to each of us individually. 

I'm going to want 2. Would you like to handle the coordination of orders since you have a dialog open with them already? I can PM you my email and billing info if they can send us each payment links or whatever like liion did.
```

---
## \#40 Posted by: treenutter Posted at: 2016-04-07T19:28:39.304Z Reads: 203

```
@longhairedboy I'm happy to coordinate w them to see if we can get a party started. For the US order I see:

@treenutter for 1 
@cmatson for 1
@paragon for 1
@Ulfberht for 1
@longhairedboy for 2
@evoheyax for 2
@Sharkface for 2  
Am I missing anyone?

I'll email them to ask if they can send these to different addresses and treat them like different orders in terms of payment and shipping.
```

---
## \#41 Posted by: akira Posted at: 2016-04-07T21:27:44.059Z Reads: 188

```
Would you mind asking the shipping cost to France for 5 to 10 units ? I could gather the EU order and dispatch the bms ...
```

---
## \#42 Posted by: cmatson Posted at: 2016-04-07T22:14:18.296Z Reads: 171

```
And you'll be able to ship mine to LHB, and I'll pay him to ship it from his place to mine. 

We are both in Florida, and only a couple hours away so it's not a big deal but could make it easier on your part.
```

---
## \#43 Posted by: treenutter Posted at: 2016-04-07T22:19:33.577Z Reads: 175

```
Thanks @cmatson. I'll report back once I hear from bestech. With these cells already on my bench I'm eager to get the order in!
```

---
## \#44 Posted by: Sharkface Posted at: 2016-04-07T23:15:48.537Z Reads: 173

```
Late bloomer here, throw me down for 2 eh bruh!
```

---
## \#45 Posted by: evoheyax Posted at: 2016-04-07T23:17:53.804Z Reads: 170

```
Yes you missed me. I'm down for two actually.
```

---
## \#46 Posted by: treenutter Posted at: 2016-04-08T00:26:09.742Z Reads: 170

```
@evoheyax @Sharkface I got ya now. Thanks! Still waiting to hear back from Bestech with more details about how to set up an order.
```

---
## \#47 Posted by: paragon Posted at: 2016-04-08T02:30:42.124Z Reads: 166

```
I am also in florida
```

---
## \#48 Posted by: Ulfberht Posted at: 2016-04-08T04:28:26.998Z Reads: 169

```
[quote="chaka, post:32, topic:2087, full:true"]
You guys should do a group buy at green bike: http://www.greenbikekit.com/battery-charger.html Pick your wattage, voltage and connector style and they do the rest. Shipping starts around $45 so you need to buy more than one to see any savings.
[/quote]

This looks like a possible lead as well. Pulled this from another thread. Thanks Chaka. Something to consider...
http://www.greenbikekit.com/bms-pcm/12s-e-bike-lithium-battery-bms.html
```

---
## \#49 Posted by: longhairedboy Posted at: 2016-04-08T14:03:11.979Z Reads: 163

```
Yeah i don't mind dispatching Florida orders if it will drive down the cost a little bit. It might add two or three days to the delivery time but if it saves money lets do it. 

If it doesn't save on the total order price though then it probably won't be worth it.
```

---
## \#50 Posted by: treenutter Posted at: 2016-04-08T14:06:04.414Z Reads: 168

```
Nice find @Ulfberht and thanks @chaka... the shipping rates from greenbikekit are actually lower than bestech. 

Bestech responded this AM but didn't answer my questions about the ordering or payment options. I tried again with a more clear bulleted list of queries. Fingers crossed for a complete response today!

@cmatson @paragon @longhairedboy @evoheyax @Sharkface can you guys take a look at this BMS that @Ulfberht found at GBK to assess whether we like it better\as much as the Bestech one? It looks like it's designed for Lifepo and thusly charges to 3.6, but our cells are 3.7 so it may not be ideal. The cost and shipping prices are good. There's an option to get one rated to 100A discharge which I don't think anyone will (or should) hit but the overhead might be a benefit.

I sent an email to GBK to see if they have a comparable BMS to our Bestech option. Just looking for an alternative given that BT communication is slow and it's hard to figure out exactly what the conditions of the order are.
```

---
## \#51 Posted by: longhairedboy Posted at: 2016-04-08T14:11:46.529Z Reads: 152

```
yeah this is lifepo.. some BMSs can do all of them because of thier adjustable voltages, or so i hear.. but this one looks like its firmly set to 3.6v and we're all running 3.7v.
```

---
## \#52 Posted by: Ulfberht Posted at: 2016-04-08T14:16:32.160Z Reads: 150

```
I had a similar experience with Bestech customer service via email. They were even monosyllabic in their responses. When I asked about group pricing and shipping her reply was simply "Resend". Which was a data sheet and price quote with the min order of 2. I already sent an email to GBK to see what kind of deal we can work out. That was last evening, so we'll see what's up hopefully today. I don't know if anyone else is on it, but it couldn't hurt to hit them with multiple emails requesting group buy. Maybe...
@longhairedboy I hear you. If the shipping added to the total doesn't benefit us, it makes it a more complicated and fruitless venture.  Like running in a hamster wheel with leg weights on. LOL
```

---
## \#53 Posted by: chaka Posted at: 2016-04-08T14:20:03.258Z Reads: 142

```
Bestech will ignore you if you send too many emails. Keep it short and concise. I normally get my orders in with 3 or 4 emails. They are not in the business of educating customers so they may have gotten a bit impatient and are now brushing you off if you have sent them 20 emails ;)
```

---
## \#54 Posted by: treenutter Posted at: 2016-04-08T14:29:49.820Z Reads: 145

```
@longhairedboy yeah, that's what I figured thx for confirming. They state that it will work with liion, but I think that means we'd sacrifice .1 volts, so not the best option.
```

---
## \#55 Posted by: Sharkface Posted at: 2016-04-08T14:33:55.409Z Reads: 146

```
One final thing to add that @longhairedboy and yall havent mentioned: If it can handle our 18650 builds, but is expecting a 3.6 nominal cell, then wouldnt it not charge the 18650s to 100%? What I mean by that is: Could using this extend the life of our packs since we are not constantly 100% charging?
```

---
## \#56 Posted by: treenutter Posted at: 2016-04-08T14:41:24.270Z Reads: 144

```
thx @chaka good advice! I haven't asked them a single technical question; just basic questions about their ordering process i.e. payment options, and total cost. Total emails to them so far has been 3 :smile:
```

---
## \#57 Posted by: chaka Posted at: 2016-04-08T14:52:50.456Z Reads: 147

```
Their english is not very good so it is best to keep things really simple when sending emails. Try to use the same wording that is on the data sheets. You guys have already picked the model so all that is left is to pick the low V cutoff and overcurrent protection amperage.
```

---
## \#58 Posted by: paragon Posted at: 2016-04-08T19:13:25.447Z Reads: 152

```
If they have a 10s li-ion option (3.7-4.2v), I'm for it.
```

---
## \#59 Posted by: longhairedboy Posted at: 2016-04-08T19:38:31.425Z Reads: 159

```
that's what we're going for. At least that what i need. I'm pretty sure that's the direction this group buy is going though. If not i'm out.
```

---
## \#60 Posted by: treenutter Posted at: 2016-04-08T20:30:17.011Z Reads: 165

```
@paragon @longhairedboy that's what we're going for! I'm hoping for more detail from Bestech tonight and then we can proceed.
```

---
## \#61 Posted by: paragon Posted at: 2016-04-08T20:44:22.738Z Reads: 160

```
This is what Bestech sent me this morning: <img src="/uploads/db1493/original/2X/c/cd900eea95cf247a6b9314e0f0edd095042a186a.png" width="690" height="247">
```

---
## \#62 Posted by: Sharkface Posted at: 2016-04-08T21:42:16.654Z Reads: 164

```
Looks like what @chaka said about their english was a legit thing. lol They didnt get us info on more than two? or did you not ask yet? 

My guess is that if they are going to have a hard time working with us to setup the deal, they would have a hard time working with us to setup individual shipping. 

Sounds to me like we might have to consider getting it shipped to one person who then ships it out to the rest of us. Anybody else getting that vibe or am I a crazy ole shark?
```

---
## \#63 Posted by: Ulfberht Posted at: 2016-04-08T22:04:54.860Z Reads: 166

```
Language barrier or no, I think we're getting slow-played on this hand. They know what we want. I already messaged them with very clear/ concise questions and they keep coming back with that same quote that @paragon just got. I have the exact same quote in my inbox. They don't seem to understand the concept of group buy, OR......They are slow playing us because a good sales department knows how to maximize profits. IDK
@sharkface I totally agree with you, dude. It sounds sketchy at best to get group pricing and individual shipping looks like it would not really be a smart $$$ move for Bestech. 
I said I was in so damn it I'm in, but if this is not the right deal for us, maybe reconsider the Supowerbattery one:
http://www.ebay.com/itm/221769582503
Here's an 80A version: 
http://www.ebay.com/itm/221759350948
Any thoughts?
```

---
## \#64 Posted by: laurnts Posted at: 2016-04-09T01:20:04.391Z Reads: 151

```
Btw sorry this is out of the question, before ordering, is it possible to use BMS of lets say 10s configuration for 6s configuration (at least lower than 10s)?
```

---
## \#65 Posted by: longhairedboy Posted at: 2016-04-09T02:39:46.345Z Reads: 152

```
I wouldn't try it but if someone else here has I'd love to hear about it.
```

---
## \#66 Posted by: Sharkface Posted at: 2016-04-09T07:23:11.706Z Reads: 154

```
[quote="Ulfberht, post:48, topic:2172"]
This looks like a possible lead as well. Pulled this from another thread. Thanks Chaka. Something to consider...http://www.greenbikekit.com/bms-pcm/12s-e-bike-lithium-battery-bms.html
[/quote]

In light of recent event, I would love to see us turn to a 12S solution for this group buy ;)

Edit: forgot that one was for 3.6v nominal cells, but still would love some 12S action.
```

---
## \#67 Posted by: treenutter Posted at: 2016-04-10T01:34:58.285Z Reads: 151

```
I've heard back from Bestech! Like @chaka has mentioned, communication with them is a little bit challenging. But here's what I was able to learn:

They are willing to send multiple invoices for the order, so we can each pay through paypal for our individual purchases. They will ship to multiple addresses, but it's not clear if the MOQ for each address is one BMS or two. I _think_ it's one, but I guess we'll find out!

Their instructions are for me to send them a mailing address and an email address for each buyer, and they then will send a quote\invoice to each of us with payment instructions. We can chose, at that point, to dive in or not.

So, if you want to give it a shot, PM me that info and I'll send it to them as a bundle. This particular BMS seems ideal, which is my motivation for trying this one instead others. 

I like the idea of many of us from the group liion order getting the same BMS for our builds, we can troubleshoot together!

DISCLAIMER: I've never ordered from Bestech before, and I can't speak to their speed or reliability, so please know that I'm just trying to help! If we all get ripped off, go after them, not me :smile:  
 
Here's the lineup for the buy

@treenutter for 1
@cmatson for 1
@paragon for 1
@Ulfberht for 1
@longhairedboy for 2
@evoheyax for 2
@Sharkface for 2

Finally, no hard feelings if you decide to go another direction!
```

---
## \#68 Posted by: evoheyax Posted at: 2016-04-10T02:01:13.680Z Reads: 141

```
If anyone wants to get down on a group buy on the Samsung 25r lipo cells in a few months, I would be down for it. I wasn't able to get on the last one due to $$$, but I'll be better off in a few months.
```

---
## \#69 Posted by: treenutter Posted at: 2016-04-11T14:57:09.588Z Reads: 142

```
Thanks for PM'ing me your info everyone. I sent the order to Bestech today. We should each receive an invoice and instructions for payment via email. My fingers are crossed that this works!

@cmatson 
@paragon 
@Ulfberht
@longhairedboy
@evoheyax
@Sharkface
```

---
## \#70 Posted by: longhairedboy Posted at: 2016-04-11T16:08:37.881Z Reads: 139

```
Hell yes! i'm looking forward to building this pack. 

Guess i better get a deck in the press for it now!
```

---
## \#71 Posted by: Michaelinvegas Posted at: 2016-04-11T17:05:29.929Z Reads: 138

```
You better post your build or I'm going to Florida and sitting in your workspace till you finish one ....lol
```

---
## \#72 Posted by: longhairedboy Posted at: 2016-04-11T17:07:06.154Z Reads: 138

```
Awesome! you can babysit so i can get some damned work done. lol
```

---
## \#73 Posted by: Michaelinvegas Posted at: 2016-04-11T17:07:31.510Z Reads: 138

```
Shit we could have daddy daycare
```

---
## \#74 Posted by: Michaelinvegas Posted at: 2016-04-11T17:08:16.774Z Reads: 133

```
Dude be happy I don't live near you... People would think we be having an affair
```

---
## \#75 Posted by: longhairedboy Posted at: 2016-04-11T17:09:26.484Z Reads: 142

```
i can only imagine the antics involved. Especially with my completely fearless little one.
```

---
## \#76 Posted by: Michaelinvegas Posted at: 2016-04-11T17:12:19.353Z Reads: 140

```
Ugh...we could start a whole new group discussion on this topic lol
```

---
## \#77 Posted by: Sharkface Posted at: 2016-04-12T06:36:10.987Z Reads: 147

```
I just got an email from Besttech showing the same model, and the same count, yet instead of $78 its $99 for two?

Can anybody else confirm this or have I been hitting the bottle too much tonight.

@longhairedboy
@evoheyax
```

---
## \#78 Posted by: longhairedboy Posted at: 2016-04-12T11:53:20.412Z Reads: 153

```
yeah that's what i got. i didn't realize it until after i paid, but it was $99 for both instead of the $78 plus shipping and a paypal fee. $133 total. But we also didn't get the 60amp version, we got the 80 amp version with a burst over current protection at 240 amps, which i thought was kind of ridiculous until i remembered the cells we bought each have a 100amp burst and 20 amp continuous and i think most of us are doing 10S4P with those cells, which is also quite ridiculous. 

but that's what we do here. We build ridiculously over powered rocket sticks.
```

---
## \#79 Posted by: treenutter Posted at: 2016-04-12T12:19:20.547Z Reads: 151

```
@Sharkface @longhairedboy my invoice is for $78.23 for one unit. The unit itself is $49.50, shipping is $25, plus their PayPal fee.
```

---
## \#80 Posted by: laurnts Posted at: 2016-04-12T13:15:02.386Z Reads: 150

```
Wow this BMS is so expensive that doesn't count the lithium setup its self. If you add a voltmeter + soft switch + fuse with just 10s3p config you'll end up same price as space cell minus the case. Not sure if buying BMS'es worth when the bms is so expensive. TBh they should cost less than 20 euro when bought together in high quantity.
```

---
## \#81 Posted by: akira Posted at: 2016-04-12T13:30:49.435Z Reads: 153

```
Why do you need the BMS for the discharge ?
Can't you just have it for the charging and bypass it for the ride ?
You could then go to a much cheaper BMS since you have less current requirements ?
```

---
## \#82 Posted by: longhairedboy Posted at: 2016-04-12T13:49:37.389Z Reads: 147

```
soft switch is on board. All you need is a push button and fuel gauge which is about $10 worth of accessories on ebay. balance leads are maybe another $5. You can buy lower powered ones for less money. We went big. 

I may step down to a 50 or 60 amp version next time, but this time around i wanted to see what i could pull out of these cells. 

my only issue with this BMS at the moment is that it doesn't have a single balance port, it is instead split across two physical ports according to the data sheet and that's going to require that i make an adapter of some kind, which is fine. Its probably a good idea to keep things modular anyway.
```

---
## \#83 Posted by: longhairedboy Posted at: 2016-04-12T13:52:23.665Z Reads: 140

```
double the over/under current/voltage protection seems like a solid reason. Things can be limited on the complete pack as well as on the VESC, but i'm not just building a pack for one application. I'm building a process to build packs for other people's boards as well.
```

---
## \#84 Posted by: treenutter Posted at: 2016-04-12T13:53:09.028Z Reads: 143

```
@laurnts I agree that it could be cheaper. I think the high shipping cost is really throwing it off for us! As far as bypassing the BMS during discharge, you're right that it's possible, but then you don't get the low-voltage protection that the BMS offers. This particular model is probably over spec'd for most esk8 purposes.
```

---
## \#85 Posted by: akira Posted at: 2016-04-12T14:08:22.505Z Reads: 140

```
But the VESC already has a low voltage protection, hasn't it ?
```

---
## \#86 Posted by: paragon Posted at: 2016-04-12T14:27:54.491Z Reads: 140

```
I think I'm going to go with the $110 quote for two that I got (from alibaba). If anyone wants the second one let me know.
```

---
## \#87 Posted by: treenutter Posted at: 2016-04-12T15:16:34.202Z Reads: 138

```
@akira That's correct. VESC has it's own low voltage cutoff feature.
```

---
## \#88 Posted by: Sharkface Posted at: 2016-04-12T15:32:01.912Z Reads: 142

```
@paragon posted a picture above that mentioned the same BMS we just got quotes on, and put that quote at  $39 a unit price. I guess that's why I was bringing this up and shit bruh. Not sure if bringing it up with them is gonna work out for me or not lol
```

---
## \#89 Posted by: paragon Posted at: 2016-04-12T15:49:06.217Z Reads: 145

```
Try getting a quote through alibaba. They gave me the higher quote when I emailed them directly.
```

---
## \#90 Posted by: cmatson Posted at: 2016-04-12T21:23:00.506Z Reads: 150

```
[quote="longhairedboy, post:78, topic:2172"]
i didn't realize it until after i paid
[/quote]

did you just paypal them through the account given on the invoice? 

just making sure before I pay for it directly through paypal, and not a website referral of some kind.
```

---
## \#91 Posted by: longhairedboy Posted at: 2016-04-12T22:06:39.790Z Reads: 149

```
Yeah and then I got a confirmation email from them. It's on it's way or so they say.
```

---
## \#92 Posted by: cmatson Posted at: 2016-04-20T20:44:36.728Z Reads: 149

```

I just emailed them again (making sure to keep the email very simple), because I didn't receive any confirmation... weird.

I paypaled them the exact amount specified, and added a note makings sure they knew the payment via paypal was for "BMS for Caden Matson (cadenmatson@yahoo.com)" yet I didn't hear back.
```

---
## \#93 Posted by: longhairedboy Posted at: 2016-04-20T21:17:43.445Z Reads: 152

```
i just heard from them yesterday, they say its shipping this week.
```

---
## \#94 Posted by: kaywerks Posted at: 2016-04-25T22:18:50.870Z Reads: 152

```
@longhairedboy I am too late :( But if anyone has a extra one or if anyone falls off, i'll take one!
```

---
## \#95 Posted by: longhairedboy Posted at: 2016-04-26T01:18:04.264Z Reads: 157

```
my 10S BMSs just arrived! and they included balance leads for the weird split port thing they did, so bonus.
```

---
## \#96 Posted by: treenutter Posted at: 2016-04-26T03:25:06.936Z Reads: 162

```
@longhairedboy I'm always a little bit amazed when orders like this actually work!
```

---
## \#97 Posted by: treenutter Posted at: 2016-04-26T13:00:38.022Z Reads: 168

```
@kaywerks I think we can still add an order if you want one. Read the thread above and PM me your details if interested.
```

---
## \#98 Posted by: cmatson Posted at: 2016-05-14T22:57:28.910Z Reads: 174

```
@longhairedboy or anyone else who got a BMS, could you post up a pic of the schematic? 

I have seemingly lost mine and therefore couldn't solder up my BMS today.. 

or if there is a web based diagram that'd be great too
```

---
## \#99 Posted by: longhairedboy Posted at: 2016-05-16T12:11:23.765Z Reads: 171

```
i think i have the paper one they sent in the package. I'll try to remember to take a pic of it and post it here.
```

---
## \#100 Posted by: Robert Posted at: 2016-05-16T22:09:14.732Z Reads: 164

```
How are they holding up / working ? I purchased a 10S BMS from eBay and it was DOA. i'm curious to see if you guys got them working
```

---
