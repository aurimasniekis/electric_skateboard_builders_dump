# Project Zephyr &#124; Rayne Reaper &#124; CarVon Dual Hub Motor &#124; Enertion SPACE &#124; Dual VESC &#124; Nyko Kama

### Replies: 52 Views: 6164

## \#1 Posted by: sgaana Posted at: 2015-12-14T05:36:10.924Z Reads: 296

```
I started putting things together this weekend and here are some pictures to show and request for advice. Decided to use Rayne Reaper as it has a very flat deck to mount SPACE cell. I still need to work on connection to Nyko Kama receiver. 
Pictures 3 and 4: Is my Canbus OK?
Pictures 5 and 6: My friend (who works with electronics) recommended soldering this way to power both VESC to Enertion Space cell, instead of soldering both power leads together onto one XT60 connector. Any comments?
<img src="/uploads/db1493/original/2X/6/6f4e68795129fffabbfb13bd7ac564aad0118bd9.JPG" width="375" height="500">
<img src="/uploads/db1493/original/2X/1/10f5703945c63b2d7dbc070ef9ad9db5d11005bc.JPG" width="375" height="500"><img src="/uploads/db1493/original/2X/8/8ecc994ce0a3f0bf31147fd32e938a50a4844fce.JPG" width="375" height="500"><img src="/uploads/db1493/original/2X/c/cfeba170a336a6d581be09e5f60ad901e6c1d3ec.JPG" width="640" height="480"><img src="/uploads/db1493/original/2X/9/93568c60e1bd375393f9ff3fceb067aa2871a298.JPG" width="640" height="480"><img src="/uploads/db1493/original/2X/7/7482879e11d0208089f26740bdbf3870d7150437.JPG" width="640" height="480">
Cheers,
```

---
## \#2 Posted by: broshi Posted at: 2015-12-14T08:44:45.992Z Reads: 265

```
Can't answer any of your questions but since I'm thinking about SPACE cell + carvons duals, I'm interested to see your speeds and range
```

---
## \#3 Posted by: longhairedboy Posted at: 2015-12-14T13:50:12.060Z Reads: 261

```
i second that interest. I'm very interested in Carvons right now. 

@sgaana How much flex is in that deck? The Space cell doesn't like to bend much. There are ways around that, but i look forward to seeing your solution. That deck is pretty low. 

Are you planning to fab your own box or repurpose something you found?
```

---
## \#4 Posted by: treenutter Posted at: 2015-12-14T14:07:08.544Z Reads: 252

```
[quote="sgaana, post:1, topic:721"]
instead of soldering both power leads together onto one XT60 connector. Any comments?
[/quote]


I think @lowGuido , @chaka , or @sl33py might have more input, but my first thought is that you're increasing the demand placed on that first set of capacitors. I don't know whether this is optimal or not. I haven't seen anyone else w the spacecell and dual ESC\VESC wire the power in this way. It seems more straightforward to just use a splitter with xt60 connectors. Either way, make sure to heat shrink all of this.
```

---
## \#5 Posted by: chaka Posted at: 2015-12-14T15:15:26.367Z Reads: 238

```
One set of caps will work fine but he is using both sets. I good idea since those samxon caps a have a really bad reputation.
```

---
## \#6 Posted by: kai Posted at: 2015-12-14T15:20:40.799Z Reads: 236

```
I agree with @treenutter about the capacitor thing but i am not a master like some of the other guys. The canbus looks good. What was your friends reasoning in connecting that way instead of the xt60 soldering like most people do? To me... i would avoid soldering things like capacitors that can be damaged from heat. But that is my opinion. Soldering the capacitor runs more risk IMO. I suck at soldering
```

---
## \#7 Posted by: kai Posted at: 2015-12-14T15:34:07.837Z Reads: 230

```
@chaka so if i solder the xt60 from both vesc together to plug into the space cell and also connect the capacitors together would that be the best way?
```

---
## \#8 Posted by: chaka Posted at: 2015-12-14T15:50:15.010Z Reads: 220

```
If you join the capacitor boards like it has been done here there is no need to join both XT-60's.
```

---
## \#9 Posted by: kai Posted at: 2015-12-14T15:51:36.219Z Reads: 214

```
Gotcha. Would it be a problem if i did connect it the way i said though?
```

---
## \#10 Posted by: chaka Posted at: 2015-12-14T16:18:58.419Z Reads: 212

```
No, it will be fine, just a bit redundant.
```

---
## \#11 Posted by: lowGuido Posted at: 2015-12-14T19:42:56.501Z Reads: 210

```
I quite like the way you have wired them together.  Nothing wrong with that at all.
```

---
## \#12 Posted by: sgaana Posted at: 2015-12-14T20:20:23.118Z Reads: 208

```
@broshi Will check the range once is running. But unlikely to try maximum speed as I will be using just for commuting. So if I reach 10km/hour, I will be pleased.
```

---
## \#13 Posted by: kai Posted at: 2015-12-14T20:45:40.059Z Reads: 204

```
Bro it will go way faster then that! Might as well walk at 10 km/h. I can kick 6 miles at a constant 21 km/h. 21 would be a good speed for commuting which your board will do all to easily. Can't wait to see your board finished bro.
```

---
## \#14 Posted by: longhairedboy Posted at: 2015-12-14T20:51:47.239Z Reads: 198

```
oh yeah that is some very clever wiring. I'm borrowing this idea for sure.
```

---
## \#15 Posted by: sgaana Posted at: 2015-12-14T20:58:07.533Z Reads: 199

```
@longhairedboy Very stiff, made of bamboo and fiberglass.
I am not sure of what type of enclosure o use. But first have to figure out how to mount.
```

---
## \#16 Posted by: sgaana Posted at: 2015-12-14T21:14:51.338Z Reads: 207

```
He said is "cleaner" without having make any changes to the wires and XT60 connectors. 
He also said this is reversible.
```

---
## \#17 Posted by: kai Posted at: 2015-12-14T21:47:33.639Z Reads: 209

```
Cool. Based on what chaka said... the way you hooked that up if one cap goes bad the other will still be good and enough for both vesc? Guess that is the best way.
```

---
## \#18 Posted by: lowGuido Posted at: 2015-12-14T21:58:27.245Z Reads: 208

```
Yeah, Also worth noting, Caps don't last forever and should replaced fairly regularly.
```

---
## \#19 Posted by: kai Posted at: 2015-12-14T22:07:57.519Z Reads: 207

```
How often would you say?
```

---
## \#20 Posted by: lowGuido Posted at: 2015-12-14T22:25:51.225Z Reads: 210

```
the correct answer is: It depends.

maybe you skate every day.. maybe only once a month.. 

I reckon I'd be doing mine yearly.
```

---
## \#21 Posted by: treenutter Posted at: 2015-12-14T23:37:51.841Z Reads: 190

```
@lowGuido that's good to know I wasn't aware of that!
```

---
## \#22 Posted by: broshi Posted at: 2015-12-15T04:54:40.036Z Reads: 179

```
You would definitely reach 10km/H
You are using a 10S space cell with good current. Should easily be able to reach 30km/h
```

---
## \#23 Posted by: longhairedboy Posted at: 2015-12-15T18:52:49.052Z Reads: 175

```
i wonder if that's all that's wrong with some of the old 8S flier dual ESCs i have on my bench. I loved those damned things but both of them have one bad side.
```

---
## \#24 Posted by: lowGuido Posted at: 2015-12-15T21:57:29.298Z Reads: 175

```
failed caps wont necessarily stop your ESC from functioning, but continuing to use it on bung caps can cause damage to the ESC.
```

---
## \#25 Posted by: trbt555 Posted at: 2015-12-16T06:43:25.882Z Reads: 179

```
Don't capacitors develop a short when they fail ? Given the fact that they are on the battery side of the esc, wouldn't failure of a cap be more than obvious ?
```

---
## \#26 Posted by: lowGuido Posted at: 2015-12-16T06:45:38.210Z Reads: 184

```
they can fail.. and then they can dry out without totally failing.
```

---
## \#27 Posted by: sgaana Posted at: 2015-12-20T20:54:10.094Z Reads: 197

```
Heat shrink both VESC today. But had to cut both wires in order to heat shrink them individually). Extended Nyko receiver wires and crimp them. Next step, get a 7pin connector and connect both VESC wires again. Then testing. 
<img src="/uploads/db1493/original/2X/b/be48c58487cc1fc8419d145f2728e69d0d6c2820.jpeg" width="666" height="500">
<img src="/uploads/db1493/original/2X/9/9eb3802d2ec0152be9e90f4738d60997ec3d51b8.jpeg" width="666" height="500">
```

---
## \#28 Posted by: elkick Posted at: 2015-12-20T21:49:22.280Z Reads: 187

```
Looks nice, but I'd suggest to insulate those PPM pins. They seem to be dangerously close to the capPCB.
```

---
## \#29 Posted by: NIK Posted at: 2015-12-22T20:32:02.196Z Reads: 188

```
@sgaana may I ask what is the type or size of that heat shrink that you use for the VESC?
```

---
## \#30 Posted by: sgaana Posted at: 2015-12-23T02:38:52.928Z Reads: 191

```
@NIK It's about 8cm width or just over 3 1/4 in. That's the only size big enough I found at my local store. But it shrank to half of its original size. 
BTW you build looks awesome!
 <img src="/uploads/db1493/original/2X/2/2399538f01de7f73b934920b75762873cb1c234a.jpeg" width="666" height="500">
```

---
## \#31 Posted by: NIK Posted at: 2015-12-23T08:16:35.127Z Reads: 183

```
Thanks @sgaana gonna but those :smiley:
```

---
## \#32 Posted by: laurnts Posted at: 2016-01-24T18:49:10.855Z Reads: 185

```
@sgaaana According to my personal opinion, that connection should work better (Your friend recommendation is good). The reason behind it is that you would have double capacity of the capacitor working simultaneously supplying to both ESC. It acts like you are using 6 capacitor instead of 3 for single ESC. In case of turning or starting, when one ESC requires sudden power draw, it will supply power from 6 caps instead of 3 to the ESC minimizing cogging effect.

Although in parallel connection from the XT60 / XT90 works as well as above scenario only in much slower rate (cable length effect) :D
```

---
## \#33 Posted by: sgaana Posted at: 2016-02-23T06:14:17.606Z Reads: 173

```
Hi dudes, right now, my board stutters when I try to start from stand still. I have tried bench test and sat on the deck. Have not tried to stand on it yet. Please go through the screen shots and see which parameters need to be changed. Cheers.
<img src="/uploads/db1493/original/2X/0/0dc3276f9cbde2bcbd5167ce8d167da251d24bcf.png" width="386" height="500"><img src="/uploads/db1493/original/2X/1/1997b9ce691ff9f0749256b10388dd111220aae5.png" width="386" height="500">
```

---
## \#34 Posted by: evoheyax Posted at: 2016-02-23T06:33:07.487Z Reads: 149

```
Have you ried a start up boost of 3 or 4. On the bench, a startup of 3 seemed much better then 1, and 4 was even better, though I can't test it under load.
```

---
## \#35 Posted by: sgaana Posted at: 2016-02-23T06:38:08.509Z Reads: 148

```
You mean increased from 0.150 to 3.0 or 4.0? Did @elkick say not to go beyond 0.150?
```

---
## \#36 Posted by: evoheyax Posted at: 2016-02-23T06:41:12.374Z Reads: 158

```
yes, sorry, I mean .04, I read your post wrong. I wish I could test my values to see. They mostly look similar to what I could come up with on the bench.

What happens at .04?
```

---
## \#37 Posted by: sgaana Posted at: 2016-02-23T06:57:11.336Z Reads: 165

```
Stutters as well, with load. . 0.150 was better. If I push, it won't stutter. 
I have to decrease nunchuck's sensitivity as well.
```

---
## \#38 Posted by: evoheyax Posted at: 2016-02-23T06:59:52.206Z Reads: 168

```
hmmm... I wish I could offer more advice. Its one of those things where the right values would be golden. But coming up with those values requires a real understanding of the motors and how to calculate these values.
```

---
## \#39 Posted by: elkick Posted at: 2016-02-23T07:28:56.126Z Reads: 169

```
There are some mistakes in your settings: the slave VESC setup ("multiple esc's over can") won't fit with "ID 0" and vice versa. 

If this is the master, you should disable "multiple esc's over can", this causes the stutter. And make sure to give the slave "ID 1" and enable the mentioned option there, master has "ID 0": 

Master: ID 0, "multiple esc's over can" disabled
Slave: ID 1, "multiple esc's over can" enabled
```

---
## \#40 Posted by: sgaana Posted at: 2016-02-23T08:03:51.153Z Reads: 168

```
Thanks @elkick. Will make these changes tomorrow. It's bedtime in Westcoast Canada now. Cheers
```

---
## \#41 Posted by: sgaana Posted at: 2016-02-24T07:13:44.274Z Reads: 164

```
Thanks @elkick, got it going more smoothly now. The other change I made was to positive and negative ramping constants. Right now, I set positive at 0.50 and negative at 0.40. I think positive 0.50 is good but still trying to figure out the negative ramping. 
<img src="/uploads/db1493/original/2X/8/82ef2795de887c7f653f5247b06f2613b1ea4e9d.png" width="690" height="414">
```

---
## \#42 Posted by: Adam0311 Posted at: 2016-03-03T04:41:13.177Z Reads: 144

```
Nice build! I'm itching to pull the trigger on dual Carvon's, but I'm not sure if the 10s space cell will be enough for some of the hills in my area. Have you done any 15% hills on yours?
```

---
## \#43 Posted by: sgaana Posted at: 2016-03-03T05:40:57.355Z Reads: 147

```
I am still figuring out the settings. From what I read, 15% should not be difficult. 
I'm trying to make a fiberglass enclosure. When it's done, I will be completing my settings. For sure will post them here.
```

---
## \#44 Posted by: sgaana Posted at: 2016-04-03T05:58:21.143Z Reads: 157

```
Here are some updates with pictures and screenshots and some questions to our community.
1) How to tame the Nyko Kama nunchuck?
2) How to start smoothly from stand still position?
3) How to limit maximum speed to 10km/hour?
4) Screenshot 4: What to do with Deadband, ERPM start and End ?
5) Enclosure is made for a science project presentation. Will find or build a more hardy one later. 
Thanks,

<img src="/uploads/db1493/original/2X/0/04358c41c9abd556066ca7b61fde4f54146846bc.png" width="690" height="413"><img src="/uploads/db1493/original/2X/9/90e8bf0520335f30a32f31c7fc106f19aeedccb7.png" width="690" height="414"><img src="/uploads/db1493/original/2X/1/1712a271a26dbd60bfa2bf32180c92153c784716.png" width="690" height="413"><img src="/uploads/db1493/original/2X/7/72de07dee4f04b8f46a600c61aa9e92a22a8cac9.png" width="690" height="426">
<img 
<img src="/uploads/db1493/original/2X/6/676d9776951f2e0e547d5c09620db9e1d181ed01.JPG" width="375" height="500"><img src="/uploads/db1493/original/2X/2/2a62de544e84eb06715982c60667978649d86902.JPG" width="640" height="480"><img
```

---
## \#45 Posted by: evoheyax Posted at: 2016-04-03T17:00:29.929Z Reads: 146

```
15% with space cell may be a problem. I am going to bypass the bms and pull 30 amps per motor, which should help with the hills. But the space cell I'm learning is not the best battery to pair with the carvons.

The smooth start will be tricky from stand still. I think it's only possible if the motors are sensored.
```

---
## \#46 Posted by: sgaana Posted at: 2016-04-03T20:53:29.459Z Reads: 140

```
How do I do this? Increase   Batt Max to 60.00A ?  thanks
```

---
## \#47 Posted by: evoheyax Posted at: 2016-04-03T21:53:02.440Z Reads: 142

```
battery max to 60 amps, each motor max to 30 amps, and rewire the battery to draw power before the bms instead of after. This is what I'm planning on doing. How it will end, is to be found.

But I got a fault code while hitting either a heat limit or amp limit, and chaka thinks it was an amp limit, and it for some reason broke my vesc.

So for the unknown reason, be careful what you doing in testing. I might end up making a lipo myself if modding the space cell doesn't do it. I would rather be able to hit 50 amps through each motor, since that is the vesc max.
```

---
## \#48 Posted by: sgaana Posted at: 2016-04-06T04:45:23.516Z Reads: 135

```
Thanks @evoheyax 
@onloop Jason, can you help with my questions?
I'm putting these numbers: Deadband 0.15, ERPM Limit Start: 2.000, ERPM Limit End: 1.000
How about batt max? Is it safe to go to 60amps?
@elkick David, any suggestions as you have built two boards with Enertion Space Cell and CarvOn ?
I'd appreciate contribution from anyone else. 
Thanks
```

---
## \#49 Posted by: elkick Posted at: 2016-04-06T12:16:35.252Z Reads: 134

```
I never had an issue with 2x30A for the Space Cell. But it's quite flat here. On the other hand the battery fuse will blow after 10 sec. on 60A anyway, so there's no big danger of damaging anything I guess.
```

---
## \#50 Posted by: evoheyax Posted at: 2016-05-03T20:23:55.348Z Reads: 116

```
@sgaana those settings  worked so much better than the ones I used before. Now, I just need to get FOC working.
```

---
## \#51 Posted by: sgaana Posted at: 2016-05-04T02:58:00.517Z Reads: 114

```
You meant these numbers: Deadband 0.15, ERPM Limit Start: 2.000, ERPM Limit End: 1.000 ?
```

---
## \#52 Posted by: evoheyax Posted at: 2016-05-04T03:00:00.537Z Reads: 116

```
no, the advanced motor config. I had many values (maybe 5 or 6) different, and with settings matching yours, I can start from stop, and much better acceleration.
```

---
