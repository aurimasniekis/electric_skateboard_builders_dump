# Load tested VESCs for sale&hellip;gauging interest

### Replies: 42 Views: 3358

## \#1 Posted by: TheRedPanda Posted at: 2016-04-11T21:40:24.395Z Reads: 179

```
So I've purchased quite a few VESCs since they've become available. Doing so I've also burned a few, and despite the varying manufacturing quality a common theme is that none(as far as I am aware) of the VESC manufacturers actually test their product under load before shipping them out. So here is where I want to gauge interest in the community.

I have been talking to a local electronics manufacturer/assembler here in the US that has proven reliability in their processes. I am having a few VESCs produced by them and as long as their quality shows through I wanted to see if anyone is interested in purchasing VESCs that are only sold after being tested under load and inspected in house by an engineer. 

We are still working on pricing, but it should be very comparable to the VESCs already on the market.

This manufacturing run would happen without taking any pre payment from the community and would be self funded to launch this effort for a more reliable VESC market.


UPDATE: I received the VESCS and they are working excellently and the placement of the components is top notch, will likely post some pictures soon. I need to do more testing with these but they seem promising.
```

---
## \#2 Posted by: barajabali Posted at: 2016-04-11T21:45:34.772Z Reads: 173

```
What kind of long term effects does the load testing have on the VESC.  

I dont want to buy something thatll break in a few rides you know?
```

---
## \#3 Posted by: TheRedPanda Posted at: 2016-04-11T21:50:31.473Z Reads: 168

```
I'm hoping to develop the tests more and more with each revision. But I was initially thinking of having it run through low and high voltage and current scenarios, testing light regen, BLDC and FOC modes. On the inspection side of things we want to develop a list of points that have a high failure rate, like the DRV placement, and inspecting each and every one to make sure it's properly placed and aligned. I'll be talking with the manufacturer about developing these tests further. Also any ideas the community has as to tests they would like to see happen I am more than willing to implement.
```

---
## \#4 Posted by: Michaelinvegas Posted at: 2016-04-11T21:52:47.417Z Reads: 160

```
The reasons I've been holding off...but would be interested in this....
```

---
## \#5 Posted by: evoheyax Posted at: 2016-04-12T00:59:35.185Z Reads: 154

```
I think this is needed. At least, plugging them in to see if they turn on without errors. I won't buy any vesc's from @onloop  again because he doesn't test them and out of 2, 1 was broken on arrival and the other broke 2 days into use. This is why I now buy from @chaka.

The VESC really is the best, if they don't break or arrive broken. But I really don't want to buy it with the way they are being sold from anyone but @chaka.

I think this might help shed more light on why they break so easily. @onloop, you say the real world test is the best way to test eboards, and I think real world tests are crucial, as I would never buy parts or a board without a video of it in use first. But we need someone to invest in testing VESCs to understand more of why they break. From all of the sellers of VESC on here, no one can tell me why when hitting either an amp limit or a heat limit, that my VESC broke and starting giving a UNDER_VOLTAGE fault code. What component is broken, and what really caused it?

This is unknown, because we don't have enough data to correlate certain fault codes with certain actions with the components that broke as a result. This is why we need a scientific approach to testing the VESC under stress to find more about the VESC out, and then vedder can hopefully fix the bugs:
```

---
## \#6 Posted by: willpark16 Posted at: 2016-04-12T01:14:41.593Z Reads: 145

```
i would be if the price was right
```

---
## \#7 Posted by: TheRedPanda Posted at: 2016-04-12T01:24:08.100Z Reads: 142

```
That's a good point, improving our understanding of the vesc through testing could actually speed up development for Vedder by providing him with specific identified bugs.
```

---
## \#8 Posted by: Pantologist Posted at: 2016-04-12T03:53:31.108Z Reads: 136

```
I would be interested in buying tested VESCs as well. Currently, the quality issues with the current suppliers are why I slightly backed off. Hopefully, something like this will improve everyone's product.
```

---
## \#9 Posted by: Ulfberht Posted at: 2016-04-12T05:08:12.465Z Reads: 130

```
Load tested VESC should become the new standard. I would definitely be interested. I would also be interested in the testing process itself.  I would suppose several rigs would need to be built to test VESC under simulated load conditions. Would there be a certification provided?
```

---
## \#10 Posted by: trbt555 Posted at: 2016-04-12T05:11:49.930Z Reads: 133

```
I have always been a strong proponent of load testing.
If you assemble a product that's supposed to be able to handle 50A continuous, I think you need to make sure it does before shipping it.
I believe @chaka already does this and now maybe even @onloop with his US batch but I'm not sure.
```

---
## \#11 Posted by: elkick Posted at: 2016-04-12T05:29:35.498Z Reads: 133

```
I am doing those tests on every single VESC before its shipped over here (esk8.de). That's one of the points which add to the price, but helps with reliability. 

Although, you will never find a test scenario which will cover all possible applications users might use. Including weird motors. They are putting those VESCs in any possible environment you can think of (incl. robotics, eBikes, pedelecs, industrial components, etc.).
```

---
## \#12 Posted by: chaka Posted at: 2016-04-12T13:32:20.410Z Reads: 120

```
I test every VESC twice, the first test is to be sure the bootloader, bldc detection and FOC calibration works as designed. After they are coated and the conformal coating has cured, each controller is load tested with a prop To be sure nothing pops when they take a load for the first time. 

I don't really advertise that I test because in the end I am still going to help out my customers if they blow up their VESC. I highly doubt I would be able to do this if I outsourced manufacturing even if that manufacturer agreed to do load testing. 

The truth is, new people to the sport are going to burn up some gear. If you are not willing to take a little loss every so often with the VESC then you should find something else to turn a profit. All the testing in the world is not going to stop someone from doing a poor installation.
```

---
## \#13 Posted by: longhairedboy Posted at: 2016-04-12T14:00:33.553Z Reads: 111

```
I think isolating problem areas and fixing them and posting about it would be beneficial to the community and generally raise awareness of issues with manufacturers. 

you mentioned bad DRVs. I have a pair of enertion VESCs that both failed at the exact same time and when i had some UCF engineering students check them out they said the DRV chips were both fried, and that was only a month after i bought them. So of course i bought 5 more when the last fire sale pre-order happened. Hopefully i won't have the same results with those. 

but when building for other people i don't have time to wait around for two months so i'll probably end up getting from Ollin or DIY or elsewhere anyway.
```

---
## \#14 Posted by: korryh Posted at: 2016-04-12T16:07:56.526Z Reads: 113

```
I would be in for 3 or so. I haven't had any issues with enertion or chaka but I keep collecting hub motors and don't want to change everything out.
```

---
## \#15 Posted by: TheRedPanda Posted at: 2016-04-13T00:10:01.904Z Reads: 110

```
That's great that you're testing them, I wasn't aware of that!(I like to buy from you currently).
```

---
## \#16 Posted by: TheRedPanda Posted at: 2016-04-13T00:20:41.938Z Reads: 110

```
So it seems like there is definitely interest, but Chaka actually does test his VESCs. 

So I'll still wait and see how these VESCs from my supplier turn out. If it seems like significantly better assembly quality than what I usually see I will likely still offer boards to sell and establish a testing plan. Doesn't hurt to have more VESCs available. 

I'll keep you guys updated!
```

---
## \#17 Posted by: onloop Posted at: 2016-04-13T01:12:49.457Z Reads: 114

```

**Load testing is a great idea! But doesn't guarantee the VESC is failure proof**

On our first three batches we didn't do a load test on all units, only did firmware loading & random selection load testing.

However, the last two batches & the new US manufactured batch was/will be load tested...

However, end users need to understand, load testing is not a guarantee that the end user will have a problem free VESC. Even @chaka who has the "self-proclaimed-best" vesc available still has faulty units that he needs to repair.... Shit happens.

_If anything doing a load test makes it easier for the manufacturer to deny warranty claims..._

At the end of the day, I think the challenge here is, having a warranty & a returns process that can be easily utilised by the end user, whilst minimising the cost for the supplier. Users need to adopt a systematic approach when setting up the vesc and promptly provide evidence that that fault is due to manufacturing so that they can quickly get a refund or replacement if a **manufacturing fault** is confirmed. Some faults are not actually hardware related and it becomes a customer service exercise... which requires resources too. Will you have a support network?

The fact of the matter is, SOME VESC WILL STILL PROBABLY FAIL! (Just like the ESC from hobbyking do).... even more so when considering the various experimental things people are doing with them... 

Such as:
1. Loading new/wrong firmware incorrectly... (this problem seems to be less common now thanks to some firmware warning messages)
2. Running the system with bad settings
3. Stressing the system with poorly designed drive trains (this will kill all ESC's)
4. Basic user error, like shorting it out on the bench.


What I will be interested in most is whether or not using a PCBA factory that adheres to strict IPC-A-610-Class-II PCB manufacturing & assembly standards improves reliability or not... of course I think it will... but the proof is in the pudding.

For those interested, Class II is the general commercial standard: items produced and inspected to IPC-A-610 Class II are deemed to be of high quality suitable for typical commercial applications. This is the standard used for making consumer electronics like mobile phones, cameras & computers. 

The next batch of Enertion VESC, Made in the US, will be the first batch of VESC produced & inspected according to these strict quality guidelines.
```

---
## \#18 Posted by: chaka Posted at: 2016-04-13T01:19:25.008Z Reads: 110

```
Haha! @onloop

I take care of my VESC users and I use quality components, if that makes them the best so be it! 

Glad you are using a US based manufacture, care to divulge the name or are we to just take your word for it? Or are you only having the pcb's manufactured in the US?  The latter seems more likely given the high cost of US based pic and place manufacturing.
```

---
## \#19 Posted by: onloop Posted at: 2016-04-13T01:21:52.655Z Reads: 110

```
[quote="onloop, post:17, topic:2296"]
Some faults are not actually hardware related and it becomes a customer service exercise... which requires resources too. Will you have a support network?
[/quote]

I just checked my user poll, out of 77 votes it seems most (50%) of people just want a lower price, they obviously don't care about service? :frowning:
```

---
## \#20 Posted by: onloop Posted at: 2016-04-13T01:29:06.058Z Reads: 110

```

I may eventually decide to reveal my VESC supplier... just not sure what commercial implications that will have for my business... I am still in talks with them about doing some electric skateboard assembly work, mostly battery & vesc integration/ sub-assembly work for the new next edition of SPACE CELL PRO, so I probably don't want the info public just yet.

But I will say this; The assembly is done 100% in house in US based PCBA factory.

**No bullshit.**

If the public demands proof I can arrange it.
```

---
## \#21 Posted by: onloop Posted at: 2016-04-13T01:35:39.201Z Reads: 105

```
[quote="onloop, post:20, topic:2296"]
If the public demands proof I can arrange it.
[/quote]

you can see in this vlog i am actually talking to the new VESC supplier... i suppose its not 100% proof, but it will have to do for now.

https://www.youtube.com/watch?v=A4UgfqW4oWI&nohtml5=False
```

---
## \#22 Posted by: chaka Posted at: 2016-04-13T01:44:50.207Z Reads: 105

```
At the end of the day all that matters is that you stand behind the product you sell regardless of who makes it. This is why name brand manufactures don't let just any sleaze ball sell their goods. They want to be sure the dealer is taking care of the customer. So, as long as you plan to do that I think you will be fine with this venture you have taken.

Or are you saying that because your VESC's are so cheap that you do not offer any after sale service? Is that what all this noise is about?
```

---
## \#23 Posted by: onloop Posted at: 2016-04-13T02:00:28.458Z Reads: 105

```
[quote="chaka, post:22, topic:2296"]
Or are you saying that because your VESC's are so cheap that you do not offer any after sale service? Is that what all this noise is about?
[/quote]

my VESC mission is; best price, quickest delivery, best warranty & best service :)

Will also probably offer a no hassle, on the spot, replacement warranty for early failure vesc's.. still working on the details for that.
```

---
## \#24 Posted by: TheRedPanda Posted at: 2016-04-13T02:15:43.257Z Reads: 104

```
:scream_cat: @onloop Sorry guys didn't mean to stir things up!
```

---
## \#25 Posted by: chaka Posted at: 2016-04-13T02:19:33.644Z Reads: 103

```
@TheRedPanda  No worries! I think Jason is getting a little touchy about another supplier coming onto the scene. It wasn't long ago that I was his only competition ;)
```

---
## \#26 Posted by: onloop Posted at: 2016-04-13T02:40:28.324Z Reads: 105

```
[quote="chaka, post:25, topic:2296"]
No worries! I think Jason is getting a little touchy about another supplier coming onto the scene. It wasn't long ago that I was his only competition :wink:
[/quote]

haha... :imp:

Actually, I do want more VESC players on the scene....I really, honestly do, I want them to feel the pain of trying to run a small operation, the agony over constant delays, to bath in the insults & abuse that flows onto our screen each day, to carry the burden of everyone's experimental DIY electric skateboard failures like they are your own, the joy of covering the cost to fix everyone's faults even if you had nothing to do with it.. it's a rush...

The truth is, In the long run I'll probably stop selling the VESC as a retail product.

Once people see the quality I am producing & realise they can buy directly from me in small quanitiy at wholesale prices, cheaper than what the china factories can offer, with a reliable warranty & instant delivery.....I suppose I'll just become a wholesaler. They won't have the hassles i mentioned above.

I've done the hard yards with the VESC, I've paved the way & invested over $100K so that the next wave of entrepreneurs can jump on the VESC bandwagon & setup shop to better service the ever increasing demand.... **So I do actually invite this**

[buy now vesc only $76 each in bulk qty](http://www.enertionboards.com/electric-skateboard-parts/vesc-motor-controller/?setCurrencyId=2)

VESC resellers enquire now!!
```

---
## \#27 Posted by: longhairedboy Posted at: 2016-04-13T13:46:25.231Z Reads: 95

```
I think your poll results are reflecting the general sentiment that people in general are tired of waiting around to ride. They didn't want to wait 3 to 6 weeks to get thier VESC in the first place, and if somebody has an inexpensive one they will buy another one rather than look into a warranty claim because they were tired of waiting to ride the first time, and they won't wait a second time for round trip mailings of things. They'd rather replace them at a lower price, and of course buy them in the first place at a lower price. I have a small bin filled with dead ESCs now and i'd love it if i could have one last more than 10 months with zero issues. 

So I'm one of these people. I want the market fucking flooded with VESCs because it will keep the price low and force higher quality in general. I'm tired of waiting on VESCs. I'm tired of fried ESCs in general. I just lost at least one of my 6S FAVs yesterday and i just got that damn rat board built. Its frustrating.
```

---
## \#28 Posted by: barajabali Posted at: 2016-04-13T14:06:09.092Z Reads: 91

```
I would buy one. for a secondary board
```

---
## \#29 Posted by: paragon Posted at: 2016-04-13T14:36:40.392Z Reads: 93

```
I'd buy one or two, but most likely one for now :)
```

---
## \#30 Posted by: evoheyax Posted at: 2016-04-13T17:06:00.993Z Reads: 92

```
> Or are you saying that because your VESC's are so cheap that you do not 
> offer any after sale service? Is that what all this noise is about?

That's pretty much my fuss. I know I did my firmware updates right. I know I am also experimenting, but 90% of people buying VESCs are also experimenting (i.e. not using using only enertion parts with their vesc). So does that mean 90% of people don't deserve to have any recourse when their VESC breaks abruptly, or has issues with low ppm voltage with the only thing having been done before the problem was noticed was a successful firmware update?

> my VESC mission is; best price, quickest delivery, best warranty & best service

The best warranty/service is what @chaka offers. If it breaks, it gets fixed, its that simple. IF you want people to trust the VESC, this is the only way. The reality is that NO, the VESC is not bug free. It seems to me that the vesc still has some bugs. I would be curious as to what the real failure rate of the vesc is, but I would be willing to bet it is quite high (i.s. 40% or higher). Your warranty @onloop is that if you get a VESC, you power it up, and you notice a problem, you can get a refund or replacement. This is hard though, because you'll likely need to configure the vesc in order to test it. In order to configure the vesc, you will likely need to change the firmware. The second you update the firmware, you lose your warranty. So its a catch 22. **Yes, you get a warranty, but what good is the warranty when you can't find the faults covered by the warranty without voiding your warranty?**
```

---
## \#31 Posted by: onloop Posted at: 2016-04-13T22:53:21.283Z Reads: 90

```
[quote="evoheyax, post:30, topic:2296"]
I would be curious as to what the real failure rate of the vesc is, but I would be willing to bet it is quite high (i.s. 40% or higher).
[/quote]

no way man.... if you had a 40% failure rate your business would die nearly instantly....no profit, can't restock, bad reputation, alcoholism etc etc...

Last time I ran the numbers of reported cases of faults & not including the 25 units that got replaced/refunded from my first batch (they had the wrong caps) the figure was 3-4%

You need to understand that I sell lots of vescs! So just because you read a few people who had a vesc problem on this forum it saturates your mind and makes you think they are all bad... last count i sold approx 800 vesc. so maybe 30-35 true faults

There are hundreds of people who never have a problem with the vesc...  Unfortunately Some of them just go pop! It is unknown why... For me 95% of the ones i have blown up is due to my own fuck ups.... shorting, wrong settings, braking parts off... the 5% that have failed on me for unknown reasons equates to maybe just 2 or 3 units total.

Even the vesc god himself aka Chaka can't tell us why it happens, or he just doesn't want anyone to have his top secret information, maybe he will give us his failure rates as well... seems like I'm the only transparent reseller of vesc atm. :slight_smile: :confused:

I am happy with the vesc so far... With my new US based supplier the quality is going to be first class and if there are no faults we can say the all the errors so far are due to manufacturing faults... But i imagine there will still be failures... somethings just fail...

anyway to put this in perspective, before I sold vesc I sold Flier ESC, my last batch from them had a 50% failure rate! thats when I stop selling their ESC
```

---
## \#32 Posted by: onloop Posted at: 2016-04-13T22:59:58.037Z Reads: 87

```
[quote="evoheyax, post:30, topic:2296"]
In order to configure the vesc, you will likely need to change the firmware.
[/quote]

that is not ture....

you don't need to upload new firmware... this where so many people stuff up... (at least now a warning message appears so that you can't easily use the wrong bldc tool/firmware combo)

In many cases the new firmwares don't do that much. Most vesc come with very new firmware preloaded

my advice would be to power the vesc & run a motor detection, if that works you set to go.

If it doesn't work post your result on this forum, if it can't be fixed with settings or new firmware you may have a faulty unit which will get replaced.
```

---
## \#33 Posted by: evoheyax Posted at: 2016-04-13T23:26:47.903Z Reads: 90

```
I have a Mac. When I looked for the tool to configure it, the only one I could find for Mac was for 2.15. I would have to go way out of my way to install a virtual machine or another operating system to get around this, and find one that supports the version 1.14 which mine were shipped with.
```

---
## \#34 Posted by: onloop Posted at: 2016-04-13T23:34:41.685Z Reads: 91

```

unfortunately, the BLDC tool is not backwards compatible, so you need to use the old versions of BLDC tool etc...

available here: www.vesc.net.au
```

---
## \#35 Posted by: TheRedPanda Posted at: 2016-04-14T14:52:52.149Z Reads: 88

```
If you do some digging in the BLDC directory there are older versions you can download actually. It's not super quick to find the exact one but they're all there.
```

---
## \#36 Posted by: akira Posted at: 2016-04-14T15:17:40.817Z Reads: 88

```
@onloop : from all vesc you are selling, what is the fraction which is actually running under a deck and what is the fraction sitting on a desk ... 
Nothing personal, it is just that I have two on my desk for more than a year ...
```

---
## \#37 Posted by: onloop Posted at: 2016-04-14T22:07:02.178Z Reads: 86

```

Honestly, I have no idea.... I don't call all (any) of my customers to ask them how they are doing... however, that would be awesome in terms of customers service level!
```

---
## \#38 Posted by: evoheyax Posted at: 2016-04-16T03:31:29.661Z Reads: 90

```
That is exactly how I feel when you say 3%. I had one sit for 7 months, the other for a few months. I think many have not used them, and of the ones that do and have problems, I wouldn't assume they would all try to contact you. When I said 40%+, I don't mean fail on arrival. I mean, given a year of operation, 40%+ will/have broken. Some are because how people use them, but that also has to be accounted for in the design of the vesc. From a programming stance point, it wouldn't be super hard for example to store the version of pcb being used, and make a button that updates the firmware by http requesting to download the files, extract whats needed, and update the firmware. Would eliminate that part of human error, which I think is one part of design the VESC is lacking. This is just a principle of software design. Always assume your user is an idiot, and try to protect your product from said idiots.
```

---
## \#39 Posted by: korryh Posted at: 2016-04-24T05:10:44.895Z Reads: 80

```
Where are we on this. Just trying to see if I should wait or just buy them now.  Is someone going to be the contact person incase something goes wrong with VESCs.
```

---
## \#41 Posted by: harpie Posted at: 2016-04-24T06:41:30.936Z Reads: 77

```
I dont have my own board or vesc's (yet). Does anyone have an idea what the primary failure mode of the vesc's are? Getting data off of a failed vesc coud help make vesc's more robust.
```

---
## \#42 Posted by: trbt555 Posted at: 2016-04-24T06:50:05.851Z Reads: 76

```
No doubt about it: DRV8302.
```

---
## \#43 Posted by: harpie Posted at: 2016-04-24T07:09:34.266Z Reads: 77

```
Could its failure be caused by spikes on its voltage rail? On first glance I dont see any clamping diodes on the drv's positive terminal. Will have a look at the github files when I have wifi again. 

@onloop send a extra drv chip with every vesc as a repair kit😜. It is a diy hobby after all.

Edit: There is indeed a clamping diode.
```

---
