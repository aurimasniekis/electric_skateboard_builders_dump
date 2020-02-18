# FOC Mode with Sensored motor

### Replies: 27 Views: 3683

## \#1 Posted by: ArsenalMain Posted at: 2018-02-09T09:25:36.101Z Reads: 417

```
Hi esk8 community, 
Now that Ive got all of my parts coming in the mail, including a:
* 80a continuous discharge BMS
* The Sensored DIY 6374 Motor
* The DIY VESC
* 5x 2s 60c 5Ah Batteries

I now have started to start planning and learn about the Vesc settings. After reading through as many of the FOC and BLDC threads that I could find, such as these: 
http://www.electric-skateboard.builders/t/new-vesc-user-read-this-complete-walktrough-of-the-vesc/2980
http://www.electric-skateboard.builders/t/vesc-in-foc-mode/5263
https://www.electric-skateboard.builders/t/vesc-faq-what-is-foc-field-oriented-control/419
http://www.electric-skateboard.builders/t/who-is-using-foc-and-whats-your-setup/4465
http://www.electric-skateboard.builders/t/focbox-in-foc-mode/33934

I have some questions that I would love answered.

* Number one on this list is if I can use sensored motors on a BLDC setup. Ive read bits and pieces about this but have yet to find a clear answer.

* Secondly, I was recommended by a fellow community member to follow this guide by vedder in setting up FOC

https://youtu.be/bYYNbxPXNEU

If i follow this setup guide to the T, testing the motors and all of that, will I have to adjust any other specs? The reason I ask this is that I have seen multiple people mention parameters such as breaking or regenerative breaking. I do already realize that I need to put in the specs of my specific battery config and current.

* Lastly, do any of you experienced builders have any recommendations with how I should go about the setup?

Thanks, I really appreciate the help.
```

---
## \#2 Posted by: rich Posted at: 2018-02-09T11:36:37.433Z Reads: 324

```
First of all I don't know if the DIY V4.12 is good for FOC, someone else maybe chime in.

[quote="ArsenalMain, post:1, topic:45949"]
if I can use sensored motors on a BLDC setup
[/quote]

Of course, it's called hybrid BLDC mode (the startup performance is better with FOC but with hybrid you have better low RPM performance than normal BLDC)

[quote="ArsenalMain, post:1, topic:45949"]
Secondly, I was recommended by a fellow community member to follow this guide by vedder in setting up FOC
[/quote]

The BLDC Tool is outdated, [download the latest VESC-Tool here](http://www.vesc-project.com/vesc_tool)
The VESC-Tool has wizards and it's easy to set up.

[You can find infos and tutorials here](http://www.vesc-project.com/node/178) 

You can find all explanations for the settings in the link above, some possible start settings for your case could be:

Motor Current Max **60A** (you could rise it up to 80A)
Motor Current Max Brake **40A**
Battery Current Max **60A** (don't go higher)
Battery Current Max Regen: **20A** (if your Lipos are 5c charge rate then it's 25A, 20A is safe)

Battery Cutoff Start: 35V
Battery Cutoff End: 32V

These are the main settings you have to change in VESC-Tool (it's in the motor wizard), then start app wizard

But power and connect your vesc first, start VESC-Tool, update the firmware and then run the wizards.

[quote="ArsenalMain, post:1, topic:45949"]
80a continuous discharge BMS
[/quote]

I like that you go this route but please only connect it when you fully understand how this specific BMS works and how to connect it properly. 

Good Luck!
```

---
## \#3 Posted by: kyletrainy Posted at: 2018-02-09T15:54:19.955Z Reads: 253

```
Also to save you from some trouble, a lot of people have broken their diy vescs by running it in foc. To be safe, sensored bldc mode should be more reliable.
```

---
## \#4 Posted by: ArsenalMain Posted at: 2018-02-09T18:19:33.412Z Reads: 244

```
Ya, from what ive heard from various people so far, youre right, the FOC, unless you know what youre doing, might not be worth the risk.
```

---
## \#5 Posted by: ArsenalMain Posted at: 2018-02-09T18:44:28.959Z Reads: 228

```
In your opinion, is trying to get a FOC system set up not worth the risk? Have you personally used FOC on any of your boards? And lastly, I have to use the BMS because I did not opt for a balance charger but instead when for a bulk, 4a charger. Also, the BMS is the only part of my board that I have the e-switch connected to. 

Thanks for your help, your reply was very informative.
```

---
## \#6 Posted by: ZackoryCramer Posted at: 2018-02-09T18:50:25.011Z Reads: 223

```
[quote="ArsenalMain, post:5, topic:45949"]
is trying to get a FOC system set up not worth the risk?
[/quote]
Yea, blew my diyesk8 vesc the second I press detect. I am not gonna try foc unless I am using an foc box 📦😅
```

---
## \#7 Posted by: Juiced Posted at: 2018-02-09T20:24:51.218Z Reads: 211

```
I have a diy vesc in foc sensored and it's completely fine. I'm following namasakis build but with a single 6374.
```

---
## \#8 Posted by: ArsenalMain Posted at: 2018-02-09T20:29:20.851Z Reads: 204

```
How many miles have you put on it so far? And I'm also following his build. Are you  using 5 2s 5Ah batteries?
```

---
## \#9 Posted by: Juiced Posted at: 2018-02-09T20:31:47.009Z Reads: 195

```
Couple hundred miles, I recently went sensored but with no sensor it was still good. And yeah, the only difference is that I made a series adapter for the batteries.
```

---
## \#10 Posted by: Juiced Posted at: 2018-02-09T20:33:04.003Z Reads: 185

```
Honestly if you follow the steps you'll be fine. I don't see why people hate diy's vesc, haven't had a problem with it.
```

---
## \#11 Posted by: ArsenalMain Posted at: 2018-02-09T21:01:12.367Z Reads: 178

```
Considering it sounds like we will have a extremely similar setup, any  chance you could screenshot the values that you use for the FOC mode? Also, i considered doing the series adapter but in the end, i think im just going to solder the wires together instead of using an adapter. If you dont mind me asking, what are the specs of your build?
```

---
## \#12 Posted by: Juiced Posted at: 2018-02-09T22:02:19.761Z Reads: 164

```
90mm clones, 10s1p lipo 60c, hobbyking mount, 80 a bms, 190kv 6374 tb motor
```

---
## \#13 Posted by: Juiced Posted at: 2018-02-09T22:04:30.407Z Reads: 165

```
Yeah I would solder them together, it's just at the time I didn't have a bms so I never changed it. Im not home right now but If you scroll to namasakis settings it's exactly the same.  -20a for batt min will be fine for our batteries
```

---
## \#14 Posted by: louwii Posted at: 2018-02-10T03:25:26.681Z Reads: 162

```
Interesting, I have the same setup 10S Lipo, DIY VESC and a single 6374. It's been running fine during the few tests I did. Running BLDC mode, sensored.
I was hesitant to try FOC as I feel like it's kind of the lottery, either it works fine or it just fries.
What's your weight ? And what's your average speed/top speed ?
```

---
## \#15 Posted by: ArsenalMain Posted at: 2018-02-10T03:29:53.454Z Reads: 161

```
Ya, my setup will be 10s1p lipo, diy vesc, and a single sensored 6374 motor. From what I have been reading, if you use the new vesc-tool with the upgraded FW then moving to Foc is alot safer and less likely to kill the vesc. I would love some input from an actually experienced builder about the new tool though
```

---
## \#16 Posted by: ArsenalMain Posted at: 2018-02-10T03:47:41.360Z Reads: 155

```
Did you use the the old bdlc tool or the newer vesc tool to set up the foc
```

---
## \#17 Posted by: Juiced Posted at: 2018-02-10T04:00:26.448Z Reads: 153

```
around 190 pounds.  With foc its a little slower but my highest is 26 and i think i still have room for more, with an average of about 18-20mph.
```

---
## \#18 Posted by: Juiced Posted at: 2018-02-10T04:00:51.471Z Reads: 152

```
old, I found it easier at the time.  I went foc because I was curious and everything worked out fine.
```

---
## \#19 Posted by: ArsenalMain Posted at: 2018-02-10T04:03:56.008Z Reads: 146

```
In your opinion, how much speed do you lose with the foc instead of bldc?
```

---
## \#20 Posted by: Juiced Posted at: 2018-02-10T04:07:46.396Z Reads: 144

```
you'll notice a difference, but I doubt you'll be going that fast all the time.  If you want to sacrifice speed for a quiet start up, go for it.
```

---
## \#21 Posted by: ArsenalMain Posted at: 2018-02-10T04:15:03.917Z Reads: 133

```
If you've run bdlc before with your setup, what was your top speed? Just curious
```

---
## \#22 Posted by: Juiced Posted at: 2018-02-10T04:16:23.214Z Reads: 137

```
probably 30, but trust me it wont matter because youll never be that fast cruising.
```

---
## \#23 Posted by: louwii Posted at: 2018-02-10T06:15:24.084Z Reads: 135

```
The new tool is super easy to use.
I tried to write down a guide on my site, it might probably help you. I still need to write the guide to setup the motor.
https://esk8bible.com/programming-your-vesc

You can check on Youtube too, there are some guides with the VESC Tool.
```

---
## \#24 Posted by: ArsenalMain Posted at: 2018-02-10T21:08:11.540Z Reads: 126

```
I thought I recognized your username. I was just going through this thread again: 
http://www.electric-skateboard.builders/t/vesc-project-com-is-online-public-vesc-tool-download/32268/31?u=arsenalmain
and recognized that you had posted on my question. In that thread, many of the posters stood by that the new vesc tool makes using FOC alot easier and supposedly, safer. Ignoring my HW, do you think the new FW makes it easier to set up FOC?

@louwii Considering you also support the new Vesc-tool, what do you think of the question I just asked @rich
```

---
## \#25 Posted by: rich Posted at: 2018-02-10T21:39:02.442Z Reads: 119

```
[quote="ArsenalMain, post:24, topic:45949"]
Ignoring my HW, do you think the new FW makes it easier to set up FOC?
[/quote]


I never did it with "old" FW but setting up FOC is as simple as BLDC (just the motor detection is different). You can click on the interrogation marks in VESC-Tool to get further information about the respective step so everything works fawlessly. The new FW is safer for FOC but for example my maytech HW didn't like it (no breaks only drop outs and multiple faults). The reason why I switched to FOC was because my sensored motors were cogging at startup in BLDC mode.

The safe way would be to test first if you get any problems in hybrid BLDC mode before trying FOC.
```

---
## \#26 Posted by: ArsenalMain Posted at: 2018-02-10T21:43:30.410Z Reads: 115

```
Ya I think I will do that, hybrid and then FOC if hybrid worked out. Quick question, what erpm did you have the sensors cut out at? Supposedly the default is supposed to be 2000 but ive checked the tool and it was defaulted to 1100.
```

---
## \#27 Posted by: rich Posted at: 2018-02-10T21:57:21.252Z Reads: 113

```
I never changed that setting, left it at the default 2000
```

---
