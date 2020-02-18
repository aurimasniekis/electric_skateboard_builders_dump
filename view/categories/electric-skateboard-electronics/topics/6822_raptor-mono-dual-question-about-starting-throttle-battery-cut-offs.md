# \[Raptor Mono/dual\] Question about starting throttle battery cut-offs

### Replies: 47 Views: 2969

## \#1 Posted by: Skitzor Posted at: 2016-07-29T16:05:04.116Z Reads: 154

```
Hi all,

I've been a raptor owner for two months now. After having some child diseases ironed out and some basic stuff I had to repair. All in all a fantastic piece of equipment. Yet there is one more annoyance I like to clear out, which wasn't present in  the first few weeks, but came into play some time later. I don't know exactly when. but since it has been a (minor but annoying) problem... I've heard similar problems from other owners. (@El_Cid so far as i know) 

My setup:
Space Cell pro 3, dual VESC (one 3300 uF CAP for both) and two 6355 R-specs.
My weight is 75kgs

My BLDC settings:
<img src="/uploads/db1493/original/2X/d/d15e082a1af99978768db84ac73b647145c54c12.PNG" width="690" height="393">

That's how I received it from Enertion. I've changed the Motor max to 60 so it is a little less responsive (read slower accelleration)

Now my problem:
In the beginning it didn't matter how hard I hit that throttle.  The deck would throw me off and go for a ride on it's own. Now If I even push it 1/4 up without a kickpush to start. The Battery shuts down.
Is there anyone here who could help me figure out that problem. I've played with the vesc settings as much as I could. Nothing would make this go away. It's frustrating

I have this problem with both my space-cells. So I'm sure it should be something in the settings...

Video's:
https://www.youtube.com/watch?v=0wyIzDYC4zU 
https://www.youtube.com/watch?v=6QnRkLBS2Tc

They are from may 18th. I've had the board like 3 weeks back then as the problem showed up

@onloop, You've seen my video about this. But I'm pretty sure it wasn't present as I first got it.
```

---
## \#2 Posted by: El_Cid Posted at: 2016-07-29T16:32:08.462Z Reads: 139

```
I'm so glad I'm not the only one with this problem! mine does the exact same I have a raptor dual and running each vesc at 25a max batt. the fuse doesnt blow it just shuts off even if its at 97% battery if i hit the acceleration hard it all of a sudden reads 0% and turns off. i cycle the power and it comes back.. always does this unless I accelerate very gently but once going its totally fine. when i first got the board it was a rocket and i could barely stay on... pls peeps help usss!
```

---
## \#3 Posted by: Skitzor Posted at: 2016-07-29T16:58:45.281Z Reads: 137

```
One possible traject could be the cap of 3300 uF
Since most vesc's come with 3x680uF =2040uF for a single, a dual could need 4080uF?
```

---
## \#4 Posted by: El_Cid Posted at: 2016-07-29T17:21:41.764Z Reads: 135

```
Yeah but why did it work fine before with the same 3300uf cap and not now? I have a feeling it has something to do with the battery BMS board thinking the battery is lower than it is so it shuts off to protect it. now I'm just basically waiting to see if @onloop will jump in and suggest something either crack the battery open and inspect or arrange for a new battery as this is a serious issue that I'm surprised no one else has even commented on.
```

---
## \#5 Posted by: Skitzor Posted at: 2016-07-29T17:23:50.574Z Reads: 126

```
BMS is my second suspect. Then I'm guessing we tripped something on there. But since this only is at startup its so strange (I know it uses the most amps to get from zero to something)

If I check the bldc window with live amps it pulls something like 42A before it trips. Question is, if this is wanted behaviour from the BMS, why didn't it happen at first.

@El_Cid, lets be patient, I'm sure onloop is going to pass by. Let the community brew on it, it's magical !
```

---
## \#6 Posted by: Photorph Posted at: 2016-07-29T19:46:35.069Z Reads: 121

```
I wonder if the VESC caps have anything to do with it all... Since you said it was working fine at first.  Someone who knows BMS electronics and VESC settings better than me needs to chime in.
```

---
## \#7 Posted by: Dedbny Posted at: 2016-07-29T23:19:14.256Z Reads: 120

```
Im sure @onloop will chime in on this as he always makes an effort for his Raptor crew.  Just be patient. Hes copping flack with the usual customer order frustrations.   It is now the weekend here now. Winter blah. 

Try searching more on forum to see if any vesc setting issues. While your waitung for response.  So much stuff on here.  Did you make changes to Vesc through BLDC.  

My vesc settings were adjusted at the shop and has been great. I never start on stop,  only ever push start which is what onloop recommends.  Puts extra strain on motor which you can avoid.  Also I think its more natural and smooth way of starting off. 

Good luck.
```

---
## \#8 Posted by: Skitzor Posted at: 2016-08-01T14:06:14.789Z Reads: 110

```
Could this have something to do with it? I'm going to check tonight if it's the case...
http://www.electric-skateboard.builders/t/psa-remember-to-reset-your-max-current-ramp-step-when-programming-your-vesc/6262
```

---
## \#9 Posted by: Skitzor Posted at: 2016-08-01T19:06:56.354Z Reads: 104

```
Allright, The VESC bug is not the problem, although my settings were at 50,000 for both vescs due to continiously changing settings to find my problem.

If I make the motor max 40 I cannot get the board to shut down anymore. As proven in previous testing 42 amps was where it cutted the battery off. (Yet the space Cell is rated for 60A since it's 3p)

Why is nobody chiming in on this thread. :frowning: 

It has worked in the first three weeks with 80Amps and 60 Amps settings for throttle control.

So can we conclude there's something wrong with both my BMS's since they start to cut off at 40 Amps?
```

---
## \#10 Posted by: El_Cid Posted at: 2016-08-03T15:47:29.978Z Reads: 99

```
@onloop please help us out... Should we be looking inside the battery? could we have our batteries replaced? theres got to be something that can be done...
```

---
## \#11 Posted by: Skitzor Posted at: 2016-08-03T17:37:28.045Z Reads: 96

```
Sorry I hadn't updated this thread yet. @El_Cid 

Latest: I've e-mailed support monday. Got a reaction from Linda Tuesday. Jacob will look at it in the next 3 days she said.
```

---
## \#12 Posted by: El_Cid Posted at: 2016-08-07T01:33:20.473Z Reads: 96

```
Have they said much yet?...
```

---
## \#13 Posted by: Photorph Posted at: 2016-08-07T06:12:17.322Z Reads: 95

```
yea I'm curious to know what happened with this?
```

---
## \#14 Posted by: Skitzor Posted at: 2016-08-08T09:32:47.435Z Reads: 93

```
I'm going to spam @onloop and @jacobbloy one more time, this definately needs some looking in to. Have sent reminders to support on friday and this morning. But so many raptors are sold. So many guru's here with BMS and VESC knowledge and nobody gave his 2 cents, weird !
```

---
## \#15 Posted by: Photorph Posted at: 2016-08-08T09:48:51.402Z Reads: 89

```
Support should get back to you within a week I would say.  If they didn't maybe email them again from a different email address, I wonder if certain email addresses go to their spam/junk folder.
```

---
## \#16 Posted by: Skitzor Posted at: 2016-08-08T09:53:22.344Z Reads: 90

```
They usually reply within 2 days. This time I got Linda again and this problem is quite technical. She said to forward it to Jacob, we'll see. I've already got 2 warranty shipments done (vesc and motors, within 2 weeks to Belgium) so that's quite nice ! No complaints here. I'm now running it at 40 amps. It's still fun, but feels like it has lost half of the power since the beginning. Battery goes further too with that limit...

edit: It's like missing the Insane mode button on a Tesla :smiley:
```

---
## \#17 Posted by: jacobbloy Posted at: 2016-08-08T10:00:56.945Z Reads: 91

```
hey mate can you just give me your order number i will see what battery you have, most likely you have one of the battery with a 50A cut off and it is tripping early. the best thing to do is set the battery current to 15A on both vesc then go for a ride, if it doesn't cut of then you know its the BMS, the one thing i can suggest if it is the BMS and you want to keep riding your board is to bypass the BMS and rely on the vesc current limiting for discharge and only use the BMS for charging. but then you will loose the switch function.

but after a little bit of experimenting we would come up with the solution for you.
```

---
## \#18 Posted by: Skitzor Posted at: 2016-08-08T10:49:33.818Z Reads: 94

```
order #2151 around may. I've got 2 space-cells with the same issue. 
Even if I put the vesc limits at 10-15 amps it's still pulling 42 amps at startup.
According to the description of the spacecell back then it should only cut at 60 amps right?
The only thing I have found to work is limit the throttle current to 40 amps ( coming from 80 amps that worked)

Edit: @jacobbloy
```

---
## \#19 Posted by: jacobbloy Posted at: 2016-08-08T12:39:38.863Z Reads: 90

```
whats the no load current of the motors?
```

---
## \#20 Posted by: Skitzor Posted at: 2016-08-08T13:06:57.617Z Reads: 91

```
@jacobbloy everything is at enertion standard settings, with motor max tuned down to 40A at the moment and battery max at 25 per vesc. Not sure what you mean by no load current for the motors...
```

---
## \#21 Posted by: Nordle Posted at: 2016-08-08T14:03:04.092Z Reads: 88

```
Could be a weak cell in your pack.
i assume space cell is 3p 25r that would be 60A, if one is faulty there are only 40A left and if you exceed these you get massive voltage sag and low voltage cutoff from vesc

try to set max amp (battery) to 15A per motor, thats low i know, you'll have limited torque but if the problem is solved then it's probally one faulty cell

 _~e~ are you mongo pusher?^^_
```

---
## \#22 Posted by: Skitzor Posted at: 2016-08-08T14:10:55.035Z Reads: 91

```
Yes I'm a mongo pusher loool, does that make me weird ? :smiley: 

Everything you say is correct. Samsung 25R Cells, 10s3p config. Should be 60 amps...
Wouldn't it be strange to have it with the 2 space-cells at the same time? I mean a bad cell in both...
Yet one of them is only charging to 89%, so that's a bigger problem than the other...

I cannot open up the space-cells cause of warranty and lack of heatshrink to close them again. They're only close to one month old and in real use for about a week of actually providing power to the board...

Edit: btw, whatever I put in the max battery, it doesn't change the operation of the board. at 15A/VESC, the board shuts down at 42 Amps. Tested that with BLDC-tool still connected for output.
```

---
## \#23 Posted by: Nordle Posted at: 2016-08-08T14:32:41.566Z Reads: 85

```
Ok that was my fault, i didnt read the whole thread^^
I just asked about mongo pusher cause i see it how you step on your board:D
```

---
## \#24 Posted by: jacobbloy Posted at: 2016-08-08T21:26:28.599Z Reads: 85

```
This doesn't seem right, change all of your current settings to 15a then test. It should limit the current.

Any way it could be a faulty MOSFET switch also.
```

---
## \#25 Posted by: El_Cid Posted at: 2016-08-11T01:03:02.536Z Reads: 87

```
Ok so I've reduced the max batt amps to 15 on each vesc, have made sure the max current ramp is set to 0.004 before writing so it ends up as 0.04. And my battery still goes from 99% to 0% as soon as i try to accelerate at full throttle and turns off. once off if I turn the switch off and then back on it goes right back to 99%... if I dont accelerate hard and get a good rolling start it seems to do okay but it did that with the max batt set to 25A or 15A. when I first got my board it never did this... infact it came from enertion programmed at 30A max batt and it was a friggin rocket.. i mean i hit the throttle and fought to stay on. now if I do the same it cuts out and I come to a rolling stop... Ive also tried e-mailing support and got no response at all... come on guys... @onloop @jacobbloy.
```

---
## \#26 Posted by: jacobbloy Posted at: 2016-08-11T02:08:11.626Z Reads: 86

```
I only work for enertion from a few hours a week sorry. But I'll keep this issue on the thread but I'm feeling it is a MOSFET switch issue and I need to try and replicate the issue to find the fix. But if this process fails we can look at replacing the battery
```

---
## \#27 Posted by: El_Cid Posted at: 2016-08-11T02:34:29.609Z Reads: 85

```
Okay perfect thank you! :) also notice quite a bit of sparking when i plug the charger into the battery. not sure if thats indication of anything but I thought this was supposed to be antispark or is that just for the switch?
```

---
## \#28 Posted by: Skitzor Posted at: 2016-08-11T07:50:39.182Z Reads: 81

```
Thanks @El_Cid for confirming. Haven't had time this week because I'm abroad for work. Now that you mention it, yes my charger has started sparking as well when I plug it in.
Edit: that is both the quick and slow charger
```

---
## \#29 Posted by: Dedbny Posted at: 2016-08-11T08:48:51.018Z Reads: 79

```
I always plug into board then flick the power switch.  No spark then.
```

---
## \#30 Posted by: El_Cid Posted at: 2016-08-11T23:47:50.218Z Reads: 77

```
Which mosfet are you referring to? I'm willing to run some tests. I have all the tools and a DMM I just want to make sure you guys are okay with me doing so without voiding the waranty. the only thing i would not be able to replace is the shrink tubing thats on the battery. if this fixes it I'm willing to wrap the battery myself and just keep it as is. but if it needs replacing then okay cool but if I can fix it then all good.
```

---
## \#31 Posted by: Skitzor Posted at: 2016-08-12T17:34:40.632Z Reads: 76

```
Hello again. My heatshrink arrived for the possible re-wrap of the space-cell. If someone of you (@jacobbloy/@onloop) could point me in the right direction for tests to perform (which mosfet). And if I don't lose the warrenty to investigate this for you... Everything Possibly needed is at hand. (Shrinkwrap, Fluke multimeter, oscilloscope, soldering iron, ...)

So give me some input for both problems (and most importantly warranty!) .

-1st battery is charging only to 89%. What should i check? I'm guessing broken cells/balance lead.
-both batteries shutting down at 40 amps. Which mosfet? which circuit?

Please, this has been an issue (40 amps) since week 3 with the raptor. The 89% only showed up since I started this thread...
```

---
## \#32 Posted by: El_Cid Posted at: 2016-08-15T17:01:12.059Z Reads: 71

```
@longhairedboy This is the rest of it.
```

---
## \#33 Posted by: longhairedboy Posted at: 2016-08-15T17:39:46.060Z Reads: 71

```
gotcha. I'll link this into the ticket.
```

---
## \#34 Posted by: longhairedboy Posted at: 2016-08-15T17:46:38.518Z Reads: 72

```
In this situation i would probably just replace the BMS and see how it goes from there. I have a handful of the older space cell BMSs. If you want to send the pack to me i can do that for you, you have my address. If its bad cells then the whole thing would need to be replaced, I don't replace individual cells or try to revive packs with imbalances.
```

---
## \#35 Posted by: Skitzor Posted at: 2016-08-15T19:56:24.852Z Reads: 69

```
@longhairedboy, I'm in Europe :( could we work something out to get an old BMS from you ?
```

---
## \#36 Posted by: longhairedboy Posted at: 2016-08-16T13:11:21.743Z Reads: 68

```
email enertion support and see what they say.
```

---
## \#37 Posted by: Skitzor Posted at: 2016-08-16T13:41:40.872Z Reads: 67

```
Allright, movement for my case as well. @nexty I tag you so you could have a look in here.
```

---
## \#38 Posted by: nexty Posted at: 2016-08-16T14:20:56.363Z Reads: 72

```
Hey Skitzor,

I did receive your email this morning, apologise for the delay Im currently on a day trip for a customer to Amsterdam and Im on my way back,

Let me review the case and discuss this internally you are more then welcome to meet each other at the workshop I'll contact you tomorrow 

Thanks for the notice using the tag ;-)
```

---
## \#39 Posted by: Skitzor Posted at: 2016-08-16T15:12:29.604Z Reads: 69

```
Take your time man, I'll be working in Atlanta usa and Yorkton Canada the next two weeks, so no rush at all...
```

---
## \#40 Posted by: Skitzor Posted at: 2016-08-23T03:41:29.927Z Reads: 67

```
@onloop, I know it is once to often, but seriously, I feel like you're ignoring this issue man.
I'm not counting on warranties, even though this all happened in the same month. I can hardly believe I'm the only one together with @El_Cid. This is a pre-made board. Reason why I ordered it to behold me of mistakes...
```

---
## \#41 Posted by: onloop Posted at: 2016-08-23T05:36:57.622Z Reads: 67

```
hey, i am not ignoring problems.... I am sorry it might feel like you are not getting my attention, but i am working on a big picture solution.

I spend nearly every hour of every day working on building up (/completely re-working) our systems to ensure our valued customers get quality answers to their questions & get problems solved & parts replaced in a timely manner

so maybe i don't personally answer everyone's email, & repair everyone's raptors myself but we are trying to ensure the processes are in place to get it done quickly and to high standards.


here is the process.
1. email support@enertionboards.com (basic fault diagnosis)
2. get referred to repair agent.
3. send your board/parts for agent for review/repair.
4. repair agent diagnose fault & orders parts
5. we send parts.
6. parts get replaced & tested.
7. board/parts gets returned working.


If i tried to fix everyone's problems single handily & didn't have systems in place my business would collapse.

if there is something you wish i would say or do please just say so & I'll try my hardest to do it.
```

---
## \#42 Posted by: Skitzor Posted at: 2016-08-23T15:38:14.328Z Reads: 66

```
Thanks for your time! Appreciate it.

It's not that I request you to do this personally for me. But however if there is something I could check out to help you proceed with analyzing the problem this is a win-win situation right ?
So far I've been sent from pillar to post. Not complaining, because I know and understand the relationship with the repair agent is just in the early stages.
But as far as we have communicated he said he is waiting on feedback from you. Hence why I've pinged you in this topic once again. Nothing more, nothing less

I've agreed with Quentin I'll go to him personally with the space-cells. Because the board is still working I don't want to have too much downtime with shipping parts around. 

I'm roughly guessing he doesn't have parts yet for the batteries except from completely built space-cells.

As most people have contributed on this topic, we suspect the BMS (Jacob thinks a specific Mosfet). Replacing it could fix the problem, but not prevent it from happening again.
```

---
## \#43 Posted by: erinbobo Posted at: 2016-08-25T19:21:54.183Z Reads: 59

```
Hey Erin Bobo here. Damon since I got my raptor back from you I've been having this same problem. My board cuts out on me when I try and accelerate. I used to be able to go up hills no problem and now it's cutting out on very small hills. You just fixed my space cell and put in a new VESC. Anything I should adjust on my BLDC tool?
```

---
## \#44 Posted by: Skitzor Posted at: 2016-08-26T07:41:22.936Z Reads: 54

```
Could you do a little test for us in this thread, 
Hook your raptor to bdlc, go to the live view amps and hold it with all your force in place and go full throttle on it (or stand on it if that's easier)

The exact thing I'm looking for is the 40 amps cut-off.
```

---
## \#45 Posted by: Skitzor Posted at: 2016-08-26T18:25:00.164Z Reads: 48

```
Could you do a little test for us in this thread, 
Hook your raptor to bdlc, go to the live view amps and hold it with all your force in place and go full throttle on it (or stand on it if that's easier)

The exact thing I'm looking for is the 40 amps cut-off.
@erinbobo
```

---
## \#46 Posted by: erinbobo Posted at: 2016-08-26T21:40:34.655Z Reads: 49

```
Yeah when I have time this weekend I'll test it and let you know.
```

---
## \#47 Posted by: Hatman30 Posted at: 2017-11-20T13:07:06.177Z Reads: 22

```
Any updates with this at all?
When I go full throttle my motors cut out for a second and I have to release the trigger, then it’s fine again. 
My motor max is set to 40 as default by the looks of things
```

---
