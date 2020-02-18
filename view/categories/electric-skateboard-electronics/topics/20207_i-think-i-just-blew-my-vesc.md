# I think I just blew my VESC?

### Replies: 27 Views: 2067

## \#1 Posted by: Guacamoleface Posted at: 2017-04-03T18:53:55.031Z Reads: 207

```
So I finally decided to try FOC after running. 
I've read a bunch of topics about this lately due to the fact I wanted to see if there was a common reason for people blowing their DRV with FOC and alot came down to none-isolated motor cables and/or changing back and forth between bldc, or having wrong firmware version.

Isolated my cables. Followed torqueboards instruction video on youtube.

Did detection as in video and applied. 
Using the arrowkeys on keyboard without load was very disfunctional, didnt work all the time(which seem to be normal behavior in FOC). But I noticed after the detection it smelt slightly burnt and also it gave DRV8302 error the times when it did not work on the arrows.

I checked my parameters - everything seemed to be correct. Decided to try it on ground. It rolled with me on it.
Tried it a couple times. One of the time it didnt wanna start. I moved it alittle and it started.

Its been running failfree on BLDC abit before this but never gone back and forth between FOC and BLDC.
My versions are 2.18 firmware and vesc is a DIYELECTRICSKATEBOARDS v4.12 vesc.
10s4p - samsung 25R. Torqueboards 6374 motor.

Is my DRV toast?
Does anyone have a clue why this would be the case?


Motormax: 60
Motormin: 30
Battmax: 60
BattMin: -12

Min volt: default
Max volt: 57v
cutoffstart: 33v
CutoffEnd: 30v


I tried to find this issue on the forum but couldnt. And alot of threads were from early development on FOC so people may sit on more knowledge in this section now.


Best regards - pontus
```

---
## \#2 Posted by: Blasto Posted at: 2017-04-03T19:05:09.101Z Reads: 191

```
can you confirm that it is giving a DRV fault by going in to the terminal and typing "faults"... sounds to me that it is another fault code

what is your absolute max current?

I would put battmax to 30A (ok maybe 40A)
```

---
## \#3 Posted by: Guacamoleface Posted at: 2017-04-03T19:11:28.385Z Reads: 186

```
[quote="Blasto, post:2, topic:20207"]
hat is your absolute max current?
[/quote]

130A is absolute max.
 Battery is at 60A (its rated for 80a).

And I was looking live analyzis in the "realtime data" and it gave me the DRV8302 on fault.
```

---
## \#4 Posted by: Blasto Posted at: 2017-04-03T19:19:30.530Z Reads: 174

```
if you go back to BLDC does the fault happen again?

if the fault does not occur, may have badly written the FOC settings (not your fault, I've had the BLDC tool bug on me where hit write and it does not (don't get the mc confirmation)). You could go through the FOC detection again
```

---
## \#5 Posted by: Guacamoleface Posted at: 2017-04-03T19:59:06.386Z Reads: 156

```
Could try, havent dared to since that used to be one of the most common ways to burn the DRV, swapping from FOC to BLDC. But at this point I dont feel like I have anything to lose.

Just reset to default and try. But smelling the DRV now I feel pretty certain its kaput.
```

---
## \#6 Posted by: PXSS Posted at: 2017-04-03T20:58:56.489Z Reads: 143

```
c18 and 26 populated?
I have 2 TB escs and these were not populated correctly which leads to errors on FOC
```

---
## \#7 Posted by: Guacamoleface Posted at: 2017-04-03T21:10:50.386Z Reads: 141

```
Not sure, according to their site it was "Upgraded C18 to 4.7µF". And tested with FOC.
Must've been my settings but I wish I knew how or which since I didnt change anything more then what I typed in this thread. Rest is default.

The card does smell burnt, and it started doing that already when I did the Parameter detect for FOC. Thought it was the motor at first. :confused:
```

---
## \#8 Posted by: Guacamoleface Posted at: 2017-04-03T21:37:29.282Z Reads: 143

```
Except for the smell there is nothing visually showing damage. From what I can see atleast
<img src="/uploads/db1493/original/3X/b/a/baea846c4d5f2d4daf730404dd671d86ca533d11.jpg" width="281" height="500">

<img src="/uploads/db1493/original/3X/1/7/17092b3d33b6ff3d97e7f8860c9c49b0aef85f78.jpg" width="281" height="500">
```

---
## \#9 Posted by: Ackmaniac Posted at: 2017-04-03T21:43:03.707Z Reads: 134

```
If you have the latest firmware the switching between FOC and BLDC is fine. The next version of my app will also have this feature. I would recommend to be at a standstill when you do the switch. It's nothing more than a myth that this killer the drive. I just found out some stuff about FOC and how it can be optimized with the parameters. But I still have to learn and test a bit more before I can give clear advices.
```

---
## \#10 Posted by: Guacamoleface Posted at: 2017-04-03T21:49:47.246Z Reads: 128

```
Alright, I had 2.18, so that should be fine if Im not misstaken. Yeah your app was next in line for my project, that will have to wait abit now. Not sure wether to go for another VESC, or try and get this repaired.

Seems like FOC is still pretty "unknown" and still "Focs" up.(see what I did there). 

Im currently lacking a hotair station so gotta find either one who can do it for me here in sweden, or borrow me a hotair station. 

If you know any good suppliers in EU for vescs, I'd love to know.
Shipping from US is just another 40dollar + wait time. 
Torture riding a board for 10kms then not be able to ride it again :p  especially in the weather we have now!
```

---
## \#11 Posted by: PXSS Posted at: 2017-04-03T22:11:24.593Z Reads: 120

```
Yeah...
I wouldn't believe it.
I ordered four 4.7uF caps for my two escs (a pair for each).
The update between HW 4.11 -> HW 4.12 was a second cap added to c18 (namely c26) which was blank in both of my TB VESCs, I've heard of people having issues with TB VESCs in FOC mode but I haven't heard of Ollin or Enertion have these issues and they do populate it
```

---
## \#12 Posted by: yakerman Posted at: 2017-04-03T22:18:31.277Z Reads: 121

```
I got my VESC from this UK ebay seller.  http://www.ebay.co.uk/itm/VESC-4-12-Motor-controller-open-source-BLDC-Speed-Controller-VESC-vedder-Pcb/182505114102. 

Have run it in BLDC and also FOC with ackmaniacs firmware and its still going strong. Would recommend.
```

---
## \#13 Posted by: Ackmaniac Posted at: 2017-04-03T22:22:16.668Z Reads: 117

```
Which motor do you use with FOC? BTW, my firmware makes no difference when it comes to the reliability with FOC.
```

---
## \#14 Posted by: Guacamoleface Posted at: 2017-04-03T23:00:18.284Z Reads: 114

```
[quote="Ackmaniac, post:13, topic:20207, full:true"]
Which motor do you use with FOC? BTW, my firmware makes no difference when it comes to the reliability with FOC.
[/quote]

I use the torqueboards 6374 motor. 

@yakerman 
Alright, Thanks alot! How was the shipping?

@PXSS 
Ah! Where are you from btw? I'd love to find a reliable source in EU for theese things, long shipping times is a bummer, aswell as sending it for service or replacement(If there is warranty that is).
```

---
## \#15 Posted by: PXSS Posted at: 2017-04-04T02:41:40.218Z Reads: 107

```
USA. Sorry
```

---
## \#16 Posted by: Eboosted Posted at: 2017-04-04T05:50:11.985Z Reads: 103

```
I've been riding BLDC fpor almost 4 months with no issues at all, riding the board was a blast and tonsof fun.

Last week I decided to try FOC. FOC sensored was amazing, really, I mean REALLY SMOOTH, however it lacked of the power BLDC gave me, I had several cutouts at maximum duty cycle, right when I pushed the throttle to the limit, VESC cutted out, made stange unpredictable accelerations and brakings, I almost crashed 3 times.

I checked the faults and I gor the DRV8302 error, I knew I was screwed, however after turning the VESC off and on again, DRV error went away, I inmediately switched back to BLDC strong as always.

I'm not planing to risk a VESC right now, so I mihght try FOC again in the future when the software has more development and FOC runs with no issues.
```

---
## \#17 Posted by: TarzanHBK Posted at: 2017-04-04T08:16:44.407Z Reads: 99

```
[quote="Guacamoleface, post:10, topic:20207"]
If you know any good suppliers in EU for vescs, I'd love to know.
[/quote]

https://www.electric-skateboard.builders/t/worldwide-vesc-directory/16764
```

---
## \#18 Posted by: rwxr Posted at: 2017-04-04T08:22:39.454Z Reads: 98

```
@Guacamoleface: Hello fellow Swede!
Where are you located? If you need a hot air station, there could be maker spaces that has one in you vicinity.
```

---
## \#19 Posted by: Guacamoleface Posted at: 2017-04-04T09:33:53.707Z Reads: 91

```
Hey! Im located just outside malmö. I've been trying to think off places that might have with no luck.
```

---
## \#20 Posted by: Guacamoleface Posted at: 2017-04-04T09:37:12.753Z Reads: 90

```
Yeah with foc it felt like my power dropped on 100% throttle, most likely due to the drv. Where is your vesc from? 
Also does your vesc still function in bldc after all that?
```

---
## \#21 Posted by: rwxr Posted at: 2017-04-04T11:14:12.150Z Reads: 78

```
@Guacamoleface: Nice. I live 90km north-west from Malmö.
Malmö has a makerspace at Stapeln that's open for the public on thursdays. There might be a reflow-machine there or at least someone who knows where to find one.

http://stpln.se/projekt/fabriken/
```

---
## \#22 Posted by: Guacamoleface Posted at: 2017-04-04T12:27:53.019Z Reads: 73

```
Oh yeah, had another one telling me they might have aswell at fabriken, Thanks alot for the tips! I'll contact them and see :) 
Else I might buy a smaller hotair station just for the future. Being able to easily swap the DRV, would be nice not having to be as doubtful about trying new settings and features! :)
```

---
## \#23 Posted by: Eboosted Posted at: 2017-04-04T15:52:26.812Z Reads: 73

```
Yeah, it's working flawlessly on BLDC again. No. More FOC testing for me for now. 

BTW you could save yourself from buying a hot air, I always use this, never used the hot air again:

https://www.amazon.com/gp/aw/d/B0019UZP7I/ref=mp_s_a_1_1?ie=UTF8&qid=1491321078&sr=8-1&pi=AC_SX236_SY340_FMwebp_QL65&keywords=chip+quik

Check some videos on YouTube
```

---
## \#24 Posted by: Guacamoleface Posted at: 2017-04-04T15:56:21.853Z Reads: 71

```
@Eboosted 
I will check that out. Was just looking at hotair stations aswell so good timing :smiley:

Thanks for the tips! 

I wanna be able to swap because it lets me "dare" to mess around with my VESC abit more.
```

---
## \#25 Posted by: Guacamoleface Posted at: 2017-04-04T16:47:44.376Z Reads: 67

```
@Eboosted 
The QuickChip seemed efficient, the only thing I think off is the thermal part(I think it is thermal)underneath the DRV that needs to get soldered to the chip aswell. Could pre-heat it and be really quick to line it up I guess, but not sure how that will be.
```

---
## \#26 Posted by: Eboosted Posted at: 2017-04-04T16:52:02.404Z Reads: 65

```
Give it a try, the chipquick is a low melting compound you could even lift the chip with your fingers, so no need to heat the whole area with expensive hot air stations
```

---
## \#27 Posted by: Guacamoleface Posted at: 2017-04-05T11:13:08.380Z Reads: 59

```
Update: Decided to plug it in again and go into BLDC and reset to default values and re-do my initial setup for the board in BLDC, along with motor detection. Motor detection went fine, inserted my values for batteries and motor.

Board ran fine on the bench - tried to see if I could get the DRV8302 error in bldc, put some load on it, throttle, used brake etc. Could not get a DRV8302 error.

I highly doubt the DRV is fine. I still think its damaged and may act up when Im going outside to try riding it with more load. Highly unlikely its not damaged considered it smellt burnt after the FOC detection and DRV errors.

Shrug
```

---
