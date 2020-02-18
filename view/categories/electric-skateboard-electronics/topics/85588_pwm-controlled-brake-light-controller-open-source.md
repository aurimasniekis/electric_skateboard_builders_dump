# PWM controlled Brake light controller \[Open Source\]

### Replies: 84 Views: 1284

## \#1 Posted by: Mich21050 Posted at: 2019-02-27T17:42:40.453Z Reads: 277

```
Hi,
Ok so I have been working on a PWM controlled brake light controller for quite a while now and I think I'm finally able to release everything. The whole project is open source so feel free to build one on your own. Currently, I'm sending a few modules out for beta testing so the design might not be final.
Also huge thank you to @janpom (for his patience and help with my code) and @StefanMe (for his help regarding the buck converter). And @linsus for his PCB design input. Thank you all... :slight_smile:     
Key functions:

* 7s-13s
* uses ws2812b led strips
* 3d printed risers to mount the LEDs  (designed by @mmaner 
* turned on/off using the 3rd channel of your remote
* cheap (around 8$ in parts per unit)
* simple setup
* site: 5x5 cm 
* 5V/3A buck converter on board
* possible setup: 119 rear LEDs; 47 front LEDs, <-- absolute maximum
* horn support coming up in the future @b264 
* extension modules coming in the future (USB breakout, horn support and so on...: slight_smile:) 
* programmable/updateable via an FTDI breakout board
* works with any kind of esc

Pictures:
![20190227_183614|690x388](upload://6wCOhtFOEoKeVFHZ7ugofEZjUyo.jpeg) 
Apple for scale :smile:

V1 vs V2 (again Apple for scale)
![20190227_183832|690x388](upload://yCafBql3YEcLuvYsA2roHzZtOLx.jpeg) 

Video: (coming up) :slightly_smiling_face:

 
I might sell a few in the future... Let's see.. :slight_smile:
Schematic/PCB:  https://easyeda.com/mich21050/light_controll_smd
Code (still need to write the instructions): https://github.com/Mich21050/Brake_Lights/blob/master/README.md 
3D Riser (holds up to 8 LEDs): https://www.thingiverse.com/thing:3457234 

If anybody got any suggestions/comments just tell me. :joy:
Thanks for reading and I hope there's some interest in these.. :slight_smile:
```

---
## \#2 Posted by: Grozniy Posted at: 2019-02-27T17:44:00.639Z Reads: 243

```
Looks promising
```

---
## \#3 Posted by: janpom Posted at: 2019-02-27T19:33:00.971Z Reads: 231

```
So are we using apples now? I thought a banana was the standard. You can't stop the progress. :smile:
```

---
## \#4 Posted by: janpom Posted at: 2019-02-27T19:33:52.303Z Reads: 223

```
BTW, it looks very cool. Looking forward to the video.
```

---
## \#5 Posted by: venom121212 Posted at: 2019-02-27T19:40:37.211Z Reads: 215

```
Sounds like a great product! This area needs to be filled
```

---
## \#6 Posted by: Mich21050 Posted at: 2019-02-27T19:43:11.199Z Reads: 218

```
I couldn't find any bananas... :slight_smile: :joy:
Sorry @moon :frowning:
```

---
## \#7 Posted by: janpom Posted at: 2019-02-27T19:44:45.006Z Reads: 210

```
We should probably add the banana to [this list](https://www.electric-skateboard.builders/t/these-items-should-be-in-the-drawer-of-any-esk8-builder/53066).
```

---
## \#8 Posted by: Mich21050 Posted at: 2019-02-27T19:45:41.337Z Reads: 203

```
Yep. Definitely @Eboosted might have to add that... :slight_smile:
```

---
## \#9 Posted by: brenternet Posted at: 2019-02-27T19:51:02.676Z Reads: 207

```
Bear with me a second while I explain my stupidity here.

I was about to ask what the time difference was between v1 and v2 because that was the same apple and it kept well. Then I realized you took the two pictures at the same time andicriedinside.

Looks sweet. @fottaz Alberto has been selling something like this for a while now (not exactly the same of course) but the price was prohibitive for me. https://eskating.eu/product/6w-waterproof-led-light-kit-with-rear-brakes-control/
```

---
## \#10 Posted by: Mich21050 Posted at: 2019-02-27T19:56:15.776Z Reads: 200

```
Just out of curiosity :slight_smile:
Any interreset in a small group buy? One unit would cost around 13$ +shipping :slight_smile:
[poll type=regular results=always public=true]
* Yes 
* No
* I don't give a flying f*ck :)
[/poll]
```

---
## \#11 Posted by: StefanMe Posted at: 2019-02-27T19:59:48.577Z Reads: 196

```
Maybe I just dont see it, but where is the Shottkey diode between output and ground?

![image|690x318](upload://dinwDzQocDgViMxLkVF5b0aZhW0.jpeg)

Also the 100uH coil is wrong if u use the 5V version. 100uH is for the 12V I use on my FeatherReceiver because of the better efficiency factor...
```

---
## \#12 Posted by: akhlut Posted at: 2019-02-27T20:03:21.349Z Reads: 190

```
Questions!

CH3 - only switched the headlight on and off - the brakelight is something that should be on whenever the board is on.  Is this the behavior?

Brakelight - always on at 50% brightness, then when brake is applied full brightness.  Is this the behavior?

This is a great start!
```

---
## \#13 Posted by: Mich21050 Posted at: 2019-02-27T20:11:34.553Z Reads: 185

```
[quote="akhlut, post:12, topic:85588"]
CH3 - only switched the headlight on and off - the brakelight is something that should be on whenever the board is on. Is this the behavior?
[/quote]
CH3 switches on/off the whole light system. Headlight/brake light

[quote="akhlut, post:12, topic:85588"]
Brakelight - always on at 50% brightness, then when brake is applied full brightness. Is this the behavior?
[/quote]

Right now it's always off until you apply brakes... But I'm working on a new version which will implement exactly that behavior. The advantage of the atmega328p is that you can update it via an FTDI breakout.. :slight_smile:
```

---
## \#14 Posted by: akhlut Posted at: 2019-02-27T20:12:44.188Z Reads: 173

```
Is good!

And +1 for open source!
```

---
## \#15 Posted by: Mich21050 Posted at: 2019-02-27T20:13:31.271Z Reads: 179

```
[quote="StefanMe, post:11, topic:85588"]
Maybe I just dont see it, but where is the Shottkey diode between output and ground?
[/quote]
I just took this part of the datasheet.. :slight_smile:

[quote="StefanMe, post:11, topic:85588"]
Also the 100uH coil is wrong if u use the 5V version. 100uH is for the 12V I use on my FeatherReceiver because of the better efficiency factor…
[/quote]
According to the datasheet not... :slight_smile:
![Screenshot_1|690x370](upload://wDH9GA149xBFkIkUIjiWgB8h8KT.png)
```

---
## \#16 Posted by: Mich21050 Posted at: 2019-02-27T20:17:17.638Z Reads: 176

```
[quote="akhlut, post:14, topic:85588"]
And +1 for open source!
[/quote]

Thanks. I just think it's fair to publish it. This community is awesome and I think open source is very important to keep the progress going... :slight_smile:
```

---
## \#17 Posted by: pjotr47 Posted at: 2019-02-27T21:24:38.006Z Reads: 176

```
Yeah I want to buy one for testing :slight_smile:
```

---
## \#18 Posted by: Therealesk8 Posted at: 2019-02-27T21:28:37.806Z Reads: 179

```
Nice work🙌❤️
It will be very nice to test it. 🙂
```

---
## \#19 Posted by: visnu777 Posted at: 2019-02-27T21:40:52.268Z Reads: 170

```
I want one too :) I bought a ws2812b led strip for the Photon remote which I didn't get in the end so now I have the chance to finally use it in the same way I wanted to before :) Thanks Mich :)
```

---
## \#20 Posted by: banjaxxed Posted at: 2019-02-27T22:37:08.198Z Reads: 166

```
You can’t compare 🍎 🍎  to  🍌 🍌 

What’s next? 🍉
```

---
## \#21 Posted by: Slak Posted at: 2019-02-27T23:54:22.665Z Reads: 163

```
Nice job, it's a good start, dude. Didn't try it yet but, by code review, my advice would be to implement a Schmitt trigger :) Pretty simple and efficient to solve threshold issue (blinking around threshold values) on PPM.

If you need help, I can give you my code, it has light ON/OFF separate from braking light by using events system.
```

---
## \#22 Posted by: Mich21050 Posted at: 2019-03-07T20:00:38.986Z Reads: 140

```
Ok, so if anybody is still interested here we go.... just a little update:

So right now I have three beta testers ( I think :slight_smile:) @mmaner @b264 and @Bor.inc . I still need to resolder the capacitors bc the solder paste didn't melt properly.. I'm still looking for two more (maybe @pjotr47 ? :wink:) After those tests were successful I'm going to organize a small GB for people who are interested.. 

Just out of curiosity... What option for updating would you prefer? An external FTDI breakout board or an integrated one (maybe even USB-C; but that would increase the price a bit) :slight_smile: 

Thanks for reading :smile:
```

---
## \#23 Posted by: venom121212 Posted at: 2019-03-07T20:05:26.560Z Reads: 133

```
As long as it's waterproof, I don't mind either option
```

---
## \#24 Posted by: Mich21050 Posted at: 2019-03-07T20:08:00.904Z Reads: 132

```
[quote="venom121212, post:23, topic:85588"]
As long as it’s waterproof,
[/quote]

You want it waterproof?... :sweat_smile:
I could conformal coat it which should give make it waterproof but no guarantees... :slight_smile:
```

---
## \#25 Posted by: pjotr47 Posted at: 2019-03-07T20:09:52.614Z Reads: 134

```
Haha yeah ! I am in :) 
I have just finished my [project](https://vimeo.com/user95946235/review/322072286/e57cd06e32) for my trampa lights that I can control with the nano x. But I have a small penny/longboard in progress that want some lights :blush:

@Mich21050 do you have tested your board with the nano x? because after some testing, I have discovered that after pressing + -10 seconds of the second channel button the receiver on channel 2 goes from 0v to 3.1v. if you press the button again for 10 seconds, the 3.1v goes back to 0v
```

---
## \#26 Posted by: venom121212 Posted at: 2019-03-07T20:10:20.528Z Reads: 132

```
Any electronics under my deck must be water resistant imo
```

---
## \#27 Posted by: Skunk Posted at: 2019-03-07T20:11:03.126Z Reads: 125

```
How have i missed this thread until now....
Very cool.  I want
```

---
## \#28 Posted by: Mich21050 Posted at: 2019-03-07T20:11:27.793Z Reads: 126

```
Btw: Video is going up as soon as I get my goddamn TB trucks...
```

---
## \#29 Posted by: Skunk Posted at: 2019-03-07T20:12:06.722Z Reads: 128

```
I saw that edit
```

---
## \#30 Posted by: Mich21050 Posted at: 2019-03-07T20:12:38.347Z Reads: 130

```
Alright. I can conformal coat them upon request... :slight_smile:
```

---
## \#31 Posted by: akhlut Posted at: 2019-03-07T20:15:15.347Z Reads: 124

```
External FTDI

Cheap, easy and dead simple.  

Easier to assemble, less complexity, less to go wrong, easier to troubleshoot.
```

---
## \#32 Posted by: Mich21050 Posted at: 2019-03-07T20:15:53.234Z Reads: 123

```
[quote="pjotr47, post:25, topic:85588"]
@Mich21050 do you have tested your board with the nano x? because after some testing, I have discovered that after pressing + -10 seconds of the second channel button the receiver on channel 2 goes from 0v to 3.1v. if you press the button again for 10 seconds, the 3.1v goes back to 0v
[/quote]

Nope. I don't have a nano-x... :slight_smile: But would you be so kind and test it once you get your board... :slight_smile:
@pjotr47
```

---
## \#33 Posted by: pjotr47 Posted at: 2019-03-07T20:19:49.173Z Reads: 126

```
Haha I saw your tracking from the shipping.... you don't want to know how long I have waited on a package from the US.... 

![image|243x500](upload://nWcv6zwnjYWBeuIJLLk2B90BsBM.png)
```

---
## \#34 Posted by: pjotr47 Posted at: 2019-03-07T20:20:17.263Z Reads: 121

```
[quote="Mich21050, post:32, topic:85588"]
Nope. I don’t have a nano-x… :slight_smile: But would you be so kind and test it once you get your board… :slight_smile: @pjotr47
[/quote]

Yeah no probs! I can test it for you :)
```

---
## \#35 Posted by: Mich21050 Posted at: 2019-03-07T20:21:52.705Z Reads: 121

```
Alright... I will stop complaining... :joy:
What did you order/where? :slight_smile:
```

---
## \#36 Posted by: pjotr47 Posted at: 2019-03-07T20:23:23.115Z Reads: 123

```
It were the parts from the groupbuy with hyperion
```

---
## \#37 Posted by: Bor.inc Posted at: 2019-03-07T20:30:25.253Z Reads: 123

```
Looking forward to it! I will print the files you have on thingiverse tomorrow just for fun and try them out :slight_smile:
```

---
## \#38 Posted by: Mich21050 Posted at: 2019-03-07T20:40:30.812Z Reads: 127

```
[quote="pjotr47, post:25, topic:85588"]
@Mich21050 do you have tested your board with the nano x? because after some testing, I have discovered that after pressing + -10 seconds of the second channel button the receiver on channel 2 goes from 0v to 3.1v. if you press the button again for 10 seconds, the 3.1v goes back to 0v
[/quote]

Wait... WHAT? If you press the ch2 button instead of a PWM signal it outputs a constant voltage? :slight_smile:
@pjotr47
```

---
## \#39 Posted by: pjotr47 Posted at: 2019-03-07T20:46:00.847Z Reads: 124

```
Yeps 10char
```

---
## \#40 Posted by: Mich21050 Posted at: 2019-03-07T20:48:20.907Z Reads: 121

```
Are you sure? Do you have an oscilloscope to verify that? You could also use an Arduino... :slight_smile:
Because that would be an odd behavior...
```

---
## \#41 Posted by: pjotr47 Posted at: 2019-03-07T20:51:52.139Z Reads: 110

```
[quote="Mich21050, post:40, topic:85588"]
Are you sure?
[/quote]
Yeah, I have tested it many times with a voltage meter. Also the program that I use on the arduino to run my lights in my trampa is based on the 3.1v signal.

Do you have a link how I can use a arduino like oscilloscope ?
```

---
## \#42 Posted by: Mich21050 Posted at: 2019-03-07T20:52:45.024Z Reads: 113

```
Just get my PWM_Readout Arduino Code from my Github... :slight_smile:

[quote="pjotr47, post:41, topic:85588"]
like oscilloscope ?
[/quote]
It wouldn't act as an oscilloscope... It just reads out the PWM value...
```

---
## \#43 Posted by: venom121212 Posted at: 2019-03-07T20:56:54.216Z Reads: 114

```
Trade Nano x for one of these kits whenever? 
:grin:
I can include a Nano V2 if it helps free of charge
```

---
## \#44 Posted by: Mich21050 Posted at: 2019-03-07T20:57:47.574Z Reads: 112

```
Nope sorry... :frowning:

I don't like the nano-x... Especially after I saw your gif :slight_smile:
```

---
## \#45 Posted by: venom121212 Posted at: 2019-03-07T20:58:19.383Z Reads: 115

```
Oh it would certainly come with a never ever ever fucking use except for bench testing warning hahaha
```

---
## \#46 Posted by: pjotr47 Posted at: 2019-03-07T21:05:10.296Z Reads: 121

```
Channel 1

Gas
![image|690x272](upload://nmt9T9oRTi9eLzFKqgWrsHdV03y.png) 
neutral
![image|690x279](upload://gMD4e9O3OQw8NZkWOPYMFTUlJsf.png) 
Brake
![image|690x274](upload://gYQU6i22j1Cz19FRvS81nORjxfY.png) 


Channel 2:
same if I push the button
![image|690x271](upload://uVH1DsXUzZ2y5iuVcMcYuSdZk2Z.png)
```

---
## \#47 Posted by: akhlut Posted at: 2019-03-07T21:09:04.794Z Reads: 111

```
GT2B CH3 does not latch
```

---
## \#48 Posted by: Mich21050 Posted at: 2019-03-07T21:13:02.450Z Reads: 109

```
Alright.. Will take a look at that... :slight_smile:
```

---
## \#49 Posted by: Mich21050 Posted at: 2019-03-07T21:13:31.185Z Reads: 110

```
It does. My HK gt2b stays at 1200 or something like that... :slight_smile:
```

---
## \#50 Posted by: akhlut Posted at: 2019-03-07T21:14:44.875Z Reads: 115

```
huh.  I had to add a switch to get it to latch for me.

https://hobbyking.com/en_us/turnigy-receiver-controlled-switch-1.html
```

---
## \#51 Posted by: Mich21050 Posted at: 2019-03-07T21:15:55.628Z Reads: 113

```
Strange. Mine latches...
```

---
## \#52 Posted by: akhlut Posted at: 2019-03-07T21:17:10.904Z Reads: 112

```
Maybe it does.  I am an idiot more often than not.  :/
```

---
## \#53 Posted by: Mich21050 Posted at: 2019-03-07T21:19:14.905Z Reads: 109

```
Could you try doing exactly the same as @pjotr47? :slight_smile:
```

---
## \#54 Posted by: Vanarian Posted at: 2019-03-07T21:28:28.111Z Reads: 104

```
That's a cool project !
```

---
## \#55 Posted by: floyd Posted at: 2019-03-07T21:34:49.678Z Reads: 103

```
I can test if you need another tester :)
```

---
## \#56 Posted by: akhlut Posted at: 2019-03-07T21:44:52.567Z Reads: 106

```
If I can find the time!

:frowning:

Busy as a one-armed paper hanger atm.
```

---
## \#57 Posted by: Mich21050 Posted at: 2019-03-07T21:45:52.179Z Reads: 101

```
Sure no problem. Just send me the results once you tried it...  :slight_smile:
```

---
## \#58 Posted by: b264 Posted at: 2019-03-07T22:24:19.050Z Reads: 108

```
[quote="Mich21050, post:24, topic:85588"]
You want it waterproof?.. :sweat_smile: I could conformal coat it which should give make it waterproof but no guarantees… :slight_smile:
[/quote]

I will conformal coat mine, as with everything.  But coming with conformal coat is never bad.  You can't have too much waterproofing
```

---
## \#59 Posted by: StefanMe Posted at: 2019-03-08T11:39:05.360Z Reads: 107

```
I destroyed the 100% poll :smiley: not really on purpose... 

Awesome work. Looks cool! Is there any video to see it in real life?
```

---
## \#60 Posted by: Mich21050 Posted at: 2019-03-08T13:29:38.935Z Reads: 110

```
[quote="StefanMe, post:59, topic:85588"]
I destroyed the 100% poll :smiley: not really on purpose…
[/quote]

https://media.giphy.com/media/Ty9Sg8oHghPWg/giphy.gif

[quote="StefanMe, post:59, topic:85588"]
Awesome work. Looks cool! Is there any video to see it in real life?
[/quote]
Thank you. I will upload one as soon as I get my goddamn TB trucks... :slight_smile:

@StefanMe
```

---
## \#61 Posted by: StefanMe Posted at: 2019-03-08T13:31:47.932Z Reads: 103

```
i have one set here laying around... :wink: Where are u from? Wien ist leider ein bisschen zu weit weg von München...
```

---
## \#62 Posted by: Mich21050 Posted at: 2019-03-08T13:33:29.808Z Reads: 103

```
Ja. Leider. I ordered them already but USPS seems to take ages.. Once I get them I can finish my build and upload some videos of it working.. :slight_smile:
```

---
## \#63 Posted by: Andy87 Posted at: 2019-03-08T13:37:50.470Z Reads: 102

```
[quote="Skunk, post:27, topic:85588, full:true"]
How have i missed this thread until now… Very cool. I want
[/quote]
...same here.... 🙈
```

---
## \#64 Posted by: Sn4pz Posted at: 2019-03-21T19:16:41.235Z Reads: 85

```
Any support for trampa? :D 

Interested in incorporating this into my build
```

---
## \#65 Posted by: b264 Posted at: 2019-03-21T19:37:52.820Z Reads: 84

```
These connect to a PWM ("PPM") RC receiver, not an ESC
```

---
## \#66 Posted by: Mich21050 Posted at: 2019-03-21T20:26:53.291Z Reads: 86

```
@b264 is right. Those modules are completely independent of any kind if esc. You only need a "PPM" remote...

On a whole other note: Anyone interested in small MOSFET modules to drive other lights than a led strip (something more powerful)? :slight_smile:
```

---
## \#67 Posted by: Sn4pz Posted at: 2019-03-21T20:32:45.509Z Reads: 88

```
You're right, this is just the controller, my bad. I thought it was a complete system
```

---
## \#68 Posted by: Bor.inc Posted at: 2019-03-21T21:43:06.659Z Reads: 88

```
yess please! What i also said earlier is that selling just the boost converter (7s-13s to 12v) is also a nice thing to do because its hard to find a good one (and efficient probably)
```

---
## \#69 Posted by: Mich21050 Posted at: 2019-03-21T21:45:27.728Z Reads: 86

```
Completely forgot about that... Sorry, I think I will be able to release it tomorrow. :slight_smile:
```

---
## \#70 Posted by: Bor.inc Posted at: 2019-03-21T21:46:58.717Z Reads: 87

```
ah realy no problems, im just trying to give you some thoughts (so you maybe can make a bit more money haha) and you can do whatever you want with it
```

---
## \#71 Posted by: pjotr47 Posted at: 2019-03-21T21:58:08.596Z Reads: 92

```
:wink: 

https://s.click.aliexpress.com/e/5JgIyXI

If you need more power: 

https://s.click.aliexpress.com/e/bXOL1bwC

@Mich21050 sorry to steal your topic 🙈
```

---
## \#72 Posted by: Mich21050 Posted at: 2019-03-21T21:59:08.470Z Reads: 90

```
Don't steal my customers... :joy: :wink:

JK :smile:
@pjotr47
```

---
## \#73 Posted by: Mich21050 Posted at: 2019-04-22T19:10:06.748Z Reads: 82

```
Sorry for my lack of updates but school has just been a pain in the a***.\
I'm still looking for beta tester, to be exact 6 persons preferably within the EU since shipping to the US is really expensive (10€). Sorry @b264 .\
 One unit would cost 15USD. :slight_smile:. \
Each unit would require some minor soldering (ppm receiver cables) :slight_smile:\
Just pm me if you would like to participate. (@pjotr47 maybe) :slight_smile:
```

---
## \#74 Posted by: Bor.inc Posted at: 2019-04-22T19:21:10.829Z Reads: 79

```
Hype! :slight_smile: 10char
```

---
## \#75 Posted by: b264 Posted at: 2019-04-22T19:42:59.963Z Reads: 76

```
I'd cover the shipping ;-)
```

---
## \#76 Posted by: Jamie42 Posted at: 2019-04-22T20:17:12.586Z Reads: 74

```
Me just doing this with an arduino :laughing:
```

---
## \#77 Posted by: pjotr47 Posted at: 2019-04-22T21:36:21.460Z Reads: 66

```
You have a pm
```

---
## \#78 Posted by: Mich21050 Posted at: 2019-04-22T21:40:27.172Z Reads: 70

```
Nice... pm'ed. :slight_smile:
```

---
## \#79 Posted by: Okami Posted at: 2019-04-23T11:22:44.825Z Reads: 66

```
So are there any photos / videos of this?

Looks promising.. im from EU but i need to get convinced whenever I need stop light or not, though I really love the idea because of added safety, especially when riding in groups
```

---
## \#80 Posted by: Mich21050 Posted at: 2019-04-23T11:46:12.000Z Reads: 65

```
[quote="Okami, post:79, topic:85588"]
So are there any photos / videos of this?
[/quote]
No, not right now. My build is currently out of commission since I need a new deck and one of my tires popped... :slight_smile:\
But I cam film a short bench test video if you would like.... :slight_smile:
```

---
## \#81 Posted by: Okami Posted at: 2019-04-23T13:36:45.999Z Reads: 62

```
Yeh, even if idea is clear would be nice to see it in action.
```

---
## \#83 Posted by: Mich21050 Posted at: 2019-05-21T17:11:28.549Z Reads: 50

```
So, I finally have some time after my "exam" phase. I'm currently not really sure where to go with this project, so I would need some feedback from you guys:

1. Is there even any interest in this?
2. I'm thinking about turning this into an "esk8duino". So like a small Arduino with an onboard buck converter and maybe an FTDI chip and a few MOSFETs.

I would greatly appreciate your opinion. :slight_smile:\
Thanks for reading... :slight_smile:
```

---
## \#84 Posted by: Mich21050 Posted at: 2019-05-25T16:12:48.201Z Reads: 43

```
Still looking for 2 beta tester's. :slight_smile:\
If you are interested just pm me.
```

---
## \#85 Posted by: Snehith Posted at: 2019-06-15T04:31:31.395Z Reads: 30

```
What's the update on this project @Mich21050  ?
```

---
