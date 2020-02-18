# Vedder&rsquo;s VESC 6.0

### Replies: 1272 Views: 97164

## \#1 Posted by: chaka Posted at: 2016-05-25T13:42:19.458Z Reads: 2442

```
Vedder released the first images yesterday! The new version is a 2 piece design with Direct Fets and heat sink. This unit also use the DRV8301 since TI seems to be phasing out the 8302 on the original VESC. Ben has put a lot of effort into making a more robust design and it should also work on a wider range of motors. This version will have a much higher constant current rating virtually ending the overheating issues faced with the older modules.

Vedder should begin testing in a couple of weeks. Lets all wish him luck and if you can, send him a little support. ;) http://vedder.se/2015/01/vesc-open-source-esc/

<img src="/uploads/db1493/original/2X/a/aafc16f6931df802f06bc276469d0314194c2993.png" width="503" height="500">
<img src="/uploads/db1493/original/2X/9/94a707f2ae50a99df3fbf0b5fe0b99086a5d5470.png" width="532" height="500"><img src="/uploads/db1493/original/2X/e/e067d7f086f771cf8655c5fe1f4f7d379d5482e2.png" width="532" height="500"><img src="/uploads/db1493/original/2X/2/2f86b0adeee26f0942257f3e62fed7b8ab7eb024.png" width="526" height="500"><img src="/uploads/db1493/original/2X/4/46e70e87094790d4d89b24008e7abdc971905f4d.png" width="512" height="499">
```

---
## \#2 Posted by: akira Posted at: 2016-05-25T13:44:13.576Z Reads: 1834

```
Do you think it is possible to solder the directFET with regular hot air gun or do you need a reflow oven ?
```

---
## \#3 Posted by: chaka Posted at: 2016-05-25T13:46:22.123Z Reads: 1795

```
I think so, I don't expect it to be anymore difficult than soldering the DRV chip. You would want to use a stencil and solder paste for accuracy.
```

---
## \#4 Posted by: Karmannghiagirl Posted at: 2016-05-25T13:48:40.547Z Reads: 1730

```
And the 2000 Vesc that enertion ordered will soon be obsolete... lol :stuck_out_tongue_closed_eyes:
```

---
## \#5 Posted by: akira Posted at: 2016-05-25T13:48:44.572Z Reads: 1637

```
Good to know !!
I have not yet started to solder my V4 VESC though.
```

---
## \#6 Posted by: ecuadorche Posted at: 2016-05-25T14:21:09.169Z Reads: 1533

```
what are the advantages of this version over the last version???
```

---
## \#7 Posted by: JTAG Posted at: 2016-05-25T14:26:19.846Z Reads: 1463

```
This version will likely need +/- 3months to be anywhere near usable for "normal" People in the most optimal case ( judged by Experience ). Software needs to change and PCB routing looks far from  ideal.
```

---
## \#8 Posted by: chaka Posted at: 2016-05-25T14:28:35.023Z Reads: 1464

```
Be sure to practice on some scrap electronics. Quick tip, you can use a tantalum capacitor to see if you get things too hot. They will darken or turn brown if they get too hot. A good visual aid when dialing in your hot air temps.

@ecuadorche The new version uses direct fets. Direct fets work better in high current applications. They are a little harder to solder by hand which is why the original used the common style of mosfet. 
http://electronicdesign.com/files/29/1476/figure_02.gif

@JTAG Yeah, it will be a little while. Vedder stated he will be doing some rerouting of the ki-cad files but will be ordering parts within a week. Don't hate on us ki-cad users ;) Plus this is not a completely new design, I highly doubt it will take Vedder that long to work it out.
```

---
## \#9 Posted by: Karmannghiagirl Posted at: 2016-05-25T14:31:22.143Z Reads: 1336

```
[quote="JTAG, post:7, topic:3813"]
+/- 3months
[/quote]

3 months in the past??? AWESOME!!! :grin:
```

---
## \#10 Posted by: JTAG Posted at: 2016-05-25T14:42:59.687Z Reads: 1280

```
Yeah man!! Time travel is genius ^^.
```

---
## \#11 Posted by: chaka Posted at: 2016-05-25T15:10:54.816Z Reads: 1259

```
> PCB routing looks far from ideal.

Care to explain? Obviously there are a few things that have yet to be routed but I am having trouble seeing what you are referencing. This version is much less crowded than the previous versions. This would be useful information for others designing their own electronics.
```

---
## \#12 Posted by: paragon Posted at: 2016-05-25T15:15:43.340Z Reads: 1224

```
@chaka
So when can we throw our money at you for one of these? 😀
```

---
## \#13 Posted by: evoheyax Posted at: 2016-05-25T15:21:09.214Z Reads: 1253

```
@chaka Than you for taking all of vedders great work, and applying it to make great vescs. Now...

http://shanereiser.com/wp-content/uploads/2014/07/Shut-up-and-take-my-money1.jpg
```

---
## \#14 Posted by: WeeChumlee Posted at: 2016-05-25T15:21:41.334Z Reads: 1194

```
@JTAG 

Could it be you are referring to the first picture?
There are obviously layers there that have not been routed yet on that picture but it is also obvious that would not be the final version.  
All other pictures show decent routing and I doubt internal layers would be overlooked by Vedder.
```

---
## \#15 Posted by: chaka Posted at: 2016-05-25T15:39:10.951Z Reads: 1169

```
I won't speculate too much on the release of the gerber files but I know of no better way to support Vedder than building his designs to the best of our ability and sending him donations from the proceeds. You know we will be on this from day one. 

Best thing to do right now is send him some $encouragement.;) Building these controllers in small quantities is expensive. We are a really lucky bunch to have a person as brilliant as Benjamin develop electronics for us.
```

---
## \#16 Posted by: JTAG Posted at: 2016-05-25T16:16:08.860Z Reads: 1173

```
[quote="chaka, post:15, topic:3813"]
designs to the best of our ability and sending him donations from the proceeds. You know we will be on this from day o
[/quote]

Yeah u a right, it is completely unfair for me to judge in this stage, my apologies. I have the weird tendency to get goose bumps when I see PCB routing like this :P (and get skeptical as well).

I do stil think that it will take several months before there is a usable and robust version ready for use under a skateboard.
```

---
## \#17 Posted by: chaka Posted at: 2016-05-25T21:39:55.195Z Reads: 1130

```
How could I forget to mention Vedder is designing a case for this version too! It will double as a heat sink. Basically this module will have the power of a high end car ESC with the plush throttle response we have all grown to love from the VESC.
```

---
## \#18 Posted by: karma Posted at: 2016-05-25T21:51:42.639Z Reads: 1118

```
This is awesome, can't wait for it. Heat sink case, in metal?
```

---
## \#19 Posted by: Ulfberht Posted at: 2016-05-25T22:24:25.046Z Reads: 1140

```
Oh Snap! These are great developments! Can I pre-order V5 now? LOL :astonished:
I love the idea of the heatsink/case. So is this rev change going to solve the issues with FOC? Is it going to be less finicky with 12s setups?
```

---
## \#20 Posted by: chaka Posted at: 2016-05-25T23:54:38.200Z Reads: 1141

```
I am not to sure about better FOC operation but I do know it will be more robust at 12s due to some revisions to some of the larger smd capacitors. 

@karma Yes, it sounds like the case will fully enclose this version. 

The hub motor crowd is going to go nuts over this version!
```

---
## \#21 Posted by: KMeyerson Posted at: 2016-05-28T01:25:00.194Z Reads: 1031

```
It'll be a game changer - with the amount of current drawn for hubs, it'll make things much more practical.

While I would love to see more voltage and fewer amps, it's not going to happen just yet. I do love the idea of unified heatsink/case.
```

---
## \#22 Posted by: chaka Posted at: 2016-05-28T23:17:25.436Z Reads: 1087

```
Another update from Benjamin today, routing is finished!

Some of the new features are a vertical micro usb port and the capacitors are now mounted directly to the pcb. 

<img src="/uploads/db1493/original/2X/1/13c06a5924c69f36d2017fe3de9fa3c9e705e507.png" width="547" height="500"><img src="/uploads/db1493/original/2X/5/5f675187f50b9130da54e43aad1cbd5006668e01.png" width="547" height="500">
```

---
## \#23 Posted by: Randyc1 Posted at: 2016-05-29T03:43:34.017Z Reads: 943

```
Do you have an idea of the dimentions?
```

---
## \#24 Posted by: chipoi84 Posted at: 2016-05-29T03:45:25.784Z Reads: 932

```
It's 60mmX60mm
```

---
## \#25 Posted by: Randyc1 Posted at: 2016-05-29T03:50:06.688Z Reads: 942

```
Hmmm , seems like a less convienient size for placement? .  V 4.10 fit nicely parrallel to 2 end to end 18650's
```

---
## \#26 Posted by: Jinra Posted at: 2016-05-29T03:52:20.350Z Reads: 934

```
Looks like 1 motor per VESC still?
```

---
## \#27 Posted by: chaka Posted at: 2016-05-29T03:54:27.098Z Reads: 950

```
Vedder has actually designed this controller to be the same thickness and width as most 18650 packs. A pack large enough to power two of the controllers to their potential would be at least 130mm wide
```

---
## \#28 Posted by: chaka Posted at: 2016-05-29T03:57:11.311Z Reads: 945

```
@Jinra from a maintenance and repair standpoint this is ideal.
```

---
## \#29 Posted by: Jinra Posted at: 2016-05-29T04:09:16.525Z Reads: 954

```
Makes sense, can't wait!
```

---
## \#30 Posted by: karma Posted at: 2016-05-29T09:49:22.933Z Reads: 960

```
@chaka So the V5 VESC will use 2 capacitors instead of 3 like the V4? How come?
```

---
## \#31 Posted by: Haimindo Posted at: 2016-06-22T11:04:30.562Z Reads: 976

```
Looks pretty compact!
<img src="/uploads/db1493/original/2X/5/517173b0dd45c7c61695c04b241d5549e6ab5e6a.jpeg" width="548" height="500">
<img src="/uploads/db1493/original/2X/e/e8f39618e0672f535d1d1a592551a1497105c356.jpeg" width="689" height="412">
(Pictures taken by Mr.Vedder) 
http://vedder.se/forums/viewtopic.php?f=6&t=149&start=150
```

---
## \#32 Posted by: onloop Posted at: 2016-06-22T11:16:23.389Z Reads: 938

```
[quote="karma, post:30, topic:3813, full:true"]
@chaka So the V5 VESC will use 2 capacitors instead of 3 like the V4? How come?
[/quote]

the qty of caps doesn't really matter, it's the total capacitance, so you could use 10 smaller ones or 2 bigger ones, or even just one larger one.
```

---
## \#33 Posted by: trbt555 Posted at: 2016-06-22T12:09:14.735Z Reads: 919

```
As good heat dissipation is a major factor in the life expectancy of a capacitor it would actually be better to use 10 smaller caps in order to maximize surface area.

Theoretically that is.
Chances are the VESC will die before the caps do...
```

---
## \#34 Posted by: chaka Posted at: 2016-06-22T13:34:11.403Z Reads: 906

```
> Chances are the VESC will die before the caps do...

Good thing I will be able to resurrect them if that happens but the whole point of this version change was to make the VESC more robust when used with larger motors. The current version 4.12 is actually very stable with smaller 50mm motors.
```

---
## \#35 Posted by: longhairedboy Posted at: 2016-06-22T13:50:28.797Z Reads: 879

```
oh shit! this is a big improvement space wise. The way i build my packs and lay them in the boxes will seriously benefit from this design update. 

I can't wait to get my hands on a pair of these.
```

---
## \#36 Posted by: chaka Posted at: 2016-06-22T13:54:58.780Z Reads: 909

```
Yes, they are designed to match the 18650 form factor. The power leads will be routed between the 2 capacitors, a much cleaner design. Keep in mind that these will come with an aluminum enclosure or at least a heat sink setup.
```

---
## \#37 Posted by: Lizardking0069 Posted at: 2016-06-22T14:05:25.406Z Reads: 950

```
Can you update the software to drive yuneec motors? These motors have the hall effect sensors mounted on consecutive poles instead of 120degrees. See photo:

<img src="/uploads/db1493/original/2X/1/1a6d4ecd3ef7e48edc3ad94d372cacde35768107.png" width="281" height="500">
```

---
## \#38 Posted by: starfunkel Posted at: 2016-06-22T15:24:32.157Z Reads: 903

```
I'm curious if you have tried it without the sensors? have you tried to power it in BLDC mode? if ya did, howed it go? i know its a bit under powered but i got a couple spares at home from replacements and another VESC on the way might make a decent beater board.
```

---
## \#39 Posted by: Lizardking0069 Posted at: 2016-06-22T15:35:00.164Z Reads: 914

```
I haven't tried it because I don't have a Vesc. Another user tried and couldn't get the sensored functionality to work. The other user was able to get it to work unsensored and bumped the speed significantly. 

I want a vesc but I want to make it work with the sensors if possible.
```

---
## \#40 Posted by: squad Posted at: 2016-06-22T15:59:37.467Z Reads: 922

```
There are external hall sensor boards available with similiar sensor spacing, I bet I saw someone on ES use it with VESC, You should try connecting it to VESC and run autodetection, I bet it might work, VESC recognizes sensor positions in autodetection.
```

---
## \#41 Posted by: lowGuido Posted at: 2016-06-22T16:23:25.743Z Reads: 867

```
 [quote="squad, post:40, topic:3813"]
I bet it might work
[/quote]

safest bet ever.
```

---
## \#42 Posted by: RainbowUnicorn Posted at: 2016-06-23T09:01:51.520Z Reads: 831

```
Hey guys, do you think its better to wait for this to be released or should I get the current vesc?
```

---
## \#43 Posted by: flatsp0t Posted at: 2016-06-23T09:09:39.245Z Reads: 832

```
If you are ok with 10s/BLDC, there is no difference.
the new one might be more stable with 12s and FOC.
```

---
## \#44 Posted by: Nordle Posted at: 2016-06-23T09:47:28.861Z Reads: 830

```
I just glued my halls between the stator teeth of my sk3 (aprox. 120 deg), and they worked after auto detection.
VESC is so nice! Hail Vedder!:raised_hands:
```

---
## \#45 Posted by: RainbowUnicorn Posted at: 2016-06-23T09:49:21.961Z Reads: 825

```
Alright thanks !
```

---
## \#46 Posted by: 91Seconds Posted at: 2016-06-23T09:53:19.935Z Reads: 810

```
Could the new vesc have a higher eRPM limit or is that not something planned for this release?
```

---
## \#47 Posted by: Nordle Posted at: 2016-06-23T12:32:33.022Z Reads: 811

```
Do you know this forum? [vedder.se](http://vedder.se/forums/index.php?sid=81259684ea10a712af27146b68820b2e)
```

---
## \#48 Posted by: chaka Posted at: 2016-06-23T13:20:23.803Z Reads: 831

```
> Could the new vesc have a higher eRPM limit or is that not something planned for this release?

Running the motor higher than 60K erpm is inefficient so it is not likely to have a higher limit than the current VESC. We will have to wait and see if it will be stable closer to 100k but again it would be a fruitless exercise since the efficiency of the motors is reduced significantly when driving higher than 60k ERPM.
```

---
## \#49 Posted by: guyguy Posted at: 2016-06-23T14:19:40.286Z Reads: 804

```
Supposedly V5 will be more stable for larger motors too.
```

---
## \#50 Posted by: Lukas Posted at: 2016-06-23T14:48:10.869Z Reads: 795

```
Did anyone change the title to 6.0? :D thought 5.0 is still in development
```

---
## \#51 Posted by: ferrice Posted at: 2016-06-23T14:54:39.542Z Reads: 797

```
Is the new design also a 4 layer pcb?
4 layer is x times more expansive.

greets
```

---
## \#52 Posted by: treenutter Posted at: 2016-06-23T15:00:43.843Z Reads: 803

```
@Lukas I'm curious about this too. I thought that version 5.0 was the one that Vedder is currently working on.
```

---
## \#53 Posted by: chaka Posted at: 2016-06-23T15:15:00.142Z Reads: 800

```
Version 5 was a two pcb design and was dropped in favor of a single 4 layer pcb resulting in version 6.
```

---
## \#54 Posted by: Blasto Posted at: 2016-06-23T15:15:42.171Z Reads: 797

```
version 5 was supposed to be a pcb stack with 2 pcbs. That design got canned before seeing the light of day, so the HW got up reved to version 6, single 4 layer pcb.
```

---
## \#55 Posted by: lowGuido Posted at: 2016-06-23T15:20:48.051Z Reads: 793

```
maybe hes doing a microsoft..
```

---
## \#56 Posted by: Haimindo Posted at: 2016-06-23T15:59:59.351Z Reads: 796

```
VESC Vista? :fearful:
```

---
## \#57 Posted by: treenutter Posted at: 2016-06-23T16:02:14.319Z Reads: 798

```
Ha @Haimindo VESC ME ?
```

---
## \#58 Posted by: treenutter Posted at: 2016-06-23T16:02:36.296Z Reads: 791

```
@chaka @Blasto thx that makes sense.
```

---
## \#59 Posted by: Hummie Posted at: 2016-06-23T17:07:25.713Z Reads: 805

```
The old vesc had (3) 680farad caps (or mili-farads or whatever) the new one uses just 2. Closer to the board is better but given the long battery wires people use on skateboards and also I heard from Ren who did the calculations the inductance of the wires is too much already for FOC.
```

---
## \#60 Posted by: KMeyerson Posted at: 2016-06-23T18:15:51.906Z Reads: 803

```
Send to Vedder.
```

---
## \#61 Posted by: Ulfberht Posted at: 2016-06-23T22:55:56.505Z Reads: 751

```
@chaka So in your professional opinion, would it be more advisable to go with smaller motors with the 4.12 rev and wait for V6 to get started building with the larger motors?
```

---
## \#62 Posted by: chaka Posted at: 2016-06-25T15:10:50.332Z Reads: 754

```
Imo smaller motors are much more trouble free on the v4.12 vesc. I have yet to experience any fault codes using the 50mm motors. V6 should be considered bleading edge untill we get though a few beta production runs.
```

---
## \#63 Posted by: appelton Posted at: 2016-06-28T06:34:30.087Z Reads: 738

```
Guys so what's the next version of VESC ..is it going to be named 5.0 or 6.0 ?
```

---
## \#64 Posted by: lox897 Posted at: 2016-06-28T06:38:45.851Z Reads: 736

```
6.0 

10 characters
```

---
## \#65 Posted by: Photorph Posted at: 2016-06-30T14:01:41.708Z Reads: 739

```
Truly appreciate Benj V developing this awesome ESC for us E-board enthusiasts.  Will it still be open source?

@RainbowUnicorn the current VESC is fine for smaller motors, but from what Chaka has told me for bigger motors the new VESC will be much better.
```

---
## \#66 Posted by: Lizardking0069 Posted at: 2016-06-30T14:35:14.183Z Reads: 728

```
What is the main difference? Why is it better for bigger (63mm?) motors?
```

---
## \#67 Posted by: makevoid Posted at: 2016-06-30T15:55:07.538Z Reads: 723

```
Usually they tend to have more power/torque, and they should always dissipate heat better ;)
```

---
## \#68 Posted by: Jinra Posted at: 2016-06-30T16:13:39.465Z Reads: 722

```
According to chaka, there are stability issues on the current VESC for 63's. Though I'm not sure why that is. My guess is that it's related to higher current in the system.
```

---
## \#69 Posted by: Photorph Posted at: 2016-06-30T17:29:18.343Z Reads: 727

```
Basically what @Jinra said, and I only know what I know because of chaka.  He's the probably the most qualified person to ask on this forum for VESC questions.   He can give you all the technical info.
```

---
## \#70 Posted by: sl33py Posted at: 2016-06-30T18:00:14.365Z Reads: 747

```
@treenutter @Haimindo - how about VESC BOB!
(https://en.wikipedia.org/wiki/Microsoft_Bob)

I'm super excited by the new design.  I'm still using 4.7/4.8 HW on mine, but could see upgrading.  Especially if it's compatible with >200kv motors on 12s?  (i like to gear down, and am looking for larger pulleys >36t for big ABEC wheels (90/97/107mm).

And it's always good to put some $ towards these improvements.  I've sent over $150 to Ben (he got 1/2 of $ from his anti-spark switches, plus other contributions as thanks).  Great to give back and help him continue to develop for the community!!
```

---
## \#71 Posted by: XvDarkVAngelvX Posted at: 2016-06-30T21:00:19.446Z Reads: 700

```
I'm excited, are they being shipped out now?
```

---
## \#72 Posted by: Pantologist Posted at: 2016-06-30T23:09:16.568Z Reads: 693

```
I don't think the PCB layout is completed yet lol.
```

---
## \#73 Posted by: onloop Posted at: 2016-06-30T23:18:40.200Z Reads: 712

```
[quote="Jinra, post:68, topic:3813"]
According to chaka, there are stability issues on the current VESC for 63's.
[/quote]

THIS IS UNFOUNDED

let's get some proof first before we start spreading false information. 

_If I was selling 50mm motors i would probably tell similar stories too._
```

---
## \#74 Posted by: onloop Posted at: 2016-06-30T23:24:56.039Z Reads: 717

```
[quote="Lizardking0069, post:66, topic:3813"]
Why is it better for bigger (63mm?) motors?
[/quote]

- Larger stator diameter. 
- Bigger stator teeth, more copper turns.
- Larger Cooper mass.
- Larger magnets.
- Better heat dissipation.
- Higher current/power rating.
- More torque!
```

---
## \#75 Posted by: willpark16 Posted at: 2016-06-30T23:40:33.145Z Reads: 691

```
:joy: u have so much potential for a possible comedian
```

---
## \#76 Posted by: Jinra Posted at: 2016-06-30T23:42:09.517Z Reads: 702

```
I'd love to see proof. I'd also like to know why FOC is killing some VESCs, but no one seems to have a conclusive answer.
```

---
## \#77 Posted by: onloop Posted at: 2016-06-30T23:45:43.256Z Reads: 718

```
[quote="Jinra, post:76, topic:3813"]
I'd also like to know why FOC is killing some VESCs
[/quote]

it seems to occur when people are switching between modes (BLDC & FOC) without having the correct motor detection parameters set in FOC.

my advice is don't play with it unless your willing to risk blowing it up.
```

---
## \#78 Posted by: onloop Posted at: 2016-06-30T23:46:43.838Z Reads: 715

```

Maybe you should be an actor. Because I can't tell if you being a dick or not.
```

---
## \#79 Posted by: Wanderer Posted at: 2016-07-01T01:53:27.840Z Reads: 733

```
One could say that if I was selling 63mm motors with vesc's that I wouldn't want people to think there were potential issues. ;-) 

Would definitely like to see some proof of the stability issues as well though.
```

---
## \#80 Posted by: willpark16 Posted at: 2016-07-01T02:00:15.135Z Reads: 748

```
:joy:no not being a dick
```

---
## \#81 Posted by: chaka Posted at: 2016-07-01T02:17:00.945Z Reads: 725

```
Plenty of threads around with people haveing issues with braking on 63mm motors which boils down to an ABS overcurrent fault. I personally still use version 4.12 on 63mm motors but I keep my ERPM well within spec and I also run very low braking current to avoid this. I originally used sk3 motors that have a smaller stator diameter than maytech/tacon and rarely had any issues, if at all. It wasn't until I started pushing my systems with larger stator motors that I began to see problems and realized a direct correlation in stability and motor size. 

It is common knowledge within the RC world that you run motors that do not exceed the max current rating of your ESC. You do this so you do not overheat your motor controller and fry your hardware. Using a motor that falls below the max current rating of your ESC allows you to drive the motor hard without triggering the overheating safety cutoff and allows you to climb hills that would normally cause the VESC to overheat and reduce power.  Finding a balance and having headroom in the correct places within your system is key to good design. Sticking large motors on an esc that cannot handle them at WOT is poor design but will work if you make enough concessions.
```

---
## \#82 Posted by: onloop Posted at: 2016-07-01T02:21:36.378Z Reads: 747

```
[quote="Wanderer, post:79, topic:3813"]
One could say that if I was selling 63mm motors with vesc's that I wouldn't want people to think there were potential issues. :wink:
[/quote]

Here is a quick search result for the words "R-SPEC" & "VESC" 
http://www.electric-skateboard.builders/search?q=vesc%20r-spec

There are at least 50 build threads published on this forum alone with this combination of R-SPEC 63mm motors & VESC....  also there are other suppliers of 63mm motors, e.g. DIY & Alien... 

Not to mention all Raptors & LHB builds use 63mm motors & VESC

**There just isn't any concrete evidence of stability issues due to 63mm motor Stator Diameter.** 

The VESC issues are most likely related to the very sensitive DRV8302 Chip & User Error/bad settings, hence the reason Vedder has dropped it from V6.0

The problem is Chaka won't admit that some of his VESC have failed for no apparent reason... He simply chooses to tell everyone that its a 63mm motor problem as this shifts the blame to someone else. **Its a great strategy & It would appear many people are believers!!**

The problem I see with this marketing strategy is that Chaka will probably want to sell 63mm motors at some point in the future, then his language will have to change. _Potters Prophecies!_
```

---
## \#83 Posted by: Jinra Posted at: 2016-07-01T03:48:55.116Z Reads: 696

```
A bit anecdotal, but @Photorph ran into an issue with a LHB board where his brakes cut out and he had to slide on his knees pads to stop. Nothing conclusively saying big motors are problematic, but i thought I'd point it out. It'd be nice to have some scientific resource for these kinds of tests.
```

---
## \#84 Posted by: harpie Posted at: 2016-07-01T10:16:26.764Z Reads: 690

```
The larger 63mm motors are probably more efficient during regen and therefore pushes more current back through the vesc. A dual motor configuration should reduce this problem by half for the same amount of braking power.
```

---
## \#85 Posted by: guyguy Posted at: 2016-07-01T10:59:10.849Z Reads: 682

```
I've had issues with braking and my LHB build and posted videos in the build thread - I also updated settings from forum advice with LHB's advice. The issue was mitigated but didn't completely go away. Not sure what the issue is - must be user error.
```

---
## \#86 Posted by: Lizardking0069 Posted at: 2016-07-01T11:49:59.131Z Reads: 667

```
Well I just ordered a Chaka Vesc and a DIY 63mm motor. I'm going to be running 16/36T 83mm @8s. I'll post my findings.
```

---
## \#87 Posted by: chaka Posted at: 2016-07-01T13:23:48.442Z Reads: 679

```
The issue seems to be caused by the initial burst of current when you apply brakes at speed. A dual configuration reduces the load but you can still induce this burst of regen current if you apply the brakes hard.
```

---
## \#88 Posted by: harpie Posted at: 2016-07-01T13:34:18.080Z Reads: 695

```
If it is a transient effect my gut feel would be inductance between the battery and VESC. Long wires/thin wires/bad connections between these two could cause a proportional voltage burst on the VESC side when current is flowing towards the battery. If this is the case the problem should be less likely to occur at the end of the ride when the battery has been drained (The sum of the battery voltage and the spike might, in this case, be lower than the threshold causing the release). Telemetry would be awesome. Will see if I can build a small SD card logger some time in the future for some offline logging (using some off the shelf Arduino parts).
```

---
## \#89 Posted by: Lizardking0069 Posted at: 2016-07-01T13:40:09.620Z Reads: 663

```
Why not turn of regen or put a diode between the battery and the vesc?
```

---
## \#90 Posted by: Kaly Posted at: 2016-07-01T13:51:44.270Z Reads: 664

```
Hi Mr. Clark

A quick question. For the sk3 motors what ERPM and braking current values do  you use ? 
Thank you
```

---
## \#91 Posted by: chaka Posted at: 2016-07-01T14:35:39.725Z Reads: 699

```
@Kaly I leave my ERPM at the defualt setting and only adjust the braking current if the battery or BMS cannot handle the regen current. Take into account that I control my ERPM with motor selection keeping it below 60k. If you are getting a fault during braking you can adjust the braking current but it does not completely solve the problem. 

@Lizardking0069 BLDC motors are in a constant state of regen while spinning, even while being powered, not something that can just be turned off.  I try not to expend too much time finding workarounds to problems caused by an unbalanced design. One thing a lot of people do not account for is the fact that motors pull power. The VESC can throttle this to a certain degree but we still see spikes in current. This also applies to regen.

One thing our resident fortune teller has right is that we will be bringing a 63mm motor to the market but we are waiting for version 6.0-6.1 VESC.  No sense using huge motors if you can't supply them with the current they need or pull. 

If you are power hungry and you can't wait for V6 then you are better off using a high quality car esc that can handle the amp draw. You lose the smooth throttle response of the VESC but the system will handle the load.
```

---
## \#92 Posted by: Ulfberht Posted at: 2016-07-03T23:13:18.598Z Reads: 666

```
@chaka Thanks! Your explanations make very good sense.  It is what it is and I think you laid all of that out very clearly. This information is very much appreciated. :nerd:
```

---
## \#93 Posted by: cjoliver Posted at: 2016-07-04T00:33:04.354Z Reads: 668

```
Could you not just increase voltage to lower the amount of amps going through the vesc?
```

---
## \#94 Posted by: Pantologist Posted at: 2016-07-04T02:38:51.062Z Reads: 680

```
Yes, you can. Miami's 12s2p battery build send to work perfectly. This is why I'm think it's best to avoid less than 10S for the current VESC.
```

---
## \#95 Posted by: chaka Posted at: 2016-07-04T15:50:26.591Z Reads: 750

```
Vedder posted some updates for everyone on his forum today.

> What is implemented, tested and working so far:
> * The built in NRF, which can be used simultaneously with other applications
> * DRV8301 configuration. I need to update the code a bit to report the faults read from the SPI bus though, but so far I didn't have any DRV faults at all, so implementing this didn't have so high priority.
> * Current sampling using all three shunts for the best possible samples (I have tested using low side samples, high side samples, combining them, and combining low/high side samples with just two shunts).
> * CAN-bus with the new transceiver.
> * Motor parameter detection works fine with these amps as well. Inductance measurement is more consistent and accurate now since I take advantage of having three shunts.
> * Both BLDC and FOC are updated and take advantage of three shunts.
> * I have fixed bugs in the firmware here and there while refactoring everything. Most notably will probably be the current control fixes when brake and acceleration currents are different.
> * The old hardware is still fully supported in the firmware.

Here are few other important details that have left me speechles!

> In general, this hardware seems to be significantly more robust than v4.x, most likely due to the layout of the new power stage where all traces are short and both ceramic and electrolytic caps are close. Some interesting test I made:

> * A 6-pole 0.6µH inrunner. This motor would always kill the DRV within a second or two on the old hardware, especially when running FOC since the inductance and resistance is so low (0.6µH is just evil). No problems at all so far, not even on FOC. I could run the motor up to 130K ERPM in FOC.

> * To test the FOC high speed performance, I tried a small high-kv inrunner at 30V and 50 KHz switching frequency. I could run it up to 230K ERPM, which is a lot higher than I expected from FOC. That means that a small ESC with FETs that are easier to drive at high speed is possible, which would be perfect for racing quads.

> * Even though the shunts are 0.5 mOhm now (half of 1 mOhm from before), small motors work a lot better, even on low speed. The overall performance of the current measurement is better now, so these amplifiers seem quite nice so far. I have a bunch of small motors that didn't work before without changing the shunts, but now all the motors I have tested work on FOC.

> * I have a Turnigy Multistar 2216-800Kv motor with a propeller on it for my RC airplance, and it works nicely. The sensorless observer for FOC can easily track the motor through 0 speed with full torque (applying active braking before the direction change), meaning that the direction can be changed very quickly with a propeller (I will show it in a video). This is cool because it can be used for multirotors like this:

> * A castle 2028 (also a quite evil motor) works nice at 120A phase current with FOC without any dead DRVs. The main problem I had with RC car motors before was the current measurement because they have so low inductance, but these problems are mostly gone now. This can be a significant improvement for RC car ESCs in general, where FOC and smooth current control can be used on really difficult motors.

[http://vedder.se/forums/viewtopic.php?f=6&t=149&start=150](http://vedder.se/forums/viewtopic.php?f=6&t=149&start=150)
```

---
## \#96 Posted by: Lizardking0069 Posted at: 2016-07-04T16:34:26.458Z Reads: 681

```
Sounds great. What is thr timeline for v6.0? Late august?
```

---
## \#97 Posted by: Haimindo Posted at: 2016-07-05T08:01:22.318Z Reads: 715

```
Interesting demo from Benjamin
https://www.youtube.com/watch?v=ugD6T4MPXUw
```

---
## \#98 Posted by: Stevemk14ebr Posted at: 2016-07-05T12:08:28.072Z Reads: 703

```
He mentioned he is also going to test a 380kv motor at 120amp limit @12s soon! Hopefully it works.
```

---
## \#99 Posted by: Lizardking0069 Posted at: 2016-07-08T13:34:36.105Z Reads: 708

```
Has anyone tried 14s on the vesc?
```

---
## \#100 Posted by: chaka Posted at: 2016-07-08T13:43:39.221Z Reads: 708

```
It will cause component failures at 14s. A few people have tried. :disappointed_relieved:
```

---
## \#101 Posted by: TheRedPanda Posted at: 2016-07-08T17:46:43.179Z Reads: 669

```
You definitely can up to a point. As you get into the 10 or 12s range you start creating a lot of heat from the increased switching frequency in the mosfets. 8-10s seems to be where the vesc is happiest(depending on application).
```

---
## \#102 Posted by: chaka Posted at: 2016-07-08T18:13:02.681Z Reads: 686

```
It is a dangerous practice though. There can be occasions where the voltage can spike during regen and exceed the max voltage threshold set within the bldc-tool. If you are using up all the buffer and setting the max voltage to 60v I am not sure the processing speed of the stm chip will be up to the task of protecting the components.
```

---
## \#103 Posted by: treenutter Posted at: 2016-07-08T19:31:26.180Z Reads: 708

```
[quote="Lizardking0069, post:86, topic:3813, full:true"]
Well I just ordered a Chaka Vesc and a DIY 63mm motor. I'm going to be running 16/36T 83mm @8s. I'll post my findings.
[/quote]



@Lizardking0069 I use this configuration now, but with 14/60 gearing. It worked very well for a season but I ended up with a DRV error, it may have been caused by a bad wiring job (I think one of the motor leads might have made contact with another one, causing a small short). The error occurred on a day when  I rode a long downhill road while braking. If it's true that the larger motor is not well-matched with the current version of VESC, this could have caused the DRV fault. 

At any rate, it worked great for about 150 miles of riding; and it's not possible to know exactly what went wrong. Thread about it here:

http://www.electric-skateboard.builders/t/another-drv8302-fault-disconnected-motor-leads-cause-short/3908
```

---
## \#104 Posted by: treenutter Posted at: 2016-07-08T19:36:03.814Z Reads: 681

```
[quote="chaka, post:81, topic:3813"]
I personally still use version 4.12 on 63mm motors but I keep my ERPM well within spec and I also run very low braking current to avoid this.
[/quote]


@chaka how low do you set your braking parameters when you run a 63mm motor w VESC? I'm trying to find a balance between good braking performance and reducing the risk of over-current when  braking.
```

---
## \#105 Posted by: chaka Posted at: 2016-07-08T20:47:31.738Z Reads: 659

```
Between -7 and -15 amps. It helps to have a stout battery pack to keep the regen from raising the voltage too rapidly also. So it really depends on several factors. This is another reason I have grown accustom to really large battery systems.
```

---
## \#106 Posted by: Ulfberht Posted at: 2016-07-08T22:06:32.097Z Reads: 675

```
[quote="chaka, post:105, topic:3813"]
This is another reason I have grown accustom to really large battery systems.
[/quote]

What would you qualify as a "really large" battery system? I'm putting together a 10s5p. Would that meet base criteria?
```

---
## \#107 Posted by: Jinra Posted at: 2016-07-08T22:08:33.597Z Reads: 672

```
His free ride deck houses 666wh, so I assume something like that :P
```

---
## \#108 Posted by: CSN Posted at: 2016-07-09T00:19:52.464Z Reads: 723

```
I think mine is around 800 watt hours

Just enough room for one VESC.



<img src="/uploads/db1493/original/2X/c/c6c5ee5f09a71dfd8710f5787f2dbb1d0a1ff5f9.jpg" width="328" height="499">
```

---
## \#109 Posted by: MidnightOne Posted at: 2016-07-19T14:47:10.304Z Reads: 694

```
I didn't want to start a new thread, so I'll ask here:
Does anyone have files for VESC HW rev higher than 4.8?
On one hand it's "open hardware & software", on the other hand a lot of resellers/makers here claim to churn out v6 ("with all the bugs fixed") soon and it's not in public access. I want to maka a single board of two ESCs with a specific footprint, so i need source files and also i don't want to build upon the 2015 version.

Thanks.
```

---
## \#110 Posted by: treenutter Posted at: 2016-07-19T14:51:06.408Z Reads: 705

```
@MidnightOne VESC V6 is still in its early stages. You can check Benjamin Vedder's website for updates.
```

---
## \#111 Posted by: DougM Posted at: 2016-07-19T15:17:50.225Z Reads: 706

```
@MidnightOne you can get VESC 4.12 off OshPark

[VESC 4.12](https://oshpark.com/shared_projects/y0ye8b2o)
```

---
## \#112 Posted by: MidnightOne Posted at: 2016-07-19T15:42:34.336Z Reads: 717

```
@treenutter Thanks for pointing out, judging by the "v5" thread there, v6 is almost read and also now drv burnouts will be less likely, which is great.

@DougM Thanks, but you didn't get my points, I need schematics (not the readymade PCB) to rearrange components and make my own PCB design with specific dimensions. I also want to have the latest revision, since i'll be doing quite some work on it, so It would be really dounting to finish rework on current gen VESC the day before v6 is released.
```

---
## \#113 Posted by: Stevemk14ebr Posted at: 2016-07-19T16:23:47.713Z Reads: 709

```
EVERYTHING you need is on vedders github
```

---
## \#114 Posted by: Skitzor Posted at: 2016-07-19T16:47:26.938Z Reads: 709

```
I might go on a limb here, but what about when this version is finished, make a VESC6 dual for dual motor setups with 2 outputs for the motors? where you can detect and configure them both... Having traction control within one config... Could save us some space and would be a little sturdier and easier to mount.
```

---
## \#115 Posted by: Jinra Posted at: 2016-07-19T17:27:23.943Z Reads: 709

```
It would be nice to have a modular design where we can easily 'layer' the pcbs into a nice little VESC sandwich :D
```

---
## \#116 Posted by: flatsp0t Posted at: 2016-07-19T17:47:18.542Z Reads: 716

```
https://github.com/vedderb/bldc-hardware
```

---
## \#117 Posted by: MidnightOne Posted at: 2016-07-19T18:28:50.958Z Reads: 737

```
@Stevemk14ebr @flatsp0t I'll stop spamming now, but one last time:
My initial post is based on github, the latest revision there is 4.8, so I was asking wheather anyone had any higher verions. Now I know to wait till v6 is ready.
But thanks anyway for tying to help.

@Jinra I don't think it will be worth it to stack vescs on top of each other. 
1. e-skates are all about how slim can you make them (not talking about Trampas).
2. Heat.
```

---
## \#118 Posted by: Blasto Posted at: 2016-07-19T18:36:18.721Z Reads: 710

```
4.8,4.9,4.10,4.11,4.12 are BOM changes, no changes to the layout, same gerber files
```

---
## \#120 Posted by: mishrasubhransu Posted at: 2016-07-19T18:51:23.222Z Reads: 726

```
What's the link to the VESC 6.0 discussion? I couldn't only find VESC 5.0 discussion.
```

---
## \#121 Posted by: Stevemk14ebr Posted at: 2016-07-19T19:19:50.292Z Reads: 726

```
Vesc 5.0 discussion morphs into vesc 6.0 at around 7 pages in. 5.0 was never actually made, it was talked about but then scrapped for 6.0
```

---
## \#122 Posted by: longhairedboy Posted at: 2016-07-19T19:48:45.212Z Reads: 722

```
[quote="Stevemk14ebr, post:121, topic:3813, full:true"]
Vesc 5.0 discussion morphs into vesc 6.0 at around 7 pages in. 5.0 was never actually made, it was talked about but then scrapped for 6.0
[/quote]

Thank you for clearing that up. I thought it was typo everyone was expected to ignore. I have 4 on my bench, I heard about 5 and then people kept mentioning 6 and i was wondering wtf they were talking about 5 isn't even out yet. 

I'm pretty pumped about the new form factor. its going to fit nicely floating over the BMS on standoffs when i find one that works in the appropriate size.
```

---
## \#123 Posted by: Skitzor Posted at: 2016-07-19T23:09:59.917Z Reads: 689

```
Nice idea, but hoping they are layered with heat-sinks then to dissipate the heat generated ;)
```

---
## \#124 Posted by: Jinra Posted at: 2016-07-19T23:11:30.023Z Reads: 698

```
get a nice piece of aluminum as the meat for the VESC sandwich :hamburger:
```

---
## \#125 Posted by: fertito Posted at: 2016-07-24T12:43:44.599Z Reads: 732

```
There is a few changes between these version, more caps, thicker traces...
```

---
## \#126 Posted by: Pantologist Posted at: 2016-08-22T01:10:32.823Z Reads: 725

```
Are there any updates from Vedder yet?
```

---
## \#127 Posted by: RayWiis Posted at: 2016-09-18T08:39:35.227Z Reads: 671

```
Vedders latest post on the 6.0 thread was back in 05 Sep 2016. He said that he'd built a second batch of prototypes and did some more testing. And he is also rewriting the BLDC tool. You can read his entire post here http://vedder.se/forums/viewtopic.php?f=6&t=149&start=180
```

---
## \#128 Posted by: Eboostin Posted at: 2016-09-18T16:26:27.843Z Reads: 658

```
Is there any chance that 6.0 will allow the controlling of 2 motors with 1 esc?
```

---
## \#129 Posted by: Hummie Posted at: 2016-09-18T16:31:28.818Z Reads: 658

```
No but two esc on one board maybe.
```

---
## \#130 Posted by: karma Posted at: 2016-09-18T17:16:20.152Z Reads: 655

```
Wait, why is this post called V6.0 when [Vedder's](http://vedder.se/forums/viewtopic.php?f=6&t=149&start=180) post is 5.0?
```

---
## \#131 Posted by: rodriguejoe1 Posted at: 2016-09-18T17:24:52.867Z Reads: 666

```
[quote="longhairedboy, post:122, topic:3813"]
Vesc 5.0 discussion morphs into vesc 6.0 at around 7 pages in. 5.0 was never actually made, it was talked about but then scrapped for 6.0
[/quote]

look a few posts up...
```

---
## \#132 Posted by: karma Posted at: 2016-09-18T17:54:51.072Z Reads: 652

```
I got a notification about a new comment and I had not read that, thanks
```

---
## \#133 Posted by: Monte Posted at: 2016-09-18T18:27:30.775Z Reads: 661

```
Does anyone know when the 6.0 vesc will be released?
```

---
## \#134 Posted by: rodriguejoe1 Posted at: 2016-09-18T19:33:20.774Z Reads: 746

```
[quote="chaka, post:15, topic:3813"]
I won't speculate too much on the release of the gerber files but I know of no better way to support Vedder than building his designs to the best of our ability and sending him donations from the proceeds. You know we will be on this from day one. 

Best thing to do right now is send him some $encouragement.:wink: Building these controllers in small quantities is expensive. We are a really lucky bunch to have a person as brilliant as Benjamin develop electronics for us.
[/quote]

this may help.
```

---
## \#135 Posted by: JTAG Posted at: 2016-11-22T23:07:15.342Z Reads: 631

```
https://www.youtube.com/watch?v=1iwN5LGGM80
```

---
## \#136 Posted by: JTAG Posted at: 2016-11-22T23:19:10.031Z Reads: 637

```
The VESC6 and VESC tool looks soooooo gooooood :heart_eyes:.

Qoute from the VESC godfather himself:
"Hopefully everything will be ready in the first quarter of 2017, including reliable and well-tested hardware. I will try to arrange beta testing this year, because that will be very helpful. With the release of the VESC6 I want to decrease the failure rate to a minimum and offer warranty for the hardware by default, while making all software much easier to use. It should also become easier to make contributions to the code with a better structure and clear procedures and guidelines. I also want to set up a solid framework for the VESC open source project, which does not really exist now.

VESC Tool has taken more time than I expected, but it really starts to look polished. There are a few things left to do though. I also set up a build server so that I can make statically linked linux builds that work on most distros without installing anything, and use policykit to ask for root permission to automatically add udev rules for the serial port from VESC Tool. Additionally, I can cross compile windows builds on my Linux server now, so there will also be an official windows version of VESC Tool.

The firmware also has a lot of updates. Many of them are bug fixes and cleanups, but there are also some new features such as throttle curves, wattage limits (in case of legal requirements), a center pulsewidth for the ppm app, ramping for the ppm app, NRF nunchuk pairing and more."
```

---
## \#138 Posted by: treenutter Posted at: 2016-11-22T23:55:58.604Z Reads: 624

```
The new VESC Tool looks incredible, I like all of the help files, instructions, and wizards. Thrilled about the new casing. WHAT he drops the whole motor into a bucket of water!? What is going on? Did he also invent some kind of new oleophobic motor!? I need to go donate to Vedder again!
```

---
## \#137 Posted by: Skitzor Posted at: 2016-11-22T23:56:44.972Z Reads: 607

```
Eating popcorn because I want a comparison from enertions vesc X vs 6.0 from vedder.
It's nice they developed the 4.0 version on their own. But what makes the difference in the end.
The video from vedder looks very promising. Especially the further development of the VESC tool and the amount of current it can handle !
```

---
## \#139 Posted by: chinzw Posted at: 2016-11-22T23:58:56.574Z Reads: 627

```
All outrunners are waterproof... nothing new there
```

---
## \#140 Posted by: Skitzor Posted at: 2016-11-22T23:59:28.369Z Reads: 630

```
True, but like @JTAG mentioned. Let's merge this one with the 6.0 thread that's going on and keep ontopic.
It's brilliant what he did there. And if the motor is insulated properly, it should perfectly work in water without shorts.
```

---
## \#141 Posted by: chuttney1 Posted at: 2016-11-23T02:36:28.830Z Reads: 632

```
I'm giving this an ETA of maybe before the end of March?
```

---
## \#142 Posted by: Pantologist Posted at: 2016-11-23T04:43:04.992Z Reads: 611

```
Does the Vesc 6.0 have a large TVS diode like the Vesc X?
```

---
## \#143 Posted by: Pimousse Posted at: 2016-11-23T07:44:40.165Z Reads: 615

```
Compare VESC-X with VESC 6 doesn't make sense at all.
- Completely new hardware design
- Completely new firmware with more features,improvements, bugs fixes
- Completely new software (even if VESC Tool seems to be compatible with VESC 4.12, i.e VESC-X)

Aaaaahhhhh, I can't test to test VESC 6 ! 2017 seems so far ! :smile:
```

---
## \#144 Posted by: evoheyax Posted at: 2016-11-23T17:11:49.472Z Reads: 605

```
@chaka you know who to send a beta v6 quad vesc to :P
```

---
## \#145 Posted by: Kaly Posted at: 2016-11-23T20:38:39.390Z Reads: 605

```
Really you want to compare a copy design from a guy who is a USER to the design of the INVENTOR  it self !!!
DANG you need to open your eyes and smell the roses. 

IMO Jason can be credited with accelerating the focus on the VESC and by being proactive on getting a different solution when the VESC 6 was taking too long to hit the market, this man is always moving forward, Kudos to him. 

But after that,what vedder is trying to accomplish here is way out of our league.
```

---
## \#146 Posted by: longhairedboy Posted at: 2016-11-23T20:48:14.146Z Reads: 571

```
I can't wait to get my hands on these. mm mmm mmmmm.
```

---
## \#147 Posted by: Badkad Posted at: 2016-11-24T17:49:03.959Z Reads: 549

```
How is the vesc delivering 70 amps to the motor and only drawing 7 from the power supply?
```

---
## \#148 Posted by: rmrf Posted at: 2016-11-24T17:57:08.793Z Reads: 543

```
Benjamin mentions that in the video if you listen carefully :slight_smile: The current circulates between motor and mosfets and not so much current is drawn from PSU.
```

---
## \#149 Posted by: sandrewvdv Posted at: 2016-11-24T17:57:40.942Z Reads: 540

```
There is only a low voltage going through the motor. PWS input voltage is 25 V.
```

---
## \#150 Posted by: Badkad Posted at: 2016-11-24T18:08:49.375Z Reads: 534

```
So the same thing happens in normal use with a battery? Some on board telemetry runs on Bens channel show the same thing, the motor drawing more current than the battery, but not to the same extent as this test
```

---
## \#151 Posted by: laurnts Posted at: 2016-11-24T19:24:49.986Z Reads: 529

```
@JTAG  If you build one VESC 6 beta, I might be interested!
```

---
## \#152 Posted by: JTAG Posted at: 2016-11-24T22:07:27.759Z Reads: 525

```
As soon as the files are released I'll order aaaalllll the parts :smiley:
```

---
## \#153 Posted by: chinzw Posted at: 2016-11-24T22:18:08.706Z Reads: 534

```
Well, by lowering the voltage you can achieve that.

10V * 7A = 70W
70W / 1V = 70A
```

---
## \#154 Posted by: WrinklyWink Posted at: 2016-11-27T04:00:17.496Z Reads: 526

```
anyone else notice that he did the second part of the test submerged under water? :astonished:
```

---
## \#155 Posted by: wmj259 Posted at: 2016-11-27T05:16:38.164Z Reads: 521

```
anyone else notice when he says "foc" :O lelelelele
```

---
## \#156 Posted by: webst Posted at: 2016-11-29T14:46:43.941Z Reads: 516

```
I only noticed that he did second part of the test with motor submerged under water. Pretty sure he remained dry for whole episode.
```

---
## \#157 Posted by: KMeyerson Posted at: 2016-11-30T23:55:41.212Z Reads: 531

```
Based on what I've seen of the new schematics, this thing is going to destroy the VESC-X and VESC 4.12 in performance and sensitivity. 

Its going to be a matter of firmware in the next few weeks, but the hardware looks nearly done.

Fingers crossed!
```

---
## \#158 Posted by: WrinklyWink Posted at: 2016-12-01T06:12:11.647Z Reads: 545

```
I really would like to see multi-vesc compatibility improved. I'm talking past traction control into virtual differential control, so that 4WD bicycle cars can be a reality. If every vesc gets its own air cooling and battery, I'm sure the vehicle can put up with a lot of weight and go quite fast. Of course, turn input, _wheel diameter, turn radius and wheel spread_ would have to be noted into the vesc,
Virtual differential can be a reality if you have all the proper specs (see italics) along with a constant update on the steer/turn position.
Then VESCS would really outdo its current capability and become easily implemented into all sorts of home-built electrical vehicles.
Batteries and general wiring is pretty easy for the other stuff, (lights, signals, horn, cabin climate, windows, etc), but having a solid multi-vesc and motor operation with a virtual differential would really be something.
The vesc would become popular in poorer nations where smaller vehicle transportation (motorcycle sidecars and peddle bikes) is a lot more popular than 4-seater sedans :cold_sweat: because the vesc power ceiling (4x spec) is above their demands. those countries are already quite polluted too so they would benefit from the cleaner energy consumption.
Virtual Differential! Woo!
```

---
## \#159 Posted by: Chris604 Posted at: 2016-12-03T01:12:27.301Z Reads: 535

```
[quote="treenutter, post:138, topic:3813"]
? Did he also invent some kind of new oleophobic motor!? I need to go donate to Vedder again!
[/quote]

Can't wait to get my hands on this!  My vesc just went, so I'm waiting for this to replace them with!  If he needs testers I would love to get a beta version!
```

---
## \#160 Posted by: jmasta Posted at: 2016-12-03T01:47:16.154Z Reads: 574

```
[quote="WrinklyWink, post:158, topic:3813, full:true"]
I really would like to see multi-vesc compatibility improved. I'm talking past traction control into virtual differential control, so that 4WD bicycle cars can be a reality. If every vesc gets its own air cooling and battery, I'm sure the vehicle can put up with a lot of weight and go quite fast. Of course, turn input, _wheel diameter, turn radius and wheel spread_ would have to be noted into the vesc,
Virtual differential can be a reality if you have all the proper specs (see italics) along with a constant update on the steer/turn position.
Then VESCS would really outdo its current capability and become easily implemented into all sorts of home-built electrical vehicles.
Batteries and general wiring is pretty easy for the other stuff, (lights, signals, horn, cabin climate, windows, etc), but having a solid multi-vesc and motor operation with a virtual differential would really be something.
The vesc would become popular in poorer nations where smaller vehicle transportation (motorcycle sidecars and peddle bikes) is a lot more popular than 4-seater sedans :cold_sweat: because the vesc power ceiling (4x spec) is above their demands. those countries are already quite polluted too so they would benefit from the cleaner energy consumption.
Virtual Differential! Woo!
[/quote]

That escalated quickly
```

---
## \#161 Posted by: Pedrodemio Posted at: 2016-12-12T00:21:04.364Z Reads: 578

```
New video, i liked how smooth is the RC car on FOC in the end

https://www.youtube.com/watch?v=bivXOlqooCE
```

---
## \#162 Posted by: saul Posted at: 2016-12-12T04:32:07.531Z Reads: 563

```
wow thats a serious rc car. 110A? HUH? :nerd:
```

---
## \#163 Posted by: rpn314 Posted at: 2016-12-12T16:14:20.772Z Reads: 543

```
This is why I generally trust the VESC: Vedder always seems to push his designs to their absolute limits. Can't wait for VESC 6 :smiley:
```

---
## \#164 Posted by: JTAG Posted at: 2016-12-12T17:50:06.916Z Reads: 549

```
I am so eager to build a bunch of these :heart_eyes:!!!!!
```

---
## \#165 Posted by: Sictrampa Posted at: 2016-12-13T05:21:44.209Z Reads: 541

```
Does anyone know what the proposed constant and peak output will be?
```

---
## \#166 Posted by: jmasta Posted at: 2016-12-13T05:25:57.488Z Reads: 550

```
He runs 70A continuously in his VESC 6.0 demo video.  Whereas he ran the same test with 4.12, and it could only handle 35A continuously without adding passive/active cooling
```

---
## \#167 Posted by: KMeyerson Posted at: 2016-12-14T23:03:41.548Z Reads: 536

```
Whoo! MORE AMPS!

Not that I enjoy increasing the entropy of the universe by wasting energy as heat, but 70 Amps sounds great!
```

---
## \#168 Posted by: jbruce Posted at: 2016-12-19T02:36:07.503Z Reads: 530

```
Who will be selling these and does anyone know approximately what the price will be? @chaka @onloop @torqueboards @JTAG Also any chance of beta testing? I would love to test these.
```

---
## \#169 Posted by: KMeyerson Posted at: 2016-12-19T05:16:34.312Z Reads: 531

```
Cost per VESC will be a smidge bit higher I suspect, but not much compared to 4.12 or VESC-X.

Check out Vedder's forum for when he opens beta.  This is going to be very different from the 4.12 in some ways so the firmware will need more testing than in previous VESC revisions.

I suspect it'll be out on the market for full time use around March.  Maybe earlier.

Also, I'm so giddy! 150k ERPM is gonna be mindblowing.
```

---
## \#170 Posted by: Chris604 Posted at: 2016-12-24T20:31:20.070Z Reads: 504

```
Im way to excited! I'm also starting to get sick of riding around mono. Second it comes out im buying a couple!  Also,  can someone explain the performance increase from the new vesc? Speed increase,  torque,  max amp output,  etc...
```

---
## \#171 Posted by: sl33py Posted at: 2016-12-25T02:29:37.629Z Reads: 515

```
@Chris604 - Higher ERPM limit, more amps, more stable (hopefully) FOC.

FOC and ERPM's were known DRV chip killers.  @Chaka found >60k ERPM was pretty much a guaranteed dead DRV chip.  This is why most folks kept to <200kv motors on 10s to keep ERPM down.  FOC is another whole thread - you'll have to know if you need it, BLDC works really really well, but FOC is the next step!!

Speed and Torque - all in your gearing and volts - regardless of ESC.
```

---
## \#172 Posted by: Atimu Posted at: 2017-01-17T03:19:59.062Z Reads: 517

```
Any update on the release of the VESC 6.0? 

And does anyone think that dual 190kv motors with a 12s (li ion) battery is worth doing at the moment (limiting the erpm to 60k in bldc, due to the current vesc's limitations which wouldn't be the case for the new one which I would switch to upon its release) over a 10s for the extra speed/range/torque or anything?
```

---
## \#173 Posted by: TarzanHBK Posted at: 2017-01-17T07:32:21.768Z Reads: 498

```
The sweet spot for a 190kv is 10s with vesc.
12s is used for lower kv motors like hubs or 149kv and works great.

If you have a good vesc, you shouldn´t be having problems using 12s + 190kv when you limit your erpm to 60k.
```

---
## \#174 Posted by: chaka Posted at: 2017-01-17T14:59:21.068Z Reads: 498

```
190kv @ 12s works but it can get ugly if you don't fully understand the effect coasting has on erpm,
```

---
## \#175 Posted by: SORRENTINO Posted at: 2017-01-17T15:24:34.466Z Reads: 494

```
How come the DRV isnt being replaced with something more robust so erpm limits are non existent?
```

---
## \#176 Posted by: TarzanHBK Posted at: 2017-01-17T15:26:54.923Z Reads: 496

```
thats what is happening with the vesc 6.
There are no similar and better drivers available than the DRV.
```

---
## \#177 Posted by: chaka Posted at: 2017-01-17T15:29:48.074Z Reads: 505

```
The next version will have the drv8301. The erpm limit of 60k is largely caused by pcb layout. We will do some testing in the next few weeks to see how far we can push the new hardware before getting errors caused by high erpm, We have optimized the pcb to keep the drv chip cooler since it does get hot on the original 4.12 pcb.
```

---
## \#178 Posted by: fedestanco Posted at: 2017-01-17T18:08:54.514Z Reads: 520

```
Somebody is already planning to sell them...<img src="/uploads/db1493/original/3X/f/9/f98480a7cf4bd8f7caa7f6a04f95f0f95e56c559.png" width="281" height="500">
```

---
## \#179 Posted by: JohnnyMeduse Posted at: 2017-01-17T18:14:16.598Z Reads: 502

```
Why there is a TRADEMARK over the logo.... IS IT GOING TO BE OPEN SOURCE ?????
```

---
## \#180 Posted by: fedestanco Posted at: 2017-01-17T18:19:42.652Z Reads: 513

```
Maybe just a way to avoid shitty vescs made with non-original BOM to be sold with such name. But I dont really know...
```

---
## \#181 Posted by: JohnnyMeduse Posted at: 2017-01-17T18:21:04.557Z Reads: 524

```
Still kind of odd for a open source to get a trademark.... Also who own the trademark Trampa or vedder ?
```

---
## \#182 Posted by: fedestanco Posted at: 2017-01-17T18:28:29.238Z Reads: 544

```
<img src="/uploads/db1493/original/3X/4/d/4d8500e4d9591e39b321c45bd1cf4bcaa64e0e27.png" width="281" height="500">
He registered in november.
```

---
## \#183 Posted by: JohnnyMeduse Posted at: 2017-01-17T18:33:14.584Z Reads: 511

```
So now how can someone sell a trademark product without the consent of the owner..... Now say hi to a 300 dollar vesc 🤔
```

---
## \#184 Posted by: fedestanco Posted at: 2017-01-17T18:44:46.448Z Reads: 518

```
I believe the best thing that could happen to the vesc would be a decent support ($$) to the creator.
If vedder made the vesc a full-time job, the quality of the product would rise exponentially.

In addition, if he started selling by himself ,price would probably decrease, since I believe with a 30% net profit goal, he would be able to sell a vesc (4.12)  for 100$ and make 30$/vesc (way more than any donation at the moment).

So probably you should be disappointed in the trademark just if you were a reseller.
```

---
## \#185 Posted by: zmoney Posted at: 2017-01-17T18:52:32.529Z Reads: 503

```
Interesting. Although, maybe the trademark is to prevent some old chum from slapping the name VESC 
 (**VEDDER**. electronic. speed. controller) on a crappy Chinese ESC.
```

---
## \#186 Posted by: chuttney1 Posted at: 2017-01-17T18:56:01.892Z Reads: 491

```
I would take a trademark even though it's open source. Gotta find a way to distinguish quality and approve from cheap.
```

---
## \#187 Posted by: JohnnyMeduse Posted at: 2017-01-17T18:58:05.583Z Reads: 477

```
Well, Cheap chinese vesc will still be for sale... since the trademark doesn't apply in china...
```

---
## \#188 Posted by: willpark16 Posted at: 2017-01-17T19:01:13.006Z Reads: 491

```
@onloop I said if I was wrong id happily admit it and seems u were definently right about you hubs in general, and it seems like you might even be correct about vedder and his 6.0 vesc. I do agree however that even if it is not open source that he has no doubt earned the right to make some real profit
```

---
## \#189 Posted by: JohnnyMeduse Posted at: 2017-01-17T19:06:45.021Z Reads: 480

```
I totally agee with the trademark... I think it is the wright move to do.... don't get me wrong... it just that people should be aware that the vesc 6.0 won't be a cheap product to get.
```

---
## \#190 Posted by: guyguy Posted at: 2017-01-17T19:15:24.001Z Reads: 496

```
Trademark and open source are separate things. Trademark is claiming ownership of a name used in trade, it's not a patent or a copyright. You could sell the exact same product under two different trademarks. So, for example, if Vedder keeps 6.0 open source he could sell the "VESC" as a brand name item. Other manufacturers could sell the same product, they would just have to call it something else, not VESC. Since he has trademarked the brand I could see current manufacturers of the VESC having to rename their product or sign licensing deals with Vedder in order to use his brand name on their product.
```

---
## \#191 Posted by: JohnnyMeduse Posted at: 2017-01-17T19:24:49.817Z Reads: 502

```
Well, that is going to be interesting... to watch people reinventing the "VESC" name... 😉 (But still, that doesn't put a cheaper price tag over original vesc)
```

---
## \#192 Posted by: Hummie Posted at: 2017-01-17T19:27:14.639Z Reads: 505

```
But the 2.14 or whatever version we're at now is solid enough for a skateboard it seems.  How many amps are you all needing...you're all amp hogs!!  I've never hit a temp cutoff with even a single hub motor.  Am I missing something and down the road my older vesc will die from some type of attrition?  12s and foc and still going
```

---
## \#193 Posted by: Atimu Posted at: 2017-01-17T19:30:22.714Z Reads: 511

```
What are the effects of coasting on erpm? 
I have 60 li ion cells coming in soon that I can arrange as needed once I understand the pros and cos of 10s and 12s with my motors. Would I get more range doing 10s6p vs 12s5p?

And I'm going dual 190kv motors from diy, 5000watt total which seems like a lot of power draw, if that changes anything. 

Thanks
```

---
## \#194 Posted by: Pantologist Posted at: 2017-01-17T23:22:39.040Z Reads: 501

```
That's is the ugliest logo I have ever seen.

LOL
```

---
## \#195 Posted by: esk8 Posted at: 2017-01-18T07:28:12.592Z Reads: 522

```
<img src="/uploads/db1493/original/3X/4/2/4257de6ccc9c7b2c26e804c214826968aace5904.png" width="690" height="280">

225.-€ by Trampa :joy:
```

---
## \#196 Posted by: TarzanHBK Posted at: 2017-01-18T07:40:45.413Z Reads: 524

```
Lots of people don´t use vescs for mountainboarding because of the low amp limit.
So that will be a nice thing with the new one.
```

---
## \#197 Posted by: esk8 Posted at: 2017-01-18T07:50:18.044Z Reads: 541

```
I am using 2 VESC 4.12 in my Trampa.

2x 3300W 200KV Motor

10S/5P LG HE4 

I have make only the FOC detection with Hal Sensor.

I have only, changed the Battry cut off and Battery end.

Al the other Settings i don´t change.

And i ride my Trampa now over 500Km and i don't have any problems

with my VESC 4.12

<img src="/uploads/db1493/original/3X/1/c/1c418e0fa0a1bc6c6e84c5dffe1227115a303097.jpg" width="666" height="500">
```

---
## \#198 Posted by: Okami Posted at: 2017-01-18T08:50:12.277Z Reads: 517

```
I think you are are right.. especially with dual there should not be such problems.. unless you go offroading and amp draw is really high..

Can you quickly chime in and tell are there also heatsinks for your vescs?
```

---
## \#199 Posted by: esk8 Posted at: 2017-01-18T09:23:56.152Z Reads: 552

```
[quote="Okami, post:198, topic:3813, full:true"]
I think you are are right.. especially with dual there should not be such problems.. unless you go offroading and amp draw is really high..

Can you quickly chime in and tell are there also heatsinks for your vescs?
[/quote]


I don't think, that with single Motor on a MTB was a good Idea :joy:

No i have the VESC in heat shrink thats al, and he was in a closed Alu Box.

I ride my Trampa al time offroad :grin:

<img src="/uploads/db1493/original/3X/8/5/85221f07b78b4a8603c6387b85c194656fc7e65e.JPG" width="666" height="500">
```

---
## \#200 Posted by: esk8 Posted at: 2017-01-18T09:33:21.945Z Reads: 542

```
I do not think about it that i want used 12S and 5 ore 6 P
what can I change by the parameters by the VESC.
I know that my Motors i used i can ride with 10S 
and that was enough for MTB on al terrain.

And i drive not more, and have fun.
```

---
## \#201 Posted by: Duffman Posted at: 2017-01-18T09:41:32.913Z Reads: 530

```
If anyone rides his VESC with standard current settings there should be no problems, but if one tries to get out more power by increasing the current settings the risk of damaging something also increases.

Btw. I'm riding at 12S with 100A motor/battery and 155A absolute current limit, did not blow anything. But I still would really like to have more current -> more torque available to ride even harder... :sunglasses:
```

---
## \#202 Posted by: Okami Posted at: 2017-01-18T15:37:53.704Z Reads: 543

```

@esk8  Would u be willing to get vesc bluetooth module? This way it would be interesting to find some really good data for emtb ride characteristics!

I think they dont cost that much! Especially if you use the app @Ackmaniac or @evoheyax developed..

---

@Duffman How does it feel when the vesc cuts power? Does it just slows down or you can feel a sharp cut in acceleration / speed when that happens?

 I have not witnessed on a video how overcurrent protection works for the vesc on an emtb :) 

I just saw a video where the temp was high and then the amps very slowly reduced to decrease the temp.. though... it was a longboard and in not that energy dense situation

 So I wonder what happens if you suddenly need lots of power from the vesc :) and then it has to cut it down..
```

---
## \#203 Posted by: okp Posted at: 2017-01-18T16:35:36.975Z Reads: 523

```
I'm riding dual VESC on my Trampa mountainboards for more one year and a half (maybe more) without any problem. 12S. I have tried once a "CAR" ESC... and man... who can handle this horrible breaking noise...!
```

---
## \#204 Posted by: Okami Posted at: 2017-01-18T17:08:11.694Z Reads: 529

```
@unik well, not all of these car escs have braking noise :slight_smile:
The only donwside of car esc's is that they are not as much customizeable.. and they just ''dump'' current into the motor.. besides not making it possible to log any data, of course, too :D
```

---
## \#205 Posted by: okp Posted at: 2017-01-18T17:11:08.588Z Reads: 513

```
MAX6 was crazy noisy. Do you have one to recommend on 12S ?
```

---
## \#206 Posted by: Okami Posted at: 2017-01-18T17:24:25.686Z Reads: 508

```
@unik You might try ''maytech'' one.. It seems it is manufactured by fvt company.. im using the 6s version with the noisy fan and for a beginner board it is actually quite good!

Search the terms ''maytech 12s esc'' this should lead you onto some results.. it looks like it has been used a lot for emtb builds..

If you want to order from usa, I think they are called / can be found: TQ 12s esc (torque boards)
```

---
## \#207 Posted by: mmaner Posted at: 2017-01-18T17:26:32.602Z Reads: 509

```
[quote="Okami, post:206, topic:3813"]
You might try ''maytech'' one
[/quote]

@unik here ya go...  http://www.maytech.cn/en/product/e-skateboard/e-skateboard-esc/e-skateboard-esc-with-fan-case
```

---
## \#208 Posted by: Okami Posted at: 2017-01-18T17:29:06.797Z Reads: 508

```
http://www.maytech.cn/en/product/e-skateboard/e-skateboard-esc/e-skateboard-esc-with-fin-case

I was actually referring to these, but perhaps, the ones with the fans also compare / are similar to these..
```

---
## \#209 Posted by: esk8 Posted at: 2017-01-18T20:19:29.577Z Reads: 530

```
I know,
you have buy your VESC by esk8.de LOL.

And they working, under 12S and FOC 1 1/2 Year :clap:
```

---
## \#210 Posted by: okp Posted at: 2017-01-18T22:00:16.756Z Reads: 547

```
hey mate, 
I'm not running FOC on 12S - even FOC at all. Just tested it on the bench from time to time but I prefer BLDC. 

I searched and found these two videos from 29th december 2015 on HW4.10.

https://www.youtube.com/watch?v=NCwhJ5EPjuk

https://www.youtube.com/watch?v=8hmc-ssPaJ8

Apart from that, I confirm that your VESCs are/were really nice, perform great and that your service is really awesome (if someone is still wondering !)

But that was before I launched my business and ride my products :slight_smile: 

@mmaner @Okami thanks folks for the links!

@all sorry to hijack the thread; my question had nothing to do with VESC6.
```

---
## \#211 Posted by: Sictrampa Posted at: 2017-01-19T05:34:45.117Z Reads: 517

```
I've ordered two MGM esc's for my build, these have data logging.
```

---
## \#212 Posted by: Duffman Posted at: 2017-01-19T06:03:06.301Z Reads: 522

```
@Okami:

There are several ways the actual VESC reduces or cuts power:

What you mentioned happens at over-temperature or under-voltage. Then it slowly reduces power to keep values in the 'green' range.

If you get a 'non latching DRV fault' or an 'absolute overcurrent fault' the VESC instantly cuts power for the user defined 'fault stop time'
If you define it with a few seconds your VESC does not respond for this time. If you define it with a few milliseconds you just feel a little glitch.
This usually happens trough current or voltage spikes when accelerating hard or giving full throttle while the motor is cogging.

If those spikes get to high the DRV gets damaged and the VESC cuts power completely.
```

---
## \#213 Posted by: Okami Posted at: 2017-01-19T10:55:33.433Z Reads: 508

```
Which one's are these ? Can you give a link?

---

@Duffman what you describe with DRV fault and absolute overcurrent does not sound very nice :D 

So yeah, it looks like if you ''accidentally'' do an over-current to the vesc.. it just fries (drv chip) / gets error code.. at least it looks like it does not throw you off a board but lets you ''coast it out'' ..

The bad things happen when motor gets locked or hits a brake..
```

---
## \#214 Posted by: flatsp0t Posted at: 2017-01-19T21:00:12.035Z Reads: 496

```
As the Maytech ones @Nowind got turned out to be, i dont think the maytech are a good choice either.
```

---
## \#215 Posted by: psychotiller Posted at: 2017-01-20T02:44:46.247Z Reads: 504

```
Yeah I sold my max6's because the noise wasn't much fun compared to sensored FOC
```

---
## \#216 Posted by: hexakopter Posted at: 2017-01-21T18:45:04.799Z Reads: 531

```
Because here where also some questions/rumors about the future of VESC regarding trademark, open source etc.

- Benjamin told me, the project will stay open for sure. So no closed source software in the future.
- Benjamin is working on things almost every day, so the project is not dead. Besides the VESC development he is also working on a website that will summarizes everything about the project.
- Some guys speculate about the VESC trademark. The trademark has nothing to do with the project being open source. It is just to identify the project correctly, so modified projects are named different.
```

---
## \#217 Posted by: Pimousse Posted at: 2017-02-13T17:58:56.588Z Reads: 539

```
http://www.trampaboards.com/vesc-6-complete--vedder-electronic-speed-controller-trampa-exclusive-p-23866.html

[img]http://i.imgur.com/7pxcHQW.png[/img]

:neutral_face: :disappointed:
```

---
## \#218 Posted by: barajabali Posted at: 2017-02-13T18:10:48.356Z Reads: 527

```
April 1st. I dont trust it lol
```

---
## \#219 Posted by: Mark Posted at: 2017-02-13T19:27:30.605Z Reads: 535

```
I'd rather stay with my vesc which is working fine and only costed me half the money. Innovation is cool, high prices aint. :confused:
```

---
## \#220 Posted by: Hummie Posted at: 2017-02-13T19:29:44.312Z Reads: 570

```
that's what I'm thinking.  will the version 6 be better/safer on foc?  I dont have a problem with the regular vesc and think it could put out more power than id need already
```

---
## \#221 Posted by: RogerD Posted at: 2017-02-13T22:49:08.828Z Reads: 602

```
That link is already dead! And at that price you can kiss my ass! :-)
```

---
## \#222 Posted by: Ackmaniac Posted at: 2017-02-13T22:55:16.572Z Reads: 592

```
It's funny that Trampa updates the site every now and then to see how the people react to different prices.
```

---
## \#223 Posted by: JohnnyMeduse Posted at: 2017-02-14T00:22:20.034Z Reads: 580

```
Why are you always removing your link @trampa .... are you commit or just trolling everybody...
```

---
## \#224 Posted by: turbo Posted at: 2017-02-14T14:18:21.170Z Reads: 596

```
We have to see how the page looks on the website from time to time, we did much development on the pages yesterday and we needed to see how they looked... i simply i forgot to turn them off that's all.. Im not smart enough for any clever business thats being suggested. The last thing i want to do is hype the market and not be able to supply so im sorry if i have stirred unnecessary interest by showing those pages for that time... 
The VESC 6 is more than amazing... ive been riding it for a while, stunning performance. For those that don't know development is expensive & low production premium quality products always cost more.... The RRP reflects the production capacity and the premium position in the market, which is top of the shop! if you are one of the lucky folk to take one of the first batch you will not be disappointed you will only be disappointed if your not one of the first to get one...... production is about start and we hope to have stock here to be distributed to you before April1st... We will be going live on the pages as soon as this is confirmed...
Turbo
```

---
## \#226 Posted by: trampa Posted at: 2017-02-14T14:29:55.303Z Reads: 592

```
We will come up with a statement very soon. It's no secret anymore that Trampa and BV banged together on the VESC 6 to create the ultimate experiance. It just got to much work for a one man show and we made the decission to support Benjamin in the process as good as we posibly could. BTW, there is no intension to close anything down in future. We know that some people fear that things go in a funky direction. They will not! 
The release will happen the moment Benjamin feels comfortable with the Hardware and Software. 
With regards to the pricing: Everyone wants a cheap and versatile product, we fully understand that. But please don't forget the designer in future. A price includes more than the pure production costs.
You have no clue how many hours of coding BV spent in the last year! It has been endless!
Please also note that UK prices include 20% VAT. We do not advertise our products without VAT and Import Tax towards overseas customers to make them look attractive. No fooling around. VESC 6 includes a CNC housing and a NRF module + antenna. So don't compare apple to oranges.

Frank
```

---
## \#227 Posted by: trampa Posted at: 2017-02-14T14:40:55.150Z Reads: 554

```
Forgot to post this link:

http://vedder.se/forums/viewtopic.php?f=6&t=149&start=280#p3544

Frank
```

---
## \#228 Posted by: Hummie Posted at: 2017-02-14T18:49:58.574Z Reads: 546

```
I'm not into any additional features beyond what the old vesc has and am just wondering will version 6 be more reliable for foc? Or are the component updates that have happened over the years for the old vesc showing to be reliable for foc now?
```

---
## \#229 Posted by: boards Posted at: 2017-02-14T18:52:38.274Z Reads: 528

```
VESC6 seems to be perfect on FOC and able to handle tons of amps.
```

---
## \#230 Posted by: JohnnyMeduse Posted at: 2017-02-14T20:10:12.915Z Reads: 530

```
[quote="trampa, post:226, topic:3813"]
So don't compare apple to oranges.
[/quote]

?????? What is your point on that????
```

---
## \#231 Posted by: trampa Posted at: 2017-02-14T23:45:17.913Z Reads: 537

```
My point is: Some vendors show a price not including VAT to make products look cheaper than they actually are. Some people compare Vesc 6 prices to Vesc 4 prices although its a different product. The Vesc 6 has more features, like a NRF chipset, built in antenna, splash proof CNC casing for heat distribution, three shunts, and many small extra features incl. proper protection for the DRV etc. Its a major improvement over V4.12. Motors or software settings killing any Vesc 4 / X in milliseconds can be handled by Vesc 6 with ease. Much higher ERPM, better FOC, really robust, super high AMP draw.... The full list of features will be published by Benjamin. 

Frank
```

---
## \#232 Posted by: trampa Posted at: 2017-02-14T23:57:39.653Z Reads: 533

```
@Hummie You can kill a VESC 4 / X using a motor with low resistance, or by running funny settings. The DRV is vulnerable to get damaged by overpower. In VESC 6 a feature will protect the DRV from destruction, continuous AMP draw is much higher. Sensor ports support different voltages, NRF wireless connection, CNC housing, splash proof, three shunts, better FOC, accurate measurement of all three phases etc. Vesc 6 is a major improvement in any aspect.
```

---
## \#233 Posted by: fedestanco Posted at: 2017-02-15T00:21:27.252Z Reads: 534

```
Hi Frank, I read Benjamin's message and I would like to buy 2 beta-vesc6. Since you won't be including a warranty in the first batch I have a couple of questions that maybe other potential buyers may be interested in:
Will the DRV-protection feature be available also in the beta batch?
Should the first buyers be concerned about an higher possibility of failure in the beta batch? (or you already did plenty of tests and nothing is likely to fail?)
In case one hidden bug burns the beta-batch vescs will you offer a repair service (fee-paying)?
Thanks
```

---
## \#234 Posted by: JohnnyMeduse Posted at: 2017-02-15T00:23:06.778Z Reads: 525

```
[quote="trampa, post:231, topic:3813"]
Some people compare Vesc 6 prices to Vesc 4 prices although its a different product.
[/quote]

I agree with you, but for a fair analysis of the price for the vesc 6, you need to take a closer look at the history of the 4,X... And as I said before it is understandable that the price range of the 6, will be around 250 to 300, since production won't be as much for the first batch as the current vesc are. Also, one of the key features of the vesc 4 (and probably what made people think that the price of the 6 will be lower) is that it was conceived to be a low cost product and easy to make product.
```

---
## \#235 Posted by: JTAG Posted at: 2017-02-15T03:01:27.244Z Reads: 514

```
Let me qoute you; I agree with you, but I don't agree.

Did Mr. Valentine ignore you today xD? Why the criticism? If you are happy with the 4.X please stick there. If you think the price is to high don't buy it and build your own when the data becomes available.
```

---
## \#236 Posted by: boards Posted at: 2017-02-15T03:13:18.718Z Reads: 512

```
2 VESC 6 are about 350 USD + shipping (Subtract VAT and I'm pretty sure there's no import duties UK -> US)? This is pretty reasonable. It's not like VESC 4 is going away.


Can't wait!
```

---
## \#237 Posted by: JohnnyMeduse Posted at: 2017-02-15T03:52:32.389Z Reads: 518

```
[quote="JTAG, post:235, topic:3813"]
Why the criticism?
[/quote]

Sorry if you miss read me, it's not a criticism, it's is more a analytic point of view.... I couldn't really care less about the price.... :wink:

[quote="JohnnyMeduse, post:234, topic:3813"]
And as I said before it is understandable that the price range of the 6, will be around 250 to 300,
[/quote]
```

---
## \#238 Posted by: DougM Posted at: 2017-02-15T04:12:33.080Z Reads: 499

```
So does this mean VESC6 is hardware complete?  I just checked Vedder's GitHub and nothing's been touched for a year.
```

---
## \#239 Posted by: baxter Posted at: 2017-02-15T07:30:17.852Z Reads: 537

```
Frank, 

Thank you for providing the link to Benjamin's latest comments.  Great to hear about all the developments for Vesc V6 and the support tools and website he is currently developing. 

As the thread notes that you are partnering to manufacture beta units, can you provide some more detail as to the expected improvements in performance of the V6 hardware over and above the (latest) V4.12?

Thanks
```

---
## \#240 Posted by: trampa Posted at: 2017-02-15T10:12:42.398Z Reads: 547

```
Hi @fedestanco , Benjamin did a lot of testing and his videos show the strenght. The Vesc 6.4 is very very robust now!
The DRV will be protected. You are never safe if you don't use safe settings. Since VESC-Tool still allows you to use crazy settings, things can ultimately go wrong. But: you have a temerature feature allowing you to define a safe and soft cutoff in case you overstress the ESC or motor (requires motor temp sensors). Three shunts measure all phases, so its not very likely to fry your Fets. VESC Tool is much more advanced than BLDC-Tool and the firmare is brand new, which took most of the time. Especially FOC is improoved by miles. Vesc 4 was really the Beta in comparison to VESC 6.
So far we did not manage to kill it, while the VESC 4 / X all failed within milliseconds, using the same beasty settings or beasty motors. Fried DRVs seam to be an issue of the past.

Benjamin knows exactly what he is doing and some users don't, so we can't guarantee 100% of the Betas will still live after the test period, although we tested to the extreme where any VESC 4 / X would have died immediately. Its a Hardware/Software/User issue. And the user is the BIG X.
Vesc 6 stays repairable, an ethos we stick to. But there is no free of charge repair service in Beta phase. We will try our best to solve issues on an individual bases. We don't think that disappointment will be the issue because we had no disapointments so far. 

Frank
```

---
## \#241 Posted by: JTAG Posted at: 2017-02-15T13:49:08.150Z Reads: 526

```
Haha I was just kidding :sunglasses: , it was a fuse test, yours is long and slow :smiling_imp: .
```

---
## \#242 Posted by: JohnnyMeduse Posted at: 2017-02-15T13:56:57.173Z Reads: 535

```
Like most of the customer Electronic, I wish to be build with a "Slow Blow".......... (Well..... That sound weird :confused: ) :joy:
```

---
## \#243 Posted by: trampa Posted at: 2017-02-15T15:32:01.132Z Reads: 528

```
Anyone wanting a VESC 6 Beta, please PM me. We are about to close the list.
Only private users are accepted, only some Betas left. 175Pond incl. UK VAT. Non EU customers pay no VAT.

Frank
```

---
## \#244 Posted by: trampa Posted at: 2017-02-17T08:52:05.245Z Reads: 534

```
The Beta list is closed now. We want to keep things to a small scale for the now.
Early next week we will send out a mail to everyone taking part in the beta test program.
Thanks for your support and interest. 

@caustin @PXSS @jos @racidon  I need your mail address to get you in.
Please PM me ASAP.  

Frank
```

---
## \#245 Posted by: onloop Posted at: 2017-02-17T09:13:02.984Z Reads: 528

```
[quote="trampa, post:240, topic:3813"]
So far we did not manage to kill it, while the VESC 4 / X all failed within milliseconds
[/quote]

You tested a vescx? What is the test?
```

---
## \#246 Posted by: trampa Posted at: 2017-02-17T11:02:18.345Z Reads: 532

```
Hi Jason, it refers to the VESC 4 design in gerneral. The feature protecting the DRV is new in VESC 6 hardware and firmware, so any derived VESC 4 design has the same issue with beasty motors and high ERPM, high power drain. Most of the work on VESC 6 is firmware related BTW. So this amount of robustness is new in VESC 6 designs, running the latest Firmware which not public yet. Benjamin does not want to release the new Software until he feels everything is 100% perfect and safe. It won't be long until its available to the public!
The new software package will allow more different VESC hardware designs and we want to stipulate more innovation to the benefit of everyone. What I wrote is no criticism about Your VESC X (VESC 4 derivate with direct FETS). We like to see innovation. It's something Benjamin worked on for countless hours and a key feature of the latest design in hardware and software.

We all know that the hardware is something very simple in comparison to the software. Most of the work achieved in the last year was purely software related and we all had to spend a lot of our free time to get thing where they are now - especially Benjamin. Please be a bit pacient with VESC 6. Its due to be released once things are 100% perfect for Benjamin. The Beta Test will give him some more input to really get the Software to brilliance. 

VESC-Tool is a lot more than BLDC-Tool. Benjamin and I created an entire environment for it, so that the VESC-Project will have a propper home from now on. We hope that everyone in the VESC business will give Benjamin the credits he deserves. It will help him to push things further and develop new products in future to the benefit of everyone.
For this reason we (Me, Ted And Benjamin) created an very transparent environment for USERS and BUSINESSES. This Environment is in Benjamins hands only! We did not intend to hijack an OS project. Some things will change in future to stipulate a certain amount of fair play and innovation. This is the reason for TM registartion in pretty much any contry of relvance incl. China, Hongkong, Austrlia, Israel, USA, EU etc etc.. VESC 6 first batches through Trampa will hopefully cover the cost for this very expensive step we sponsored to Benjamin. Anyone complaing about prices should know that we needed a lot of cash to help to put the VESC project on a proper legal foundations, just like any other major OS project. VESC is from now on a TM to identify the orignal hardware and most important: software by BV.
Benjamin will publish information about the OS Vesc-Project soon. There is still a fair amount of work left!
Some info can be found here: http://vedder.se/forums/viewtopic.php?f=6&t=149&start=280

I hope everyone in the game will understand that all these steps (including hiding away for a while) were inavitable and for the benefit of the OS VESC-Project.

Frank
```

---
## \#247 Posted by: Pimousse Posted at: 2017-02-17T11:15:12.565Z Reads: 491

```
Trademark is the way to go !
You've done in a really proper way.

Thanks for keeping this amazing project fully Open Source. ;)
```

---
## \#248 Posted by: trampa Posted at: 2017-02-17T12:17:36.023Z Reads: 501

```
We always try to do things in a proper way. Thx for the compliments.
But the real perfectionist is BV. Its amazing to see his progress of the last year. He shouldered most of the burden and our combined demand for perfection didn't really help to reduce the level of stress. 
Please support him in future to encourage innovation. Once the new Website is up, you all have a change to show some respect. Many people giving small contribution will help to see a lot more progress. We created a way to give something back to you in case you decide to support the project. 

Frank
```

---
## \#249 Posted by: Pimousse Posted at: 2017-02-17T12:58:02.198Z Reads: 518

```
B. Vedder has my full respect and admiration. I promote his work to everyone (even to those who don't care about electric skateboard :smile: ) 

I brought my contribution by donating. I hop we could help in another way like every open source project by sending pull request, and so on.
Vedder is very talented, so are other guys who could bring their support.
Thanks to the new system (like the website), this would be improved I guess.

I'm on the beta list, and I'll do my best for feeding BV with lot's of inputs ;)

Thank you Frank for the feedback on the forum.

(BTW, Thank you for my new Holypro 35 529T, it's a piece of art, received in 2 days !! :astonished: )
```

---
## \#250 Posted by: Hillso Posted at: 2017-02-18T09:39:00.919Z Reads: 525

```
new video from Benjamine Vedder:
https://www.youtube.com/watch?v=x6lPdI9OVQg
```

---
## \#251 Posted by: JeffS Posted at: 2017-02-24T13:12:18.123Z Reads: 513

```
Have you considered using a passive loop heat pipe (PLHP) cooling system to dump the heat? It has an evaporator and condenser with no moving parts.
```

---
## \#252 Posted by: Eboostin Posted at: 2017-02-24T18:07:51.650Z Reads: 512

```
Maybe I missed it in the thread, but what are the dimensions with and without the aluminum case?
```

---
## \#253 Posted by: ekitesurfer Posted at: 2017-02-24T19:34:22.108Z Reads: 501

```
I didn't read the whole thread, so excuse me if the question has been asked or if it is just plain stupid, but do you guys think this would work powering a 54v ebike?
```

---
## \#254 Posted by: fedestanco Posted at: 2017-02-24T20:32:36.371Z Reads: 500

```
If that means 14s I'd suggest you to wait for Vedder's approval. I am almost certain that trampa made its motors to run on 12s, and I would stick to that at least for the betas. 
Theoretically fets are rated 60v but no one ever pushed 4.12vesc this far without damage: quote "The DRV8302 failed/burned after 5 minutes of playing on 14S 
while failling it showed the same erratic behavior it did on 12S so maybe my earlier problem was a not good DRV.
Or maybe a bad ground solder underneat it.
It failed after maybe 30 secondes full throttle."

There is a thread on endless sphere about that: http://vedder.se/forums/viewtopic.php?t=6
```

---
## \#256 Posted by: trampa Posted at: 2017-02-24T21:37:31.199Z Reads: 485

```
12S max! A fully charger 12S is @ 51V already! 13S is killing it. 
Its perfect for an eBilke. Benjamins eBike is a beast and runs on guess what?

Frank
```

---
## \#257 Posted by: ekitesurfer Posted at: 2017-02-24T21:48:09.684Z Reads: 480

```
Know what kind of throttle/ brake he uses?
```

---
## \#258 Posted by: trampa Posted at: 2017-02-24T22:24:56.860Z Reads: 491

```
I don't,  but its something standard. The Vesc-Tool allows you to select such a throttle as input device.

Frank
```

---
## \#259 Posted by: Eboostin Posted at: 2017-02-24T22:37:02.355Z Reads: 488

```
@trampa Are you able to release the dimensions yet?
```

---
## \#260 Posted by: jaykup Posted at: 2017-02-24T22:57:21.397Z Reads: 489

```
@trampa seconded
```

---
## \#261 Posted by: Jebe Posted at: 2017-02-25T00:04:00.156Z Reads: 501

```
like they used to use in old valve amplifiers
```

---
## \#262 Posted by: trampa Posted at: 2017-02-25T15:15:54.560Z Reads: 514

```
I can send a sketch out to the beta group.
Its roughly 68 x 72 x 18mm.

Frank
```

---
## \#263 Posted by: whitepony Posted at: 2017-02-25T15:43:17.623Z Reads: 533

```
[quote="trampa, post:262, topic:3813"]
Its roughly 68 x 72 x 18mm.
[/quote]

hehe, perfect 18650 dimensions :smiley:
```

---
## \#264 Posted by: trampa Posted at: 2017-02-25T18:51:45.338Z Reads: 520

```
We tried to keep The 18650 cell format, yes.
Its roughly 3 cells long. 

Frank
```

---
## \#265 Posted by: squad Posted at: 2017-02-25T21:56:55.265Z Reads: 514

```
That would be actually great, as I wrote to You I plan to mount both of my beta VESC 6 on a custom heat-sink and sketch would let me to make it before VESC itself arrives.
```

---
## \#266 Posted by: JeffS Posted at: 2017-02-27T13:45:32.035Z Reads: 504

```
There is at least one other technique using coherent porous silicon.
```

---
## \#267 Posted by: Pimousse Posted at: 2017-02-27T15:20:11.883Z Reads: 503

```
Yes please.
Like @squad, I'm in the way to build a mount plate for them (will be mounted using Holypro truck screw).
Having the dimensions now allows to save few weeks of beta testing ;)
```

---
## \#268 Posted by: JTAG Posted at: 2017-03-02T18:17:11.749Z Reads: 488

```
Just out of curiosity, how many beta users / devices are there ( @trampa )?
```

---
## \#269 Posted by: trampa Posted at: 2017-03-02T18:51:58.583Z Reads: 490

```
We limited it to 50 devices. Overlookable...
If you are interested PM me, maybe I can find a last pair of Vescs for you.

Frank
```

---
## \#270 Posted by: Chris604 Posted at: 2017-03-02T19:54:00.132Z Reads: 485

```
I'm interested in beta testing!
```

---
## \#271 Posted by: JTAG Posted at: 2017-03-02T23:48:45.503Z Reads: 483

```
Thanks for the info and offer (and all your effort organizing all of this with BV)! I am already one of the 50 :smiling_imp: (so I just learned ^^).
```

---
## \#272 Posted by: mt37 Posted at: 2017-03-06T19:47:27.187Z Reads: 470

```
I'm making my first build with a vesc 4.12. I'm new but fairly handy, and have a background in engineering.

I would also be interested in beta testing if it's still an option.
```

---
## \#273 Posted by: Journ Posted at: 2017-03-07T23:12:30.471Z Reads: 467

```
Any room for a newbie to get in on this.. in other words i am also interested in beta testing & or getting on the list to purchase once beta tested? Or are there prequalifications/prerequisites that i may lack? Either way much respect. I look forward to purchasing two when they are ready. Thanks
```

---
## \#274 Posted by: Pr0dy Posted at: 2017-03-07T23:26:38.071Z Reads: 456

```
I would be down to beta test
```

---
## \#275 Posted by: trampa Posted at: 2017-03-08T08:21:45.174Z Reads: 467

```
There is some room left since we increased the Beta batch due to min order quantities.
So anyone who is still wanting to get in please PM me your name and mail + quantity ( 1 or 2).
I'll drop you on the list and send you a mail later this week.

Frank
```

---
## \#276 Posted by: trampa Posted at: 2017-03-08T15:04:07.111Z Reads: 467

```
Hi Beta II testers, after doing some more maths on the VESC 6 Beta, we have to announce that we can't sell the VESC 6 Beta II at the same price we did before. I would love to be able to offer you guys the same deal, but its not possible at this stage. So we made the decision to offer you the following limited forward ordering deal:

If you buy two VESC 6 Beta, we can offer you 195 GBP per VESC.
If you buy a single you can get it for 220GBP.

All Beta VESCs will have all cables and connectors (XT 90) + Housing (Heat Sink), basically Plug and Play.

Sorry that we can't offer the 175GBP price any more. Actually this was price was based on a miscalculation and Beta I testers were more than lucky to get away with it. Ted and I did the maths today based on the latest quotation. 

Anyone on the list not agreeing on the new pricing: Don't worry your purchase is not compulsory, so its up to you to step back. 

Frank
```

---
## \#277 Posted by: Plumb77 Posted at: 2017-03-09T01:27:19.653Z Reads: 448

```
I would hope people just building their first board wouldn't be buyers for the beta $268 USD is alot for you to screw up on a possible mistake building your first build. Just saying leave this to experienced builders to test first.
```

---
## \#278 Posted by: Journ Posted at: 2017-03-09T03:56:15.046Z Reads: 461

```
I hear you. But i am seeking the best brains (Vesc) for my ride so i don't waste money only to regret it and come back to buy the cutting edge anyway later although i can wait too. Idk what i should do... i'm a newbie ready to build my ride and the price is what i expected to pay anyway even though it keeps changing... if its $268 for one and i need two it may be true the test is one i can't afford to do. Any advice is welcomed.  http://www.electric-skateboard.builders/t/first-build-project-upgrading-mbs-colt-to-electric-2wd-mountainboard/18264/45 So maybe someone can clarify the price for two and if there is any warrenty? "limited forward ordering deal:
If you buy two VESC 6 Beta, we can offer you 195 GBP per VESC.
If you buy a single you can get it for 220GBP." What is GBP Great Britain Price? Cuz yeah I'm in the USA and am not sure the exchange rate. Seeking advice, Thanks
```

---
## \#279 Posted by: Plumb77 Posted at: 2017-03-09T04:10:20.769Z Reads: 450

```
Yes that's the conversion for usd.id recommend a 12esc for @torqueboards that's what most set ups I see use for a mountain board.
```

---
## \#280 Posted by: Journ Posted at: 2017-03-09T05:04:49.549Z Reads: 443

```
What are the big and small differences between the two besides price?
```

---
## \#281 Posted by: Stevemk14ebr Posted at: 2017-03-09T05:24:54.301Z Reads: 441

```
Just wait for official release
```

---
## \#282 Posted by: Okami Posted at: 2017-03-09T08:46:27.249Z Reads: 452

```
Try to find the ''preview''... or if trampa is kind enough maybe he will answer..

Basically I think it was this:

Improved current capability
More customizability / better software side to deal with all kinds of things
Less (almost non?) possibility of error, fried drv chips..

Maybe some more.. but yeh
```

---
## \#283 Posted by: trampa Posted at: 2017-03-09T10:08:32.335Z Reads: 495

```
Basically the VESC 6 is - quote Benjamin "Magnitudes better than any VESC 4 out there". 
And its true, its magnitudes better. Sure the VESC 4 will also profit from VSC-Tool, but its still the old hardware.
I really never had problems with my quality VESC 4 controllers on streetboards - but I keep it at 40A drain @ 12S + use temp control on the VESC and Motor.

Frank
```

---
## \#284 Posted by: racidon Posted at: 2017-03-09T10:43:26.311Z Reads: 506

```
[quote="Journ, post:280, topic:3813, full:true"]
What are the big and small differences between the two besides price?
[/quote]

if you're building a regular eboard, just go with an improved version of the VESC 4

Ollinboards has (from my experience) a very reliable vesc 4, I've not had an issue with it and not seen any (except 1) have a problem with it

Enertion also has a similar product (VESC-X) that I've seen positive feedback about too,

Try those as I can't see that a first build would greatly benefit from the VESC6 as it is now
```

---
## \#285 Posted by: trampa Posted at: 2017-03-09T11:08:31.210Z Reads: 517

```
Well, some guys always want the latest stuff. In some cases its wise to invest a bit more and have the new model. In some cases you could say the old model does the job. So its a matter of attitude and your budget.
I'm always astonished by the cues in front of the modern cathedrals called a...pl store. Folks sleep in front of the stores to be the first to have the latest stuff. I bet in 2018 no one will make VESC4s any more. VESC6 is the future. The latest VESC 6 firmware is just so much better. Its a software issue, not a hardware issue. You can't run VESC 6 Firmware on VESC 4. But I do also agree that VESC 4 designs do work quite well in most cases, just like my two year old smartphone still does the job. Well, the camera could be better....

Frank
```

---
## \#286 Posted by: longhairedboy Posted at: 2017-03-09T13:34:44.405Z Reads: 517

```
I have 14 reasons to be interested in a better VESC. 

<img src="/uploads/db1493/original/3X/4/9/491ee89b55ea7ae3011f0da0a3650d12849b2aa3.jpeg" width="666" height="500">

All of those units are basically dead. Fried DRVs, melted mosfets, or weird intermittent shutdowns and generally buggy behavior which have plagued 4.10, 4.11, and 4.12. 4.12 has been much much better than the other versions though, and when tuned properly 99% of its issues seem to be mitigated 99% of the time. But you can still trigger braking failures on occasion. And believe it or not, pulley ratios are just as important where braking is concerned when trying to overcome those issues as BLDC settings tuning is. 

For now Enertion's VESC-X is holding up to the street abuse we give it very well. No braking issues so far, smooth hard acceleration, and they seem to shut down properly to protect themselves when you do stupid things like put too much load on the PPM power output by running LEDS and shit from them. The form factor is perfect and lends itself to doing things like thermally coupling the existing heatsink to an exterior one exposed through the box, mounting to plates, etc. 

So far the only issue i have is when the brakes change modes during hard braking. It can be kind of startling, but if expected its a non issue. In general they are a breath of fresh air and so far we love them. 

So I'm very excited to see you doing this work and i'm hoping to get my hands on some of your VESCs the minute they are available. If you can make them stand up to the abuse of off-roading and extreme usage than they will definitely take the abuse we give them in our street rods and the community will have something that's well suited for both.
```

---
## \#287 Posted by: Jebe Posted at: 2017-03-09T13:42:34.463Z Reads: 504

```
I have 5 reasons, including a vescx 
<img src="/uploads/db1493/original/3X/4/a/4a4ff61bc402927d115549b50d7ae1fce796c5e3.JPG" width="281" height="500">
Have you ever fried a chaka vesc?
```

---
## \#288 Posted by: JohnnyMeduse Posted at: 2017-03-09T13:46:54.316Z Reads: 506

```
Pffffff...... Beginner 😂

<img src="/uploads/db1493/original/3X/d/a/da1b7cb68d01ecd971b1e6911e28012f599918e1.JPG" width="375" height="500">
```

---
## \#289 Posted by: trampa Posted at: 2017-03-09T13:52:16.470Z Reads: 496

```
In the end its a lot cheaper to invest a bit more in the first place. That's what we are preaching all day long!

Frank
```

---
## \#290 Posted by: JohnnyMeduse Posted at: 2017-03-09T13:55:37.698Z Reads: 493

```
Nah.... **They are all still good**... but I need the 20 dollar MCU and 10 dollar DRV for quick prototype assembly... :stuck_out_tongue_winking_eye:

EXCEPT: for those dual VESC... those where just shitty.
```

---
## \#291 Posted by: longhairedboy Posted at: 2017-03-09T14:41:39.269Z Reads: 492

```
Two of those are very early Ollins, one is a Maytech, some are Enertion from a batch of 12 i ordered late last year, and some are direct from Macrofab that i ordered after uploading the stuff to them from the repository to test on my own. 

I've got three coming from AXLE right now to use in some warranty repairs. We'll see how well those hold up. 

I've pretty much decided to move completely to VESC-X for my customer builds from now until VESC6 is available. We haven't been seeing any real problems at all from them so far for street builds, even when doing really dumb shit like running 15/33 pulleys on 100mm wheels. Even if they are just modified 4.12s with direct fets and the V6 board layout,  and i kind of think there's more going on than just that, they're a vast improvement over typical 4.12s.
```

---
## \#292 Posted by: jaykup Posted at: 2017-03-09T16:06:10.176Z Reads: 477

```
I think Ollin has a direct fet (VESC-X competitor) too, but don't know how well it works, and at the price ($220 vs $150) it probably doesn't make sense if the VESC-X is holding up.

Does the VESC-X have 12s FOC problems?
```

---
## \#293 Posted by: Blasto Posted at: 2017-03-09T16:19:53.959Z Reads: 484

```
[quote="jaykup, post:292, topic:3813"]
Does the VESC-X have 12s FOC problems?
[/quote]

@barajabali and @longhairedboy are beating them up at 12S. All my builds are 10S with foc, no problems at all.

Btw, @longhairedboy, if you did not try it yet, foc sensored is crazy awsome smooth.

Edit: should prob move this convo in the vescx thread, keep the thread on topic
```

---
## \#294 Posted by: monkey32 Posted at: 2017-03-09T16:27:51.336Z Reads: 470

```
Living in the past gentlemen.....Vesc 6.0 will be Amazeballs.
```

---
## \#295 Posted by: Blasto Posted at: 2017-03-09T16:34:27.720Z Reads: 468

```
[quote="monkey32, post:294, topic:3813, full:true"]
Vesc 6.0 will be Amazeballs.
[/quote]

Very possible, i just have a hard time justifying to myself the price difference for extra features that won't be used, that a cheaper and very reliable solution is already available.

220 GreatBrittainKilograms is over 400 canadian pesos... thats to steap for my wallet
```

---
## \#296 Posted by: akira Posted at: 2017-03-09T16:42:01.092Z Reads: 454

```
I still don't get it why the VESC 6.0 should be so much more expensive. The price of the components is not really different, is it ? You get an aluminium enclosure but does that explain the price increase ?
```

---
## \#297 Posted by: zmoney Posted at: 2017-03-09T16:45:07.497Z Reads: 447

```
The new VESC has components that essentially cost more. There's a few new bells and whistles on the board too, which I also agree is not 100% necessary.
```

---
## \#298 Posted by: akira Posted at: 2017-03-09T16:57:38.991Z Reads: 443

```
Which component would cost more ? I thought the DirectFETs were even cheaper than the other SMD package ? Maybe the microcontroller is different.
```

---
## \#299 Posted by: fedestanco Posted at: 2017-03-09T17:33:56.919Z Reads: 456

```
Please don't estimate the value of a product simply considering the price of materials. 
These are the main reasons why trampa's vesc 6 will always be more expensive than the maytech one: [quote="trampa, post:226, topic:3813"]
Everyone wants a cheap and versatile product, we fully understand that. But please don't forget the designer in future. A price includes more than the pure production costs.You have no clue how many hours of coding BV spent in the last year! It has been endless!Please also note that UK prices include 20% VAT. We do not advertise our products without VAT and Import Tax towards overseas customers to make them look attractive. No fooling around.
[/quote]

Even gasoline its FREE if you manage to extract it from your backyard...
```

---
## \#300 Posted by: jaykup Posted at: 2017-03-09T17:36:42.957Z Reads: 454

```
It's got a CNC aluminum housing that adds some cost.  I think after this beta and Trampa production run, the source files will be released which will let other companies start to manufacture it, and we will start to see lower cost options.  Trampa has a lot of R&D and prototype costs to recoup so I believe the price is higher than just the manufacturing costs.  If I had to guess, VESC 6 in two years might sell for around $150 (+/- for aluminum housing).

The other thing is that Vedder worked hard to make this firmware/software expandable and configurable to other hardware.  The goal is to run VESC firmware regular ESC devices.  This means anyone making an ESC with compatible hardware should be able to modify the firmware easily to run on their device.  This means companies might make a 6s ESC with VESC firmware, or a 16s 300A monster ESC with VESC firmware.  It really changes the game.  The firmware/software is where the real value is, and we are lucky he's keeping that open source!
```

---
## \#301 Posted by: Eboostin Posted at: 2017-03-09T17:59:15.351Z Reads: 441

```
I'm interested to hear what the warranty will be on the VESC 6.0. 

If they are going to be $300 and promised to be near bullet proof, I would like a warranty on it that backs up that claim.
```

---
## \#303 Posted by: longhairedboy Posted at: 2017-03-09T18:53:32.187Z Reads: 449

```
[quote="Blasto, post:293, topic:3813"]
Btw, @longhairedboy, if you did not try it yet, foc sensored is crazy awsome smooth.
[/quote]

Sorry, too busy riding the brakes down hills and slamming on them at full speed. lol

Seriously i may try that out. I've been running sensored hybrid with my own motors for the past month or so and.. well... holy shit that's nice.
```

---
## \#304 Posted by: trampa Posted at: 2017-03-09T21:25:48.411Z Reads: 469

```
Well, you dont pay the british VAT in that case. So a twin is 195 x 2 = 390GBP incl 20% VAT. Without VAT its 325/2=162 GBP per VESC. Import Tax depends on your countries legislation.

BTW, just talked to Benjamin - he reckons the housed VESC 6 can handle triple the power of any VESC 4 while design being totally robust.
He is banging on stuff night and day to get you the best beta experience of your life. 200 Ponds sounds expensive but you guys get a real decent product without the need to spend 1000 hours on development. Do the VAT balance before estimating the price you pay when sitting outside Europe!

Frank
```

---
## \#305 Posted by: JohnnyMeduse Posted at: 2017-03-09T21:32:19.616Z Reads: 477

```
Well it is still a f*** lots of canadian pesos and without taxe and duty


<img src="/uploads/db1493/original/3X/c/c/cc72afa56c6231d82ee656ef3ea4e7479c4f3828.PNG" width="281" height="500">
```

---
## \#306 Posted by: trampa Posted at: 2017-03-09T21:33:41.466Z Reads: 458

```
The pound has never been lower. But the USD picked up when the grand casino reopening was announced + the proposed increase of the interest rate is in reach.
```

---
## \#307 Posted by: trampa Posted at: 2017-03-09T21:38:29.333Z Reads: 449

```
Deduct the british 20% VAT and convert to dollars. Import Tax is not terrible in the states and VAT is pretty low in most states. You will get it cheaper than the Europeans!

Frank
```

---
## \#308 Posted by: trampa Posted at: 2017-03-09T21:46:39.384Z Reads: 445

```
All Alphas will have full warranty! All Betas will be helped if there is an issue. Trampas service is outstanding. Truth is: in 15 Years we never had a board returned to us. We only sell bullet proof stuff. If a parts fails we usually just ship a spare. Google "Trampaboards problem". Zero results.

Frank
```

---
## \#309 Posted by: Chris604 Posted at: 2017-03-09T22:14:30.142Z Reads: 440

```
Im from Canada, the conversion is way to much. I don't see the benefit of being a beta tester if we are taking a risk at that price. There has to be something in it for us. Im going to have to give up my position as a beta tester to someone a bit more willing to take a risk at that price.
```

---
## \#310 Posted by: Pr0dy Posted at: 2017-03-09T22:26:16.777Z Reads: 434

```
Same, not willing to pay 550$ for VESC right now :P
```

---
## \#311 Posted by: okp Posted at: 2017-03-09T22:45:51.300Z Reads: 435

```
the benefit is that you are helping the VESC to be a better product. The risk you are willing to take is not for you, it's for the community to move forward.

if a limited number of people would have not put a lot of their time and personal money in this kind of project, we would be still running car ESCs.
```

---
## \#312 Posted by: Sion Posted at: 2017-03-09T22:55:31.047Z Reads: 438

```
Thanks for unbanning.... So I don't need a second account longer. :slight_smile:

[quote="trampa, post:308, topic:3813"]
All Alphas will have full warranty! All Betas will be helped if there is an issue.
[/quote]


Who is ALPHA and who is BETA?

I think that the VESC 4.12 has never leave the BETA stadium. It was just that people selling them don't talk about it for marketing reasons.
```

---
## \#313 Posted by: Chris604 Posted at: 2017-03-09T22:56:28.099Z Reads: 437

```
I like the idea of supporting vesc to be a better product, but that still doesn't justify me spending $641 plus shipping for two vescs. I will jump on the next beta opportunity when its in my price range. How many are you planning on buying?
```

---
## \#314 Posted by: JTAG Posted at: 2017-03-10T00:53:53.654Z Reads: 455

```
The VESC 6 has:
* Upgraded FET driver
* Extra buck converter (it is no longer in the DRV)
* 3 times a current shunt amplifier (the DRV ones are unused)
* WAY WAY better power stage (this in combination with better CAPs and in phase shunts allow for very low induction motor)
*Build in receiver for a remote including antenna
*Build in capacitors
*Coolable alu enclosure

Choosing VESC6 above 4.12 is really justified if you want big low inductance motors or/and driving motors at high current. If you don't niet either of those options then just stay at 4.12 nobody is forcing anyone :sunglasses:.
```

---
## \#316 Posted by: Jebe Posted at: 2017-03-10T02:47:36.831Z Reads: 447

```
Use the search function bud. All those questions have been asked and answered
```

---
## \#317 Posted by: racidon Posted at: 2017-03-10T06:09:58.795Z Reads: 461

```
Benefits:
You can contribute, even if it's the risk of your money + personal well being :stuck_out_tongue:
You also get the VESC6 before anyone in the world, were you around when getting ahold of a Vesc 4 took 6-12months depending on backlogs...

As for the alpha/beta comment by @trampa I believe this is a lost in translation thing. Correct me if I'm wrong @trampa but I assume when you say Alpha, you mean when your product goes publicly available on your site.
Beta you mean the current  people selected for first testing, those of us that required a code to purchase the product for limited time frames.


If this is correct I'll help you out in your phrasing:
Alpha = generally first wave testers, before a product is even finished
Beta = generally 2nd wave testers, after the product is finished, but may contain bugs that need ironing out
Official Release = finished product, all testing complete, publically available
```

---
## \#318 Posted by: okp Posted at: 2017-03-10T06:42:36.810Z Reads: 450

```
two of them - already in.
```

---
## \#319 Posted by: Gromok Posted at: 2017-03-10T07:17:19.968Z Reads: 450

```
Got two of them - already in

@trampa, I sent you a second PM reply correctly answering your information request. My head was asleep the first time around :(
```

---
## \#320 Posted by: trampa Posted at: 2017-03-10T09:27:58.004Z Reads: 448

```
Alpha is after Beta and will probably be 100% identical. Beta still gives us the chance to get some feedback and we might do a tweak to the software for Alpha. VESC 6 release was late due to sorting out al the details. Now we are there. Anyway, we want to do a slow start, rather than shooting out thousand units. So that slow start is called Beta. We simply could not deal with the feedback rolling back to Benjmin when selling a big volume.

Frank
```

---
## \#321 Posted by: hexakopter Posted at: 2017-03-10T11:03:53.266Z Reads: 446

```
[quote="JTAG, post:314, topic:3813"]
Extra buck converter (it is no longer in the DRV)
[/quote]


Are you sure? Where do you get this information? I was thinking that they changed from DRV8302 to DRV8301, but use the internal buck converter for the V6.0 version also.
```

---
## \#322 Posted by: JTAG Posted at: 2017-03-10T12:44:50.187Z Reads: 427

```
I might indeed be wrong, let me check.
```

---
## \#323 Posted by: akira Posted at: 2017-03-10T13:03:49.410Z Reads: 440

```
Hi Trampa
Thank you for your effort to help Ben make the VESC6.0 the ESC of the future !!
Do you already know when (in this schedule of alpha, beta ... ) are the files to be released ?
I'd love to try and build my own :-)
```

---
## \#324 Posted by: Michael319 Posted at: 2017-03-10T15:17:41.085Z Reads: 433

```
Hey man, Btw, alpha always comes before beta, beta is the last stage before release.
```

---
## \#326 Posted by: trampa Posted at: 2017-03-10T15:41:55.977Z Reads: 463

```
Hi Builders, Benjamin wants to work on a VESC 6 reference design after finishing everything that needs to be done to publish VESC-Tool OS and the BOM and wiring scheme. With this information you can start to design your own VESC 6 straight away. The reference design will help those without the skills to design their own PCB or will help make modified VESCs from there. We really would like to see more different VESC designs, rather than a 100% copy paste product being purely sold on price point. There is so much you can do to make the VESC specific for purpose, better or just different. Benjamin and I have been debating this for ages and found that a reference design is a good way to stipulate more Innovation. OS hardware can have a negative impact on Innovation when everything is served on a silver plate. We try to stipulate innovation by finding a healthy balance. Please give Benjamin the time to work things out. We don't have the manpower to work on 10 things simultaneously, which has something to do with the lack of appropriate funding. Everyone wants a cheap VESC 6, available in a short period of time - unfortunately the two facts contradict each other.

I am writing up a statement that will go a bit more into detail. The fundamental change will be a system enabling hardware manufacturers to associate themselves to the OS project through a license model, so that users can see that contributions are made according to a transparent system. Its a win win system and funds Benjamins work and the OS-Project.  Hardware manufacturers should prepare to invest a bit into future innovation if they want to stay credible. 
Customers should prepare that innovation will be priced in VESC 6 designs. Some things have to change to keep this piece of technology alive. We want to play it fair in future! This world needs a bit more balance! Stand up for it!

Frank
```

---
## \#327 Posted by: jaykup Posted at: 2017-03-10T15:42:19.254Z Reads: 430

```
[quote="JTAG, post:314, topic:3813"]
Build in receiver for a remote including antenna
[/quote]

Does this work with the GT2B?
```

---
## \#328 Posted by: trampa Posted at: 2017-03-10T15:44:29.054Z Reads: 429

```
No! It works with a custom PCB for the Nunchuck or any other remote. A good point to start to innovate!

Frank
```

---
## \#329 Posted by: Stevemk14ebr Posted at: 2017-03-10T15:51:10.063Z Reads: 432

```
Alpha comes first, then beta. It's confusing to flip those. Love the work though, and I'll gladly pay a little more if it results in a better product and a happier BV!
```

---
## \#330 Posted by: trampa Posted at: 2017-03-10T15:53:27.375Z Reads: 433

```
If everyone would pay the equivalent of beer in $$ this would help a lot!
We will give everyone the chance to invite Ben for a beer in a nice Bar.

Frank
```

---
## \#331 Posted by: akira Posted at: 2017-03-10T16:10:41.898Z Reads: 430

```
Well, I am not interested in selling VESC, I just would like to solder my own one :slight_smile:
How would the new schema work for individuals wishing soldering their own device ? 
In strict definition, I am not a customer for VESC ... and I will happily continue to donate. But I do not have the competence to design my PCB and BOM from a reference design.

Do I understand correctly that they will be no OS hardware, even for individuals producing their VESC for non commercial purposes (that do not have the time/money to invest to design their own but would like to solder their own device) ? It would be sad ...

I understand that you're thinking mostly in terms of VESC beeing sold (because it is the largest part) but there are some people here that enjoy producing VESC for themselves without selling it. How does all of this apply to them ?
```

---
## \#332 Posted by: trampa Posted at: 2017-03-10T16:18:10.762Z Reads: 421

```
The reference design is 100% OS and you can just grab it and make it. No work needs to be done except soldering. Just like VESC 4. If you like to donate something to Ben for writing VESC-Tool, you are welcome to do so.

Frank
```

---
## \#333 Posted by: akira Posted at: 2017-03-10T16:32:34.483Z Reads: 411

```
Great !
Internet communication (especially in languages that you do not master ... like english for me) is always so prone of misunderstanding !! And I will surely donate again for his hard work !
```

---
## \#334 Posted by: Eboosted Posted at: 2017-03-12T06:44:52.445Z Reads: 416

```
@longhairedboy [quote="longhairedboy, post:291, topic:3813"]
really dumb shit like running 15/33 pulleys on 100mm wheels
[/quote]

Why is this a really dumb shit? 

What would you say is the minimum ratio you could use on 100mm wheels?
```

---
## \#335 Posted by: whitepony Posted at: 2017-03-12T07:31:55.027Z Reads: 412

```
I actually like long ratios - its slowly blending from belt to hublike driving. went from 16/36 to 15-16/33 on 90mm wheels and 190kv single motor on my latest board.

throttle response is smoother, coasting better, less noise especially with foc cause youre in mid rpms, and the torque is still fine for 10% slopes.
```

---
## \#336 Posted by: notepad Posted at: 2017-03-12T19:13:23.063Z Reads: 411

```
I dont see a problem with people trying different ratios.

My latest ratio is 20-36 on 90mm wheels.  its all about seeing what you personally prefer.
```

---
## \#337 Posted by: notepad Posted at: 2017-03-12T19:19:51.418Z Reads: 411

```
Anyway, back to the topic.  Do we have an ETA till we can purchase one.   £220 might be steep, but its a good step towards cheaper ones in the future.  

plus a VESC is the last think I need for my build!
```

---
## \#338 Posted by: psychotiller Posted at: 2017-03-12T23:41:15.905Z Reads: 416

```
I have! But he gladly fixed them.
```

---
## \#339 Posted by: Jebe Posted at: 2017-03-13T02:55:15.126Z Reads: 419

```
Wow, that's service. I'm still waiting for a reply from enertion
```

---
## \#340 Posted by: Pazzo Posted at: 2017-03-13T06:53:54.496Z Reads: 426

```
Hey, so the reason the vesc 6 is priced at 220 for a single unit right now, is for

* The fact that it will show up in 4/5 weeks
* The absence of a warranty
* The limited usergroup due to being unreleased yet
* Of course the added features, and improved hardware

Am I correct that the vesc 6 once officially sold by Trampa, will have a higher cost ?
For two vesc 4 you get less than one vesc 6.
```

---
## \#341 Posted by: Mox Posted at: 2017-03-13T07:58:13.925Z Reads: 412

```
Im surprised that the vesc 6 isnt designed to be waterproof like the EZRUN escs. I feel like there is still work to be done.
```

---
## \#342 Posted by: Maxid Posted at: 2017-03-13T08:00:26.902Z Reads: 417

```
The water proof ESCs are just submerged in Epoxy - this reduces heat transfer and thus makes them less powerful.
With VESC6 you could however make the case waterproof - that is up to you though. Personally I'd rather be able to open the case again than have a waterproof VESC in my already waterproof enclosure.
```

---
## \#343 Posted by: chuttney1 Posted at: 2017-03-13T08:44:36.550Z Reads: 423

```
The cost will be less in the future. They are just testing the "beta" iteration since that is why it cost 220 GBP. Full release won't be until Vedder sorts out the last part of documenting the VESC project to be release as open source platform that can be adapted to more than just electric skateboards for other application and a way to keep funding the development of the project in future.
```

---
## \#344 Posted by: trampa Posted at: 2017-03-13T09:22:12.925Z Reads: 448

```
Hi Mox, the Vesc 6  will have a rubber sealing , so when you tape off the ports, its pretty much splash proof.
Dropping the PCB into epoxy will have three mayor disadvantages. You can't repair things any more, heat dissipation is limited and compliance is an issue - Recycling not possible. Do you really want all these disadvantages? Splash proof is good enough if you ask me. We don't want to create more waste than necessary.

With regards to the price @ VESC (you really should pick a different username BTW, give this one to BEN if you play it fair.): 

-The price includes some product development costs (something Benjamin has swallowed so far).
-Compliance costs (testing to applicable standards) 
-Trademarking (absolutely necessary for Benjamin to have)
-Legal advise through attorneys
-Website for OS-Project (www.vesc-project.com) 
-costs for travelling  
-Extra features (heat sink, sealing, extended bill of materials)
-costs for tooling (injection moulding)
-British VAT ( 20%) which does not apply when you purchase from outside Europe.
-Quality testing
-etc. etc.

In the past a lot of  VESC-Vendors have excluded most product related costs. Playing it fair you would need to ad a good portion on top and send this to Benjamin. 
Many forget about the fact that a product can only be sustained if funding is guaranteed. Its easy if something is available and you can download all the work to send it to a manufacturer. Don't forget that 95% of the work is software related! The reason why no VESC 6 is available yet is not the fact that the hardware is not yet available on github. There is enough public to make the hardware right now! But it will not work without the software and firmware, which is not published yet. You should think about reasonable pricing + should take the mentioned above in consideration when doing so. We will not make a product excluding costs that can't be excluded without an impact on the sustainability of the entire product. This is not in the interest of any manufacturer, nor the customer. 

Everyone wants everything cheap - everyone wants a decent job and a healthy environment. These things do not go well together! Buy less, buy a better quality is our motto. Today quality is mostly refereed to: How is something designed and made. In future you can see who is cutting corners and who is not - then its up to you to make your decision.

Frank
```

---
## \#345 Posted by: trampa Posted at: 2017-03-13T10:00:54.545Z Reads: 418

```
Last call for BETA II! I will close the list in 24 hours. After that we will notify everyone on the list via mail. 


Frank
```

---
## \#346 Posted by: hexakopter Posted at: 2017-03-13T13:09:43.048Z Reads: 412

```
Is the receiving date still end of march? Or any time change because of the Beta II? Thanks.
```

---
## \#347 Posted by: trampa Posted at: 2017-03-13T13:17:07.478Z Reads: 412

```
Hi, Beta II has nothing to do with the date.
We try to push things to get the VESCs ASAP.
I will soon write an update to the group.

Frank
```

---
## \#349 Posted by: longhairedboy Posted at: 2017-03-13T14:13:55.412Z Reads: 439

```
squishy brakes, stretched belts, less powerful accelleraation, and more heat in the sink,which is partially what this thread is about, the VESC6 and how it handles load and other important info. But yeah top speed is the bonus there. When i express opinions like that, its because i've done it myself and found it to be a wtf moment in my personal experience. ITs not intended to disway people from experimentation. God knows we do "dumb shit" all the time in my garage. We call it Science. 

my golden ratios are as follows: 15/36 is about damned perfect on 100mm wheels. For 83s i think 15/33 is where its at, and for 80mm like kegals, 15/32 for a nice balance or or 16/32 if you need that top end. These ratios all are based on a 12S running VESC 4.12

If you like climbing trees or throwing dirt uphill on a trail, i have found that 100mm MBS AT wheels also like 15/37, 15/38, and 14/36 on 63mm cans. 

But now we have the VESC X and VESC 6 is right around the corner, which will certainly change what we consider to be "dumb shit." The VESC X has already changed my mind about some things. Especially when it comes to approaching 2:1 ratios on larger wheels and still expecting a satisfactory amount of torque. 

When VESC 6 is actually here and I have two in my box, I fully expect "dumb shit" to change even more.
```

---
## \#350 Posted by: squad Posted at: 2017-03-13T17:12:38.518Z Reads: 456

```
I'm ready, GIVE IT TO ME :D Custom milled heatsink for dual VESC 6 set up, it will be mounted in UK 206 box lid, of course it will be black :sunglasses:

http://i.imgur.com/Dv0mCsk.jpg

@trampa one more question, will VESC tool be available for OS X at beta stage? Or only windows? It won't be a problem if not, just asking.
```

---
## \#351 Posted by: IDVert3X Posted at: 2017-03-13T22:02:46.304Z Reads: 436

```
Vedder is primarily developing it for Linux, I guess if there is a Windows port, there will be definitely an OSX port as well.
```

---
## \#352 Posted by: Homer900 Posted at: 2017-03-14T02:31:08.164Z Reads: 416

```
Am I to late to get on the Beta?
```

---
## \#353 Posted by: trampa Posted at: 2017-03-14T05:58:34.349Z Reads: 414

```
No, but i need your Name ans email asap.
Frank
```

---
## \#354 Posted by: trampa Posted at: 2017-03-14T08:09:29.384Z Reads: 431

```
For the now macOS is not Benjamins priority. Benjamin will compile a Linux and Windows version to get started. 
Benjamin and Apple are not best friends!
MacOS will need more attention and will only create delays right now. So this will come at a later stage.
Ideally you want to have an App for your smartphone. Apple does not allow any Open Source Software in the App store!
They simply don't like to share. App store policies and OS license contracts contradict each other in a way that no solution is in sight. Its not possible to provide that legally and will probably never be! You would need to use your laptop with macOS and Parallels if you fancy Apple products.

Frank
```

---
## \#355 Posted by: trampa Posted at: 2017-03-14T12:15:16.907Z Reads: 416

```
Dear Betas: Please check your email! Frank
```

---
## \#356 Posted by: monkey32 Posted at: 2017-03-14T14:50:30.632Z Reads: 425

```
Hey Frank,
Betas including the originals, because I don't see anything new from you in my inbox.
```

---
## \#357 Posted by: JTAG Posted at: 2017-03-15T21:43:01.474Z Reads: 431

```
+1        

 
 
 
 
(I hate this forum)
```

---
## \#358 Posted by: Gromok Posted at: 2017-03-15T22:47:39.041Z Reads: 440

```
Frank says there will be a second chance for those who missed. Part message quoted.

"Anyone who missed this opportunity will have a second chance to purchase later this week."
```

---
## \#359 Posted by: Ackmaniac Posted at: 2017-03-15T23:14:22.276Z Reads: 451

```
@trampa Seems that the price went a bit up. I guess this is the final price then because you said already that you don't want to test how the people react on different prices.
<img src="/uploads/db1493/original/3X/d/3/d32149e8cadb97da6a3e3aed8366e0a52721b53f.jpg" width="690" height="430">
```

---
## \#360 Posted by: IDVert3X Posted at: 2017-03-15T23:24:04.555Z Reads: 424

```
Nobody is gonna buy these for dual motor setups at this price point...
```

---
## \#361 Posted by: JohnnyMeduse Posted at: 2017-03-15T23:25:01.180Z Reads: 421

```
@trampa, I hope you know that Bullet , XT and JST connector aren't splash proof, and water can easily travel inside them...
```

---
## \#362 Posted by: Pazzo Posted at: 2017-03-16T05:22:27.875Z Reads: 433

```
It will be interesting to see how much Trampa will offer to Benjamin with his expertise in manufacturing.

Personally I feel that its going to the wrong direction, Trampa and his attorney's don't make a good product, Benjamin does.

I am downhill, push boarder, there's nothing in the world of skateboarding that Trampa has invented and that has revolutionized anything.

The selling for Benjamin's profit of the V6 could have been done in 1 billion different ways, I hope that Benjamin will not have a bad year, so he can keep on laying vesc designs like a chicken.

As for my name, Trampa, you should ask your attorney's about free speech.
```

---
## \#363 Posted by: trampa Posted at: 2017-03-16T07:57:06.853Z Reads: 431

```
Well, I want to prevent this. Basically I'm on a trip to the coast this weekend and I will be offline. We offered a time frame and asked everyone interested in Betas to do the purchase within this period. Sometimes someone misses the chance or faces problems with payment methods etc. and then I have to reopen for these customers, which creates unnecessary work. So if you feel like ordering, please do so now. If you struggle, get back to me ASAP.

Frank
```

---
## \#364 Posted by: trampa Posted at: 2017-03-16T08:15:29.417Z Reads: 445

```
Hi Johnny, you can tape off the JSTs, since its a flat surface, you can shrinctube your connectors. You can silicone seal your JST plugs etc. Don't go diving!. Its just a method to prevent water getting inside when you hit a puddle. We Say "for easy splash proofing" not "splash proof". IP class splash proof would mean to pot it in Epoxy or Urethane and use bulky IP class connectors, use super expensive anti capillary cables no one can solder any more etc. This would basically mean that repairs are not possible + the product would be bulky and even more expensive to make. Having a nice rubber seal and the ability to close the non used JSTs with tape, you are 100% more safe to use it in conditions where a splash could occur. The internal PCB is using an expensive coating BTW. This will still allow repairs. We have pretty much done what we could to improve the situation of current VESC designs. If you like to Pot it, it should be easy to achieve now. We recommend to place your VESC in a dry location if possible. If you want your trousers to be 100% safe from slipping down you better use braces + belt. 

Frank
```

---
## \#365 Posted by: trampa Posted at: 2017-03-16T08:19:37.351Z Reads: 448

```
Keep smiling brother!
```

---
## \#366 Posted by: smurf Posted at: 2017-03-16T09:37:05.036Z Reads: 450

```
I believe repairs on boards dipped in epoxy are easier than you expect. Urethane would be better for smd stuff.

https://youtube.com/watch?v=vpgMn88Qfjs
```

---
## \#367 Posted by: trampa Posted at: 2017-03-16T09:37:09.501Z Reads: 456

```
Update on Monday Guys! I'm away from home spending time with my family from today till Monday! 
Everything is in the make and we push things! Benjamin is improving VESC-Tool further. 
He added a nice little feature to the PCB (Voltage adjustment switch) which caused a minor delay but its worth the time spent. You guys want the ultimate experience and we try to provide it. 
We also made a special Beta-Forum on he official Website to get you guys in touch with each other and us.
This way we can debate the product and VESC-Tool with BETAS.

Frank
```

---
## \#368 Posted by: okp Posted at: 2017-03-16T10:22:04.193Z Reads: 453

```
awesome ! have a blast with your family mate!
```

---
## \#369 Posted by: trampa Posted at: 2017-03-16T10:30:49.481Z Reads: 452

```
Looks like a Video from the 70ths. We use a Coating -its just thinner these days! 

Thx for the info, Frank
```

---
## \#370 Posted by: caustin Posted at: 2017-03-16T12:44:09.509Z Reads: 447

```
great, let us know how to register access to the vesc project website for beta-forum, http://www.vesc-project.com/

...after you get back!
```

---
## \#371 Posted by: trampa Posted at: 2017-03-16T12:45:19.475Z Reads: 447

```
At this stage I will have to set up your accounts and send you the login. You will then change your password.

Frank
```

---
## \#372 Posted by: Pazzo Posted at: 2017-03-17T07:18:02.348Z Reads: 448

```
For the kind of battery two vesc 6 needs and the price they cost, I would consider high end controllers such as the asi bac cadmium 2000.

This is totally the wrong forum for selling packs of two vesc 6, what are you supposed to do ? give one to a friend ?

Skateboards are the wrong platform to go +60Km/h...lmao
Where I live skateboards are in a very nice grey legal zone, despite being speed limited like in a lot of places.

I really want to play with the vesc 6, but for the price of the vesc 6, I can get fulfilled elsewhere, and so can many of you guys as well.

In this time of total craze where everyone is talking about the Vesc6(don't get me wrong its awesome)
...make sure you think wisely about the platform, batteries, speeds you are talking about.
```

---
## \#373 Posted by: Maxid Posted at: 2017-03-17T07:24:32.155Z Reads: 426

```
[quote="vesc, post:372, topic:3813"]
asi bac cadmium 2000
[/quote]

just had a look at the data sheet and the "bigger" version only supports 50A continuous - that is what the VESC 4.12 can do already. VESC6 is a different league and I doubt you will find a cheaper commercial alternative with the same specs.
```

---
## \#374 Posted by: akira Posted at: 2017-03-17T08:07:12.307Z Reads: 426

```
I also looked at the specs. And this ESC can do 50A to 75A ... at 100V !!!
This is very different than 50A at 10 or 12S.

Not saying the VESC is bad, personnaly I prefer the VESC open-source project but you have to compare comparable specs.
```

---
## \#375 Posted by: Maxid Posted at: 2017-03-17T08:47:23.037Z Reads: 436

```
It says:
Output Power (Continuous)(with heatsink) is 2000W. At 50A that means 40V.
So either their data sheet is shit or their controller is not really better than a VESC 4.12 ;)

Link to datasheet:
http://www.accelerated-systems.com/files/20150522_BAC2000-48-70_Datasheet.pdf

PS: It also states: Nominal Input Voltage 36-72V
```

---
## \#376 Posted by: akira Posted at: 2017-03-17T09:17:27.251Z Reads: 432

```
Very True @Maxid
The specs I found did not include the Output Power.
VESC Rulezzzzz :slight_smile:
```

---
## \#377 Posted by: jaykup Posted at: 2017-03-17T14:48:01.197Z Reads: 462

```
[quote="vesc, post:372, topic:3813"]
This is totally the wrong forum for selling packs of two vesc 6
[/quote]

I bought two VESC 6s for $185ea shipped from Europe to USA.  That's comparable to Ollin's VESC 4.12 at $170ea and less than his direct fet version for $220.  I understand that I paid a premium to get them early.  The price will come down in a year or two as more people make them and I see this becoming as popular as the VESC 4.

A 12s4p battery made of Samsung 25R cells is only $150 + some solder.  Gives a 20 mile range with a top speed of 30+.  20mph is a comfortable pace for a smooth flat trail, and the additional power makes hill climbing easy.

Since the original VESC 4 is somewhat unreliable, this seems like a no-brainer.

I get it - Trampa/Frank is the business man, the sales guy, the capitalist, trying to make a buck, and you want open source stuff untainted by the evils of capitalism.  You hate that he's profiting off of Vedders hard work.  

Let me tell you, getting something manufactured isn't easy.  I worked as a project manager for an injection molder and getting tools designed, priced, built, qualified, shipped, tested in house again, work instructions, quality checks and finally product shipped to the customer is a ton of work.  A full time job, literally.  

This partnership makes sense.  Let Trampa manage the manufacturing, delivery, etc and let Vedder do the design.  Trampa's reward for this hard work is first dibs on initial sales ($$$).  As long as he follows through and makes sure everything is released and remains open source, I don't see a problem.  

I just hope Vedder is getting a decent sized chunk!
```

---
## \#379 Posted by: squad Posted at: 2017-03-18T16:54:16.676Z Reads: 444

```
Hi Frank, so just to make things clear, what is the VESC 6 first beta batch ETA for now? Just can't wait to try it out, but I understand Benjamin wants to make sure everything is perfect.

And what is the benefit of this voltage adjustment switch added to the PCB?
```

---
## \#380 Posted by: trampa Posted at: 2017-03-18T17:01:59.264Z Reads: 463

```
Hi Squad I'll check the ETA and get back to you ASAP. The voltage switch allows different Sensors (ABI Hall, AS5047) to work seamless. Some require 3.3, others 5V.
This way you don't need an external voltage regulator. 

Frank
```

---
## \#382 Posted by: Kaly Posted at: 2017-03-20T21:39:45.474Z Reads: 462

```
Great ! 
:slight_smile:
```

---
## \#383 Posted by: squad Posted at: 2017-03-21T21:19:41.666Z Reads: 458

```
Thanks for an update! That's good to hear things are coming along nicely.
```

---
## \#384 Posted by: JTAG Posted at: 2017-03-21T23:55:34.108Z Reads: 464

```
Thanks for the update!

And I am eager to see some production pr*n (6). Please share every picture you have !!!!1!11!1!!1!!!
```

---
## \#385 Posted by: Dimitri Posted at: 2017-03-22T00:26:36.925Z Reads: 456

```
With VESC6, is it still using:  **2.0mm** Pitch JST Connectors like the older ones? or has the pitch changed now?
Thanks :slight_smile:
```

---
## \#386 Posted by: trampa Posted at: 2017-03-22T10:40:55.479Z Reads: 457

```
We use the 2mm JSTs!
```

---
## \#387 Posted by: Tbeg Posted at: 2017-03-22T13:50:36.406Z Reads: 460

```
I love all the work that gets done on all of the Vesc's and I appreciate all of the work that goes on in order for these great devices to be made. I would happily donate but as a student, I cannot even come close to the asking price of the beta V6, so I was wondering what sort of time scale we would be looking at for the pcb files and the same sort of great support for the v4.12 ?

as a novice builder what would you recommend for me ? just going with a v4.12 or waiting for whatever the next form of the v6 will be?
i plan to use either a Turnigy Aerodrive SK3 - 6374-192kv or an Alien 6374 240KV
what esc would be preferred for this setup?
sorry in advance for the off-topic question (it was sort of relevant)
```

---
## \#388 Posted by: jaykup Posted at: 2017-03-22T15:12:34.522Z Reads: 456

```
If you stay at 8-10s with a 192KV motor a 4.12 VESC will be a great setup.  It would be safer to run the VESC in sensored BLDC mode and use a sensored 6374. Less chance of failure.  Stay under 192kv and just change gearing if you need more take-off or top speed performance.  Alien has some sensored ones if you are in the EU, otherwise diyelectricskateboard has a good sensored 6374 for US customers.  I believe Alien will make you a custom motor (any size, KV, sensors, etc) if you are willing to wait.

The VESC 6 really shines at 12s and really high current requirements, and may be somewhat unnecessary for normal riding below that.
```

---
## \#389 Posted by: Tbeg Posted at: 2017-03-22T16:02:24.411Z Reads: 457

```
that's good because I was going to run a custom 10s 18650 pack (or a 2107 pack if they arrive) and a 190 ish kv with a sensor kit.
thanks for the reply, tho I would still be interested in the sort of time frame for the publishing of the vesc 6.
```

---
## \#390 Posted by: Journ Posted at: 2017-03-22T23:58:03.545Z Reads: 452

```
I believe this question is relative to this thread.. Please tell me if it is not and i will gladly delete it.

Where can i find a spec sheet? I need to make sure the Vesc 6.0. Will work best with my build intentions.. I live in the mountains of Western NC USA and need a hearty hill climber.. i know gearing is important but i do not want to burn out the Vesc6.0 also i hope to get a good range and ideally regenerative energy back to the batteries while in use. Also hope to get a nice smooth downhill glide to motorized transition as well as the same for the reverse direction up down backwards and forwards. I was also hopeing to run some Led lights if possible for turn signals, breaking and headlights if possible. Thanks again ~Journ
```

---
## \#391 Posted by: Stevemk14ebr Posted at: 2017-03-23T00:56:07.840Z Reads: 454

```
The vesc can do anything better than any other ESC on the market. So vesc if your best option no matter what it can do. But im pretty sure it can do everything you want with the right gearing
```

---
## \#392 Posted by: Landshark Posted at: 2017-03-23T02:12:25.018Z Reads: 450

```
Is Trampa the only place offering Vesc 6.0?
```

---
## \#393 Posted by: monkey32 Posted at: 2017-03-23T06:12:58.227Z Reads: 463

```
They are the first and currently only....They are working directly with Vedder, the creator of (Vedder Electronic Speed Controller) VESC
```

---
## \#394 Posted by: jaykup Posted at: 2017-03-23T16:52:22.726Z Reads: 498

```
Hill Climbs - this video is great to see what kind of continuous power the VESC 4 and 6 can handle.

**Highlights:**

**VESC 4 testing**
70A for 30 seconds before temperature protection kicks in
35A Continuous from 45 seconds and beyond

**VESC 6 testing**
70A for 3 minutes before temperature protection kicks in
Drops from 70 to 50A from 3 to 5 minutes as temperature protection kicks in
50A continuous from 5 minutes and beyond.

Keep in mind this is all limited by temperature, and adding a fan or some other sort of active cooling can increase the times for both the VESC 4 and 6 to run under high current loads.

As for lights, another video showed the VESC 4 running headlight, taillight and turn signals.

https://www.youtube.com/watch?v=1iwN5LGGM80

https://www.youtube.com/watch?v=G8f0xg7DNmM
```

---
## \#395 Posted by: notepad Posted at: 2017-03-23T23:39:00.663Z Reads: 472

```
Does anyone know how you can access   http://www.vesc-project.com/

The email from Frank from two days ago say we need to use our email addresses and a default password. But I am having no luck,  is anyone else having any luck with this?
```

---
## \#396 Posted by: sl33py Posted at: 2017-03-23T23:42:37.067Z Reads: 457

```
IIRC - Frank is going to email you/us the password when ready.  I know he was traveling and likely still catching up.  Patience...
```

---
## \#397 Posted by: notepad Posted at: 2017-03-23T23:43:28.690Z Reads: 464

```
Cheers.  just a bit eager to get working.  this last part is all I need to finish my first build... The Excitement Is Real!
```

---
## \#398 Posted by: Nordle Posted at: 2017-04-03T16:06:02.997Z Reads: 457

```
Some one knows dimensions from the aluminium case?
```

---
## \#399 Posted by: notepad Posted at: 2017-04-03T17:46:17.555Z Reads: 466

```
Dimensions would be very good to get our hands on.  
I know I want to strap a cpu cooler to the case to give it better cooling, just not sure if the aluminium case is too large/small to make it work.
```

---
## \#400 Posted by: Brad Posted at: 2017-04-04T00:43:43.576Z Reads: 458

```
+1

I also need to know, for enclosure design.
```

---
## \#401 Posted by: whitepony Posted at: 2017-04-04T04:30:07.170Z Reads: 455

```
frank said it somewhere in this thread not superlong ago, scroll up for a while or look for @trampa posts!
```

---
## \#402 Posted by: trampa Posted at: 2017-04-04T10:53:25.703Z Reads: 459

```
I sent a sketch to all beta users. We will not publish the casings details until we got the feedback from beta. Changes might happen and publishing now will frustrate people who start milling things, based on the sketch. 

Frank
```

---
## \#403 Posted by: sanjoy Posted at: 2017-04-04T14:58:00.498Z Reads: 445

```
Frank i didn't receive any sketches!

sanjoy
```

---
## \#404 Posted by: trampa Posted at: 2017-04-04T15:54:39.065Z Reads: 442

```
Just send me a mail. Frank at Trampaboards dot com

Frank
```

---
## \#405 Posted by: sanjoy Posted at: 2017-04-04T16:09:24.694Z Reads: 449

```
Maybe that's why "frank at Trampa boards dot com"
```

---
## \#406 Posted by: Mathias Posted at: 2017-04-06T19:03:27.943Z Reads: 450

```
@trampa So what is the ETA for a VESC 6 for the people that order one now?
```

---
## \#407 Posted by: trampa Posted at: 2017-04-06T20:49:20.508Z Reads: 461

```
We try to get them ASAP to Nottingham. Benjamin just got the first sample for confirmation ( after a week of FEDEX not being able to stick the dam sample into Benjamins letter box.  We hope to get everything assembled and sent to us in the week 17ths to 21 April. We are getting very close to holding them in our hands. For the now we want Beta Testers to do their Job and get them ASAP.  Send me a PM if you wish to be on Beta II, which will ship at the same time as BETA I.

Frank
```

---
## \#408 Posted by: Mathias Posted at: 2017-04-07T11:02:53.474Z Reads: 461

```
OK, thanks! I'll think about it. But right now I am not sure how soon I'll have time to assemble the board, so I'm not sure I am beta material. Might be end of May or so before I could do some serious testing.
```

---
## \#409 Posted by: notepad Posted at: 2017-04-09T01:44:56.264Z Reads: 479

```
@trampa 

Just to double check, was your email " frank@Trampaboards.com "
because  ill pop you an email about those sketches as well,  my builds getting kinda cramped so I was just wondering about dimensions.
```

---
## \#410 Posted by: Jebe Posted at: 2017-04-09T02:15:54.063Z Reads: 470

```
https://www.electric-skateboard.builders/t/vedders-vesc-6-0/3813/262?u=jebe
```

---
## \#411 Posted by: notepad Posted at: 2017-04-09T02:23:10.227Z Reads: 464

```
cheers,  thankyou

This is perfect.  Its just the right size to fit the stock Intel heatsink.  cool temperatures here I come!
```

---
## \#412 Posted by: trampa Posted at: 2017-04-10T12:56:22.483Z Reads: 469

```
Hi, we just did a little test riding this weekend. First production sample landed for confirmation! Benjamin is testing the sample thoroughly, so that we can get BETA VESCs shipped over. 

Benjamin set it up to push 70A towards our motor (40-45Amp rated). We could easily get the motor to 100°C, doing some continuous up hill riding and pushing a second skateboarder (something you should never do).
The VESC 6 stayed completely cool, not even hand warm. So before you are planning to drop heat sinks on, its probably not necessary at all, since the housing is a heat sink already. Next test will be 100A on a bigger motor, which should also just work fine without additional cooling. VESC 6 can handle a lot!
Truth is: it makes no sense to push more Amps in most cases, since your motor stator will reach saturation and increasing any further will have no big effect, except having a terrible low efficiency and a boiling hot motor, which will make it even less efficient, finally ending in a negative spiral towards system shutdown or fried motors. 

Frank
```

---
## \#413 Posted by: notepad Posted at: 2017-04-10T14:15:12.019Z Reads: 461

```
Now you can colour me impressed.  I absolutely cant wait now!!  it sounds like you and Benjamin have made something great again!!!
```

---
## \#414 Posted by: webst Posted at: 2017-04-10T14:36:06.915Z Reads: 450

```
If only they had chosen America!
```

---
## \#415 Posted by: trampa Posted at: 2017-04-10T14:37:32.237Z Reads: 464

```
What we also did was spinning a heavy pneumatic wheel from full forward to full reverse (4500RPM@motor) in a fraction of a second. And Benjamin did that 10 times in 10 seconds. You basically think your drive train will come apart next! Basically it did because I forgot the Locktite on the pulley grub screw (-; 

Then we set the throttle delay to almost zero and implemented an aggressive throttle curve to have a maximum boosted acceleration performance (full power instantly). Very impressive performance.... Driving like that is really scary. I call that the @nowind settings from now on (on/off). All you need is a hand held button.

We do all tests on a single drive with heavy riders to get max. strain on the VESC, motor and drivetrain.

Frank
```

---
## \#416 Posted by: notepad Posted at: 2017-04-10T14:38:56.430Z Reads: 456

```
not gonna lie.  Im getting hyped for this. its sounding amazing!!

keep up the fantastic work!
```

---
## \#417 Posted by: trampa Posted at: 2017-04-10T14:47:38.996Z Reads: 472

```
Me too!  Currently I don't hold one in my hands, just like everyone else. They are all in Sweden to get max. abuse testing in Benjamins ESC torture chamber. Unfortunately Benjamin could not kill one yet, which concerns me a bit. I like destruction testing....
Vesc 4 with BLDC-tool to VESC 6 with VESC tool is a bit like the transition from a flip style cell phone to a modern smart phone. Another league... 

Frank
```

---
## \#418 Posted by: trampa Posted at: 2017-04-10T15:03:59.800Z Reads: 474

```
Benjamin made VESC great again! That's an international achievement and it will be Open Source (no great walls). Zero protectionism and even available to Mexicans. 

Frank
```

---
## \#419 Posted by: Jebe Posted at: 2017-04-15T04:46:03.668Z Reads: 472

```
And carbon neutral for those who believe!
```

---
## \#420 Posted by: JTAG Posted at: 2017-04-19T12:25:45.796Z Reads: 477

```
To all Beta's: There is a lengthy update on the Vedder VESC6 Beta topic on vedder's forum.
```

---
## \#421 Posted by: trampa Posted at: 2017-04-19T12:35:53.616Z Reads: 476

```
http://vedder.se/forums/viewtopic.php?f=6&t=590&start=10

Frank
```

---
## \#422 Posted by: solidgeek Posted at: 2017-04-19T18:44:24.712Z Reads: 487

```
I have considered buying one of the new VESC-X from Enertion, since my ESC from Alien went aflame a few weeks ago... However, the more I read about the upcoming VESC 6.0, it sounds like it is worth waiting for. Are Vedder himself planning to sell the new VESC's then its finished? That would be amazing, especially since I live in Denmark – shipping would be easy!
```

---
## \#423 Posted by: trampa Posted at: 2017-04-19T19:11:11.351Z Reads: 483

```
Hi @solidgeek, Benjamin will not sell them directly. We do that in cooperation. Benjamin can't do everything, so that burden is off his shoulders. PM me if you want one.

Frank
```

---
## \#424 Posted by: hexakopter Posted at: 2017-04-27T23:43:43.379Z Reads: 480

```
[quote="trampa, post:407, topic:3813"]
We hope to get everything assembled and sent to us in the week 17ths to 21 April. We are getting very close to holding them in our hands.
[/quote]


So you already have them in your hands? Would be great to get an update.
```

---
## \#425 Posted by: Brad Posted at: 2017-05-05T01:53:20.529Z Reads: 470

```
@Trampa

Can the vesc 6.0 handle 14 series at 57.4 volts?
```

---
## \#426 Posted by: PXSS Posted at: 2017-05-05T03:49:42.011Z Reads: 466

```
@trampa
I have the same question as above, what is the max voltage??
```

---
## \#427 Posted by: trampa Posted at: 2017-05-05T07:08:00.807Z Reads: 466

```
12S! That's 51V fully charged. Anything higher will kill it.

Frank
```

---
## \#428 Posted by: Brad Posted at: 2017-05-05T07:15:07.113Z Reads: 458

```
Fair enough.

I was hoping I could push 170kv motors to within a hair of the 65,000 limit by going 14 series. (64,890.7 to be exact at 4.1 volts times 14)
```

---
## \#429 Posted by: Maxid Posted at: 2017-05-05T07:18:33.250Z Reads: 462

```
the VESC6 does not have the ERPM limit of the VESC4 - I think I read somewhere that Vedder actually got up to 150.000 ERPM
```

---
## \#430 Posted by: trampa Posted at: 2017-05-05T07:19:10.251Z Reads: 443

```
What 65.000 limit? Vesc 6 can go higher.
150.000 ERPM was no problem so far.
Benjamin tested very fast motors with success. Basically we melted the motor, not the Vesc. 

Frank
```

---
## \#431 Posted by: Brad Posted at: 2017-05-05T07:20:17.244Z Reads: 430

```
That is great!
```

---
## \#432 Posted by: Brad Posted at: 2017-05-05T07:21:31.488Z Reads: 435

```
No worries.

Would be nice to not be limited to 12 series though. :wink:
```

---
## \#433 Posted by: PXSS Posted at: 2017-05-05T10:01:37.469Z Reads: 433

```
Yup... I am currently building a pack that can put out 5kW continuous. :imp:
```

---
## \#434 Posted by: trampa Posted at: 2017-05-05T11:14:40.003Z Reads: 436

```
Trouble starts when you go higher. Different chipsets, and different Standards (low voltage directive etc.).
So we try to stay with 12S.

Frank
```

---
## \#435 Posted by: longhairedboy Posted at: 2017-05-05T11:28:55.578Z Reads: 459

```
[quote="trampa, post:434, topic:3813"]
Trouble starts when you go higher. Different chipsets, and different Standards (low voltage directive etc.).So we try to stay with 12S.
[/quote]

How complex would the upgrades be to go to 13S for example?
```

---
## \#436 Posted by: Ackmaniac Posted at: 2017-05-05T11:52:15.238Z Reads: 474

```
Would be interesting for a ebike with geared motor. There you can't brake with the Motor. So 13S should be OK. Maximum is 54.6V and i also heared that some use it in this configuration. So even with spikes or wrong measurements it shouldn't go higher than 55V. 
But for a longboard it wouldn't work. Or you need a very big battery that can handle the power that get's generated by the motor.

On my 12S8P i checked the data from one of my videos and the voltage goes from 46.67V in idle to 48.11V when i brake with 20 battery amps.
So that's a difference if 1.44V.

Let's assume that we have nearly fully charged 13S battery. (54V).
Then even with some wiggle room and some spikes i shouldn't raise the voltage by more than 2V.
So that would result in 56V. And at 57V is the shutdown.

All very very close to the limit's but it could work.
But for safety it would be a bad idea and it is only doable with a big battery. Guess with a 13S4P you have no chance.

But you could also only charge your cells to 4.1V a cell which would give you 53,3V and more wiggle room to the shutdown at 57V.

Just my 2 cents.
```

---
## \#437 Posted by: trampa Posted at: 2017-05-05T12:03:09.536Z Reads: 457

```
That's up to you to try. We will not rate the VESC to 13S. Sure, you could just charge to 85%, which is healthy for the pack anyway. No Warranty in that case.

Frank
```

---
## \#438 Posted by: Ackmaniac Posted at: 2017-05-05T12:15:56.843Z Reads: 460

```
I totally agree. It's definitely not something you can rate the product for. You need to know what you do when you try to raise your battery to 13S.
```

---
## \#439 Posted by: Necromenz Posted at: 2017-05-09T13:36:37.372Z Reads: 450

```
Hi,

Does anyone know when the beta 2 starts? 
Thx for reply!
```

---
## \#440 Posted by: trampa Posted at: 2017-05-09T13:41:05.206Z Reads: 450

```
We will ship to all BETAS at the same time.

Frank
```

---
## \#441 Posted by: notepad Posted at: 2017-05-09T16:17:56.045Z Reads: 442

```
@trampa  You got them in your hands yet?  if so,  whats your view of the quality?

also does anyone know when the shipping date is?
```

---
## \#442 Posted by: trampa Posted at: 2017-05-09T19:31:29.338Z Reads: 436

```
Quality is spot on. We controlled the entire process A to Z. Samples were shipped to Benjamin and tested. 
Ted and I visited the Company and debated every single detail for two days.
We are 100% happy. No compromise whatsoever. That's what we stand for with our Name.

Frank
```

---
## \#443 Posted by: notepad Posted at: 2017-05-10T02:24:13.270Z Reads: 431

```
I can feel your inner giddy kid over them. #FrankSealOfApproval
```

---
## \#444 Posted by: trampa Posted at: 2017-05-10T06:59:47.667Z Reads: 446

```
We just try our best to make the best gear possible. I hate to cut corners. In the end we all want the best gear possible and a worry free solution. Sometimes that means to dig deeper.

Frank
```

---
## \#445 Posted by: Badkad Posted at: 2017-05-13T17:44:38.058Z Reads: 440

```
If i were to buy one off your site, when would it arrive? (In UK)
```

---
## \#446 Posted by: trampa Posted at: 2017-05-13T18:16:28.686Z Reads: 454

```
Usually it's built the same day and shipped the same day. Monday to Friday....

Expect 2-3 days.

Frank
```

---
## \#447 Posted by: solidgeek Posted at: 2017-05-13T20:31:30.128Z Reads: 456

```
Does that mean that the VESC 6 will be shipping out soon? Would be nice with an update :slight_smile:
```

---
## \#448 Posted by: JTAG Posted at: 2017-05-14T12:43:35.092Z Reads: 462

```
https://youtu.be/cbUzDxM67ng
```

---
## \#449 Posted by: Print3r Posted at: 2017-05-14T12:50:54.018Z Reads: 458

```
Will this test bench be open sourced or is it closed source?
```

---
## \#451 Posted by: Mathias Posted at: 2017-05-18T21:38:18.494Z Reads: 455

```
Let's get past this stupid trademark outrage and get back to the real thing:
[quote="trampa, post:446, topic:3813, full:true"]
Usually it's built the same day and shipped the same day. Monday to Friday....

Expect 2-3 days.

Frank
[/quote]

@trampa, I'm a bit confused: 2-3 days from when? Will this be different from the beta version? (beta 1/beta 2, is there a difference between the two?)?  Your webpage still states "DISCOUNTED ADVANCED PRE-ORDERS BEING TAKEN NOW!". Could you please clarify?
```

---
## \#452 Posted by: trampa Posted at: 2017-05-18T22:18:25.467Z Reads: 438

```
I referred to boards. The VESCs all arrive next week and will be shipped after a spin up test. 

Frank
```

---
## \#453 Posted by: Badkad Posted at: 2017-05-19T14:27:19.530Z Reads: 436

```
I was referring to the VESC's, that confused me because of the pre orders being on the page still. I understand now, I'll hold off until you have it properly listed on your site.
```

---
## \#454 Posted by: Titoxd10001 Posted at: 2017-05-20T20:49:48.103Z Reads: 430

```
When will vesc tool be available to the public? Will it be compatible with non-vescs based on vesc's (4.12, focbox). What improvements can we expect? Duty cycle?
```

---
## \#455 Posted by: trampa Posted at: 2017-05-22T12:13:57.009Z Reads: 444

```
Sure, after BETA. The list of improvements is far to long to be named here. 100% new software, no old code, 100% new firmware, multiple hardware support incl. the old designs, setup wizards, throttle curves for different input devices, NRF pairing, update server telling you that updates are available, weekly updates, firmware integrated, no more looking for suitable firmware, automatic hardware detection, better graphs and analysis, better structure.....it's endless. 
Basically a full restart of everything! VESC 4 will profit a lot from VESC-Tool. My VESC 4 runs a treat with the latest firmware. FOC is so much better now!
Once available, you can download it from Benjamin's server, through www.vesc-project.com. 
You will also be able to donate some $$ to Benjamin during the checkout (downloading) process.
People donating will get a nice bonus on top. Surprise! 

Frank

A tiny detail I forgot: Benjamin integrated a full documentation into the Software. Question marks behind every single setting let you know more about everything, and will help you to understand better what you do or could do.
```

---
## \#456 Posted by: JTAG Posted at: 2017-05-22T13:45:20.392Z Reads: 412

```
:grin: WE NEEDZ PICTURES OF ELECTRONICS :grin:
```

---
## \#457 Posted by: Hummie Posted at: 2017-05-22T13:58:58.387Z Reads: 413

```
I believe the 6 will have an over-ride motor amp limit of 120 amps unfortunately.  Just like the version 4.  So while it could possibly put out way more power it's being held back by the software and even if u put your motor amps past 120 it won't go
```

---
## \#458 Posted by: Brad Posted at: 2017-05-22T14:11:17.842Z Reads: 411

```
I'm not sure why you would need more than 120amps per ESC on a skateboard? 

Fully charged in 12s at 120amps for a single motor would be 6,048watts, 10s would be 5,040watts......Double that for dual motors at 240amps.
```

---
## \#459 Posted by: jaykup Posted at: 2017-05-22T14:32:49.048Z Reads: 399

```
Ebikes, other EVs, could use the _VESC_(TM)(R)(C)(Made by Vedder)(Property of Vedder)(Also Trampa)*** but usually need higher amperage.

Also off-road mountain boards.
```

---
## \#460 Posted by: trampa Posted at: 2017-05-22T15:01:09.288Z Reads: 398

```
Vesc(R) SIX by Trampamean Vedder is strong enough! Limit isn't set by software. Vesc-Tool will tell you "you are doing something stupid" in case you drop in potentially destructive values. I think the DRV issue will shift towards cooked motors. 

Frank
```

---
## \#461 Posted by: Brad Posted at: 2017-05-22T15:02:39.196Z Reads: 401

```
@jaykup Yes that is what I thought, just was not thinking of e-bikes due to this being an e-sk8 board. Trampa is a mountain board shop, so not sure why they would restrict it if mountain boards would need more? We will see if it is capped at 120amps or not :confused: Dual motors would be as much at 12,096watts.

@Trampa I'm aware that speed can be capped, but what about wattage? I mean say, at 5% charge, the wattage is 1,500 per motor, could I put a cap so it stays at 1,500 watts per motor when fully charged and there fore the max wattage the motor uses is the same through out the battery charge range?
```

---
## \#462 Posted by: Hummie Posted at: 2017-05-22T15:05:08.675Z Reads: 389

```
At low duty cycle, (low speeds) the "effective voltage" is reduced way down. At 5% duty ur at 5% max speed and 5% of pack voltage.  The math there brings the wattage way down at the lower speeds.  Multiply using maybe 2 or 3 volts.
```

---
## \#463 Posted by: trampa Posted at: 2017-05-22T15:08:35.884Z Reads: 398

```
Are you talking about WATT control?

Frank
```

---
## \#464 Posted by: Brad Posted at: 2017-05-22T15:10:30.779Z Reads: 399

```
Yes, please be gentle.:neutral_face:
```

---
## \#465 Posted by: Brad Posted at: 2017-05-22T15:20:41.472Z Reads: 434

```
Just explaining how I came to this line of thought.

I set max ESC amps at 40 so it would be 80 amps max with two ESC's.

What I did was calculate the speed at low voltage by going 10 series to make the voltage 37v as you can see below. Top speed weighted is 35.96km/h. Lets round it at 36km/h

<img src="/uploads/db1493/original/3X/f/0/f0e0b6f000e0cba25c2555dade3bb416c738cf0b.png" width="626" height="499">

Now when the battery is fully charged in the esk8 calculator by going 12 series to get 44.4v, I get top speed weighted at 43.16km/h, lets round it to 43km/h

<img src="/uploads/db1493/original/3X/7/2/72cd9703d95373814d49bff4dc2781dec5b5653e.png" width="627" height="499">

What I assumed to do is at max wattage on low voltage of 37 would be 37 times 40amps = 1480 watts for 36km/h

Fully charged at 44.4v would be 44.4 times 40amps = 1776 watts at 43km/h.

I cap the speed at 36km/h so I get 36km/h when fully charged and still get the same top speed till voltage is down to 37v so I have consistent top speed for my commuting board. 

I assumed if I also cap the wattage at 1480 watts even when fully charged, the power level would also be more consistent due to also capping top speed at 36km/h although I understand there will still be a bit more torque at full charge due to higher voltage.

In nutshell, consistent speed and wattage usage despite 100%,50% or 20% battery.
```

---
## \#466 Posted by: Hummie Posted at: 2017-05-22T15:32:27.477Z Reads: 414

```
I'm saying if u hook up a wattmeter or an amp meter from the battery to esc you'll find due to the way an esc works w pwm at low speeds there's an "effective voltage", which will be much lower than the pack voltage.  At maybe 5% of ur max speed ur at 5% duty cycle and that means with continuous switching on and off, and a lot of off at so low a duty cycle, the motor will see 5% of what the pack voltage is.  So while u can hit 120 motor amps, as that's the software limit, the voltage u would multiply with to figure the wattage ur doing is..5% of whatever the pack voltage is.   At higher speeds the duty cycle goes up, follows the speed,  so u will hit max power at 100% duty cycle and at that point u can multiply using the full pack voltage
For example if u set ur max motor amp to 120 and battery max amps to 60 and u have 12s 50volts.... At 5% of max speed you'll still only have access to ...120(close to) X 5v...so 600 watts.
The 6 is said to be able to do
Much much more but none-the-less the motor amp limit limits power out at low duty/speed
```

---
## \#467 Posted by: Brad Posted at: 2017-05-22T15:36:07.780Z Reads: 408

```
Ahhh, now I'm starting to see what you are getting to. Going up a mountain may be a bit slow therefore 5% not gonna work unless you jack up the amps for torque at low speed due to low duty cycle.

I only knew if battery is nearly flat, need more amps but not if battery is full but you want to go slow and need torque at the same time.

Sooo nice to learn something new :+1:
```

---
## \#468 Posted by: Hummie Posted at: 2017-05-22T15:41:56.132Z Reads: 407

```
im saying if ur going very slowly and hit full throttle, even if ur batt and motor amp limits are set to their Max, u won't get near the power output possible of the 6 until u go faster
```

---
## \#469 Posted by: trampa Posted at: 2017-05-22T16:18:46.913Z Reads: 416

```
Sorry, I was kidding.

Frank
```

---
## \#470 Posted by: JTAG Posted at: 2017-05-22T21:12:26.262Z Reads: 428

```
@trampa Please pinky promise to send us PCB NUDES :smiling_imp::stuck_out_tongue_winking_eye: (once they arrive ofc)!
```

---
## \#471 Posted by: sl33py Posted at: 2017-05-22T21:23:26.707Z Reads: 446

```
Take a look at the videos from Ben - plenty of PCB pr0n:

https://www.youtube.com/watch?v=bivXOlqooCE

https://www.youtube.com/watch?v=1iwN5LGGM80

https://www.youtube.com/watch?v=DSFHutWW5fM

Can't wait!
```

---
## \#472 Posted by: trampa Posted at: 2017-05-22T21:29:21.804Z Reads: 428

```
Promised if you promise to tame yourself.

Sad news: Benjamin broke is foot on Saturday. Guss how? Doing dangerous esc- research on an Evil twin drive 12S 7P, dual VESC SIX Trampa MTB, thrashing down the craters test track at ridiculous speed.
Just kidding: Tire exploded, worn out, couldn't wait for the parcel with new tires.
He thought the battery exploded and jumped off at speed. One foot got stuck, board spun the foot 270deg. FUCK!

Result:
Eight titanium kingpins in his right foot and leg. Just had a longer conversation with him. BETA is in no danger. He has his fingers on the keyboard already, slightly slowed down by a good portion of morphine, still faster than anyone else.

Do me all a favor and send him your best wishes through his forum! 

Frank
```

---
## \#473 Posted by: caustin Posted at: 2017-05-22T21:45:50.652Z Reads: 409

```
best wishes, and OUCH!
```

---
## \#474 Posted by: doh Posted at: 2017-05-22T21:53:24.120Z Reads: 406

```
Get well soon! Reminds me to get me some protective gear...
```

---
## \#475 Posted by: Achmed20 Posted at: 2017-05-22T22:25:44.734Z Reads: 407

```
ouchy. maybe i should use my motorcycle boots after all ^^
best wishes to the ESC grandmaster
```

---
## \#476 Posted by: trampa Posted at: 2017-05-22T22:26:40.356Z Reads: 411

```
Do so! Worth every penny. He had a helmet at least. Heal straps are a must have when riding with bindings.

Frank
```

---
## \#477 Posted by: makevoid Posted at: 2017-05-22T23:09:42.974Z Reads: 408

```
 :no_mouth: omg, hugs to BV, get well soon!
```

---
## \#478 Posted by: JTAG Posted at: 2017-05-22T23:23:18.349Z Reads: 415

```
[quote="trampa, post:472, topic:3813"]
promise
[/quote]

I will, I will, Its just; every update expands my patience a little, I think pictures will expand it even further... Just kidding :grin: , keep up the good work you doing and try to get some rest, you seem to be online 24/7 :fearful: .

I went to the forum and wished him all the best, and the other thing -> The BETA is nowhere near as importance as your personal life / health. You guys should take enough rest, and especially Ben right now :(, we can wait!
```

---
## \#479 Posted by: chuttney1 Posted at: 2017-05-23T01:21:36.653Z Reads: 398

```
Can we at least get the dimension of the VESC 6.0 or a CAD version of the completed reference board?
```

---
## \#480 Posted by: squad Posted at: 2017-05-23T07:05:28.944Z Reads: 404

```
I know this only too well, 14 stainless screws, 2 stainless plates in my forearm and one titanium screw in my wrist, 5 more weeks of immobilization to go 😐. Morphine was nice tho 😄 Hope Ben recovers fast, I'm literally tired of waiting to get back on my boards, this time with wristguards on.
```

---
## \#481 Posted by: trampa Posted at: 2017-05-23T08:04:45.631Z Reads: 400

```
I will try to book a flight to see him and help him a bit next week, shopping cooking etc.
Putting pressure on my wife though, needing to care for the kids all alone. 

Frank
```

---
## \#482 Posted by: squad Posted at: 2017-05-23T08:10:26.274Z Reads: 393

```
I wouldn't be able to tie a shoelaces without my girlfriend, I'm sure Ben would appreciate some help if You have a chance.
```

---
## \#483 Posted by: trampa Posted at: 2017-05-23T09:21:09.503Z Reads: 394

```
I will try my best! Lucky he is, that Air Berlin flies four times a day, 7 days a week. Not cheap though, 300€ per trip.

Frank
```

---
## \#484 Posted by: akira Posted at: 2017-05-23T09:24:01.414Z Reads: 389

```
Can you please stop using this very sad accident of BV to promote yourself and show how good you are ?
```

---
## \#485 Posted by: trampa Posted at: 2017-05-23T10:53:47.319Z Reads: 392

```
Sorry, not my intension. People want the BETA to start, there is some serious pressure on his shoulders right now. 
Such an accident is a bad thing and I will do what I can to help out if necessary. He can't walk, stand up, nor go shopping. 
I'm a bit worried to be honest! I'm pretty tied in and not as flexible in taking time off because it creates pressure for my better half. It's a miserable situation.... 

Last comment on that!
```

---
## \#486 Posted by: notepad Posted at: 2017-05-23T10:55:14.253Z Reads: 390

```
what are you talking about.  all Frank is doing is saying how his friend has broken his leg.  We are all part of the eSk8 family and BV is part of that family.
```

---
## \#487 Posted by: trampa Posted at: 2017-05-23T12:00:11.105Z Reads: 391

```
Benjamin and I will start with the reference design as soon as the software is out. It's sketched up but still needs a bit of attention. It needs to be really good and flexible to adopt. The only way to do it is to make one thing happening after another. To little man power! Now Benjamin can't stand up, walk nor solder the prototype and test ride it. So I will send the designs to be made somewhere in a small batch, rather than hand solder them. It will slow things down a bit. Please no pressure right now. Bones need to cure! This accident will delay things slightly. Health is more important. He is really not capable of standing up! Foot was pointing backwards and hanging down in a 90°angle! Hurts thinking about it. 

Frank
```

---
## \#488 Posted by: hexakopter Posted at: 2017-05-23T16:38:54.832Z Reads: 403

```
[quote="trampa, post:487, topic:3813"]
To little man power! Now Benjamin can't stand up, walk nor solder the prototype and test ride it. So I will send the designs to be made somewhere in a small batch, rather than hand solder them. It will slow things down a bit.
[/quote]
First of all best wishes to Benjamin. Hope he will get well soon.
Why building small incredible expensive batches somewhere and not team up with a third person that is able to handsolder and also test things? I think outsourced sample production in china in the developing phase slows the whole process down a lot (less important), but also costs unnecessarily a lot of money. (more important) I think it would be possible to find a person that can handsolder himself, knowing a little bit about EE to contribute and is willing to help. :wink:
```

---
## \#489 Posted by: trampa Posted at: 2017-05-23T17:08:07.498Z Reads: 396

```
Thx man! Vesc needs good guys helping.

Frank
```

---
## \#490 Posted by: hexakopter Posted at: 2017-05-23T17:20:42.105Z Reads: 412

```
I hope you see the hint who that person maybe is. :blush: At least one of them.
```

---
## \#491 Posted by: JTAG Posted at: 2017-05-23T17:48:18.055Z Reads: 420

```
@trampa 

I am willing to solder your  (and benjamins ) prototypes :grin:. For an impression of my soldering skills look at this topic: 

https://www.electric-skateboard.builders/t/diy-6s-to-12s-bms-with-can/2639
```

---
## \#492 Posted by: trampa Posted at: 2017-05-23T18:17:35.005Z Reads: 414

```
Now we are starting to talk VESC again! 
People standing together to make things happen! I can't here all that ... anymore.
Make stuff happen should be the spirit!

Frank
```

---
## \#493 Posted by: JTAG Posted at: 2017-05-23T21:35:24.294Z Reads: 408

```
Haha, ofc, electronics prototyping is relaxing for me. Let me know when / if you need help!
```

---
## \#494 Posted by: trampa Posted at: 2017-05-23T21:52:12.170Z Reads: 404

```
Would be nice! Helping hands are welcome!

Frank
```

---
## \#495 Posted by: dakota4e Posted at: 2017-05-24T01:41:02.749Z Reads: 393

```
How are we sitting on Beta Frank?  Still on schedule to go out this week?
```

---
## \#496 Posted by: trampa Posted at: 2017-05-24T07:44:53.015Z Reads: 402

```
They are on the way to us! following tracking....
As soon as they are there, Ted will drop the firmware on and will do the test runs. Then we pack and ship.
I will fly over to Benjamin and will help him. Frank does the cooking, Benjamin the coding. Fair split of work....
I started to create your accounts on the Website. An email notification is in preparation. You should be able to log in the day you get your VESC SIX. 
Benjamin will ad another nice feature to the tool! Be surprised. We will try to provide weekly updates for the Software.

Frank
```

---
## \#497 Posted by: Brad Posted at: 2017-05-24T08:27:47.323Z Reads: 394

```
Just curious, are you and Ted co-owners of Trampa or ?
```

---
## \#498 Posted by: trampa Posted at: 2017-05-24T08:30:19.530Z Reads: 407

```
YES we are.We are a small outfit. Ted is in Nottingham, banging on stuff and sorting out your orders. I'm in Berlin, sorting out the R&D. We both do customer service. I fly over once a while and Ted flies over once a while.

Frank
```

---
## \#499 Posted by: trampa Posted at: 2017-05-24T08:58:29.947Z Reads: 414

```
They have arrived! Photos soon. We will do the flashing and testing ASAP. Full of excitement!

Frank
```

---
## \#500 Posted by: JTAG Posted at: 2017-05-24T09:26:16.175Z Reads: 417

```
YOU PINKY PROMISED!!!?!?!?!???!!!!!

<img src="/uploads/db1493/original/3X/5/b/5b79e5e044b57771d4c8f7a9a285e801757c0c00.jpg" width="690" height="388">
```

---
## \#501 Posted by: trampa Posted at: 2017-05-24T09:58:05.802Z Reads: 428

```
Ted is still doing some moving today and tomorrow. He organized a Truck and need to make the most of it.
He promised to take some pics and send them over the minute he finds the time. Flashing and testing will be done when Ted has sorted moving stuff and Benjamin feels up to the task to join in on Skype on Friday. I fire in your accounts into the System, so everything should finish at the same time. Next week, when you all have your VESCs, I'll be in Sweden, so customer support should be no issue.  We want some footage of VESC SIX in action BTW.

<img src="/uploads/db1493/original/3X/4/2/42416dc5740b111934eb0b66b3ee41494d453a4f.jpg" width="690" height="387">

Frank
```

---
## \#503 Posted by: notepad Posted at: 2017-05-24T13:17:41.801Z Reads: 416

```
Dont worry Frank, everything for my board is ready,  just waiting on the VESC, should be able to get some decent footage for ya.
```

---
## \#504 Posted by: trampa Posted at: 2017-05-24T13:19:55.695Z Reads: 429

```
<img src="/uploads/db1493/original/3X/d/8/d89faa24bd48160ff35f4ded18e1190be12df890.JPG" width="375" height="500"><img src="/uploads/db1493/original/3X/5/4/54ac45991aa8b2e465e01f1fafb6e6488fabd108.JPG" width="375" height="500">
```

---
## \#505 Posted by: JTAG Posted at: 2017-05-24T13:33:40.376Z Reads: 425

```
Sorry is was driving as well:
<img src="/uploads/db1493/original/3X/8/0/80bc403b147980347e1e4b75d0e23f346358978a.jpg" width="375" height="500">

I see you managed it all ^^!
```

---
## \#506 Posted by: elektrinis Posted at: 2017-05-25T13:48:39.950Z Reads: 420

```
Very interesting project, was a follower for a long time.
Has anyone have a version of this or similar PCB on Altium? I would love to do some PCB mods per my personal liking...
```

---
## \#507 Posted by: Boesila Posted at: 2017-05-29T14:58:03.165Z Reads: 411

```
How is the recovery of Benjamin, was he able to join the Skype call last Friday?  Was the testing and falshing of the VESCs sucessfull... please give us some update :-)

@BV: Get well soon! Hopefully you are on a good way :+1:
```

---
## \#508 Posted by: trampa Posted at: 2017-05-29T15:26:20.973Z Reads: 410

```
I will fly over tomorrow and will help Benjamin. Doctors made a mistake (to long titanium screws) and needed to do the job again. Mechanics... Unbelievable! 
Anyway, we will flash your VESCs and ship them tomorrow or on Wednesday. We are prepared and just wait for me being in Sweden tomorrow afternoon. I think its better this way and its not a terrible delay.

Frank
```

---
## \#509 Posted by: DougM Posted at: 2017-05-29T15:31:14.100Z Reads: 403

```
Only go to doctors who are also e-sk8ters.  They always use the right screw.

All our best to Benjamin
```

---
## \#510 Posted by: JTAG Posted at: 2017-05-29T18:20:52.874Z Reads: 399

```
Ouch that sounds awful :sweat:.
```

---
## \#511 Posted by: trampa Posted at: 2017-05-29T19:39:31.542Z Reads: 390

```
Yes, to bad when screes poke through the bone into the joint... 
In a couple of years we will probably see artificial joints with bldc motors running on VESCs. 

Frank
```

---
## \#512 Posted by: Jebe Posted at: 2017-05-29T20:42:10.883Z Reads: 390

```
And loctite ;)
```

---
## \#513 Posted by: JTAG Posted at: 2017-05-30T18:13:58.918Z Reads: 392

```
How is the VESC godfather doing :hushed:?
```

---
## \#514 Posted by: trampa Posted at: 2017-05-30T18:27:03.451Z Reads: 404

```
In bed and ready for the task in the morning. We just came back from hospital...
Tomorrow is the exiting day! Flashing, packing, sending.

Frank
```

---
## \#515 Posted by: longhairedboy Posted at: 2017-05-30T18:38:00.228Z Reads: 398

```
@trampa They did thread lock his screws though right? we don't need them falling out in the street.
```

---
## \#516 Posted by: trampa Posted at: 2017-05-31T01:49:03.577Z Reads: 397

```
That's how I specified it. I didn't touch one yet. I'm in Sweden, banging on BETA stuff with Benjamin. I'll ask Ted to wind some screws out.

Frank
```

---
## \#517 Posted by: squad Posted at: 2017-05-31T07:46:33.057Z Reads: 396

```
I think @longhairedboy meant Benjamin's foot :wink:
```

---
## \#518 Posted by: sebaszz Posted at: 2017-05-31T08:32:26.723Z Reads: 400

```
Good luck guys! also Ben with his recovery , these are exiting times for us all :slight_smile:
```

---
## \#519 Posted by: caustin Posted at: 2017-05-31T11:59:54.730Z Reads: 409

```
No, I think he is pulling his leg lol.
```

---
## \#520 Posted by: JTAG Posted at: 2017-05-31T19:12:55.267Z Reads: 416

```

MUST HAVE TRACKING NUMBER. WILL LOSE ALL SELF CONTROL in 10. 9. 8. 7....
```

---
## \#521 Posted by: dakota4e Posted at: 2017-05-31T19:19:47.420Z Reads: 421

```
This......just waiting for speed controllers.......;)
<img src="/uploads/db1493/original/3X/2/2/2250429674610c3a26349920a4dfc606f305587d.png" width="666" height="500">cid:BBF541F3-1B2C-4794-9FEE-C8522FE225D2@midcoip.net
```

---
## \#522 Posted by: monkey32 Posted at: 2017-05-31T20:15:38.922Z Reads: 411

```
daaaaaaaaaaaanm what size or those motors?
```

---
## \#523 Posted by: Maxid Posted at: 2017-05-31T20:19:48.801Z Reads: 409

```
Those look like the standard trampa motors: 6364
```

---
## \#524 Posted by: dakota4e Posted at: 2017-05-31T21:37:40.293Z Reads: 411

```
Correct! 136Kv.

This dog is ready to hunt upon arrival of VESC6.
```

---
## \#525 Posted by: trampa Posted at: 2017-06-01T10:09:55.813Z Reads: 415

```
Today is the day! We flashed some yesterday and will do the rest today. Packing and shipping today and tomorrow morning. Benjamin and I bang on the website and your VESC-Tool Original every single minute. I think tomorrow afternoon we can open your accounts for the website and you can download VESC-Tool for VESC SIX. VESC-Tool with VESC 4 support will follow next week. 

Frank
```

---
## \#526 Posted by: notepad Posted at: 2017-06-01T12:57:31.554Z Reads: 406

```
I cant wait,   what type of shipping, and parcel size, so I can make sure I am in the house at roughly the correct time?
```

---
## \#527 Posted by: sayreul Posted at: 2017-06-01T15:22:56.681Z Reads: 406

```
Hi @trampa 
> VESC-Tool with VESC 4 support will follow next week.

do VESC Tool will add functionalities for VESC 4 or do we have to wait for a new FW for VESC4
```

---
## \#528 Posted by: chaka Posted at: 2017-06-01T15:57:50.724Z Reads: 402

```
It comes with new firmware.
```

---
## \#529 Posted by: trampa Posted at: 2017-06-01T16:29:25.688Z Reads: 403

```
Right! FW integrated.

Frank
```

---
## \#530 Posted by: trampa Posted at: 2017-06-01T16:30:26.618Z Reads: 403

```
Small box, not fitting through the letter slot.

Frank
```

---
## \#531 Posted by: notepad Posted at: 2017-06-02T02:10:26.500Z Reads: 415

```
Thanks Frank.   will we be getting a tracking number?
```

---
## \#532 Posted by: trampa Posted at: 2017-06-02T13:23:33.774Z Reads: 412

```
I have to ask Ted if he can fire that into our System. We will send them tracked anyway.

Frank
```

---
## \#533 Posted by: trampa Posted at: 2017-06-02T14:34:10.281Z Reads: 410

```
Betas just got a mail! BETAs can now log in to www.vesc-project.com and download the software + use the forum.

Frank
```

---
## \#534 Posted by: notepad Posted at: 2017-06-02T16:10:24.155Z Reads: 407

```
WOO HOO, hype train all ahead full!
```

---
## \#535 Posted by: JTAG Posted at: 2017-06-02T16:25:28.578Z Reads: 414

```
The new vesc tool looks AWESOME!
```

---
## \#536 Posted by: trampa Posted at: 2017-06-02T17:40:45.239Z Reads: 414

```
<img src="/uploads/db1493/original/3X/5/6/564d14c0936f371e3e393ec91211abcb90b24e88.jpg" width="375" height="500">
```

---
## \#537 Posted by: Necromenz Posted at: 2017-06-02T18:47:37.983Z Reads: 410

```
Hi frank,

I got no email for the Betaforum. The shippingemail i got. 
?? Hope you can help.
```

---
## \#538 Posted by: trampa Posted at: 2017-06-02T20:16:11.111Z Reads: 408

```
Pm your mail and I'll drop you on instantly.

Frank
```

---
## \#539 Posted by: Necromenz Posted at: 2017-06-02T20:52:48.274Z Reads: 400

```
Nice new vesc-tool!! 
THX Frank
```

---
## \#541 Posted by: Tarzan Posted at: 2017-06-04T21:28:55.206Z Reads: 388

```
Damn!
It hurts so mutch but I can't touch the VESC6s when they arrive at my place, because of life.... ☹️😭
With luck I will test them end of June.
```

---
## \#542 Posted by: notepad Posted at: 2017-06-05T17:26:59.790Z Reads: 391

```
I cant wait for mine to arrive,  I have no idea what I am doing though,  anyone got any good tutorials for using the new VESC Tools?
```

---
## \#543 Posted by: HTownBomber Posted at: 2017-06-05T17:35:04.863Z Reads: 402

```
Trampa included some damn good documentation in the VESC 6 manual that Frank emailed to us.  Also the software should be more intuitive (although I haven't played with it yet).  For further reading on motor detection, testing & tweaking your settings to match the rest of your setup, do a search for the VESC 4 and start reading.  Then read some more.  Then put your board on the bench and play around wiith it.  

While the interface and design is all new, I have to imagine that much of the info / recommended settings from the old BLDC-tool will translate over to the new VESC-tool / VESC 6.
```

---
## \#544 Posted by: sl33py Posted at: 2017-06-05T17:57:45.997Z Reads: 425

```
Just downloaded the new VESC Tool and poked about a bit.  It is *stupid simple* now and has simplified wizard step-through processes for most common needs.

Re-D/L it to look for you at work.  

<img src="/uploads/db1493/original/3X/5/f/5f86d1253f4da00d4bb3e0eb096893b232137021.jpg" width="690" height="440">
Try "Motor Setup Wizard [MOTOR]" button right in the middle when VESC connected.

I don't have VESC at work, so i cannot go past first step in Wizard:
<img src="/uploads/db1493/original/3X/d/d/dd8de92e0d52d018710d587a2105129f7ca27d4a.jpg" width="690" height="414">

Or you can go to the BLDC "tab" on left side (or FOC if you want):
<img src="/uploads/db1493/original/3X/e/8/e800162eb068e74928cab2a1f8060dc40aac75f1.jpg" width="690" height="440">
The new information hover overs and pop ups are AWESOME!  Tons of info, so click and read as you go and have questions.  Then the "run" button is the detect motor start.  Follow similar steps to the videos for older BLDC tool, but with easier "apply" steps after detection.

And don't forget there's a pretty detailed user guide Ben already published on vesc-project.com - so start reading and you should be set by the time your VESC Six arrives.

HTH - GL!
```

---
## \#545 Posted by: NAF Posted at: 2017-06-05T19:39:19.748Z Reads: 400

```
Is there a MAC version ?? Where can I download it ?
```

---
## \#546 Posted by: sl33py Posted at: 2017-06-05T19:59:06.955Z Reads: 394

```
Just Windows and Linux on vesc-project.com site.  Access to the site has been given as part of the VESC 6 beta.

Waiting on support for VESC 4.xx in the new VESC Tool - currently only has FW for v6.  Supposed to be about a week...
```

---
## \#547 Posted by: TranxFu Posted at: 2017-06-05T20:10:46.074Z Reads: 389

```
Is this going to benefit users of the VESC 4.XX besides a cleaner user interface and experience ?
```

---
## \#548 Posted by: hexakopter Posted at: 2017-06-05T21:18:13.141Z Reads: 398

```
[quote="sl33py, post:544, topic:3813"]
And don't forget there's a pretty detailed user guide Ben already published on vesc-project.com - so start reading and you should be set by the time your VESC Six arrives.
[/quote]

What user guide do you mean? I can't find it.

@TranxFu Yes
```

---
## \#549 Posted by: sl33py Posted at: 2017-06-05T21:30:44.267Z Reads: 413

```
I thought it was on the site, but actually got it via email.

i have the pdf @Trampa sent me 3 days ago.  Look in your inbox for email w/ subject "vesc-project.com"

<img src="/uploads/db1493/original/3X/e/5/e5c3a87a5b229e9cf8f378492aa8b9ac818e08fb.png" width="676" height="500">
```

---
## \#550 Posted by: hexakopter Posted at: 2017-06-05T21:36:27.914Z Reads: 402

```
Ah thanks. Now I know what you were talking about. 
Btw I dont know if it is wanted that your share all your pictures here or if it is just for the BETAs right now.  Maybe @trampa could clarify that.
```

---
## \#551 Posted by: sl33py Posted at: 2017-06-05T21:41:38.641Z Reads: 400

```
Yeah - and that's why i just showed a quick screen grab of it, vs attaching.  I don't want to share something that's still being refined and "beta".

@Trampa / Frank - let us know if any issue sharing the pdf?
```

---
## \#552 Posted by: trampa Posted at: 2017-06-06T08:16:07.783Z Reads: 417

```
It's fine to show it, since it will go public very soon (after 4weeks of BETA). Anyway, if you want to debate stuff and place questions, please use the www.vesc-project.com Beta Forum, since Benjamin is on there and not here. So that will help us to keep the flow of information condensed and in one place. This way we can generate a better documentation for new users. I think in future its best to deal with VESC-related QA via the official VESC forum. 

VESC-Tool for MAC: That is another step to take. For the now you want to use parallels. We will try to sort out an app ASAP. The problem about MAC is that Open source and iPhone contradicts each other. Open source code in the apple store is not allowed (read their terms and conditions)! Benjamin does not want to support closed source software. The VESC-Project is Open Source! Since a official VESC-APP is overdue, its on Benjamin's priority list. 

Frank
```

---
## \#553 Posted by: lock Posted at: 2017-06-06T09:13:36.447Z Reads: 416

```
[quote="trampa, post:552, topic:3813"]
since it will go public very soon (after 4weeks of BETA)
[/quote]

Awesome, at which point we'll be able to purchase VESC's from Trampa?

[quote="trampa, post:552, topic:3813"]
VESC-Tool for MAC: That is another step to take. For the now you want to use parallels.
[/quote]

[VirtualBox](https://www.virtualbox.org/) is a free open source alternative for those that don't wish to purchase parallels. It should work just as well.

There's a few points in that paragraph that are a little off...

MacOS / OSX is the operating system that runs on Apple's desktop and laptop computers, not iPhones. There are many open source applications that are available for MacOS, Apple has no problem with you running this on your Mac.

The issues you touch on arise with the official Apple App Stores (both on Macs and iPhones), in that they impose additional restrictions on the software. These restrictions conflict with the restrictions imposed by the GPL open source license. There are several other open source licenses (MIT, Apache, etc) that do not conflict with the App Store agreement. You'll actually find a lot of open source applications in the App Store...just not usually GPL licensed applications.

Also, if Vedder holds the copyright to *all* the code, then he can license it however and to whoever (eg; Apple) he wants.
```

---
## \#554 Posted by: trampa Posted at: 2017-06-06T09:20:12.189Z Reads: 409

```
Sure, but it's GPL. I know that MAC OS is not an issue. In future the issue will be only the iOS and Apple store.
For the now Benjamin compiled the Windows and Linux versions. He can't work on everything in parallel, since we need a solution to compile the software with ease, every single week (weekly update service). So MAC is a currently not priority Nr. 1. If VirtualBOX works out that is the way forward until the MAC stuff has been taken care about.

Frank
```

---
## \#555 Posted by: dakota4e Posted at: 2017-06-07T03:40:31.299Z Reads: 407

```
http://www.getfpv.com/vortex-sbus-futaba-ppm-cable.html

Will this cable go from my flysky FS-GR3E reveicer to the VESC 6.0?

I have not yet received my instructions PDF, and am confused on how to connect my receiver to my dual VESC 6 setup.  Someone help this newb!  Love you guys!
```

---
## \#556 Posted by: Jebe Posted at: 2017-06-07T04:01:07.033Z Reads: 404

```
Check his youtube channel :thumbsup:
https://www.youtube.com/watch?v=1iwN5LGGM80&t=1039s
```

---
## \#557 Posted by: MysticalDork Posted at: 2017-06-07T05:27:20.523Z Reads: 401

```
@trampa I'm not sure what the protocol is, but I just figured I'd poke my head in here and check how the shipping of the VESCs is going. I got the vesc-tool email but no shipping confirmation yet. (I'm in USA if that helps) Sorry if this is a pointless post, I'm just getting antsy over here sitting on my hands waiting to play with the new goodies.

Hope Benjamin is doing well and not overtaxing himself - We need him up and vedder-ing again!
```

---
## \#558 Posted by: Pimousse Posted at: 2017-06-07T06:56:00.763Z Reads: 403

```
New VESC Tool is amazing ! Ben told us months and months ago that he dedicated all its free time to.
We can feel now why. Congratulations !

I run it on a virtual linux machine on my Mac flawlessly.
As Benjamin develops on Linux, and because it's totally free, I think it's worth more to do like this than a Mac version which won't benefit of latest updates because of the time-consuming it requires.

At least for the beta and the regular updates VESC Tool will surely receive. ;)

@trampa : just my 2cents for the user manual : you should add a drawing for the mounting holes, and details about mechanical installation before electrical connection chapter (such as the screw size) ;) 
And for "Connectors and switches" chapter, please add the type of connector (JST-PH I guess).

BTW, by reading the user manual, it feels like we're holding a professional state-of-the-art device. Congrats !
```

---
## \#559 Posted by: trampa Posted at: 2017-06-07T07:03:39.374Z Reads: 395

```
This is the BETA Manual. I will do some updates. THX for the input. 

JST-PH 2mm is correct. 

Frank
```

---
## \#560 Posted by: MatthiasU Posted at: 2017-06-07T08:22:00.816Z Reads: 394

```
Can we see the new schematics?

The reason I'm asking for that is that, looking at the "old" VESC, PC6/PC7 as well as PB10/PB11 seem to be connected to pins 5+6 of P3. I don't quite understand why that is and would rather have both separately so that I²C and serial both work (I²C to talk to sensors and serial for command and debug).
```

---
## \#561 Posted by: JTAG Posted at: 2017-06-07T10:28:45.693Z Reads: 397

```
Schematic is already released. Dive into the VESC world and you will find it.
```

---
## \#562 Posted by: caustin Posted at: 2017-06-07T21:11:31.925Z Reads: 414

```
Awesome, arrived today!

<img src="/uploads/db1493/original/3X/f/0/f09c3671e7c39ff6d2a1f59bfc6f75c1907af601.JPG" width="375" height="500">
```

---
## \#564 Posted by: Pimousse Posted at: 2017-06-08T07:27:08.754Z Reads: 397

```
@trampa, Thank you soooo much for the goodies, I (and surely all other betas) appreciate a lot this kind gift !

Can't wait to power my Holypro with them now ! (but have to replace 4mm by 5.5mm bullets before for connecting Overion motors) :slight_smile:
```

---
## \#565 Posted by: Maxid Posted at: 2017-06-08T08:17:32.587Z Reads: 393

```
so when can we hear the first reviews? @caustin @JTAG @sl33py
```

---
## \#566 Posted by: JTAG Posted at: 2017-06-08T09:34:37.703Z Reads: 402

```
I have to think of an application first, one that puts the ESC to the limit, it is so beefy that full power usage is almost scary xD. 

I think that I will mount it to my electric scooter, that should at least initially on acceleration draw some power.

If you have any other ideas please name them!
```

---
## \#567 Posted by: makevoid Posted at: 2017-06-08T09:55:41.685Z Reads: 393

```
I'm planning to run a single motor build (6374) with it and test it on very steep hills something that was an almost impossible task for the 4.12 without cutting off due to overheating
```

---
## \#568 Posted by: notepad Posted at: 2017-06-08T10:09:36.232Z Reads: 384

```
Im still messing around with settings.  After Vedder's torture test seeing how the he got the ERPM to such a high number,  makes me wonder what I should set mine at.
```

---
## \#569 Posted by: Brad Posted at: 2017-06-08T10:18:32.398Z Reads: 382

```
Nice shirt! Perfect size for me!

The two vesc's were a little bigger than I thought but it will fit with my planned battery size, so all great! They feel great in my hands. :ok_hand:
```

---
## \#570 Posted by: Maxid Posted at: 2017-06-08T10:30:29.117Z Reads: 374

```
Well this is the esk8 builders forum so I'd obviously like to know how they do on an esk8/eMTB.
How robust is FOC mode and can it make dual drives obsolete?
```

---
## \#571 Posted by: JTAG Posted at: 2017-06-08T11:13:01.789Z Reads: 382

```
Well my skateboard is completely finished and waterproof, I wont be taking it apart to test the VESC6. It is build so compact that it would take quite some time to do that. Next to that the VESC6 is to powerfull that at full power it will destroy the motors on my board. My electric scooter on the other hand does have a big motor, that would really put an ESC to the test.

Single drive esk8 will always be uncomfortable since the board tends to steer either left or right when braking / accelerating aggressively, putting a big motor controller on a single drive system will only magnify this discomfort. 

I think that this weekend we will build a nice test setup and maybe will even be able to document it.
```

---
## \#572 Posted by: okp Posted at: 2017-06-08T11:15:13.918Z Reads: 375

```
I will try this on my existing 12S prototype
```

---
## \#573 Posted by: makevoid Posted at: 2017-06-08T11:19:47.833Z Reads: 378

```
I agree, uneven braking is my main issue with single belt drives, but at least there's less drag than dual
```

---
## \#574 Posted by: notepad Posted at: 2017-06-08T11:21:08.314Z Reads: 378

```
At the moment im building a single belt 12S. so I can tell you how bad it is with the beefy VESC attached to it if you want?
```

---
## \#575 Posted by: JTAG Posted at: 2017-06-08T11:50:49.316Z Reads: 382

```
We are not telling its impossible. Its just less comfortable than riding a dual motor board. Once you are used to the steering action accelerating / braking introduces everything is fine (my board was single motor a couple of months). It is going from a dual motor setup to a single motor that makes you really notice the difference.
```

---
## \#576 Posted by: sebaszz Posted at: 2017-06-08T11:59:31.230Z Reads: 384

```
running 12s with 6374 single drive. runs perfect. only hard braking is difficult depending on your own weight.
```

---
## \#577 Posted by: Dwain Posted at: 2017-06-08T13:20:33.164Z Reads: 386

```
Is the Vesc 6 designed to mount onto the motor mount hex pannel on the Trampa Drivetrain system ?
Or can it be ?
```

---
## \#578 Posted by: fedestanco Posted at: 2017-06-08T13:50:21.693Z Reads: 384

```
Remember that vesc 6 is not waterproof nor dustproof yet. You want it to stay as enclosed as your batteries are.
If you are brave enough you can dip it into epoxy or do a precision job with silicone, filling the gaps of the enclosure.
```

---
## \#579 Posted by: trampa Posted at: 2017-06-08T16:37:31.980Z Reads: 378

```
Fits! 10char

Frank
```

---
## \#580 Posted by: Dwain Posted at: 2017-06-08T17:09:55.339Z Reads: 378

```
??? sorry huh , dont understand. Does it fit the hex pannel and screw holes on hex pannel ?
```

---
## \#581 Posted by: trampa Posted at: 2017-06-08T17:37:54.735Z Reads: 366

```
Yes it does, four of the six bolts screw it on.

Frank
```

---
## \#582 Posted by: sl33py Posted at: 2017-06-08T18:35:16.437Z Reads: 383

```
DANGIT!  Just saw i missed a package (stayed and "worked from home" as late as i could)...  

Hopefully i can grab it tomorrow at the post office.

I have a couple decks i might try to power with it - and an eagletree logger to measure/test with.  Just takes time which is in short supply currently.  I'll try to do something fun to show performance vs 4.12.
```

---
## \#583 Posted by: okp Posted at: 2017-06-08T18:52:52.483Z Reads: 385

```
Well, made some progress. Replaced my existing V4 with these two jewels. 12S4AH - 150C / Sensored 150kv 

http://www.e-sk8.fr/wordpress/wp-content/uploads/2017/06/IMG_9036.jpg
```

---
## \#584 Posted by: leonsc Posted at: 2017-06-08T19:22:34.208Z Reads: 377

```
Do we know when we can start buying these or when they will be in stock
```

---
## \#585 Posted by: Dwain Posted at: 2017-06-08T19:26:35.567Z Reads: 365

```
On backorder at the moment, contact Ted or Frank directly for more info.
```

---
## \#586 Posted by: trampa Posted at: 2017-06-08T20:03:42.262Z Reads: 372

```
We just ordered a new batch. I will post when you can purchase them. The next two weeks we need to focus on BETA.
Since the CNC Job took so long the last time, we will start the process ASAP. 

Frank
```

---
## \#587 Posted by: nmagz3 Posted at: 2017-06-08T20:07:25.544Z Reads: 374

```
Those look so bad ass!  I also saw a picture of these on Instagram.  Can't wait to hear regarding the results.
```

---
## \#588 Posted by: chuttney1 Posted at: 2017-06-09T00:21:18.435Z Reads: 374

```
At this point. Someone should just make a go-kart and haul a truck. Haveing to wait another few more week before the release of the ESC files is annoying.
```

---
## \#589 Posted by: trampa Posted at: 2017-06-09T09:28:51.109Z Reads: 385

```
The new VESC-TOOl is now compiled and ready for download. Version 0.78 
BETAS please download the latest VESC-Tool!

You can now upload the missing Bootloader via USB and VESC-Tool.
After installing the Bootloader, you can upload the Firmware 3.25. 

Benjamin nailed that last night. Big congrats for making this happen - magic!

<img src="/uploads/db1493/original/3X/7/d/7d1e5b5ce7c1722e1904caacbdaaa56a8390e467.jpg" width="690" height="371">

Frank
```

---
## \#590 Posted by: Pimousse Posted at: 2017-06-09T09:43:25.831Z Reads: 371

```
Being able to update the bootloader through USB is amazing !
Benjamin's talent won't stop to impress me.

Thank you both for sorting this bug out so quickly !
```

---
## \#591 Posted by: trampa Posted at: 2017-06-09T12:47:20.957Z Reads: 381

```
This is very nice, because now VESC-Tool can ad a missing bootloader to HW 4.xx VESCs via USB as well. 
The bootloaders for all HW 4 VESCs is now included. Tank Benjamin for that!
So if you have a China VESC without bootloader, you are sorted now. Straight update to FW 3.25, once the VESC 4 FW support is added in. Not good for the people selling St-Link/V2 (-;

Frank
```

---
## \#592 Posted by: Maxid Posted at: 2017-06-09T13:34:14.224Z Reads: 380

```
I want it so bad.

Did I miss it or is there some explanation of what the benefits for the V4 VESCs will be?
I mean functionality wise it always seemed perfectly fine and only hardware deficiencies caused errors in say FOC for example (at least that was my impression). Does the new firmware improve the V4?
```

---
## \#593 Posted by: trampa Posted at: 2017-06-09T13:43:57.133Z Reads: 398

```
It does improve stuff a lot. As soon as VESC-Tool is public you want to sack off BLDC-Tool ASAP!
We do not recommend to use BLDC any more for safety reasons. 

Frank
```

---
## \#594 Posted by: Maxid Posted at: 2017-06-09T14:01:22.266Z Reads: 399

```
will there be some sort of changelog so that we can actually see what changed for V4?
No doubt VESC-Tool is better than BLDC-Tool but what does that have to do with the actual firmware on the VESC?

And when you say you do "not recommend to use BLDC any more" does that mean BLDC mode or just the tool?
I am confused...
```

---
## \#595 Posted by: caustin Posted at: 2017-06-09T14:54:51.076Z Reads: 388

```
having trouble uploading bootloader via USB and VESC -Tool, what are the exact steps as missing something and need to do that before uploading new firmware 3.25
```

---
## \#596 Posted by: caustin Posted at: 2017-06-09T15:01:02.517Z Reads: 379

```
connected serial via com port but in limited mode until get bootloader sorted out, how am I supposed to get bootloader and then upload it?
```

---
## \#597 Posted by: Pimousse Posted at: 2017-06-09T15:01:10.516Z Reads: 373

```
Look at the forum on vesc-project.com
Ben wrote the procedure for it. ;)
```

---
## \#598 Posted by: caustin Posted at: 2017-06-09T15:03:36.000Z Reads: 365

```
awesome, doing this on phone in transit so looking quick lol
```

---
## \#599 Posted by: caustin Posted at: 2017-06-09T15:08:15.356Z Reads: 370

```
ok great, that works, actually thought I already tried that but mush not have highlighted the file in bootloader tab...duh!  lol
```

---
## \#600 Posted by: Randyc1 Posted at: 2017-06-09T15:15:09.911Z Reads: 369

```
Will this new Vesc Tool be good for all the Older Vesc's as well ?
```

---
## \#601 Posted by: sl33py Posted at: 2017-06-09T15:17:13.935Z Reads: 383

```
[quote="Randyc1, post:600, topic:3813, full:true"]
Will this new Vesc Tool be good for all the Older Vesc's as well?
[/quote]

When they add the firmware for v4 it should work for both older v4.xx and new v6!  They've said it's about a week out to add v4.xx FW's (realistically likely a couple weeks - busy folks!).

Or is your question will it work with older 4.6/4.7 VESC?
```

---
## \#602 Posted by: trampa Posted at: 2017-06-09T15:53:43.645Z Reads: 380

```
The Vesc-Tool with FW 4.xx support will be out for BETAS next week. Its pretty much  finished but the website needs updating, so you can access it. Its all linked together now - VESC-Tool and the Website and the VESC-Server. It's an Environment, not a stand alone Software. After BETA the VESC-Environment will go public anyway and everyone wants to switch over to VESC-Tool and forget about BLDC-Tool. 
BLDC-Tool will not get any attention in future. No more updates in case of bugs, which makes BLDC-Tool 100% obsolete.
Since we know that the old Firmware is by far not as perfect as the new one, we do not recommend to use it any more. It's safer to use the latest FW coming with VESC-Tool. 
For those requesting a change log: It's probably easier to pubish a short list of thing that have not changed (-;

Frank
```

---
## \#603 Posted by: whitepony Posted at: 2017-06-09T17:02:10.051Z Reads: 377

```
[quote="JTAG, post:571, topic:3813"]
Single drive esk8 will always be uncomfortable since the board tends to steer either left or right when braking / accelerating aggressively, putting a big motor controller on a single drive system will only magnify this discomfort.
[/quote]

try ronins, none of that happens with the support pin!
```

---
## \#604 Posted by: solidgeek Posted at: 2017-06-09T17:05:16.206Z Reads: 374

```
I just received my VESC 6 and it looks amazing :slight_smile: ! Where can I download the PDF-manuel (haven't received it on mail)?
```

---
## \#605 Posted by: trampa Posted at: 2017-06-09T17:35:30.830Z Reads: 376

```
I send out a mail and will drop it on The vesc-project and Trampa site.

Frank
```

---
## \#606 Posted by: Maxid Posted at: 2017-06-09T17:50:16.099Z Reads: 382

```
Oh and what I also wanted to ask: was there any progress by Ben to also support other Nunchuck brands besides the Nyko Kama? I can't seem to find any affordable ones anymore - especially in Europe. 
Or is there a new preferred way of controlling the VESC6?
```

---
## \#607 Posted by: notepad Posted at: 2017-06-09T18:13:55.666Z Reads: 403

```
Not sure if its the correct place to ask but it is about the VESC so,  ehh worth a shot.

A),  where the hell do I put this.<img src="/uploads/db1493/original/3X/5/c/5cb599ead5c86463e1f4c5546121db3515bd5aa9.JPG" width="666" height="500">

I can see that the 3pin on the right has a space on the VESC, but if I put it the wrong way round would it bugger it up?  and where does the thing on the left go?


B) For settings.<img src="/uploads/db1493/original/3X/3/6/367fdb55e1940ec272f5bc71e690343a32919f87.png" width="690" height="453">
Which one should I choose as I have no experience as of yet. (sorry if this is the wrong place to ask as its mostly build questions )
```

---
## \#608 Posted by: Hummie Posted at: 2017-06-09T18:21:51.692Z Reads: 391

```
i never noticed torque steering or braking with single motor with paris v2 or caliber either.  I don't think it happens really 


how reliable is the nunchuck now that the 6 has a built in receiver for it?  that's true right?  any nyko nunchuck?
```

---
## \#609 Posted by: sl33py Posted at: 2017-06-09T19:32:12.310Z Reads: 402

```
Woohoo!  At work so haven't been able to connect them yet... but hopefully this weekend i'll get them configured and at least one temporarily mounted to test and compare!

[img]https://goo.gl/1c449w[/img]
[img]https://goo.gl/aGkjPU[/img]
[img]https://goo.gl/8eKahj[/img]

@Hummie - it sounds like nunchuck via the "onboard NRF" is only select devices in EU.  I was told that in the US and possibly other locations they weren't able to include it!  bummer...  

In the US there's a bunch of FCC certifications and testing required (quite expensive and repetitively expensive w/ any versioning).  GT2b still it seems...
```

---
## \#610 Posted by: trampa Posted at: 2017-06-09T19:32:15.353Z Reads: 388

```
Mind control is the future! Not kidding! 

Frank
```

---
## \#611 Posted by: Maxid Posted at: 2017-06-09T19:46:11.389Z Reads: 387

```
:astonished: Say whaaat!
```

---
## \#612 Posted by: whitepony Posted at: 2017-06-09T20:11:13.593Z Reads: 397

```
[quote="Hummie, post:608, topic:3813"]
i never noticed torque steering or braking with single motor with paris v2 or caliber either.  I don't think it happens really
[/quote]


its quite strong on calibers and paris unless you use really stiff bushings. its unbearable on evolve kind of sidewinder trucks. it simply does not happen on ronins due to the support pin - one among many reasons to love them for eboarding. :slight_smile:
```

---
## \#613 Posted by: Pimousse Posted at: 2017-06-09T20:12:54.122Z Reads: 408

```
@notepad : you have to build your own adapter
<img src="/uploads/db1493/original/3X/1/7/17219ff1ea0d5b20fc0286b0af09625ed70c773b.jpg" width="666" height="500">

 <img src="/uploads/db1493/original/3X/3/b/3bcc21a77cd0cc5fa45e28f37dd93c0626382511.jpg" width="666" height="500">
```

---
## \#614 Posted by: notepad Posted at: 2017-06-09T20:17:36.585Z Reads: 387

```
That looks fantastic.  is the white connector called molex?
```

---
## \#615 Posted by: trampa Posted at: 2017-06-09T20:20:24.915Z Reads: 394

```
You think it, it happens. Magic....
No cables, hand held devices, no transceivers.

Not Kidding, just had the pleasure to test a prototype. 

VESC SIX is just the start of things beyond your mind. 

Frank
```

---
## \#616 Posted by: trampa Posted at: 2017-06-09T20:21:41.704Z Reads: 393

```
JST-PH, 2mm pitch, three pins.
```

---
## \#617 Posted by: sebaszz Posted at: 2017-06-09T20:31:17.252Z Reads: 397

```
just finished my first test drive, works great! wow what a piece of technology

I have a 12s single drive 6374 192kv + i'm 100kg  and with the old vesc even with extra cooling it started to overheat within 5 min. Now with the new vesc not a single issue.

I tried both BLDC and FOC but i still prefer the more agressive sound(feeling) of BLDC. 

To me the JST connector is unnecessary complicated. A lot of people now cannot start because they don't have connector like that at home for the receiver. If you make that discussion also supply the connector to my opinion.

Downloading the upgraded vesc-tool 0.78 was a bit unclear to me. I needed this because mine also missed the bootloader. At the end I re-ordered the tool and used the new download link.

Downloading the manual also unclear. I think not possible at the moment.

But hey we are still in BETA stage :) 

For the rest. Very well done
```

---
## \#618 Posted by: notepad Posted at: 2017-06-09T20:32:51.904Z Reads: 371

```
Thanks Frank,  Time to go order some connectors :stuck_out_tongue:
```

---
## \#619 Posted by: trampa Posted at: 2017-06-09T20:41:47.687Z Reads: 378

```
Hope you got my reply on the www.vesc-project.com  BETA Forum.
I could not resist to drop in the geographical location of the secret headquarter.

Frank
```

---
## \#620 Posted by: notepad Posted at: 2017-06-09T20:43:13.203Z Reads: 380

```
I saw it and have a nice little giggle to myself :D
```

---
## \#621 Posted by: Hummie Posted at: 2017-06-09T20:53:10.146Z Reads: 378

```
how does mind control work?
```

---
## \#622 Posted by: Dwain Posted at: 2017-06-09T20:55:20.521Z Reads: 368

```
Does anyone know if the winning remote has NRF and if it will work with the vesc's sent out with NRF and no additional reciever ?
```

---
## \#623 Posted by: trampa Posted at: 2017-06-09T20:57:49.028Z Reads: 370

```
Top Secret! But with some more funding of the VESC-Project stuff like that is closer than you think.
I hope that VESC-Tool will result in a better project support and more things will happen faster.

Frank
```

---
## \#624 Posted by: Pimousse Posted at: 2017-06-09T21:05:55.277Z Reads: 368

```
Just updated bootloader and 3.25 FW.
Everything went flawlessly on both VESC 6 :slight_smile:
```

---
## \#625 Posted by: sl33py Posted at: 2017-06-09T22:11:00.638Z Reads: 384

```
[quote="sebaszz, post:617, topic:3813"]
To me the JST connector is unnecessary complicated. A lot of people now cannot start because they don't have connector like that at home for the receiver. If you make that discussion also supply the connector to my opinion.
[/quote]


Agreed.  I don't have any adapters provided with these.  I *might* have a 3pin JST at home, but if not this adds delay before i can test...  For the price - they should've been included.  Beta or not.
```

---
## \#626 Posted by: Dwain Posted at: 2017-06-09T22:17:24.173Z Reads: 381

```
I know its frustrating guys i will have the same problem when my 2 arrive on monday, but i think Frank and Ted are super swamped with everything they have to do .So much has happened so fast, imagine how much they have to deal with . Anyone know if the winning remote will work with the NRF reciever on the vesc 6 ?
```

---
## \#627 Posted by: notepad Posted at: 2017-06-09T22:20:54.016Z Reads: 372

```
I feel you,  I now have to wait 20 days for amazon to deliver :frowning:
```

---
## \#628 Posted by: Dwain Posted at: 2017-06-09T22:23:35.803Z Reads: 369

```
No R.C hobbie shops anywhere near you surely they would have ? I was hoping i could get mine from one nearby me.
```

---
## \#629 Posted by: notepad Posted at: 2017-06-09T22:32:33.725Z Reads: 363

```
unfortunatly lincoln uk is a bit sparse
```

---
## \#630 Posted by: Dwain Posted at: 2017-06-09T22:34:15.387Z Reads: 376

```
Might have same problem bro so prob just going to order one now just in case.
```

---
## \#631 Posted by: bigben Posted at: 2017-06-09T22:40:36.697Z Reads: 379

```
RS components sell them next day.
```

---
## \#632 Posted by: oyta Posted at: 2017-06-09T22:46:51.312Z Reads: 407

```
<img src="/uploads/db1493/original/3X/8/8/8880f70552134e6c2b337e4108d26cea0f1be947.JPG" width="375" height="500"><img src="/uploads/db1493/original/3X/f/d/fd636ef5389b8d68e43d4bb77dc64173be2016e6.JPG" width="375" height="500">

The bullet connectors from the motor does not fit :frowning: I thought it was 4.5mm bullet connectors, but measuring the inside diameter I get about 2 mm. Am I correct that the VESC 6 uses 2 mm connectors? I need to order some - rather get it right the first time :slight_smile:

Would these connectors fit? https://www.rc-shop.no/products/am-1002-b-20mm-gullkontakter-2par-2male-2female

I guess I am better of changing the ones one the motor rather then the VESC.

**EDIT: I was too tired and didn't notice that my tool was way off! I remeasured it to 4mm and that is according to the information on Trampas website.** :) :)
```

---
## \#633 Posted by: Maxid Posted at: 2017-06-09T23:00:19.913Z Reads: 387

```
the vesc should have 4mm female bullets so you need 3.5 male ones
```

---
## \#634 Posted by: chaka Posted at: 2017-06-09T23:18:24.136Z Reads: 403

```
> Agreed. I don't have any adapters provided with these. I might have a 3pin JST at home, but if not this adds delay before i can test... For the price - they should've been included. Beta or not.

I like the lower profile of the jst-ph connectors but I will admit they are a difficult combination to find. We made a small batch if anyone needs them. Here is our listing.
[http://www.ollinboardcompany.com/product/vesc6-ppm-connector](http://www.ollinboardcompany.com/product/vesc6-ppm-connector)
```

---
## \#635 Posted by: trampa Posted at: 2017-06-09T23:27:37.600Z Reads: 401

```
I thought you guys are DIY. Just strip off the plastic from the dam PPM plug, shrink tube the metal clips and plug in. Secure the cable/connection with some Gaffa -Tape, so that the connectors will not move or vibrate out. Order a JST-PH and get the connection sorted as soon as the parcel arrives. 

Update:
As Hexacopter stated quite right, this method is for testing and adjusting the RC-Controller and playing around a bit, not for riding your board. The JST-PHR connectors can be found at RS-Components, Farnell, Mouser and online auction houses. @hexakopter s criticism is quite right! 

Frank
```

---
## \#636 Posted by: chaka Posted at: 2017-06-09T23:28:46.807Z Reads: 392

```
We only ride like savages, we take  pride in what we build ;)
```

---
## \#637 Posted by: Dwain Posted at: 2017-06-09T23:33:28.225Z Reads: 383

```
Frank can u tell me if the winning remote will work with the vesc 6 and the built in NRF reciever it has ? Or will i still have to use an additional reciever ?
```

---
## \#639 Posted by: chaka Posted at: 2017-06-09T23:35:55.152Z Reads: 386

```
If it was me and I didn't have the connectors I would remove the jst-ph and solder directly to the pcb to keep it "clean".
```

---
## \#640 Posted by: trampa Posted at: 2017-06-09T23:38:03.176Z Reads: 393

```
No it will not work. That device is standard 2.4Ghz equipment. To use the NRF, you want a pimped Nunchuck with replacement NRF-PCB.

Frank
```

---
## \#641 Posted by: Dwain Posted at: 2017-06-09T23:40:23.759Z Reads: 378

```
Ok thanks. Any links on where i can get a nice one from ?
```

---
## \#642 Posted by: Hummie Posted at: 2017-06-09T23:53:26.042Z Reads: 377

```
you shrink tube with tiny shrink tubing the 3 bare wires to ..are they pins or fins or what?    And then use tape to hold it you say.  I'm just curious what people do.  why not solder?

i used j and b weld once and shorted.
```

---
## \#643 Posted by: notepad Posted at: 2017-06-10T00:36:42.614Z Reads: 373

```
risk of shorting out our loverly new VESC.  but now you mention it.  soldering the wires into place is getting more and more tempting as I really want to finish my first build :slight_smile:
```

---
## \#644 Posted by: sl33py Posted at: 2017-06-10T06:48:11.456Z Reads: 377

```
[quote="trampa, post:635, topic:3813"]
I thought you guys are DIY. Just strip off the plastic from the dam PPM plug, shrink tube the metal clips and plug in. Secure the cable/connection with some Gaffa -Tape,
[/quote]

Hey Frank - you know I speak my mind.  Yeah i'm DIY, and that's exactly what I will do... cables are already ordered.  Won't slow me down too much, but where i'd normally solder it i'm actually being gentle with this gorgeous case/pcb - trying not to hack it up just yet.

BUT you are missing the point - this is a *premium* ESC and it's missing somewhat specialty connectors to use it.  That's a miss on Trampa's part IMO.  A <$100 4.12 VESC from another seller came with a short servo cable
```

---
## \#645 Posted by: hexakopter Posted at: 2017-06-10T07:08:58.110Z Reads: 390

```
[quote="trampa, post:635, topic:3813"]
I thought you guys are DIY. Just strip off the plastic from the dam PPM plug, shrink tube the metal clips and plug in. Secure the cable/connection with some Gaffa -Tape, so that the connectors will not move or vibrate out. Order a JST-PH and get the connection sorted as soon as the parcel arrives.
[/quote]

Please don't do that. The crimp contact from the 2.54mm plug doesn't fit the lot smaller pinheader from the JST PH 2.0mm socket.
I often used this method for connecting individual pins from the 2.54mm plug to the 2.54mm pinheader and that works, but with the JST PH it will not work and don't makes a proper connection. 

Btw I also thought the people here (in the BETA batch) are more DIY and they know the fact that the PPM header on the VESC 6 has a JST PH 2.0mm socket installed for over half a year so ordering one could have happen a lot earlier, but putting some JST PH connectors with one side of the wire unsoldered to our packages would have been still a good and useful idea.
```

---
## \#646 Posted by: hexakopter Posted at: 2017-06-10T07:10:56.113Z Reads: 403

```
[quote="sl33py, post:644, topic:3813"]
Yeah i'm DIY, and that's exactly what I will do...
[/quote]


Please don't even consider doing it. Its stupid and you don't get a reliable connection.

@Maxid
[quote="Maxid, post:633, topic:3813, full:true"]
the vesc should have 4mm female bullets so you need 3.5 male ones
[/quote]
Nope. For 4mm female bullets also use 4mm male ones. You can see it in the picture [here](https://oscarliang.com/choosing-gold-bullet-connectors-motor-esc/) that there is a big difference between 3.5mm and 4mm bullets.
```

---
## \#647 Posted by: Maxid Posted at: 2017-06-10T07:32:03.065Z Reads: 400

```
It is what trampa says:
<img src="/uploads/db1493/original/3X/3/1/31678ac35127d31b9a303363bb753bc32722203c.jpg" width="281" height="500">

The left says 4mm bullets that fit 3.5male
```

---
## \#648 Posted by: sebaszz Posted at: 2017-06-10T07:34:26.919Z Reads: 392

```
Anyone else already tried the Vesc?

The connector for me is a minor thing. 
The focus should be on the incredible performance and possibilties of this new vesc.
Ben did a incredible job with the assistance Frank, thank you both for offering a major improvement to the DIY community.
```

---
## \#649 Posted by: hexakopter Posted at: 2017-06-10T07:35:35.057Z Reads: 387

```
They also told you "Just strip off the plastic from the dam PPM plug, shrink tube the metal clips and plug in. Secure the cable/connection with some Gaffa -Tape, so that the connectors will not move or vibrate out."
But just don't do it.

@sebaszz Haven't received mine yet, because trampa thought it would be a good idea to repack the german VESCs by Frank and then send it out again. Will tell my experiences when I received it.
```

---
## \#650 Posted by: oyta Posted at: 2017-06-10T07:50:47.527Z Reads: 389

```
I tested with 4mm and it seems to fit. According to the Trampa website it is 4mm connectors and 3.5mm should fit as well. My bad about the photo I posted last night - it was too late (I was too tired) and I didn't notice that my measurement tool was totally off! :sweat: The tool should have said 4 mm diameter as said on the Trampa website :slight_smile:

I can not wait to test the VESC - it really looks good! :smiley: Nice work @trampa and BV!
```

---
## \#651 Posted by: hexakopter Posted at: 2017-06-10T08:21:33.168Z Reads: 392

```
[quote="oyta, post:650, topic:3813"]
According to the Trampa website it is 4mm connectors and 3.5mm should fit as well.
[/quote]


Yes it maybe will not fall out that easy, but you can push the most current through a connector when it is using the most connection area available. So maybe it works for low current applications, but I would not trust using the wrong diameter in a serious build that is pushing a lot of amps.
```

---
## \#652 Posted by: oyta Posted at: 2017-06-10T08:46:06.138Z Reads: 383

```
I agree. I'll use the 4mm connectors :slight_smile:
```

---
## \#653 Posted by: Jebe Posted at: 2017-06-10T09:05:56.184Z Reads: 384

```
go cart 10 chars
```

---
## \#654 Posted by: trampa Posted at: 2017-06-10T09:38:13.557Z Reads: 392

```
4mm male is the one.

Frank
```

---
## \#655 Posted by: trampa Posted at: 2017-06-10T10:42:53.228Z Reads: 402

```
Cables and connectors: 
We will soon offer all sorts of cables and connectors, so that you CAN have your Board up running without soldering.

A JST-Ph to PPM is on the list.

SAFETY: IF YOU BUILD A NEW BOARD AND RIDE IT FOR THE FIRST TIME, SET A SAFE RPM/SPEED LIMIT AND DROP YOUR MOTOR MIN/BATTERY MIN TO A VALUE THAT THE BOARD WILL NOT BRAKE HEAVILY. SET YOUR MOTOR MAX TO VALUES ONLY ALLOWING GENTILE ACCELERATION. TEST YOUR BOARD FOR A WHILE, SO YOU KNOW EVERYTHING IS STABLE AND WORKS RELIABLE. THEN YOU START TO INCREASE THE VALUES AND TEST AGAIN. THIS WAY A POOR CONNECTION WILL NOT CAUSE MAJOR TROUBLE OR ACCIDENTS. RIDE YOUR BOARD SOMEWHERE WHERE NO ONE IS PUT TO DANGER IN CASE OF A FAILURE.

FRANK
```

---
## \#656 Posted by: makevoid Posted at: 2017-06-10T12:54:30.897Z Reads: 396

```
I had only 6 pins JST, I cut one in half with a cutter and there you have a 3 pin jst that fits very well. 
Also to be safe against connectors unplugging while you're going downhill you can configure the VESC to brake after a second or so after the connection with the remote is lost. you can also chose the braking amount - now this setting in the vesc tool is in the App Setting (General) section: Timeout and Timeout Brake Current.

I have tried the 6 with a single motor 6374 in FOC with conservative settings (60A motor max) and it's amazing, with my ~105kg I can climb very steep hills no problem (0.5km - Avg Grade 6% for example), I changed with 90A motor max as with 60A the motor still runs cool, and will try it soon with that too

I'm wating for a way to log data from the new Vesc to be available as there have been (small?) changes in the protocol, I would like to get the max temp reached and the power drawn to check the efficiency. Overall I'm impressed with it and I don't think I will ever need to add extra cooling to it (like exposing the metal part outside of the enclosure).

Link to some data / pics: https://gist.github.com/makevoid/36da9aa49a575c4bab9bd83adae5a590

edit: note the build is 8S even if I plan to change it to a 10S probably to increase max speed + efficiency
```

---
## \#659 Posted by: Hummie Posted at: 2017-06-10T18:28:39.311Z Reads: 382

```
xt90s.  
although I'm still waiting to hear how a connection with nothing but a bit of vaseline or anti-electric paste would do.  stops the arc through the air and then slide the two conductors together.
```

---
## \#660 Posted by: trampa Posted at: 2017-06-10T18:34:21.026Z Reads: 401

```
Now it's possible to scale up, other components need to be beefed up as well.
A good setup should still limit the amp flow as much as possible. Voltage up, amps low is still the best way to go.

I don't think there is an of the shelf solution available yet. Have you thought about a parallel array?

Frank
```

---
## \#661 Posted by: Dwain Posted at: 2017-06-10T18:41:50.208Z Reads: 410

```
There is this guys i am thinking of buying 2 as i have a dual drive trampa with 2 batteries one for each vesc so i would need 2. Only problem is they say hole diameter is 12mm and i have 16mm hole already drilled, so going to make a plan of some sort . What you think ?

<img src="/uploads/db1493/original/3X/3/a/3ac0a66dd7c2c24e0776d3c0ebd2d1aca892f185.jpg" width="690" height="388">
```

---
## \#662 Posted by: makevoid Posted at: 2017-06-10T21:25:21.837Z Reads: 402

```
The vedder anti spark switch can go more than 40A you just need to change the fuse, I changed to a 50A fuse and it holds 50A w/o problem, the mosfets should be rated for much more (240A?) but probably there are no small fuses (ATO/regular fuse) over 50A  that can fit that holder. There are posts on the forum of people soldering a bigger fuse or two in parallel even if the cleanest solution is probably to change the holder to put a bigger fuse (size: maxi) that can go up to 120A.
```

---
## \#663 Posted by: notepad Posted at: 2017-06-10T23:36:09.320Z Reads: 396

```
Cant say I have. honestly I only started dabbling in electronics thanks to this first build I am making ( now I cant stop upgrading stuff :P )

@makevoid   Thats good to know as if I did want to up the Amps, Atleast I know there is a way without worrying about the mosfets blowing.
```

---
## \#664 Posted by: Jebe Posted at: 2017-06-11T11:28:41.158Z Reads: 382

```
Seriously?  You don't need 2. Split the power to the vesc after the switch.
```

---
## \#665 Posted by: jazzcool Posted at: 2017-06-11T11:49:23.826Z Reads: 390

```
this looks fantastic and I wish I could have waited for this project (just bought first build, a pair of VESC 4.12). 
One thing about the design and how would you be mounting those: if the metal heatsink should be on top it means all the connectors are sitting on the bottom plate. If you would simply place the VESC on the top side of the board, won't the connections obstruct the clearance?
```

---
## \#666 Posted by: Dwain Posted at: 2017-06-11T19:14:48.115Z Reads: 392

```
 I want to run vescs and motors to their maximum and if i only get one  that will limit me to 60 Amp per motor as it is rated for 120 amp. With 2 i can have settings upto 120 Amp if the vesc and motors can handle it , i dont want my power switch to be the bottle-neck in my system. Correct ?
```

---
## \#667 Posted by: makevoid Posted at: 2017-06-11T22:04:15.545Z Reads: 408

```
I logged my ride with my vesc 6 based single motor build ([single motor 6374 190kv 8S FOC](https://gist.github.com/makevoid/36da9aa49a575c4bab9bd83adae5a590)) and that's the result:

https://metr.at/r/JOfun

I tried to do a full-throttle test uphill and it's awesome, nothing compared to the 4.12 which without cooling (heatsink) had problems not overheating 
 https://metr.at/r/JOfun?zoom_start=3209&zoom_end=3467

Then right after it I was able to reach full speed no prob. (40km/h, it's an 8s) 
 https://metr.at/r/JOfun?zoom_start=3475&zoom_end=3660

I also did a braking test and I was able to brake at min current (-60A motor) for more than 30 seconds: https://metr.at/r/JOfun?zoom_start=5276&zoom_end=5459

note you need a beta version of the app, don't try it with the current one (see post on vesc-project)

edit2: links fixed
```

---
## \#668 Posted by: Ackmaniac Posted at: 2017-06-11T22:10:26.765Z Reads: 391

```
Did anybody try the VESC 6 with my app? Does it work?
```

---
## \#669 Posted by: Randyc1 Posted at: 2017-06-12T00:10:49.864Z Reads: 392

```
Ackmaniac,.. is your appt useful with single motor boards ?, ..i can understand wanting to tame a double motor's torque but what advantages do you get with a single ?
```

---
## \#670 Posted by: Maxid Posted at: 2017-06-12T02:09:43.529Z Reads: 387

```
He's talking about the app not the firmware. Why shouldn't the app be useful in a single motor build?
```

---
## \#671 Posted by: Maxid Posted at: 2017-06-12T02:11:41.570Z Reads: 386

```
What type of battery do you have that can withstand 60A charge current?
```

---
## \#672 Posted by: MysticalDork Posted at: 2017-06-12T03:31:06.675Z Reads: 394

```
I think he means the circulating current in the motor/VESC output stage. You can configure motor regen and battery regen separately.
```

---
## \#673 Posted by: makevoid Posted at: 2017-06-12T08:17:28.924Z Reads: 391

```
Yes, edited
```

---
## \#674 Posted by: Pimousse Posted at: 2017-06-12T14:28:31.161Z Reads: 397

```
Someone tested the VESC 6 with metr.app and brick his VESC 4 because communication has changed a bit.
He recovered the VESC with a STLink. Now they have fixed the issue with a bit a reverse engineering.

So sorry, but testing your app with VESC 6 before BV release the protocol seems to be a bit risky. ;)
```

---
## \#675 Posted by: makevoid Posted at: 2017-06-13T00:43:24.515Z Reads: 398

```
links are now fixed if anyone is interested - acceleration full throttle uphill (note elevation - green) https://metr.at/r/JOfun?zoom_start=3209&zoom_end=3467 - full throttle on flat - https://metr.at/r/JOfun?zoom_start=3475&zoom_end=3660 -  braking low speed on steep downh (30s): https://metr.at/r/JOfun?zoom_start=5276&zoom_end=5459
```

---
## \#676 Posted by: abenny Posted at: 2017-06-13T00:59:23.601Z Reads: 389

```
use a washer :grinning:
```

---
## \#677 Posted by: Hummie Posted at: 2017-06-13T02:38:56.586Z Reads: 392

```
That's a great link with its scan through time on the phone.  
You hit 90 percent duty cycle

I'm looking at ur negative amps. Assuming the battery can take it what current can you go for and how do you get it?  What bat and motor regen numbers are good
```

---
## \#679 Posted by: notepad Posted at: 2017-06-13T14:48:58.617Z Reads: 403

```
Forgive me for I have sinned. <img src="/uploads/db1493/original/3X/0/2/02af031531670124a7007e32fe1ef32cf6566d89.jpg" width="375" height="500">   
( It has been filed down to fit,  cant be bothered to wait 20 days for the right connector :P )

@trampa You asked for DIY,  well here is some bodge instead.
```

---
## \#680 Posted by: trampa Posted at: 2017-06-13T15:28:49.712Z Reads: 393

```
Just make sure to adjust the VESC-Settings to be safe. (PPM- Timeout settings, brake, top speed).
You don't want your board to brake hard, nor have a top speed you can't handle in case of a failure, nor brakes that would lock in, throwing you off.

Frank
```

---
## \#681 Posted by: notepad Posted at: 2017-06-13T15:31:44.255Z Reads: 393

```
Any setting you would reccomend for a first time rider (of an eboard)

Im still pretty new to the tool so I get kinda lost.
```

---
## \#682 Posted by: trampa Posted at: 2017-06-13T15:44:58.802Z Reads: 394

```
Basically I adjust my board to be ridable for my 6 year old son. He rides with 8-9A Motor, 8A Regeneration, 15.000 ERPM (depends on gearing you use, I use 14/33 with 83mm wheels). 
When I try my boards first time, I go for 20A Motor, -10A Regen. I use the same settings for the Motor and Battery.
You can set a Brake, when you loose the connection between your Input device and the VESC. This should be a soft setting, not throwing you off, but rather slowing your board down gently.
To configure what your board does in case of a signal loss,
go to App Settings >General > Timeout and Timeout Brake Current.

You can try out the "fail safe" by switching off your Radio, or pulling the ppm connector out while riding (sitting on your board at low speed).

Once you are comfortable with your setting, you can increase your Amp draw and Brake.

Frank
```

---
## \#683 Posted by: notepad Posted at: 2017-06-13T16:02:48.836Z Reads: 370

```
Cheers frank,  Ill try that,  Dont want to break a bone before I even get to do a first proper ride.
```

---
## \#684 Posted by: hexakopter Posted at: 2017-06-13T16:33:15.775Z Reads: 367

```
I would not recommend driving like this, but I already told you that the crimp contact of the 2.54mm is different then on the jst ph 2.0mm and will not hold properly. So you can't say no one warned you before.
```

---
## \#685 Posted by: notepad Posted at: 2017-06-13T16:35:02.884Z Reads: 370

```
its mostly because I wanted to see if everything worked correctly and that the JST connectors seem to be coming on snail mail from china in 20 days :(
```

---
## \#686 Posted by: hexakopter Posted at: 2017-06-13T16:37:25.749Z Reads: 378

```
This someone was me and if @Ackmaniac hasn't changed the communication protocol of his app then it can't work for sure.
```

---
## \#687 Posted by: sl33py Posted at: 2017-06-13T17:07:22.372Z Reads: 387

```
I found some on Amazon Prime.  20 sets = 40 connectors!  So have a "few" extra for anyone who wants to PM me in the US i'll drop a stamp and send your way.  Share the love a bit.  Or grab a set for the $8 and share w/ your friends...  

https://www.amazon.com/gp/product/B01KLQL4IO

My international brethren - i'd look at Amazon for your area if reasonable/fast.  Otherwise ebay/aliexpress/etc. - not as quick i'm sure but dirt cheap.  I know we are more than a bit spoiled in the US w/ fast shipping on these.
```

---
## \#688 Posted by: trampa Posted at: 2017-06-13T20:04:53.277Z Reads: 383

```
To set up your board and play around with settings that's fine. If you want to boost your settings and go for a proper ride, please use the Jst-connector for safety.

Frank
```

---
## \#689 Posted by: Pedrodemio Posted at: 2017-06-13T22:06:13.347Z Reads: 383

```
@trampa whats the dimensions with the aluminum case? i remember seeing them a while back but couldn't find, i will start to 3D print my enclosure but need to know if it will fit

and the mounting holes are all 4mm?

Thanks
```

---
## \#691 Posted by: jaykup Posted at: 2017-06-14T13:28:14.863Z Reads: 380

```
Agreed - they are currently priced too high.  The first batch betas got a steep discount, so that's how I got it for $185.  Give it a year or so for the price to come down.  Right now a $99 VESC 4 will probably work fine.  I've got 500 miles on mine.  If you run 12s on a VESC 4 just don't run FOC.
```

---
## \#693 Posted by: DSnell Posted at: 2017-06-14T19:35:55.935Z Reads: 377

```
im using a VESC 4.12 for my ONDA CORE conversion at the moment.
its working really well. I plan on getting another one soon to make it a dual Setup like you were saying.

Here is a link to the EBay Seller i am in contact with.
[VESC 4.12](http://www.ebay.co.uk/itm/VESC-4-12-Brushless-Motor-Speed-Controller-eBike-eSkateboard-eScooter/122542291035?_trksid=p2047675.c100012.m1985&_trkparms=aid%3D777003%26algo%3DDISCL.MBE%26ao%3D2%26asc%3D43782%26meid%3D0b13a90586fd4bda8356cfa3d00248fa%26pid%3D100012%26rk%3D1%26rkt%3D12%26sd%3D122448085029)
```

---
## \#694 Posted by: solidgeek Posted at: 2017-06-15T14:31:45.997Z Reads: 377

```
@trampa do you have any information on how to use the built-in NRF module? I have tried the automatic pairing function, but the VESC can't seem to connect to my custom NRF remote. How do I prepare my custom NRF-remote for the VESC 6 automatic pairing? :slight_smile:
```

---
## \#695 Posted by: trampa Posted at: 2017-06-15T14:39:33.746Z Reads: 386

```
https://github.com/vedderb/nunchuk_mod

Cheers, Frank
```

---
## \#696 Posted by: solidgeek Posted at: 2017-06-15T15:09:24.746Z Reads: 388

```
Hi Frank,

Im not sure if I don't see it, but what you just linked is not documentation, but the source code for vedders nunchuk mod (thousands of lines). I am only a novice developer and C is not my main language - I can't even understand half of the code as there are no code comments... 

A simple example of how to utilize the built-in NRF-module would be great :slight_smile:
```

---
## \#697 Posted by: trampa Posted at: 2017-06-15T18:51:46.706Z Reads: 383

```
Benjamin basically dropped the latest firmware onto mine, using a tunnel to Sweden through my Linux laptop. It's not plug and play yet. If you tell me what HW you have, I can see what is the best way to sort out the FW for your device.

Frank
```

---
## \#698 Posted by: DeathCookies Posted at: 2017-06-15T20:50:13.850Z Reads: 371

```
Any Updates on the Firmware for vesc 4.12?
```

---
## \#699 Posted by: squad Posted at: 2017-06-16T18:34:07.771Z Reads: 361

```
@trampa Do You think that in future there will be an option to implement communication with smartphone app via onboard NRF? This would be awesome, being able to change basic VESC parameters on the go, or monitor basic stuff like current, wattage etc.
```

---
## \#700 Posted by: JLabs Posted at: 2017-06-16T22:35:05.843Z Reads: 368

```
I don't think it will be able to because smartphones use Bluetooth and not NRF.
```

---
## \#701 Posted by: trampa Posted at: 2017-06-16T23:26:12.024Z Reads: 375

```
Bluetooth is necessary for that sort of communication. Unfortunately it's quite a task to implement, especially from a legal point of view. Bluetooth communication is not something you can have for free.

Frank
```

---
## \#702 Posted by: trampa Posted at: 2017-06-16T23:27:11.284Z Reads: 378

```
Relax, coming soon. 

Frank
```

---
## \#703 Posted by: notepad Posted at: 2017-06-16T23:54:50.425Z Reads: 359

```
instead of adding bluetooth to the VESC,  one possible way is to have an attachment that allows BT connectivity while the base VESC can understand BT but doesnt have any form of receivers - might be an idea.
```

---
## \#704 Posted by: walshy Posted at: 2017-06-17T07:02:01.190Z Reads: 360

```
i think it would be awesome to have a programme card for vesc so we could program it on the go and make it much simpler for people
```

---
## \#705 Posted by: trampa Posted at: 2017-06-17T09:23:41.101Z Reads: 354

```
That card is called smart phone in future.
The connection will need to be Bluetooth.

Frank
```

---
## \#706 Posted by: walshy Posted at: 2017-06-17T10:33:24.053Z Reads: 351

```
that would be wicked!!!
```

---
## \#707 Posted by: walshy Posted at: 2017-06-17T10:42:40.306Z Reads: 354

```
hey frank how long does it normally take to restock your ultimate mtb,s ruffly? sorry for the off topic question guys
```

---
## \#708 Posted by: DeathCookies Posted at: 2017-06-17T10:59:31.338Z Reads: 356

```
[quote="DeathCookies, post:698, topic:3813, full:true"]
Any Updates on the Firmware for vesc 4.12?
[/quote]

Bump this up
```

---
## \#709 Posted by: trampa Posted at: 2017-06-17T12:18:17.790Z Reads: 355

```
HW 4.xx FW works, we use it and its integrated into another VESC-Tool Version. 
Benjamin wants to open that section on the Website soon, so that Betas can download the Vesc-Tool with FW 4 Support.
After Beta all VESC-Tools will go public.

Frank
```

---
## \#710 Posted by: trampa Posted at: 2017-06-17T12:20:37.309Z Reads: 356

```
I need to check if we have an estimated delivery date already. We are desperate to receive the goods. 

Frank
```

---
## \#711 Posted by: DeathCookies Posted at: 2017-06-17T12:32:29.352Z Reads: 360

```
How long does this beta takes?
```

---
## \#712 Posted by: TranxFu Posted at: 2017-06-17T12:35:12.964Z Reads: 370

```
Maybe you should consider a separate Beta User-base just for the VESC 4's :) You should get more data if its just people that only have access to a VESC4.
```

---
## \#713 Posted by: walshy Posted at: 2017-06-17T14:25:13.674Z Reads: 369

```
ok thanks frank
```

---
## \#714 Posted by: trampa Posted at: 2017-06-17T17:00:11.564Z Reads: 372

```
Well, it gets a bit to much. The feedback should be of a scale that it can be handled.
Vesc-Tool is not far away.

Frank
```

---
## \#715 Posted by: NAT-Frank Posted at: 2017-06-18T15:22:13.787Z Reads: 376

```
$300 a piece is insane! I will wait for a China clone if that's the case. $185 is fine.
```

---
## \#716 Posted by: JLabs Posted at: 2017-06-18T16:44:10.921Z Reads: 374

```
It's actually $385usd when converted from British pounds
```

---
## \#717 Posted by: fedestanco Posted at: 2017-06-18T17:05:47.562Z Reads: 375

```
Minus 20%, because european prices include tax.
```

---
## \#718 Posted by: JLabs Posted at: 2017-06-18T17:08:22.313Z Reads: 371

```
I wasn't aware. Ecerytime I go to Trampas site and go through the checkout process it didn't deduct the 20%. Thanks for the heads up tho
```

---
## \#719 Posted by: fedestanco Posted at: 2017-06-18T17:35:42.220Z Reads: 371

```
<img src="/uploads/db1493/original/3X/b/5/b57dc4c345d1af73c3631a7796fffefcbfc0662c.PNG" width="411" height="179">
287$ is still pretty high but the quality is just astonishing. Plus a good portion goes to the creator (vedder); 
@NAT-Frank buying chinese clones is like using torrents for movies; buying from some reputable sellers is like using netflix (5-10% goes to the creator); the only equivalent of buyng the original dvd right now is going with trampa (I guess they share about 50% with vedder).
```

---
## \#720 Posted by: trampa Posted at: 2017-06-18T18:08:08.551Z Reads: 368

```
It didn't ad it on in the first place. So it didn't subtract it.

Frank
```

---
## \#722 Posted by: JLabs Posted at: 2017-06-18T20:20:23.138Z Reads: 390

```
<img src="/uploads/db1493/original/3X/e/c/ec3e37164d20b1e138aae511fbdcaa9ea609dfa7.PNG" width="281" height="500">
I find that Trampas estimates are always way off for some reason. I even sent an email about 4 months ago about this and I think it was Ted who said that they can be off a bit.

I have a Trampa deco in my cart. This just shows that the Pound is worth more than the dollar and the estimate is off. 

On a side note: the price of the VESC 6 is now 250 pound (not 300).
<img src="/uploads/db1493/original/3X/7/5/75916ec8347bda94585edfa00c6a55c1d3f4d8d6.PNG" width="281" height="500">
```

---
## \#723 Posted by: mmaner Posted at: 2017-06-19T18:46:07.967Z Reads: 376

```
[quote="fedestanco, post:719, topic:3813"]
buying chinese clones is like using torrents for movies
[/quote]

The reason movie torrents are so popular is that its expensive as hell to go the movies.  If you figure $20 for tickets (2 people), another $8 for popcorn + $12 for drinks and another $5 for the obligatory twizzlers...that's $45 bucks for 2 hours of entertainment.  I don't know of anything that has that high of a price point.  

I'm not justifying the use of torrents to pirate movies, software, etc...just trying to see the other side of this thing.  When you straight up molest people on the price of a thing, you have to expect some blackmarket duplication.  Might be a lesson in there for someone.
```

---
## \#724 Posted by: NAT-Frank Posted at: 2017-06-20T00:16:31.698Z Reads: 365

```
I've been flying multirotors for the past 8 years. Now I mostly do freestyle FPV and racing. Lots of guys from the FPV community are starting to get into electric longboards and come over to these forums. Companies like EMAX and DYS are starting to follow the trend too and it won't be very long until we see versions of the vesc6 on banggood. Banggood was the best thing to ever happen to R/C in general. Cheap parts which allow ease of entry to the hobby and forced innovation to stay competitive because of the competition.
```

---
## \#725 Posted by: sl33py Posted at: 2017-06-20T00:23:26.273Z Reads: 366

```
[quote="NAT-Frank, post:715, topic:3813, full:true"]
$300 a piece is insane! I will wait for a China clone if that's the case. $185 is fine.
[/quote]


I'd wait for the reference design to release and your *trustworthy* vendors will offer them hopefully for a lot less.  Enertion, DIYes, Chaka (sounds like he has another variant in the works already), Axle, etc.

Or reflow your own when released!
```

---
## \#726 Posted by: Wolfcola Posted at: 2017-06-20T02:09:58.792Z Reads: 359

```
Sports. You could easily spend $200+ for 3-4 hours of sports entertainment.
```

---
## \#727 Posted by: mmaner Posted at: 2017-06-20T02:37:55.889Z Reads: 357

```
I'm trying to figure it what your point is, not really seeing it.
```

---
## \#728 Posted by: Wolfcola Posted at: 2017-06-20T03:09:20.681Z Reads: 368

```
[quote="mmaner, post:723, topic:3813"]
I don't know of anything that has that high of a price point.
[/quote]

Referring to that.
```

---
## \#729 Posted by: mmaner Posted at: 2017-06-20T03:10:20.040Z Reads: 361

```
Buy what has that got to do with the issue?
```

---
## \#730 Posted by: trampa Posted at: 2017-06-20T10:36:28.666Z Reads: 369

```
Hi JLabs, you pay in pounds anyway. The Pound goes up and down all the time, and I don't think that the situation will change soon. Best way to figure out the actual price is a quick lookup on the internet. Your bank will not give you the daily rate you see. We should ad in Bitcoin, fluctuating even more than the pound (-;

The VESC 6 we make is not cheap to manufacture and the price reflects that. I think other vendors will have cheaper HW SIX design available soon, which is nothing that really worries me and good for customers having a tight budget, or not wanting to spend more than X. 
There are many options to cut down the price or make even more expensive HW for other applications. I'm pretty sure we will see lots of variety and lots of different prices, which is good for the consumer. 

Frank
```

---
## \#731 Posted by: stewii Posted at: 2017-06-20T14:48:42.874Z Reads: 360

```
Hi all. I am currently designing a cheaper version of this PCB. Will keep you guys updated.
```

---
## \#732 Posted by: Dwain Posted at: 2017-06-20T20:32:35.839Z Reads: 374

```
If you got the blueprints to build a Ferrari and built one yourself is it still a Ferrari ? Not really , it wont have the same quality and feel as the real one . This is why i would only buy a vesc 6 from Trampa. They know what they are doing all their products are made with the best parts and quality in mind plus they developed it with Ben. Just take the vesc 4.12 for example , so many variations and differences in quality, its almost impossible to know if ya got a good one or bad one until its actually proven to work well . I have built my MTB a few times now because of faulty or cheap parts , now i only use Trampa for everything i can and their parts are just amazing , never ever had a problem. Yes would be nice to buy a vesc 6 for $100 but if its not from Trampa its not really a vesc 6 in my opinion.  If you buy Trampa you know you have the best and you wont be dissapointed.

Only Trampa for me :)
```

---
## \#733 Posted by: sl33py Posted at: 2017-06-20T20:43:44.173Z Reads: 384

```
[quote="Dwain, post:732, topic:3813"]
If you got the blueprints to build a Ferrari and built one yourself is it still a Ferrari ? Not really , it wont have the same quality and feel as the real one . This is why i would only buy a vesc 6 from Trampa.
[/quote]


I have a pair in hand from Trampa - so i'm not a hater.  BUT i think you are missing the point @Dwain - this will be released as a reference design for our trusted vendors to further develop.  If you haven't seen the improved 4.12 variants from @chaka and @onloop then you will be tied to a single option, which may not always be the "best" depending on your intended use.  And budget, and location (avoid customs delay/costs, or faster shipping), etc.

I agree Trampa is a high quality company, but sometimes it's nice to have a less $ option, at an acceptable quality.  Not always less quality - it's not always "more expensive is nicer".  In particular the new Ollin ESC is gorgeous - just got hands on with his direct FET version helping @smurf with his build.  Not sure how costs line up, but i'd look before buying and compare.

my .02
```

---
## \#734 Posted by: mmaner Posted at: 2017-06-20T21:53:23.698Z Reads: 377

```
[quote="Dwain, post:732, topic:3813"]
If you got the blueprints to build a Ferrari and built one yourself is it still a Ferrari ?
[/quote]

Nope, it's better.  Because you built it yourself...researched every fastener position, material used, assembly process, etc.

You are on DIY site, and telling people not to DIY???
```

---
## \#735 Posted by: Hummie Posted at: 2017-06-21T00:34:58.281Z Reads: 377

```
What a turn of events and we were all waiting for the 6 and now want some updated four.  Puts the challenge on all these other places to take the huge reasonably-priced market. Are the fours that unreliable? If running a dual at least you're safe. 
What are four killers?
I heard running high erpm for one reason.  What else? Just a quick summary if u know
```

---
## \#736 Posted by: trampa Posted at: 2017-06-21T07:45:36.745Z Reads: 381

```
The new VESC-Environment is set up in a way to stipulate variety, so that we will see more different designs soon.
This was one major reason to make the decision to publish reference designs that can be changed, extended, stripped etc. After BETA the reference design will be made and published together with VESC-Tool and the FW.

I personally think the more different designs we will see, the better for the customer and the project itself. 

Frank
```

---
## \#737 Posted by: Minim Posted at: 2017-06-21T08:34:48.634Z Reads: 378

```
Atleast then the confusion will be complete chaos :D
```

---
## \#738 Posted by: trampa Posted at: 2017-06-21T08:43:07.434Z Reads: 383

```
No, its just more choice and reviews will be written etc. 
When you buy a mobile, you also tons of choices - same with cars and bikes, frying pans etc.
Lots of choices create confusion some times, but that's the way it is.
There is no way to change that. 

Frank
```

---
## \#739 Posted by: BigBoyToys Posted at: 2017-06-21T08:55:54.360Z Reads: 378

```
1. High erpm
2. 12S FOC
3. More than 30A continous(doesn't die, but overheats over and over)
4. 4wd CAN BUS has killed 4 of my FOC box's
```

---
## \#740 Posted by: Hummie Posted at: 2017-06-21T16:41:17.527Z Reads: 370

```
maybe your 30 "continuous" is different and being in a city the stop and go is saving me.   You blew 4 vescs at once...that would send me into fits.  You are a big dude
```

---
## \#741 Posted by: notepad Posted at: 2017-06-21T18:47:04.986Z Reads: 374

```
Just took the new Vesc out for a spin on my 12S 33Mph roadster,  and omg it feels so smooth.   plus it never even got close to overheating even when going up a 10/15% incline.  very welldone Frank,  send my regards to the big V aswell
```

---
## \#742 Posted by: BigBoyToys Posted at: 2017-06-21T18:58:55.098Z Reads: 390

```
I actually blew two CAN tranceivers on slaves 3 and 4 and then same thing happened again a month later so it was only 2 at a time lol.

By 30A continuous I mean actually pulling 30A through the VESC for more than say a minute ofr two strait per a vesc current log. Like  when climbing a mile long hill.  I hit soft back off on all the 2wd vesc powerd boards Ive made going up the hill near my house. Yeah Im big lol. 6'2 270lbs.
```

---
## \#743 Posted by: racidon Posted at: 2017-06-21T23:44:45.105Z Reads: 382

```
Finished building my battery for my eMTB last night and setup a very conservative FOC setup (never used FOC before) and it seems to run amazing. I've yet to stand on the thing and take it for a ride, as it was 430am when I was near finished and had realised the time. So went to bed for a few hours for work :) 
I'll hopefully get to ride it tonight as the controller wasn't connecting to the receiver this morning so had to leave it home :frowning:
Setup: 
12s8p   2xVESC6   2xLeopard 8072
```

---
## \#744 Posted by: stewii Posted at: 2017-06-22T09:47:46.601Z Reads: 377

```
That's an unfair comparison. The level of complexity of a Ferrari is many levels above a single 25 cm2 PCB. I don't doubt the trampa's VESC quality but you cannot say what I'm designing is worst or better at the moment. I will use quality parts as well. It will definitely be cheaper and customised.  It is ok if you only buy trampa's. But many of us don't want to spend that much on an ESC.  I love DIY and designing PCB's and have some spare time. ;)
```

---
## \#746 Posted by: Mikeomania12 Posted at: 2017-06-22T14:31:49.055Z Reads: 380

```
I fully support you. I miss real DIY and ppl just making things for free then sharing with community. seems like too many ppl turned this community into a marketplace..
```

---
## \#747 Posted by: DougM Posted at: 2017-06-22T15:00:25.490Z Reads: 373

```
It would be nice if you could offer a bare-board version (no wires, no heat sink no fancy packaging) for $175.
```

---
## \#748 Posted by: JohnnyMeduse Posted at: 2017-06-22T15:06:43.695Z Reads: 375

```
[quote="DougM, post:747, topic:3813"]
no heat sink
[/quote]

then I would only be able to support less than 30 AMP, a good heatsink is a necessity.
```

---
## \#749 Posted by: DougM Posted at: 2017-06-22T15:24:03.562Z Reads: 370

```
@JohnnyMeduse - I realize that but I can make my own heat sink, or find an off-the-shelf that will work.  There are some great heat sinks at online surplus electronics sites.
```

---
## \#750 Posted by: JohnnyMeduse Posted at: 2017-06-22T15:41:36.651Z Reads: 382

```
[quote="DougM, post:749, topic:3813"]
I realize that but I can make my own heat sink
[/quote]

Yes, but It is a crucial part of the design, if it's done badly you can easily hurt yourself and damage the product. In this case it would be a mess for the warranty and insurance issue, because they can't provide real warranty since the product is so easy to temper with....
```

---
## \#751 Posted by: DougM Posted at: 2017-06-22T15:59:29.188Z Reads: 398

```
@JohnnyMeduse I realize that too, but on the other hand you're opening up a whole new market at the $200 level that you're not going to get at the $300 level - me for instance :slight_smile:

So call it a "DIY Special" package and limit the warranty to out of box failures.

I know there are issues, but I also surmise that the $300 price point is too high for this kind of market.  Somebody will offer this.
```

---
## \#752 Posted by: JohnnyMeduse Posted at: 2017-06-22T16:02:31.757Z Reads: 394

```
Yeah, but I'm pretty sure in a few month you will find them at around 200$, from other vendor or maybe trampa... The price is so high right now because they have the exclusivity :wink:
```

---
## \#753 Posted by: okp Posted at: 2017-06-24T18:13:48.643Z Reads: 405

```
Thank you Benjamin, Frank, Ted.

https://youtu.be/uumy8TfTfAw
```

---
## \#754 Posted by: TarzanHBK Posted at: 2017-06-25T12:04:30.603Z Reads: 409

```
yah yah yah! Trying to impress the waving girls, not concentrating and falling of the board :monkey:
```

---
## \#755 Posted by: okashira Posted at: 2017-06-27T18:22:42.916Z Reads: 418

```
Is the VESC 6 firmware ...
(and the updated tool) ...
Going to be open source?
I have read conflicting things... seems the board may or not be open source. But the firmware was going to be open source?
However the repository does not seem to have been updated in quite a while and I am sure firmware updates are needed for the new design.
Does anyone know the plan in terms of the Ben Vedder's recently firmware?
```

---
## \#756 Posted by: oyta Posted at: 2017-06-27T22:27:57.400Z Reads: 431

```
According to Vedder and Trampa: It will be open source after the beta is finished. Timespan of the beta not known by me. It is currently ongoing. I guess Vedder wants things well done before releasing it.

The reference design of the hardware and the software will be released.
```

---
## \#757 Posted by: okashira Posted at: 2017-06-27T23:10:20.617Z Reads: 436

```
I ordered one a few days ago and there was nothing about a beta?
http://www.trampaboards.com/vesc-6-complete--vedder-electronic-speed-controller-trampa-exclusive-p-24166.html
```

---
## \#758 Posted by: longjohn Posted at: 2017-06-28T01:58:05.199Z Reads: 427

```
It won't be served on a silver plate again according to the vesc team
```

---
## \#759 Posted by: trampa Posted at: 2017-06-28T08:40:19.341Z Reads: 429

```
Sure it will be OS. But Beta gives the time to make sure everything is sorted and the code is ready to be published. In the end everyone wants a software with little to no bugs. The time span is up to Benjamin, since he needs to feel comfortable to release it.

Frank
```

---
## \#760 Posted by: racidon Posted at: 2017-06-28T22:44:31.420Z Reads: 422

```
It rides amazing, for the time being until I get a CAN cable sorted I'm running 1 motor at max 40A. I went with 40A as I've never used FOC before (because of apparent issues with it on old hardware). I can see why people much prefer it over BLDC, I wouldn't say it's quiter but it's smother.
```

---
## \#761 Posted by: Pedrodemio Posted at: 2017-06-29T03:38:43.440Z Reads: 420

```
Frank, do you have any idea when the next batch will be available?
```

---
## \#762 Posted by: trampa Posted at: 2017-06-29T04:56:50.269Z Reads: 425

```
I July. Mid to end of July.
I'll try to get an estimated arrival date.

Frank
```

---
## \#763 Posted by: Pedrodemio Posted at: 2017-06-29T05:06:07.968Z Reads: 433

```
Thanks
10char
```

---
## \#764 Posted by: longjohn Posted at: 2017-06-30T07:21:58.769Z Reads: 421

```
Thanks Benjamin and Tramp for this work !

All I am missing is trampa electric KICK SCOOTER FROM HELLLLLLLLLLLLLL
```

---
## \#765 Posted by: notepad Posted at: 2017-07-04T14:07:51.781Z Reads: 407

```
@trampa  Have you and "Big V" concidered making a stripped down lower quality VESC 6.  Something that can only handel 6S or 8S maybe.  The question came to me when I was shopping for a cheap ESC (that wont blow up in my face) as I want to build a cheap E-Pennyboard for going around my local highstreet instead of using my new (Powered by the VESC6) speedster as the VESC is still a bit pricey for a budget build.   

 Plus I absolutely love the new VESC Tool, its a very nice peice of work.
```

---
## \#766 Posted by: Silverline Posted at: 2017-07-04T14:18:18.300Z Reads: 405

```
Why is Vedder not writing in this forum ??
```

---
## \#767 Posted by: NAF Posted at: 2017-07-04T14:41:13.271Z Reads: 414

```
He has his own forum.
```

---
## \#768 Posted by: trampa Posted at: 2017-07-05T08:04:07.676Z Reads: 409

```
Correct! And he has very limited time. He can't get lost in conversation.

Frank
```

---
## \#769 Posted by: okp Posted at: 2017-07-09T06:37:41.368Z Reads: 408

```
https://www.instagram.com/p/BWUN4IuhdCP/
```

---
## \#770 Posted by: trampa Posted at: 2017-07-09T19:04:48.528Z Reads: 400

```
Its a Holy (Pro) Board. Funky helmet BTW.

Frank
```

---
## \#771 Posted by: okp Posted at: 2017-07-11T18:57:03.283Z Reads: 393

```
a quick opportunity to provide feedback. The VESC 6 performs flawlessly. The VESC tool is really great and the wizards addition also a good move for all the people that are getting into VESC. I'm really impressed how strong these bad boys are. 12S FOC dual 6374; silent and bulletproof. I've been using this in all terrain and in urban.

I need now to be able to report data of my rides, but I'm really happy.
```

---
## \#772 Posted by: chuttney1 Posted at: 2017-07-12T04:19:36.267Z Reads: 392

```
The place where Inception was shot. Very easily recognized.
```

---
## \#773 Posted by: Titoxd10001 Posted at: 2017-07-12T07:58:19.563Z Reads: 392

```
@trampa what's the status of the VESC-tool. When will it be available and will non vescs (v4.xx) be supported still
```

---
## \#774 Posted by: trampa Posted at: 2017-07-12T08:42:52.825Z Reads: 396

```
VESC-Tool fro 4.xx is out for betas. Benjamin will go on holidays soon and will be back mid of August.
After the holidays the release will happen. This way we get more feedback from VESC 4.xx users and 
Benjamin has time to answer questions that will arise once the software is available. 
So we are 4-5 weeks away from a release. 

Frank
```

---
## \#775 Posted by: TranxFu Posted at: 2017-07-12T09:03:07.538Z Reads: 389

```
@trampa Frank, Is there still a way to apply for the beta (VESC-Tool 4.XX) ?
```

---
## \#776 Posted by: sl33py Posted at: 2017-07-12T22:52:40.880Z Reads: 392

```
Just to confirm the new VESC Tool works great with 4.xx hardware.  I've configured two VESC 4.7, and one 4.12 w/o issue.

All updated to 3.25/3.26 fw (not sure exactly since not in front of me), the 4.12 running FOC (149kv 8s).

Wizards are stupid simple and make it so much easier.  Even fixed both 4.7 which were missing bootloaders.  No STLink needed (but good to have just in case).

Have a 4th to configure as soon as i get a moment - for my GF's board.  Think i'm moving her to FOC as well (192kv 8s).
```

---
## \#777 Posted by: Maxid Posted at: 2017-07-13T05:11:10.050Z Reads: 383

```
Do you know what changed firmwarewise for the Vesc 4s? I am kind of hoping that the real contribution by Vedder is not even the new 6 hardware but the changes he made to the firmware - no matter the Vesc version
```

---
## \#778 Posted by: karma Posted at: 2017-07-13T11:11:45.936Z Reads: 387

```
@sl33py have you tried running FOC on 10S or 12S with the new VESC Tool?
```

---
## \#779 Posted by: dannyboy Posted at: 2017-07-13T12:02:45.831Z Reads: 399

```
Hopefully not completely off topic, does involve VSEC 6, so we'll see... Any fundamental reason that the VSEC 6 would not be able to drive a single LARGE hub, and I mean larger than those used on skateboard, or even mountainboards, about 200mm total wheel, stator likely about 70-80mm?

You're probably thinking "how can he possibly ask such a question without including specs of the motor!??" And you're right. Probably should wait until I have it and have measured everything. I have cheapy HK car escs to test with and intend to determine max current draw at 0 RPM WOT torque, so should know more soon.

But figured I might ask anyway, there might be something fundamental to the VSEC 6 that would prohibit it's use for larger hub motors. Something that would mean that even if I limited the current in software, if I had massive batteries to soak up regen current spikes, if I had alu/acetone heat pipes attached to active sinks to keep it super cool, even with all that maybe I should be looking elsewhere for a controller for such a massive wheel.

P.s. love this forum, I haven't built anything yet, but have read pretty much every post! Even the commercial arguments with the guys trading and manufacturing are fascinating, such a good community.
```

---
## \#780 Posted by: dannyboy Posted at: 2017-07-13T12:19:58.126Z Reads: 379

```
Maybe I should include the basics that I do know (haven't had delivery from mysterious Chinese supplier yet), I believe these are well within VSEC capabilities: I intend to run at 10-12s, maximum continuous (>60s) power draw of 300W, so about 7A, perhaps 40A at start up. I don't know stator count or winding topology, so cannot calculate ERPM, but even with lots of stators the wheel is so large that at 15mph (max speed) I cant imagine ERPM will be >60k.

I just worry as there is mention on these forums of large motor instability and if that might be a result of stator counts then maybe I'm way off looking at VSEC. I just like all the features and the quality. The fact that the electronics are well understood by the community etc.
```

---
## \#781 Posted by: sl33py Posted at: 2017-07-13T15:44:37.772Z Reads: 378

```
@dannyboy - yes.  You sound like you are doing e-bike stuff.  VESC has been used frequently for this running large hub motors for e-bikes.

VESC Six will remove the 60k ERPM limit and has been tested around 150k ERPM from what i've heard and seen on Benjamin's test videos.

I would suggest looking at the ebike section of ES as they will have a ton of experience to help you.  Assuming you are thinking bike and not something else.  

Added benefit of 6 will be more constant current capacity vs v4.xx.

GL!
```

---
## \#782 Posted by: sl33py Posted at: 2017-07-13T15:48:35.494Z Reads: 380

```
@karma - i've not yet.  I will still need to avoid >60k ERPM on the 4.xx hw.  I won't run 12s given 192kv - BLDC or FOC.  I might go up to 12s on my guest board as it's only 149kv... but being for guests i'm trying to keep it safe/slow'ish - so most of the time will probably only run 6 or 8s.

I have another couple in process and building some 18650 packs, so something will get at least 10s if not 12s and likely FOC.
```

---
## \#783 Posted by: Jinra Posted at: 2017-07-13T15:54:01.817Z Reads: 374

```
I run 230kv @ 10s which is the same theoretical eRPM as 190kv @ 12s with no issues. Real motor kv's tend to be about 10kv lower than advertised, and after you factor in various inefficiencies such as voltage sag, you get an eRPM approximately 5k lower than calculated.
```

---
## \#784 Posted by: chaka Posted at: 2017-07-13T15:55:14.150Z Reads: 379

```
The [FOCBOX](http://www.enertionboards.com/vesc-x-speed-controller.html) and our[ Ollin ESC](http://www.ollinboardcompany.com/product/direct-vesc-v2-0-pre-order) are both based on v4.12 with the same or higher constant current capability of the vesc6. If you are using motors outside the scope of eboarding you will probably want the 3rd current shunt resistor the vesc6 offers.
```

---
## \#785 Posted by: sl33py Posted at: 2017-07-13T16:02:12.117Z Reads: 376

```
I've seen that as well.  I've also found that "bleeding edge" of the VESC is rarely a good idea for long term reliability.  I have 4.7 hw that has been going strong for 2+ years now...  I've found being moderate in your settings and sticking to BLDC is the best way to keep it simple and reliable.  I've got a couple Axle VESC's with the improved BOM components which i'll test FOC a bit more.
```

---
## \#786 Posted by: Jinra Posted at: 2017-07-13T16:05:31.833Z Reads: 380

```
Axle, Ollin, or FOCBOX are the only VESC4's I'd buy. Too many people cheap out on their VESC and complain when they break. Better to overspec, than to get the bare minimum and be surprised or inured when it breaks beyond that.

I'll play around with FOC once I get my focboxes from the group buy.
```

---
## \#787 Posted by: dannyboy Posted at: 2017-07-14T11:59:42.750Z Reads: 392

```
Thanks for the encouragement! I thought I'd read a lot on this forum, apparently I missed an entire section - did not know there was an ebike section for ES. I'll check it out.

As it happens I'm making a scooter not a bike, as in a kick scooter. I intend to run initially off one hub motor at back. (ultimately, if time allows building the whole thing and having two wheel drive with a hub at both ends). Larger than most have at about 200mm external tyre diameter. Because the width puts the effective moment of inertia midway between a skateboard and a bike I thought I'd read lots here first and just liked the 'lively' nature of the discussions and the (mostly) fairly technical / knowledgeable responses. And as I said previously, the VSEC - specifically the 6 - looks like a very nice bit of electronics and far more interesting than the big(er) branded EV / ebike controllers.

And in case you're wondering: the scooter solution because its for commuting and: I can't skate, think folding bikes on UK trains should be punishable by death unless they fit in the overheads because of the vital standing room they use up, because whilst not legal on pavements I think at 8-10 mph at 7am even in london the rush is small enough to allow for safe mixing with pedestrians, and having commuted through central london on a sports bike for half a decade and fluking survival, I want to use my making obsessions to engineer myself some transport!
```

---
## \#788 Posted by: sl33py Posted at: 2017-07-14T19:33:23.625Z Reads: 381

```
Definitely check out ES.  I've seen a few scooter builds (most w/ motor/gears not hubs), and they look perfect for your use.  Might have some inspiration as you get closer to building.

Because i'm a bigger guy i would opt for a stealthy motor setup vs hubs (gearing helps with hills and keeps speeds down on high voltage), but know this will be covered on ES too.

Post a build here - most of the electronics will carry over and it's much more active here for help and feedback.

The VESC Six seems ideal, but even a 4.12 VESC likely could do what you need without trouble.  I'd look at a single setup until you need dual (motor or hubs) since it's significantly more complex/costly to go dual vs single.

If you start a thread on ES, let us know and will follow either location!

GL!
```

---
## \#790 Posted by: TeleRando Posted at: 2017-07-15T03:54:21.213Z Reads: 353

```
Sweet scoot. Will it chooch?
```

---
## \#791 Posted by: Minim Posted at: 2017-07-15T08:48:20.085Z Reads: 362

```
What does "with NRF" means? 

Side note, is it just me or is the trampa website horrible? It feels really messy and it's hard to get around. Like internet 1998 all over :D
```

---
## \#792 Posted by: JTAG Posted at: 2017-07-15T11:47:24.081Z Reads: 364

```
Hahahaha sorry @trampa but this is true :joy:  :joy:  :joy:  :joy:  :joy: .
```

---
## \#793 Posted by: trampa Posted at: 2017-07-15T20:59:02.975Z Reads: 375

```
NRF is a radio transceiver, integrated in VESC SIX. Due to difficult regulations (e.g. FCC), we do not ship them with NRF to countries outside the EU. Anyway, there is currently no NRF hand held radio controller available, so the NRF transceiver is only interesting for those , who can build a replacement PCB for the Nunckuck, according to the files provided by Benjamin Vedder on Git Hub. 

Frank
```

---
## \#794 Posted by: Minim Posted at: 2017-07-15T22:34:41.503Z Reads: 387

```
Thanks for the explanation.
```

---
## \#795 Posted by: fedestanco Posted at: 2017-07-16T01:38:34.256Z Reads: 396

```
Actually a few days back I saw this nrf controller on taobao: <img src="/uploads/db1493/original/3X/e/a/eaaa6bafd72ec2182194f94f673dfc0cca8d36d7.jpg" width="500" height="500">
Maybe you want to check it out since it has some nice specs like 18650 cellholder and joystick. Plus it is just 6€.
http://c.b1yt.com/h.mx6Yht?cv=HZJZ00TFzaF&sm=510bba
```

---
## \#796 Posted by: trampa Posted at: 2017-07-16T15:27:48.147Z Reads: 386

```
The china NRF are a gamble. We didn't have to much success with those devices.

Thx for the Info, Frank
```

---
## \#797 Posted by: dannyboy Posted at: 2017-07-18T10:40:19.036Z Reads: 390

```
Apologies if the answer to the following is well established, but will cheaper 6.0's be available later in the year from anyone, any plans?

Once the beta phase is done, the designer happy, no immediate tweaks required, the circuit designs released as open source (or whichever complicated variant), once that is all done and beta testers of the 6.0 all have 100km of trouble free FOC silently and smoothly logged ;), are there plans for anyone else to start making boards? I know there are a few people here making the old(er) design at more sensible prices, but the new one currently available at $350 is bit out of my league at the moment. Just wondering if it always will be.

N.B. not sure if anyone else thinks like this, but: while I'd struggle to accurately solder up the whole thing in under a year and for less than a $1000 (I'd break the fets 7 times each), all the tertiary bits I can do myself - things like the case, heat sinks, connectors. Also I understand the drive and market for a version which is tested on the production line (twice apparently) for the more financially endowed out there, but there would also be a market for those of us who would happily do the testing ourselves, risk having to send it back or debug (with a little help!) if that meant saving a couple of quid.

P.s. By the way - no implied rebukement of the price point or work done on the ones in production, I have no right or inclination to criticize, if anything they look great, I just wonder if cheaper versions are planned by anyone.
```

---
## \#798 Posted by: chuttney1 Posted at: 2017-07-19T06:52:41.912Z Reads: 376

```
The thing about VESC 6.0, an aluminum heatsink is mandatory for cooling the DirectFET MOSFET. I assume 33% of $350 was in the cost of CNC machining an aluminum case for the VESC 6.0.
```

---
## \#799 Posted by: longjohn Posted at: 2017-07-19T07:14:26.788Z Reads: 373

```
Chuttney.

Whatever the cost was for the aluminium heatsink,

A good chunk of money went to Trampa and Benjamin.

And I am GLAD it did, it well make the future of the VESC project much better.

Everyone should be happy about Benjamin getting rewarded !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!

one love, Benjamin.
```

---
## \#800 Posted by: trampa Posted at: 2017-07-19T07:28:17.816Z Reads: 368

```
Actually US customers don't pay VAT! Its easy to deduct 20%. A twin set is 550pounds incl.VAT.
So that equals 288$ per VESC. Price drops with volume. The casing and second PCB ad cost, just like the testing does. We want 100% happy customers. So we try not to cut any corners. In the end its still cheaper than dealing with cheap but fried HW. 

Frank
```

---
## \#801 Posted by: Mathias Posted at: 2017-07-19T10:03:46.621Z Reads: 369

```
I don't think we can really complain about the price. You can get 4.12s for about 100$. @chaka's version with a reputation to be superior in quality is already 165$, and his DFET version is 220$. The step to the 6s with 340$ is not that big. It is a brand new product, probably a big advance, includes NRF etc... Of course it's expensive! I don't think it was ever supposed to be a kind of low end or more affordable version. The different 4.12s versions are still around and fill that niche. And the new firmware/software will make those more awesome too! I'm sure as soon as the VESC6 goes open it won't take long until this community releases new spins on the 6 with more affordable versions for different applications. 

For most people it doesn't make sense to buy the current design for dual setups with two NRFs and more power than most riders would ever want under their feet, or their batteries could handle...  If you can't wait, buy a 4.12 for now. That's what I'm doing for my first build. My second build will be hopefully already be with the 6! Just be patient!:+1:
```

---
## \#802 Posted by: dannyboy Posted at: 2017-07-19T10:18:32.110Z Reads: 366

```
Sorry, just to be clear, I wasn't complaining about the price, not sure if I was misunderstood, or if the ensuing comments were just coincidentally unrelated remarks by people on how they think the price is fine. I did actually literally write "P.s. By the way - no implied rebukement of the price point...if anything they look great"

I really was just wondering if anyone else had any **plans** to make any no-frills versions based on the new designs, **eventually**, i.e. in many months. No lack of patience here.
```

---
## \#803 Posted by: Mathias Posted at: 2017-07-19T11:10:10.911Z Reads: 368

```
OK, I wasn't criticizing you! Sorry if my post gave that impression! I just had a feeling that this is the opinion of many users here (based on numerous posts about the VESC6), and I don't really agree. Many were hoping for something more affordable, and are disappointed. My point was more, that they don't need to be, because they will get it. It will just take a while. 

I guess about plans for different versions we will know very soon, when the usual suspects in this community regarding electronics get their hands on the reference design, firmware, software etc! Should be a matter of weeks before we know more. Pretty excited, too... It's going to be a good year!
```

---
## \#804 Posted by: dannyboy Posted at: 2017-07-19T12:29:09.590Z Reads: 376

```
cool :slight_smile: And I do see your point - a lot of grumbling here about the price in a way that makes no sense, it seems perfectly fair to charge more initially to offset R&D.

Excitement abound here too. And frankly I'm too busy (and poor) to actually get any electronics just yet anyway, every night consumed with 6 month old son & messing with printing new molds for the carbon arms and pillow blocks for the giant hub for my electrified decathlon scooter (or Frankenstein's Scooter as I think I shall call it). Am just hoping that when (in maybe 5 years) I have made the arms fit, there will be a reliable ESC I can afford!

Machining my own heat sinks, packing in my own capacitor boards as it happens will likely be needed anyway for my machine due to the design you see, so am hoping a more 'barebones' product might be released by someone, but it wouldn't' be the end of the world if I end up paying for bits I dont need.
```

---
## \#805 Posted by: chinzw Posted at: 2017-07-19T18:38:54.510Z Reads: 356

```
And im here still waiting for someone to do a dual vesc (a real dual, not just to vescs botched together)
```

---
## \#806 Posted by: Kaly Posted at: 2017-07-19T19:35:43.483Z Reads: 356

```
The problem with dual ESC has been that if one dies the other will die too. 

Same goes for a DUAL DUAL :stuck_out_tongue_winking_eye:
```

---
## \#807 Posted by: chinzw Posted at: 2017-07-19T20:52:27.107Z Reads: 355

```
@kaly vescs can be repaired fairly easily, that's not an issue. Also there's a ton of components that are duplicated that wouldn't be needed anymore, thus bringing the overall cost down.
```

---
## \#808 Posted by: Jinra Posted at: 2017-07-19T20:55:19.835Z Reads: 356

```
If you share the components across 2 VESCs then you're essentially doubling the amount of work, calculations, and switching the VESC has to do. You'll need completely different components to make up for it.
```

---
## \#809 Posted by: chuttney1 Posted at: 2017-07-19T21:24:26.774Z Reads: 361

```
I'm hoping the files are released by the fourth quarter.
```

---
## \#810 Posted by: dannyboy Posted at: 2017-07-20T08:09:02.974Z Reads: 359

```
I'm looking ultimately for two driven wheels, so the dualness is interesting. I was under the impression that two VESCs could be set to communicate over the CAN bus, even including such cunning as least-node-speed traction control. But I guess that not the sort of duality to which you refer?

Maybe you mean more of a hot-standby, fail over redundancy type config? I.e. both wired to the same wheel with some sort of keep-alive comms between them and the standby able to jump into action the moment the other fails. Sounds scary - if the failure mode were not a simple total death then having both wired in parallel to the phase wires could be quite nasty.
```

---
## \#811 Posted by: trampa Posted at: 2017-07-20T10:32:12.007Z Reads: 349

```
A TWIN VESC SIX.... We thought about it, but It doesn't cut a lot of cost and if you have a problem with it, you have a twin problem. Not worth it. Traces also get to long, which is not in favour of performance. 

Frank
```

---
## \#812 Posted by: notepad Posted at: 2017-07-20T13:17:50.667Z Reads: 353

```
Just wondering.  but what happened to the vesc 5?  all I seem to see is 4,  4.1,  4.12, 6
```

---
## \#813 Posted by: trampa Posted at: 2017-07-20T13:29:07.765Z Reads: 361

```
VESC 5 was skipped, since Benjamin and I wanted better performance. When we teamed up, BV made the decision to rewrite the software ground up, instead of tweaking BLDC-Tool further. We had that moment of - come on, lets bite the bullet.... The new software/FW allowed the design of VESC 6. In consequence Vesc 5 was outdated before it even hit the market. Its all about the software!

Frank
```

---
## \#814 Posted by: notepad Posted at: 2017-07-20T13:33:19.124Z Reads: 351

```
thats a nice little story. makes me a bit happier the 6 is out instead of the 5 as well.  you guys rock!
```

---
## \#815 Posted by: trampa Posted at: 2017-07-20T13:51:04.377Z Reads: 349

```
I personally think it was good to bite the bullet and boost the project to the next level. 
There was so much involved. Website, legal issues, communication, software, GUI, hardware prototyping, testing, finding an outstanding manufacturer etc., tons of research.... 15 months of hard work. I think everyone will profit from that, not only Benjamin and us. Manufacturers will start make their own HW designs, rather than copying one design over and over. They will start to build up their own brands in future, backed by a project on solid foundations and a strong community surrounding it. We know it took time and caused delays - but in the end its worth it. You got the see the bigger picture.

Frank
```

---
## \#816 Posted by: akira Posted at: 2017-07-20T15:18:05.856Z Reads: 357

```
Hi Franck,
Why do you say that manufacturer will develop new HW with the new VESC6. If you release a reference design that is good enough (and I wish it will be since I plan to solder it myself instead of buying it), don't you think that manufacturer will stick to it ? 
What make the new buisness model any different that the 4.12 one ? The changes in HW of the 4.12 from the manufacturers were quite minimal (except for the FOCBOX and the directFET from Chaka). What make you think it will be any different with the reference VESC6 ? Will the reference design be that much below the trampa one that manufacturer will be forced to develop their design to be competitive/usable on an e-sk8 ?
```

---
## \#817 Posted by: trampa Posted at: 2017-07-20T15:43:26.011Z Reads: 358

```
Hi Akira, the new FW simply allows more different HW designs. That easy. I also think that a growing project will encourage people to make products with USPs. Some will sell on price point, others on innovation and quality.

Frank
```

---
## \#818 Posted by: akira Posted at: 2017-07-20T16:54:24.065Z Reads: 350

```
Thanks for the answer. I didn't make the link with the FW. 
Looking forward to the release.
```

---
## \#819 Posted by: psychotiller Posted at: 2017-07-20T17:36:07.241Z Reads: 356

```
Oh shit!!! If it makes him feel better to know, I now feel better knowing I'm not the only one hobbled..I hope his recovery is speedy!!!
```

---
## \#820 Posted by: trampa Posted at: 2017-07-20T21:23:15.923Z Reads: 362

```
It's all fine now. Plaster is off, back on two feet.
I serviced his board, so in September we can do a little tour again. Titanium kingpins, titanium bones...
All we need now is a titanium VESC housing.

Frank
```

---
## \#821 Posted by: wafflejock Posted at: 2017-07-20T21:26:08.197Z Reads: 362

```
Ti TM... Unfortunately Texas instruments has that one I'd imagine.
```

---
## \#822 Posted by: ironsquirrel89 Posted at: 2017-07-25T00:34:55.944Z Reads: 360

```
Frank, will the non-beta VESC 6 be shipped when Benjamin gets back from holidays or before then?
```

---
## \#823 Posted by: trampa Posted at: 2017-07-25T06:43:45.229Z Reads: 362

```
About second week of August if everything goes to plan.

Frank
```

---
## \#824 Posted by: DougM Posted at: 2017-07-26T20:08:55.831Z Reads: 354

```
Is there a list we can get on for the second-week-of-August shipment?
```

---
## \#825 Posted by: Pedrodemio Posted at: 2017-07-26T22:45:22.761Z Reads: 345

```
@trampa Hey frank, what can we modify on the VESC 6 without losing warranty? Can I open it and solder new wires?

I sent you a email about that a few weeks ago
```

---
## \#826 Posted by: trampa Posted at: 2017-07-26T23:12:53.070Z Reads: 339

```
We run everything through our system. If you order one, it will get shipped as soon as as we flashed and tested them.

Frank
```

---
## \#827 Posted by: trampa Posted at: 2017-07-26T23:14:57.425Z Reads: 350

```
What should I say.... If you open them, you need a new heat pad. If you solder close to the FETs, you have to be careful. The new batch has 25cm long silicone cables. Why do you want to solder?. I can not warrant your mods.

Frank
```

---
## \#828 Posted by: Pedrodemio Posted at: 2017-07-27T01:58:22.706Z Reads: 342

```
Thanks, my board will have motor wires running through the deck, and I want to avoid one more conector, but no problem, I will add a bullet in the deck - vesc connection 

Cutting the wires shorter and changing the connectors is ok them?
```

---
## \#829 Posted by: gogomrrobot Posted at: 2017-07-27T02:10:42.824Z Reads: 350

```
Anybody in the US organizing a VESC-6 group buy?  If you are please PM or link it to me. I am good for (2).
```

---
## \#830 Posted by: trampa Posted at: 2017-07-27T06:57:31.307Z Reads: 364

```
**This is what keeps us alive:**

_MORNING . _

_I JUST RODE MY STREET CARVER FOR THE FIRST TIME - VESC 6 - _

_O M G _

_THIS IS THE BEST CONTROL I HAVE EVER HAD - PROGRESSIVE BRAKING , SMOOTH ACCELERATION….._

_YOU GUYS ROKK…._

_THIS IS IT _

_PLEASE SAVE ME 12 VESC 6 UNITS.._

_I AM BLOWN AWAY BY THE EXPERIENCE I HAVE JUST HAD ON A SINGLE MOTOR………_

_THANKS !_

_over …… :_)_
```

---
## \#831 Posted by: trampa Posted at: 2017-07-27T07:05:45.392Z Reads: 363

```
BTW: The new batch is on its way to us. Revision 6.41, 25 cm long motor cables, and some minor changes on the PCB and casing. 

Frank
```

---
## \#832 Posted by: onloop Posted at: 2017-07-27T07:19:16.486Z Reads: 363

```
[quote="trampa, post:830, topic:3813"]
THIS IS THE BEST CONTROL I HAVE EVER HAD - PROGRESSIVE BRAKING , SMOOTH ACCELERATION…..
[/quote]

Have these aspects been improved with the new VESC 6 hardware/software?

common with all vesc, no?
```

---
## \#833 Posted by: trampa Posted at: 2017-07-27T08:17:56.370Z Reads: 366

```
three different types of throttle curves, three shunts, major FOC improvements etc...
```

---
## \#834 Posted by: trampa Posted at: 2017-07-27T08:32:21.157Z Reads: 361

```
Chop them!
```

---
## \#835 Posted by: phantomi Posted at: 2017-07-27T20:29:10.070Z Reads: 362

```
If I order now, will I receive the latest revision (6.41)? How long will it take from ordering to shipment?
```

---
## \#837 Posted by: trampa Posted at: 2017-07-27T20:52:59.862Z Reads: 369

```
Fast. I think we will have them on Tuesday. We do extensive testing before we ship, so that will take some days.
```

---
## \#838 Posted by: trampa Posted at: 2017-08-02T19:13:05.017Z Reads: 362

```
The VESC Six is back in stock. We ship the day you order.

Frank
```

---
## \#839 Posted by: JTAG Posted at: 2017-08-02T21:32:55.118Z Reads: 361

```
Did you fix the missing bootloader issue with the recently shipped batch?

On the VESC I received today the Bootloader seemed te be missing :astonished:.

Edit: Both new VESC's had the bootloader missing :sweat_smile:.
```

---
## \#840 Posted by: trampa Posted at: 2017-08-02T23:04:18.922Z Reads: 358

```
No, Benjamin was on well earned hollidays and Vesc-Tool let's you update it anyway. Next batch.

Frank
```

---
## \#841 Posted by: JTAG Posted at: 2017-08-02T23:09:33.916Z Reads: 353

```
Than why didn't you do it? Receiving a flashed bootloader and updated the firmware version would have made the hands-on experience a lot better for new user.:neutral_face:
```

---
## \#842 Posted by: trampa Posted at: 2017-08-03T13:28:41.697Z Reads: 343

```
It's one process doing the FW upload, spin up test and a reference VESC comparison. We will update the software of the test bench for the next batch. 
It's just two clicks in Vesc-Tool and you are sorted.

Frank
```

---
## \#843 Posted by: JTAG Posted at: 2017-08-03T14:01:27.642Z Reads: 349

```
"It's just two clicks in Vesc-Tool and you are sorted." --> Than why didn't you do it during testing?

The first thing people need to do when they receive the VESC is upgrade the firmware. During that procedure NOTHING will tell the user it failed, it will just do nothing, that's a bad user experience. You knew this was an issue with your test setup, you had chance to fix this issue with the current batch with a computer that was probably no more than 2 meters from your test setup.

It's a 300 GBP product! With the knowledge you had you should have lived up to the quality you claim to deliver.
```

---
## \#844 Posted by: trampa Posted at: 2017-08-03T16:12:14.410Z Reads: 352

```
Benjamin is still on holidays. The test bench will get its update very soon. We need to nail the VESCs in one hit, otherwise it's to time consuming. People want their boards being made the same day they order and everyone is already at the limit.
We are a small company and try our best to get the goods to the customer veey very fast. The US customers are always surprized to recieve their boards four days after purchase! 
We need to nail all orders till 14:30 to get them out the same day. This is why we set up a system to handle the VESCs efficiently on a test bench. The test bench doesn't start VESC-Tool. So the staff has no chance to do do the job. 
Everyone got a mail, so they know they need to do that additional click on "upload bootloder". 
Not perfect but not tragic.... We will sort that out ASAP.

The issue has a positive effect as well: It forced Benjamin to implement the boot loader upload. Everyone with a HW 4.xx having no boot loader aboard can now simply update the missing boot loader. 

Frank
```

---
## \#845 Posted by: chaka Posted at: 2017-08-03T16:21:15.504Z Reads: 344

```
Nice feature to have! I can confirm, final testing is time consuming. Would be nice to have an automated tester to run the vesc through a firmware upload/bootloader test. Right now I am still testing the bootloader manually on each VESC before running a motor test. It is tedious!
```

---
## \#846 Posted by: trampa Posted at: 2017-08-03T16:24:25.661Z Reads: 351

```
Benjamin can send you the same software we use. 
It will be the standard in future. We are the test bench for the test bench.

Frank
```

---
## \#847 Posted by: sebaszz Posted at: 2017-08-04T08:04:56.404Z Reads: 360

```
I have 1 VESC 6.0 for sale

http://www.electric-skateboard.builders/t/vesc-6-0-eu-300/29666
```

---
## \#849 Posted by: notger Posted at: 2017-08-06T15:05:37.821Z Reads: 358

```
Hi,

a question that i couldnt find answered until now.:

Is a antispark (switch) recommended with the VESC6 or maybe even "onboard"?

and where are detailed infos on the VESC6 like: max rated Amps, measurements, uF of the Caps,.......................

greets

Notger
```

---
## \#850 Posted by: trampa Posted at: 2017-08-06T15:52:30.569Z Reads: 346

```
A switch is not integrated. So you need to buy one of you want one. Max continuous Amps are 80A, depending on your cooling. I have to look up the exact caps value (I think it's 2x 680uF). They sit just next to the FETs /power stage, which helps a lot. 

Frank
```

---
## \#851 Posted by: notger Posted at: 2017-08-06T16:08:23.010Z Reads: 344

```
so will the quick and rough precharge of the 5,8ohm inbuild resistor in XT90-Antispark   be ok or do you recommen a "FET-based slow precharge"

2x 680uF does not sound that much for 80A continuous ?

and @Trampa are currently availeable VESC6's still "beta"  or do you call it "stable"  now ??
```

---
## \#852 Posted by: trampa Posted at: 2017-08-06T16:34:09.668Z Reads: 348

```
They are stable. The caps are fine, no one will push 80A continuous on a skateboard. There are applications putting a lot more strain on the caps. 
The design of the power stage and cap integration has a very big impact on the strain you put to the caps. Benjamin has a video online, showing the caps heat under load. The power stage of VESC six is magnitudes better than on HW 4.xx. 

XT 90 works. A power switch with FETs is a very good option. I would still use a XT90 loop key in addition.

Frank
```

---
## \#853 Posted by: racidon Posted at: 2017-08-08T00:56:08.448Z Reads: 350

```
[quote="onloop, post:832, topic:3813, full:true"]
[quote="trampa, post:830, topic:3813"]
THIS IS THE BEST CONTROL I HAVE EVER HAD - PROGRESSIVE BRAKING , SMOOTH ACCELERATION…..
[/quote]

Have these aspects been improved with the new VESC 6 hardware/software?

common with all vesc, no?
[/quote]

Without a lot of setting up they don't **_feel_** much different to the improved 4s
But the ability to go 12s eMTB is reason enough to go with these. Along with the feature of what the VESC does when the control loses connection.
I'm currently at 12s @80A (iirc) with dual VESC (can) using Leopards 8072 175kv
```

---
## \#854 Posted by: notger Posted at: 2017-08-08T05:50:40.505Z Reads: 349

```
[quote="racidon, post:853, topic:3813"]
Without a lot of setting up they don't feel much different to the improved 4s
But the ability to go 12s eMTB is reason enough to go with these. Along with the feature of what the VESC does when the control loses connection.
I'm currently at 12s @80A (iirc) with dual VESC (can) using Leopards 8072 175kv
[/quote]


wait, i'm not sure if i understand what you are saying but it sounds interesting ;-)

- the improved 4s is what ? (does it mean -> you changed from VESC4. to VESC6 or from 8s to 12s)  cause you could have done that with the VESC4 too
- also the VESC4 with newest firmware was able to go with 12s ? so whats different ?
- holy shit,.. really.. you use 80A constant and no problems with overheating - whow if,.. then they are pretty amazing --> do you life in a flat or hilly/mountain area ?
```

---
## \#855 Posted by: chaka Posted at: 2017-08-08T12:56:47.556Z Reads: 337

```
Our v1.1 ESC formerly known as VESC can power an eMTB without any trouble. It can match the VESC 6 in throughput. You are really only using 45 amps max for any extended period of time on an eboard of any type during hard acceleration. Sure we get some spikes during initial takeoff but they are momentary. Of course, I could be wrong but my testing and record keeping shows we never use much more than 2000-2500 watts max with a 200# rider.
```

---
## \#856 Posted by: notger Posted at: 2017-08-08T13:43:16.140Z Reads: 342

```
Heres some Question that just came up for me today when finishing my Trampa-magura-Servo-brake.

I use a HV-Servo with 2slipos so max 8,4Volts.
my Gt2B receiver takes that 8,4 Volts quite well as it seems (cause its max is rated to 6Volts)

So what about the PPM in of the VESC (6 and 4.12) will i get troubles if i plug the PPM cabel into a HV (8,4Volts max) receiver ??

greets

Gernot
```

---
## \#857 Posted by: i2oadsweepei2 Posted at: 2017-08-08T14:58:42.154Z Reads: 339

```
Going above the max rating of anything is not recommended. But you know that :) If you are powering your receiver externally with a receiver pack then you would remove the red wire going to the vesc and tape it off safely. Normally the vesc would power the receiver with 5 or 6 volts. I can't see it liking 8.4v.
```

---
## \#858 Posted by: akira Posted at: 2017-08-08T17:08:45.711Z Reads: 343

```
I was wondering if the VESC6 will be able to run 240KV motors at higher voltage that the older 4.12 version.
Will 240KV with 10S (or even 12S) be possible and safe ?
```

---
## \#859 Posted by: Titoxd10001 Posted at: 2017-08-08T19:51:41.574Z Reads: 342

```
Is there a update to when vesc tool will go public
```

---
## \#860 Posted by: trampa Posted at: 2017-08-08T20:35:21.951Z Reads: 342

```
The ERPM limit is not an issue any more. Up to 150K ERPM is fine. A 240KV Motor is no issue at all.

Frank
```

---
## \#861 Posted by: onepunchboard Posted at: 2017-08-08T21:23:41.836Z Reads: 339

```
Wow, 150k?! so you guys solved drv issue? amazing
```

---
## \#862 Posted by: trampa Posted at: 2017-08-08T21:49:19.558Z Reads: 340

```
There is no DRV issue any more. That is a matter of the past. Since we made the first prototypes, till today, we have not burned a single device. Rock solid. Frank
```

---
## \#863 Posted by: trampa Posted at: 2017-08-08T21:50:01.669Z Reads: 342

```
Soon. It's in Benjamins hands. Frank
```

---
## \#864 Posted by: racidon Posted at: 2017-08-08T22:32:36.989Z Reads: 357

```
[quote="notger, post:854, topic:3813, full:true"]
[quote="racidon, post:853, topic:3813"]
Without a lot of setting up they don't feel much different to the improved 4s
But the ability to go 12s eMTB is reason enough to go with these. Along with the feature of what the VESC does when the control loses connection.
I'm currently at 12s @80A (iirc) with dual VESC (can) using Leopards 8072 175kv
[/quote]


wait, i'm not sure if i understand what you are saying but it sounds interesting ;-)

- the improved 4s is what ? (does it mean -> you changed from VESC4. to VESC6 or from 8s to 12s)  cause you could have done that with the VESC4 too
- also the VESC4 with newest firmware was able to go with 12s ? so whats different ?
- holy shit,.. really.. you use 80A constant and no problems with overheating - whow if,.. then they are pretty amazing --> do you life in a flat or hilly/mountain area ?
[/quote]

Sorry the "improved 4s" was in relation to VESC4 (plural). Meaning Chaka's improved FET version and enertion's FOCBOX? (formerly VESC-X) Sorry if I got names wrong, I honestly don't remember the names.
Not all VESC4 would be able to regardless of firmware, I'm sure chaka's would, I have one of his on my 10s board, but it was never "supported" so I never risked it, I've never had a problem with his
80A wouldn't be constant, it's just the limit set in the VESC itself. I live in a hilly area and I have no problem getting up or down any of them, even when my battery was running low I could still cruise up an extremely hill at about 40km/h
```

---
## \#865 Posted by: racidon Posted at: 2017-08-08T22:35:33.115Z Reads: 357

```
[quote="chaka, post:855, topic:3813, full:true"]
Our v1.1 ESC formerly known as VESC can power an eMTB without any trouble. It can match the VESC 6 in throughput. You are really only using 45 amps max for any extended period of time on an eboard of any type during hard acceleration. Sure we get some spikes during initial takeoff but they are momentary. Of course, I could be wrong but my testing and record keeping shows we never use much more than 2000-2500 watts max with a 200# rider.
[/quote]

I'd say I use more than 45 in at least initial take off and hill climbs. I only say this because I had originally set the limit of the board to 40A max only as I was playing with a lot of settings and it still hadn't been extensively tested by users. I noticed a massive difference between 40A and 80A max values. I do doubt though that it's ever tried to pull 80A at any point. I might have to record some numbers for you all :)
```

---
## \#866 Posted by: WrinklyWink Posted at: 2017-08-12T05:43:45.265Z Reads: 348

```
hey, I was wondering what JST connectors max amps are for the 5v?
Can I connect a micro usb to it and charge a phone? :sweat_smile:
```

---
## \#867 Posted by: Hanok Posted at: 2017-08-14T08:08:36.237Z Reads: 352

```
I received VESC6.
Is this waterproof?
Silicone seal is not visible.
Trampa hompage -> "Precision made Silicon seal prevents the ingress of dirt & water"

https://www.youtube.com/watch?v=ReXeavPoW0Q&feature=youtu.be
```

---
## \#868 Posted by: Nowind Posted at: 2017-08-14T10:28:16.718Z Reads: 342

```
Nice lights :sunny:
```

---
## \#869 Posted by: trampa Posted at: 2017-08-14T15:51:22.198Z Reads: 342

```
The moulds are finished soon. So we will offer the sealing and another silicone part soon.

Frank
```

---
## \#870 Posted by: notger Posted at: 2017-08-14T16:53:41.711Z Reads: 341

```
comeon, thats not nice,......to advertise something thats actually not part of the product you buy.
Or did you inform your beta testers that the silicone seal is not included ?

are the VESC6 we could order right now from the trampa webshop still BETA ?
```

---
## \#871 Posted by: onepunchboard Posted at: 2017-08-14T17:34:06.541Z Reads: 337

```
I agree with you, and for $500 usd too
```

---
## \#872 Posted by: notepad Posted at: 2017-08-14T19:42:27.081Z Reads: 340

```
the part was never advertised as being water proof. only water resistant, which is already is.  But frank has been taking on advice from the beta backers to add a silicone front part to the wires not for water resistance, but so the wires dont get damaged by the sharp metal heatsink.  more water resistance was only a by product of the upgrade.
```

---
## \#873 Posted by: trampa Posted at: 2017-08-14T22:18:25.288Z Reads: 334

```
We redesigned the housing slightly and will make two different parts.

a: a silicone insert for the housing (quite a complex 3D shaped thing)
b: a silicone sleeve, similar to a smartphone cover, considering the JST connections and cables

Both moulds are currently in the make.
If you combine the two parts, water has very little to no chance entering the housing.

The parts can also be used for the first beta VESC SIX. 

Frank
```

---
## \#874 Posted by: chuttney1 Posted at: 2017-08-14T22:28:34.536Z Reads: 331

```
If it's a silicone seal. I would rather go to my local auto store and use the black stuff for sealing transmissions instead of buying a gasket.
```

---
## \#875 Posted by: notger Posted at: 2017-08-15T09:52:05.452Z Reads: 326

```
sounds interesting, could you post some photos or renders of the silicone sleeve-thing.
I'm interested how it will effect the total height of the VESC6
```

---
## \#876 Posted by: trampa Posted at: 2017-08-15T09:57:20.229Z Reads: 326

```
A few mm only.

Frank
```

---
## \#877 Posted by: Tarzan Posted at: 2017-08-15T10:36:03.059Z Reads: 333

```
Not Ok!
If you like I can search the post or mail where you said "all beta testers will get the gasket when it's finished!"
```

---
## \#878 Posted by: longjohn Posted at: 2017-08-16T00:32:00.672Z Reads: 336

```
[quote="Tarzan, post:877, topic:3813"]
e I can search the post or mail where yo
[/quote]

hehehehe £££££££££££££££££££££££££££££££££££
```

---
## \#879 Posted by: dakota4e Posted at: 2017-08-16T02:05:37.959Z Reads: 329

```
Finally wrestled my USB ports into connecting to my VESC betas.

Now says my firmware is not up to date, and firmware updates seem to be unsuccessful.

What can I do now?

Sorry, I am not an electronics wizard, so please talk softly! LOL
```

---
## \#880 Posted by: racidon Posted at: 2017-08-16T04:00:47.466Z Reads: 330

```
[quote="dakota4e, post:879, topic:3813, full:true"]
Finally wrestled my USB ports into connecting to my VESC betas.

Now says my firmware is not up to date, and firmware updates seem to be unsuccessful.

What can I do now?

Sorry, I am not an electronics wizard, so please talk softly! LOL
[/quote]

@dakota4e if you use the link in the email that you should have got from frank about getting on to the VESC Beta forum there is a thread there explaining how to load the firmware onto your VESC
```

---
## \#881 Posted by: dakota4e Posted at: 2017-08-16T04:31:35.439Z Reads: 327

```
Finally got it figured out.  Thank you so much.

I feel like a moron.  I have them both working now, but they spin in opposing directions when connected via the CAN bus connector I made.

Furthermore, forward on my throttle (FSky) transmitter makes the master VESC go in reverse, while the slave goes forward.  I have been messing with it (including reversing the throttle switch on on the transmitter, and checking all wiring) and I cannot get the master to behave correctly or get the slave to mimic the master.

What in the hell?

Again, not an expert.  But holy cow.
```

---
## \#882 Posted by: racidon Posted at: 2017-08-16T05:14:15.517Z Reads: 334

```
[quote="dakota4e, post:881, topic:3813, full:true"]
Finally got it figured out.  Thank you so much.

I feel like a moron.  I have them both working now, but they spin in opposing directions when connected via the CAN bus connector I made.

Furthermore, forward on my throttle (FSky) transmitter makes the master VESC go in reverse, while the slave goes forward.  I have been messing with it (including reversing the throttle switch on on the transmitter, and checking all wiring) and I cannot get the master to behave correctly or get the slave to mimic the master.

What in the hell?

Again, not an expert.  But holy cow.
[/quote]

All you have to do is swap 2 of the motor wires around for your master vesc.

So if you have "A B and C" connected to say Blue green and yellow (your motor wires may not have any descriptive markings, purely an example) then you just change A and B around so that they are connect to the other's original connections.
```

---
## \#883 Posted by: dakota4e Posted at: 2017-08-16T05:19:34.824Z Reads: 334

```
Annnnnnnd.  It works as I am sure you know.

I really respect all the electronics knowledge around here.  Motor phases are something my biology degree did not help me understand shockingly LOL.

I really just loaded a lot of defaults as I set these up.  Wondering if there are any golden settings that make the board work at its peak?   

I have not ridden yet, have to mount all of the components definitively to the board now.  I suppose I should evaluate the ride-ability of it before I go adjusting anything.  The new VESC tool is fairly easy to use, although much of what is adjustable I do not understand as you could imagine.

Much thanks!  I am an expert in wakeboats and wakesurfing if you should ever need advice in that arena!  HAHAHAHA
```

---
## \#884 Posted by: landonkun Posted at: 2017-08-16T05:26:48.429Z Reads: 336

```
[quote="dakota4e, post:883, topic:3813"]
I really just loaded a lot of defaults as I set these up.  Wondering if there are any golden settings that make the board work at its peak?
[/quote]

Most of the vesc settings depend on what type of battery and motor(s) you have.
If you post what type of setup you have, I'm sure someone will be able to help you out. There are also many threads about how to program the vesc, so you'll find your answer if you do some digging :slight_smile:
```

---
## \#885 Posted by: DougM Posted at: 2017-08-16T07:33:57.544Z Reads: 326

```
is the serial interface the same in 6 as it was in 4?  I'm using the VESCUART library currently.
```

---
## \#886 Posted by: onloop Posted at: 2017-08-16T08:57:19.823Z Reads: 343

```
[quote="dakota4e, post:883, topic:3813"]
The new VESC tool is fairly easy to use, although much of what is adjustable I do not understand as you could imagine.
[/quote]

When the vesc tool is _eventually_ released the entire community will work on it and help create instructional videos and furthermore be able to offer one-on-one direct support here to noobs on this forum. No Doubt will Help debug it too.

It seems counterintuitive to limit access to this, we all know, from the beginning the vesc project greatly benefited from the masses working together as a collective.... The masses made it what it is today.

This is starting to feel slow, boring and closed... Not open and innovative.

**Don't be a fool, release the tool.**
```

---
## \#887 Posted by: scepterr Posted at: 2017-08-16T09:01:56.068Z Reads: 339

```
Rather wait than deal with something that doesn't perform to expectations. #UnderPromiseOverDeliver
```

---
## \#888 Posted by: Nexo Posted at: 2017-08-16T09:19:18.557Z Reads: 345

```
I am waiting for a proper VESC6 as well, but at least for now it looks like something is "not finished"

I need to have vesc that will handle dual 6374 mountainboard setup powered by 12s battery and VESC6 seems like the best choice for that
...but on the other hand I can see opinions about problems with sealings, vesc tool, etc
```

---
## \#889 Posted by: scepterr Posted at: 2017-08-16T09:47:48.047Z Reads: 346

```
For every person thats not happy about it's current state there's a person who wants it now regardless of any possible issues lol
```

---
## \#890 Posted by: dakota4e Posted at: 2017-08-16T13:06:41.687Z Reads: 340

```
Truth--I was getting weary of digging, honestly.  Turned into a lazy bum.  I have a  12S twin trampa 136Kv vesc 6 urban carver.  Freshly built, and obviously first build.
```

---
## \#891 Posted by: racidon Posted at: 2017-08-16T22:35:29.201Z Reads: 345

```
I would be careful using that, I'd make sure to get an answer from BV before you can be certain you won't brick your vesc. I know that upon first release an app that iirc used that library caused issues for a user as the UART codes have changed. This could all be a thing of he past now, but likely that the VESCUART needs updating to match the interface for VESC 6.
```

---
## \#892 Posted by: racidon Posted at: 2017-08-16T22:36:45.202Z Reads: 342

```
As @scepterr said.
However with that said, @chaka is confident that his improved VESC 4  (sorry can't remember the new official name) will handle all that without issues.
```

---
## \#893 Posted by: DougM Posted at: 2017-08-17T02:30:15.091Z Reads: 341

```
Thanks for the feedback @racidon, I'll post on the VESC Project forum and see what they say.  Will report back here.

Is RollingGecko here?
```

---
## \#894 Posted by: Minim Posted at: 2017-08-17T08:49:54.162Z Reads: 352

```
Hehe what a commedy this whole namechange is... all should be named VESC 4 or whatever they where made from and a little note about who produced it. Now it's just annoying and misleading for the customers. Also it's starting to look like the vesc project is going from open source at the same time. Not cool!

I don't need another fairy tail about TM frank, we disagree, heavily. To me this is trampa trying to make some extra $$$ out off benjamins work nothing else. No point trying to hide it ^^
```

---
## \#895 Posted by: bavo Posted at: 2017-08-17T09:59:03.742Z Reads: 356

```
it is still open source, benjamin is working together with trampa to sell it, trampa is selling the beta (not 100% sure on this one) once benjamin is ready with the software he will release it and its open source again

as for the naming, with the trademark only trampa is allowed to call it VESC all the others have to use another name but can still use the same pcb/software etc
```

---
## \#896 Posted by: trampa Posted at: 2017-08-17T14:02:50.243Z Reads: 364

```
Ben is still on holidays and so am I. You guys know that he had a bad accident and that caused delays.
Proper recovery is important! 

The Software is ready, but the structure for project support needs a couple of days of attention. A lot of people want to contribute to the code and things need to be set up for that. Otherwise things get messy. It's better to have one tidy place for everyone's needs than scattered information and code. I think most people would agree on that.

After the software release we can focus on the hardware. Beta gave some good feedback that can be used to make a better reference HW design. Its 95% done.
Unfortunately a day has only 24 hours and a week 7 days. Not everything ca be done simultaneously. 

Frank
```

---
## \#897 Posted by: DougM Posted at: 2017-08-18T16:12:24.612Z Reads: 350

```
Update:

RollingGecko has created a VESC6 branch on his GitHub.  Haven't had a chance to look at it yet but will report back.
```

---
## \#898 Posted by: hexakopter Posted at: 2017-08-19T22:53:55.367Z Reads: 346

```
@Tarzan Here you go:
"For now the VESCs will be shipped without a rubber seal for the cables and cover since the mold for it takes more time, but once it is ready we will ship it to you."
So I think at least all people from BETA batch 1 will get the sealing shipped for free as it was mentioned back in time.
```

---
## \#899 Posted by: xxlv Posted at: 2017-08-20T13:30:14.653Z Reads: 339

```
Now it is mid August and still not open sourced... :(
```

---
## \#900 Posted by: squad Posted at: 2017-08-20T14:23:32.118Z Reads: 339

```
That's what I'm was hoping for too! 😎
```

---
## \#901 Posted by: Minim Posted at: 2017-08-20T14:26:00.613Z Reads: 333

```
Don't hold your breath :D Maybe it will get a TM and the developers can buy access to the code for only $9999,99 from trampaboards :joy:
```

---
## \#902 Posted by: racidon Posted at: 2017-08-21T01:26:36.545Z Reads: 349

```
[quote="Minim, post:894, topic:3813, full:true"]
Hehe what a commedy this whole namechange is... all should be named VESC 4 or whatever they where made from and a little note about who produced it. Now it's just annoying and misleading for the customers. Also it's starting to look like the vesc project is going from open source at the same time. Not cool!

I don't need another fairy tail about TM frank, we disagree, heavily. To me this is trampa trying to make some extra $$$ out off benjamins work nothing else. No point trying to hide it ^^
[/quote]

I'll happily pay the extra $ for the added quality that has come from this new approach. I had 3 VESC 4s fail on me in a row for no apparent reason without any responsibility taken by the manufacturer. Don't get me wrong there are some good VESC 4s out there, but this will mean that someone can't just take a well known and respected name and stamp it on trash.
```

---
## \#903 Posted by: mmaner Posted at: 2017-08-21T01:38:09.974Z Reads: 345

```
[quote="Minim, post:901, topic:3813"]
Don't hold your breath :smiley: Maybe it will get a TM and the developers can buy access to the code for only $9999,99 from trampaboards :joy:
[/quote]

Just figured I'd quote this since someone is getting flag happy when they dont like something they see...shame
```

---
## \#904 Posted by: Klattrup Posted at: 2017-08-21T16:31:34.264Z Reads: 345

```
Any chance you need guys help testing the bootload-upload function over USB? I've got at couple 4.12's without bootloader and I would love to give your software a try as I haven't got a SWD tool. :( Thx
```

---
## \#905 Posted by: notepad Posted at: 2017-08-22T02:07:32.483Z Reads: 350

```
Just thought id tell you why I flagged this.  I found it not directly relating to the topic and of bad taste. It didnt provide any extra information towards the topic other than to be a cheap dig towards frank and the current dealings.  The vesc 6 is of a superb quality and will get the development needed by frank and vedder before being released as open source.  

development takes time. and I am willing to stand by frank and vedder while they continue to develop this amazing product.
```

---
## \#906 Posted by: flywithgriff Posted at: 2017-08-22T02:19:49.850Z Reads: 354

```
Well with ten likes apparently he is not the only one that feels this way. I can understand your siding with Frank and Trampa as you have been here for only a few months and have no clue of the past in vesc development. By all means, support who you choose but do not chastise the guys that have been here the whole time and know what has been done.
```

---
## \#907 Posted by: racidon Posted at: 2017-08-23T06:21:23.353Z Reads: 354

```
[quote="flywithgriff, post:906, topic:3813, full:true"]
Well with ten likes apparently he is not the only one that feels this way. I can understand your siding with Frank and Trampa as you have been here for only a few months and have no clue of the past in vesc development. By all means, support who you choose but do not chastise the guys that have been here the whole time and know what has been done.
[/quote]

Have you been here long enough to know when certain people had a bad rep with some users here about either CS, QA, or ETAs and anyone that complained had their topics locked, renamed, or even were threatened to be banned if they continued. Why should the bad mouthing towards Trampa be treated any different?
```

---
## \#908 Posted by: trampa Posted at: 2017-08-23T15:50:51.650Z Reads: 342

```
Release is very soon! Benjamin bangs on it right now. First software then hardware, since both needs some attention and manpower is limited. Yes, release is very close. 

BTW: most people don't get the point that the motivation behind the project, and most OS stuff is not to serve random hardware manufacturers with free and instant available designs to be copied over and over. The motivation is to share the code and ideas about hardware designs, so the knowledge is not in a locked off box.
Free code helps software developers to learn from other developers. It's about sharing the knowledge among each other, so the same thing doesn't need to be re-invented over and over. This will help to focus on interesting and new developments instead of digging around with problems that have been solved already be someone else.
It helps to connect and debate solutions that can be used in all sorts of applications.
If someone has a good idea, code can be written, debated and might be integrated to make the software even better in future. 99% of the work is in the software.

Frank
```

---
## \#910 Posted by: akira Posted at: 2017-08-23T16:27:35.447Z Reads: 337

```
[quote="trampa, post:908, topic:3813"]
ideas about hardware designs
[/quote]

only ideas about HW ? 
No reference design PCB+schematics ?
```

---
## \#911 Posted by: trampa Posted at: 2017-08-23T18:32:05.633Z Reads: 335

```
Akira, there will be a working reference design. The last paragraph is about the motivation in general. People share ideas and not every idea ends in a product, but still serves others as an inspiration. There are already some guys who made their own Version 6 design, for hobby purpose. Most look completely different to the design we came up with. 

Frank
```

---
## \#912 Posted by: nw-esk8 Posted at: 2017-08-25T00:53:57.517Z Reads: 335

```
Is this still the case or is this based on the old beta hardware?  I haven't been able to find any more recent info on 13s/14s+VESCs, but looking at the current manual online, it says the VESC6 is rated up to 60v... If that's accurate, 14s charged and *fully* topped off is still less than that, so I'm hoping it's doable on the latest H/W?  (My ebike has an ESC with a 60v limit and that thing handles 14s all day long.)

Being able to squeeze out those extra watts w/o increasing the current is certainly nice... and even just going from 13s to 14s is _very_ noticeable (...at least on an ebike...)  Thanks.
```

---
## \#913 Posted by: JohnnyMeduse Posted at: 2017-08-25T01:01:29.324Z Reads: 323

```
Nah the New DRV is rated as the same voltage as the old, so is the new vesc, pushing it to more than 12S is asking for trouble.
```

---
## \#914 Posted by: nw-esk8 Posted at: 2017-08-25T01:05:54.985Z Reads: 332

```
Ahhh, that is a bit of a bummer... but thanks for the info.  I brought up the question once before, but the answers I got felt more like guesses :).

It sounds like the manual needs an update, though, if 60v is going to fry things.
```

---
## \#915 Posted by: nw-esk8 Posted at: 2017-08-25T01:11:39.898Z Reads: 337

```
I'll throw another question at ya while I've got your attention...since you seem to know more things :sweat: ...

Is there any technical reason (beyond that it just isn't currently supported now/yet) why two VESCs couldn't provide double the current when used in parallel and synchronized via CANbus (with each motor having a master and a slave VESC, the slave only contributing available current (...and data back to the master))?  ...since canbus supports full duplex and has plenty of bandwidth, AFAIK.

It seemed like a potentially cheaper way to scale current while the product is matured (IE: 100a FOC for ~$200ish +/-, if doable)... but I don't know enough to know why it wouldn't be possible.  I've tried asking it a few times, but haven't got any good bites.
```

---
## \#916 Posted by: SORRENTINO Posted at: 2017-08-25T18:30:07.163Z Reads: 330

```
Does anyone have the dimensions of the VESC6?
```

---
## \#917 Posted by: JohnnyMeduse Posted at: 2017-08-25T18:37:57.336Z Reads: 341

```
Sorry you did loose my attention :sweat_smile:

[quote="nw-esk8, post:915, topic:3813"]
Is there any technical reason (beyond that it just isn't currently supported now/yet) why two VESCs couldn't provide double the current when used in parallel and synchronized via CANbus (with each motor having a master and a slave VESC, the slave only contributing available current (...and data back to the master))?  ...since canbus supports full duplex and has plenty of bandwidth, AFAIK.
[/quote]

Just to be sure are you asking if you can use two vesc to control one motor ?... If it is just a current issue, direct fet can drive a crazy amount of current if the heat is sink properly.
```

---
## \#918 Posted by: nw-esk8 Posted at: 2017-08-25T21:38:08.847Z Reads: 349

```
Hah, well at least I got it back.

...but yeah, that's essentially what I'm asking... and it is a current issue... 

...but hopefully there'd be an option w/o requiring the skillz to solder direct fets by hand or a reflow oven, designing a heatsink, etc.... but even the VESCs w/ direct fets + improved heatsinks don't double the continuous current rating, AFAIK (even though they may double (or more) in price).

Thoughts?  Thanks.
```

---
## \#919 Posted by: notger Posted at: 2017-08-26T07:11:48.801Z Reads: 361

```
You are a reader of Jensos [Direct-Drive-Vesc-6-Thread](http://www.electric-skateboard.builders/t/e-toxx-directdrive-vs-trampa-vesc6-vs-leopard-8072-170kv-vs-nowind/30822/112) so you probably read that he used the "unleashed-Firmware" that is availeable.
There you can set you Amps to whatever. Jenso tried it up to 130 Phase Amps and 100 Batt Amps if i remember right.
So i guess with really huge heatsink and good cooling you could potentially go to 200Amps ?
But High Amps produce High Temperature (generally speaking), so a better Solution to get more Watts is increasing the Voltage. 

But whats the Purpose actually ? an Ebike ?  
The Vesc (6) is for sure a great skateboard ESC but its save Limit is at 12 s (50Volt fully carged, and potentially 60Volt Spikes). It think for High-Power-Ebikes (5000Watts and more) there are other Controllers with the ability of taking ~100Volts (20s-25s). with the effect of needing less Amps then.
Ceck out [Adaptto](http://adaptto.com/Products/Controllers/) controller from Russia, they are amazing, i use two of the Minis with up to 4KW, an they include BMS, Carging-coil, Display,.... Sure, not Open-Source, but really amazing customer-service and reaction on customers wishes in my experience. (They will actually release a new Version "soon")
```

---
## \#920 Posted by: notger Posted at: 2017-08-26T07:15:35.539Z Reads: 365

```
[quote="hexakopter, post:909, topic:3813"]
For all the FOCBOXs that are failing right now because of cheap and crap production
[/quote]

Really? havent heard of that ? Many Focboxes are failing right now ? I thouhgt they are said to be pretty steardy. But for sure produced in China with that Price.
```

---
## \#921 Posted by: nw-esk8 Posted at: 2017-08-26T08:19:58.484Z Reads: 370

```
Me? I didn't catch that it was some special unleashed firmware, but I did see the values... does that kill the warranty, since the manual has a rating of 80a, IIRC?  ...and ideally overclocking wouldn't be necessary :).

e-bikes is how transitioned over here... 3000w is plenty for me on that front... gears :).

...my application is potentially for a mountainboard build... still figuring out what my options are.
```

---
## \#922 Posted by: notger Posted at: 2017-08-26T09:16:29.499Z Reads: 376

```
[quote="nw-esk8, post:921, topic:3813"]
my application is potentially for a mountainboard build... still figuring out what my options are.
[/quote]

So, you were asking for 200Amps,..Stick to @Nowind 's experiences, i think he is one of the Guys here pushing it to the Limits, and he seems to be Quite happy with his Actual VESC6 Settings 

[quote="Nowind, post:129, topic:30822"]
130MC-100BC-175AC
[/quote]

So i guess you first have to try how  2X2000 Watts on a e-(MT)board feel like and then think about Pushing Limits further.

[quote="nw-esk8, post:921, topic:3813"]
does that kill the warranty
[/quote]
I'm pretty sure about that, otherwise i would be surprised that Trampa accepts "willful destruction"
```

---
## \#923 Posted by: nw-esk8 Posted at: 2017-08-26T12:28:00.698Z Reads: 359

```
120-150a for me (TBD)... but the question wasn't necessarily for my specific build, I just wanted to know if something like that would be possible in general (and a potential future feature/option).  

...but as far as my specific goals, I definitely look to nowind for inspiration/guidance, but I think he pushes the limits to the breaking point.  I'd be hoping for something that can be pushed on 24/7 without breaking.
```

---
## \#924 Posted by: xxlv Posted at: 2017-08-29T09:03:59.267Z Reads: 353

```
Just wondering if you and Ben are OK? Still no Release and it is end of August
```

---
## \#925 Posted by: trampa Posted at: 2017-08-29T09:58:50.710Z Reads: 368

```
He bangs on it and we are not far away! 

Frank
```

---
## \#926 Posted by: NAF Posted at: 2017-08-30T07:57:57.941Z Reads: 381

```
[quote="hexakopter, post:909, topic:3813"]
For all the FOCBOXs that are failing right now because of cheap and crap production
[/quote]

What are you talking about ? Are those FOCBOX made in China bad all of a sudden ? I havn't seen anyone here complaining about the quality. I am just curious cause it used to be good.
```

---
## \#927 Posted by: onepunchboard Posted at: 2017-08-31T05:11:20.077Z Reads: 373

```
@NAF I actually use heavily but it back itself off before I  kill drv. which is very good feature. and even over 60k erpm limit, tho I didn't test extensively, I don't have any problem so far.
```

---
## \#928 Posted by: mkeboard Posted at: 2017-09-04T01:15:54.843Z Reads: 370

```
Does anyone know what the power output from the comm port is? I'm hoping to run a 5V led strip off of it, which may need around 2 amps.
```

---
## \#929 Posted by: MysticalDork Posted at: 2017-09-04T01:23:27.455Z Reads: 371

```
IIRC the 5v output is limited to 1.5 amps, and some of that is required to run the board itself, so I wouldn't go over 1 amp.
```

---
## \#930 Posted by: mkeboard Posted at: 2017-09-04T02:02:03.832Z Reads: 365

```
:pensive: Oh well. It might be a good idea to have a 3s lipo to run 12v headlights and other accessories anyway. I could still run the led strips by using one of those car usb chargers to drop the voltage down.
```

---
## \#931 Posted by: MysticalDork Posted at: 2017-09-04T02:03:57.208Z Reads: 370

```
I used a constant-current LED driver to run the headlight on my board, and it works very well, you might want to look into that.
```

---
## \#932 Posted by: ironsquirrel89 Posted at: 2017-09-04T21:08:25.926Z Reads: 380

```
Hey guys just letting you know that http://www.vesc-project.com/ is open to the public now
```

---
## \#933 Posted by: trampa Posted at: 2017-09-04T22:06:12.098Z Reads: 390

```
This is why I started a thread about it.

http://www.electric-skateboard.builders/t/vesc-project-com-is-online-public-vesc-tool-download/32268

Frank
```

---
## \#934 Posted by: sl33py Posted at: 2017-09-05T00:02:58.340Z Reads: 379

```
Kudos to both Ben and @trampa for bringing this to the rest of the VESC users here.

Seriously - you have to try the new VESC Tool - it is AWESOME!  I've programmed more VESC 4.xx than my two VESC 6. 
 It is so much simpler and easy to configure!!!

Don't know what improvements in the FW vs older BLDC tool, but simplicity and ease of configuring is a huge huge improvement!!

Thanks guys!!!
```

---
## \#935 Posted by: notepad Posted at: 2017-09-05T14:16:28.627Z Reads: 371

```
So, Im starting a new project that uses 8 motors (all need to do the same task). 

Does anyone know how many VESCs can be daisy chaned together as I cant seem to find any threads on how many can be used in unison or what problems can arise from using multiple together?
```

---
## \#936 Posted by: Pimousse Posted at: 2017-09-05T14:52:00.301Z Reads: 369

```
If the limit is the CAN ID number, it should be 256 devices (8bit coded), so you have some margin.
```

---
## \#937 Posted by: sl33py Posted at: 2017-09-05T18:44:38.138Z Reads: 374

```
I believe if any fail in the chain - the ones past that controller will also lose signal/control.  So you might want some form of redundant signal.  I know Ben suggested against split servo control and only canbus for dual VESC 6, but i've run dual VESC 4.xx this way without issue, so besides cost savings 8 4.xx might be better (redundant) vs 8 VESC Six.

If you want to go all Six's - i'd post up on his forum and see if he has any suggestions.

HTH - GL!
```

---
## \#938 Posted by: notepad Posted at: 2017-09-06T00:08:46.693Z Reads: 371

```
Thats some good advice there.  The plan is to make a small plannetary engine using 8 planet gears, therefore 8 motors to run a beefed up gocart.   Do you know of any resons a split servo shouldnt be used as wouldnt the input signal be the exact same for each vesc that way?

paging @trampa  What are your thoughts on this as I see you posted in another thread about never using the Y splitters

Edit:  Would it be possible to have multiple receivers connected to a single remote, so each motor/vesc combo can have a dedicated receiver..  that way if one of the motors fail, it wont shut down the rest of the chain??
```

---
## \#939 Posted by: Pimousse Posted at: 2017-09-06T06:38:22.965Z Reads: 361

```
Using Y PPM slpitter on VESC 6 result in fried components.
There are more sensitive on VESC6 than VESC4, so if you never experienced trouble doing it with HW4.xx, ask @Nowind about HW6 ;) 

See the thread where we're talking about it.
```

---
## \#940 Posted by: bigben Posted at: 2017-09-06T06:48:25.923Z Reads: 370

```
Multiple receivers can be connected to a single remote. 
For the small cost of the extra receivers I would think in this application that that would give you the best backup?
There was a lot of discussion of the pros and cons on this thread.
http://www.electric-skateboard.builders/t/y-piece-or-canbus/26461
```

---
## \#941 Posted by: BigBoyToys Posted at: 2017-09-06T07:29:57.465Z Reads: 367

```
Yes, Im using 4 receivers and 1 remote with the HKGT2B
```

---
## \#942 Posted by: notepad Posted at: 2017-09-06T22:48:23.036Z Reads: 371

```
Thats perfect news then.

Thanks for the help @BigBoyToys @bigben @Pimousse.  next step is putting the DIY engine together :stuck_out_tongue:
```

---
## \#943 Posted by: lrdesigns Posted at: 2017-09-07T01:29:59.790Z Reads: 387

```
[quote="notepad, post:942, topic:3813"]
next step is putting the DIY engine together
[/quote]

Will there be a build thread here or somewhere? That will be great popcorn material! :heart_eyes:
```

---
## \#944 Posted by: notepad Posted at: 2017-09-08T03:24:21.177Z Reads: 390

```
There definitely will be ( even though its not directly esk8 based )

and it all starts by me finally finishing building a £1.2k printer to make the large-ass gearbox for the motors ( pls save my wallet )
```

---
## \#945 Posted by: okp Posted at: 2017-09-16T19:38:21.054Z Reads: 385

```
a quick update. The VESC 6 are still performing perfectly in whatever conditions. I got an eagle tree heavy duty and they barely go above 30°C in most of the cases. I'm running dual FOC 12S.
```

---
## \#946 Posted by: okp Posted at: 2017-09-17T19:30:22.773Z Reads: 398

```
<img src="/uploads/db1493/original/3X/c/a/ca8a35e0ac2571eb531acfe1aaec7bcd2b1ac61d.png" width="690" height="481">
```

---
## \#947 Posted by: stewii Posted at: 2017-09-18T15:49:55.067Z Reads: 387

```
Just a quick update, I am waiting for my PCBs to arrive of my own version of the VESC6 , it is very similar to the original. Got all the components and reflow oven is waiting :)  fingers crossed that all is going to work.
```

---
## \#948 Posted by: bigben Posted at: 2017-09-18T18:04:05.580Z Reads: 387

```
<img src="/uploads/db1493/original/3X/6/9/69c5d936cfc6ce9449031e884a927dd09fde56a2.JPG" width="375" height="500">
Looks like you might not be the only one waiting for their PCBs. These guys have even got their boxes ready!
```

---
## \#949 Posted by: rich Posted at: 2017-09-18T18:11:06.121Z Reads: 379

```
Oh no :confounded:
Please Maytech, don't sell more crap!
```

---
## \#950 Posted by: bigben Posted at: 2017-09-18T18:11:54.562Z Reads: 379

```
And they'll have to fold it to fit in the box...
```

---
## \#951 Posted by: gogomrrobot Posted at: 2017-09-18T18:32:05.018Z Reads: 379

```
I don't understand, I didn't see Vedder release the PCB yet on vesc project, so how did you already order the PCB?
```

---
## \#952 Posted by: stewii Posted at: 2017-09-18T18:38:13.767Z Reads: 375

```
He released the schematics only, not the PCB. I have designed the PCB myself with Altium software. It took quite a while to do it in my spare time, but it is a hobby for me.
```

---
## \#953 Posted by: gogomrrobot Posted at: 2017-09-18T18:39:28.944Z Reads: 378

```
Cool stuff man ;)  I can't wait to see what happens when you fire yours up. Please do share... really exciting times.
```

---
## \#954 Posted by: banjaxxed Posted at: 2017-09-18T18:40:24.081Z Reads: 375

```
Would you consider releasing some readymade to the hungry hoardes here?
```

---
## \#955 Posted by: stewii Posted at: 2017-09-18T18:58:18.699Z Reads: 375

```
Definitely, after populating the PCB and run some tests.
```

---
## \#956 Posted by: akira Posted at: 2017-09-19T11:31:54.228Z Reads: 370

```
Can't wait !
I also have a reflow oven heating :-)
```

---
## \#957 Posted by: mishrasubhransu Posted at: 2017-09-19T18:05:41.993Z Reads: 369

```
Did you buy a solder mask too? If so from where? Your PCBs are from OSHPark?
```

---
## \#958 Posted by: chaka Posted at: 2017-09-19T19:06:27.871Z Reads: 377

```
I get mine from oshstencils, they do stainless now.
```

---
## \#959 Posted by: notepad Posted at: 2017-09-20T00:06:21.400Z Reads: 387

```
Quick question.  How many Watts can the Vesc 6 push before overheating.  I was looking into possible upgrades for my board to fully utilise the Vesc and I found something interesting with the motors.

I have a SK3 168kv which can push 2.4Kw  but the sk3 192kv can push ~4Kw.  Its seems that the 192Kv motor is the most powerful sk3 you can purchase for raw Watt output.

What do you guys think.  Might be worth the change in motor to get more performance even with the higher Kv
```

---
## \#960 Posted by: MysticalDork Posted at: 2017-09-20T05:59:00.091Z Reads: 379

```
I don't know if anyone has found the absolute limit in terms of burst current with adequate cooling, but the vesc6 can do at least ~80 amps continuous with minimal cooling other than free air. I'd take Hobbyking's ratings with a grain of salt too, since the rating of a motor is basically its ability to withstand and reject heat - more cooling means more power rating. More copper means more burst rating. I doubt they've added much more copper or managed to add a cooling fan, so I'd be skeptical of a 60% power rating increase. 

With large enough battery, vesc6 plus a 6374, I think the vesc will win if given enough cooling. 

Of course unless you're going up a 50% grade at 50km/h for a few km continuously, I think you'll be safe.
```

---
## \#961 Posted by: trampa Posted at: 2017-09-20T07:12:14.982Z Reads: 373

```
Vesc will win, that's sure. Different KV motors are perfectly the same when the copper fill is identical.
Both motors should perform nearly identical.
But: Lower KV is better for your esc and battery, since the amp flow is lower at the same torque produced. We want a low amp flow!

Frank
```

---
## \#962 Posted by: notger Posted at: 2017-09-20T08:37:15.820Z Reads: 365

```
does the VESC6 actually also have this ERPM Problem (worst case blown DRV) known from VESC4 with Motors above 190KV ?
```

---
## \#963 Posted by: Cobber Posted at: 2017-09-20T09:19:28.127Z Reads: 365

```
Jenso, NoWind has put 135A + through his Vesc6... for you know science... search him out dudes, burnouts and hotdog runs... Frank might need some convincing for a warranty but it has been done, by a few people now ;)
```

---
## \#964 Posted by: Brad Posted at: 2017-09-20T09:49:00.323Z Reads: 369

```
No, it can go well over 60k ERPM. Been pushed up to 120k ERPM with no issues.

No idea where the limit is.
```

---
## \#965 Posted by: stewii Posted at: 2017-09-20T17:33:21.496Z Reads: 376

```
Not sure it that was for me, but yes got a stainless steel stencil and pcb both from pcbway.
```

---
## \#966 Posted by: chinzw Posted at: 2017-09-20T17:44:28.822Z Reads: 373

```
Sk3 192kv is rated for 2.5kw
```

---
## \#967 Posted by: notepad Posted at: 2017-09-20T19:19:37.812Z Reads: 378

```
You sure.  the website says just over 4Kw

<img src="/uploads/db1493/original/3X/5/6/56a30498ee12c455e8233d9c3d4d2a5a0375a8f1.png" width="227" height="201">
https://goo.gl/n1dZ2B ( link to website )

If I am right with my Physics. Wattage is measured from Voltage * Amp   so thats 50 * 80 = 4000W or 44 * 80 = 3520W
```

---
## \#968 Posted by: Okami Posted at: 2017-09-20T20:30:46.089Z Reads: 362

```
Well I have pulled about 32-40A constant.. the motor did get quite hot (that it is hard to touch the windings with finger).. so I assume 60-70A might be possible.. though someone should check this with infra red camera or thermo-meter
```

---
## \#969 Posted by: chinzw Posted at: 2017-09-20T20:30:50.372Z Reads: 357

```
Yep, you're right, i assumed it was 6364 and not 6374
```

---
## \#970 Posted by: banjaxxed Posted at: 2017-09-20T20:53:25.201Z Reads: 362

```
150k erpm 10 chars
```

---
## \#971 Posted by: notepad Posted at: 2017-09-20T21:05:04.577Z Reads: 362

```
Safe to say then the vesc can handle the new king of sk3's then :smiley:
```

---
## \#972 Posted by: trampa Posted at: 2017-09-20T21:19:33.898Z Reads: 358

```
No, 150k erpm tested.
```

---
## \#973 Posted by: BigBoyToys Posted at: 2017-09-22T00:10:55.960Z Reads: 354

```
@trampa So I just confirmed that the 3.28fw gives me the R=0 error during foc detection using the FOC box. I can also confirm that this error does not occur using the 3.26FW with the FOC box. I thought that might be helpful for Ben to know. Thanks.
```

---
## \#974 Posted by: notepad Posted at: 2017-09-22T14:54:21.836Z Reads: 365

```
So,  I think my vesc just died.

Ive written a post on the forum (http://vesc-project.com/node/161) as it pretty long so I wont post it here.

In short, slow riding on a good day from uni. board stops responding but doesnt lock up.  vesc is fine but cant control the motor. here are some pictures https://imgur.com/a/hv5hc. vesc securely stored in a water&shockproof container)

No idea what to do so any help would be appreciated.
```

---
## \#975 Posted by: Silvio Posted at: 2017-09-22T15:48:35.102Z Reads: 365

```
Awesome man! I'm also designing my own board, can you share your altium files? 
Can't wait to see your design!
```

---
## \#976 Posted by: fedestanco Posted at: 2017-09-22T17:34:58.833Z Reads: 368

```
<img src="/uploads/db1493/original/3X/0/4/04218ea7b44afd1cfa118f1b16a7a2579857c42b.jpg" width="281" height="500">

The bluish corrosion on the directfets seems water corrosion to me.
```

---
## \#977 Posted by: fedestanco Posted at: 2017-09-22T17:36:01.828Z Reads: 366

```
<img src="/uploads/db1493/original/3X/5/9/595a437b4fac837a50cf72f01a680f916f730fed.jpg" width="500" height="333">
```

---
## \#978 Posted by: SORRENTINO Posted at: 2017-09-22T17:36:56.255Z Reads: 367

```
If its waterproof how come it looks like there is a ton of debris that got in there?
```

---
## \#979 Posted by: JTAG Posted at: 2017-09-22T17:54:14.435Z Reads: 373

```
The VESC6 is nowhere near waterproof, its just enclosed by a piece of aluminium and a PCB as coverplate. There are still enormous openings for connectors and the wiring.
```

---
## \#980 Posted by: notepad Posted at: 2017-09-22T18:21:02.040Z Reads: 376

```
@fedestanco @JTAG    The weird thing is the vesc is housed inside a custom made mount ( which is water proof ) and a custom made protective cover which is water resistant.  I can absolutly say without a doubt, no water got anywhere close to the vesc :/

Does anyone know what the Caps are made out of.  I know some of them are liquid based, could it be one might be leaking?
```

---
## \#981 Posted by: JTAG Posted at: 2017-09-22T18:40:23.023Z Reads: 382

```
I don't claim that it was liquid for outside (I just wanted to state that the VESC6 by itself is not waterproof :sweat:), in your case it indeed looks like liquid electrolyte leaked from the capacitor damaging the FET, it seamed to leaked directly into the case of the direct-FET.  The capacitor could be a faulty one or the ripple current exceeds the limits of the capacitor.

I think that Ben might be interested in analysing what happend with your unit, at least I am curious. Good luck solving the issue.
```

---
## \#982 Posted by: notepad Posted at: 2017-09-22T18:43:35.191Z Reads: 384

```
Cheers.  Lets just hope Ben can find out what happend to inform others about a possible faliure
```

---
## \#983 Posted by: notepad Posted at: 2017-09-22T21:06:19.190Z Reads: 396

```
With help from @hexakopter. It appears the capacitor is a "Wet" type cap and that is what probably caused to corrosion.  Ill contact @trampa  to check on what the next steps are going to be.
```

---
## \#984 Posted by: stewii Posted at: 2017-09-23T12:34:35.712Z Reads: 406

```
<img src="/uploads/db1493/original/3X/a/3/a33b2541a40e6720d6e2e83e849e6e43d26e7dda.JPG" width="375" height="500">

It is not yet completed, ordered the wrong package for the AD8418, but almost there. Does anyone know how to upload the firmware on this?
```

---
## \#985 Posted by: akira Posted at: 2017-09-23T12:41:13.635Z Reads: 400

```
Sweet !!
Looks nice !
```

---
## \#986 Posted by: Pimousse Posted at: 2017-09-23T12:47:44.386Z Reads: 403

```
I guess you need a STLink.
Just follow the "How to" on vedder.se (or on this forum).
```

---
## \#987 Posted by: stewii Posted at: 2017-09-24T21:57:52.719Z Reads: 399

```
Firmware uploaded, was easier than I thought. Used an STlink from ebay (connected the 4 pins VCC included and did not destroy the  LM3671 DC-DC converter). Plugged in the usb cable and vesc tool recognised it straight away. Sweet.
```

---
## \#988 Posted by: Vanarian Posted at: 2017-09-25T11:18:06.410Z Reads: 395

```
Looks quality with the directFETs, I'm looking forward to how your VESCs perform :)
```

---
## \#989 Posted by: stewii Posted at: 2017-09-25T16:59:51.020Z Reads: 389

```
Thanks. I'm looking forward too. I will post it here, but only in early October after getting back from holiday :slight_smile:
```

---
## \#990 Posted by: SilentException Posted at: 2017-09-25T18:13:44.125Z Reads: 389

```
Curious, what was the total cost of making this?
```

---
## \#991 Posted by: stewii Posted at: 2017-09-25T18:32:00.444Z Reads: 399

```
The components are about £50, it can be cheaper if you don't populated some parts like the wireless transceiver or if you order free samples from STMicroelectronics and TI. Plus the PCB. You also need a heatsink for the FETs. It is worth it considering the original price tag :)
```

---
## \#992 Posted by: SilentException Posted at: 2017-09-25T18:38:13.887Z Reads: 400

```
[quote="stewii, post:991, topic:3813"]
It is worth it considering the original price tag
[/quote]

Exactly why I asked. Still, gotta count R&D and the TM :) 
In your case, the time spent designing the PCB layout is also valuable.
```

---
## \#993 Posted by: notepad Posted at: 2017-09-25T21:42:43.244Z Reads: 390

```
Wow.  at this rate your gonna be getting many many customers.  My Vesc 6 just blew ( bad cap ) so its definitely a tempting offer if its going to be around the £100 mark!
```

---
## \#994 Posted by: marsrover001 Posted at: 2017-09-25T23:07:43.068Z Reads: 383

```
$150 And I'd still buy 2.
```

---
## \#995 Posted by: Pimousse Posted at: 2017-09-26T12:37:36.480Z Reads: 385

```
@stewii, I don't get where you got the schematics ?
I am looking carefully for them, but didn't notice that it was already released.

So if you have it, I have a (noob) electronic question for you :
One of my VESC 6 is connected via UART to an Arduino, they share GND. But I need to reference the PWM signal of a led driver to the Arduino GND. For that I have to connect battery (-) (which is Vin of led driver) to Arduino GND.
So finally I've gote : VESC GND <-> Arduino GND <-> Battery (-).

Is it something "dangerous" to have a loop like this ?
On HW4.12, VESC GND is connected to battery (-) if I'm right so should be ok, right ?

Thanks for your help (asked that on Vedder forum but no answer :confused: )
```

---
## \#996 Posted by: Dwain Posted at: 2017-09-26T12:39:20.712Z Reads: 381

```
Vesc 6.4 not connecting to pc through usb any help guys please
 dont know what to do !!!
```

---
## \#997 Posted by: Dwain Posted at: 2017-09-26T14:39:11.627Z Reads: 383

```
problem fixed bad usb ha ha so simple , i did try 2 first that did not work 3rd time lucky i guess. I bet a few people have encountered this .
```

---
## \#998 Posted by: linsus Posted at: 2017-09-26T15:49:34.487Z Reads: 388

```
Hi,

In DC applications minus is considered "GND" or ground, meaning the potential 0.

However, if your application uses minus voltages( f.e -12V) it is no longer the potential 0 anymore and not GND ( in other words an independant voltage rail).

To answer your question, no. No danger with the "loop".

//Linus
```

---
## \#999 Posted by: Pimousse Posted at: 2017-09-26T17:23:32.340Z Reads: 385

```
Thank you to confirm that !
Yes, I know about DC conventionbut as the VESC 6 was a black box (was, becayse I found schematics, thanks to @ThierryGTLTS), so I wanted to confirm there weren't no "floating" ground or something.
For instance, Vedder strongly recommends to not use PPM Y adapter because it may fry 3.3V DC/DC converter because  current may flow through GND between both VESC.
I  don't want that happening on mines. ;)
```

---
## \#1000 Posted by: akira Posted at: 2017-09-26T21:13:42.046Z Reads: 381

```
Can you share the schematics ? Or are they still kinda secret ?
```

---
## \#1001 Posted by: stewii Posted at: 2017-09-26T22:08:44.767Z Reads: 389

```
Sorry to hear that. Should be an easy fix thou if no other component is damaged. For £100 or 150 USD I might do it. But need to see if my design runs well first.
```

---
## \#1002 Posted by: stewii Posted at: 2017-09-26T22:13:25.031Z Reads: 404

```
Sounds good. But I need to test my pcb first :)
```

---
## \#1003 Posted by: stewii Posted at: 2017-09-26T22:16:14.897Z Reads: 414

```
I downloaded from here  http://vedder.se/forums/viewtopic.php?f=6&t=590&start=10

Scroll down and you  will see a PDF. Regards the rest no problem at all. Battery - is ground on vesc 6 too.
```

---
## \#1004 Posted by: akira Posted at: 2017-09-27T07:26:39.609Z Reads: 407

```
Thank you. I think I will wait for someone to share the PCB. 
Designing such a PCB is beyond my ability. I can solder it, but not design it :-)
```

---
## \#1005 Posted by: Johnonon Posted at: 2017-09-27T08:47:47.811Z Reads: 398

```
How long does it take to solder all the components to a PCB? Just curious.
```

---
## \#1006 Posted by: gogomrrobot Posted at: 2017-09-27T09:01:17.241Z Reads: 408

```
[quote="stewii, post:1002, topic:3813, full:true"]
Sounds good. But I need to test my pcb first :)
[/quote]

(a) You are doing god's work -- much appreciated.  Very curious to see how it compares against a Vesc6

(b) Don't listen to the vultures -- gimme the design, gimme the pcb, gimme, gimme, gimmie ...lol. I would just test the heck out of it and post your results first. If it's viable you should sell it for a good price that includes your hard work ;)

(c) Do you intend to design a housing?
```

---
## \#1007 Posted by: akira Posted at: 2017-09-27T10:18:59.461Z Reads: 393

```
Nice to see that opensource spirit is compared to vulture. 
I am able to help on some opensource projet and not on others. Does that make a vulture of me ? 
I do not sell anything, I build for my own ...
```

---
## \#1008 Posted by: gogomrrobot Posted at: 2017-09-27T10:40:29.015Z Reads: 388

```
Hey I wasn't being specific -- just look thru the thread, there are a lot of people asking. Also, I think BV will release the hardware reference PCB (soon maybe?) then anyone can take the BOM / Gerber files and then get then their own Vesc quoted out?

I didn't try to make this so political so quickly, also you don't know where @stewii stands on the opensource spirit of things which we cant automatically assume is everyone's belief system... maybe he wants to sell it and not do that?

He says so much here...

[quote="stewii, post:1007, topic:3813, full:true"]
For £100 or 150 USD I might do it. But need to see if my design runs well first..
[/quote]
```

---
## \#1009 Posted by: Vanarian Posted at: 2017-09-27T15:56:55.987Z Reads: 377

```
No matter what, @stewii is currently making quite the nice work. Just let the man focus on development. What comes next comes next !
```

---
## \#1010 Posted by: stewii Posted at: 2017-09-27T16:49:03.096Z Reads: 388

```
Alright guys. I never really clarify things but here it goes. I love electronics and designing PCBs. I started a fez months ago on a "replica"of VESC6  based on those schematics I shared on that link. There is only one difference which is I used an updated Motion tracking chip (MPU9250 ) instead of MPU9150, but that chip isn't populated in the original VESC 6 to my knowledge.
I won't share the Gerber files. But whoever is interested in the bare PCB  I'm happy to ship it for the roughly same price that cost me and will share BOM and stencil file. If someone would be interested in a populated PCB then I might do it, but it might take a while  depending on the number of pcbs pand on the free time I have, because even with a stencil and reflow oven it takes TIME and lots of patience.  All that assuming my design works well and performs as expected. So far I haven't test it. The missing components will arrive on the first week of October.
```

---
## \#1011 Posted by: gogomrrobot Posted at: 2017-09-27T17:07:10.281Z Reads: 394

```
[quote="stewii, post:1010, topic:3813, full:true"]
If someone would be interested in a populated PCB then I might do it, but it might take a while  depending on the number of pcbs pand on the free time I have, because even with a stencil and reflow oven it takes TIME and lots of patience.
[/quote]

Lol... dude you would get possibly hundreds of orders.  Open one of those survey polls i.e. ("Who would be interested in a fully working VESC6 alternative?") see what response you get. My belief is that it would be high... and you would need to do a production run to satisfy everyone's appetite.  Even many people who already have VESC6 would want your product to test on a second/third/x build.

EDIT:  I would be interested in (2) populated units... let me know the results from your prototype testing so I can let you take my money ;)
```

---
## \#1012 Posted by: Maxid Posted at: 2017-09-27T17:23:45.273Z Reads: 390

```
Not saying @stewii is doing anything wrong - I don't have the knowledge to do so but isn't NOT releasing the files against the VESC license?
```

---
## \#1013 Posted by: notepad Posted at: 2017-09-27T19:36:32.121Z Reads: 388

```
Not going to lie.  but I would be up for purchasing 10+ as I have loads of projects that use multiple smaller motors for power hungry tasks.
```

---
## \#1015 Posted by: DougM Posted at: 2017-09-30T00:12:18.511Z Reads: 387

```
Couple of hours if all the components are leaded.  leadless components are a bit trickier.

This is assuming you've got some strong soldering skills in your background.
```

---
## \#1016 Posted by: notger Posted at: 2017-10-07T07:32:55.550Z Reads: 385

```
[quote="trampa, post:262, topic:3813"]
Its roughly 68 x 72 x 18mm.
[/quote]


Is this still valid for the Dimension including the heatsink ?
```

---
## \#1017 Posted by: Skifree Posted at: 2017-10-07T14:46:02.048Z Reads: 405

```
I'm also curious of the exact dimensions while I wait for mine to come in. I'd like to design a milled aluminum watertight enclosure.
```

---
## \#1018 Posted by: rich Posted at: 2017-10-07T15:32:58.901Z Reads: 412

```
@notger @Skifree I measured exact dimensions: 70.87 x 74.90 x 18.15mm 
But you have to add some space to 74.90mm due to the cables. I have no idea how people manage to squeeze 2 VESC 6 in UK Ultrabox 206 (8.89 cm width) without damaging the wires. The power cables are 10AWG and as you can see on the picture there is a kind of "bending protection".

<img src="/uploads/db1493/original/3X/f/1/f1ce0ee8faa5fdfebbeee664a0c7f87fe72913c1.jpg" width="690" height="388">
```

---
## \#1019 Posted by: stewii Posted at: 2017-10-08T12:41:12.288Z Reads: 412

```
It works! There was a few little things that I needed to tweak (I already corrected them in the design for the next batch). I haven't ride my skateboard yet cause I still don't have proper heatsink / housing. Here is a quick video running on a 10S battery. [Here](https://www.dropbox.com/s/mpv994joau8kynk/1080p.mov?dl=0)
```

---
## \#1020 Posted by: MrEpiquad Posted at: 2017-10-08T14:16:13.350Z Reads: 402

```
Does someone have a download link for the New vesc tool ? 
The website seems to be down (http://www.vesc-project.com/)
```

---
## \#1021 Posted by: gogomrrobot Posted at: 2017-10-08T15:41:19.099Z Reads: 406

```
[quote="stewii, post:1019, topic:3813, full:true"]
It works! There was a few little things that I needed to tweak (I already corrected them in the design for the next batch). I haven't ride my skateboard yet cause I still don't have proper heatsink / housing. Here is a quick video running on a 10S battery. [Here](https://www.dropbox.com/s/mpv994joau8kynk/1080p.mov?dl=0)
[/quote]

That's really cool! Congrats ;)  You are the first guy with a working VESC6 alternative based on Benjamin's design. What are you going to call it? May I suggest V6ESC? Also, once you get the housing figured out... please consider going into production with it. There are many online services that can make 50-100 boards for you and alot of people on this forum including myself who would throw up money to help you place that order.
```

---
## \#1022 Posted by: marsrover001 Posted at: 2017-10-08T18:21:39.536Z Reads: 391

```
My money is ready.

Kickstarter in a month? Ship in 2 years?
```

---
## \#1023 Posted by: notger Posted at: 2017-10-08T18:49:36.129Z Reads: 388

```
[quote="gogomrrobot, post:1021, topic:3813"] May I suggest V6ESC [/quote]

Hmm, lets get creative now F**box, why not SIXESC, ESCSEX, or SEXBOX   ;-)
```

---
## \#1024 Posted by: Surfer Posted at: 2017-10-08T18:50:04.595Z Reads: 384

```
I'm in for 2! Congrats buddy!!
```

---
## \#1025 Posted by: gogomrrobot Posted at: 2017-10-08T19:54:32.253Z Reads: 390

```
Those are good names too.  Just as long as it's identifiable without infringing on Trampa rules for the naming.

EDIT: @stewii - you should put your findings/product in it's own thread I think to not hijack VESC6 thread. imho.
```

---
## \#1026 Posted by: TarzanHBK Posted at: 2017-10-09T13:53:59.578Z Reads: 388

```
gimme a SEXBOX pls!
```

---
## \#1027 Posted by: banjaxxed Posted at: 2017-10-10T08:53:18.517Z Reads: 391

```
The Sextet
```

---
## \#1028 Posted by: Vanarian Posted at: 2017-10-10T10:40:08.458Z Reads: 396

```
Keep me updated for two units price & availability shipped to France please!
```

---
## \#1029 Posted by: Pimousse Posted at: 2017-10-12T11:55:55.966Z Reads: 402

```
[quote="Vanarian, post:1028, topic:3813, full:true"]
Keep me updated for two units price & availability shipped to France please!
[/quote]

Same for me ! ;)
```

---
## \#1030 Posted by: chuttney1 Posted at: 2017-10-15T07:09:59.724Z Reads: 389

```
What's the status on the reference hardware?
```

---
## \#1031 Posted by: Yann Posted at: 2017-10-16T12:04:05.537Z Reads: 382

```
Hi,
Ready too for 2 units , shipping to France
Keep me updated for price etc😉👍👍
```

---
## \#1032 Posted by: Clonkex Posted at: 2017-10-17T21:52:03.458Z Reads: 379

```
@Chaka idk if you're reading this thread still but I thought I'd just make sure you know people are asking you to take their money :P
```

---
## \#1033 Posted by: notepad Posted at: 2017-10-17T21:55:35.140Z Reads: 373

```
@Chaka  Take my money!
```

---
## \#1034 Posted by: chaka Posted at: 2017-10-17T22:01:54.810Z Reads: 374

```
It is in the works!
```

---
## \#1035 Posted by: notepad Posted at: 2017-10-17T22:03:22.234Z Reads: 386

```
Im not actually kidding when I say, if you get the product ready in the next couple months. I will legitamately purchase 25+ units from you as Im doing a massive project!
```

---
## \#1037 Posted by: gogomrrobot Posted at: 2017-10-19T19:32:25.713Z Reads: 384

```
Guys why are @stewii flagging his content? He has a legitimate VESC based on VESC6 schematics and is taking orders.  What's up with the censoring? Myself and others are placing orders with him. His VESC matches the schematics.  I have (4) VESC6's already and love to see how they perform against his product... we shouldn't censor builders/providers like this.

If needed move this to another thread -- but flat out censoring... that's not the spirit here.
```

---
## \#1038 Posted by: SORRENTINO Posted at: 2017-10-19T19:35:26.105Z Reads: 383

```
I agree with what @gogomrrobot said.  Besides open source is open source :stuck_out_tongue_closed_eyes:
```

---
## \#1039 Posted by: longhairedboy Posted at: 2017-10-19T19:47:05.402Z Reads: 390

```
[quote="trampa, post:635, topic:3813"]
I thought you guys are DIY. Just strip off the plastic from the dam PPM plug, shrink tube the metal clips and plug in.
[/quote]

That has to be one of the worst responses from a vendor i've ever seen. 

The correct response would be "we see that presents a problem and are looking into a solution." It doesn't even matter if you really are. But don't sandwich a solution in insults. Pretend you fucking care if you don't.
```

---
## \#1040 Posted by: b264 Posted at: 2017-10-19T19:54:13.282Z Reads: 380

```
I'll have to disagree here.  I'd rather them speak their mind even if it's not what I want to hear.  Rather than feed me unadulterated bullshit
```

---
## \#1042 Posted by: Pr0dy Posted at: 2017-10-19T22:38:51.714Z Reads: 385

```
I would be down for 2 units. Keep me updated
```

---
## \#1043 Posted by: Skifree Posted at: 2017-10-20T00:58:48.896Z Reads: 385

```
Also agree, there is no need to censor here.


Edit- sensor
```

---
## \#1044 Posted by: Clonkex Posted at: 2017-10-20T02:06:38.272Z Reads: 389

```
I was like wth are you going on about until I realised you meant "censor" :grin:
```

---
## \#1045 Posted by: ThierryGTLTS Posted at: 2017-10-20T15:51:21.998Z Reads: 387

```
I think that a better place for these orders would be in the "New Items for sale" category!
```

---
## \#1046 Posted by: chaka Posted at: 2017-10-20T15:54:38.299Z Reads: 385

```
Since this is my thread I think i should have the final word on that. Its a free market, if you have vesc six developed and want to share it this is the thread to do it!
```

---
## \#1047 Posted by: notepad Posted at: 2017-10-20T16:00:47.751Z Reads: 389

```
I agree.  As much as we all love Frank, this isnt about a singular product, but instead Vesc6 and its architecture as a whole
```

---
## \#1048 Posted by: xxlv Posted at: 2017-10-20T21:40:57.989Z Reads: 387

```
Maybe because he is taking advantage of an open source project and making money without releasing his sources? I am not a lawyer :) Just guessing. But there is a scheme with vesc and open source and releasing. :) *sorry*
```

---
## \#1049 Posted by: mmaner Posted at: 2017-10-20T21:58:06.471Z Reads: 389

```
Give him some time.  Fran spent months evangelizing before they released the code.  The kool-aid is strong in this one :)
```

---
## \#1050 Posted by: JohnnyMeduse Posted at: 2017-10-20T22:03:27.481Z Reads: 400

```
They only thing he use was the schematic... the only thing he need to share is the schematic IF he had made any modification... the open source rules are different for software and hardware... Also the Hardware hasn't been release yet, so is it really open source ?
```

---
## \#1051 Posted by: stewii Posted at: 2017-10-20T22:08:13.214Z Reads: 399

```
Taking advantage of the schematics yes, why don't you make your own PCB then ?
```

---
## \#1052 Posted by: gogomrrobot Posted at: 2017-10-20T22:33:01.232Z Reads: 410

```
@stewii has offered to release the BOM (bill of materials) and stencil if you read this thread.

Anyways, if this isn't just about moving this to another thread (which it isn't as @chaka the thread originator said its OK to post about it here) then this flagging @stewii for sale of his offering accompanied by pics and videos of a legitimate product has to do with:

1) People being haters

2) Heavily entrenched interests that have products or want to bring their own VESC product to market

3) Heavily entrenched interests with regards to the owners of this forum to pick winners/losers that may be their own friends or businesses in "cahoots"

4) The above 1,2,3 only have relevance because lets face it - he who has VESC owns DIY esk8 more than anyone else

I can't think of any other reasons.  I am in no way anti-Trampa - I have $$$$ invested in them and love their products.

へ[ ᴼ ▃ ᴼ ]_/¯
```

---
## \#1053 Posted by: ThierryGTLTS Posted at: 2017-10-21T10:58:04.316Z Reads: 391

```
I wanted to calm the things, but it seems it didn't work :frowning:

Please cool down, I think (hope) everything (HW sources) will be available soon.
```

---
## \#1054 Posted by: Skifree Posted at: 2017-10-23T20:13:53.847Z Reads: 402

```
I would be willing to bet it is something like the openBCI project.
http://openbci.com/

TL;DR
It is a brain computer interface that allows you to think and then it runs through a microcontroller to give you outputs. Would be tough to have a variable control though.
```

---
## \#1055 Posted by: Giga Posted at: 2017-10-27T04:55:57.800Z Reads: 403

```
[quote="stewii, post:1036, topic:3813, full:true"]
I am ready to take orders. PM me.
[/quote]

I got no idea how to PM you, since there is no button next to your name. But I'd like to have one.
```

---
## \#1056 Posted by: vishal_tejwani Posted at: 2017-10-27T06:13:36.898Z Reads: 395

```
Hey do you have vesc6 pcb designs?
```

---
## \#1057 Posted by: SpeedyGonzales Posted at: 2017-11-01T21:53:19.000Z Reads: 390

```
I would like one please.
```

---
## \#1058 Posted by: Maxid Posted at: 2017-11-04T16:08:45.193Z Reads: 401

```
Is there any news on the reference design by vedder? It's been a couple months since launch and I'd like to see the stripped down versions frank was talking about. I have no need for NRF for example and would love some focbox-price-level Vesc6s
```

---
## \#1059 Posted by: gogomrrobot Posted at: 2017-11-04T16:54:09.888Z Reads: 411

```
They aren't incentivized to release it quickly... for all we know maybe BV is splitting his time fixing bugs... I see a lot of firmware releases. 

@stewii is making gr8 progress on shipping out his first units... cover will be white not yellow.

<img src="/uploads/db1493/original/3X/8/4/840d2b86ed01da5870edf2ae40aea5520fe9e087.JPG" width="375" height="500"> 

There are people who like him who are using the schematics that have been released to create their own for now until we get the reference design.
```

---
## \#1060 Posted by: luis99945 Posted at: 2017-12-25T02:25:24.671Z Reads: 358

```
hello i need 2
```

---
## \#1061 Posted by: gogomrrobot Posted at: 2017-12-25T02:35:56.967Z Reads: 362

```
Luis you can't just randomly get on the site and start pm'ing people who don't sell things to sell you those things.

Here bud let me help you out :slight_smile:

@stewii Vesc6 clone 
@trampa Vesc6 original (trampaboards.com)

If you need bms... you need go to batterysupports.com or lucy @   http://bestechpower.com

any other thing you need?
```

---
## \#1062 Posted by: H_man Posted at: 2018-02-04T08:36:28.310Z Reads: 331

```
Can a 2.4Ghz RC remote be used with the vesc 6 as it was used with the vesc 4?
```

---
## \#1063 Posted by: rich Posted at: 2018-02-04T09:05:29.467Z Reads: 339

```
Yes of course, the only difference is that you need a 3pin JST-PH cable with 2mm pitch and female connector to connect the receiver. In my case I soldered it directly to the receiver but you can solder or buy an adapter cable.

![20180204_100244|690x388](upload://j92uiTFSBLMijXSkHKZK8Fjh1Pc.jpg)
```

---
## \#1064 Posted by: H_man Posted at: 2018-02-04T09:23:19.447Z Reads: 334

```
Thanks dude!
```

---
## \#1065 Posted by: WrinklyWink Posted at: 2018-02-12T21:57:42.118Z Reads: 332

```
So, is it just me or am I the only one getting frustrated by the VESC 6?
First, my vesc tool has different firmware versions between operating systems (3.27 for windows) (3.32 for linux)
When I load up either of the vesc tools, it says theres an update.. to go to the website. But on the website there isn't any update! however you can see that the "vesc platinum" was updated at the mid of the year 2017, but the others haven't been touched since 2016. Anyone else notice this? So I guess I should just ignore the update notice? that a strike on vedder. because there is literally no quick way of telling which version is what. Like all the zips are labeled the same and it shows purchased date but not updated date. I don't know if  my problem is isolated to a software or hardware because of this lack of date records.
What is the latest update for the vesc_tool? And are there differences in these updates between windows and linux?
Then theres the STLink. Had to modify the one which worked on the last vesc in order to work with this one.
Then theres the over voltage fault. in other words. I check the battery and its at 48.1 volts. however when I look at the real time data. it says its at 61.7 volts. why? if the voltage isn't the right one, is it a hardware fault or a software fault?
then out of the 2 I ordered the other one of them worked for maybe a minute before status lights never came on again. I smelled something burning so I quickly shut it off. <s>I think I got a lemon. thats a strike for trampa.</s> I already messaged Trampa.. about a warranty. But is there even a warranty? I mean these vescs have never left the house yet ones burning up and the other is giving me a wrong voltage.
I find it hard to believe that because I'm getting issues with 2/2 of the vescs I received, that I'm the only one. Has anyone had issues setting up like these?
Anyone get it fixed promptly?

Hardware version V6.41

UPDATE: Trampa contacted me and we discussed back and forth. Strike striked out because we narrowed it down to a notice issue. Notice was about installing an ubuntu environment and immediately connecting an STLink for firmware update without notice of the 3.3v voltage injection issue.
```

---
## \#1066 Posted by: JohnnyMeduse Posted at: 2018-02-12T22:11:36.025Z Reads: 326

```
The 57v could be related to hardware issue, if it calculates in the same way as on the 4,12. And before it burn have you been able to connect your vesc to the PC, because I think you burn the DRV you also lost the ability to connect to a pc (I’m still not sure about that)
```

---
## \#1067 Posted by: WrinklyWink Posted at: 2018-02-12T22:34:57.124Z Reads: 322

```
i have 2 vescs. one shows 61.7v and the other I'm pretty sure burned out. Thanks for responding
```

---
## \#1068 Posted by: JohnnyMeduse Posted at: 2018-02-12T22:38:03.720Z Reads: 314

```
Where are you located?
```

---
## \#1069 Posted by: squad Posted at: 2018-02-12T22:43:07.490Z Reads: 318

```
Get in touch with Frank @trampa I'm sure he'll help You out.
```

---
## \#1070 Posted by: GrecoMan Posted at: 2018-02-12T22:54:44.894Z Reads: 314

```
Johnny the legend can probably fix it

@JohnnyMeduse
```

---
## \#1071 Posted by: trampa Posted at: 2018-02-12T23:26:13.427Z Reads: 322

```
Hi WrinklyWink, I mailed you as soon as I received your mail. You got a response within less than a day.

You should always download the latest file from The VESC-Project.com website.
In fact you can't download old versions, no matter of the date of "purchase".
The download will always be the latest VESC-Tool having the latest FW aboard.
There where plenty of updates last year!
Please update the VESC and see if the Voltage is still calculated funny/wrong.
I will also ask Benjamin about this issue. 

Frank
```

---
## \#1072 Posted by: WrinklyWink Posted at: 2018-02-13T00:56:07.955Z Reads: 305

```
nyc
10 characters
```

---
## \#1073 Posted by: JohnnyMeduse Posted at: 2018-02-13T04:09:40.645Z Reads: 301

```
Nice, well as @GrecoMan said if you can't get help from trampa I can probably fix them for you.
```

---
## \#1074 Posted by: ThermalM16 Posted at: 2018-02-13T04:18:44.529Z Reads: 304

```
@WrinklyWink send me one and send the other to @JohnnyMeduse then we can race to see who can repair them first :joy:
```

---
## \#1075 Posted by: JohnnyMeduse Posted at: 2018-02-13T04:20:19.609Z Reads: 306

```
Do you really wanna bet... because guess who's doing repair for enertion support :sunglasses:

Edit: Sorry I had badly express myself FocBox repair only for Enertion
```

---
## \#1076 Posted by: ThermalM16 Posted at: 2018-02-13T04:24:31.750Z Reads: 305

```
Oh yeah well I do repairs for people and stuff too :man_mechanic:
```

---
## \#1077 Posted by: ThermalM16 Posted at: 2018-02-13T04:27:52.192Z Reads: 306

```
Also you should tell enertion I'm cool and they should hire me so I can get cool equipment and be forced to test Raptor 2's occasionally :wink:
```

---
## \#1078 Posted by: JohnnyMeduse Posted at: 2018-02-13T04:51:42.986Z Reads: 312

```
![image|568x335](upload://2wkFSjeIISco9Ttcu6QNIezjNrt.jpg)
```

---
## \#1079 Posted by: ThermalM16 Posted at: 2018-02-13T05:37:56.929Z Reads: 310

```
...except for me :sunglasses:
```

---
## \#1080 Posted by: trampa Posted at: 2018-02-13T12:11:35.440Z Reads: 304

```
I would say dead voltage regulators and dead STM due to 3.3V SWD-Port injection from ST-LINK V2. 
The internally shortened STM32 heats up and starts to smell in consequence.
Should be quite easy to fix if no other parts fried as well. 

Frank
```

---
## \#1081 Posted by: fedestanco Posted at: 2018-02-13T12:18:36.856Z Reads: 300

```
Hi, do you have a rough idea on the release date of the reference pcb files?
```

---
## \#1082 Posted by: trampa Posted at: 2018-02-13T12:27:31.511Z Reads: 298

```
http://vesc-project.com/node/311

Frank
```

---
## \#1083 Posted by: akira Posted at: 2018-02-13T12:43:30.072Z Reads: 294

```
I don't see the answer to that question in the link. Can you be more specific ?
```

---
## \#1084 Posted by: stewii Posted at: 2018-02-13T13:02:54.283Z Reads: 291

```
Short answer: they won’t release
```

---
## \#1085 Posted by: JohnnyMeduse Posted at: 2018-02-13T14:01:25.760Z Reads: 297

```
It could be, If the DRV is badly soldered the reference point for the Buck is offset and the voltage could higher than 5.5 which is more than the step-down can take.
```

---
## \#1086 Posted by: Pimousse Posted at: 2018-02-13T15:36:47.413Z Reads: 311

```
Check what BV said on [vesc-project.com forum](https://vesc-project.com/node/306) :

> A short summary:
    The VESC firmware and VESC Tool are and will stay open source.
    The VESC 6 schematic is open source, and available on the hardware documentation page along with other open hardware designs.
    The VESC 6 layout and gerber files will not be released to the public, for reasons explained in the hardware page.
    A complete 3 shunt reference layout kicad project, very similar to the VESC 6, will be released as soon as I have time.
```

---
## \#1087 Posted by: akira Posted at: 2018-02-13T16:19:47.861Z Reads: 301

```
Trampa said many times here that a reference design would be published ... with the PCB gerber. Or am I mistaken ?
```

---
## \#1088 Posted by: Pimousse Posted at: 2018-02-13T16:38:25.846Z Reads: 298

```
VESC is a trademark of Benjamin Vedder.
VESC project is owned by Benjamin Vedder.
Whatever Trampa could have said, the final word belongs to Benjamin Vedder. ;)
```

---
## \#1090 Posted by: trampa Posted at: 2018-02-13T17:07:54.919Z Reads: 309

```
As Pimouse pointed it out, Benjamin will do a KiCad project, very similar to VESC 6. If you need the Gerbers, KiCad will spit them out for you after you have tuned your piece of hardware to your needs.

As Benjamin described, It is well worth learning KiCad, making your own layouts from the schematics that are public.  
A lot of people have done that already and in future we will see more different hardware, rather than boring copy paste projects. It is not easy to find a good compromise between stipulating Innovation and being 100% OS on the hardware side. OS hardware is problematic, since a 100% copy paste product will end in cheap and likely poor quality products, unhappy customers, unnecessary electronic waste and negative effects on the Project Brand itself. 
If you don't understand the Hardware, how can you control the quality? If you understand it, you can design your own PCB with ease anyway.  
If someone wants to make hardware, he should put some effort into it and offset it from the competition, offering a set of USPs, or versions that are more specific for a certain application. If you simply copy a design and try to push sales, battling for the lowest price, quality will ultimately suffer. Quality is also in the field of project support, customer support, warranty, product availability, meeting standards etc. A lot of discount vendors don't offer any of those services/requirements to get the price down to a minimum. 

All of this is the reason why Benjamin did a write up, posted on the VESC-Project.com website.
It is not easy to find the best balance between being OS and stipulating innovation and product variety. 

Frank
```

---
## \#1091 Posted by: gogomrrobot Posted at: 2018-02-13T23:44:34.076Z Reads: 311

```
Something something... pants on fire?

![2018-02-13 (2)|564x499](upload://AhDdQzK6tVynsHSGtOiQb2cfpij.png)
```

---
## \#1092 Posted by: PXSS Posted at: 2018-02-14T00:27:51.278Z Reads: 299

```
He's minutes away from releasing it... just you wait /s
```

---
## \#1093 Posted by: Whitehawk Posted at: 2018-02-14T11:46:02.648Z Reads: 305

```
Just burned a focbox, I need new ESC more powerful, so we have : 
- focbox 140€
- stewii vesc6 clone 170€
- trampa vesc6 300€

What else ? stewii's vesc6 is the best  ? or we will have something else cheaper soon ?
```

---
## \#1094 Posted by: Nordle Posted at: 2018-02-14T12:52:22.407Z Reads: 305

```
Probably not much cheaper, components do also have their cost.
```

---
## \#1095 Posted by: anorak234 Posted at: 2018-02-14T22:27:37.580Z Reads: 304

```
FOCBOXs are slow on production, and trampa's VESC6 is vastly overpriced. I just ordered from @stewii considering his units have been good so far, using the exact same components as trampa with better pricing
```

---
## \#1096 Posted by: Deckoz Posted at: 2018-02-14T22:39:20.700Z Reads: 310

```
If your so cool how do you reflow...


Jk lol
```

---
## \#1097 Posted by: JohnnyMeduse Posted at: 2018-02-14T22:42:18.771Z Reads: 313

```
![image|225x225](upload://iiLi5eqsSiFL72p1rDFmXJyYZvU.jpeg)
```

---
## \#1098 Posted by: WrinklyWink Posted at: 2018-02-16T01:55:04.416Z Reads: 306

```
Lol so this Topic is between ppl who have issues and those who want the secret plans to the lair.
I'm kidding.
wait maybe not so much, ... .. .

Offers on the table. I'm all for using less resources so I'm going to go the repair route. But the generosity is noted @trampa.
If @ThermalM16 is serious I might actually consider what he's offering. @JohnnyMeduse 
I mean think about the logistics we can learn from this. We can make this a team effort. I can ship them off at the same time at a time we agree on and see how long it takes to reach each of you. And then we can do a sync unboxing, with a not a rush but more like a genuine competitus between you two.
```

---
## \#1099 Posted by: WrinklyWink Posted at: 2018-02-16T02:08:00.727Z Reads: 299

```
@Trampa, I really wanna like the vesc 6 but at its top-tier price, it needs to have a top-tier manual. This why there are vigilantes looking for batman's cave. When I buy a pc motherboard for the same price it comes with a thick manual of all it's chips, the explanation for their purposes, the voltages allowed, the logic pathways, the temperature data sheet, and then my favorite, an explanation of the particular apps the motherboard allows for. If people truly knew how to compile for your "mobo" there wouldn't be so much exclamation for the reference design. Also. i think its kinda funny vedder isn't on these forums. is he an introvert? lol
come on. a nice thick manual. like quality. ya know? then i think your vescs will "fly" off the shelves. (they're on shelves right?)
```

---
## \#1100 Posted by: ZackoryCramer Posted at: 2018-02-16T02:11:51.150Z Reads: 290

```
[quote="WrinklyWink, post:1099, topic:3813"]
thick manual of all it’s chips
[/quote]

You actually read those?! I don’t know about you but I wouldn’t want to buy a $300 vesc just because it comes with the manually that explains the nitty gritty.
```

---
## \#1101 Posted by: Pimousse Posted at: 2018-02-16T07:55:31.245Z Reads: 298

```
I second @WrinklyWink about documentation.
VESC 6 is meant to be used in a wider scope of application than only e-skate.
But today, if you want to integrate the VESC into your application, you have to reverse-engineer the firmware source code.
For instance, there is NOTHING about the UART protocol !
Even the VESC 4.12 was more detailed ( http://vedder.se/2015/10/communicating-with-the-vesc-using-uart/ ).

I even discovered while reading the source code that the number of red led flashes tells you exactly which fault has been triggered.
This is so useful and it could have helped a lot of guys instead of telling them "don't power off, connect vesc/bldc tool and type faults in terminal"...

IMO, B. Vedder doesn't need to come on this forum wasting his time to read complains against one or the other.
Vedder has to focus on his project, not about all the mess surrounding it (Trademark stuff, FOCBOX, derivative discussion, lie or not lie...).
We definitely miss him on the vesc-project.com forum to answer questions about real contributions. :confused:
```

---
## \#1102 Posted by: Maxid Posted at: 2018-02-16T09:34:39.312Z Reads: 291

```
There is also @esk8's own modified VESC that is supposed to be more robust than a Focbox. It's sad to see these not being more frequently considered - they seem to be well made and have only good reviews so far
```

---
## \#1104 Posted by: trampa Posted at: 2018-02-16T09:49:59.247Z Reads: 309

```
The VESC-Project is an OS-Platform, and the amount of work is tremendous.
Before the Project started there was no controller like that available at all.
It is a given Horse! Documentation is coming together bit by bit and it is pretty much an endless job to do. Remember that Benjamin is doing all this in his time off, after work!
If funding will get to level, where it generates enough to fund his life, that is a different game then.

The VESC is also no product that is made by the millions, unlike mother boards and graphic etc. cards.

Before sending the devices, we opened up a forum and made some sticky threads containing very useful information about what not to do, and how to upgrade the FW and upload missing bootloders etc. We sent every customer a mail (together with the login) to be sure that the most critical information is passed over and the customer is informed about issues with Clone ST-Links, HM-10 modules and the like.
Benjamin added a lot of information into VESC-Tool itself. There is a ? behind nearly every setting you can change. That is a big fat manual inside the software itself.

The VESC is an advanced piece of hardware and the VESC-Tool an advanced piece of OS-software. You can use it on all levels of personal experience. You can configure it manually all by yourself, or simply use the wizards.

A striped down mobile version will be available in future. Tuning your VESC will become very easy and user friendly. You will even be able to upload the latest firmware through your mobile phone/tablet.

I know that it is frustrating to deal with a damaged device. Since we know what caused the issue (SWD 3.3 V injection), I am sure that it can be fixed with ease.
This is why I got you in touch with the DRV-Wizard and put together a list with the electronic parts numbers etc. You could also sell the VESCs cheap to someone with electronic experience, someone who can fix them and use our 50% discount code to get some new ones. Plenty of options on the table…

Frank
```

---
## \#1105 Posted by: trampa Posted at: 2018-02-16T09:52:31.924Z Reads: 292

```
And being printed on a lot of paper, the rain forest killer No1.

Frank
```

---
## \#1106 Posted by: b264 Posted at: 2018-02-16T09:54:02.680Z Reads: 293

```
[quote="trampa, post:1105, topic:3813, full:true"]
And being printed on a lot of paper, the rain forest killer No1.

Frank
[/quote]

Actually, cars and coal power plants are the rain forest killers...  VESC actually helps them by slightly reducing car numbers.
```

---
## \#1107 Posted by: trampa Posted at: 2018-02-16T10:11:17.766Z Reads: 297

```
A lot of people with e-bikes and e-boards have their cars standing around a lot more time of the day. I hope that the VESC-Project helps to improve the situation a tiny little bit. 

Paper is still one of the biggest forest killers. We use to much paper! I recently bought a mixer and it came with 1KG of manuals in 16 languages. Ridiculous! All you need is a shot code with a link to an online documentation. 

Frank
```

---
## \#1108 Posted by: Pimousse Posted at: 2018-02-16T11:33:09.080Z Reads: 301

```
WWF stuff are off topic.
What about documentation ? I mean real documentation, not forum thread or email.
PDF files and websites exist, no need to cut tree...

[quote="trampa, post:1104, topic:3813"]
Remember that Benjamin is doing all this in his time off, after work!
[/quote]
So we, DIY guys, **all** do !
I'll write a UART protocol article, but where to submit it ? Forum ?
Which one ? Vedder.se ? Vesc-project.com ? Both are active.
I'll be glad to contribute, but I can't since I don't have any answer on the forums since 3 weeks to a VESC Tool bug report.

The point is that contribute to VESC Project seems to be complicated...
```

---
## \#1109 Posted by: trampa Posted at: 2018-02-16T11:38:05.318Z Reads: 302

```
I think Benjamin will gladly give you access to the documentation pages, so that you can drop it there and edit it there . Benjamin was travelling for two weeks and got the quite i'll last week. That's life....

Writ it up, and we we will find a nice spot to put it and you will be able to access it.

Frank
```

---
## \#1110 Posted by: Pimousse Posted at: 2018-02-16T12:56:08.272Z Reads: 300

```
Frank, it's not about **ME**.
It's about finding a **sustainable** way for the whole project to gain more contribution, manage and integrate them.
Several pull requests are still waiting for approval.
People who did them spent time off as well to contribute.

But ok, I'll write something about UART.
```

---
## \#1111 Posted by: rpasichnyk Posted at: 2018-02-16T16:19:46.905Z Reads: 300

```
Yes, [my pull request](https://github.com/vedderb/vesc_tool/pull/8) is waiting very long time, I submitted it more than 4 months ago. I bumped it and hope Benjamin will find time to have a look :+1:
```

---
## \#1112 Posted by: esk8 Posted at: 2018-02-17T06:48:46.002Z Reads: 307

```
Thank you @Maxid that you remember thats we have redesigned the Vesc too.
We have working in the last month´s very hard on new projects and on the 
esk8 1.2 controller, some thing we have changed on the PCB and one component
is coming new on the PCB.
Now you can connecting a LCD Voltage battery indicator with the esk8 1.2 controller.
So that you don't must soldering the cable from the LCD.
Then we have modernized our CNC milling machine, and we hope that we can
now producing the cases for the controller myself.
That was extreme important for the Price.
Next week i became the new 1.2 PCB and then i opening a new tread 
about the esk8 1.2 controller with pictures and new lower prices.

Regards Attila
```

---
## \#1113 Posted by: PXSS Posted at: 2018-02-17T15:02:34.127Z Reads: 294

```
[quote="trampa, post:1105, topic:3813"]
And being printed on a lot of paper, the rain forest killer No1.
[/quote]
Wait a second... you're now worried about rainforest?
Weren't you the one saying that @longhairedboy and company needed to print out the terms of GPL and ship it with every esc sold??
```

---
## \#1114 Posted by: WrinklyWink Posted at: 2018-02-17T15:56:12.222Z Reads: 299

```
could calculate the price of a manual printed, but still offer the manual as a pdf. For those who want it printed it could be added on in the cart..
```

---
## \#1115 Posted by: trampa Posted at: 2018-02-18T16:48:41.126Z Reads: 304

```
I was the one saying you should send an email containing the information about the GPL, so that customer knows the device contains GPLed FW and where to get access to the source code. If you don't want to send emails, you have to print the info onto paper, which is stupid (rain forest wise).

Frank
```

---
## \#1116 Posted by: banjaxxed Posted at: 2018-02-19T12:28:10.629Z Reads: 328

```
@chaka I know you don't frequent these parts anymore but perhaps you would care to share the gerber for your direct fet mod, I think you indicated you were going to do that but failed to find it anywhere (oshpark gives a 404 not found)

http://www.electric-skateboard.builders/t/v4-12-direct-vesc-ollinboardco/13104

Since things have moved on, it may not be the IP it once was
```

---
## \#1117 Posted by: lock Posted at: 2018-02-19T23:25:07.452Z Reads: 325

```
Just something I stumbled on in a random internet search...

The [A200s](http://www.fightingrobots.co.uk/threads/13621-300a-vesc-in-the-works-feature-suggestions-wanted) is a 18s 200a VESC.

![image|281x499](upload://en6oa9UWd9NmujpeLP7eDw1o0PZ.jpg)

Probably overkill, but still interesting.
```

---
## \#1118 Posted by: Riako Posted at: 2018-02-20T01:09:09.247Z Reads: 313

```
Probably yes ! So,.. neeeeeded :smile: for ebike, ekart or e-toxx !!!
```

---
## \#1119 Posted by: chuttney1 Posted at: 2018-02-20T04:05:20.246Z Reads: 310

```
I took a look at it. They are on the battle bots forum.
```

---
## \#1120 Posted by: E1Allen Posted at: 2018-02-20T04:09:40.376Z Reads: 307

```
That vesc is killer.  Think about 18s board🤔
```

---
## \#1121 Posted by: Exiledd_Top Posted at: 2018-02-20T04:12:32.727Z Reads: 311

```
It would be possible but it would be like reinventing the wheel most motors only can get fed so many amps and only go up to 12s new motors (bigger) and bigger motor mounts unless u use it but only rum 12-13s
```

---
## \#1122 Posted by: telnoi Posted at: 2018-02-20T06:38:57.951Z Reads: 314

```
Would already help if it doesn't overheat like the focbox after a 5 minute off-road climb. Not sure if the vesc6 would fair better.
```

---
## \#1123 Posted by: Riako Posted at: 2018-02-20T09:39:55.751Z Reads: 321

```
Yes, they're some people who actualy could be needed this on their board :smile:
http://www.skate-the-planet.com/images/reviews/worldsBiggestSk8.jpg
http://3.bp.blogspot.com/_qoJr7kKgahs/TDruZCmWeaI/AAAAAAAAA5U/ys368eg7j9k/s400/Worlds-Largest-Skateboard-01.jpg
```

---
## \#1124 Posted by: Kug3lis Posted at: 2018-02-20T12:58:36.724Z Reads: 314

```
Freaking 15kW continues... Mother of god this is beast :D
```

---
## \#1125 Posted by: Kug3lis Posted at: 2018-02-20T13:01:35.566Z Reads: 325

```
Damn I feel like someone took my idea....

![54 PM|271x500](upload://bEjjxYAkwkZoufGtqrnzvdPvOHe.jpg)

![06 PM|275x500](upload://7MpPKLdCW3o4DUgVBxFkeKVaU3h.jpg)
```

---
## \#1126 Posted by: banjaxxed Posted at: 2018-02-20T13:03:07.212Z Reads: 311

```
What are the specs don't be a tease
```

---
## \#1127 Posted by: Kug3lis Posted at: 2018-02-20T13:04:32.735Z Reads: 315

```
I mean even the MOSFET driver IC, current sense resistors are at the same position :D

The same specs basically same mosfets so around 15kW continues :D
```

---
## \#1128 Posted by: Blitz Posted at: 2018-02-20T13:06:03.497Z Reads: 317

```
@Kug3lis Could you see that Vesc used In the worlds fastest Esk8?
```

---
## \#1129 Posted by: banjaxxed Posted at: 2018-02-20T13:06:32.544Z Reads: 316

```
Pcbs, populated pcbs, cases tbd on 3dservisas?
```

---
## \#1130 Posted by: Kug3lis Posted at: 2018-02-20T13:06:39.692Z Reads: 315

```
Apart MCU program its not vesc anymore ;)
```

---
## \#1131 Posted by: Blitz Posted at: 2018-02-20T13:08:42.924Z Reads: 313

```
Ok fully off topic Question If someone Gave you 5k and told you to make the worlds fastest esk8 could you do it. And would you consider the esc?

Edit: Question was pointed at @Kug3lis
```

---
## \#1132 Posted by: Kug3lis Posted at: 2018-02-20T13:11:49.485Z Reads: 321

```
Lol 5k would not even be enough for that kind of stuff ;) But if I was going to do something really high power, I would just buy 3 phase bridge mosfets blocks which are 800A each and 2k$/ea and just drop some other shit :)
```

---
## \#1133 Posted by: Kug3lis Posted at: 2018-02-20T13:15:29.968Z Reads: 324

```
Ok he started way earlier and just came to same conclusions as me so its not copy :D I went a step down and did smaller version, will be ordering pcbs next week try out if it works will be cool :) It would be smaller version of that beast, same mosfets, no DRV and etc.

I am just curious how the hell he steps down 75V to 3.3V as I don't see any buck converter apart small LDO's :D
```

---
## \#1134 Posted by: Pimousse Posted at: 2018-02-20T14:02:41.104Z Reads: 322

```
[quote="Kug3lis, post:1133, topic:3813"]
I am just curious how the hell he steps down 75V to 3.3V as I don’t see any buck converter apart small LDO’s :smiley:
[/quote]

Are you planning to copy him ? :smile:
```

---
## \#1135 Posted by: Kug3lis Posted at: 2018-02-20T14:47:25.732Z Reads: 321

```
I have no need for 15kW continues current drive :D So I am just making my VESC style ESC with just 6 mosfets ;) It will be VESC compatible but I will not run VESC :D
```

---
## \#1136 Posted by: Pimousse Posted at: 2018-02-20T14:53:31.636Z Reads: 336

```
[quote="Kug3lis, post:1135, topic:3813"]
It will be VESC compatible but I will not run VESC
[/quote]

Why ?
10char
```

---
## \#1137 Posted by: Kug3lis Posted at: 2018-02-20T14:56:33.631Z Reads: 336

```
One thing is compatibility with other things I am working on second, there are some features which I do not like for e.g in new firmware version brakes are not really good so if you stand on hill it will not hold it :D When in 2.** version worked fine :)
```

---
## \#1138 Posted by: Pimousse Posted at: 2018-02-20T15:09:24.491Z Reads: 342

```
I'm riding a MTB with dual VESC quite uphill (ski slopes), never had something to say about the brakes.
And the 3.xx is wayyy better about switching from backwards to forward.

However, if you detect a bad behaviour and know how to fix it, feel free to send a pull request and thus spray the improvement to ALL the VESC users.

This is the power of open source project. ;)
```

---
## \#1139 Posted by: JTAG Posted at: 2018-02-20T16:01:47.656Z Reads: 346

```
https://www.vesc-project.com/node/228
```

---
## \#1140 Posted by: eSkateNorway Posted at: 2018-03-03T20:01:47.390Z Reads: 344

```
Hey,

Can I use a FOCBOX pared with a Vesc 4.12 (can bus) for a dual drive? I already have a Vesc 4.12 and just started on a dual drive project.
```

---
## \#1141 Posted by: b264 Posted at: 2018-03-03T20:10:50.012Z Reads: 337

```
[quote="Pimousse, post:1138, topic:3813"]
send a pull request
[/quote]

What repository/branch are you pulling this from?
```

---
## \#1142 Posted by: Pimousse Posted at: 2018-03-03T22:10:37.078Z Reads: 341

```
The official one : 
Github.com/vedderb/bldc
```

---
## \#1143 Posted by: b264 Posted at: 2018-03-04T00:08:40.165Z Reads: 338

```
That's the one that hadn't been merging pull requests.  I thought maybe there was another fork that people were working on.  Nobody is going to contribute if they see that nothing gets merged.  I do see there was activity 4 days ago though
```

---
## \#1144 Posted by: Pimousse Posted at: 2018-03-04T05:34:13.445Z Reads: 345

```
Yes Vedder got active this week and merged several pull requests, mine includdd.
I keep thinking that contributong through the offical repository is the way to go.
Otherwize we see unofficial branch gettinh popular (ie Ackmaniac) and it's the mess to follow.
```

---
## \#1145 Posted by: b264 Posted at: 2018-03-04T05:36:41.763Z Reads: 357

```
[quote="Pimousse, post:1144, topic:3813"]
I keep thinking that contributong through the offical repository is the way to go.
[/quote]

It's definitely the way to go -- IF (and only if) the repository is maintained, which, until 4 days ago, it was not

I'm glad to see this.  Still weary he will go dark again.  He needs to give someone else commit access then the official repo would be king.  Ask him...
```

---
## \#1146 Posted by: Pimousse Posted at: 2018-03-04T05:43:08.086Z Reads: 365

```
I already complain to Frank on this thread (Vedder.s VESC 6), but as usual, Frank didn't answer anything (or the answer is far away from the question).
But yes, this project can't rely only on Vedder's shoulders.
```

---
## \#1147 Posted by: scepterr Posted at: 2018-03-05T00:59:49.470Z Reads: 361

```
Found the kicad a while back
https://www.electric-skateboard.builders/t/uniqueego-dual-diag-160kv-10s-vesc4/30774/33
```

---
## \#1148 Posted by: WrinklyWink Posted at: 2018-04-02T21:52:49.962Z Reads: 342

```
I've searched the query: "update firmware vesc 6" and only got the old stuff.
my vesc6 firmware is 3.34. my vesc_tool is 0.91 for windows. when connected it says to update firmware. so I upload a firmware wait 10 seconds restart but it still holding the latest firmware. what do I do?
```

---
## \#1149 Posted by: banjaxxed Posted at: 2018-04-02T22:13:08.626Z Reads: 342

```
Well I'll be dipped in dogshit, thank you
```

---
## \#1150 Posted by: WrinklyWink Posted at: 2018-04-04T02:45:28.961Z Reads: 341

```
nvm, found the answer here: https://vesc-project.com/node/47
issue was bootloader needs to be uploaded before firmware upload.
there really should be information added to the after-the-firmware upload pop up that explains a non-sticking updated firmware needs a bootloader uploaded first. its intuitive thinking that the firmware is needed before a bootloader because the tabs are arranged accordingly.
```

---
## \#1151 Posted by: Charles_Chan Posted at: 2018-05-18T20:40:58.860Z Reads: 319

```
Is it vesc 4? Is it riding on 100A? if yes, would you help to share the setup on vesc tool to me. I want to setup my vesc 4  accroding it. thanks
```

---
## \#1152 Posted by: Gaza65 Posted at: 2018-06-17T04:18:33.443Z Reads: 291

```
Im building a quad and need 4 vesc6 so watching with interest...
```

---
## \#1153 Posted by: SammiHuangabc Posted at: 2018-07-12T06:11:08.594Z Reads: 274

```
Veder is great, but it's a little expensive. Now a Chinese company named flipsky also make ESC6 Base on VESC6. Much cheaper.
```

---
## \#1154 Posted by: Surfer Posted at: 2018-07-12T06:47:58.069Z Reads: 274

```
Much shitier I would say
```

---
## \#1155 Posted by: SammiHuangabc Posted at: 2018-07-12T06:55:56.173Z Reads: 271

```
Did you have bad experience from them?
```

---
## \#1156 Posted by: DeathCookies Posted at: 2018-07-12T13:53:48.108Z Reads: 269

```
Well why should it be bad? because it is not by vedder who mostly refuses pull requests?

They use more mosfets, upgraded components, ... I dont know if it is pure advertisement but it seems better to me than a vesc 6
```

---
## \#1157 Posted by: rpasichnyk Posted at: 2018-07-12T14:20:44.289Z Reads: 267

```
Please do not be harsh on Benjamin. It is not as simple as it might look to maintain such a big project. One has to be patient with pull request and be prepared it doesn't always gets accepted. I agree this can be disappointing at times though.
```

---
## \#1158 Posted by: DeathCookies Posted at: 2018-07-12T14:36:21.768Z Reads: 276

```
Lol. He refuses Pull requests about Watt control and then He makes a new Version with new Features about Watt controll. My only concern is that he did not mention that these Features already exists due to other members. It seems as He just claim the work by him self. 

I do not say that he had made a bad product or He has not deserve some honor but to me it seems as He Tales glory of everything good
```

---
## \#1159 Posted by: Pimousse Posted at: 2018-07-12T14:46:44.847Z Reads: 283

```
I can understand @DeathCookies 's point about the pull requests (even I don't totally agree with it).
Because it's a big project which can't rely on a single (super)man shoulders, delegation/collaboration is the way to go, isn't it ?
There are a few old pull requests which can be close now, others can be merged as it's only minor compilation stuffs.

From my point of view, having a pull request opened since a while is even more frustrating than having it rejected for some reasons.

[quote="DeathCookies, post:1158, topic:3813"]
I do not say that he had made a bad product or He has not deserve some honor but to me it seems as He Tales glory of everything good
[/quote]

Defo not agree with that.
He's claiming NOTHING.
Example :
I asked for a NRF power off feature, Trampa told me that was useless.
I coded it, made my pull requests which was merged few hours later (and my BLE dropouts were fixed :relieved:)
So, that proves that even if it's not coming from Vedder himself, new features are welcome ! :slight_smile:

But letting people collaborate though pull requests and not having a look at those doesn't comply with the OS spirit Vedder and Trampa are claiming.
For this, I'm agree.
```

---
## \#1160 Posted by: trampa Posted at: 2018-07-12T15:06:10.556Z Reads: 267

```
Easy easy. Benjamin is quite stressed out at the moment. He is finishing his PHD and you can imagine that there is only a certain amount of time. Sometimes life is a bit to full to be able to please every request.
Things move forward, but at the very moment a bit slower. 

And BTW: Benjamin never implemented a Watt controll. His opinion about it is very clear!
He bangs on something much better, but that needs more attention and is a bit tricky to implement.
Once nailed this will be the mode everyone will use.

Frank
```

---
## \#1161 Posted by: Pimousse Posted at: 2018-07-12T15:38:18.301Z Reads: 272

```
[quote="trampa, post:1160, topic:3813"]
Once nailed this will be the mode everyone will use.
[/quote]
This kind of statement enhances people's feeling that only Benjamin's words are the truth.
IMHO, this is NOT how collaborative projects work.
Lot's of other people have awesome ideas, wonderful skills, amazing knowledge.
Making easier for them to collaborate and bring their ideas will get the whole project greater.

BTW, all the best for Ben's PHD !
This is a good evidence though that the project is still relying on one person : nothing can't go ahead during that time. :confused:
```

---
## \#1162 Posted by: webst Posted at: 2018-07-12T15:59:44.977Z Reads: 272

```

[quote="Pimousse, post:1161, topic:3813"]
This kind of statement enhances people’s feeling that only Benjamin’s words are the truth.
[/quote]
https://mlpforums.com/uploads/post_images/img-1384034-1-Bxp9A4B.gif

@trampa But really, can you unveil the mystery and give us something more about that new better way of controlling output power? There's no place for PID or easy way to implement ABS or real life traction control which would be cool. I'm fairly used to current mode and it's pretty intuitive. Watt mode is probably good for beginners and people that do not yet feel the throttle curve. What might be better and what is the reasoning behind it except one I already stated?
```

---
## \#1163 Posted by: trampa Posted at: 2018-07-13T04:24:15.682Z Reads: 261

```
As usual, Benjamin tries to nail problems at the very root, rather than patching things together. Current Control is super nice but there are some things that could be even better. In future you will be able to keep the full power (max output power wise) while making your vehicle safely controllable for beginners or even kids. Sounds contradictive but is achievable if you manage to compute a set of different parameters in real time and feed that back into a smart, new control loop. It's quite tricky but achievable. 

Frank
```

---
## \#1164 Posted by: lock Posted at: 2018-07-13T05:06:28.586Z Reads: 264

```
It'd be interesting to see his PhD research merge into the VESC Project... apart from the fact he seems to be using the VESC in his PhD project. A smart power control loop that takes into account things like weight balance and other external factors has much potential if done well.

I've had a pull request sitting in the VESC-Tool repo for almost a month. It's not been merged in, and TBH I really don't mind. I wont make another though. . . well not until I'm convinced it's a productive use of my time.
```

---
## \#1165 Posted by: trampa Posted at: 2018-07-13T07:45:26.208Z Reads: 274

```
As I told before, Benjamin was super busy in the last months. He usually works on stuff quite focused in blocks of spare time. Once he finds the time to sit down he nails things quite fast. 
Currently he sorts out permanent and non-permanent profiles and precise computation of all values from single VESCs and VESC arrays for VESC-Tool and VESC-Tool mobile. This way we will have a precise display of speed, battery usage, amp-flow, distance travelled etc. Precise statistics and RT-Data across multiple VESCs.
You need to be very concentrated when coding things and if you have a lot of distraction from other things its hard to focus. Plenty of patience, is one of Benjamin's biggest strength. 
On top of that its sometimes wise to work down certain things in a certain sort order to prevent going forward and backward. Implementing new features without considering future developments is not very wise.
The VESC code base is quite complex and there are many dependencies that need to be addressed. You can imagine that distraction is not good when digging yourself through the code base. If your pull request has been sitting there for a month that means nothing. Benjamin looks at the pull requests and considers the suggestions once he decides to sit down and code intensively fore some days.  
Good things take time to ripen.
```

---
## \#1166 Posted by: Pimousse Posted at: 2018-07-13T08:08:17.361Z Reads: 265

```
[quote="trampa, post:1165, topic:3813"]
You need to be very concentrated when coding things and if you have a lot of distraction from other things its hard to focus.
[/quote]
Do you code Frank ?
```

---
## \#1167 Posted by: trampa Posted at: 2018-07-13T08:51:43.999Z Reads: 269

```
No I do not code. I did some coding 15 years back, but that is not worth mentioning. But I do know the feeling of distraction while handling complex tasks. And I know how Benjamin works. When he starts something, he doesn't stop until its finished, and he does it with max patience and endurance. And if things don't work out straight away he can sit down for hours in the night until thing work perfectly sweet.
```

---
## \#1168 Posted by: Pimousse Posted at: 2018-07-13T09:32:57.231Z Reads: 270

```
Please Frank, stop talking for Benjamin.
Really.

We know how he works well before you became his agent.
```

---
## \#1169 Posted by: Minim Posted at: 2018-07-13T15:04:34.181Z Reads: 262

```
Haha exactly my thoughts. 

I can to some degree understand the part about distractions and focus tho. I do this for a living and I def get most done the days where my phone isn’t constantly buzzing or if I close my email :D This is not a case only for programming tho it’s for whatever you work with ^^ 

Hope there can be more collaboration in the future so it can move forward faster. I’m sure there are a lot of good contributors out there that would love to help out.
```

---
## \#1170 Posted by: b264 Posted at: 2018-07-13T16:44:58.611Z Reads: 261

```
Then he could give someone else commit rights to the repo so others could work on it, too if he doesn't have time.
```

---
## \#1171 Posted by: webst Posted at: 2018-07-13T19:04:31.298Z Reads: 271

```
It’s his repo so just fork it and do whatever you want.
```

---
## \#1172 Posted by: Jc06505n Posted at: 2018-07-13T20:19:58.839Z Reads: 279

```
![image|400x400](upload://s5oTUkZSVVOUtTL2gBYRxVV0BM.jpeg)


Why not have someone of the community fork the project and then have all your pull request there? That way Benjamin can do things his way , and the community will be able to contribute and progress without having to wait for one man ?
```

---
## \#1173 Posted by: esk81 Posted at: 2018-07-17T09:49:26.060Z Reads: 265

```
Will Maytech also make VESC6? 
Has anyone any news from them?
```

---
## \#1174 Posted by: SammiHuangabc Posted at: 2018-07-18T09:48:03.443Z Reads: 263

```
My friend told me that Maytech doesn't make VESC6, though it's an open source, but still not easy to make it. It has higher requirement for RD teams. But I heard that Flispky make it out!  I will test it. Sounds good! with half price.
```

---
## \#1175 Posted by: b264 Posted at: 2018-07-18T18:25:04.473Z Reads: 261

```
There is no R&D when using an open-source design.  It's only about execution.
```

---
## \#1176 Posted by: skatardude10 Posted at: 2018-07-18T19:04:22.469Z Reads: 266

```
In a general sense, when simply just using the open source designs and that's it, yes.
```

---
## \#1177 Posted by: nw-esk8 Posted at: 2018-07-19T23:08:49.194Z Reads: 265

```
Has anyone tried Maytech's 100a vesc4?  It seemed to do well in some stress tests.  Not sure how much I care about any vesc6 offering if I have a vesc4 that can handle 100a continuous :star_struck: .
```

---
## \#1178 Posted by: dareno Posted at: 2018-07-23T05:01:18.924Z Reads: 259

```
Only if you completely trust that source.  When putting something on the market its always best to do your own r&d.  We trust BV but that doesn't mean maytech does.
```

---
## \#1179 Posted by: amf Posted at: 2018-08-01T11:04:39.016Z Reads: 252

```
@nw-esk8  ... we tested Maytech's with 1440w (48v / 30a) constant conditioned power in a lab, no airflow, ambient temp about 23 degrees c. It took 10 minutes to get to 100 degrees c. Much better than standard VESC 4.12. About 2x better. VESC 4.12 took 5 minutes.

Same test on FlipSky 6.6 ... see data on https://www.electric-skateboard.builders/t/new-vesc-from-china-seems-like-not-only-maytech-is-making-vescs-now/5207/409 thread ... did not get over 70 degrees c in 30 minutes.

FlipSky has been responsive, helpful and their hardware knowledge seems good. Can't really fault them at this point. Still testing.

FWIW, I wish everyone including the vendors would talk in watts ... amps are not really the right measure.

Cheers
```

---
## \#1180 Posted by: Maxid Posted at: 2018-08-01T11:13:35.822Z Reads: 250

```
[quote="amf, post:1179, topic:3813, full:true"]
FWIW, I wish everyone including the vendors would talk in watts ... amps are not really the right measure.
[/quote]
Won't watts be worse? Temperature is mainly dependent on current and not voltage AFAIK.
Like you can push say max. 40a at 6S or 12S without overheating but the watts will be vastly different.
```

---
## \#1181 Posted by: amf Posted at: 2018-08-01T11:37:03.722Z Reads: 247

```
@Maxid ... not as far as I understand. It seems to be the case with some things where only amps matter (eg: wires) ... I don't understand why but say 10 AWG is rated based on amps, but can do up to 600v. The amps matter, the volts don't so much. Do not understand, but this is the case. 

With current running through the controller, it matters.  See Vedder's video where he is demonstrating that the 4.12 VESC can run at '34amps all day' ... he was at 21v (from memory), but for sure and certain at 48v, this is not true. We know this, because we tested it in a lab. It can probably run at 600w all day, but not 34a at any input voltage.

There are plenty of people on this forum smarter than me who can explain this. It got a bit of airtime in the other thread I pointed to ... you can't have any amount of volts and I'm certain based on our testing that you'd be creating vastly different load with 40a @ 6s Vs 12s. You might not overload them at 12s, but it doesn't mean the load is the same. 

You'd could ride it uphill for a long period and monitor it on an app to see . Uphill will draw a lot more current than top speed on flat ground. You'll max the system out much faster as you'll draw max amps this way. Obviously depends on your weight etc, but this is a general rule as far as I can understand.

Cheers
```

---
## \#1182 Posted by: mishrasubhransu Posted at: 2018-08-01T13:41:09.299Z Reads: 235

```
Hmm, that's interesting. People say that temperature is related to current and not watts because formula for heat produced in a resistor is I^2R( I am sure almost everyone here has seen this). But that resistance R might not be a constant like we assumed. Maybe it does change with voltage, then we'll see the effect you are talking about.
```

---
## \#1183 Posted by: linsus Posted at: 2018-08-01T14:33:40.212Z Reads: 245

```
[quote="amf, post:1181, topic:3813"]
4.12 VESC can run at ‘34amps all day
[/quote]
The 4.xx VESCs are famous for going poof above 10S. Wouldnt recommend going past it. Not sure how far down I have to go to make you understand the concept of Voltage and current. But yes. Voltage only describes the potential between to conductors. to carry large currents you need fat cables or pcb traces, no matter of voltage. 

[quote="amf, post:1181, topic:3813"]
It can probably run at 600w all day, but not 34a at any input voltage.
[/quote]
Watts are simply a measurement of energy and not only coorelated to electricity. 

[quote="amf, post:1181, topic:3813"]
. You might not overload them at 12s, but it doesn’t mean the load is the same.
[/quote]
Correct, By increasing the Voltage, the amps needed to be drawn to produce the energy needed to propell you forwards are less. And the other way around obv.

[quote="mishrasubhransu, post:1182, topic:3813"]
But that resistance R might not be a constant
[/quote]
Resistance Changes with temperature. google superconductors and you'll understand.
```

---
## \#1184 Posted by: Maxid Posted at: 2018-08-01T17:50:07.029Z Reads: 237

```
Just from today:
https://www.electric-skateboard.builders/t/focbox-unity-dual-motor/52706/377?u=maxid
```

---
## \#1185 Posted by: b264 Posted at: 2018-08-01T18:05:02.545Z Reads: 240

```
[quote="Blasto, post:377, topic:3813"]
Input voltage is irrelevant in max current/thermal testing
[/quote]

at this point is an unproven conjecture and is no more correct than @amf 

Until there are side-by-side tests, it's just one person's opinion versus the other.
```

---
## \#1186 Posted by: Maxid Posted at: 2018-08-01T18:20:15.489Z Reads: 235

```
I am pretty sure @Blasto has done those tests. Up until today I thought we all agreed on P=RI² being the one formula to consider for our electronic systems.
I am open to be proven wrong though. @all: who will do those tests and publish them?
```

---
## \#1187 Posted by: JohnnyMeduse Posted at: 2018-08-01T18:29:24.477Z Reads: 246

```
[quote="b264, post:1185, topic:3813"]
at this point is an unproven conjecture
[/quote]

![download|234x215](upload://hd1YCBBnhyQjBbWvcKBkseciKE6.jpg)
```

---
## \#1188 Posted by: Blasto Posted at: 2018-08-01T18:42:15.536Z Reads: 250

```
using a pseudo random fet, all same circuit, with a 50A load. input voltage varying between 20V to 50V with a 10V increment

![image|690x277](upload://7sRQfQFmXLLqZZP34iYAegufjfL.png)


All the same drop across the fets
```

---
## \#1189 Posted by: linsus Posted at: 2018-08-01T18:44:22.692Z Reads: 243

```
LTspice ftw, what conclution are you trying to reach with the sim? Only the losses?
```

---
## \#1190 Posted by: Blasto Posted at: 2018-08-01T18:54:55.829Z Reads: 237

```
[quote="linsus, post:1189, topic:3813"]
what conclution are you trying to reach with the sim? Only the losses?
[/quote]


that input voltage is irrelevant for max current and thermal testing
```

---
## \#1191 Posted by: linsus Posted at: 2018-08-01T19:01:58.356Z Reads: 238

```
[quote="Blasto, post:1190, topic:3813"]
that input voltage is irrelevant for max current and thermal testing
[/quote]

Alright, the delta voltage is a function of the resistance thru the FET, which once again brings up the P=U*I, U=R*I -> P=R*I^2. 
Showing the square relation from the current. Anyone familiar with a exponential function knows that the current is the heaviest factor. Are people still debating this? :sleeping: :rofl:
```

---
## \#1192 Posted by: fedestanco Posted at: 2018-08-01T19:07:47.831Z Reads: 229

```
@linsus Can I ask you a more technical question? 
Since rpm depends upon voltage, and since higher switching frequency leads to higher impedance in the traces+mosfets, is it correct to assume that driving a motor with higher voltage at the input could produce more heat in the esc(because of the higher impedance)?
```

---
## \#1193 Posted by: linsus Posted at: 2018-08-01T19:19:19.217Z Reads: 227

```
Its a complicated question, switching frequency depends on sevral different factors other then the voltage level.
But yes the RPM or ERPM is directly correlated to the switching and while i dont meddle with power electronics that much as a proffession, I know quite abit about semiconductors. I'm afraid its not as easy as a yes or no answer. Both current and voltage play a part towards the actual losses while current being the desiding culprit. One cant exist without the other.
```

---
## \#1194 Posted by: Deodand Posted at: 2018-08-01T19:46:34.843Z Reads: 232

```
I agree, fairly certain at this point that current dominates the losses overall for the eskate operating regime. Started looking into modeling the FETs in the system analytically and it was way more complicated than I anticipated and got lazy a few hours in. 

As far as real world testing, ran some tests on the unity comparing our bench testing of 60 amps through motor at like 5-10% duty cycle vs. real-world hill climbing of 60 amps at around 80% duty cycle. In terms of thermals there wasn't much noticeable difference in the rate the boards heated up suggesting that motor current and not power is the best indicator of heat losses in the FETs.
```

---
## \#1195 Posted by: b264 Posted at: 2018-08-01T20:43:10.057Z Reads: 235

```
@Blasto But this is kind-of irrelevant because the *average* current in the ESC is probably limited by pulsewidths and impedances, and not by voltage drops across resistive loads.

We just need a side-by-side thermal test with same load on identical esk8 ESCs (using mechanical resistance on the motor axle) but different battery voltages.
```

---
## \#1196 Posted by: webst Posted at: 2018-08-01T21:41:32.313Z Reads: 239

```
[quote="amf, post:1181, topic:3813"]
I don’t understand why but say 10 AWG is rated based on amps, but can do up to 600v
[/quote]

Amp rating is for copper wire while voltage rating is telling you about arcing protection that cable insulation provides.
```

---
## \#1197 Posted by: amf Posted at: 2018-08-01T23:26:21.716Z Reads: 240

```
Thanks @Deodand ... this thread of amps / volts / heat is running in several places. Seems like motor amps (which seems to be a 'balancing number) Vs battery amps (less efficiency loss). It would help if the real world was bench simulated so that there's consistency in how this is talked about. There is a long rant here from 2016 which goes into a lot of detail http://buildelectricboards.com/showthread.php?tid=164&page=2 ... about how the battery and motor amps balance out.

When we tested our worst case of max motor torque based on full input of 48v/30a constant, we get a reading of someone doing their worst until the battery runs out. We are trying to make sure nothing can be broken. It was explained to me that there is less going to the motor due to efficiency, but this nonetheless represents our system running at full torque @ max speed the torque is available.

I'm not sure that the '80 amps all day' statement is a good description of what the controller does. Even the Maytech 100a ... with no airflow, it won't sustain our test for longer than 10 minutes before it gets to 100 degrees. So, this is not 100a ... we are using 30a. Obviously, the 100a is the wrong measure and is maybe a peak inbound measure ... or something.

Not sure of the solution, but we are doing our own testing as we can't work out from the marketing material what the actual maximum thresholds are. It's not the same with commercial controllers. What they will do is very clear.

The VESC community 'big brains' could devise a series of measures / tests that all vendors need to supply data for so that comparisons can be made ... now that would be interesting :slight_smile:

Cheers
```

---
## \#1198 Posted by: esk81 Posted at: 2018-08-17T03:52:15.658Z Reads: 209

```
Maytech is responsive and more honest
```

---
## \#1199 Posted by: esk81 Posted at: 2018-08-17T04:28:12.185Z Reads: 212

```
Flipsky is just bullshit, no R&D, but just sell cheap price by changing low quality components.
```

---
## \#1200 Posted by: amf Posted at: 2018-08-17T05:02:05.813Z Reads: 219

```
@esk81 Not my experience.
```

---
## \#1201 Posted by: amf Posted at: 2018-08-17T05:10:10.738Z Reads: 227

```
@esk81 again, not my experience. We've had flipsky develop a custom remote control for us. It wasn't easy and they have done a good job so far. 

They've taken the reference V6 design and done what appears to be a good implementation with anti-spark and other features added as well as a smart layout for heat. Clearly, they've done R&D. We've tested their FSesc 6.6. Can bus works great, heat dissipation is the best we've tested by a long way.

Have you got any evidence, or just insults?

Your posts look like sabotage posts ... 

Cheers
```

---
## \#1202 Posted by: esk81 Posted at: 2018-08-17T07:20:20.559Z Reads: 218

```
We tested Maytech 100A vesc, much better than 50A
```

---
## \#1203 Posted by: amf Posted at: 2018-08-17T11:40:23.335Z Reads: 216

```
The answer is that it depends on use. Amps and Volts together are the relevant measure and are what creates heat. See my previous posts. If you are using standard components for an e-board, chances are it'll be fine unless you are doing something off the map. I'd buy a V6 if you can as they are a substantial step up. Cheers
```

---
## \#1204 Posted by: kalebludlow Posted at: 2018-08-17T12:10:27.332Z Reads: 211

```
Obviously the ESC with the higher amperage is going to be able to get more performance. Unfair comparison
```

---
## \#1205 Posted by: Kug3lis Posted at: 2018-08-17T12:43:34.202Z Reads: 206

```
That remote is a copy from Firefly remote project... you can even see from views on OLED... So not much R&D was done just new case
```

---
## \#1206 Posted by: amf Posted at: 2018-08-17T12:45:49.292Z Reads: 207

```
@Kug3lis ... no, this is not public. It's a new remote. We haven't released it yet. So far, so good. Cheers
```

---
## \#1207 Posted by: Kug3lis Posted at: 2018-08-17T12:48:18.040Z Reads: 211

```
[quote="amf, post:1206, topic:3813"]
We haven’t released it yet.
[/quote]

Before you said you were independent from flipsky, and now "we" so you work for flipsky so all the stuff mentioned was just biased reviews? :D
```

---
## \#1208 Posted by: Jc06505n Posted at: 2018-08-17T13:08:43.444Z Reads: 210

```
I think the "we" he's using in this instance is the same "we" that had Flipsky developed the remote such as when he says: 

[quote="amf, post:1201, topic:3813"]
**We**’ve had flipsky develop a custom remote control for us.
[/quote]

So we would me him and who ever he's associated with to make Flipsky make the remote , not we as in him and Flipsky
```

---
## \#1209 Posted by: Kug3lis Posted at: 2018-08-17T13:09:41.523Z Reads: 205

```
Maybe, but I can't find right now video, I saw in some flipsky thread where you can clearly see oled screen :D
```

---
## \#1210 Posted by: Jc06505n Posted at: 2018-08-17T13:10:40.415Z Reads: 206

```
Oh yea i agree with you on that, More than likley they took Solidgeeks Firefly and ran away with it, just wanted to clarify his use of we in context.
```

---
## \#1211 Posted by: amf Posted at: 2018-08-17T22:06:47.912Z Reads: 197

```
@Kug3lis ... 'we' are a company ... not FlipSky. 

They are a potential supplier. We are testing their FSESC 6.6 as a possible solution and also had them develop a custom remote.

Cheers
```

---
## \#1212 Posted by: amf Posted at: 2018-08-18T11:05:41.736Z Reads: 195

```
Seems to us it's about watts, not just amps. Our tests show amps quoted by suppliers as not much use for our case of constant 48v with only amps varying. We go nowhere near the amps they quote (at least on the battery / inbound side) ... see my previous posts. 

Bottom line, it's not just about constant amps when it comes to generating heat in the VESC. The constant voltage matters.

Cheers
```

---
## \#1213 Posted by: Maxid Posted at: 2018-08-18T11:25:25.221Z Reads: 194

```
[quote="amf, post:1212, topic:3813, full:true"]
Bottom line, it's not just about constant amps when it comes to generating heat in the VESC. The constant voltage matters.
[/quote]
no it does not (at least not significantly) - we had this discussion before.
```

---
## \#1214 Posted by: amf Posted at: 2018-08-19T02:37:59.998Z Reads: 194

```
@Maxid ... Doesn't make sense. Why would it be in the lab we can overheat all VESC 4.12s (including Maytech's 100a one) with 48v / 30a constant from the battery in 5-10 minutes? Have you done any bench testing you can share or do you have any other reasoning as to why this would happen?

Cheers.
```

---
## \#1215 Posted by: Maxid Posted at: 2018-08-19T07:27:12.895Z Reads: 197

```
Because a 4.12 VESC is not capable of 30A continuously (irrespective of the voltage) - duh.
I have a dual VESC 4.12 setup and get it to overheat in a couple minutes with a battery current of 40A in total (so 20 each) by just doing acceleration tests.
Nobody cares because nobody actually needs 30A * 40V = 1200W continuously. 
I can throw the P=I² * R equation at you again but you don't want to accept that.

Did you do the same 30A test also at 24V? I am sure the results will be the same.
```

---
## \#1216 Posted by: amf Posted at: 2018-08-19T08:49:49.872Z Reads: 194

```
@maxid In his video, Vedder has the 4.12 at 21v and 34a ... says it will do this 'all day'. Maybe argue with him first, then me.

Cheers.
```

---
## \#1217 Posted by: Maxid Posted at: 2018-08-19T08:50:42.415Z Reads: 201

```
So you didn't do the test at 24V. Come back with your numbers once you have them. Cheers

Also which video are you talking about?

Just to give an idea:
https://youtu.be/1iwN5LGGM80
When Vedder says 70A he is referring to motor current and not battery current. That is a difference!!! What's important here is that the current actually going into the VESC is only 7A.
@amf did you mix up motor current and battery current?
```

---
## \#1218 Posted by: amf Posted at: 2018-08-20T03:01:17.203Z Reads: 200

```
[quote="Maxid, post:1217, topic:3813"]
did you mix up motor current and battery current?
[/quote]

I'm not sure that I mixed it up, but yes, I am talking about battery current not motor / phase current. What we are trying to deal with is the VESC overheating.

In the video Vedder points to the watts and says 'and dissipating X watts of losses in the system, so things are going to get really warm'  ... so he's saying watts (battery amps x input Volts) are relevant to heat. He goes on to say it can run at 34a all day but this is only around 50 watts from the battery.

As I've said before, our constant voltage is 48-52 per motor / VESC. Our minimum amps from the battery is 6 with an average of around 15 and max 30 but this could be sustained for several minutes on and off.

So, I can see what you are saying, but it's not what we are focused on the as the motor / phase current is not a good proxy for heat.

Cheers
```

---
## \#1219 Posted by: AlexBE Posted at: 2018-08-20T04:06:42.825Z Reads: 190

```
I'm late to this conversation, but I'm fairly sure the dominant contributor to the temperature of the VESC is the I2R (IxIxR) losses in the FETs. So this means the limiting factor will be motor/phase current.

This means if you are running Bat=50V@5A input to the VESC and it is driving the motor at 5V@50A. You will get 50x50xR (~50x50x0.01=25W) of heat in the fets. Note that I have made up the value of 10mOhm for the FETs. 

Increasing the input power to Bat=50V@25A, but running the motor at a higher speed and hence Mot=25V@50A will lead to the same 25W of heat in the fets/VESC. So even though the VESC input power is 250W vs 1250W, the heat/temperature of the VESC is the same.
```

---
## \#1220 Posted by: Maxid Posted at: 2018-08-20T04:55:52.598Z Reads: 186

```
Sounds to me like you really did mix them up. No wonder you thought voltage matters. You can't use motor current for your calculation as that is not at constant voltage but varies due to the duty cycle. For easy comparison only use battery voltage and battery current when talking about how much current the VESC can handle. Vedders 34A is meaningless as the "real" amps going into the system are only 2A.
```

---
## \#1221 Posted by: amf Posted at: 2018-08-20T05:03:22.352Z Reads: 190

```
@AlexBE @Maxid ... maybe our setup is atypical. It's possible.

Our engineering partner took the various VESCs to a test lab. They put 30a / 48v into the VESC through conditioned power and had a motor drawing max amps running at constant voltage on the other side. With efficiency losses, slightly lower than 30 amps. This was to represent our worst case to allow us to work out what a customer who maxxed the system out until the battery was dead would do to the controllers ... an unlikely situation, but one that needs to be allowed for.

[quote="Maxid, post:1220, topic:3813"]
For easy calculation only use battery voltage and battery current!
[/quote]

Thanks. That is what we are using. Maybe I wasn't clear.

Cheers.
```

---
## \#1222 Posted by: Maxid Posted at: 2018-08-20T05:06:13.376Z Reads: 188

```
But then you should have seen that voltage does not matter!
```

---
## \#1223 Posted by: b264 Posted at: 2018-08-20T05:07:00.002Z Reads: 191

```
[quote="Maxid, post:1220, topic:3813"]
Vedders [sic] 34A is meaningless as the “real” amps going into the system are only 2A.
[/quote]

This may not be true when dealing with square waves.  You can have pulses of 34A going to the inductive motor windings but drawing 2A into the filter capacitor from the battery -- in this case, it actually is the 34A that will be expending energy according to the "on" resistance of the FETs and P = I²R, but even then only through the inductance of the windings

The only real test is empical and see how much the ESC heats up a known volume of water under a known load
```

---
## \#1224 Posted by: Maxid Posted at: 2018-08-20T05:09:11.916Z Reads: 185

```
I am not sure if it is that easy as i²r when you talk about an AC signal instead of the DC one coming from the battery.
```

---
## \#1225 Posted by: b264 Posted at: 2018-08-20T05:10:19.403Z Reads: 184

```
[quote="Maxid, post:1224, topic:3813, full:true"]
I am not sure if it is that easy as i²r when you talk about an AC signal instead of the DC one coming from the battery.
[/quote]

It is P = I²R ***at any one instant in time***.  For the time-based "work" expended (watt*hours instead of watts, aka "degrees Centigrade times grams of water"), you need to get calculus involved.  Or do an empirical test according to water temperature.
```

---
## \#1226 Posted by: Maxid Posted at: 2018-08-20T05:28:23.357Z Reads: 188

```
It still can't be that the 34A are responsible for the heat loss as that would give you a situation where P coming from the battery is less than what the P in the fets would be.
In the example with Vedder (If I remember the numbers correctly he draws 70 motor amps and battery amps of 2).
So the power the VESC has to dissipate is 2² * r and not 70² * r. How should that work otherwise if you have a total of 50W going in but are supposed to dissipate more than that :confused:
```

---
## \#1227 Posted by: b264 Posted at: 2018-08-20T06:10:45.038Z Reads: 187

```
Because the phase wires aren't on constantly, they are pulsing on and off, and, even while on, the voltage is fluctuating due to the inductance of the windings, and isn't necessarily full battery voltage
```

---
## \#1228 Posted by: AlexBE Posted at: 2018-08-20T06:28:48.681Z Reads: 192

```
Using your Vedder example. 70 motor amps means that the power the VESC has to dissipate is ~70x70xR (r=fet on resistance). This is why he does his temperature testing at 70 motor amps with only 2 battery amps. So he can temperature test the VESC without having to supply it with a huge amount of power.

Of course the power he has to supply it with has to be more that what the VESC needs to dissipate. Power(battery) = Power(VESC)+Power(Motors).

So making up some numbers. If we have Battery=50V@2A=100W. FET/MOTOR current of 50A. and FET on resistance of 0.01ohms.

Battery(50V*2A=100W) = VESC(50x50x0.01=25W) + MOTOR (50Ax(2-(50Ax0.01) = 75W)

You can see that with the motor current of 50A, you have a total of 2V across the FETs and motor windings. 0.5V across the FETs and 1.5V across the motor windings.
```

---
## \#1229 Posted by: b264 Posted at: 2018-08-20T06:36:57.801Z Reads: 188

```
No, all three phases are switching on and off at irregular times based on complex formulas.  The battery amperage is the only *somewhat* steady flow.  Think "calculus versus algebra"

Ye have to understand the difference between something happening right now, and something that happens now then turns off, then turns on, then turns off, and there are three of those things turning on very briefly at weird times controlled by complex formulas.

The definitive truth is [in the BLDC firmware](https://github.com/vedderb/bldc/blob/43c3bbaf91f5052a35b75c2ff17b5fe99fad94d1/mcpwm_foc.c) source code, feel free to have a look anytime
```

---
## \#1230 Posted by: AlexBE Posted at: 2018-08-20T06:49:57.965Z Reads: 188

```
In this case, the battery current/voltage/power are fairly constant. On a VESC they are not directly measured but inferred from the phase current/duty cycle. I understand the firmware, it's what I do for a living.

My point from my previous post still stand, my simplified power equation stands. 

Power(battery) = Power(VESC)+Power(Motor)

So in general for VESC temperature testing, you need to increase the phase current, because that will increase the power heating up the VESC. You can do this in many ways. You could put a large load on the motor and run a very high battery power. Or you can use the tools built into the vesc to run an open loop with a set motor current. The advantage of that is you don't need a huge battery power, and you don't need to load the motor down (and dissipate the heat that generates).
```

---
## \#1231 Posted by: Maxid Posted at: 2018-08-20T07:11:36.708Z Reads: 186

```
ok i think I got it now - thanks for your explanation.
What I still don't understand however is how @amf is able to test his setup when he applies 30A battery current. What phase current is he then using (the VESC seems to regulate the input current itself based on the load no?).
Also how is @amf doing his tests that he still thinks voltage matters noticeably?

@moderators you might want to put this discussion in its own thread - it has nothing to do with VESC6 but ESC power losses in general.
```

---
## \#1232 Posted by: AlexBE Posted at: 2018-08-20T07:31:37.903Z Reads: 187

```
No problem (if you were thanking me). This is a complex topic.

It's important the way things are phrased, @amf is not applying 30A battery current, the vesc is pulling 30A from the battery. The phase current at this battery current/voltage depends on  many things like motor winding resistance, motor speed (back emf) etc.

What I am assimung about @amf's test is that he is running a motor at some duty cycle, say 90%. Lets assume at 24V, 90% duty cycle that particular motor, under whatever load it is under has 20A phase current. So if they increase the voltage to 30V and keep the duty cycle the same, the phase current might increase to 25A.

In answer to your other question, the VESC takes a throttle input in some form (analog, PPM, PWM) but it has many different modes to turn that throttle value into output duty cycle. IF you run the VESC in the duty cycle mode, it will turn the throttle directly into duty cycle. So at 50% throttle, you will get 50% duty cycle. On the other hand if you run in Current mode, 50% throttle will turn into 50% of your set motor max current.

The other complication is that in duty cycle mode, you will still have a current limit. So if your throttle is 90%, but you have a motor current limit of 50A, if 90% duty means motor=100A, the VESC will turn down the duty cycle until the motor current=50A.

Similarly if you are running in current mode and you have 90% throttle and current max of 50A, so set current =45A. If 95% duty cycle only gives you motor=20A, there is no way of increasing the motor current.

So maybe @amf is increasing his VESC power(heat) by increasing his input voltage because he is either at a duty cycle limit or a current limit, and increasing the voltage allows either of those to be overcome.
```

---
## \#1233 Posted by: Maxid Posted at: 2018-08-20T07:37:06.005Z Reads: 182

```
But he said this:
[quote="amf, post:1221, topic:3813"]
They put 30a / 48v into the VESC through conditioned power and had a motor drawing max amps running at constant voltage on the other side.
[/quote]

that is why I said he "supplies" 30A as it sounds like he keeps this constant - but in the video the VESC regulates the input current dynamically and keeps the phase current constant.

I am just trying to debunk his mentions of the voltage having an effect on the heat loss in the VESC. Even with the P=I²R formula he still seems to think it is not true.
```

---
## \#1234 Posted by: AlexBE Posted at: 2018-08-20T07:45:51.830Z Reads: 185

```
I suppose the details are important and maybe they have been posted but I didn't read far enough.

They say 

@amf "They put 30a / 48v into the VESC through conditioned power and had a motor drawing max amps running at constant voltage on the other side."

What is max amps? and at what voltage. The maximum number of amps depends on the motor winding resistance. Absolute worst case is the motor being stationary, and they they will draw hundreds of amps (if you don't control the duty cycle).

"With efficiency losses, slightly lower than 30 amps."
If it's slightly lower than 30 amps, its really not max amps or a worst case scenario.

Maybe they mean that in their product, they have the motor current limit set to 30 amps, and so they wanted to test what would happen running at that motor current? And so they or their test place naively thinks that current battery = current motor, but that is a complete misunderstanding.
```

---
## \#1235 Posted by: AlexBE Posted at: 2018-08-20T08:29:08.353Z Reads: 191

```
I think I caught up and found where the problem in understanding started. I should have read it sooner. @amf says this

[quote="amf, post:1179, topic:3813"]
we tested Maytech’s with 1440w (48v / 30a) constant conditioned power in a lab, no airflow, ambient temp about 23 degrees c. It took 10 minutes to get to 100 degrees c. Much better than standard VESC 4.12. About 2x better. VESC 4.12 took 5 minutes.
[/quote]

This test is only valid IF the motor current is controlled. It also doesn't guarantee a worst case scenario. If you have Battery=48V@30A, but motor current is only 30A, you aren't testing worst case. You could have Battery=48V@30A and Motor=9V@144A. This is the kind of thing that could happen with a heavy person riding up a large hill.

In the second case, you would have ~20 times more power being dissipated in the VESC. (this is why you would limit the motor current to less than 144A :) )
```

---
## \#1236 Posted by: amf Posted at: 2018-08-20T08:35:19.976Z Reads: 180

```
@Maxid @AlexBE ...  
[quote="AlexBE, post:1235, topic:3813"]

This is the kind of thing that could happen with a heavy person riding up a large hill.
[/quote]

Yes, or someone riding your product on soft sand ... uphill  :) 

The motor current was limited to 100a (not 30a) ... my mistake ... I can see the motor at over 40a in the data I have from the Metr app here under 'normal' load, but what you outline is the right principle.

Apologies for the confusion.

Cheers.
```

---
## \#1237 Posted by: AlexBE Posted at: 2018-08-20T08:37:34.969Z Reads: 182

```
@amf, AHH! that makes more sense now. If you have the motor current set at 100A, and you have some way of keeping it at 100A, then you have one way of comparing one controller to another. Do you know how they kept the motor current at 100A? Did they put a large variable load on the motor or was it done using some of the vesc tools like FOC_OPEN_LOOP?
```

---
## \#1238 Posted by: Maxid Posted at: 2018-08-20T08:39:16.059Z Reads: 184

```
but he just said that only the LIMIT was set to 100A and that the actual load was dynamic (e.g. "40A in metr app").
I still don't get how they are doing repeatable tests between controllers.
```

---
## \#1239 Posted by: AlexBE Posted at: 2018-08-20T08:41:04.478Z Reads: 187

```
It's certainly not the way I would do it, using the FOC_OPEN_LOOP like vedder did in his videos is the easiest and best way to compare current handling.

It's not completely crazy though to have a big motor and load it down so that it always current limits at 100A.
```

---
## \#1240 Posted by: amf Posted at: 2018-08-20T08:42:02.919Z Reads: 194

```
[quote="AlexBE, post:1237, topic:3813"]
Do you know how they kept the motor current at 100A? Did they put a large variable load on the motor or was it done using some of the vesc tools like FOC_OPEN_LOOP?
[/quote]

They put a load on the motor as far as I know.

@Maxid They weren't using the Metr app: I have it here with a prototype. 

The VESCs were tested on a bench. It was a commercial test lab inside a large company that makes motors.

Cheers
```

---
## \#1241 Posted by: Maxid Posted at: 2018-08-20T08:43:22.270Z Reads: 185

```
well according to the results you defend (you say "voltage matters") the test lab has no credibility to me right now no matter what company it is part of.
```

---
## \#1242 Posted by: Maxid Posted at: 2018-08-20T08:44:37.593Z Reads: 196

```
[quote="AlexBE, post:1239, topic:3813, full:true"]
It's not completely crazy though to have a big motor and load it down so that it always current limits at 100A.
[/quote]
But if they did then they should have arrived at the point where the input voltage does not matter no?
```

---
## \#1243 Posted by: AlexBE Posted at: 2018-08-20T08:47:12.597Z Reads: 202

```
Yes I agree with this @Maxid and your other comments. Definitely to do temperature testing it is not necessary to use large input and output powers. Only output current has a real effect on temperature.

However I would say in testing a product like a speed controller, if you are doing engineering testing, it will be important to test at both high voltage and current, input and output to see if there is anything wrong with your design.
```

---
## \#1244 Posted by: amf Posted at: 2018-08-20T08:48:29.619Z Reads: 203

```
Thanks for the advice. I'll pass it onto the engineers.

Cheers
```

---
## \#1245 Posted by: SammiHuangabc Posted at: 2018-08-21T09:48:56.605Z Reads: 195

```
Provide your proof!
```

---
## \#1246 Posted by: luis99945 Posted at: 2018-10-06T03:00:42.370Z Reads: 169

```
how much it?
```

---
## \#1247 Posted by: kalebludlow Posted at: 2018-10-06T03:02:47.315Z Reads: 182

```
http://www.trampaboards.com/vesc-6-complete--vedder-electronic-speed-controller-trampa-exclusive-p-24166.html
```

---
## \#1248 Posted by: Lasse_Bierstrom Posted at: 2018-10-07T07:44:40.775Z Reads: 183

```
Don't forget, that motor current is always carried by the Fets! Irrespective of battery current...
And we sum up the current on the three windings, so they run somehow also in parallel. Not three at the same time, but it is also a factor playing a role.
```

---
## \#1249 Posted by: Volts Posted at: 2018-11-21T10:38:52.522Z Reads: 164

```
Has anyone used a Photon remote and receiver setup on BV VESC 6 if so can they post pics of how they connected the receiver to the controller?
```

---
## \#1250 Posted by: J0ker3366 Posted at: 2018-11-21T10:40:30.711Z Reads: 160

```
Reciever to controller? Binding them?
```

---
## \#1251 Posted by: Volts Posted at: 2018-11-21T10:42:15.287Z Reads: 154

```
need pics or explanation of the wire connection between the receiver and controller VESC 6, like how do I connect to the UART from a 6 pin receiver?
```

---
## \#1252 Posted by: J0ker3366 Posted at: 2018-11-21T10:43:32.439Z Reads: 158

```
Its a ppm cable. See those three little metal prongs sticking up in the corner of the pcb?
```

---
## \#1253 Posted by: Volts Posted at: 2018-11-21T10:44:48.298Z Reads: 161

```
its not a ppm its 6 pin UART, the VECS 6 has a 5 pin and an 8 pin connector
```

---
## \#1254 Posted by: J0ker3366 Posted at: 2018-11-21T10:46:42.066Z Reads: 160

```
Which vesc 6? Does the 6 not use ppm anymore?
```

---
## \#1255 Posted by: Volts Posted at: 2018-11-21T10:48:10.647Z Reads: 165

```
It does but i have a Photon remote I want to use, however am confused as to how it works on the VECS 6, if at all? Do you have a VECS 6?
```

---
## \#1256 Posted by: J0ker3366 Posted at: 2018-11-21T10:51:53.425Z Reads: 167

```
No but we're good. Show me pictures of your remote, receiver and vesc please.
```

---
## \#1257 Posted by: Volts Posted at: 2018-11-21T10:54:40.360Z Reads: 176

```
https://eboardshop.net/product/advanced-electric-skateboard-remote/
https://www.trampaboards.com/vesc-6-complete--vedder-electronic-speed-controller-trampa-exclusive-p-24166.html
```

---
## \#1258 Posted by: J0ker3366 Posted at: 2018-11-21T11:01:20.487Z Reads: 172

```
Gotcha. So I'm not familiar with the remote as I use the Mini. Bit I'm sure you could do a general search here and find out. Try something like, photon vesc 6 wiring. Add diagram if your ballsy lol.
```

---
## \#1259 Posted by: Volts Posted at: 2018-11-21T11:08:02.295Z Reads: 176

```
Nothing, either no one uses this combo or they just haven't posted about it. I'll start a new thread.
```

---
## \#1260 Posted by: J0ker3366 Posted at: 2018-11-21T11:15:29.882Z Reads: 183

```
Funny cause searching exactly what I told you brought this up...
![Screenshot_2018-11-21-04-14-39|281x500](upload://ArdKaqS4mJnQurw2SmY88IiuamM.png)
```

---
## \#1261 Posted by: Volts Posted at: 2018-11-21T11:20:00.829Z Reads: 181

```
That's a different receiver to the one  I got, I could be mistaken but I think this is the older version, the new version, mine, doesn't look like that.
```

---
## \#1262 Posted by: J0ker3366 Posted at: 2018-11-21T11:21:48.116Z Reads: 180

```
Fair enough. How ever if you search photon vesc 6 wiring, the second thread, as this thread will be the first, is the threat for the photon remote. Read through that thread. If you don't find your answer, ask your question there as well.
```

---
## \#1263 Posted by: b4zz Posted at: 2018-12-24T13:54:57.294Z Reads: 153

```
Are pins SL_A, SL_B and SL_C directly tied to ground coming from the DRV8301 chip?
```

---
## \#1264 Posted by: linsus Posted at: 2018-12-24T14:37:13.390Z Reads: 151

```
Check the schematic
```

---
## \#1265 Posted by: b4zz Posted at: 2018-12-24T14:42:14.375Z Reads: 159

```
Thanks for the reply, I've checked the schematics, there it seems that these pins are connected to ground. All SL pins are going to the Sources of the fets. See attached image. ![10|690x290](upload://qbhwgVdTbotZzv2Gsfb8F5FuVh7.png)

I want to know if these pins can thus be directly tied to ground from the DRV8301.
```

---
## \#1266 Posted by: linsus Posted at: 2018-12-24T14:49:31.689Z Reads: 159

```
Point might be that the source need to tied relativly close to those ports on the DRV, no matter jag if theyre ground in General
```

---
## \#1267 Posted by: b4zz Posted at: 2018-12-24T15:31:21.373Z Reads: 160

```
Hmm that will be a tough one since I'm designing a vesc 6 with only two layers. So the entire bottom is GND with signal lines crossing. So it isn't possible to run a trace to the source that easy.
```

---
## \#1268 Posted by: Kug3lis Posted at: 2018-12-24T15:43:32.654Z Reads: 161

```
Ahm if you have these questions, I suggest to stop and do some research for like about designing current/voltage sense paths and etc stuff... Because they are really important and will cause so major issues with sensing currents/voltages on the shunts and drive stages.
```

---
## \#1269 Posted by: linsus Posted at: 2018-12-24T15:48:03.192Z Reads: 162

```
Id recommend a 4 layer design on the VESC6 to keep it in a relative good size. As @Kug3lis said, the current sense amplifiers need identical paths for optimal performance, also. Your going to have a hard time doing the Power stage with 2 layers only. I dont agree with kugelis on stoppning tho. Learning experience is always a good one. But dont be too dissapointed if you run into problems :)
```

---
## \#1270 Posted by: Kug3lis Posted at: 2018-12-24T15:51:54.177Z Reads: 164

```
Well I am suggesting to stop just because spending money on not working PCB it is not fun :) But if you don't mind spending some money on some steps until success when yeah go ahead the best experience is learning from mistakes.. Talking from experiences :D
```

---
## \#1271 Posted by: Stevemk14ebr Posted at: 2018-12-24T15:55:14.647Z Reads: 168

```
The vesc is PWM. It's not PPM, everyone mislabels it. THE VESC IS PWM
```

---
## \#1272 Posted by: mmaner Posted at: 2018-12-24T15:57:13.437Z Reads: 165

```
Why not just answer the question or be silent?
```

---
## \#1273 Posted by: b4zz Posted at: 2018-12-24T15:59:17.099Z Reads: 167

```
Thanks for the replies guys. Designing the pcb with 2 layers should be doable. I need a maximum of around 15A continuous. Currently I'm using a the equivalent of a 400mil trace for the SUPPLY. I do have a pretty good understanding of designing pcb's. 

It's only the sense lines that get me. Because when looking at the datasheet from the DRV8301, there are 10mOhm resistors placed in series with the source and ground. Yet in the vesc's schematics these aren't used. 
![45|598x500](upload://A301dPVgECvbU1vwbjBo0Piv3uU.jpeg). 
This would mean there is no voltage drop to be measured so nothing is sensed.
```

---
## \#1274 Posted by: linsus Posted at: 2018-12-24T16:04:12.398Z Reads: 161

```
Sound like every project ive ever been in :stuck_out_tongue: gotta start somewhere
```

---
## \#1275 Posted by: linsus Posted at: 2018-12-24T16:09:14.984Z Reads: 167

```
[quote="b4zz, post:1273, topic:3813"]
are 10mOhm resistors placed in series with the source and ground.
[/quote]

That sound like a low side shunt. Th vesc6 has the shunt resistor like the schematic you posted previously.

Unless theyre specifying the trace impedance
```

---
## \#1276 Posted by: b4zz Posted at: 2018-12-24T16:13:18.139Z Reads: 168

```
Exactly my point. These two shunts are used in the 4.12 HW design. They are not trace resistance. But the created voltage can be measured as a current flow. In the 6 HW design three shunts with current sense amplifiers are used for this purpose. 

But that eliminates the two shunts and the voltage potential, so nothing can be measured. Or I must be making some mistake somewhere.
```

---
## \#1277 Posted by: linsus Posted at: 2018-12-24T16:17:37.824Z Reads: 167

```
Keep those SL points as close as you can and I think you're fine. CADing a dual vesc6 atm but havnt started layout that far yet
```

---
## \#1278 Posted by: Minim Posted at: 2019-01-01T22:10:15.280Z Reads: 163

```
What firmware are people running on their vesc6? I got a escape vesc6 and I've tried ackmaniac and the stock one. Is the stock one more up to date? The ackmaniac has been on the same version for quite a while now.
```

---
## \#1279 Posted by: Volts Posted at: 2019-01-28T05:03:02.319Z Reads: 148

```
Just tryed duel receivers on my duel motor setup and now one of my VESC 6 wont turn on, help?
```

---
## \#1280 Posted by: b264 Posted at: 2019-01-28T05:14:53.632Z Reads: 152

```
Is the only connection between the VESCs the two fat power wires?
```

---
## \#1281 Posted by: Volts Posted at: 2019-01-28T05:28:15.679Z Reads: 151

```
actually Im running the two VESC 6 off a positive and negative bus bar, negative is to the BMS positive to the battery terminal and this is a UART, Photon, receiver setup, it was working for like a .5 of a sec then the slave controller went dead, and no blue light could be seen.
```

---
## \#1282 Posted by: hazza Posted at: 2019-01-28T05:50:13.418Z Reads: 149

```
is there any place we can get design files?
```

---
## \#1283 Posted by: chuttney1 Posted at: 2019-01-28T06:10:02.518Z Reads: 149

```
Only the schematic.
```

---
## \#1284 Posted by: hazza Posted at: 2019-01-28T06:11:15.695Z Reads: 151

```
where would I be able to find that?
```

---
## \#1285 Posted by: trampa Posted at: 2019-01-28T06:23:15.168Z Reads: 153

```
Please sketch up the entire system. It's hard to know what killed the ESC if there is no diagram of the setup.
```

---
## \#1286 Posted by: Volts Posted at: 2019-01-28T06:42:57.450Z Reads: 155

```
![Untitled|690x388](upload://b9GI2W1GRwRBd4IVcyPgKPtQ5J3.png)
```

---
## \#1287 Posted by: Volts Posted at: 2019-01-28T06:44:26.809Z Reads: 158

```
sorry for it looking like crap, i hope you get the idea, that UART are separate modals
```

---
## \#1288 Posted by: Andy87 Posted at: 2019-01-28T06:51:54.435Z Reads: 181

```
Just to get it right, every vesc has his own uart receiver module for the remote?
Or you connected the wires from both vescs to one uart module?
Sorry if you wrote that in your last comment, but it’s not clear for me.
```

---
## \#1289 Posted by: Volts Posted at: 2019-01-28T06:52:42.950Z Reads: 183

```
they are separate as you said, they are not connected each VESC 6 has its own UART receiver. If I take apart the VESC6 will i find a reset switch or something like that? or is this more like a blown transistor or a blown capacitor problem, came from the Ebike world before starting this biuld, with ebikes most everything is analog with Eskates is mostly digital, digital = confusion
```

---
## \#1290 Posted by: trampa Posted at: 2019-01-28T07:42:46.481Z Reads: 180

```
There is probably something wrong with the receiver if there is no connection in between the VESCs.
If there would have been a connection, a ground loop would probably have been the issue. 
Dual receivers are not needed BTW. A simple CAN cable would be the best way to interconnect the VESCs.

My guess is a dead voltage regulator or a dead STM processor. Can be fixed by someone with experience with VESCs. I would not try to plug the potentially faulty receiver into the other VESC. 
Please check the wiring on the receivers. 
Did you use the receiver to switch other things like lights?
```

---
## \#1291 Posted by: Volts Posted at: 2019-01-28T07:47:07.600Z Reads: 173

```
No lights where added to the setup, the only thing that was done was to plug in the UART receiver to the UART on the controller, making sure to line up the wires correctly, as stated in the earlier post, the setup worked for like a sec then the controller went dead, even when powering on the system the other controller can be seen to have its lights on where are the slave controller has no blue light showing which would indicate a dead component somewhere in the controller.

Ill have to open the controller up sometime to see where the dead component is, the receiver works on the master controller just fine, and i tried powering the slave receiver to the master controller and it seemed to power on so its hard to say if the receiver is really the problem?
```

---
## \#1292 Posted by: Volts Posted at: 2019-01-28T07:55:46.257Z Reads: 156

```
Have you had someone ask you about this problem before trampa?
```

---
## \#1293 Posted by: trampa Posted at: 2019-01-28T08:04:54.491Z Reads: 158

```
I would say there is a component that is dead. Hard to say which one. I guess the receiver has an issue, so I would not try it on the other VESC. 
Visual inspection will probably not help. If there is no light, the 3.3V and/or 5V rail is dead. 
This points to a dead voltage regulator circuit and maybe a dead STM32, which points to a faulty receiver. 
If the VESC had its lights on prior to plugging in the receiver, the 3.3V rail was just fine before the VESC tried to powered up the receiver.  It is a guess, but usually things don't fry just like this. To avoid further damage, I would isolate the receiver and mark it. 

Frank
```

---
## \#1294 Posted by: Volts Posted at: 2019-01-28T08:12:42.040Z Reads: 147

```
Can the parts be de soldered and replaced, or will i to send it back to you for repairs, buying another controller seems like a waste?
```

---
## \#1295 Posted by: trampa Posted at: 2019-01-28T08:17:27.255Z Reads: 161

```
Yes, they can be fixed, but we don't do that. 
Depending on where you are located, there are people specializing in repairs. 
If someone has the skills and the equipment needed, it is quite simple to replace the components.
```

---
## \#1296 Posted by: Volts Posted at: 2019-01-28T08:18:21.182Z Reads: 166

```
in that case ill give it a try my self whats the part number for those parts?
```

---
## \#1297 Posted by: trampa Posted at: 2019-01-28T08:19:13.636Z Reads: 168

```
Send me a mail: frank at trampaboards dot com
```

---
## \#1298 Posted by: trampa Posted at: 2019-02-22T09:52:58.204Z Reads: 151

```
The VESC 6 Plus just landed in the UK.
 http://www.trampaboards.com/vesc-6-plus-benjamin-vedder-electronic-speed-controller-p-26762.html

The VESC 6 Plus is a complete re-design of the VESC 6, unlocking some of the powerful features of the VESC 75/300 in the VESC SIX package.
```

---
## \#1299 Posted by: taz Posted at: 2019-02-22T09:55:40.828Z Reads: 152

```
Apart from the UAV features (accelerometer etc) what are the differences compared to the normal VESC 6 for eskating applications?
```

---
## \#1300 Posted by: trampa Posted at: 2019-02-22T13:24:38.631Z Reads: 152

```
The 6 plus features adjustable voltage and current filters, so it is super smooth and detects any motor very precise, IMU (accelerometer, gyro compass), re-designed logic, added robustness in the low voltage rail, footprint for NRF51 installation, Can run fast inrunners and detect motors with low inductance. 
Is a three phase shunt design, like VESC 6.
Fully prepared for upcoming features of VESC-Tool.
Reduced price.
```

---
## \#1301 Posted by: The_Dude Posted at: 2019-02-25T12:25:32.123Z Reads: 149

```
@trampa Just to make sure, I thought that an IMU was already in the first VESC6 release (I bought one as a beta tester)?
```

---
## \#1302 Posted by: trampa Posted at: 2019-02-25T13:35:09.728Z Reads: 141

```
The 6plus has a different IMU chip, since the IMU of the 6 is no longer made and active. Benjamin never coded anything for that old IMU. The VESC 6 never had the IMU place, but features a footprint for MPU9150.
```

---
