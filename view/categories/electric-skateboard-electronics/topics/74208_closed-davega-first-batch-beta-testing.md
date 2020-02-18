# \[CLOSED\] DAVEga first batch (beta testing)

### Replies: 95 Views: 2583

## \#1 Posted by: janpom Posted at: 2018-11-10T22:25:24.046Z Reads: 474

```
I'll be ready to start shipping the first batch of [DAVEga](https://www.electric-skateboard.builders/t/davega-battery-monitor-odometer-speedometer/71509) kits in a few days. I only have about 25 pieces so there probably won't be enough for everyone, but it's not even meant for everyone. The purpose of the first batch is to test and tweak the gadget. I'm looking for volunteers.

This is an open source project that I'm doing in my spare time. I'll be shipping the kits for as cheap as I can without loosing money.

I would like to ship the kits to people who
- have some background in electronics and at least basic experience with Arduino;
- will know what they are doing when assembling the kit;
- are ready to encounter and address issues;
- would like to contribute to making DAVE better in any way;
- are willing to help support other people in using the next generation of DAVE;
- ideally have access to a 3D printer.

Dave has been reasonably well tested. The risk that you will end up with something completely unusable is low. However, there are some areas where I can see potential issues and/or need for figuring things out on your own. In particular:

- compatibility with various VESC derivatives and various VESC FW versions;
- spacers between the display PCB and the DAVE PCB;
- fitting DAVE into an enclosure;
- accessing buttons;
- routing cable out of the enclosure;
- making the harness for connecting to VESC and for updating the FW.

Enclosures are currently being designed by @mmaner and @lrdesigns, but are not finished yet and thus obviously haven't been tested by anyone. The PCB design may not be ideal wrt the enclosure and we may need to work around issues in the first generation. These issues will then hopefully be fixed for the next generation.

If there are any FW problems, I'll do my best to address them ASAP.

The kit will include the following:
- PCB
- ATMEGA 328P-PU with bootloader and pre-programmed DAVE FW
- USB-UART adapter
- crystal, capacitors, resistor, diode
- 3x button
- 5 pin right angle female header for connecting the UART adapter
- 2x 5 pin female header for connecting the display (not in the picture)
- JST connectors for the PCB and the VESC

![DSC01656|690x460](upload://5wDN3cRvbKKVRNRA5IL76alxTyk.jpeg) 

You will also need:
- **ILI9225 2.0" TFT LCD Display,** SPI, 176x220 pixels (can be found on AliExpress or similar for ~$5)
- 4 or 5 conductor cable of custom length

The JST connectors contain pre-crimped wires, which is handy if you don't have crimping pliers. To connect to VESC, you'll need to remove the wires from the 4-pin JST and plug them into the 8-pin JST housing.

![IMG_1509|528x500](upload://5XNeXuGgAs85CcUXNHD7ST78oln.jpeg) 

I will ask **$9 / €8 shipped** (world wide) for one kit. I'm located in Brno, Czech Republic. I'll ship untracked with the Czech Post. The $9 includes a $1 of "insurance" that I'll use to re-ship in case any packages are lost. (Still cheaper than shipping tracked.) The experience so far is that the delivery time is **3-4 days to Europe** and **1-2 weeks to the rest of the world**.

My time for dealing with the orders is limited, so I need to make it simple for myself. I can ship
- **one kit for $9 / €8**, or
-  **two kits for $15 / €13.50**. 

No more flexibility. I'm sorry if this is inconvenient. Please **don't order two unless you're ordering for someone else**. For the small/cheap parts, I'll include some spares, no worries.

To order, please PM me your address. I'll assume one kit unless specified otherwise. Please send the correspondent amount to my PayPal account jan.pomikalek@gmail.com. I'll aim to ship the first kits on Wednesday. After that, I should be able to ship every next morning after receiving the order.

If you prefer to wait for the package before you send the money, that's fine, but please do **friends and family** on PayPal so that no fees are deducted. I'm doing my best to keep this cheap and don't want to waste money on transfers. I accept both USD and EUR. **[Please do NOT convert to CZK](https://www.electric-skateboard.builders/t/davega-first-batch-beta-testing/74208/18?u=janpom).**

Please don't PM me with questions unless absolutely necessary. Ask any questions related purchasing the kit in this thread. Ask any questions related to DAVE in the [DAVE thread](https://www.electric-skateboard.builders/t/davega-battery-monitor-odometer-speedometer/71509). Thanks!

I'm looking forward to people having their own DAVEs. Some exciting developments on the enclosure are already in progress and there has been a bunch of great ideas in the DAVE thread. I'm sure we'll make it a great gadget together!

Useful links:
- [DAVEga thread](https://www.electric-skateboard.builders/t/davega-battery-monitor-odometer-speedometer/71509)
- [DAVEga repository](https://github.com/janpom/davega) - contains the FW source code and instructions how to install it
- [Few tips on kit assembly](https://www.electric-skateboard.builders/t/davega-battery-monitor-odometer-speedometer/71509/280?u=janpom)
- [Thoughts on making the harness](https://www.electric-skateboard.builders/t/davega-battery-monitor-odometer-speedometer/71509/293?u=janpom)
```

---
## \#2 Posted by: Grozniy Posted at: 2018-11-10T22:29:21.036Z Reads: 329

```
Great work. I'll wait until you can ship assembled kit :slightly_smiling_face:
```

---
## \#3 Posted by: yelnats8j Posted at: 2018-11-10T22:29:21.180Z Reads: 323

```
Kinda wanna get one but gonna leave the beta testing to people that understand electronics better. Im sure these will go insanly fast. :+1:
```

---
## \#4 Posted by: Andy87 Posted at: 2018-11-10T22:36:22.797Z Reads: 309

```
Got two displays today 😅
But unfortunately i‘m not experienced with arduino yet, so I probably also will wait till the beta tests are finished.
```

---
## \#5 Posted by: High-roller Posted at: 2018-11-10T22:39:55.020Z Reads: 281

```
I'm gonna wait for the updated version, but I can help with designing the enclosure if anyone needs help. I also have a 3d printer to test designs on.
```

---
## \#6 Posted by: brenternet Posted at: 2018-11-10T23:13:25.911Z Reads: 255

```
Will beta test through the bits Ben has ordered. 

Just want to say again, making this as open as you have and not trying to turn a huge profit from the community is pretty noble. It's appreciated and I'm sure this project is going to see loads of awesome offshoots and usage in the years to come. Thanks again for this.

Edit: Obviously it's been successful because of the name and not your hard work, but take a little credit of course.
```

---
## \#7 Posted by: deucesdown Posted at: 2018-11-11T06:55:19.403Z Reads: 226

```
Ah hell I already ordered the display and all, but I'm pretty lazy. I'll wait for batch #2.
```

---
## \#8 Posted by: JonathanLau1983 Posted at: 2018-11-11T10:32:01.544Z Reads: 212

```
Annoyed with myself for being impatient any getting all the bits now 😣
```

---
## \#9 Posted by: janpom Posted at: 2018-11-11T22:15:32.782Z Reads: 206

```
Update about PayPal: I accept both USD and EUR. No need to convert to CZK. Please do friends and family, so that we don't waste money on transfers. If you prefer to wait for the package before you send the money that's fine. I could accept Transferwise or direct bank transfers as well, but I prefer not to simply because it would make it more difficult for me to keep track.
```

---
## \#10 Posted by: Surfer Posted at: 2018-11-11T22:58:43.640Z Reads: 194

```
 Thanks @Janpom, what you do and how you do it is what it does this community different.
 I just want a odometer to hide it inside the enclosure, maybe, in the future!!!
:heart_eyes:
```

---
## \#11 Posted by: janpom Posted at: 2018-11-12T06:24:32.305Z Reads: 189

```
Dave lite (aka DAVIEga :)) is on my TODO list. I already have some ideas. I just now have full time job and two kids to take care of, so my time for this is limited. It will take a while, but we'll get there.
```

---
## \#12 Posted by: janpom Posted at: 2018-11-12T07:15:26.525Z Reads: 173

```
I received $9 (or $8.35 after fees) from someone named Klaus Noelp with a message that he's new on the forum. If you read this, could you please PM me or email me at jan.pomikalek@gmail.com. Thanks.
```

---
## \#13 Posted by: janpom Posted at: 2018-11-12T07:18:00.294Z Reads: 173

```
@Mich21050 You messaged me that you would prefer to do a bank transfer. We can do it if necessary, but I would prefer PayPal to make things easier. I'm trying to understand the reasons why PayPal doesn't work for some and if there's something I could do about it. Could you please explain what the trouble is? Thanks.
```

---
## \#14 Posted by: Mich21050 Posted at: 2018-11-12T07:19:48.512Z Reads: 168

```
Yeah no problem.  My paypal Account has been hacked and someone bought something for 600€ :frowning:
```

---
## \#15 Posted by: janpom Posted at: 2018-11-12T07:22:43.430Z Reads: 169

```
Ugh, that sucks. I'm sorry. I will PM you and we'll figure something out.
```

---
## \#16 Posted by: janpom Posted at: 2018-11-12T12:23:42.631Z Reads: 169

```
I keep receiving some payments in CZK and it turns out that costs some 20% on fees (most of that on the sender side). I'll tweak my PayPal account settings later on today. **Please don't send me any money until then.**
```

---
## \#17 Posted by: rojitor Posted at: 2018-11-12T18:09:23.837Z Reads: 175

```
- no arduino background
- got issues enough on my own
- no 3d printer
- i suck
i guess i will have to wait for another batch
```

---
## \#18 Posted by: janpom Posted at: 2018-11-12T20:22:02.752Z Reads: 178

```
I may need some crowd wisdom here to correct me, but from what I understand so far, to avoid PayPal fees (which are pretty ridiculous), the following is necessary:

- do not convert the currency
- do the transaction as "friends & family"

Here's how I believe it should be done:
- select "Send & Request"
- send payment to: jan.pomikalek@gmail.com
- you send: 9 USD
- recipient gets: 9 USD
- set "Sending to a friend"

... or if you're doing EUR then
- you send: 8 EUR
- recipient gets: 8 EUR

I hope that EUR and USD covers 90% of people. If you have neither EUR, nor USD, you can either do the currency conversion and pay the fees or we can do Transferwise.

Note: Given the amounts to be paid, I find it completely unnecessary to use the buyer protection and pay extra. If anyone is uncomfortable doing "friends & family" as an advance payment, feel free to send the payment only after you have received your package.
```

---
## \#19 Posted by: deucesdown Posted at: 2018-11-13T04:21:14.465Z Reads: 165

```
Sigh I'm getting itchy. Any more spots left?
```

---
## \#20 Posted by: janpom Posted at: 2018-11-13T07:14:50.364Z Reads: 164

```
@deucesdown Yes, there are. I should be able to ship 11 kits tomorrow. Then I'm out of buttons though and they don't have them here so I'll need to wait for the package from China, which I expect any day now. More kits to hopefully go out next week.
```

---
## \#21 Posted by: ARetardedPillow Posted at: 2018-11-13T08:13:28.265Z Reads: 132

```
I have no arduino experience so I'll wait for batch 2

Can't wait for a more polished gadget!
```

---
## \#22 Posted by: deucesdown Posted at: 2018-11-13T15:28:50.990Z Reads: 134

```
Interesting, there's a new fee on the sender side.

[quote]
You'll send $9.00

Fee $0.99

We've used the cheapest payment option available in your wallet.There's a small fee when you pay using a credit or debit card. It's free if you use [a bank account](https://www.paypal.com/myaccount/wallet/add/bank) instead.

You'll pay$9.99
[/quote]
```

---
## \#23 Posted by: janpom Posted at: 2018-11-13T15:33:12.445Z Reads: 135

```
Thanks for the info. That's probably only if you pay with a credit card, which makes sense since PayPal gets charged for accepting a credit card payment. 11% fee is still pretty steep. That's definitely not what they get charged.

I'm getting pretty annoyed with PayPal. I think the batch 2 will be dogecoin payments only. :smile:
```

---
## \#24 Posted by: janpom Posted at: 2018-11-13T15:56:20.484Z Reads: 142

```
Guys, I'm going to collect a few missing bits tomorrow, complete you packages in the evening and ship them to you on Thursday morning. I'll be shipping to the following people:

- @Jumpman :white_check_mark: 
- @clistpdx :white_check_mark: 
- @amazingdave :white_check_mark: 
- @ROFEN13 :white_check_mark: 
- @swimmydude :white_check_mark: 
- @The_Dude :white_check_mark: 
- @Mich21050 :white_check_mark: 
- @deucesdown :white_check_mark: 

(:white_check_mark: = ready to do some SMD soldering :wink:)

 I also have an order from @SourPlumGoose. I'm sorry but I have to put you (and any other orders received henceforth) on hold until more buttons arrive, which is hopefully in a few days.

There's a small problem about capacitors. I wasn't able to get the right size THT locally. I'm expecting a big caps package, which will hopefully have the right (small enough) size. I can provide SMD capacitors though. Is everyone comfortable soldering them? It's not that hard. I managed to do it and I'm not particularly good at soldering. If you think it would be a problem for you please PM me and we'll figure it out.

To keep this thread uncluttered, I'll consider a like to this post as "I'm good with SMD".
```

---
## \#25 Posted by: swimmydude Posted at: 2018-11-13T16:27:57.895Z Reads: 133

```
I know you don't want clutter but I just want to say that I'll have a shipment soon of a bunch of capacitors. Both normal and ceramic, on top of the small assortment I already own. So feel free to ship without the problem part and just inform me. Though I imagine it'll be easier to ship everything at once anyway.
```

---
## \#26 Posted by: janpom Posted at: 2018-11-13T16:34:39.324Z Reads: 131

```
Looks like there's a misunderstanding. It's actually my plan to ship without the THT capacitors and give you SMD capacitors instead. This is to speed things up. Another option is to wait for the THT capacitors to arrive and I don't know when that will be.
```

---
## \#27 Posted by: swimmydude Posted at: 2018-11-13T16:36:36.020Z Reads: 122

```
Yea, that's fine. Sorry about that, makes sense now.
```

---
## \#28 Posted by: Battosaii Posted at: 2018-11-13T16:58:44.018Z Reads: 124

```
Hey sorry I payed but PayPal didn't let me pay in any other.currency except for yours I don't mind sending a bit extra to cover the conversion rate.
```

---
## \#29 Posted by: deucesdown Posted at: 2018-11-13T18:27:19.343Z Reads: 115

```
[quote="janpom, post:24, topic:74208"]
I can provide SMD resistors
[/quote]

You mean SMD capacitors?
```

---
## \#30 Posted by: janpom Posted at: 2018-11-13T18:56:40.728Z Reads: 112

```
Of course, sorry.
```

---
## \#31 Posted by: dg798 Posted at: 2018-11-13T19:46:23.021Z Reads: 113

```
@Kug3lis would be a great tester.
@Kug3lis do u agree?
```

---
## \#32 Posted by: Kug3lis Posted at: 2018-11-13T20:14:37.649Z Reads: 114

```
I had run the firmware with simple arduino and it works, but to do more in deep test don't have literally time :smiley:

Too many things on the hands right now to even pick something more :) Plus I have to finish shit loads of stuff before holidays :)
```

---
## \#33 Posted by: spesh Posted at: 2018-11-13T23:33:43.874Z Reads: 112

```
Put me down for one :)
```

---
## \#34 Posted by: ROFEN13 Posted at: 2018-11-14T03:34:44.685Z Reads: 112

```
I am so excited to test your amazing work!
```

---
## \#35 Posted by: janpom Posted at: 2018-11-14T20:48:37.664Z Reads: 123

```
I gathered all the bits and was about to complete the kits.

![IMG_1515|690x409](upload://svEXdMVX1TftaSYeXgAya5P1pCi.jpeg) 

I figured I would assemble one Dave using the parts I'm about to ship to double-check all works.

![IMG_1516|690x417](upload://8tjp9Lf9CrR4XPdi4Nl7PUu7g6L.jpeg) 

And it turned out that wasn't a completely stupid idea since though it did work, I wasn't able to update the firmware. The MCU wouldn't reset. It wasn't that hard to debug. The 100 nF caps I got are actually 20 pF caps. :( So I have to drop into my local electronics store again tomorrow and get the correct caps. They do have them on stock. They just messed up the order.

This will unfortunately delay me one day. I hoped I would be able to ship the kits to you guys tomorrow morning. It will have to wait until Friday morning, sorry.
```

---
## \#36 Posted by: ROFEN13 Posted at: 2018-11-15T00:55:54.335Z Reads: 110

```
Its ok!!! We all appreciate putting everything together for us!
```

---
## \#37 Posted by: mmaner Posted at: 2018-11-15T03:18:32.052Z Reads: 107

```
Printing the revised enclosure now, should see it in a couple of hours if I don't fall alseep.
```

---
## \#38 Posted by: lrdesigns Posted at: 2018-11-15T05:44:38.144Z Reads: 108

```
:beer::beer::beer::beer::beer::beer: :sleeping: :sleeping_bed:
```

---
## \#39 Posted by: janpom Posted at: 2018-11-15T19:11:55.485Z Reads: 118

```
I got the correct capacitors and finalized the kits. 14 Dave kits ready to go:

![IMG_1519|488x500](upload://bT3CMLEJ65SMvlE4uqhrTz7L6rL.jpeg) 

This took way more time than I have anticipated. I think I'll hire an assistant for the second batch... or at least get my kids to help. :smile: 

Tomorrow morning, the kits go to:
- Jumpman
- clistpdx
- amazingdave
- ROFEN13
- swimmydude
- The_Dude (2 kits)
- Mich21050 (2 kits, no buttons)
- ltsmedant
- deucesdown 
- JonathanLau1983 (no buttons)

I also have orders from:
- SourPlumGoose
- Battosaii
- spesh (who has sent money, but no address! :smile:) 

I'll ship the kits to you guys as soon as the buttons arrive.

A few words of caution. **The capacitors are really tiny.** Make sure you don't loose them or accidentally throw away thinking it's just a piece of paper. The strip with 1 piece has a 100nF cap; the strip with 3 pieces has 20pF caps (1 spare).

![IMG_1517|690x444](upload://dUnSXToIVelBpruIlKjuCruBvXI.jpeg) 

The 2x 5 pin headers are for the display. The display has 11 pins, but not all are used. If you use the headers, leave a 1 pin space in the middle ([see here](https://www.electric-skateboard.builders/t/davega-first-batch-beta-testing/74208/35?u=janpom)).

Note that if you do use the headers, it will make the whole thing thicker than if you solder the display directly to the PCB. However, if you [remove the yellow plastic from the display pins and cut them](https://www.electric-skateboard.builders/t/davega-battery-monitor-odometer-speedometer/71509/478?u=janpom), it will be only ~1mm thicker than if you solder directly. Do whatever works best for you.

Good luck!
```

---
## \#40 Posted by: janpom Posted at: 2018-11-15T19:21:23.333Z Reads: 104

```
BTW, I replaced the capacitor and checked that all works. It does!

Looking for 7 more guinea pigs! :smile:
```

---
## \#41 Posted by: JonathanLau1983 Posted at: 2018-11-15T20:28:01.222Z Reads: 101

```
Any advice for soldering on the capacitors?
Tin the pads before?
```

---
## \#42 Posted by: Jumpman Posted at: 2018-11-15T21:00:58.199Z Reads: 98

```
Tin one end first only, otherwise might be difficult to get it flat against the board.
```

---
## \#43 Posted by: mmaner Posted at: 2018-11-15T21:21:32.433Z Reads: 109

```
I don't like to cross post, but I thought there were likely people in the beta group that aren't watching the main post.  Here's the housing I designed, its tested and good.

https://www.electric-skateboard.builders/t/davega-battery-monitor-odometer-speedometer/71509/538?u=mmaner
```

---
## \#44 Posted by: janpom Posted at: 2018-11-16T08:35:42.825Z Reads: 99

```
All shipped.

I'm going to ship the remaining 7 kits assembled. Looking for people to test those. It's fine if you're not much into electronics/Arduino. It will be good to test whether updating the FW is feasible even for people with no previous Arduino experience and figure out how the FW updates could be made easier.

It would still be nice if you could help us tweaking the enclosures, so mechanical DIY skills and/or access to a 3D printer are much appreciated.

Please PM me if you're interested in an assembled test kit. Price will be the same as for unassembled.

@Grozniy @yelnats8j @Andy87 @High-roller @ARetardedPillow
```

---
## \#45 Posted by: Grozniy Posted at: 2018-11-16T08:47:35.827Z Reads: 94

```
I can't really ride due to snow... So I'll still wait ;)
```

---
## \#46 Posted by: High-roller Posted at: 2018-11-16T09:08:06.813Z Reads: 97

```
Reeeealy tempted! Pm'ing you now!
```

---
## \#47 Posted by: janpom Posted at: 2018-11-19T20:09:00.792Z Reads: 102

```
All remaining parts came in today:

![IMG_1522|690x446](upload://sFNoCPhctyHeAt2nARYUzgYKZ1S.jpeg) 

The capacitors are nice and small, no taller than the crystal:

![IMG_1523|629x500](upload://AKvTTt3tEHnaeSF9P7CY3cd7Mj.jpeg) 

The problem is that the legs of the 22 pF caps are too close to each other and they don't fit well in the PCB. I will update the next version of the PCB such that they fit. For this batch, I'll just keep adding the SMD caps.

It's late and I had a busy day, so I won't be able to get the packages ready tonight, but I should be able to make it tomorrow and ship on Wednesday morning.
```

---
## \#48 Posted by: Mich21050 Posted at: 2018-11-20T16:39:36.988Z Reads: 99

```
Ok so first of all thank you @janpom for the great kit. :smile: 
Is there someone who could maybe sell me a display withi the eu?
I can't find one locally and I don't want to wait :smile:
```

---
## \#49 Posted by: janpom Posted at: 2018-11-21T08:12:51.592Z Reads: 93

```
All shipped to [these guys](https://www.electric-skateboard.builders/t/davega-battery-monitor-odometer-speedometer/71509/618?u=janpom). I accidentally posted to the wrong thread yesterday. Just to make things clear here, **the batch 1 is now closed**. We'll do some testing now and once all is tweaked I'll start the second batch. It will probably happen early next year (January or February).
```

---
## \#50 Posted by: amazingdave Posted at: 2018-11-21T09:13:26.884Z Reads: 89

```
I’m still waiting for delivery on mine. Not a big deal as my screens haven’t turned up either...
```

---
## \#51 Posted by: janpom Posted at: 2018-11-21T09:44:38.121Z Reads: 89

```
That's too long for UK. I'll PM you.
```

---
## \#52 Posted by: Battosaii Posted at: 2018-11-21T20:06:06.722Z Reads: 88

```
Still waiting for screens wish I knew of a local source.
```

---
## \#53 Posted by: venom121212 Posted at: 2018-11-21T20:15:02.440Z Reads: 86

```
Ebay had some under 10
```

---
## \#54 Posted by: Battosaii Posted at: 2018-11-30T16:17:33.380Z Reads: 85

```
How long does the kit usually take to get delivered, I have not seen mine yet.
```

---
## \#55 Posted by: janpom Posted at: 2018-11-30T17:10:35.848Z Reads: 89

```
About 2 weeks if it's outside of Europe. It should arrive early next week.
```

---
## \#56 Posted by: Andy87 Posted at: 2018-12-01T14:32:34.325Z Reads: 92

```
Mine just arrived 😌
I losted a bit the latest news about Dave, so time to catch up reading the main thread and than... 🛠
```

---
## \#57 Posted by: Darkie02 Posted at: 2018-12-02T10:42:47.691Z Reads: 91

```
It arrived but the screen still some were in the post got a feeling it’s going to get lost in Christmas post. ☹️
```

---
## \#58 Posted by: ROFEN13 Posted at: 2018-12-05T22:33:23.985Z Reads: 86

```
I still havent gotten anything. Hopefully it arrives next week.  Before i leave for the holidays!
```

---
## \#59 Posted by: janpom Posted at: 2018-12-06T03:08:49.206Z Reads: 92

```
It looks like the packages outside of EU are taking their time. Could people please confirm whether their received theirs yet?

* @SourPlumGoose - ?
* @Battosaii - ?
* @venom121212 - ?
* @Andy87 - yes
* @High-roller - ?
* @yelnats8j - no

@ROFEN13, yours went out 19 days ago. It might have got lost. I believe all other packages to US from the same batch already arrived. I'm sorry. Let's give it a few more days. If you don't have it by Monday, please let me know and I'll ship another one or refund your payment.

Next time, we should probably do tracked outside of EU.
```

---
## \#60 Posted by: SourPlumGoose Posted at: 2018-12-06T03:11:45.499Z Reads: 91

```
As of today, I have yet to receive it.
```

---
## \#61 Posted by: Battosaii Posted at: 2018-12-06T03:22:39.424Z Reads: 81

```
Have not gotten it yet.
```

---
## \#62 Posted by: swimmydude Posted at: 2018-12-06T03:23:16.370Z Reads: 80

```
I'm US and haven't received my package yet. My screens from Ali hasn't came in yet either.
```

---
## \#63 Posted by: venom121212 Posted at: 2018-12-06T03:28:52.721Z Reads: 84

```
US and nothing here either. I will keep you posted.
```

---
## \#64 Posted by: ROFEN13 Posted at: 2018-12-06T03:36:30.648Z Reads: 85

```
Bummer! I will let you know.
```

---
## \#65 Posted by: janpom Posted at: 2018-12-06T06:16:45.316Z Reads: 85

```
Thanks everyone for getting back. It's unlikely that all packages got lost. No packages have been lost previously. It's reasonable to assume they just got delayed this time, which make sense since it's a busy period for carriers. Please be patient.
```

---
## \#66 Posted by: High-roller Posted at: 2018-12-06T06:19:36.752Z Reads: 84

```
Israel, I'm still waiting too. In general, standard shipping here takes around three weeks.
```

---
## \#67 Posted by: Andy87 Posted at: 2018-12-06T06:23:35.027Z Reads: 87

```
one of my parcels is stuck somewhere in france already 4 weeks and was on the way to US too. 
Could really be that they just slowly because of the busy time at the moment.
```

---
## \#68 Posted by: High-roller Posted at: 2018-12-06T16:56:29.956Z Reads: 89

```
![IMG_20181206_173442|375x499](upload://cLzjg2Rlcbk6SSMqQNVJOgHHydM.jpeg) 
Mine just arrived! I'll start working on enclosure designs tomorrow.
```

---
## \#69 Posted by: ROFEN13 Posted at: 2018-12-06T18:27:44.165Z Reads: 85

```
I got my screen. Still no DAVEga
![20181206_132553|375x500](upload://h58jCPhtqp8uD9C5AluB5QYCh2Y.jpeg)
```

---
## \#70 Posted by: venom121212 Posted at: 2018-12-07T00:25:58.521Z Reads: 85

```
That's funny, I just got my screen too! ![20181206_190500|281x500](upload://spizLtX9KsaEcmWb1wu2TCz8pIp.jpeg)
```

---
## \#71 Posted by: swimmydude Posted at: 2018-12-07T01:23:58.522Z Reads: 87

```
I ordered my screen a day or two within when I said I'd do beta testing. Dunno when exactly that was, too lazy to look. I got an email today that my screens arrived at my local post office. Does that count for something? lol

I'm not too worried about my package getting here super fast. I'm still waiting on my last few pieces of my build and my Unity. So who knows when I can actually test it. I'm really hoping before the end of the year. If Dave comes within the week, it'll be the first section of my board I can fully assemble even though it was the last thing on my list to have added.

_Edit: Screen came today, whoops._
![20181206_204427|374x500](upload://gRm0kGBpquGvHXV7RwfRi6swhYs.jpeg)
```

---
## \#72 Posted by: SourPlumGoose Posted at: 2018-12-07T04:56:27.580Z Reads: 83

```
Just received it today. Thank you :)
```

---
## \#73 Posted by: High-roller Posted at: 2018-12-08T18:39:26.526Z Reads: 88

```
![IMG_20181208_201258|375x499](upload://8lhHqc8208Ypsm8KoVRAi9wUpzz.jpeg) 
Well, I sure screwed this one up...
I got a hold of a screen from a guy here who didn't need it, turns out it was the wrong one. At least it was free...
I've yet to find the correct one in any stores here so does anyone have a spare they'd be willing to part with? I'll happily pay express shipping, it beats having to wait a month and a half for it to arrive from China.
```

---
## \#74 Posted by: janpom Posted at: 2018-12-08T21:26:17.359Z Reads: 89

```
That one unfortunately won't work. Maybe if you built an adapter for it, you could get the picture on screen, but it would be trimmed since it has a lower resolution than the correct display.
```

---
## \#75 Posted by: Andy87 Posted at: 2018-12-08T21:34:42.390Z Reads: 92

```
I have one spare, but shipping from Russia will be not fast too I guess
```

---
## \#76 Posted by: ROFEN13 Posted at: 2018-12-10T13:30:31.479Z Reads: 95

```
Look what just arrived!!!
![15444486051258424702339762749408|375x500](upload://8tP7NT9Uu6jYs1XPqCby8ufDPhZ.jpeg)
```

---
## \#77 Posted by: Battosaii Posted at: 2018-12-10T16:58:37.511Z Reads: 89

```
Nice man, still waiting for mine haha. This is such a cool device. 

Hopefully didn't get lost
```

---
## \#78 Posted by: new Posted at: 2018-12-11T15:38:25.690Z Reads: 83

```
Finally finished my assembly. The display works just fine. Now I need a VESC to try it out :slight_smile:
```

---
## \#79 Posted by: swimmydude Posted at: 2018-12-12T01:47:04.011Z Reads: 84

```
I got my kit today in the mail. I will be assembling it in the next few days. It would be sooner but seeing as I don't have a case or even my unity, I'm not in a rush.
```

---
## \#80 Posted by: PickSix24 Posted at: 2018-12-13T18:52:40.566Z Reads: 85

```
Anyone have one they would like to sell ?
```

---
## \#81 Posted by: janpom Posted at: 2018-12-13T19:37:41.546Z Reads: 77

```
@ROFEN13 might have a spare one... in a few weeks. :smiley:
```

---
## \#82 Posted by: Rithblu Posted at: 2018-12-13T20:43:12.379Z Reads: 74

```
Also looking, if someone have a spare.
```

---
## \#83 Posted by: Mich21050 Posted at: 2018-12-13T20:49:35.435Z Reads: 75

```
If somebody wants some pcbs I have some spare ones. Just send me a pm :smile:
```

---
## \#84 Posted by: ROFEN13 Posted at: 2018-12-13T21:58:13.098Z Reads: 80

```
I should as long as I dont mess up the first one!
```

---
## \#85 Posted by: PickSix24 Posted at: 2018-12-13T22:49:53.457Z Reads: 82

```
Good luck ! Let me know
```

---
## \#86 Posted by: mmaner Posted at: 2018-12-13T22:51:28.396Z Reads: 84

```
I have some extra PCB's if someone needs
```

---
## \#87 Posted by: janpom Posted at: 2018-12-13T22:54:03.205Z Reads: 85

```
Guys, also note you can order 10 PCBs directly from JLCPCB for about $8 shipped.
```

---
## \#88 Posted by: Rithblu Posted at: 2018-12-13T23:58:03.543Z Reads: 87

```
Hey Mike,  I'll like 2 if thats doable.
```

---
## \#89 Posted by: mmaner Posted at: 2018-12-14T00:08:47.211Z Reads: 88

```
Sure just PM me an address.
```

---
## \#90 Posted by: Battosaii Posted at: 2018-12-27T19:46:31.589Z Reads: 83

```
Hey @janpom any word on packages. I still have not gotten my kit yet.
```

---
## \#91 Posted by: janpom Posted at: 2018-12-27T19:56:12.377Z Reads: 90

```
Hi, they all went untracked so unfortunately I know nothing more than you. None returned. So far everyone received theirs... eventually. Please be patient. I don't have any spares to send out now. I may have in a few weeks so I'll reship if you still don't have yours by then. I'm sorry about the delayed delivery, but unfortunately that is to be expected during the Christmas period.
```

---
## \#92 Posted by: Battosaii Posted at: 2018-12-27T20:00:05.738Z Reads: 94

```
Alright thanks, I'll be waiting :slight_smile:
```

---
## \#93 Posted by: venom121212 Posted at: 2019-01-05T23:16:51.885Z Reads: 93

```
Mine came today! Can't wait to get it set up. Thank you again
```

---
## \#94 Posted by: annihil8ted Posted at: 2019-06-18T07:29:23.249Z Reads: 40

```
@janpom, I'm really interested in your kit! Are anymore available?
```

---
## \#95 Posted by: janpom Posted at: 2019-06-18T07:30:40.973Z Reads: 39

```
No, sorry. New DAVEga is coming soon though.
```

---
