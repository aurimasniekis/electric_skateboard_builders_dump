# Can I use my Boosted Board controller and replace the electronics inside for my DIY build?

### Replies: 34 Views: 7944

## \#1 Posted by: shunpo Posted at: 2016-07-03T15:53:02.274Z Reads: 335

```
Long time lurker. 

I sold my Boosted Board so I can pursue the DIY life, as I wanted to have my own touch and look and MORE Range, I can't stress how bad the range on BB was... So I've got wood to make my own deck and already bought all my parts, just need an enclosure and remote. I still have a Boosted Board remote, and thought, why not just use that? Could I crack it open and replace it with other electronics so it works with my build? 

I already bought a VESC and a motor from Enertion, and I'm gonna be using 18650 batteries. It's gonna be a single motor build.
```

---
## \#2 Posted by: ArmandR Posted at: 2016-07-03T17:46:42.285Z Reads: 326

```
Anything is possible.
```

---
## \#3 Posted by: shunpo Posted at: 2016-07-03T18:05:18.776Z Reads: 318

```
Aha, indeed. On a more serious note, do you actually know how or know of anyone who's done it or has knowledge in doing so?
```

---
## \#4 Posted by: michaeld33 Posted at: 2016-07-03T18:07:29.120Z Reads: 310

```
I don't know of anyone who has done it, but I am fairly confident that it can be done, you just need the right stuff. I would gut the entire thing and just use the case, the knob and the trigger. and then use my own PCB or arduino.
```

---
## \#5 Posted by: shunpo Posted at: 2016-07-03T18:20:51.815Z Reads: 298

```
That's what I was thinking. I love how it feels and use whole wheel thingy system, so I'd love to maintain that comfort. I'll probably keep the casing the trigger system and put new electronics in.
```

---
## \#6 Posted by: ArmandR Posted at: 2016-07-03T18:33:03.990Z Reads: 287

```
No, it's pretty hard.
```

---
## \#7 Posted by: chris_13 Posted at: 2016-07-03T22:31:18.493Z Reads: 274

```
you could maybe use a remote from torque boards and modify it so, that it would fit the case... but if you would buy such a remote it would not make a lot of sense to modify it...
```

---
## \#8 Posted by: DougM Posted at: 2016-07-03T22:48:28.336Z Reads: 273

```
it looks like it's been reverse engineered:

https://www.wired.com/2015/08/hackers-can-seize-control-of-electric-skateboards-and-toss-riders-boosted-revo/

so could you use the remote as-is and build a BT+Arduino receiver that decodes and converts to VESC compatible commands?

Admittedly not easy, but maybe easier than designing/fitting a custom board in the housing.
```

---
## \#9 Posted by: Stevemk14ebr Posted at: 2016-07-03T23:48:45.901Z Reads: 259

```
They added aes encryption after that article so good luck. If you could rip out the hardaware receiver too you may get it to work but the whole thing is a longshot
```

---
## \#10 Posted by: cjoliver Posted at: 2016-07-04T00:30:35.593Z Reads: 245

```
You could use the battery and sliding mechanism with another mcu, like the arduino so you can have the same "feel" of controller. Trying to reverse engineer the prebuilt commands is possible but harder than the former.
```

---
## \#11 Posted by: Stevemk14ebr Posted at: 2016-07-04T00:58:44.530Z Reads: 230

```
Oliver is on the right track. If you stuck an arduino in rhe controller it'd be really easy. I've controlled my board with an arduino before its like 3 lines of code, just google control servo with arduino, you have to use the pulsein command and an equivalent to write since our boards use pulse widths as the control mechanism.
```

---
## \#12 Posted by: cjoliver Posted at: 2016-07-04T03:58:32.908Z Reads: 218

```
If you posted pictures of the internal parts of the controller here, I'm sure myself and others could point you in the right direction
```

---
## \#13 Posted by: michaeld33 Posted at: 2016-07-04T05:00:39.389Z Reads: 221

```
May be wrong, but I wasn't aware they had updated the bluetooth hack... Spoke with them a couple weeks ago and they stated that there were more issues than they originally thought and therefore never released the software version 2.0, still in dev.
```

---
## \#14 Posted by: shunpo Posted at: 2016-07-04T05:24:36.709Z Reads: 213

```
I don't have the remote with me but a quick google search yielded some good results:

http://m.imgur.com/pvtnqSr.jpg
```

---
## \#15 Posted by: DougM Posted at: 2016-07-04T15:20:51.118Z Reads: 199

```
That's a nice big circuit board - it goes under the battery, so presumably there's space on the other side as well.

if you did a double-sided repro of that it would be pretty easy to fit everything you want on there.  It would take some time but really is just a BT and an integrated arduino of some sort.  And a LiPo charge chip.
```

---
## \#16 Posted by: shunpo Posted at: 2016-07-04T16:37:02.034Z Reads: 188

```
So, I've never done anything like this. What would be the action here? Take out the board, replace it with other components? Or add to the board?
```

---
## \#17 Posted by: DougM Posted at: 2016-07-04T16:53:24.343Z Reads: 209

```
Yes, take out the board, replace it with another board that has a processor that you can program, a BT chip, a LiIo charge chip and the proper connections to the thumbwheel and some kind of power switch and any other features the handheld has that you want to replicate.

If you're not skilled in electronics you're going to need to find someone who is.
```

---
## \#18 Posted by: shunpo Posted at: 2016-07-13T21:34:59.702Z Reads: 202

```
@DougM and everyone else who read this thread, I finally got to open my remote and got some pictures of the board, the housing, and all the parts. So here they are. What do you guys think, is it possible to mod this with the Arduino? 

http://puu.sh/q0H2u/cdccebec69.jpg

.

http://puu.sh/q0H22/c4e4110c1f.jpg

.

http://puu.sh/q0H1j/d31ce5097e.jpg

.

http://puu.sh/q0H0b/ccfb3e1047.jpg

.

http://puu.sh/q0GZj/69c90803b8.jpg

.

http://puu.sh/q0GYe/8241ecf223.jpg
```

---
## \#19 Posted by: Stevemk14ebr Posted at: 2016-07-13T21:40:51.429Z Reads: 188

```
It doesnt matter what is inside. We were saying replace their electronics with an arduino.
```

---
## \#20 Posted by: shunpo Posted at: 2016-07-13T21:43:51.336Z Reads: 191

```
Will it fit? I Googled it, but saw it's kinda large, could you link me to a tiny one? Cheers.
```

---
## \#21 Posted by: Stevemk14ebr Posted at: 2016-07-13T22:00:31.683Z Reads: 179

```
The actual board is large but that isn't what you would put in there. You would buy the ic they put in the arduinos and you'd make your own circuit that would fit in there. If you dont know electronics id stop now.
```

---
## \#22 Posted by: DougM Posted at: 2016-07-14T02:38:24.991Z Reads: 174

```
mod it?  no.  You'd have to design your own custom replacement board.  However, it sure looks like there's lots of space so could you fit a custom Arduino-based board in there?  Yes.

But again, this is a job for someone who really knows electronics.
```

---
## \#23 Posted by: cjoliver Posted at: 2016-07-14T03:11:44.082Z Reads: 176

```
Well good news is the mechanical parts that give the controller its "feel" are separate from the pcb, so you could take everything out and put a custom one in! From the picture I see a buzzer, battery, and the BR LE4(Bluetooth thing).

May be worth looking into reprogramming the chip as you only need to buy a little more hardware, but the programming would be C++ without a whole lot of support
http://www.blueradios.com/nBlue%20BR-LE4.0-S2%20Summary%20Datasheet.pdf

Or find an Arduino as it's noob friendly if you're not too experienced in electronics, salvage some parts like the battery and buzzer
```

---
## \#24 Posted by: jacobbloy Posted at: 2016-08-12T09:43:19.069Z Reads: 162

```
Just the one thing that's cool is the boosted board remote uses a hall sensor for the trigger so no pot making it actually really simple to use the same mech.

I did some packet sniffing with the remote and board and I could get the vesc to work with it, it's the pairing that is the problem.
```

---
## \#25 Posted by: shunpo Posted at: 2016-09-08T09:35:32.177Z Reads: 157

```
Hey, sorry for the late reply. So you got it to sorta work I guess? Do you think it's viable to use? Or should I just get something like an Enertion remote or GT2B?
```

---
## \#26 Posted by: michaeld33 Posted at: 2016-09-08T11:29:23.549Z Reads: 151

```
If I had one I would do it, just use an arduino pro mini with a btle module...
```

---
## \#27 Posted by: mrpj Posted at: 2016-09-16T11:31:12.124Z Reads: 146

```
I am currently working on a DIY solution and I pretty much liked the form factor boosted (and stary) offer. Thank you for the pictures of the inside of the boosted remote, it provides me with some inspiration for designing my own case.

The groundwork for the schematic is done (charging, battery protection, usb connection and microcontroller IOs) - I am currently reevaluating the choice of micro controller (currently esp8266) and communication (esp8266 onboard wifi with wpa2). 

I am not sure how current boosted remotes handle their communication (and safeguarding it) - but with any homebrew solution I would be careful picking some modules for your own safety. (See @DougM link to the "hacked boosted board")
 
Most "consumer" available bluetooth or other communication modules do not offer encryption for the communication and it would be easily intercepted and manipulated. Hence I am considering to use wifi , even though the wifi band is conquested in most cities. On the other hand, chips like the esp8266 have the wifi protocol stack embedded and during my testing seemed to be pretty efficient dealing with interference. (Still have to test some more) - Good thing is, that besides the physical layer, the inbuild tcp stack of the esp8266 provides a reliable network layer, which again helps to improve reliability of cummincation. 

Another option to consider for your home project would be some microcontroller (avr / arduino) with RFM69HCW modules. They use either the 433 Mhz or 868/926 ISM Band - less conquested and also offer AES128bit encryption - while not as strong as wpa2 - for everyday usage it should be sufficient. The downside of this module is however, you need a "large" Antenna to be fit into your casing

Anyhow - if anyone would be interesting working together on a DIY remote, send me a message. Even if is just to bounce off some ideas and thoughts. I am also looking for someone helping with the casing part for the remote - I am more an electronics guy and haven`t done much with 3d printing yet
```

---
## \#28 Posted by: DougM Posted at: 2016-09-16T17:24:56.059Z Reads: 127

```
Are you making this to sell?  or as a one-off?
```

---
## \#29 Posted by: boards Posted at: 2016-09-16T18:05:30.805Z Reads: 126

```
i do not trust wifi as a communication method.
```

---
## \#30 Posted by: Pantologist Posted at: 2016-09-16T18:41:13.448Z Reads: 119

```
How the hell does the thumb wheel function?
```

---
## \#31 Posted by: mrpj Posted at: 2016-09-16T18:45:59.747Z Reads: 122

```
@DougM 'd like to publish it as open source. Depending on the state of the design and the interest at some point a group buy for cheaper parts could be possible. Or if someone could provide contacts for low quantity production somewhere in asia we could arrange a small group buy for that - but that's a couple of weeks/months down the road when working prototypes have been built. 

 
@boards
 Well the thing is, bluetooth and wifi share the same frequency band(s) (2.4 GHZ range) - so both will have to deal with interference and congestions in these frequency bands. If you compare the bluetooth stack against the wifi stack, the wifi stack provides a far more robust protocol (imho). Additionally consider wifi's wpa2 security mechanism - which is again more robust then current bluetooth implementations. AFAIK wifi`s specifiaction also allow for more power (200mv vs 100mw of bluetooth). 
Anyhow - as I said - both will be affected by 2.4 ghz congestion in cities. To avoid that issue it would be best to switch to a different frequency band. Which requires different design considerations (i.e. antenna design in small spaces).

@Pantologist
It`s a simple hall effect sensor - see https://en.wikipedia.org/wiki/Hall_effect_sensor

Edit: I just wonder why they decided to use two magnets - one should be sufficient for detecting the movement (magnet moves closer to sensor, or moves away) - might help with magnetic interference though
```

---
## \#32 Posted by: Pantologist Posted at: 2016-09-16T18:53:56.970Z Reads: 116

```
Thanks. I was pretty confused.. don't the Winning and mini remote use potentiometers or something for the thumb control?
```

---
## \#33 Posted by: mrpj Posted at: 2016-09-16T18:59:03.771Z Reads: 118

```
I am not sure about these - but you can use both (potentiometer and hall sensor) for that matter. Most joysticks in gamepads (i.e. the nun chuck) use potentiometers. ([example](http://www.compareelectronicsprices.uk/product/fb034582-a-analog-stick-joystick-thumbstick-potentiometer-microsoft-xbox-one-controller/b019yh1l1q/9df/). But in the end it does not matter - what you want to have is a way to measure the effect a physical interaction creates. So here it is either the changing resistance in a potentiometer, or the change of magnetic field with the hall sensor - the change is always in relation to a point you define as neutral.
```

---
## \#34 Posted by: michaeld33 Posted at: 2016-09-17T02:27:31.719Z Reads: 114

```
Yes, they do.
```

---
