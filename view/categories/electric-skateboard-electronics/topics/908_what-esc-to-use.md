# What esc to use?

### Replies: 30 Views: 25583

## \#1 Posted by: forangejuice Posted at: 2016-01-04T17:18:15.709Z Reads: 760

```
So i have absolutely no idea about what esc to use for my build. ive found these three:
http://www.hobbyking.com/hobbyking/store/__80518__Aerostar_70A_Electronic_Speed_Controller_with_5A_BEC_2_6S_.html
Hobbyking 70amp OPTO ESC with 5 Amp External UBEC
HobbyKing Red Brick 70A ESC
to be in use with this motor:
http://www.hobbyking.com/hobbyking/store/uh_viewitem.asp?idproduct=38036

I have no idea what is good and what isnt i just know that voltage cut off will prevent a lipo from becoming dangerous
Any help is appreciated
```

---
## \#2 Posted by: longhairedboy Posted at: 2016-01-04T17:37:21.801Z Reads: 757

```
Typically people try to stay above 120 amps when choosing ESCs because they are built to withstand higher currents and can therefore handle lower one far more reliably. I'm not sure how well a 70amp ESC will perform under constant load, it might just melt. @torqueboards has an excellent 6S ESC on his site that has proven to run well in both single and dual drive configs. I'm actually using a pair of them right now in my daily rider. Don't forget the programming card if you get one. 

product/single-motor-120a-6s-esc/

its $70 but unless it comes bad from the factory it will run great basically forever. It has a fan on it though, so your board will sound like some serious shit when you turn it on. He also has some 12S ESCs that will work fine with anything 6S and above and will be equally reliable but will give you plenty of headroom to take that motor on up to 10S when you're ready to upgrade your batteries one day. 

All of this is to say that your ESC is NOT the place to save cash. You'll just burn them up and end up spending more on replacements. I have a bench full of fried ESCs. 

Also, VESC. Its pricier, but the feature set is sooooo worth the money. I'm in love with them now. There's nothing I can really say about VESC other than "where has this been all of my life and why didn't i get them sooner."

Two places you can buy these:
From Enertion in Australia: http://www.enertionboards.com/electric-skateboard-parts/vesc-motor-controller/

From Ollin Board Co in the US: 
http://www.ollinboardcompany.com/product/vedder-s-speed-controller
```

---
## \#3 Posted by: forangejuice Posted at: 2016-01-04T18:04:19.188Z Reads: 644

```
wow thats some pretty sound advice, so what kind of benefit does a VESC have over a standard ESC?
```

---
## \#4 Posted by: longhairedboy Posted at: 2016-01-04T18:30:19.591Z Reads: 586

```
EVERYTHING. 

It's literally the ONLY ESC out there designed specifically for electric skateboards. Which of course means you can use it for sumo bots or anything else you want. If you aren't using a VESC, you're using a Car, Airplane, or Boat ESC, none of which are designed to carry a person up over 30mph but still seem to do a pretty good job at it. 

I don't even know where to start. It uses configuration and firmware updating software that runs on windows, mac, and linux, and is pretty easy to get set up and get running.

features? good god man. Traction control, complete granular control over remote throttle sensitivity, the ability to bridge two of them using a jumper wire over the CAN bus and only plug one into the receiver, motor detection, import/export of configuration settings to XML files to share with your freinds, real time motor performance data, more ways of controlling the thing than you can shake a stick at (PPM on analog remotes like the GT2B is just ONE option), and it works on Windows, Mac, and Linux. I'd stick with Windows if that;s what you have already, its probably the easiest. It's so over-engineered that it doesn't even need heatsinks or fans. And its Open Source. 

One downside is that there's almost too much info on it out there and some of it is old and useless. But that's what you get for staying on the bleeding edge. Also you have to take your time and configure the thing, its not plug and play. It will work with just about any battery and motor config, but you have to tell it what you're using or it will do Bad Things.
```

---
## \#5 Posted by: treenutter Posted at: 2016-01-04T19:42:18.337Z Reads: 502

```
@forangejuice VESC is the best option in my opinion @longhairedboy nailed it. The only reason to use something else is if you are unwilling to read a bit and learn to manage VESC, or if you require a complete stand-alone option that doesn't require a computer to configure.
```

---
## \#6 Posted by: longhairedboy Posted at: 2016-01-04T19:51:39.008Z Reads: 492

```
it has a 32bit ARM Cortex on it for christ's sake. If that doesn't make your nips hard then you're not geek enough and i may have to flag your account for review.
```

---
## \#7 Posted by: forangejuice Posted at: 2016-01-04T19:59:26.832Z Reads: 486

```
Oh jesus, everything just got real on me! im honestly kind of in shock at the sheer enthusiasm shown for this thing and you have definitely convinced me! I'm now sure of the direction i want to be going in for my build so I really cant thank you enough for all this help!!!
```

---
## \#8 Posted by: EnertionSupport Posted at: 2016-01-04T21:08:57.801Z Reads: 471

```
The VESC might seem overwhelming at first, but with the VESC faq section, and all of our member who are currently using the VESC, you should have no trouble setting it up. If you ever have any questions just ask!

You can buy a VESC here: http://www.enertionboards.com/electric-skateboard-parts/vesc-motor-controller/

The VESC faq section here:
http://www.electric-skateboard.builders/search?context=topic&context_id=298&q=vesc%20faq&skip_context=true
```

---
## \#9 Posted by: MonsterCoatings Posted at: 2016-01-05T12:10:36.771Z Reads: 458

```
AND don't forget the FOC option for super stealth operation now being worked out by Vedder and I hope others for even more set up options.
```

---
## \#10 Posted by: chaka Posted at: 2016-01-05T14:49:01.222Z Reads: 432

```
@forangejuice We provide full product support on all of the hardware we manufacture including the VESC. Usually a 5 or 10 minute phone call will get you up and running if you are having trouble with the software side of things. 

We also stand behind our product and will replace or repair any vesc that comes out of our shop. We have had zero failures since we began manufacturing. All the repair work we have done so far has been customer related electrical shorts which we also cover on a case by case basis.

[http://www.ollinboardcompany.com/product/vedder-s-speed-controller][1]


  [1]: http://www.ollinboardcompany.com/product/vedder-s-speed-controller
```

---
## \#11 Posted by: Braylon31 Posted at: 2016-01-14T05:02:36.528Z Reads: 380

```
What country are you  in ? Also i think  i shorted my first vesc from enertion through  a battery wire that touched a karma reciever after it wouldnt connect suddenly after power  up i shifted som things in my box battery wire touched spark now no led on back of vesc i dont think he offers repairs i want to buy two from you scince you iffer support but also wanted to know could you repair other one from enertion there is no visible burns or damage im thinking its somthing techy but fixable will you take a look if i send it?
```

---
## \#12 Posted by: chaka Posted at: 2016-01-14T14:04:59.034Z Reads: 359

```
We are in the US and would be happy to fix your VESC. Turn around time is usually same day on repairs. We only charge for the components and shipping to OllinBoardCo customers.

You can send the faulty VESC to:

Ollin Board Company
PO Box 3391
Truth or Consequences, NM 87901

@cmatson still waiting on yours, did you send it yet?
```

---
## \#13 Posted by: cmatson Posted at: 2016-01-14T22:44:44.304Z Reads: 341

```
[quote="chaka, post:12, topic:908"]
@cmatson still waiting on yours, did you send it yet?
[/quote]

I had sent it back to Jason first (before I knew you would repair it), and he was considering sending it to you. 

He wanted to find someone that would do VESC repairs for him, so he just ended up keeping it for whenever that happens.

Either way, I bought a new VESC from you, and was sent a replacement for the dead one from enertion's last batch.
```

---
## \#14 Posted by: Braylon31 Posted at: 2016-01-15T01:49:23.017Z Reads: 320

```
Thanks man your like the American Bruno or vedder lol its such a inconvenience to ship things like this back over seas for repair and American brainac like your self i should see faster shipping and turn around  thanks! For that ....can you customize a 10s with bms if so about how much?
```

---
## \#15 Posted by: barajabali Posted at: 2016-01-15T15:57:10.683Z Reads: 310

```
What esc do you guys recommend  for 12s for a sensored setup?

Let's keep things cheap please
```

---
## \#16 Posted by: trbt555 Posted at: 2016-01-15T16:05:47.914Z Reads: 297

```
You can't go wrong with a VESC.
```

---
## \#17 Posted by: barajabali Posted at: 2016-01-15T16:06:12.587Z Reads: 295

```
Vesc isnt sensored though right?
```

---
## \#18 Posted by: chaka Posted at: 2016-01-15T16:07:59.152Z Reads: 304

```
It is both. DIY's/torqueboards motors and ESC might be a better solution for you though. The VESC isn't the most user friendly to setup.
```

---
## \#19 Posted by: barajabali Posted at: 2016-01-15T16:10:53.071Z Reads: 308

```
I like to keep things simple with my boards, I dont want to do much programming on my computer or however its set up.  And DIY's esc's are none sensored @torqueboards  correct me if im wrong please. 

I want something as simple as the FVT 120 amp 6s sensord esc but capable of 12s. 
I guess the hunt continues


http://alienpowersystem.com/shop/esc/alien-150a-2-12s-evolution-3-car-esc-hv-twin-sensored/

Maybe that? upgrades always costs me so much
```

---
## \#20 Posted by: cmatson Posted at: 2016-01-16T04:58:51.721Z Reads: 314

```
[quote="barajabali, post:19, topic:908"]
Maybe that? upgrades always costs me so much
[/quote]

Some people have burnt those out really quickly, and others swear by them... It's sorta the luck of the draw.

I'd just buy a VESC :smile:
```

---
## \#21 Posted by: awcany Posted at: 2016-07-29T16:34:56.862Z Reads: 253

```
so u can say that a esc designed fot a quadcopter may work for a electric skateboard?
```

---
## \#22 Posted by: longhairedboy Posted at: 2016-07-29T17:22:17.774Z Reads: 250

```
i can't say that, no. In fact i probably wouldn't even try it. quadcopters don't have brakes or reverse as far as I know, and their motors are small compared to esk8s so who knows if they can even handle the amps.
```

---
## \#23 Posted by: DIY4Life Posted at: 2016-12-09T12:44:18.303Z Reads: 201

```
Guys,
Could some-one please help me out for a sec.

I have this ESC laying around, its a badass ESC, super solid and reliable
http://rctimer.com/download/HW-SM013_PL100A-HV-en.pdf

And i would like to use it as an eboard ESC.
But it actually isnt a car ESC(brake mode and stuff included) , but a HELI ESC... with flight modes

First i thought i wasnt able to use it, and have to buy a new one :-(, but when reading the manual, 
i can set it to have a brake mode?? Correct?

And i can set the flight mode as 'HELI GOVERNOR OFF' and then it will have a straight throttle curve (check the throtthle curves in the manual please...), this is what an eboard ESC would offer me to right??
Or wil it just have a forward and reverse with that curve? 

is setting forward and brake mode possible? (no reverse, straight throttle line,...)
Please help me out, i know a lot about building and electricity but nothing about programming ESC's.

Looking forward to answers from you guys!!!
```

---
## \#24 Posted by: Monk Posted at: 2017-01-10T20:13:55.415Z Reads: 183

```
Have you had any luck finding out if that ESC will work? I have two of the same one and would like to use them on my dual drive build.
```

---
## \#25 Posted by: RogerD Posted at: 2017-01-11T09:45:04.489Z Reads: 178

```
Oh yes you can. There are countless posts on here regarding blown vescs and I've first hand experience with two blowing up for no apparent reason.

If you don't know electronics well and don't like tweaking settings then the vesc can be a very frustrating and expensive experience. 

Just take a look at the posts for vesc drv failures alone.
```

---
## \#26 Posted by: AutoNoe Posted at: 2017-12-31T09:10:24.904Z Reads: 94

```
Ok so according to all your geeking out the VESC is the way to go for a skateboard. But what's up with the seemingly low continuous max current? If it can only handle 50A continuous how is it going to manage powering my 90A max motor? Is there something I'm missing in the way it handles power? Otherwise it seems rather underwhelming...
```

---
## \#27 Posted by: FredrikHems Posted at: 2017-12-31T12:19:27.764Z Reads: 93

```
Your motor will never pull 90A continious, unless you weight 500 pounds and tries to Go up a 30 degrees hill. 
Most people draw around 10+- amps in average, depending on weight and riding style
```

---
## \#28 Posted by: GrecoMan Posted at: 2018-01-01T02:02:48.424Z Reads: 89

```
hey man what’re you trying to say? i’m 608lbs and climb 95 degree hills daily with a vesc without problems. lol

but yea, you will never even get close to 50a continuos.  most of our motors are 80-90a too
```

---
## \#29 Posted by: mmaner Posted at: 2018-01-01T02:10:52.671Z Reads: 86

```
I've been running dual 6354s on VESC's for almost 2 years and very seldom.go over a 15a draw. On my Evo that has dual 6374s I've hit 50a a couple if times while accelerating up big hills and carving hard...but it's rare.
```

---
## \#30 Posted by: GrecoMan Posted at: 2018-01-01T02:12:54.550Z Reads: 86

```
and continuous and burst are very different. think i’ve hit 50a gunning it up a super long hill, but not for more than a few seconds.  bottom line is, if your actually pulling 50a continuous your doing something else wrong 😉
```

---
