# Benchwheel remote &amp; receiver

### Replies: 131 Views: 10776

## \#1 Posted by: yaca Posted at: 2016-12-04T18:21:31.614Z Reads: 750

```
I recently got the Benchwheel remote and receiver and want to show some pictures.

<img src="/uploads/db1493/original/3X/4/9/49ac51f74977b655a0db9947aed41059bbbcd9e1.JPG" width="690" height="460">

The inside:

<img src="/uploads/db1493/original/3X/2/5/2526949b215dd610b98df31d109cbbe5061b00c4.JPG" width="690" height="460">

compared to the Winning remote and receiver:

<img src="/uploads/db1493/original/3X/d/c/dc4b0f8ff45d0e35fff5057f3ceb0350f40272c4.JPG" width="690" height="460">

The benchwheel remote has a beginner mode (cruise mode/low speed mode) that means on the VESC display for the break 10% and for throttle 70% instead of 0% and 100% in sport mode/high speed mode.
The receiver has a second connector but I don't know what it is used for. The remote has three LEDs for the battery but only the red bottom shines at full battery!? I just tried the remote for a few minutes, so I don't know if it is reliable so far.
```

---
## \#2 Posted by: Luke Posted at: 2016-12-04T18:49:38.571Z Reads: 668

```
Hey dude, the second channel is just a second "channel 1" so you can actually run 2 vescs from the  1 reciever without needed a split Y cable or a canbus. 
The three indicators that aren't showing are made to show the battery level on a real benchwheel, but since we don't have one it won't show anything. The battery lasts for days. 
Haven't had a dropout or heard of anyone having one, so you should be ok :)
```

---
## \#3 Posted by: SirDiff Posted at: 2016-12-04T19:03:49.160Z Reads: 641

```
How much did you pay them and where did you buy? They seem to cost around 50 euros now :confused: but they may be the best ones out there yet
```

---
## \#4 Posted by: yaca Posted at: 2016-12-04T20:11:08.336Z Reads: 627

```
I bought it from Aliexpress and paid 40,37 Euros. That includes shipping and 5% charge for paypal.
```

---
## \#5 Posted by: saul Posted at: 2016-12-04T20:56:13.154Z Reads: 610

```
I didn't know it was an nrf. can you read the numbers on the rx chip.

this one.. atmega328p maybe?
<img src="/uploads/db1493/original/3X/7/c/7c1eb790c68fc0e1450beb0ef74c4637ea9f228f.JPG" width="690" height="460">
```

---
## \#6 Posted by: yaca Posted at: 2016-12-04T22:06:32.393Z Reads: 572

```
Sorry but on the chip is nothing written on it. On the pcb antenna board the small chip has a number which starts with nrf. Do you need this or isn't useful for you?
```

---
## \#7 Posted by: saul Posted at: 2016-12-05T00:51:01.476Z Reads: 559

```
thanks i was just curious. if its what I think it is it could be "hackable" :sunglasses:
```

---
## \#8 Posted by: themegak Posted at: 2016-12-05T02:20:19.395Z Reads: 553

```
This remote is by far the most reliable remote I've used for esk8 outside of the gt2b.  Always works, never drops signal, battery lasts a long time, fairly compact and has two modes so it makes it a little safer for a friend or someone who wants to try your board feel okay with the speed.
```

---
## \#9 Posted by: Luke Posted at: 2016-12-05T07:51:20.015Z Reads: 534

```
Do you (or anyone) get a high pitched noise every time you use the remote? I do, I got acclimatised to it pretty quick and dont really notice it, but it's certainly making a faint high pitched noise/squeal..
```

---
## \#10 Posted by: yaca Posted at: 2016-12-05T08:39:13.946Z Reads: 521

```
When do you get the noise? When I switch on or off the remote it makes beep but exept of this no noise.
```

---
## \#11 Posted by: Luke Posted at: 2016-12-05T08:58:33.960Z Reads: 522

```
Whenever i send a signal to the vesc.. soo all the time. apart from when I tested it right now now to show you via video.. murphy's law I guess..I 'll film it if I notice it again
```

---
## \#12 Posted by: yaca Posted at: 2016-12-05T18:15:18.903Z Reads: 518

```
I found a chip on the board of the remote which looks similar and has a number on it. Maybe it helps.

<img src="/uploads/db1493/original/3X/4/b/4b18cc711f5c0427e489f60b7e42f9b68dbc9302.JPG" width="690" height="460">
```

---
## \#13 Posted by: saul Posted at: 2016-12-05T18:54:22.714Z Reads: 501

```
thanks it does help with my curiosity.  :nerd:

but sadly not much else... most of the data is in chinese but good to know anyways!
http://www.essemi.com/product/32.html
```

---
## \#14 Posted by: Norco Posted at: 2016-12-10T00:45:09.294Z Reads: 493

```
Just want to check but did you pick up this one? https://www.aliexpress.com/item/Electric-skateboard-refitting-parts-remote-control-bench-technology/32731985084.html?spm=2114.01010208.3.10.IAeWrr&ws_ab_test=searchweb0_0,searchweb201602_3_10065_10068_10084_10083_10080_10082_10081_10060_10061_10062_10056_10055_10054_10059_10099_10078_10079_426_10073_10103_10102_10096_10052_10050_10051-10052,searchweb201603_6&btsid=9e89f31e-449a-47b3-b207-3f93314239a4 

and was it the 4th option (remote and receiver)?

Thanks
Norcs
```

---
## \#15 Posted by: yaca Posted at: 2016-12-10T09:59:21.370Z Reads: 475

```
Yes that's the place where I've ordered the remote. I don't think they have different options but click on the 4th to be sure. The page is full of wrong pictures so you should not calculate on that what you see.
```

---
## \#16 Posted by: Norco Posted at: 2016-12-13T10:43:57.642Z Reads: 472

```
Well that was interesting - I did some late night shopping while in bed last night and ordered a Benchwheel remote and receiver (as per link above) anyway it was late and my wallet was all the way on the other side of the room :sweat: so I thought I'll just pay for it in the morning. I way up to a message from the Ali App telling me that there had been a price adjustment. Expecting it to be a few pence different due to currency fluctuations I log in to pay and it has dropped by £5! Happy days. £32 inc delivery ($40.60 or 38e)
```

---
## \#17 Posted by: darkkevind Posted at: 2016-12-14T15:28:37.635Z Reads: 462

```
Hi guys, anyone know if you can pair this remote with a standard 2.4gz receiver?

I've just received mine, thought I ordered remote & rec but only received the remote...
```

---
## \#18 Posted by: Norco Posted at: 2016-12-14T17:28:27.809Z Reads: 449

```
I almost made the same mistake but selected the 4th option (furthest to the right). Hopefully a receiver will turn up too. I'll be complaining if not. Does it say on your order Remote and Receiver?
```

---
## \#19 Posted by: darkkevind Posted at: 2016-12-14T17:58:43.878Z Reads: 444

```
Hmm can't see anything saying receiver, but I'm 98% sure I chose remote & rec.
```

---
## \#20 Posted by: yaca Posted at: 2016-12-14T19:08:43.570Z Reads: 446

```
You can see what you ordered in your account from Aliexpress - "My orders". In my case it says "remote and receiver". I don't know if other receivers work. For example the Winning remote works with the GT2B receiver but usually different brands don't work together. I would order an original receiver from the seller of the remote.
```

---
## \#21 Posted by: Norco Posted at: 2016-12-14T20:01:45.239Z Reads: 398

```
Yes mine definitely says remote and receiver. Will update when it arrives.
```

---
## \#22 Posted by: darkkevind Posted at: 2016-12-14T20:25:18.422Z Reads: 400

```
Hmmm, mine doesn't :frowning:

Maybe I did cock up :rolling_eyes:
```

---
## \#23 Posted by: korryh Posted at: 2016-12-15T00:30:21.098Z Reads: 392

```
I ordered one as well but just received the transmitter.  I checked my order and it was for both Tx and Rx, I emailed and instead of shipping the Rx they gave me my money back and said keep the Tx.  Anyone know where I can get a receiver.
```

---
## \#24 Posted by: yaca Posted at: 2016-12-15T09:52:24.666Z Reads: 380

```
What was the answer from Benchwheel. Do they have receivers in stock?
```

---
## \#25 Posted by: JullianS Posted at: 2016-12-15T10:15:47.843Z Reads: 371

```
I got one and it is super nice, the throttle is smooth, and it feels more solid than the Winning.

Bought the DIY Kit with Rx+Tx.
```

---
## \#27 Posted by: Norco Posted at: 2016-12-15T10:57:56.606Z Reads: 373

```
Do you have a link to the one that you bought so that we can see if it is the same one. Doesn't fill me with confidence that 2 people above have both not received a receiver (even though my order explicitly says Remote + Receiver). I suppose if they refund and you can find a receiver that will work with it then you'll be well in front. Not sure how you could check compatibility though - I guess its more complicated than just both being 2.4Ghz?
```

---
## \#28 Posted by: yaca Posted at: 2016-12-15T11:26:37.867Z Reads: 364

```
Contact the seller and he will give you the answer what he sent to you. He answered always pretty fast.
```

---
## \#29 Posted by: korryh Posted at: 2016-12-15T14:57:57.160Z Reads: 353

```
They apologized and said due to stock restrictions we returned your money. They were very nice about it.
```

---
## \#30 Posted by: darkkevind Posted at: 2016-12-15T16:45:11.215Z Reads: 351

```
They contacted me. Turns out I did just order the remote (shmuck!), but said if I pay just $14 more through paypal then they'd send me a receiver too...

So I did...

I'll just wait to see if that turns up.....................................
```

---
## \#31 Posted by: JullianS Posted at: 2016-12-16T04:26:16.422Z Reads: 340

```
Ordered it through Taobao, I live in China :sunglasses:
```

---
## \#32 Posted by: Norco Posted at: 2016-12-29T12:06:20.318Z Reads: 337

```
So my benchwheel has arrived and I can confirm it came with a receiver. Remote seems doa though. Will try and charge it now but no leds are lighting up on power press and there is an ominous rattle from inside the remote.
```

---
## \#33 Posted by: Norco Posted at: 2016-12-29T12:07:25.160Z Reads: 327

```
Must add though that if it works this will be a winner. Comfortable to hold and nice feel to the thumb control.
```

---
## \#34 Posted by: darkkevind Posted at: 2016-12-29T20:29:42.737Z Reads: 322

```
Mine was dead. Took a long time to charge first time but was OK after that.
```

---
## \#35 Posted by: Norco Posted at: 2016-12-29T21:51:05.742Z Reads: 319

```
New report. It's alive! Charged and seems to work. Won't know for sure until I can power up the receiver and VESC and test it. Will probably take apart at some point and investigate the rattling. Happy so far.
```

---
## \#36 Posted by: darkkevind Posted at: 2016-12-30T10:51:45.195Z Reads: 319

```
Good work.

On my side, I was told that the receiver could not be paired with the remote I had once it had left their factory, so getting a separate receiver is not an option. Makes you wonder why they sell them separately in the first place!!!

I have to send my remote back and order both together! :frowning:

I won't do that now though because my board accident (where I popped my knee sideways) has put me out of action for the next 6-8 weeks! :frowning:
```

---
## \#37 Posted by: Norco Posted at: 2016-12-30T22:46:59.452Z Reads: 310

```
Ouch - That sounds nasty and at Christmas time too! Hope you have a quick recovery. 

That is a strange one. I assume that this means that the one I have will be already paired. Hopefully so as the instructions are terrible otherwise.

The receiver looks pretty simple so hopefully plug and play once the VESC arrives.
```

---
## \#38 Posted by: darkkevind Posted at: 2016-12-31T00:31:27.080Z Reads: 327

```
It was pretty nasty, found myself breathing through the pain on the pavement/sidewalk like Peter Griffin! Lol. Managed to haul my ass up on my board to sit on it to ride it home. Lucky I was just round the corner...
There was, and is, a lot of pain... sprained a ligament. 

Yeah your remote and receiver will definitely be pre-paired, no worries about that... happy boarding!
```

---
## \#39 Posted by: yaca Posted at: 2017-01-01T13:00:52.804Z Reads: 341

```
[quote="darkkevind, post:36, topic:14171"]
I was told that the receiver could not be paired with the remote I had once it had left their factory, so getting a separate receiver is not an option.
[/quote]

So why do they describe the pairing in the manual? When I received mine I did the pairing, maybe it wasn't necessary.

<img src="/uploads/db1493/original/3X/2/a/2ac0073ed1ad075b36175ece980f46fa230c862d.JPG" width="690" height="460">
```

---
## \#40 Posted by: darkkevind Posted at: 2017-01-02T09:43:51.898Z Reads: 326

```
Well that's annoying! :unamused:
```

---
## \#41 Posted by: ekitesurfer Posted at: 2017-01-02T10:35:19.277Z Reads: 322

```
I ordered one of these things from aliexpress and it came without a receiver after about a month.... I ordered a couple from MEB, got them a couple days later, one quit working after I switched into slow mode and they replaced it quickly. Besides the one that quit working after switching to slow mode, I haven't had any drop outs. When you first get one of these remotes play with it and make sure the throttle is not sticking. The other day after getting my new remote I turned my board on and started rolling downhill on it, then I hit the power button on the remote and busted my ass because the throttle was stuck on full. I opened up the remote, shaved off a tiny bit of plastic and it wont happen again....
```

---
## \#42 Posted by: AbdeTy Posted at: 2017-01-02T10:59:02.064Z Reads: 304

```
i got one as well then our customs asked me for a CE certificate like if i am importing a military radar, fucking assholes , thanks god i got a  wii nunchuck or i would of been stuck with a board and no remote lol
```

---
## \#43 Posted by: leroy Posted at: 2017-01-02T11:31:32.608Z Reads: 293

```
That cat down in Miami sells these, I got one from him.

http://miamicustomboardshop.com
he's cool
```

---
## \#44 Posted by: ekitesurfer Posted at: 2017-01-02T16:07:42.336Z Reads: 299

```
MEB = miamielectricboards.com. Those guys stood behind their remote and fixed the problem ASAP. Why roll the dice and order from China with a month wait, when you can support an (hopefully) American, get what you ordered in a couple days, and have a warranty? Best remote, best vendor for it imo...
```

---
## \#45 Posted by: leroy Posted at: 2017-01-04T21:27:13.648Z Reads: 285

```
I bought stuff from miami,
he was great to deal with and a huge help.
```

---
## \#46 Posted by: Bender Posted at: 2017-01-22T04:13:35.815Z Reads: 288

```
Can anyone post the manual?

I cannot get the reciever to work.
The remote seems fine charges lights up, ect.
But I can't get the reciever to light up or pair or do anything.
Tried both channels still nothing
```

---
## \#47 Posted by: yaca Posted at: 2017-01-22T19:11:08.544Z Reads: 294

```
<img src="/uploads/db1493/original/3X/5/d/5d0dae16615e9128768c4729531aa36e3d10f947.jpg" width="363" height="500">
```

---
## \#48 Posted by: mccloed Posted at: 2017-01-22T21:17:54.256Z Reads: 284

```
The manual that @yaca posted does not show this, but I messed around with the two buttons on the receiver (pressed them both at the same time) and was able to bring a receiver back to life.
```

---
## \#49 Posted by: yaca Posted at: 2017-01-22T23:02:26.604Z Reads: 280

```
[quote="mccloed, post:48, topic:14171"]
I messed around with the two buttons on the receiver
[/quote]

your receiver has two buttons? Mine has only one.
```

---
## \#50 Posted by: Norco Posted at: 2017-01-22T23:20:30.642Z Reads: 268

```
Mine only has one if it makes you feel any better. Not tried it yet though so can't say if it is working or not.
```

---
## \#51 Posted by: mccloed Posted at: 2017-01-23T01:56:02.287Z Reads: 260

```
Dammit! It is only one botton. I was thinking of something else. I held the one button down while trying to bind when nothing else worked.
```

---
## \#52 Posted by: mt37 Posted at: 2017-02-03T21:43:50.903Z Reads: 246

```
Yep I did the same thing, and they insist it's my fault..

How is it that multiple people make the same mistake but they do not question their process ?
```

---
## \#53 Posted by: yaca Posted at: 2017-02-22T20:45:05.953Z Reads: 239

```
Just want to know if the LED of your receivers also has a undefined blue flashing or is it a constant blue light? Thanks!
```

---
## \#54 Posted by: mt37 Posted at: 2017-02-23T00:37:12.495Z Reads: 246

```
Is anyone interested in reverse engineering the Benchwheel remote ?

I'm pretty sure it would be possible to graft an arduino nano and some xbee chip if we could figure out what the remote board sends to the Benchwheel "transmitter daughter card"
```

---
## \#55 Posted by: mmaner Posted at: 2017-02-23T00:44:56.740Z Reads: 242

```
I've got a Benchwheel I could take the RX out while connected and measure it, if you wanna tell me how to do said measurement.
```

---
## \#56 Posted by: mt37 Posted at: 2017-02-23T00:47:28.546Z Reads: 250

```
I frankly have no idea how to reverse engineer such protocol. I just have the intuition that it can't be that hard. 
I imagine you'd need to have a logic analyzer such as this [1]. Or at the very least an oscilloscope.

[1] https://www.saleae.com/
```

---
## \#57 Posted by: yaca Posted at: 2017-02-23T12:39:25.899Z Reads: 251

```
Nobody can give me an answer?
```

---
## \#58 Posted by: amc Posted at: 2017-03-02T15:15:02.724Z Reads: 258

```
Hey all!

Is there any shop out there that sells these except aliexpress and can ship globally? With the reciever included?

Thanks!
```

---
## \#59 Posted by: kptheinventor Posted at: 2017-03-02T22:13:38.007Z Reads: 257

```
@amc  https://electric-skateboard.market/product/small-handheld-remote/ Although global shipping on these are pretty expensive
```

---
## \#60 Posted by: mt37 Posted at: 2017-03-15T21:22:47.206Z Reads: 250

```
I just bought one of the cheapest logic analyzer on ebay that is compatible with this program [1]
$6 for 8 channel, 24mhz logic analyzer. Not bad!

Hopefully this will be enough for me to rewire the benchwheel remote with Arduino nano + xbee transmitter / receiver.

[1] http://sigrok.org/wiki/Supported_hardware#Logic_analyzers
```

---
## \#61 Posted by: Norco Posted at: 2017-04-11T20:51:28.865Z Reads: 240

```
Does anyone know if you can take 5v from the spare 3 pins? Need a 5v from somewhere to power a battery voltage display and this seems a simple way to do it if it works?
```

---
## \#62 Posted by: yaca Posted at: 2017-04-11T21:07:02.080Z Reads: 230

```
My multimeter says 0V at the second pins. I don't know for what those pins are used for.
```

---
## \#63 Posted by: Norco Posted at: 2017-04-11T21:52:45.105Z Reads: 233

```
OK thanks for checking for me @yaca

I have a feeling  they are going to be for a second VESC. 

I'll have to find my 5v elsewhere.
```

---
## \#64 Posted by: Skateman Posted at: 2017-04-12T00:20:21.490Z Reads: 244

```
Here are 2 pics of Benchwheel receiver with the middle row pins solder bridged together. (excuse my solder bridge, not to pretty, but worked) This connects 5vdc to the next row. Supposedly, this row is channel 2. (not marked)  Not sure what the red marks are for on component side. I did this to get 5vdc for an exhaust fan. It worked fine. I'm still looking for that all allusive channel 2. Not sure it works like that though. But it will work for 5vdc. Trace out the traces and use a volt/ohm meter to understand what's going on. Good luck. 



  <img src="/uploads/db1493/original/3X/a/f/af808874bc394efe24ae38053efc087cf9a853ac.JPG" width="375" height="500">


<img src="/uploads/db1493/original/3X/e/c/ec01a386f1484b7bf9525cacb09df559836ae16d.JPG" width="375" height="500">
```

---
## \#65 Posted by: Norco Posted at: 2017-04-12T06:44:40.684Z Reads: 232

```
Great stuff. That looks like a good way to sort it.
```

---
## \#66 Posted by: lowGuido Posted at: 2017-05-17T03:39:59.527Z Reads: 219

```
are these benchweel remote and receivers still out there?? 
I bought one a while back and was looking to get another and when I went looking I could only find the remote by itself without receiver :frowning:
```

---
## \#67 Posted by: Tomer Posted at: 2017-05-17T04:49:31.638Z Reads: 215

```
It seems that the remote + reciver is currently out of stock. 
I have contacted the seller to understand if he will sell more in the future.
I'll update you accordingly.
```

---
## \#68 Posted by: Jinra Posted at: 2017-05-17T05:28:52.793Z Reads: 214

```
It goes in and out of stock on aliexpress. Luckily, I stocked up on a few ;)
```

---
## \#69 Posted by: Tomer Posted at: 2017-05-17T10:03:13.103Z Reads: 219

```
Benchwheel respond: "It's out of stock now. It'll take a few days".

Hope that helps.
```

---
## \#70 Posted by: ACIN Posted at: 2017-05-17T11:23:00.150Z Reads: 216

```
But running dual VESC's parallel on one receiver will mess up your traction in sharp turns right? I'm not sure what the BLDC tool really does when you configured the canbus connection, I always thought it lets the motors spin at different speeds (to certain programmable erpm limit).
```

---
## \#71 Posted by: mmaner Posted at: 2017-05-17T13:33:05.703Z Reads: 214

```
You can turn on traction control if you are using a CAN bus connection between VESC's.  In a practical sense, I can see no performance difference between traction control with a CAN bus and splitting the RX cable to 2 VESC's.  I actually tested the hell out of it :slight_smile: .

I used 1 board with the same VESC's, battery pack, batteries, wheels...everything.  I did a 5 mile ride with traction control along a predetermined path.  The next day I did the same exact path using roughly the same speeds, using a split RX lead instead of traction control. There was no performance or battery discharge difference.

I still prefer the CAN bus, that way you can write both VESC's via bluetooth using @Ackmaniac F/W.
```

---
## \#72 Posted by: Mark Posted at: 2017-05-26T09:29:41.303Z Reads: 202

```
Is anyone having problems with the receiver? They tend to break quickly
```

---
## \#73 Posted by: Okami Posted at: 2017-05-26T11:04:39.103Z Reads: 207

```
Got more info on that?.. Sucks ass, if there is a problem with more than 1 benchwheel remote
```

---
## \#74 Posted by: squad Posted at: 2017-05-26T11:18:08.254Z Reads: 207

```
I had to resolder 2,4Ghz module to the main board, I believe this may be the issue.
```

---
## \#75 Posted by: trancejunkiexxl Posted at: 2017-06-01T01:10:35.771Z Reads: 204

```
posted about benchwheel remote also!!! its alfull ditch it.. I was going to suggest the nano clones but am having issues now so cant suggest it anymore
```

---
## \#76 Posted by: Jinra Posted at: 2017-06-01T01:12:31.890Z Reads: 204

```
I've used 4 remotes, none of which gave my any problems
```

---
## \#77 Posted by: Mark Posted at: 2017-06-01T06:57:22.199Z Reads: 205

```
Receivers going fatal after connecting at full voltage. Factory says its not theyre fault but I got 3 dead receivers
```

---
## \#78 Posted by: sandrewvdv Posted at: 2017-06-01T09:44:31.339Z Reads: 209

```
What do they mean, full voltage? My battery is 6s. How can this not be their fault?
```

---
## \#79 Posted by: tueboard Posted at: 2017-06-01T09:45:32.707Z Reads: 207

```
i broke one benchwheel receiver, by mistake i bought one controller without the receiver, so i have 2 useless controllers.

i don't know why they sell the controller without the receiver, but they don't sell only the receiver...
```

---
## \#80 Posted by: darkkevind Posted at: 2017-06-01T12:12:16.594Z Reads: 204

```
My receiver stopped working after the first connection!

BW have sent me a new one though as I went back to them and complained...
```

---
## \#81 Posted by: yaca Posted at: 2017-06-01T12:40:27.651Z Reads: 201

```
What do you mean with full voltage? It has always to be 5 volts, normally it's coming from the the esc.
```

---
## \#82 Posted by: Mark Posted at: 2017-06-02T18:52:43.893Z Reads: 185

```
I have bought a batch of 10 remotes. Now 4 receivers went fatal. I'm trying to fix it but BW wont cooperate.... thats what you call shitty service
```

---
## \#83 Posted by: SirDiff Posted at: 2017-06-02T18:54:54.511Z Reads: 185

```
Wow that's kinda strange. Maybe bad batch for them? I noticed the receiver image on alibaba is different from the one I have, they may have changed something
```

---
## \#84 Posted by: Jinra Posted at: 2017-06-02T18:56:37.806Z Reads: 182

```
alibaba/express receiver is the old style. Everyone should be getting the squarer new style as of half a year (or more) ago.
```

---
## \#85 Posted by: fraannk Posted at: 2017-06-07T16:20:29.204Z Reads: 184

```
I bought one from @Mark's batch a while ago and it still works fine. What happens when the receiver breaks? Runaway board? Or does it just coast?
```

---
## \#86 Posted by: Jinra Posted at: 2017-06-07T16:45:23.255Z Reads: 184

```
Depends on your VESC settings. You could have it brake when it doesn't receive PPM signal.
```

---
## \#87 Posted by: fraannk Posted at: 2017-06-07T16:56:46.545Z Reads: 182

```
Would it be the same reaction as when turning the remote off?
```

---
## \#88 Posted by: Mark Posted at: 2017-06-07T20:36:19.706Z Reads: 174

```
Yes definitly, if you set up the vesc right
```

---
## \#89 Posted by: fraannk Posted at: 2017-06-07T21:03:40.675Z Reads: 177

```
Okay, I've set the timeout low, and when I turn off the remote it coasts. So I hope it does the same when/if failing :P
```

---
## \#90 Posted by: rok Posted at: 2017-06-07T22:30:44.526Z Reads: 179

```
I also almost ordered just the remote but there are actually two ads on aliexpress, one with both reciever and remote and one with just the reciever, so choose wisely :wink:
Still waiting for my tho.
```

---
## \#91 Posted by: rok Posted at: 2017-06-14T06:36:35.369Z Reads: 174

```
I recieved remote and reciever today, everything seems to be working good, altough the reciever is a little bit different than the photo in the ad shows.
```

---
## \#92 Posted by: yaca Posted at: 2017-06-14T08:00:54.356Z Reads: 167

```
They just didn't change the picture. It's the same receiver as shown here in the first post?
```

---
## \#93 Posted by: rok Posted at: 2017-06-14T08:21:41.331Z Reads: 165

```
Yes, true that, my bad!
```

---
## \#94 Posted by: Tomer Posted at: 2017-06-15T08:26:47.753Z Reads: 172

```
I just received my Benchwheel remote & receiver. This thing is so hard to sync... 
Anyways, when I push the throttle half way, nothing happens. But when I push it more than half way, the motor runs immediately at max speed. I don't have the ability to control the speed by just pushing the throttle a bit. Does anyone knows why? Is it how this remote works? maybe it is defective? Maybe my VESC settings are wrong?
```

---
## \#95 Posted by: mmaner Posted at: 2017-06-15T13:32:04.451Z Reads: 170

```
You need to setup the PPM parameters

http://www.electric-skateboard.builders/t/vesc-ppm-settings/526
```

---
## \#96 Posted by: Tomer Posted at: 2017-06-15T13:50:27.601Z Reads: 167

```
I tried to play with the PPM, but for some reason the remote doesn't like it when I am changing the default parameters (min Pulsewidth - 1.00, max Pulsewidth - 2.00). When I changed those values, the remote didn't respond at all. When I rolled back to default parameters it got back to working state.

I will be near it in a few hours and I'll post my BLDC setup as well as the results that I receive with them.
```

---
## \#97 Posted by: mmaner Posted at: 2017-06-15T14:04:13.807Z Reads: 166

```
Make sure you have the remote in "Full Power" mode when altering PPM settings.  

1. power off the remote
2. power on the remote
3. short press the power button

It should change from Low to High or High to Low.  You want it on High when adjusting PPM Settings.
```

---
## \#98 Posted by: Tomer Posted at: 2017-06-15T15:02:37.948Z Reads: 166

```
When I short press the power button, it stays on Low power mode. Is something wrong with the sync perhaps?
```

---
## \#99 Posted by: mmaner Posted at: 2017-06-15T15:29:59.916Z Reads: 169

```
That function takes place in the remote, so at least that's not a sync issue.  You have to set the power mode as the first action, you cant hit the throttle or anything before.
```

---
## \#100 Posted by: Tomer Posted at: 2017-06-15T20:11:21.665Z Reads: 185

```
You are correct, I am able to switch modes now.

I tried [this guy's video](https://www.youtube.com/watch?time_continue=3&v=OtuofrQr3F8) on how to set the PPM, unfortunately it didn't help me. 
I would like to share with you my results;

My Maximum Pulsewidth (ms) is set to 1.95 and the Minimum Pulsewidth is set to 1.10. 
The motor still starts at max speed. Here's a video to demonstrate it.

https://www.youtube.com/watch?v=p1GJbx_VKNU

Another thing is that my motor spins at the wrong direction, it goes backwards instead of forward.

https://www.youtube.com/watch?v=RxrXlQG8IRM

It also fluttering and makes strange noises. I tried to release a bit the nut on the wheel where's the motor, but it didn't make any difference.

Another thing - I am not able to stand on it and ride, the motor just can't handle it.

https://www.youtube.com/watch?v=Lb-kgiMr4oU

----------
Here are my VESC settings: 

## Motor values

<img src="/uploads/db1493/original/3X/0/5/05ed3798daa209534fd04fd76788e03d8594f0bc.png" width="690" height="379">

## BLDC values

<img src="/uploads/db1493/original/3X/d/7/d7ac2e8107f8bf53ef38e84149dc732ee53af70c.png" width="690" height="379">

## General values
<img src="/uploads/db1493/original/3X/4/e/4e558a00980e0352680d204ed2caaa08b7dc8658.png" width="690" height="379">

## PPM values

<img src="/uploads/db1493/original/3X/9/0/90a78a76f87793b6bb7b5ef38e1c8e1e1bf147d2.png" width="690" height="379">

My battery is ACTON's Blink board battery which I believe is 10s1p 42V. The motor is also from this board and I have no idea what are the motor specs. I am using Maytech VESC.

Many, many thanks...
```

---
## \#101 Posted by: mmaner Posted at: 2017-06-15T20:31:28.824Z Reads: 177

```
I see where you did the motor detection, but you didn't apply it & save.  Try doing that and see if it helps.  Also, you need to have a load on the board when testing, testing on the bench will not show you the actually AMP/Voltage delivery under load so it looks like it spins at 100% when in reality it doesn't.

Lastly, I would use a multimeter to find out the voltage of the battery for sure before I went any further.
```

---
## \#102 Posted by: Tomer Posted at: 2017-06-15T20:42:18.801Z Reads: 181

```
I tested the battery in the past, here are the results.

<img src="/uploads/db1493/original/3X/9/b/9ba9b4657093e93df1c8698bcc958ba5a7f58c26.jpg" width="375" height="500">

What do you mean by "you did the motor detection, but you didn't apply it & save"?
So you also suggest to raise the motor max higher then 60amp?
```

---
## \#103 Posted by: mmaner Posted at: 2017-06-15T21:06:27.066Z Reads: 179

```
if you look at your BLDC values pic in the Detect Parameters section you will see...
<img src="/uploads/db1493/original/3X/0/c/0c1fc04550a5736cad8f442cc8f0218f531e7b2a.png" width="504" height="137">

But in the Sensorless section those values have not been applied...
<img src="/uploads/db1493/original/3X/e/7/e7c2a5e2ce0db20b3d49d657c778496fb348712b.png" width="546" height="174">

I would leave the Current Limits as they are, you might lower the Batt Min to -15 until you can test the breaks, but they look fine.
```

---
## \#104 Posted by: Tomer Posted at: 2017-06-15T21:19:06.016Z Reads: 170

```
Great info right there, didn't know I was supposed to press the Apply button. Done, thank you.

I will keep with the motor load testing tomorrow, but for now, do you know what's wrong with the remote settings?
```

---
## \#105 Posted by: mmaner Posted at: 2017-06-15T22:03:26.197Z Reads: 169

```
Your PPM tab looks fine to me, it may just be that you need to test it with a load on the board with the power settings correct on the remote.  Id try it and see what it does.
```

---
## \#106 Posted by: on1y Posted at: 2017-07-08T17:13:42.121Z Reads: 158

```
Ur motor spins backwards because ur 3 phase wires aren't in correct order. Switch 2 of them up until it spins correctly. Also ur battery cutoff levels need to be changed to 30 and 28 for 10s
```

---
## \#107 Posted by: SBMTB Posted at: 2017-07-26T02:17:51.369Z Reads: 149

```
Same as darkkevind 15min or so...:disappointed: no other backup for the moment
```

---
## \#108 Posted by: tueboard Posted at: 2017-09-14T09:12:22.458Z Reads: 133

```
a little offtopic... but it seems that benchwheel won't sell the remote and receiver anymore

<img src="/uploads/db1493/original/3X/8/8/88cc1e32e629bf5ca3a6e64738d2b88c828b3217.png" width="690" height="270">
```

---
## \#109 Posted by: Nordle Posted at: 2017-09-14T10:30:29.511Z Reads: 136

```
https://www.aliexpress.com/item/Electric-skateboard-refitting-parts-remote-control-bench-technology/32731985084.html?spm=a2g0s.13010208.99999999.314.UGJnhA
```

---
## \#110 Posted by: tueboard Posted at: 2017-09-14T10:47:16.162Z Reads: 136

```
they don't sell the receiver apart...
```

---
## \#111 Posted by: Nordle Posted at: 2017-09-14T10:50:38.941Z Reads: 142

```
Ok, i somehow doubt it's both. my fail^^
```

---
## \#112 Posted by: louwii Posted at: 2017-11-17T07:12:38.444Z Reads: 124

```
It's back in stock. I just ordered one.

https://www.aliexpress.com/item/Electric-skateboard-refitting-parts-DIY-800MAH-remote-receiver-2-4G-bench-technology-benchwheel/32791243047.html
```

---
## \#113 Posted by: darkkevind Posted at: 2017-11-17T09:20:59.067Z Reads: 119

```
Thanks! Just ordered one! 😁
```

---
## \#114 Posted by: Nitsudo Posted at: 2017-11-25T03:17:05.571Z Reads: 113

```
Is the battery soldered onto the board or connected with a connector?
```

---
## \#115 Posted by: yaca Posted at: 2017-11-25T09:31:52.426Z Reads: 114

```
You can see it on a foto in the first post here. It is soldered.
```

---
## \#116 Posted by: louwii Posted at: 2018-01-31T17:26:49.453Z Reads: 110

```
Benchwheel remote users, I tried mine and it has a dead zone on acceleration. No big deal, though, I have to get used to it.

I was wondering if you guys have that dead zone too.

I looked in the Vesc tool, and I confirm that it's coming from the remote. There's just nothing happening when pushing the thumb joystick (or whatever it's called), up to a certain point.

Also, I was wondering if it's possible to make the battery indicator working using some soldering, like it is on the Maytech remote http://www.electric-skateboard.builders/t/new-maytech-mtskr1712-remote-receiver-42-shipping/26981/23?u=louwii Could be useful.
```

---
## \#117 Posted by: Surfer Posted at: 2018-01-31T17:46:17.394Z Reads: 110

```
You can change the dead zone in vesc tool, the default setting is 15% try with 5%
```

---
## \#118 Posted by: louwii Posted at: 2018-02-01T07:51:49.770Z Reads: 109

```
Thanks à lot, that did help. I went down to 2%, still have a dead zone but it's way better
```

---
## \#119 Posted by: Minim Posted at: 2018-04-10T22:08:39.882Z Reads: 96

```
I'm split between this and a photon remote but is it even possible to get these anymore?
```

---
## \#120 Posted by: sanrory Posted at: 2018-07-16T13:58:38.517Z Reads: 80

```
I'm also having issues with the remote. Compared to the winning, lots of delay when accelerating and braking. Really quite scary and dangerous. 

Tweaked all the settings around deadband etc and no luck. Exact same settings on winning were amazing. 

Any ideas?
```

---
## \#121 Posted by: Skunk Posted at: 2018-08-14T06:31:55.012Z Reads: 68

```
Anyone know where to buy just the receiver? got my benchwheel today and it didn't come with one, could have sworn it said it did in the eBay listing and it was in the photo.
```

---
## \#122 Posted by: Andy87 Posted at: 2018-08-14T07:13:57.128Z Reads: 67

```
https://www.electric-skateboard.builders/t/benchwheel-remote-receiver/14171/30?u=andy87

Looks like not only you had this problem.
```

---
## \#123 Posted by: Skunk Posted at: 2018-08-14T07:22:33.994Z Reads: 63

```
[quote="darkkevind, post:36, topic:14171"]
I have to send my remote back and order both together! :frowning:
[/quote]

Balls.... that's lame. 
Is there really no way around this
```

---
## \#124 Posted by: darkkevind Posted at: 2018-08-14T08:37:18.129Z Reads: 66

```
Yeah apparently that have to be ordered together!

But they've stopped selling this remote and receiver now :frowning:
```

---
## \#125 Posted by: Skunk Posted at: 2018-08-14T08:41:18.180Z Reads: 67

```
Sooo I'm SOL...... cool.
And you would have a different controller they would recommend
```

---
## \#126 Posted by: Skunk Posted at: 2018-08-14T10:22:50.072Z Reads: 64

```
I guess I'll try contacting the seller and returning. Only took like 4 weeks delivery from China.
 I'm probably going to go with an alternative remote from an American seller seeing I plan on starting to put my deck together in about 2 weeks.
```

---
## \#127 Posted by: rok Posted at: 2018-08-14T11:01:42.579Z Reads: 64

```
I have a spare reciever if you want but idk if they can be paired with just any remote. If you want i can send it to you with you just paying for shipping. Where are you from?
```

---
## \#128 Posted by: Skunk Posted at: 2018-08-14T11:04:56.616Z Reads: 64

```
USA @rok 
I'd be willing to try
Thanks man.
```

---
## \#129 Posted by: rok Posted at: 2018-08-14T11:10:25.174Z Reads: 69

```
Ok, i will pm you in about a week because i'm on holidays atm.
```

---
## \#130 Posted by: Allofyoush Posted at: 2019-01-10T04:23:16.565Z Reads: 38

```
I checked the Aliexpress link, but the Benchwheel remote is no longer available. Where does one find one with the receiver for cheap now?
```

---
## \#131 Posted by: Andy87 Posted at: 2019-01-10T07:50:17.194Z Reads: 39

```
https://www.ebay.co.uk/i/282956035811?chn=ps&ul_ref=https%253A%252F%252Frover.ebay.com%252Frover%252F1%252F710-134428-41853-0%252F2%253Fmpre%253Dhttps%25253A%25252F%25252Fwww.ebay.co.uk%25252Fi%25252F282956035811%25253Fchn%25253Dps%2526itemid%253D282956035811%2526targetid%253D522579819983%2526device%253Dm%2526adtype%253Dpla%2526googleloc%253D2826%2526poi%253D%2526campaignid%253D1593678467%2526adgroupid%253D67072923984%2526rlsatarget%253Dpla-522579819983%2526abcId%253D1139126%2526merchantid%253D6995734%2526gclid%253DCj0KCQiA1NbhBRCBARIsAKOTmUtRJDt-p1dx65qiGhgxmJ9JRFKyofJwhAfOKzOLGqjq8dFe5MSZMXMaAmk1EALw_wcB%2526srcrot%253D710-134428-41853-0%2526rvr_id%253D1814059532352%2526rvr_ts%253D36bc96291680ab446dd51bbdffc1cac9

Google is your friend...(sometimes)
```

---
## \#132 Posted by: Allofyoush Posted at: 2019-01-10T08:02:22.897Z Reads: 36

```
Well, it actually seems like Benchwheel sells them directly.
https://www.benchwheel.com/collections/patrs/products/diy-remote-receiver?variant=7507694026811
```

---
