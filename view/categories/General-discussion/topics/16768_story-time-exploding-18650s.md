# Story Time. Exploding 18650s

### Replies: 24 Views: 1934

## \#1 Posted by: hj01 Posted at: 2017-01-27T17:41:04.675Z Reads: 289

```
story time guys, this one is going to be good.

So i have been gathering parts for the board for quite a while now, about two months. ebay delivery times are frustrating. 

My Friday activity was esk8 stuff. First thing was to finally make a fiberglass encloser for the board. It's drying as i write this post and it came up great:

<img src="/uploads/db1493/original/3X/6/a/6a70c12ee3b1db41c4dfdb76695c4cdefbda8725.JPG" width="666" height="500">4

Next thing was to have a little fun with my setup:

12S1P 18650s battery --> anti spark switch --> amp,volt meter --> VESC --> motor

The setup wasn't connected to the board itself because of the fiberglass so i just put all the components on a small skateboard i have.

Started to play with the motor: gas, brake, gas brake. At a certain moment the motor stopped completely, one of the FETs on the VESC started smoking and the red led on the VESC turned on.
I quickly turned the anti spark switch off and than figured the vesc got stuck for some reason and that if i turn it on again it'll be OK. sort of like restarting it. **WHAT A MISTAKE**.

Turned it On. FET started smoking again and with no warning one of the batteries in my setup burst and started releasing gas. Moments past and another battery burst into flame.

Side note: The batteries i had were two 6S1P connected in series, both of them were made by me from 18650 LG HG2 cells. Those M***********s burn like a nuclear reactor. A complete surprise to me. Did not think they can burn like this.

I ran to take my lipo guard bags and thru the battery that kept burning into one of them. I figured that it's going to continue burn till all the six cells are dead. I was not wrong cause the moment i thru the battery into the bag another flame burst from it. Till then i managed to run to my balcony and put the bag on the window. It kept burning and it seemed as if it's only starting to get stronger. I knew i cannot throw it to water but i do not have a suitable fire extinguisher.

I looked down to the street and saw no one was down there so i thru the bag to the street since the chance of it burning the asphalt was lower than the chance of it burning my furniture. Then i ran downstairs to check weather it was OK and it was. The fire was out. Then i remembered there was the second battery, at this moment I already realized those batteries can burst out of nowhere when their hot - and they still were. ran upstairs and everything was alright. The scene ended. 

**WHAT AN ADRENALINE RUSH.**

FACTS:

1. I checked all the FETs on the VESC and all but two are down, means their drain-source resistance is zero.
2. The FETs on the anti spark switch are down as well. made it just this week :(
3. I clearly remember that first thing that happened was the motor stopping and the FET smoking.
4. I did not have a fuse on the spark switch. 
5. The motor seems OK, all the leads are shorted and nothing is shorted to it's housing. But i have no means to check weather it's working.
6. That's the second VESC that i break :(. This hobby is starting to be pricey.

My personal conclusions:
1. A big mistake not to put a fuse on the switch. It would have prevented the fire.
2. Those lipo guard bag are life savers they did the job and did not melt.
3. I need a suitable fire extinguisher.
4. I'm going to pad the inside of my encloser with the material the lipo guard bag is made of.
5. I cannot be 100% sure but by the sequence of events it seems that the VESC got wrong first. I'm really starting to be frustrated from the product.

Some obliviously requested photos:

<img src="/uploads/db1493/original/3X/a/9/a9d99064bbfbb38bab3f55f00ab74305300472c9.JPG" width="640" height="480">

<img src="/uploads/db1493/original/3X/7/2/722738e7d2b5e6ada506fe5722a07291ed810725.JPG" width="640" height="480">

<img src="/uploads/db1493/original/3X/7/8/78b1f87c961fd6b310d062433c2df78e6c4bf867.JPG" width="500" height="500">

 Hope you can learn from my mistakes.
Cheers guys.
```

---
## \#2 Posted by: Okami Posted at: 2017-01-27T17:56:24.808Z Reads: 271

```
This was one.. crazy and.. at the same time entertaining story.. :D 

Did not want to be the first one to comment.. but yeah.. just my first reaction when reading through all of this.. not entirely sure what caused your batteries  to self ignite... but that's some serious stuff you went through.. hope you get ''back on feet'' soon with your board.. and that this little incident wont set you back :slight_smile:

Good thing you had these lipo safety bags.. turns out they are useful :)
```

---
## \#3 Posted by: barajabali Posted at: 2017-01-27T17:56:50.369Z Reads: 265

```
holy fuck thats scary. 

Do you think the batteries exploded due to the burned fet? or just faulty battery construction ? This is real life and its good you posted so everyone understands the dangers of making your own board.
```

---
## \#4 Posted by: hj01 Posted at: 2017-01-27T18:04:44.832Z Reads: 265

```
I'm pretty sure it's because of the FETs. If those are ruined it's basically shorting the battery with the coils of the motor. 
If it was the other way around (battery going wrong first) i can't see how the FETs would be affected.
That's my theory. can't know for sure.
```

---
## \#5 Posted by: Blasto Posted at: 2017-01-27T18:20:49.838Z Reads: 249

```
not trying to rub this in your face @hj01 

But this practice should not be done, use a fuse, do not by-pass them

<img src="/uploads/db1493/original/3X/1/9/19d681ee13ad407ed23482e05239e77a351a64c1.jpg" width="644" height="500">
```

---
## \#6 Posted by: hj01 Posted at: 2017-01-27T18:22:39.015Z Reads: 243

```
completely agree.
```

---
## \#7 Posted by: Blasto Posted at: 2017-01-27T18:24:45.684Z Reads: 237

```
hard to tell by the pictures, but your vesc looks fine. can you probe the input to see if you have a low impedance (resistance)
```

---
## \#8 Posted by: Hummie Posted at: 2017-01-27T18:28:36.404Z Reads: 233

```
Maybe the motor could have been shorted first. 
I've heard of it taking out other components when it's shorted. 
According to lg's testing on their site those cells aren't supposed to go up in flames with a short.  I suspect there's a lot of stating things are safer in manufacturer tests. I shorted lg hg2s once and got lucky and it just puffed up the steel can.  I've seen them shoot like bullets and makes me think Lipo are safer
```

---
## \#9 Posted by: hj01 Posted at: 2017-01-27T18:29:13.438Z Reads: 227

```
That's what i did with all the six FETs separately. Four are ruined and two are OK.
That's why i believe it's the VESC that got wrong first.
```

---
## \#10 Posted by: hj01 Posted at: 2017-01-27T18:32:01.441Z Reads: 225

```
I think that the 18650s lit on fire because they were close together in the battery. The First one did only puff up and release gas but it probably got worm and ignite one of the other ones.
```

---
## \#11 Posted by: PXSS Posted at: 2017-01-27T18:44:17.107Z Reads: 216

```
FETS usually fail closed. I don't know what you expected when you saw it smoke and still decided to turn it back on without troubleshooting first...

Not trying to be an ass but that was really stupid...
You cannot blame it on the VESC. 

The failed FETs created a short, that probably made your switch also fail since you bypassed the fuse and therefore you shorted your cells. Once the first cell failed, it acted as a short for the rest of the cells and there was nothing you could do then. 

Throwing burning batteries off a balcony? Seriously??? Even if there was nobody in the immediate area, the cells can explode violently and throw shrapnel tens of feet away with the pressure they build up inside, add to that a drop of at least 20 feet and you sure as hell just created a way more dangerous situation. 

All you needed were Lipo bags and a bin to contain the fire.

A regular fire extinguisher will not be suitable for lipo fires either. You need at the very least a Halon extinguisher. 

I'm glad you and nobody else got hurt but please think about what you did wrong and what you should have done instead of blaming the ESC
```

---
## \#12 Posted by: Blasto Posted at: 2017-01-27T19:07:38.841Z Reads: 197

```
[quote="PXSS, post:11, topic:16768"]
FETS usually fail open
[/quote]

95% of the time they fail closed (short)
```

---
## \#13 Posted by: longhairedboy Posted at: 2017-01-27T19:11:45.142Z Reads: 191

```
That's been my experience with failed e-switches for sure.
```

---
## \#14 Posted by: hj01 Posted at: 2017-01-27T19:47:46.970Z Reads: 186

```
@PXSS can't really understand whether you read the entire post.

But i reckon that even if the FETs failed first on the anti spark switch they would not short the batteries since it will only power up the VESC. I don't know whether you are familiar with the anti spark switch vedder design. 

In addition, i do not blame the VESC for the entire chain of events, i realize the what i have done wrong, and it is written in the post. 

Nonetheless, it seems that the first element that failed is the FETs on the VESC. The other option is the motor but i can't check that right now.
```

---
## \#15 Posted by: treenutter Posted at: 2017-01-27T20:08:47.413Z Reads: 188

```
Thanks for sharing this @hj01 it's a good reminder for everyone!

Here are some take-away messages in summary: 

* If you ever see smoke, even a little, turn everything off, disconnect, and inspect.

* Have a bin, lipo bags, and a fire extinguisher nearby

* Use a fuse on your anti-spark switch, if you don't have an anti-spark switch, add a fuse in the line somewhere else
```

---
## \#16 Posted by: cmatson Posted at: 2017-01-28T04:53:53.629Z Reads: 172

```

here is a video of a single 18650 cell exploding in a "controlled envirenmnt" 

this video is actually from a while ago with an old flashlight battery; just now uploaded it to youtube for this thread's purpose though:

https://www.youtube.com/watch?v=Gn0GgZuFNEc&feature=youtu.be
```

---
## \#17 Posted by: Jebe Posted at: 2017-01-28T05:06:50.653Z Reads: 167

```
Thanks for sharing. Solid reminder that these aren't toys
```

---
## \#18 Posted by: Okami Posted at: 2017-01-28T08:12:51.318Z Reads: 160

```
I like the comparison with fuel and gas.. batteries are not that much different in that they also hold dangerous energy into them.. which, if, is released in short amount of time.. might be bad :)
```

---
## \#19 Posted by: lox897 Posted at: 2017-01-28T09:32:52.502Z Reads: 151

```
Happened to me recently. My anti spark started smoking (I believe it was the Zener diode) and I turned it off. Took out the anti spark switch and plugged back in, works fine. I wish there was an easy to solder through hole switch. I guess I just have to get better at SMD. For now I'll just use xt90s
```

---
## \#20 Posted by: PXSS Posted at: 2017-01-28T20:00:52.224Z Reads: 136

```
Yes! That's what I meant as seen in the third paragraph but obviously wrote the opposite lol.
```

---
## \#21 Posted by: PXSS Posted at: 2017-01-28T20:27:28.924Z Reads: 130

```
I did read your entire post. I made a typo in my first sentence but go back and read the third paragraph. If your VESC had failed and caused a short, then massive amounts of current would also make your switch fail. Your VESC definitely failed first. A failed switch cannot short a VESC but a shorted VESC will short your switch without a fuse. BTW, you don't need a 40A fuse, even a 100A fuse would have saved your build. 

Things to add to your list:
#Do your research,
you should have known how bad a bursted battery fire is, it should not have been a surprise, there are plenty of youtube videos out there. Same thing with failing FETs, it is common knowledge in the electrical engineering world that FETs fail as a short most of the time, a simple google search would have had you better prepared. 

#If you see smoke, do not power things up,
That is really where you F'd up. You should have had the patience to check things out thoroughly before ever making that choice. Whether it was a FET or anything else on the board, you should have made an inspection. 

#Do NOT throw batteies off a balcony!!!!
Putting others at risk is seriously not cool. Plus you could have made the fire much much worse! This is more of a having common sense thing but again, knowing how batteries fail would have helped in not making that mistake. 

#Check, double check and triple check your VESC settings, 
Given that this is the second time you've had a failed VESC, the odds of them both having manufacturing defects are low unless you purchased them from a non reputable source (in which case the common sense and research arguments apply), I would post all your settings for others to look through, maybe they can spot what was wrong.
```

---
## \#22 Posted by: PXSS Posted at: 2017-01-28T20:29:52.394Z Reads: 123

```
Chassis mounted FETs with through hole legs do exist
```

---
## \#23 Posted by: deucesdown Posted at: 2018-02-18T15:59:23.068Z Reads: 73

```
Wait a minute the fets on vesc short battery to motor on fail? It makes sense, feeling pretty dumb. Fuse going in asaply...
```

---
## \#24 Posted by: PXSS Posted at: 2018-02-18T16:51:53.497Z Reads: 63

```
FETs commonly fail closed so yes. :)
```

---
