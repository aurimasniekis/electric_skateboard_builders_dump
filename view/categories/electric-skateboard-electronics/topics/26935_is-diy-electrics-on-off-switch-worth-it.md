# Is DIY Electric&rsquo;s On/Off switch worth it?

### Replies: 40 Views: 3033

## \#1 Posted by: TSThunder Posted at: 2017-07-06T21:20:00.336Z Reads: 292

```
So I was planning to buy DIY electric's on/off switch, but I am pretty hesitant after reading reviews about failures shortly after installation. Is there anyone who has had the switch work well for them? 

Also, if anyone has a different On/Off switch, please link it to me because I don't want to spend $60 on something that will last 10 seconds. Thank you!
```

---
## \#2 Posted by: JLabs Posted at: 2017-07-06T21:22:36.505Z Reads: 291

```
@JdogAwesome is going to have some in a week or two I think! Custom made and reliable from the review.
```

---
## \#3 Posted by: Jinra Posted at: 2017-07-06T21:22:48.694Z Reads: 291

```
I have the DIYES switch. Bought it used for $40. Been nearly a year and hasn't failed on me so far. I'm running 10s dual 6355's.
```

---
## \#4 Posted by: flywithgriff Posted at: 2017-07-06T21:25:49.320Z Reads: 281

```
I have run a MEB switch on my 6s build for months and never had an issue.

https://miamielectricboards.com/shop-1/120amp-12s-power-switch
```

---
## \#5 Posted by: TSThunder Posted at: 2017-07-06T21:27:35.341Z Reads: 258

```
I would buy that one but it is sold out :(
```

---
## \#6 Posted by: TSThunder Posted at: 2017-07-06T21:28:05.897Z Reads: 254

```
DIY electric's? How did you get it for $40?
```

---
## \#7 Posted by: flywithgriff Posted at: 2017-07-06T21:28:32.616Z Reads: 251

```
Ahh I didn't realize that! I posted one for sale yesterday but it has already been purchased.
```

---
## \#8 Posted by: JdogAwesome Posted at: 2017-07-06T21:31:52.405Z Reads: 245

```
@JLabs Thanks for the kind words! Anyways yeah I will have my new EBoard Switches in stock in about 2-3 weeks, price is $35 a piece. My switch can handle 40A continuous and far higher bursts which is far more than enough for most boards. Im currently using in my board an old design of mine using just a single FET (compared to the two in my new design) which means it has a max of 20A continuous and it doesn't even get warm. My switch also comes in at just 1.8" x 1.15" which makes it one of, or the most compact on the market. They also come with a lifetime satisfaction guarantee so ill do whatever I can to make you happy with your purchase.
```

---
## \#9 Posted by: Jinra Posted at: 2017-07-06T22:03:59.950Z Reads: 225

```
I bought it used from @willpark16
```

---
## \#10 Posted by: TSThunder Posted at: 2017-07-06T22:06:24.076Z Reads: 216

```
Alright, I'm just gonna buy it and hope that it doesn't break
```

---
## \#11 Posted by: Jinra Posted at: 2017-07-06T22:07:14.162Z Reads: 205

```
I have a feeling people that have broken theirs have something setup wrong.
```

---
## \#12 Posted by: TSThunder Posted at: 2017-07-06T22:34:14.061Z Reads: 194

```
How did you set yours up?
```

---
## \#13 Posted by: Jinra Posted at: 2017-07-06T22:36:08.266Z Reads: 196

```
Pretty straight forward, negative to battery (or BMS) and positive to battery positive, then the other end had an XT-60 which goes to my parallel connector. I also attached a voltmeter to the end with the XT-60.

Perhaps others had it hooked up to the battery, voltmeter, fuse, or other device in a weird way.
```

---
## \#14 Posted by: mmaner Posted at: 2017-07-06T22:48:18.319Z Reads: 194

```
I've bought two and both failed within a few weeks, I'm absolutely POSITIVE it was installed correctly.  I use either the BMS switch and/or XT90-S now.
```

---
## \#15 Posted by: Jinra Posted at: 2017-07-06T22:51:03.454Z Reads: 186

```
Hm weird, could be a variety of various factors. Maybe we'll never know..
```

---
## \#16 Posted by: mmaner Posted at: 2017-07-06T22:56:47.677Z Reads: 190

```
I think there might have been a run of bad fets, I don't really care as I just don't trust switches.  I prefer the loop key arrangement, even if its not the most attractive.
```

---
## \#17 Posted by: TSThunder Posted at: 2017-07-06T22:59:44.738Z Reads: 196

```
Ok I changed my mind, do you know any tutorials on youtube about installing the loop key?
```

---
## \#18 Posted by: thisguyhere Posted at: 2017-07-06T23:15:48.175Z Reads: 194

```
i'm using a loop key now but going with a antispark switch for this main reason.

the female end of the loopkey is mounted to my enclosure.  the constant inserting / removing of the male part has quickly dislodged the female end mounted to the enclosure.  now the female end is just kind of hanging there loose and i need to grab with one hand while inserting the male end.  basically, loop keys get a lot of abuse.  and you'd be surprised how quickly you get tired on pulling the loopkey in and out.

in terms of how...

http://www.electric-skateboard.builders/t/how-to-anti-spark-xt-90-loop-key/204
```

---
## \#19 Posted by: JdogAwesome Posted at: 2017-07-06T23:24:08.906Z Reads: 175

```
@mmaner im really interested in why some of the vendors ive seen switches keep breaking on people so quickly. Ive had mine running for over a year just fine. I would love to get a hold of one of these broken switches, is there any chance I could buy one of the broken ones off of you for examining it? Im in the US FYI. It sounds similar to the problem I was having with my VERY early designs a year or more ago were I didnt have zeners and was driving the gates with way to high of a voltage, maybe its the same problem? Anyways let me know!
```

---
## \#20 Posted by: Jinra Posted at: 2017-07-06T23:26:14.537Z Reads: 173

```
I've heard some information from various people stating their their mosfets blew leaving it in an "always on" position
```

---
## \#21 Posted by: JdogAwesome Posted at: 2017-07-06T23:28:00.090Z Reads: 161

```
Yeah thats the most common type of MOSFET failure its just a drain to source short and is exactly what was happening to my old designs. By "their MOSFET's Blew" did you mean like actually blew up, or just stopped working?
```

---
## \#22 Posted by: Jinra Posted at: 2017-07-06T23:30:22.881Z Reads: 149

```
Ah, that I'm not sure of.
```

---
## \#23 Posted by: mmaner Posted at: 2017-07-06T23:38:41.313Z Reads: 149

```
I'll send you one, maybe you can give .e a discount on a new one 😀.  PM your address, I'll send it out tomorrow.
```

---
## \#24 Posted by: Mobutusan Posted at: 2017-07-06T23:45:09.531Z Reads: 150

```
I have a dead switch that I could send you as well. I bought it used, but still basically brand new from another member and it worked once for me, then got stuck in the on position. I'd like to try again with one of your switches, and a discount world be awesome, but honestly, if it just works, I'll be happy to pay full price for it. I'll pm you later.
```

---
## \#25 Posted by: JdogAwesome Posted at: 2017-07-06T23:48:30.498Z Reads: 144

```
Hey yeah I might be interested in another one, if its from a different vendor then @mmaner switch. And FYI Mike what company did you get your switches from? I forgot to ask. And @Mobutusan what company or person is your switch from as well? Would definitely love to take a look at some different ones and find out whats wrong with them.
```

---
## \#26 Posted by: Mobutusan Posted at: 2017-07-07T01:18:04.932Z Reads: 141

```
Mine is a Torqueboards/DIY switch.
```

---
## \#27 Posted by: JdogAwesome Posted at: 2017-07-07T01:19:24.142Z Reads: 138

```
Yeah I would definitely want a Torque boards switch, I'll dm you my address.
```

---
## \#28 Posted by: rpn314 Posted at: 2017-07-07T01:24:24.147Z Reads: 142

```
I soldered my own using the Vedder (original design)/Chaka (upgraded board) design. No issues so far.

http://www.electric-skateboard.builders/t/vedders-anti-spark-v1-4/2624?u=rpn314
```

---
## \#29 Posted by: ipv6app Posted at: 2017-07-07T02:56:02.879Z Reads: 138

```
I got these from GoldenHusky here.  DirectFET anti-spark switch thats based on vedder's but improved. So far I have tested this using the recommended 12v LED switch but I'm only running 25-35 amps thru the system.  I really like it, really small and clean look.  Inline fuse rated higher than what the other available switches seems to be OK for now, I will run this over the week some more and see how it holds up to the constant on-off.  Check this out as an option...

<img src="/uploads/db1493/original/3X/b/4/b47703061444871410396e992e96966a18979605.JPG" width="375" height="500"><img src="/uploads/db1493/original/3X/1/8/1873f69447be93568dae1845c9ef0f3b6cc32ee6.JPG" width="375" height="500">
```

---
## \#30 Posted by: jotatsu Posted at: 2017-07-07T03:14:17.408Z Reads: 135

```
why not buy a BMS with eswitch, whats the advantage of an external e-switch?
```

---
## \#31 Posted by: Jinra Posted at: 2017-07-07T03:46:37.997Z Reads: 127

```
Having to turn on your board to charge is kind of annoying
```

---
## \#32 Posted by: torqueboards Posted at: 2017-07-07T06:33:14.518Z Reads: 126

```
If they happen to crap out on you. Send them back in and we'll send you a new one.

We're working on a new design hopefully have it tested soon.
```

---
## \#33 Posted by: Namasaki Posted at: 2017-07-07T06:37:31.562Z Reads: 126

```
[quote="Jinra, post:31, topic:26935, full:true"]
Having to turn on your board to charge is kind of annoying
[/quote]

I don't find it annoying but it could get ugly if your remote's fail safe isn't properly setup.
Besides the E-switch on the Bestec bms's double as a reset switch incase one of the protection circuits shuts it down.
With other bms's you have to open the enclosure and disconnect power to reset them.
```

---
## \#34 Posted by: TSThunder Posted at: 2017-07-07T06:41:06.322Z Reads: 122

```
Free shipping too?
```

---
## \#35 Posted by: torqueboards Posted at: 2017-07-07T06:46:25.157Z Reads: 123

```
For a replacement if within the USA.
```

---
## \#36 Posted by: JdogAwesome Posted at: 2017-07-07T19:56:44.233Z Reads: 113

```
I love @goldenHusky DirectFET design, I cant imagine the amount of current you can run through that thing!  Definitely check that one out if you want a really beefy switch!
```

---
## \#37 Posted by: Lambjr088 Posted at: 2017-11-03T00:24:01.196Z Reads: 86

```
@ipv6app how has this switch been acting? Still holding up?
```

---
## \#38 Posted by: chopper064 Posted at: 2018-08-16T04:58:13.290Z Reads: 41

```
@JdogAwesome you still selling the switches?
```

---
## \#39 Posted by: JdogAwesome Posted at: 2018-08-16T05:24:37.950Z Reads: 36

```
I am, kinda. I have stock of my EbSC V3 Switches which are super compact however im still working on finishing my website to sell them, and mainly other stuff, on.
```

---
## \#40 Posted by: chopper064 Posted at: 2018-08-16T05:54:25.886Z Reads: 33

```
I would love one if possible
```

---
