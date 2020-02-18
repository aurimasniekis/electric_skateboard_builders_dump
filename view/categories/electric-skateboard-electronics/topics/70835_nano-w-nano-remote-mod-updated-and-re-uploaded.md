# Nano-W &#124; Nano Remote Mod \[Updated and Re-uploaded\]

### Replies: 159 Views: 3925

## \#1 Posted by: Winfly Posted at: 2018-10-11T04:42:07.952Z Reads: 543

```
Got sick of the small battery in my Nano X and the small throttle throw so I upgraded it. Might as well take out the unnecessary stuff and add some simple features.

+2000mAh lipo.
+Deadman switch
+Bigger radius thrumb wheel
-channel 2 button
-reverse button

Still got that stupid ass calibration tho. :cry: 
![15392327564833534908820325639572|375x500](upload://A2XtpFQCwfmw0kjucxjWtwp1gJ4.jpeg)
![image|246x500](upload://g2KvbUWFhzFR4isWcZRa8wjXekS.jpeg)


Edit: (10/12/18)
Ok. I was dumb and thought i could just splice a wire and add a button in the middle.
Here was the situation,:
1.   if button was on V, signal rails to ground when trigger is released (full brake)
2.   if button was on G, signal rails to V when trigger is released (full throttle)
3.   if button was on S, signal floats to 3/4 V when trigger is released

I fixed it using (3) and adding a voltage divider to stabilize the signal to 1/2V (center of ppm) using 2 10k omp resister. I chose 10k cus that's the highest I have atm. theoretically you can go higher as long as they are identical.

![image|246x500](upload://4CRyqGzzGdqU3xTefEzXsAl0fEQ.jpeg)

https://youtu.be/WZFWofeVias
```

---
## \#2 Posted by: Blacksheep Posted at: 2018-10-11T04:44:31.451Z Reads: 473

```
What calibration?
```

---
## \#3 Posted by: Winfly Posted at: 2018-10-11T04:45:54.282Z Reads: 460

```
when you turn on the nano you need to full swing the thumb wheel to let it know its range to calibrate or it will be very touchy
```

---
## \#4 Posted by: Blacksheep Posted at: 2018-10-11T04:49:11.790Z Reads: 448

```
That’s why it’s touchy hehehe thanks for the info
```

---
## \#5 Posted by: Winfly Posted at: 2018-10-11T04:55:50.645Z Reads: 428

```
lol no problem I knowledge was passed down to me. apparently it's on the Raptor 2 manual but as you might know the nano X manual is shit.
```

---
## \#6 Posted by: skatardude10 Posted at: 2018-10-11T05:18:08.912Z Reads: 408

```
Nice! Got some files, build log, parts list... ? I'm interested!
```

---
## \#7 Posted by: Grozniy Posted at: 2018-10-11T09:00:13.838Z Reads: 389

```
Great mod :muscle:
```

---
## \#8 Posted by: Winfly Posted at: 2018-10-11T10:09:52.887Z Reads: 370

```
files later still need to use it a while to see if i like the shape. part list is 1x Nano Remote and 1x 2000mAh lipo. thats all it is.
```

---
## \#9 Posted by: Schulerbible Posted at: 2018-10-11T10:24:30.531Z Reads: 361

```
It took me 2 years to figure that out. And it wasn't touchy every time, just randomly.
```

---
## \#10 Posted by: rey8801 Posted at: 2018-10-11T10:42:50.712Z Reads: 350

```
On mine is written on the remote itself, plus on the manual. When I forget to do it, It's really clear mostly during braking.
```

---
## \#11 Posted by: Winfly Posted at: 2018-10-11T11:09:13.608Z Reads: 333

```
yeah it's random af. sometimes you dont need to recalibrate after turning it on and off (with the receiver kept on). that's why im adding this deadman switch and upgraded battery so I can leave the remote on to save my calibration when we stop to charge in a groupride.
```

---
## \#12 Posted by: Schulerbible Posted at: 2018-10-11T11:28:00.890Z Reads: 318

```
My brakes felt like as if there is no throttle range, like a binary on off switch. Going downhill and having a brake in ludicrous mode is no good :slight_smile:
```

---
## \#13 Posted by: Winfly Posted at: 2018-10-13T02:07:41.806Z Reads: 292

```
updated 10char
```

---
## \#14 Posted by: tardyparty7 Posted at: 2018-11-18T21:08:57.798Z Reads: 287

```
u got the Prints?
```

---
## \#15 Posted by: Winfly Posted at: 2018-11-19T02:50:49.977Z Reads: 284

```
I can upload the STL tonight but I don't really like the shape atm. Need to print a few more prototypes.
```

---
## \#16 Posted by: Winfly Posted at: 2019-01-24T21:10:30.244Z Reads: 277

```
Finally Published it. give it a try and let me know how you feel.

https://www.thingiverse.com/thing:3378933
```

---
## \#17 Posted by: gmurad Posted at: 2019-02-12T04:44:17.603Z Reads: 261

```
Will this work for modding the Nano V2 as well? I'm not sure but thought they were the same inside.
```

---
## \#18 Posted by: Winfly Posted at: 2019-02-12T05:28:06.556Z Reads: 252

```
Yeah they are the same inside.
```

---
## \#19 Posted by: Bobby Posted at: 2019-02-12T05:47:59.525Z Reads: 242

```
So i have a nano x laying around but i have no clue about what capacitors and what to solder where. Im pretty new to electronics and just learned how to solder Mind breaking that down a bit? Maybe a drawing when you have time?
```

---
## \#20 Posted by: Winfly Posted at: 2019-02-12T06:09:39.246Z Reads: 232

```
Yeah sure. The mod is really easy. I'll draw a diagram later.
```

---
## \#21 Posted by: landonkun Posted at: 2019-02-12T20:27:59.604Z Reads: 217

```
This is great! I'm gonna print one out for myself. I have big hands, so the Nano-X always felt pretty small.
```

---
## \#22 Posted by: Jansen Posted at: 2019-02-12T22:46:12.973Z Reads: 208

```
IS the deadman switch only a deadman switch and that's it or can it be used as cruise control instead I'm hoping...? Also, are you going to send out a parts package for people who want to do this by chance or is it a completely DIY fend for yourself type of mod / situation?
```

---
## \#23 Posted by: Jansen Posted at: 2019-02-12T22:46:45.935Z Reads: 201

```
Great work BTW, looks great and will be doing it since I have a spare nano-x remote laying around
```

---
## \#24 Posted by: gmurad Posted at: 2019-02-13T06:12:07.984Z Reads: 195

```
How is there a deadman switch now with no extra hardware (I saw the material list in thingverse)? Is it reusing a button that wasn't used before from the remote itself?
```

---
## \#25 Posted by: Winfly Posted at: 2019-02-13T06:14:44.292Z Reads: 198

```
I took it off from the channel 2 button. otherwise the button is pretty generic, you can find them easily.
```

---
## \#26 Posted by: Winfly Posted at: 2019-02-13T09:18:49.149Z Reads: 206

```
@Bobby
 here's a MS paint dragram LMAO. uses 2x 10k+ resistor and desolder the button from bottom left of the pcb.

![image|540x458](upload://453gBXSwWIDilRgLOLgQmrUYm7d.png)
```

---
## \#27 Posted by: yelnats8j Posted at: 2019-02-13T20:38:21.124Z Reads: 192

```
What print settings do you recommend ?
```

---
## \#28 Posted by: Winfly Posted at: 2019-02-13T22:04:04.400Z Reads: 198

```
I would print a rough one with PLA first to see if you like the shape. Personally I think the shape have much to improve. I need some feedback from ppl to motivate me to change the geometry. :sweat_smile:
```

---
## \#29 Posted by: yelnats8j Posted at: 2019-02-13T22:09:06.650Z Reads: 206

```
Already on it
I let you know how it feels when its done

![15500957096777955471373068155841|375x500](upload://yTsg4i2hO96jvRGCV4PS5GF8VRP.jpeg)
```

---
## \#30 Posted by: Bobby Posted at: 2019-02-13T23:05:25.686Z Reads: 199

```
If you could let me know the time it takes to make, id appreciate it a lot!!! Gonna be doing this at my public library and want to get a time table
```

---
## \#31 Posted by: Winfly Posted at: 2019-02-13T23:18:56.688Z Reads: 201

```
printing at 60mm/s 0.2mm height, top bottom 4 layers, 3 shells. give or take add another hour to that.
![image|690x359](upload://38aGEZONX2b6Yx70MWnNsOigNnX.png)
```

---
## \#32 Posted by: yelnats8j Posted at: 2019-02-14T01:25:46.874Z Reads: 200

```
![15501073124667979643864762677538|375x500](upload://hQRIsgpcBbO82Agv03soo1FnVVL.jpeg) 


It fits preaty well in my hand, but it could be a little thinner and thats about it. Or more round on the figer side for comfort 

Also is it only held together by pressfit right now?
Or am I missing something
```

---
## \#33 Posted by: Winfly Posted at: 2019-02-14T01:45:00.141Z Reads: 183

```
there should be 3 screw holes. on the back side. rip I might have broke my files when i adjusted it. let me re-upload them.
```

---
## \#34 Posted by: landonkun Posted at: 2019-02-14T01:54:39.581Z Reads: 175

```
Wait, what! You tell us this after I already printed one?! Haha.

The snap fit seems fairly tight though. I can't see mine coming apart unless I really tried to pry it apart.
```

---
## \#35 Posted by: Winfly Posted at: 2019-02-14T01:56:15.374Z Reads: 179

```
lol it really depends on the quality of your print I guess. 
@yelnats8j can you elaborate on what to change? would be awesome if you can draw it on your pic.

edit: the holes weren't through all the way. I uploaded fixed STL just now.
```

---
## \#36 Posted by: yelnats8j Posted at: 2019-02-14T02:15:43.719Z Reads: 176

```
Would i be able to drill or no?

Also i will after I get the feel for it a little more
```

---
## \#37 Posted by: Winfly Posted at: 2019-02-14T02:23:14.603Z Reads: 179

```
yeah can can also just drill them there just won't be a counterbore for the screws to sit flush. there are 4 holes on there already. my current one only use 3 out of the 4 (not using the top one)
```

---
## \#38 Posted by: yelnats8j Posted at: 2019-02-14T02:34:29.588Z Reads: 188

```
Alright so far my only complain is the trigger. Its a little shakey moving side to side
![15501116270842875737523386334175|375x500](upload://qQoHXHOvHnhpaT66PXhjSXcvFsU.jpeg)
```

---
## \#39 Posted by: Winfly Posted at: 2019-02-14T03:05:35.209Z Reads: 182

```
lets hold off until I get everything fix. that's not supposed to happen. might have gotten some wrong files when I uploaded it. sorry for inconvenience.
```

---
## \#40 Posted by: yelnats8j Posted at: 2019-02-14T03:07:19.191Z Reads: 181

```
No problem its just a test anyways. 
Definitely a upgrade from the normal nano tho.
```

---
## \#41 Posted by: landonkun Posted at: 2019-02-14T03:19:18.605Z Reads: 182

```
Ah, you're right. I hadn't assembled the thumb wheel before. Is it loose even with the electronics inside? Either way, I feel like the gap should be closed off more to protect from water/rain. You could even just print a thicker thumb wheel for the time being.

I have bigger hands, so I always have trouble with the wheel being right under my thumb joint, instead of the soft part of my thumb. Would be nice if it was a little higher, but I dunno how that would affect other people. Either way, this is a nice design.

![00000IMG_00000_BURST20190213211327918_COVER|375x500](upload://iLSMRuWj49x2KTRxL54ZtZ1E1pA.jpeg)
```

---
## \#42 Posted by: landonkun Posted at: 2019-02-14T03:40:23.736Z Reads: 178

```
When your printer is calibrated juuuust right 😍

![00000IMG_00000_BURST20190213213414429_COVER|666x500](upload://9KdApcZwNIJoGL3p3HcjkwCCjb.jpeg)
```

---
## \#43 Posted by: yelnats8j Posted at: 2019-02-14T03:42:08.878Z Reads: 169

```
What printer?
```

---
## \#44 Posted by: landonkun Posted at: 2019-02-14T03:45:40.479Z Reads: 168

```
Ender 3. I've been using this CF PLA from Enotepad, and it produces by far the cleanest prints out of any filament I've tried so far. Prints just as easily as normal PLA, but even better. The red is just normal PLA.

Can't find it on amazon.com right now (seems to come and go), but I bought mine here in Canada:
https://www.amazon.ca/Filament-Enotepad-Printing-Materials-Dimensional/dp/B07FXWMQLS/
```

---
## \#45 Posted by: yelnats8j Posted at: 2019-02-14T03:47:50.617Z Reads: 170

```
Ender 3 pro or ender 3?
Right now I share a cr 10s with my brother.
Great sometimes but really needs some work.
Hopefully Ill be able to get one in time there look really good.
```

---
## \#46 Posted by: landonkun Posted at: 2019-02-14T04:00:52.475Z Reads: 165

```
Regular Ender 3. I bought it recently, so it came with a lot of upgraded things compared to the Ender 3 from a few months ago. I didn't think the Pro was worth the money. I wound up doing other small upgrades to it instead. I've heard good things about the CR-10S. I would definitely buy a Creality printer again someday. I keep recommending the Ender 3 to people who want to get started.
```

---
## \#47 Posted by: Winfly Posted at: 2019-02-14T04:19:07.622Z Reads: 159

```
i have both. what's the small upgrades for the ender3?
```

---
## \#48 Posted by: landonkun Posted at: 2019-02-14T08:20:44.893Z Reads: 162

```
Just things like upgrading the bed springs myself, glass bed, better PTFE tube, etc.
```

---
## \#49 Posted by: Winfly Posted at: 2019-02-14T08:38:47.633Z Reads: 171

```
Just printed another one myself since I need to replace my beat up one anyways. Yeah the model I uploaded is slightly different than what I had. I'll reupload again with slight modifications.

My older model is only 22mm tall whereas the one I uploaded is 24. I quite like this girth, so I guess I'll upload different thickness models later.

* I've always found the index finger dividing part is too pointy and kinda hurt my index finger over time. So it is rounded and I added a fillet on the chamfer.

* also extended the trigger on the exterior so it's easier to press.

![IMG_20190214_003154|234x500](upload://ys52PlizAKkKOjLw9DnU3moBDvr.jpeg)![IMG_20190214_003941|234x500](upload://jFxVVlW2WAUIhaICrcl2PWuad2x.jpeg)
```

---
## \#50 Posted by: gmurad Posted at: 2019-02-14T11:23:19.572Z Reads: 159

```
I like this last version, is it on thingverse? 

I just printed the hammer head mod but I have 2 Nanos so I will also make a nano-w
```

---
## \#51 Posted by: banjaxxed Posted at: 2019-02-14T14:06:07.681Z Reads: 163

```
hmmm, latest Cura says no to my 0.8mm nozzle for unsupported

![image|595x500](upload://69xEB8XBZCXOUB45T69mZUUheVG.jpeg)

Otherwise going great, I just noticed a little splurge off print, this is solid gyroid, it’s a thing
![image|375x500](upload://mwJsDcgQZnPJsU53CEiVpl1pKKk.jpeg)
```

---
## \#52 Posted by: Winfly Posted at: 2019-02-14T14:18:06.689Z Reads: 160

```
I would suggest hold off printing high quality print right now. There are a few things I need to fix / change. Also the thumb wheel and trigger aren't the right size. I'll get the best dimensions and update them.
```

---
## \#53 Posted by: venom121212 Posted at: 2019-02-14T14:32:48.751Z Reads: 158

```
Awesome, thank you for taking the time to work on this. Not sure if you saw my horrible nano-x failure the other day...
```

---
## \#54 Posted by: banjaxxed Posted at: 2019-02-14T15:56:25.635Z Reads: 161

```
Yessir!  Build plate supported would probably be best for this angle![image|281x500](upload://td9xbKw55zsjszi7G3gN7mSgle0.png)
```

---
## \#55 Posted by: venom121212 Posted at: 2019-02-14T16:35:51.507Z Reads: 153

```
Support is usually generated by the slice software
```

---
## \#56 Posted by: banjaxxed Posted at: 2019-02-14T16:46:41.918Z Reads: 157

```
If selected...

I shoulda done this...build plate support 
![image|690x442](upload://f4Pgsb6eFp1IlyqzBbZt1cLEns.jpeg)
```

---
## \#57 Posted by: landonkun Posted at: 2019-02-14T20:48:49.431Z Reads: 155

```
If/when you upload new models, I'd love having the option of having one with screw holes and one that's just held together by the snap-ins :slight_smile:
```

---
## \#58 Posted by: Indiangummy Posted at: 2019-02-14T20:50:57.416Z Reads: 153

```
Have you had any luck printing nylon with the stock nozzle? I recently also bought a ender and I'm just trying to get t a list of things I need to upgrade
```

---
## \#59 Posted by: venom121212 Posted at: 2019-02-14T20:53:15.216Z Reads: 153

```
$25 Glass bed from amazon is the first thing you should purchase. There's a lot of printables that help like the bullseye fan. Updating the FW is free and not too hard. Direct extruder is my next potential upgrade
```

---
## \#60 Posted by: Winfly Posted at: 2019-02-14T20:53:22.215Z Reads: 148

```
not sure how to design a snap in one that will hold together lol. maybe snap in with a screw on the side right above the speed mode switch.
```

---
## \#61 Posted by: landonkun Posted at: 2019-02-14T21:00:06.217Z Reads: 149

```
@Indiangummy

Haven't tried nylon yet. I think you can buy certain variations of nylon that might work stock, but otherwise nylon can require temps that go way too high for the PTFE tube, among other things, and I'd also probably need to build an enclosure to keep temps regulated. Too much work for me. Maybe someday in the future.

@venom121212

My old Monoprice printer was a direct drive. I honestly didn't notice ANY difference in how things print. If anything, I can print faster with bowden. I know flexible filaments work better with direct, but I don't really print anything like that. Maybe a fancy direct drive setup would change my mind. I've looked into a bunch of random stuff, but for now.. my printer seems to be accommodating my needs :slight_smile:

@Winfly

The model I printed out without the screw holes snaps together perfectly fine and won't come apart unless I really pry at it, so maybe keep a version like this, but with other updates? :relieved:
```

---
## \#62 Posted by: Winfly Posted at: 2019-02-14T21:52:33.611Z Reads: 149

```
ok i think im keeping the rounded finger part that divides the index finger. what do you guys think about adding a fillet here? (fillet at the index finger part is here to stay.) personally i dont mind the sharper chamfer.
![image|483x500](upload://1hvr16cf2yqpued8W4M8oZblOZP.png)
```

---
## \#63 Posted by: venom121212 Posted at: 2019-02-14T22:01:21.106Z Reads: 141

```
I like it, especially for right handed riders
```

---
## \#64 Posted by: Winfly Posted at: 2019-02-14T22:06:12.125Z Reads: 140

```
it will be on both sides.
```

---
## \#65 Posted by: venom121212 Posted at: 2019-02-14T22:12:36.487Z Reads: 141

```
Even better
```

---
## \#66 Posted by: Winfly Posted at: 2019-02-15T05:49:35.447Z Reads: 151

```
After a day I, finally made enough changes and have everything aligned [mostly] properly. My prints are not super good. I forgot my extrusion multiplier for the ender3 and the store setting wasn't right. I will upload everything now.

if you have already printed them. you should print these new files instead because the usb port opening wasn't aligned.

Changes are:

* Added fillets at some edges
* Extended Trigger
* Correct trigger and thumb wheel height/width
* Corrected usb port opening
* Overall girth of the remote is 24mm (same as the one currently uploaded)
* deeper cutout for the trigger button and more walls behide it.


![IMG_20190214_214531|234x500](upload://bToHgpTZBGpdlFNn6rpBemsP798.jpeg) ![IMG_20190214_214525|234x500](upload://uyPUPPIeAHMahMlPUOUY73lAGAv.jpeg) ![IMG_20190214_214545|234x500](upload://bSJTSBRVWDf7e2zw8QX8jh9jtrm.jpeg) ![IMG_20190214_214517|234x500](upload://j33NumH3VyQmGxA0aohmfPFhB7w.jpeg) ![IMG_20190214_214458|690x323](upload://9eJOKMMm0fUhg0omoUGjJfJEQTh.jpeg)
```

---
## \#67 Posted by: Winfly Posted at: 2019-02-15T06:32:39.705Z Reads: 143

```
ok they are updated now. there are 2 thumbwheel models, v7.1 is basically the same as the old one but  wider, v7 has a slightly bigger (0.5mm) inner arc radius for a looser and smoother wheel. once you rest your thumb on the wheel, they dont feel any different.
```

---
## \#68 Posted by: banjaxxed Posted at: 2019-02-15T14:06:45.952Z Reads: 144

```
cool thanks man, I was heading that way
![image|621x500](upload://n9XMDJAnBFuPRLfq2m4YlWLzTay.png)
```

---
## \#69 Posted by: venom121212 Posted at: 2019-02-15T16:50:49.581Z Reads: 142

```
I've never used dead man's trigger before.. I imagine you have to keep it held the whole time to engage motor?
```

---
## \#70 Posted by: Indiangummy Posted at: 2019-02-15T18:12:09.778Z Reads: 141

```
this guy claims to print nylon with the stock setup. could this be true?
https://youtu.be/a8Z-9ncYsps?t=372
```

---
## \#71 Posted by: Winfly Posted at: 2019-02-15T23:08:38.014Z Reads: 146

```

here's the dimension of the v7.1 if you need it.

11.5mm tall

![image|466x441](upload://5lHxgiQip7B6Wu4OhF2MAYRKd1o.png)
```

---
## \#72 Posted by: banjaxxed Posted at: 2019-02-15T23:09:40.478Z Reads: 138

```
Thanks pal
```

---
## \#73 Posted by: banjaxxed Posted at: 2019-02-18T00:02:09.369Z Reads: 140

```
The deadman’s switch could also be thicker?
```

---
## \#74 Posted by: xsynatic Posted at: 2019-02-18T00:35:19.772Z Reads: 138

```
Not sure how Nylon compares with TPU. I use TPU too with my stock ender 3.
```

---
## \#75 Posted by: Indiangummy Posted at: 2019-02-18T00:36:28.136Z Reads: 137

```
Haven't explored tpu, gonna a look into it. Thanks!
```

---
## \#76 Posted by: Winfly Posted at: 2019-02-18T08:26:11.676Z Reads: 138

```
Np. I just reuploaded everything again with updated file names.

added a no trigger version. a bigger trigger as per requested and a regular style thumb wheel.

not sure if I have ever linked it. this is the lipo I use. 

https://hobbyking.com/en_us/turnigy-2000mah-1s-1c-lipoly-w-2-pin-jst-ph-connector.html
```

---
## \#77 Posted by: gmurad Posted at: 2019-02-18T15:43:55.452Z Reads: 133

```
Hey, I printed the main shell overnight just before you uploaded a new version. I noticed the internals changed slightly (remove one screw, changed internal wall a bit, etc) and I printed the triggers this morning from the new design. Should I reprint?

This remote feels really nice on my hand.

btw, my printer had a lot of problems with the NANO-W text and the holes for the screws came out closed, will fix it with a drill. These are probably issues with my printer. I printed at 0.15 layer height and PETG.
```

---
## \#78 Posted by: Winfly Posted at: 2019-02-18T21:39:28.373Z Reads: 132

```
I think you printed the very first file I uploaded. I would suggest you to reprint it. The current version is much better. Sorry about that. I think I have made all the changes I wanted on the case atm so there will be no more changes on this thingiverse link specifically. If there's other stuff I wanna add, I'll make a new thingiverse link.
```

---
## \#79 Posted by: landonkun Posted at: 2019-02-18T21:52:18.541Z Reads: 132

```
I wouldn't mind trying the wheel with that kind of pattern. Did it work out for you? Any way you can upload the STL file? :slight_smile:
```

---
## \#80 Posted by: Winfly Posted at: 2019-02-18T21:54:50.060Z Reads: 133

```
@banjaxxed if you share the file, I can put it on the link too. With proper credit ofc.
```

---
## \#81 Posted by: gmurad Posted at: 2019-02-18T23:12:01.846Z Reads: 125

```
No worries! Already printing the latest version in black PETG
```

---
## \#82 Posted by: banjaxxed Posted at: 2019-02-19T00:34:20.202Z Reads: 121

```
Sure! Need to print it first tho, tomorrow
```

---
## \#83 Posted by: gmurad Posted at: 2019-02-22T05:56:57.984Z Reads: 121

```
Noticed the model changed again on the 19th, is that a significant change? Just printed 2 a few days ago
```

---
## \#84 Posted by: Winfly Posted at: 2019-02-22T07:53:44.117Z Reads: 126

```
Nope I just made the holes and counter bored a little bit deeper. So the screws can grab better beyond the trigger. No major change.
```

---
## \#85 Posted by: gmurad Posted at: 2019-02-23T16:09:12.484Z Reads: 120

```
![image|690x335](upload://l6YZhk5nbawWNbvohD8zAvDxKmW.jpeg) 

Left is Prussament PLA printed on teh Prusa MK3S
Right is PETG printed on the CR10S PRO
```

---
## \#86 Posted by: landonkun Posted at: 2019-03-01T02:18:16.486Z Reads: 115

```
Good to know I'm not the only one whose PETG turns out less than stellar (no offense).

I've tried COUNTLESS suggestions, including other peoples' specific Cura profiles for the Ender 3, but can never get anywhere near the same results, even trying three different brands of filament.

I'm close though. I don't want to give up, but damn is it ever disheartening sometimes.
```

---
## \#87 Posted by: Winfly Posted at: 2019-03-01T02:29:26.097Z Reads: 115

```
I havent tried too many brands but HatchBox is my go to.

235C/70C 40mm/s

but honestly for a remote PLA is more than good enough.
```

---
## \#88 Posted by: gmurad Posted at: 2019-03-01T02:31:07.767Z Reads: 116

```
Not sure what you are talking about, the PETG turned out almost perfect. Those thin strands that you see are easily removable with your finger or with a heat gun. Maybe the flash from the camera is throwing you off?
```

---
## \#89 Posted by: landonkun Posted at: 2019-03-01T02:45:36.926Z Reads: 113

```
Possibly. It looks a bit warped and blobby in a few spots, but it could just be the flash/finish of it.

I'm just spoiled by how good PLA always turns out.

@Winfly I did do the remote in PLA, but I've been trying to perfect PETG for enclosures and stuff like that. Maybe I'm setting my standards too high :smiley:
```

---
## \#90 Posted by: Winfly Posted at: 2019-03-01T02:47:10.981Z Reads: 112

```
yeah. PETG is great and all but it's just a little too sticky. unless you nail it down, it will never be as good as PLA prints.
```

---
## \#91 Posted by: M.Hboards Posted at: 2019-03-01T03:29:39.538Z Reads: 111

```
Is it possible to get the files without the nano w ingraved also just wondering what do the 10k resistors do?
```

---
## \#92 Posted by: Winfly Posted at: 2019-03-01T05:36:23.083Z Reads: 108

```
it's a voltage divider. so when the trigger is not press, sensor value return to the center.

with a little be of editing i'm sure you can erase the letters yourself.
```

---
## \#93 Posted by: Bundymus Posted at: 2019-03-02T20:19:20.977Z Reads: 103

```
In the thingiverse instructions it says to use a thin strip of smooth paper in installation of the deadman's switch, how is it used?
```

---
## \#94 Posted by: Winfly Posted at: 2019-03-02T21:03:41.712Z Reads: 104

```
It's for the thumb wheel. If your print isn't very smooth, put it between the inner diameter of the thumbwheel and the casing to not have your thumb get stuck.
```

---
## \#95 Posted by: yelnats8j Posted at: 2019-03-09T16:20:46.160Z Reads: 107

```

![15521483786181140520909052107201|375x500](upload://cCt8npsyHHsbOT7pCAsoSWJsE4R.jpeg)
```

---
## \#96 Posted by: yelnats8j Posted at: 2019-03-09T16:35:50.489Z Reads: 107

```
Decided to skin it in True CF looks amazing
Gonna give it another shot with different color PLA

![15521492759547819247852169760112|374x500](upload://dHUFNvlKEmaxvK17cWdMIckrKQ7.jpeg)
```

---
## \#97 Posted by: Winfly Posted at: 2019-03-24T16:52:14.434Z Reads: 112

```
Took some pictures when I assembled a second one. Pictures should be in order.

Solder on the battery.
![IMG_20190316_025318|690x388](upload://fVM5xNC0GyF3q2vkGPFG0pYCgG6.jpeg)

Remove channel 2 button for trigger.
 ![IMG_20190316_025330|281x500](upload://gX8LvH9bwAvpXGR389j3yBHB3tk.jpeg)

Trim the button into size.
 ![IMG_20190316_025502|690x388](upload://6Vz0ihg79eWtP7oD5B8I99fOQ4t.jpeg) 

Button should fits right there. You can move it up and down a little to change how the trigger feels. 
![IMG_20190316_025643|690x388](upload://d9w8llO94MK3O03vHaSMNNV9GOY.jpeg) 

Voltage divider when trigger is not pressed.

![IMG_20190316_030315|690x388](upload://rQcQpkXZ6hnxosnFxHjaCtgJvwW.jpeg)

Cut the middle wire and solder to each end to complete the trigger.
 ![IMG_20190316_030833|690x388](upload://qNmurMaozlYaEypPFIIsutQlCSq.jpeg)

Cut that long ass button to bare.
![IMG_20190316_030921|281x500](upload://z3FK4HAdg1wODASGWpJtn7OqBHv.jpeg) 

After that, tuck all the wires into the channel and try to close the top. When everything is in place it will close shut tightly with a littl resistance from the battery popping out.

P.S. when you turn on the remote, you would still need to calibrate the throttle range. So hold down the trigger when you do that.
```

---
## \#98 Posted by: banjaxxed Posted at: 2019-03-24T16:59:23.471Z Reads: 103

```
Thanks great instructions
```

---
## \#99 Posted by: Bobby Posted at: 2019-04-01T07:07:49.243Z Reads: 101

```
![image|375x500](upload://asnARc2p05veqA72LjO3iNX874U.jpeg) 
Love the feel of this remote! Converting both nano-x’s to use this design. Fits the hand great and that extra battery life is clutch!!!
```

---
## \#100 Posted by: Jansen Posted at: 2019-04-02T20:06:53.013Z Reads: 103

```
Can one of the fine and friendly gentlemen on hear be a true scholar and print a fellow esk8 brotha the printed parts needed for this mod and send them to me in SoCal by chance..... pretty please and thank you in advance..... :-)  Happy to PayPal some funds for the time and postage etc (not looking for a free one unless someone wants to offer that) but I have a extra nano-x and need a good remote for my next build with the TB DD's and 110's that are supposed to ship this week. 

Oh and I don't need the dead-mans switch if that changes anything. Is there just a whole if you don't use the dead-mans switch or is there a print to fill that in for people who don't use it?

LMK and thanks so much in advance to anyone who can help me out. Would prefer the best quality print and material possible FYI.

PM or hmu here.
```

---
## \#101 Posted by: Bobby Posted at: 2019-04-02T20:40:38.174Z Reads: 100

```
Talk to my boy @redbaron. Charges around 15 for the print. He is in San Diego
```

---
## \#102 Posted by: Jansen Posted at: 2019-04-02T21:09:33.458Z Reads: 98

```
Whats good wid it mr. @RedBaron? Can you hook me up por favor...? LMK what the deal is, I'm ready to grab a print ASAP. Very cool you live just south of me. I am due for a trip down to SD to visit a buddy so maybe I can just plan that for a weekend or two out and link up with you while I'm down there...? Go for a ride too if we can....? LMK and thanks in avdance brotha.
```

---
## \#103 Posted by: RedBaron Posted at: 2019-04-02T21:36:25.418Z Reads: 101

```
I could definitely hook you up my man. I've got a cool red translucent and black Petg on order. I can order other colors, just give me a heads up. Like bobby said $15, and if you don't feel like waiting $8 for 2 day shipping. I'm working on getting a better deal shipping wise. @Jansen
```

---
## \#104 Posted by: Jansen Posted at: 2019-04-03T19:28:30.306Z Reads: 99

```
Word @RedBaron IM SOLD! I already modded my mini remote with the avio mod in red so don’t really want that color and my feather remote is black so don’t really want that and would like to have something different.... you don’t have any other colors on deck though....? Would love a dope green (kinda feeling neon  and that would actually match my deck perfect because I have the moonshine outlaw Which has neon green polyurethane rails around the whole board…)  don’t really want to wait superlong though so let me know if those are my only two color options at the moment and if you are down for ordering other colors then let me know how long that would take if you don’t mind… thanks brotha. Can’t wait to get it printed up and in my hand!
```

---
## \#105 Posted by: Bobby Posted at: 2019-04-04T05:17:03.240Z Reads: 86

```
Damnnnn.... i want green.
```

---
## \#106 Posted by: RedBaron Posted at: 2019-04-04T18:29:53.405Z Reads: 82

```
For sure, let me look for a suitable green and ill get back to you. On average it takes two days to receive the filament. If it takes longer ill let you know.
```

---
## \#107 Posted by: RedBaron Posted at: 2019-04-04T18:35:58.805Z Reads: 80

```
I found a pretty sweet semi transparent neon green petg. I just ordered it, says it should be here tomorrow.
```

---
## \#108 Posted by: Jansen Posted at: 2019-04-04T19:18:40.746Z Reads: 80

```
Fuuuuuuuuck yes. That sounds sick, way down. You got a pic by chance? Down either way. LMK as soon as it can be picked up or mailed and ill figure out what Im gonna do. Do you use the deadman switch on your remote? I don't like them so didn't want it but am wondering if I still need to have that added button/trigger there, or if there is a version where that is just sealed so there isn't just a hole if I didn't want to have the trigger switch there. It can't be used for cruise control like on my feather since it's really just a swap and not a from scratch build right? Thanks again brotha @RedBaron
```

---
## \#109 Posted by: landonkun Posted at: 2019-04-04T19:20:12.746Z Reads: 78

```
In the download for the STL file there are two versions: one with trigger and one without (sealed). ;)
```

---
## \#110 Posted by: RedBaron Posted at: 2019-04-04T19:24:24.391Z Reads: 84

```
Heres the pic of the color. And yes the folder has a few variations of the remote. So neon green remote with no deadmans switch. I can have it done by Saturday if all goes well. And yeah its just a swap of the internals.![_AC_SY400_|493x400](upload://fhYhpdFfhaWxztlUeoaz8rjvTgP.jpeg)
```

---
## \#111 Posted by: Jansen Posted at: 2019-04-04T19:40:21.679Z Reads: 84

```
You da man brotha, making my day and my next build I'm about to wrap up and this thing will be peeeeeerfect. Can't wait. I actually might be going down to chill for a day or two in SD this weekend so lmk when it's done and we can either link up, or if I don't end up making it down I will have you drop it in the mail. Thanks again my dude.

That color looks fucking siiiiiiiiick! Could I do a black thumbwheel for the main front and back pieces this green?
```

---
## \#112 Posted by: RedBaron Posted at: 2019-04-04T21:09:19.920Z Reads: 81

```
No worries, black thumb wheel with green body, got it!
```

---
## \#113 Posted by: landonkun Posted at: 2019-04-05T00:52:34.683Z Reads: 80

```
Mmm that sounds sexy. I made one black body with red trigger, and one red body with black trigger.
```

---
## \#114 Posted by: RedBaron Posted at: 2019-04-05T23:49:44.558Z Reads: 78

```
Filament came in today, I'm starting the print in a few minutes. I'll keep you updated.
```

---
## \#115 Posted by: Jansen Posted at: 2019-04-05T23:53:36.676Z Reads: 81

```
[quote="RedBaron, post:114, topic:70835"]
starting the print in a few minutes. I’ll keep you updated
[/quote]

Woot woot! Sounds excellent. Will be staying in OC this weekend so I am going to have you mail that shit up to me. PM'ing now fine sir. You da man!
```

---
## \#116 Posted by: gmurad Posted at: 2019-04-06T12:11:11.846Z Reads: 81

```
Ideally the deadman's switch would only affect the accelerating and not breaking but this is probably not possible without software is it?
```

---
## \#117 Posted by: gmurad Posted at: 2019-04-06T18:16:07.044Z Reads: 83

```
Re-printing with toy like colors so it can never be confused with a gun handle

![image|690x335](upload://so7Q0T32oyH7a3SOqwD2beXBEf1.jpeg)
```

---
## \#118 Posted by: Battosaii Posted at: 2019-04-06T18:22:17.265Z Reads: 81

```
Going to try this out, i do like the closed fingerhole cause you can let go of the remote and not drop it but i like how your internals look might make the trigger butter smooth.
```

---
## \#119 Posted by: gmurad Posted at: 2019-04-08T00:01:08.546Z Reads: 83

```
Bad news to report.

I've printed about 5 of these remotes and each version was improved from the last. I used my best version yesterday for the first time and did about 15km, at one point I lost control of my board and didn't understand why but didn't think it was the remote.

Today I went for a ride again with another remote that had this mod, it was fully bench tested and in that environment it didn't have any issues, but on the road the thumbwheel got stuck while accelerating and I got in an accident, I won't talk much about it but it might take a while to recover and be able to operate an e-skate again. I guess remotes is something to be very careful when DIYing.

@Winfly When analyzing the casing of the nano-w and comparing to the nano v2 my recommendation to avoid this would be to not create a "slot" for the thumbwheel inside the casing and instead make the thumbwheel hole for potentiometer shaft tight and just deep enough. That's how the nano v2 does it and it works really well. Any chance you would give this a try?
```

---
## \#120 Posted by: Winfly Posted at: 2019-04-08T01:05:10.191Z Reads: 80

```
I can look into it. Fyi it really depends on how smooth your print is and the starting point of your layers. I also recommend adding smooth paper between the thumbwheel and the case to make it even smoother. I've done that to mine and it's butter smooth.

Are you ok? How bad was the crash?
```

---
## \#121 Posted by: Bobby Posted at: 2019-04-08T02:34:44.771Z Reads: 80

```
I cant say ive had the same experience. Zero cutouts, zero sticking issues and survived me eating shit when
Y battery cut out. Maybe the nano v2 is a just lil different than the nano-x?
```

---
## \#122 Posted by: Battosaii Posted at: 2019-04-08T19:28:42.208Z Reads: 77

```
A little bit of lithium grease can help smooth out the trigger too. Not to much all you want is enough for a thin coating so it dosnt get everywhere. 

I plan on using the remote with out the dead man swith activated.
```

---
## \#123 Posted by: Winfly Posted at: 2019-04-08T21:28:01.082Z Reads: 81

```
the trigger has minimal travel. just the travel of the button, so like 1-ish mm.
```

---
## \#124 Posted by: RedBaron Posted at: 2019-04-08T23:11:53.879Z Reads: 81

```
Your printer is underextruding a bit. Bump up that extrusion multiplier up one or two so those gaps go away.

Ps. Can you make the notch a little wider and further away from the edge? Its a little to close and sometimes brakes.

![20190408_161433|690x287](upload://Ahg96Fu8Nc52xo0ab5uKJXj74lP.jpeg)
```

---
## \#125 Posted by: Winfly Posted at: 2019-04-08T23:52:54.416Z Reads: 83

```
I will look at it later tonight.
```

---
## \#126 Posted by: gmurad Posted at: 2019-04-09T00:29:18.927Z Reads: 84

```
Thanks for being open to it. I've printed about 6 or 7 of these so far on different printers and different materials. The one that got stuck (only 1 time but it's enough to wreck you) was a very smooth print. I think the problem is that my prints are not dimensionally accurate, being a little bit off is enough to make the thumbwheel stick.

Either way there is no need to create a channel for the thumbwheel inside the casing, if we are already talking about adding the thin smooth paper or grease I think for safety reasons it's best to instead change the design to what I was suggesting above(like the Nano V2 does it) or something similar. I think it's too great of a risk to take (e.g.: what if the smooth thin paper moves out of the way?) if there is a viable safer alternative.

Regarding the accident I will be ok, it will just take a bit of time for my leg to recover but I think I can be back on the e-skate for the summer.
```

---
## \#127 Posted by: RedBaron Posted at: 2019-04-09T20:39:02.060Z Reads: 72

```
I took a razor and smoothed out every contact patch inside the thumb wheel. No problems with sticking.
```

---
## \#128 Posted by: gmurad Posted at: 2019-04-09T20:52:26.017Z Reads: 74

```
It must have been very rough if you needed to use a razor! Either way I don't know how you can make a curved surface smooth and even throughout the curve with a razor.
```

---
## \#129 Posted by: RedBaron Posted at: 2019-04-09T21:26:04.094Z Reads: 77

```
It wasn't very rough, I just did it for good measure. And its not hard to smooth a round surface with a razor if you have a steady hand and a good eye.
```

---
## \#130 Posted by: Battosaii Posted at: 2019-04-15T13:25:33.087Z Reads: 75

```
My first one printing okay. The tip above where your index finger goes came out a bit boogery but nice print over all.

Going to use a smooth glass bed and better quality filament with my next print. 

![20190414_202915|374x500](upload://viwPPIRtqTg7F1PVTS2qiQh67LN.jpeg) 

Feels really nice, the trigger throw is longer and there no longer that clicky feel when you go full throttle or full brakes.
```

---
## \#131 Posted by: Battosaii Posted at: 2019-04-15T20:34:36.751Z Reads: 73

```
Btw what screws are you guys using? I have m3 10mm long and they work but only 1 screw got tight the others stripped out easily.
```

---
## \#132 Posted by: Jansen Posted at: 2019-04-15T20:41:41.763Z Reads: 68

```
m2 12mm is what I used and worked good
```

---
## \#133 Posted by: Jansen Posted at: 2019-04-15T20:44:53.367Z Reads: 74

```
3 in black socket head I thought looked clean and is the perfect length ![image|375x500](upload://uej2BNKFuRYr9ZEiCog00ehvPC2.jpeg) ![image|375x500](upload://1jmZaTEcuovjVoRqq9c1VS19wfy.jpeg)
```

---
## \#134 Posted by: Battosaii Posted at: 2019-04-15T21:02:02.093Z Reads: 65

```
Wow i feel like m2 would just fall in the hole.
```

---
## \#135 Posted by: Jansen Posted at: 2019-04-15T21:14:56.960Z Reads: 68

```
Maybe depends on what you printed with...? Mine were actually tight going in and had to almost drill it out some with the screw as they went in. You can ask @RedBaron what he did on the print different than you.... (as you saw from the post about me being untrustworthy....:kissing_heart: )
```

---
## \#136 Posted by: Battosaii Posted at: 2019-04-15T21:20:38.292Z Reads: 65

```
I doubt it was my print setting cause everythng else electronic wise fit like a glove.
```

---
## \#137 Posted by: RedBaron Posted at: 2019-04-15T21:25:38.016Z Reads: 68

```
All printers depending on the slicer software have fluctuation in scale, you will never get two identical parts from a 3d printer. Sometimes outline perimeter layers also slightly effects hole sizing. I use 3 to 4 outline perimeter layers for strength in holes that accept screws.
```

---
## \#138 Posted by: Battosaii Posted at: 2019-04-15T22:24:26.900Z Reads: 69

```
You are right im a 3d printing noob. I used 3 walls ill try a bit thicker my next print.
```

---
## \#139 Posted by: Battosaii Posted at: 2019-04-16T12:00:16.995Z Reads: 65

```
Finished a print with polymaker polymax filament and some supports and the print came out much nicer.

![20190416_071412|666x500](upload://zUGNFtvQIeQwoWIBLRaEsBP8I9h.jpeg) 

![20190416_071458|666x500](upload://sTJ0QqPR7DYZx7qLsgfMOlfnJoD.jpeg)
```

---
## \#140 Posted by: Battosaii Posted at: 2019-04-17T20:42:53.353Z Reads: 60

```
@Winfly i dont see a place to add a lanyard but i saw a pic of one of your earlier models using a lanyard. Where did you put yours? Id like to not drop my remote by accodent.

![20190416_212347|375x500](upload://qmHmJZE1P3hundWWc7hTbN1SbjU.jpeg)
```

---
## \#141 Posted by: gmurad Posted at: 2019-04-17T20:49:49.343Z Reads: 58

```
I added it between the power switch and the usb port. On another Nano-W I put it under the screw (the bottom one).
```

---
## \#142 Posted by: gmurad Posted at: 2019-04-17T21:01:28.283Z Reads: 61

```
I also thought of another way to make the thumbwheel super safe and just more premium. Imagine if the thumbwheel was a full circle, with a hole in the middle for a small bearing and a mount for the bearing in the casing. The potentiometer gets moved to the bottom left of the wheel with it's shaft inside it. Here is a terrible drawing:

![image|629x500](upload://9TUu0uqhkedrL12Vod3mcyzdB8w.png)
```

---
## \#143 Posted by: Battosaii Posted at: 2019-04-17T21:01:49.991Z Reads: 60

```
Thats a good idea im going to add those tonight before the ride. Ill be testing one on the group ride and im bringing an extra to see if anyone else wants to ride with a nano w
```

---
## \#144 Posted by: Battosaii Posted at: 2019-04-17T21:04:24.398Z Reads: 63

```
That would be arguably more dangerous because for that to work the shaft of the potentiometer would have to constantly slide in and out of the thumb wheel and that can cause a wonky trigger feel and very fast wear in the plastic.
```

---
## \#145 Posted by: gmurad Posted at: 2019-04-17T21:14:36.602Z Reads: 62

```
humm, I didn't consider the wear caused by the friction, that's not ideal. The wheel would be pushing the shaft left and right tho and I don't think it would be a problem if some material at the tip of that triangle got worn down. My original suggestion a few posts up is probably simpler tho which was `to not create a “slot” for the thumbwheel inside the casing and instead make the thumbwheel hole for potentiometer shaft tight and just deep enough.`
```

---
## \#146 Posted by: Battosaii Posted at: 2019-04-18T18:50:56.684Z Reads: 59

```
Trip report.

I made 2 of these remotes and i brought them to the group ride last night i used one and another friend used the other for the entire ride. The remote is amazing i love the feel in the hand and we both loved the longer trigger throw especially on our fast boards. The boards no longer felt twitchy just super smooth.

I only wish the index finger grove was a complete circle like the winning remote so that i can open palm the remote with out dropping it, i like to do this to give my hand a rest from time to time.and helps dry the hand sweat.
```

---
## \#147 Posted by: Bobby Posted at: 2019-04-18T18:57:31.092Z Reads: 60

```
[quote="Battosaii, post:146, topic:70835"]
only wish the index finger grove was a complete circle like the winning remote
[/quote]

Ewww no... maybe add some fabric or something for the sweat on the handle. I hate that “circle around the index finger” look
```

---
## \#148 Posted by: RedBaron Posted at: 2019-04-18T19:12:10.976Z Reads: 54

```
I really like how the entire remote is. Only thing id like to see is 4 screw holes instead of 3. But honestly this is my favorite 3d printed remote by far. Dont fix whats not broken! Lol
```

---
## \#149 Posted by: landonkun Posted at: 2019-04-18T19:18:57.192Z Reads: 50

```
Did you modify your thumbwheel at all to make it smoother?
```

---
## \#150 Posted by: Battosaii Posted at: 2019-04-18T19:30:05.594Z Reads: 52

```
Not in the print i just did about 30 seconds worth of sanding on the thumbwheel. It made everything work smoothly.
```

---
## \#151 Posted by: Winfly Posted at: 2019-04-18T19:59:47.195Z Reads: 54

```
taking advise from @gmurad  i'm modifying the hole that the joystick pokes into the thrumbwheel. so that the inner circle is not rested on the case anymore. I am still making a few adjustment to make it absolutely right. hopefully i can get it nailed down by tonight. if it all goes well. all you need is print a new thrumbwheel and not the entire case.
```

---
## \#152 Posted by: Winfly Posted at: 2019-04-19T07:30:20.613Z Reads: 56

```
@gmurad try this one and let me know. file is on thingiverse named "Nano-W Thumb Wheel 2 v2".
![image|239x208](upload://n4I95xvum5maeAziXNCTCldNQpH.png)

 the two holes are slightly offset so you can flip it around to see which side is looser.

https://www.thingiverse.com/thing:3378933/files


 ![15556584189618912264842689825666|250x250](upload://f9xQRZkFb6ziLwgNQPlEicMHzSN.jpeg)  ![15556583575508754025113081533316|250x250](upload://l7HvX3h0Zz6YwqenLg64u5jPVfp.jpeg)
```

---
## \#153 Posted by: landonkun Posted at: 2019-04-19T08:07:04.561Z Reads: 57

```
Gonna give this bad boy a try tomorrow.
```

---
## \#154 Posted by: gmurad Posted at: 2019-04-19T15:33:26.543Z Reads: 55

```
Thanks @Winfly! I printed a few and it's massive improvement. 

I had to take 0.2mm out from one side (PCB side) and 0.75mm from the other side (just using windows 10 3d builder). With the original width it could still get stuck in the casing if I pressed the case hard. (This is the limit of my current 3d modeling skill)

![image|242x499](upload://lRUeZqBQsADrEHPYZQKUmLSYuJ0.jpeg) 

Now regarding the circle thickness, under certain circumstances I can still make the inner circle rub against the casing and make it stick, are you able to thin the thumb wheel a bit more? It's really close to being fool proof and tolerating 3d printers with some dimensional inaccuracies.
```

---
## \#155 Posted by: xsynatic Posted at: 2019-05-17T15:27:48.902Z Reads: 50

```
Not Sure what i'm doing wrong.

I can't seem to get it fit, wether its the case or the thumbwheel. if i look at @gmurad 's print, holy shit thats clean.
The slits are way to small for the insert.

Using Ender 3 with 0.2mm
Heavy sanding to make it look "good"

Printing took 4 1/2 hours.![photo_2019-05-17_17-26-11|375x500](upload://6NZBBcsdKgjjZQfSqHewvCjmdLc.jpeg) ![photo_2019-05-17_17-26-18|375x500](upload://wcu6YtKWj1q19hmmqKZfCbpOLsU.jpeg) ![photo_2019-05-17_17-26-23|375x500](upload://zTMyomzeykE13ImM4TnwYROapzj.jpeg)
```

---
## \#156 Posted by: landonkun Posted at: 2019-05-17T18:46:53.511Z Reads: 44

```
I'm noticing a bit of bubbling in your top layers. What material are you printing with?
```

---
## \#157 Posted by: Winfly Posted at: 2019-05-17T18:47:56.327Z Reads: 44

```
The whole print is wobbly maybe extrusion multiplier too high and not enough top layers.
```

---
## \#158 Posted by: xsynatic Posted at: 2019-05-17T23:52:45.240Z Reads: 44

```
PLA. I never had so much bubbling tbh.
```

---
## \#159 Posted by: McErono Posted at: 2019-05-18T19:46:49.745Z Reads: 34

```
Totally forgot the great work of winfly. Had it in my thingiverse collection since last year :see_no_evil:

Today I did a rough print.
Man I love it! What an improvement!

![20190518_213837~2|375x500](upload://492nC7ARHCndJq1w6ZH1aC3Gan7.jpeg) 
![20190518_213903~2|447x500](upload://toUk9igYPrQM0PUkidtnJm5lcMI.jpeg)
```

---
