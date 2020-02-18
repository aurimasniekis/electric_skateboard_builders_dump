# What is the best 2.4GHZ controller for VESC?

### Replies: 117 Views: 16311

## \#1 Posted by: Moja Posted at: 2015-08-30T13:36:53.801Z Reads: 689

```
I am interested to hear what everyone thinks is currently the best solution out there for controlling an e-board using VESC. I am looking for a sturdy and reliable controller that fits well in my hand and uses a good interface solution that isnt going to get me killed, maybe a solid spring loaded wheel like the boosted boards remote.

Important features would be a button for switching into reverse and possibly an extra button for toggling LED lights if I fit them down the line, a good rechargeable lithium battery, a solid wireless connection, a usb port for programming (is this necessary?).

The Kama nunchuck seems like a good solution apart form the joystick which I imagine is a bit fiddly and the quality of the wireless connection which could be dangerous. I like the look of the GT2B mod (http://www.electric-skateboard.builders/t/build-your-own-compact-eboard-controller-gt2b-case-mod/104/3)  but I don't have the time and resources to built one and I imagine it has no reverse feature. The original GT2B is far too big...

What do you all think is the best option out there?
```

---
## \#2 Posted by: torqueboards Posted at: 2015-08-30T18:55:22.381Z Reads: 637

```
GT2B is by far the best solution. It's my sole controller and 2900+ miles and not a single drop except for when I didn't charge my GT2B batteries but even the GT2B batteries last for months before changing too.
```

---
## \#3 Posted by: onloop Posted at: 2015-08-31T02:04:18.379Z Reads: 630

```
AGREED!.... GT2B is the only affordable option that is reliable.

there will be some custom made Wii Nunchucks "Style" controllers coming in the next few weeks that will be reliable & affordable & 100% plug & play compatible with VESC
```

---
## \#4 Posted by: siggs3000 Posted at: 2015-08-31T03:59:11.015Z Reads: 621

```
Is the Kama connection really pretty sketchy compared to the GT2B?
```

---
## \#5 Posted by: lowGuido Posted at: 2015-08-31T10:18:20.489Z Reads: 605

```
I found the weak link in the Kama is the connection to the dongle. I have soldered the dongle directly and I don't get anymore drop outs.

the GT2B re housed in a smaller case is a cheaper option though
```

---
## \#6 Posted by: Moja Posted at: 2015-08-31T13:32:11.632Z Reads: 594

```
What do you mean when you say you soldered the dongle directly? Are you referring to the connection between the VESC and the nunchuck receiver?

@ onloop: I'm excited to see these nunchuck style controllers, seems like there is a real gap for a controller that ticks all the boxes. Good luck with getting them to market!
```

---
## \#7 Posted by: longhairedboy Posted at: 2015-08-31T19:05:04.820Z Reads: 563

```
just my 2 cents: the GT2B is the most reliable controller that money can buy, and at $25 its dirt cheap. 

I've never even thought about other control schemes because the GT2B gives you such a solid analog "gas pedal" feel in the trigger, not to mention that it never drops out and the battery lasts seemingly forever on a single charge. ITs also not heavy at all and feels great in your hand. Yes, its kind of large, but not at all heavy. And lots of knobs to tweak. I play with the trim a lot when trying to set a good cruise speed, and if i want to switch to front wheel drive mode i can do so with the flip of a switch. Yes, i do that sometimes because the ride is kind of interesting. 

Also, it can take a beating. Mine's bashed and scratched to hell and back and its still working flawlessly.
```

---
## \#8 Posted by: lowGuido Posted at: 2015-09-01T01:04:49.692Z Reads: 552

```
yeah I soldered the wires in the dongle direct. the biggest failing pint of the wiiceiver imho is that it ises a direct PCB connection to the dongle.. the PCB is actually a tiny bit thinner that the actual nintendo socket so vibrations can break the connection, and once its broken the dongle "reboots" causing a brief loss of connection.
I have added solder to the tracks on the wiiceiver PCB making it thicker and the improves it a lot. I have also added a proper nintendo socket to the board. the nintendo socket also improves it. but it was never designed to handle the vibration of a skateboard.
soldering the dongle direct is the best option. and so far I have not had any issues with drop outs.

incidentally the way you connect the dongle to the VESC is by soldering the dongle to a plug on the VESC so I would take an educated guess that the nunchuck with VESC would work a lot better than having a wiiceiver.
```

---
## \#9 Posted by: Moja Posted at: 2015-09-01T02:33:18.168Z Reads: 524

```
The GT2B sounds like a solid workhorse. Is there anywhere I can buy a smaller housing for it? I don't access to a 3D printer.
 Also, I have a few Fiik remotes for my Chinese made boards, they are actually pretty awesome, they feel good in the hand, never drop out and the shape of the gun allows me to do slides using the remote as if it were a downhill glove (massively awesome feature) Can I mod one of these to work with the VESC easily?
```

---
## \#10 Posted by: onloop Posted at: 2015-09-03T00:48:37.739Z Reads: 521

```
[quote="lowGuido, post:8, topic:155"]
have added solder to the tracks on the wiiceiver PCB
[/quote]

We want pictures... ;)
```

---
## \#11 Posted by: Moja Posted at: 2015-09-11T07:19:37.587Z Reads: 516

```
What is the best way to connect the GT2B PCB to the VESC?
```

---
## \#12 Posted by: onloop Posted at: 2015-09-11T07:36:24.586Z Reads: 524

```
if you have a servo extension lead you can solder it on as pictured. BROWN RED ORANGE

<img src="/uploads/db1493/original/1X/15cdab51d8aa5456022fe14777e66a951db9bb5b.jpg" width="318" height="500">
```

---
## \#13 Posted by: CSN Posted at: 2015-09-11T18:59:27.970Z Reads: 514

```
The GT2B conversions like the Bad-Wolf just need to add a button and function for cruise control.

The nunchuk/wiiciever's cruise is really helpful so the rider doesn't have to constantly have a tense trigger finger on the throttle. The cruise function means the rider can relax a lot more.
```

---
## \#14 Posted by: longhairedboy Posted at: 2015-09-14T01:04:37.443Z Reads: 498

```
The GT2B's C channel button would be perfect for a cruise control toggle. Make it so. lol
```

---
## \#15 Posted by: Stuartmac Posted at: 2015-10-23T13:34:22.348Z Reads: 501

```
I'm currently using a wiiciever/nunchuck setup however I think this is the part that is stalking my build (it simply won't go). Would it be simple to hook up a GT-2B reciever and remote in its place? The connections to the current wiiciever are the ESC signal wires (brown, red, yellow) and the UBEC power wires (red and black).
From reading all of your comments the GT-2B seems like the most reliable remote to fault find with so I'm keen to give it a go.
```

---
## \#16 Posted by: lowGuido Posted at: 2015-10-23T14:52:57.987Z Reads: 502

```
or you could fault find with a $2 servo tester
<img src='/uploads/db1493/original/1X/0aaa547c435062d360d441456353e07ded7dac3a.jpg'>
```

---
## \#17 Posted by: Stuartmac Posted at: 2015-10-24T01:12:37.665Z Reads: 487

```
Cheers thats a great idea which I will definately try. I am however pretty sure the motors are working as they are giving me the correct feedback (beeping and vibrating) when I am programming my ESC. 
If it does turn out that the motors are ok would my original idea of switching the wiiciever/nunchuck with a GT-B2 kit work or would I need to do some additional programming? 
I've invested a bit in this board and I'm getting very close to scrapping the current esc's in favor of the highly praised vesc's ha ha.
```

---
## \#18 Posted by: jacobbloy Posted at: 2015-11-05T13:35:24.707Z Reads: 493

```
Has any one tried the custom nunchuck pcb that Vedder and I designed, it's great uses standard 2.4ghz good connection you can use long rang antenna if you want! It has cruise and direction change. And the throttle is smooth and creamy.

I had some samples made through macrofab cost be $35 for the pcb assembled. Or I did some my self for $25.

Maybe by the end of the week I will have it working with the wiiceiver so you just plug in a nrf24l01 and away you go, will still work with cruise!  See my 2 dev boards 1 stm32f100 the other is a uno<img src="/uploads/db1493/original/1X/ee4e1dd0d6821a02954bed9089c31acdc2d90de5.jpeg" width="690" height="414">

One thing you can do is take the custom nunchuck pcb and and solder on your 10k ohm pot trigger and make a super small 3D printed case.<img src="/uploads/db1493/original/1X/1b2450a7a77615184c1a014ca3898e02d0576222.jpeg" width="666" height="500"><img src="/uploads/db1493/original/1X/d6a5ecd4a8df1ae6bf976a497c255f321fdfc9b2.jpeg" width="375" height="500">
```

---
## \#19 Posted by: lox897 Posted at: 2015-11-05T20:43:31.091Z Reads: 475

```
Nice job! Hope this takes away "connection drops" if it does I might be in for one for another build.
```

---
## \#20 Posted by: Moja Posted at: 2015-11-06T01:28:10.508Z Reads: 484

```
I would like one of those nunchuck kits, the nyko setup is great but not reliable enough. Can I order one from you?
```

---
## \#21 Posted by: jacobbloy Posted at: 2015-11-06T09:37:29.505Z Reads: 482

```
Video demonstration
https://youtu.be/PV64I1yTcsM
```

---
## \#22 Posted by: disastorm Posted at: 2015-11-06T10:33:28.376Z Reads: 478

```
With everyone talking about connection drops, does that actually happen when the nyko receiver is connected directly to the UART ? I thought I've heard most people say it almost never drops once you do that ?
Also what actually happens during a drop, what happens if connection drops while you are riding around, you have to stop with your foot ? Could something bad happen like the machine keeps accelerating or something like that?
```

---
## \#23 Posted by: lowGuido Posted at: 2015-11-06T12:16:07.216Z Reads: 461

```
Yeah something bad like that can happen.
```

---
## \#24 Posted by: treenutter Posted at: 2015-11-06T14:21:41.034Z Reads: 454

```
This looks great @jacobbloy. One thing I notice is that as you increased your speed while using cruise control, there was a nice smooth transition from one speed to another. [On my current build using VESC][1], when I to increase or decrease speed while using cruise control, [tap up (to speed up) or down (to slow down)] the result is a "jerky" transition that almost knocks me off the board. I've been playing with settings in BLDC to see if I can fix it but perhaps the custom nunchuk PCB is the solution.


  [1]: http://www.electric-skateboard.builders/t/the-village-build-s9-faultine-paris-195mm-sk3-6764-diyes-mount-8s-vesc-127mm-pneumatic-wheels/292
```

---
## \#25 Posted by: onloop Posted at: 2015-11-08T00:00:23.270Z Reads: 444

```
Very cool remote!...
```

---
## \#26 Posted by: lowGuido Posted at: 2015-11-08T00:11:26.086Z Reads: 435

```
That's interesting @treenutter I use a wiiceiver and all the acceleration and deceleration on cruise is smoooth as.
```

---
## \#27 Posted by: treenutter Posted at: 2015-11-08T00:27:17.012Z Reads: 432

```
@lowGuido it's the only thing I don't like about the nunchuck implementation for VESC. There's a workaround; it's just to release the cruise button, accelerate (or decelerate), and then press+hold the cruise button again. But it would be better if that wasn't needed. There's likely a fix that I haven't discovered yet...
```

---
## \#28 Posted by: lowGuido Posted at: 2015-11-08T02:59:30.627Z Reads: 424

```
Wow. That sucks. One of the big sellers for me on the VESC was the built in nunchuck support.
I haven't got my VESC yet so Im yet to judge. But if its as you say that's pretty lame.
You could use a wiiceiver signal split into the VESC. But then there's the additional cost of the wiiceiver. .
```

---
## \#29 Posted by: disastorm Posted at: 2015-11-08T06:24:29.980Z Reads: 416

```
So do drops happen when you solder the nunchuck receiver to the VESC or is that only when you use with the wiiceiver ?
Also in what case might it get stuck as accelerating ? I would think if it disconnects it would just stop ( unless cruise control is on ) since its not receiving any signal ? So is the only danger if cruise control is on ?
```

---
## \#30 Posted by: lowGuido Posted at: 2015-11-08T07:05:28.373Z Reads: 414

```
I use a wiiceiver so i cannot assure you 100% with VESC.  But i can assure you that with wiiceiver, with my nyko kama soldering stops all the dropouts. 
I can also tell you that before i soldered it and i was using the slide on connection that I have slammed a number of times from droppout related incidents. 
Including but not limited to:
Acceleration stuck on.
Acceleration stops suddenly while climbing a hill.
Brakes don't work at all, and then they work full. (This one is the worst)

In any case soldering is always better.
```

---
## \#31 Posted by: treenutter Posted at: 2015-11-08T17:53:45.631Z Reads: 394

```
Hey @lowGuido when you get your VESC and solder the wires to the port, could you take pic and share it? I've never soldered thin wires like this to a port, so I'm wondering about the amount of solder to use and the direction to guide the wires.
```

---
## \#32 Posted by: treenutter Posted at: 2015-11-08T17:57:25.572Z Reads: 404

```
@lowGuido keep in mind that I'm a total novice, so there is probably a setting that I'm missing somewhere. Does anyone else w VESC and nunchuck experience have thoughts about jerky acceleration when using cruise control? @jacobbloy ?
```

---
## \#33 Posted by: lowGuido Posted at: 2015-11-08T21:40:20.080Z Reads: 400

```
I was going to remove the JST connector and through hole solder the wires.
like this:
<img src='/uploads/db1493/original/1X/a45408b3f4a266318d2b5f9ea527b79c9053e828.gif'>
```

---
## \#34 Posted by: elkick Posted at: 2015-11-08T21:58:55.917Z Reads: 396

```
You could do that but why not just use the solder spots at the backside of the VESC and solder it horizontally?

I just use a JST-connector and simply solder those wires which came with the connector to the wires coming from the receiver.
```

---
## \#35 Posted by: jacobbloy Posted at: 2015-11-08T22:01:31.808Z Reads: 391

```
I only use a jst plug, and have no connection problems!
```

---
## \#36 Posted by: lowGuido Posted at: 2015-11-08T22:06:41.416Z Reads: 396

```
seeing as I don't have my VESC yet, its difficult for me to make a final decision on how i will do it, because Im not super familiar with the layout. i'll definitely use a JST plug to start with while testing and configuring. if I don't have any issues with it then I may well leave it.
I have had problems in the past where the servo connector from my ESC has fallen off while skating. I like to keep things as solid as possible.. plugs and connectors to me just seem like one more possible point of failure.
I have always tried to minimize plugs wherever I can
```

---
## \#37 Posted by: jacobbloy Posted at: 2015-11-08T22:15:40.391Z Reads: 385

```
I think that the nyko Kama and regular wii nunchucks the vesc is trying to understand the code sent to it, where the code on the pcbs isn't really made for electric skateboards. It like when my 1 yr old talks to me the words are broken up and I have to smooth it out to understand it.

The wiiceiver and vesc do a great job at this but I would say Vedder wrote custom code and designed the pcb for this reason!
```

---
## \#38 Posted by: Blasto Posted at: 2015-11-09T02:26:45.822Z Reads: 386

```
@treenutter jst press in connectors, just need a fine flat head screw driver and "jam" the wire in the connector. 

4 pin:  http://www.digikey.ca/product-detail/en/04KR-6H-P/455-2689-ND/2797475

6 pin: http://www.digikey.ca/product-detail/en/06KR-6H-P/455-2687-ND/2797480?fullsite=true

7 pin: http://www.digikey.ca/product-detail/en/07KR-6H-P/455-2686-ND/2797469
```

---
## \#39 Posted by: kai Posted at: 2015-11-09T03:32:32.650Z Reads: 375

```
Hmm i wonder if those press in connectors would handle the vibration without them starting to break the exposed wire after a while.
```

---
## \#40 Posted by: treenutter Posted at: 2015-11-09T21:12:33.374Z Reads: 408

```
@lowGuido @jacobbloy I got in a few hours of riding this weekend and I've realized something; my comments about VESC and jerky cruise control were due to my own user error.

One of the challenges\joys of DIY is that there aren't typically "user manuals" for different devices and tools. We have to  figure out how a designer intends for us to use something.

So when using cruise control with VESC and a nunchuck, here's how it works:

**Hold down Cruise Button:** This will lock the current speed. On descents, the motor will work to reduce the speed if needed. This is totally awesome. Very controllable downhill!

**To Accelerate:** (While holding Cruise Button) gently move the throttle upward a small amount. The cruise throttle is cumulative; you are "adding" to the existing speed when you use the throttle. Only a small addition of throttle is needed to increase speed. If you give it too much throttle while in cruise, and you have sufficient torque, you'll feel a "knock" while you rapidly increase speed (not recommended!)

**To Decelerate** (While holding down the Cruise Button):  Release the Cruise Button momentarily, and then depress and hold it down again. You have now achieved smooth deceleration! If you need to reduce speed further, do it again or depress for a longer period of time.

DO NOT PULL DOWN OR TAP DOWN ON THE THROTTLE WHILE HOLDING DOWN THE CRUISE BUTTON. This activates the brake and you'll feel strong braking instead of smooth deceleration. You may fall off if you're not expecting this!

I'll also note that cruise works amazingly well when climbing hills. You can climb at a consistent speed and VESC regulates the amount of power needed to achieve the climb at your desired speed. All hail the mighty VESC!
```

---
## \#41 Posted by: treenutter Posted at: 2015-11-09T21:15:11.138Z Reads: 368

```
@lowGuido I still haven't experienced any dropouts yet, using the JST plug. I agree with you, however, that reducing potential failure points is the best way to go. With more hours on this build I can see how the JST plug's connection could weaken.
```

---
## \#42 Posted by: lowGuido Posted at: 2015-11-09T22:20:47.490Z Reads: 365

```
@treenutter
Ahh. Your description sounds very different to the wiiceiver method of cruising.
Im not sure i like the idea of brakes while on cruise. Sounds dangerous. But some of the other aspects like down hill decent sounds really good.

Im sure its something i'll get used to.
```

---
## \#43 Posted by: longhairedboy Posted at: 2015-11-10T19:09:53.106Z Reads: 355

```
the idea of cruise control on an eboard in general just makes me nervous.
```

---
## \#44 Posted by: treenutter Posted at: 2015-11-10T20:37:16.346Z Reads: 357

```
@longhairedboy it made me nervous at first as well, but I've grown to really love it. Unlike a car's cruise control, you have to constantly supply input to the ESC to keep moving, so there's no way for the board to run off without you if you release the remote (unless a hardware error occurred, in which case effffff!)
```

---
## \#45 Posted by: lowGuido Posted at: 2015-11-10T21:38:04.580Z Reads: 375

```
@longhairedboy have you ridden a board with cruise control?
I never ride without it. 
its so nice. you just get to the speed you want to skate at and then hold the button down.
dont have to worry about anything. if a small pug runs out in front of you and you get a shock, you almost instinctively release the button and glide to a slower speed. when the monster is gone you hit the button again and you back on your way.
in fact I never eve decelerate. I just release the button whenever I feel I want to slow down.
cruise control is a bad word.. maybe it should be constant speed button.

edit nah forgedabout it.. from this moment forward I'm calling it the "perpetual Steez button"
```

---
## \#46 Posted by: treenutter Posted at: 2015-11-12T00:36:26.181Z Reads: 372

```
@Moja I found [this controller at HK][1]. I've never tried it, but it is much smaller than a GTB2 and really cheap at $21USD. Has anyone tried it?
<img src='/uploads/db1493/original/1X/6bdf39a3e2ff146565bb9cb3df5b8d760fd7d699.jpg'>
  [1]: http://www.hobbyking.com/hobbyking/store/__44693__Quanum_2_4Ghz_3ch_Pistol_Grip_Tx_Rx_System.html
```

---
## \#47 Posted by: onloop Posted at: 2015-11-12T00:39:31.337Z Reads: 364

```
its not as good as gt-2b
```

---
## \#48 Posted by: psychotiller Posted at: 2015-11-12T01:07:58.502Z Reads: 353

```
Horrible binding issues.
```

---
## \#49 Posted by: treenutter Posted at: 2015-11-12T01:09:43.082Z Reads: 353

```
@onloop @psychotiller That's too bad; I was hopeful that it might be a decent alternative to GTB2 for folks who don't want to do the Badwolf mod :cry:
```

---
## \#50 Posted by: onloop Posted at: 2015-11-12T01:12:15.124Z Reads: 355

```
ive been using a gt-2b unmodified since day one... i couldn't give a F it looks big / bulky etc... i'm not in it for the vanity!.... however i am eagerly awaiting the NEW VESC remote
```

---
## \#51 Posted by: psychotiller Posted at: 2015-11-12T01:25:33.263Z Reads: 365

```
Yeah,  It was maybe the single most frustrating period of time for me trying to get those pieces of crap to bind consistently...or at all

Someone could try the small generics that are popping up on Amazon? They may work
```

---
## \#52 Posted by: lox897 Posted at: 2015-11-12T05:10:17.253Z Reads: 367

```
Ooooooooo. The "NEW VESC" Remote, what is it? Tell me more please.
```

---
## \#53 Posted by: lowGuido Posted at: 2015-11-12T05:33:53.713Z Reads: 366

```
@treenutter I actually just bought one of those Quanum transmitters for science.
haven't tried it yet but I'll let you know.
I don't know how i will go with no perpetual Steez button though.
```

---
## \#54 Posted by: sgaana Posted at: 2015-11-12T05:43:16.271Z Reads: 367

```
@onloop Is this ready to be shipped out?<img src="/uploads/db1493/original/1X/61c477d781a647304b42aae0dc1badb3afb0e3f5.jpg" width="240" height="320">
```

---
## \#55 Posted by: onloop Posted at: 2015-11-12T08:28:53.572Z Reads: 362

```
No... still testing. .. needs some fine adjustments. Mostly software related.
```

---
## \#56 Posted by: elkick Posted at: 2015-11-12T09:41:50.687Z Reads: 365

```
Have got one and it works well since 4 weeks. First binding was a bit tricky, you have to hold the power button at the remote while switching on the board until you hear 3 beeps. Then it's done. Didn't know that before though...😉
```

---
## \#57 Posted by: treenutter Posted at: 2015-11-12T13:21:41.636Z Reads: 369

```
@lowGuido awesome! Please let us know how it goes! Ya; I'd miss perpetual Steez but maybe the "gas pedal" feeling is cool. Note @elkick 's comment about binding below. @psychotiller had a bad experience binding these, but maybe they've improved since.

[quote="elkick, post:56, topic:155"]
hold the power button at the remote while switching on the board until you hear 3 beeps
[/quote]
```

---
## \#58 Posted by: Glenn Posted at: 2015-11-12T14:23:16.988Z Reads: 369

```
I will be looking forward to seeing them when they get here.
```

---
## \#59 Posted by: Glenn Posted at: 2015-11-12T14:29:22.833Z Reads: 363

```
I have this remote and it's reliable but kinda looks like a hand gun when in hand. The only thing I don't like about it is changing out the batteries.(none rechargeable type)
```

---
## \#60 Posted by: psychotiller Posted at: 2015-11-12T14:43:15.580Z Reads: 366

```
Man! Wish I would have known that...Haha.  I kid I kid, that never worked.
```

---
## \#61 Posted by: treenutter Posted at: 2015-11-12T14:47:17.072Z Reads: 365

```
Thanks @Glenn good feedback. I suppose we could get rechargeable AA's but of course then that drives up the cost.
```

---
## \#62 Posted by: lowGuido Posted at: 2015-11-13T06:49:58.849Z Reads: 366

```
Well i checked my mail today and it was like Christmas! 
I bought a lot of this stuff cheap, for science.  Im going to build a hack board and just use it to test all types of transmitter and ESC combos.
<img src="/uploads/db1493/original/1X/36b1f6687d5deddfae8dfa00937115f055eb5759.jpg" width="690" height="388">
```

---
## \#63 Posted by: treenutter Posted at: 2015-11-13T15:53:48.478Z Reads: 357

```
@lowGuido awesome! I haven't seen that controller with the red molding before what is that?
```

---
## \#64 Posted by: lowGuido Posted at: 2015-11-14T06:18:06.242Z Reads: 340

```
Well so far so good with the quanam.  Binds up without any issues so far. But its raining so I cant take it for a skate.

The red one i bought as an impulse buy online somewhere. I cant even remember.  I just remember buying it because it looked pretty compact. 
However it didn't come with a reciever so. Its kinda useless to me at the moment.
```

---
## \#65 Posted by: lowGuido Posted at: 2015-11-15T12:56:19.439Z Reads: 349

```
Ok so my quanam experience so far has been pretty good. To bind i simply turn it on and place a jumper on the receiver an then take the jumper off. Done.
Every time i power on the transmitter after that it just syncs up.
I even tried to un-bind it by putting the jumper on an not turning on the transmitter.  It just binds up again as soon as i turn on the transmitter. 
I don't know. Seems almost too easy.
As for how people skate without perpetual steez button I'll never know. I have only had one skate but it required 100% of my concentration on that trigger finger. It was easier than trying to skate with the nunchuck joystick alone, which was a relief. 
I'll give it a few more tries, but I cannot see myself ever enjoying a skate with a trigger type transmitter. 
Nunchuck is just so effortless. 
Perpetual steez 4 lyfe!

Oh. Also you need to remember to turn the transmitter off. Nunchuck just powers itself off when you turn the board off. Thats got me a couple of times now.
```

---
## \#66 Posted by: lowGuido Posted at: 2015-11-18T01:17:47.325Z Reads: 346

```
Well I just did a 10 km skate with the quanam. And while i have absolutely no technical issues with the transmitter  I will never ride another trigger driven transmitter so long as I live. I am sure that i can fine tune a few things and probably get used to it, but it just isnt anywhere near as fun as the nunchuck.  My trigger finger is cramping, and even though its the same board I just cant seem to go as fast as with the nunchuck.  While it is physically capable I just dont seem to be able to pull the trigger all the way down. And the brakes seem less responsive.  I feel that I need to tune them up on the esc or something.  Again its nothing to do with the capability.  But more with me and my finger being too cautious. 

TLDR: Im concentrated so much on the trigger I can't enjoy my skate.
```

---
## \#67 Posted by: lowGuido Posted at: 2015-11-18T09:26:24.778Z Reads: 350

```
I don't want to harp on here... 
but in the interests of science I have ordered a receiver for the red transmitter. even though I have pointed out my hate for the trigger, I'm going to follow this though.
one thing I have noticed is that the handle of the red transmitter is empty sans battery in the red part. so I could effectively hack off the bottom of it to make it even more compact.

here's my not an artists impression:
<img src="/uploads/db1493/original/1X/9518022a2605adf2530fe86f80bfa47f9e6c6fb1.jpg" width="432" height="173">

also worth pointing out that this transmitter cost USD$5
so it would be very economical if I can sort something out with the receiver.
```

---
## \#68 Posted by: treenutter Posted at: 2015-11-18T20:42:41.796Z Reads: 335

```
@lowGuido Thanks for all of this great feedback, keep it coming! I'm enjoying this testing process.
```

---
## \#69 Posted by: treenutter Posted at: 2015-12-03T16:34:23.830Z Reads: 334

```
@lowGuido any tips on removing the JST connector safely? 

[quote="lowGuido, post:33, topic:155"]
I was going to remove the JST connector and through hole solder the wires.
[/quote]
```

---
## \#70 Posted by: lowGuido Posted at: 2015-12-03T21:32:29.825Z Reads: 327

```
Its tricky.  Best done with a desoldering iron.
```

---
## \#71 Posted by: treenutter Posted at: 2015-12-11T18:08:59.305Z Reads: 328

```
@lowGuido did you ever get the "Red Demon" working? Could you share where you found it?
```

---
## \#72 Posted by: lowGuido Posted at: 2015-12-11T21:42:18.502Z Reads: 315

```
I have all the  parts but i havent got around to testing it yet. I am going to build a dirty  hack board that i can pull things on and off of for science.
```

---
## \#73 Posted by: lowGuido Posted at: 2015-12-18T14:50:26.563Z Reads: 312

```
well the so called "Red Demon" seems to be a big fat fail. even with the specified receiver I can't seem to get it to bind at all.
while I am a little disappointed I couldn't get it to work and wasted about $12 on it. I'm also not too worried about it because Trigger throttle sucks anyway.
```

---
## \#74 Posted by: treenutter Posted at: 2015-12-18T16:03:13.083Z Reads: 306

```
@lowGuido lol I enjoy your complete disdain for trigger throttle! I've recently been using GT2B and I find it quite nice when paired w VESC. Have you tried it w VESC? For me, it feels very smooth and easy to control. It's not ideal, and I really need a **perpetual steez** button to fully enjoy the ride; but after a few rides I've started to enjoy it.
```

---
## \#75 Posted by: lowGuido Posted at: 2015-12-18T16:17:34.107Z Reads: 314

```
yeah don't get me wrong. its smooth and I can ride it, but I just don't find it as enjoyable as the perpetual steez.
i even worked a system where I braced my trigger finger against my middle finger a little so that I could relax a bit more.
but still..
if only the damn Nyko Karma wasn't so hard to get in Australia..
I suppose the only next logical step is the custom vedder nunchuck..
```

---
## \#76 Posted by: chaka Posted at: 2015-12-18T16:19:30.853Z Reads: 330

```
Just pull it all the way.
```

---
## \#77 Posted by: lowGuido Posted at: 2015-12-18T16:24:41.145Z Reads: 346

```
LOL. I dont want to die.
```

---
## \#78 Posted by: treenutter Posted at: 2015-12-18T16:26:03.603Z Reads: 350

```
ha! @chaka ! Ya @lowGuido , just use electrical tape to hold the trigger in the 100% position.
```

---
## \#79 Posted by: treenutter Posted at: 2015-12-18T16:27:51.191Z Reads: 374

```
[quote="lowGuido, post:75, topic:155"]
I suppose the only next logical step is the custom vedder nunchuck..
[/quote] 

@lowGuido yep I'm waiting to hear that a stable build is ready! Until then it's GT2B city!
```

---
## \#80 Posted by: psychotiller Posted at: 2015-12-18T16:37:53.891Z Reads: 397

```
No one here gets out alive -Jim Morrison
He would've pulled it all the way haha
```

---
## \#81 Posted by: Moja Posted at: 2015-12-18T17:54:52.971Z Reads: 378

```
I just tested out my Nyko Kama with the 4.10 VESC and 2.3 BLDC. The cruize control is drastically improved and its working like a dream, very smooth speed increases and decreases. It seems like allot of work as been done on the programming. 
However I do have issues using the remote in my front hand, my VESC's are mounted near the right truck and holding it in my front hand results in my led obscuring the 2.4GHz transmission, no problems in my back hand with a clear line of sight though.
```

---
## \#82 Posted by: treenutter Posted at: 2015-12-18T18:27:18.118Z Reads: 371

```
@moja that's really interesting... is the connection between the Nyko Kama receiver and transmitter really that finicky? I've had lots of problems with mine (I've tried two different Kama's) and I figured the problem was with wiring as opposed to signal interference... now that I think about it, my VESC is mounted to the rear of my board and I also hold the remote in my front hand. The plot thickens!
```

---
## \#83 Posted by: Moja Posted at: 2015-12-19T09:50:55.396Z Reads: 361

```
I get the same problem when I am riding on the beach with my Fik big daddy, if I am barefoot and there is moisture on my feet and I have my foot over where the receiver is mounted I loose connection. The straight line of sight range is decent with these lower grade wireless connections but they cant pass through objects at all.
```

---
## \#84 Posted by: lowGuido Posted at: 2015-12-19T10:05:30.590Z Reads: 347

```
this is interesting.. I never really thought much about front hand and back hand..
I did some experiments today with my board, rode 7km with the Kama in the front hand, and 7 in the back hand.

no difference for me.
```

---
## \#85 Posted by: Moja Posted at: 2015-12-19T10:07:01.659Z Reads: 339

```
I have my receiver inside a micro pelican case which is pretty tightly sealed with thick plastic, Im going to extend the wires and mount the receiver PCB outside the case and hopefully I get the same results.
```

---
## \#86 Posted by: lowGuido Posted at: 2015-12-19T10:08:12.232Z Reads: 341

```
mine is inside a carbon fibre moulded container, I was a bit worried about the carbon fibre blocking the signal at first, but have had no issues.
```

---
## \#87 Posted by: lowGuido Posted at: 2015-12-19T11:37:16.697Z Reads: 342

```
I wonder if there are external factors like other RF noise in the area?
```

---
## \#88 Posted by: trbt555 Posted at: 2015-12-20T17:01:11.051Z Reads: 351

```
Or maybe just the rider's own cellphone creating interference ?
Anyway, putting this small receiver antenna next to a VESC doing a lot of high frequency switching seems like asking for trouble to me.
I wonder if putting the rx further from the VESC may improve reliability.
```

---
## \#89 Posted by: Dedbny Posted at: 2016-01-06T10:34:28.837Z Reads: 363

```
Whats fhis controller? On gumtree at the moment. Looks  cool.

http://www.electric-skateboard.builders/uploads/db1493/original/2X/e/e78bb13799ac3d97dff8557c7b33d6cd04227ce3.jpg
```

---
## \#90 Posted by: lowGuido Posted at: 2016-01-06T10:42:18.209Z Reads: 356

```
link doesn't work


----------
```

---
## \#91 Posted by: trbt555 Posted at: 2016-01-06T13:11:47.484Z Reads: 343

```
Found a [working link][1].


  [1]: http://www.gumtree.com.au/s-ad/surfers-paradise/skateboards-rollerblades/worlds-most-advanced-epic-electric-skateboard-hand-controller/1098721311
```

---
## \#92 Posted by: lowGuido Posted at: 2016-01-06T13:19:15.048Z Reads: 346

```
link is fixed now as well. looks like the Rolls Royce of transmitters there..  speedo, battery indicator, flashlight.. probably controls the skateboard too!
```

---
## \#93 Posted by: longhairedboy Posted at: 2016-01-06T13:21:16.818Z Reads: 352

```
Somebody needs to buy this and tell me how it works with VESC. I want a speedometer and i like the idea of a light on the remote.
```

---
## \#94 Posted by: NIK Posted at: 2016-01-06T14:25:33.166Z Reads: 367

```
There is too little information but quite good for the functionality and not sure whether they provide international shipping:

Wireless (2.4 GHz)
Speedometer
Flashlight
Regenerative Brake
Reverse
Horn (optional)

http://www.epicelectricskateboards.com/product/hand-control-2015/
```

---
## \#95 Posted by: Dedbny Posted at: 2016-01-06T22:36:10.335Z Reads: 356

```
Not sure whether it will work with vesc  Didnt realise it was for the epic boards. Maybe someone can check with supplier to confirm. Looks like it can be shipped to US.  Found it in our local sellers website, so Epic must have had separate adv. Thought it was just a private seller,
```

---
## \#96 Posted by: lowGuido Posted at: 2016-01-07T09:36:22.035Z Reads: 353

```
I contacted the seller, he said that you need an EPIC board for it to work.
```

---
## \#97 Posted by: trbt555 Posted at: 2016-01-07T11:02:42.789Z Reads: 356

```
This is begging to be hacked.
```

---
## \#98 Posted by: longhairedboy Posted at: 2016-01-08T13:50:50.832Z Reads: 363

```
all the input hardware is in there! we could swap the board out with a gt2b board and hook the thumb control up to the trigger port. Its hackerin' time!

btw i ordered one of those things from Carvon, for science. It could potentially be sort of what i just described anyway.
```

---
## \#99 Posted by: trbt555 Posted at: 2016-01-08T16:49:30.180Z Reads: 373

```
I am actually really starting to like/trust my Kama nunchuck, it has been very reliable up to know.

BTW, doesn't the VESC take care of the dead-man-switch ? There's a timeout for no control signal received.



[quote="longhairedboy, post:98, topic:155, full:true"]
btw i ordered one of those things from Carvon, for science. It could potentially be sort of what i just described anyway.
[/quote]
Looking forward to your findings.
```

---
## \#100 Posted by: lowGuido Posted at: 2016-01-08T21:58:00.719Z Reads: 373

```
yeah, after all my testing I still only ride with the Kama.
```

---
## \#101 Posted by: lowGuido Posted at: 2016-01-31T07:26:30.938Z Reads: 362

```
hey, anyone out there ever used a GT2E??
I just realized today that I have one for my RC car and its almost identical to the GT2B from what I can tell?
```

---
## \#102 Posted by: Dedbny Posted at: 2016-01-31T09:03:41.044Z Reads: 365

```
Got one now. Just trying to find time to actually set it up with the tool, Had difficulty binding the receiver to transmitter, but think that is now good.
```

---
## \#103 Posted by: Abdulz Posted at: 2016-03-22T01:43:46.491Z Reads: 360

```
That's really reliable , it has never let me down or dropped connection over 7months
```

---
## \#104 Posted by: lowGuido Posted at: 2016-04-05T07:01:41.534Z Reads: 356

```
just worth noting that the GT2E is different internally and wouldn't fit in a bad wolf enclosure.
```

---
## \#105 Posted by: DeathCookies Posted at: 2016-04-05T14:04:31.498Z Reads: 408

```
I just bought a FlySky GT2E transmitter and i am so happy with it. I couldn't miss it.

I tried the smaller Quanum Pistol (HobbyKing) and a Nunchuck(@Hummie) and both transmitter had problems with the connection to the VESC. But now I have the GT2E and it is reliable as hell. You can start your board (VESC) and can turn on the Transmitter and you will always have a good and reliable connection.

I would assume that the GT2 transmitter series (GT2B, C, D, E) is the best transmitter with a good price about 30€.

[quote="lowGuido, post:104, topic:155, full:true"]
just worth noting that the GT2E is different internally and wouldn't fit in a bad wolf enclosure.
[/quote]

The circuit board, the trigger and that stuff is smaller in the GT2E. I found a picture of the internal:
<img src='/uploads/db1493/original/2X/1/1cc16cd4a2d91fea138cd47e800fa8aebbfb3457.jpg'>

You just need to buy one Cell LiPo Battery like this one: [One Cell LiPo][1]
and one charging board [Charging Board][2]

Then you can build a Bad Wolf Mod.

Maybe I make a Build Thread about that. Should I?


  [1]: http://www.hobbyking.com/hobbyking/store/__7649__ZIPPY_850mAh_20C_single_cell.html
  [2]: http://www.ebay.de/itm/Mini-USB-Lader-1A-Lithium-Lipo-Akku-Battery-Charging-Board-3-7V-1S-/171541621042?hash=item27f0ad6932:g:zQUAAOSwjwlXA7t2
```

---
## \#106 Posted by: MasterCho Posted at: 2016-04-05T14:43:06.766Z Reads: 397

```
try this http://www.thingiverse.com/thing:1013293
```

---
## \#107 Posted by: lowGuido Posted at: 2016-04-10T12:18:19.984Z Reads: 392

```
there you go. 

looks nice.
```

---
## \#108 Posted by: WrinklyWink Posted at: 2016-04-10T15:54:54.807Z Reads: 398

```
i made sure to read all replies before sending this message.. I have a wiiceiver and a wireless nyko kama as well and I'm curious about how you went about soldering the receiver to the wiiceiver. Did you open up the receiver? or did you just add solder onto the wiiceiver's contacts? You're right about the thickness of the wiiceiver being too thin; it wobbles a lot.
```

---
## \#109 Posted by: lowGuido Posted at: 2016-04-10T15:57:58.112Z Reads: 395

```
here's one I prepared earlier.
http://www.electric-skateboard.builders/t/opening-up-the-nyko-kama-dongle/1477
```

---
## \#110 Posted by: lox897 Posted at: 2016-04-20T12:13:10.297Z Reads: 379

```
https://instagram.com/p/BEZsp-YQ2lK/

New evolve remote has a built in display.
```

---
## \#111 Posted by: barajabali Posted at: 2016-04-20T13:56:28.725Z Reads: 362

```
Oh man.... Need.... 
20 characters blah
```

---
## \#112 Posted by: JuniorPotato93 Posted at: 2016-07-15T06:37:23.866Z Reads: 318

```
I'm having some serious issues binding the receiver once I printed a smaller enclosure for it. How did you solve your binding issues?
```

---
## \#113 Posted by: Dedbny Posted at: 2016-07-15T10:10:06.537Z Reads: 321

```
Maybe try this https://youtu.be/mVDJDHCGwQ4

Id just play around with it.  Been ages since I last tried it.
```

---
## \#114 Posted by: Monk Posted at: 2017-02-25T16:12:23.123Z Reads: 215

```
Does anyone know if this remote will work on a DIY board? Its $30 with free shipping from Indiana. I like the form factor. Does NOT come with a receiver so Id like to find out what kind of receiver would be required before I pull the trigger on one (no pun intended).
<img src="/uploads/db1493/original/3X/1/9/19868439225042f0f4654b69497d25cc20bfc120.jpg" width="666" height="500">
```

---
## \#115 Posted by: lowGuido Posted at: 2017-02-25T17:57:17.759Z Reads: 211

```
if it doesn't come with a receiver there's a fair chance you will have a hard time getting it to work.
```

---
## \#116 Posted by: Monk Posted at: 2017-02-25T20:33:13.749Z Reads: 212

```
Bummer. Knew it had to be too good to be true.
```

---
## \#117 Posted by: MannyM0E Posted at: 2018-01-26T02:14:47.068Z Reads: 97

```
How you get the GT2E to connect with the BDLC ?
```

---
