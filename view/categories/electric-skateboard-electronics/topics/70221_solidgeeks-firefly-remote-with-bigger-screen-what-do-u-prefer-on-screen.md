# Solidgeeks FireFly Remote with bigger screen. What do u prefer on screen?

### Replies: 20 Views: 768

## \#1 Posted by: StefanMe Posted at: 2018-10-05T10:18:03.503Z Reads: 231

```
Super crazy how difficult it is to developed a new GUI. Never thought it is so hard to find a nice looking solution. I need a bigger screeen do fit everything inside 😂

I decided to fit in a screen that has double height and write a new GUI. Works fine for now. Added some addisionl features like vibration alarm and headlight support(not yet finished) and a button to change the main screen for additional views.

After a while I found out, that I really needed something like an tuning screen... a screen where u can just se my power and different amperages from the battery and motor. So I created this view.

On the bottom is the trigger indicator, above a big battery bar, on the right site the battery, wifi and headlight status.

I have some huge problems with my battery, so I decided to display also battery amps(top) and motor amps(bottom)

I think about an all data screen with just numbers on it with nearly everything technical data from the Vesc on it... temperatures, amps, voltages, everything.... like a debug site.

Now I want to ask u, what do you want for this? What do information do u prefer to look while riding? 

![image|375x500](upload://5jXYRpm4s358AfEPPpw4NxJrsOu.jpeg)
![IMG_5927|375x500](upload://zctdXkkUnigSdgQhkhgIkAwzhlL.jpeg)
```

---
## \#2 Posted by: Acido Posted at: 2018-10-05T10:47:17.012Z Reads: 214

```
Imo the less stuff on the screen the better
Battery voltage
Range traveled/remaining calculated by average wh usage
Vesc temp
Maybe also something else but i can not rember of anything
```

---
## \#3 Posted by: deucesdown Posted at: 2018-10-05T12:48:46.116Z Reads: 198

```
Per cell voltage with diebiems would be so cool
```

---
## \#4 Posted by: Yegmesh Posted at: 2018-10-05T14:25:26.826Z Reads: 185

```
Are you able to upload the STL file for the larger screen?
```

---
## \#5 Posted by: pjotr47 Posted at: 2018-10-05T14:34:37.580Z Reads: 175

```
Best firefly mod :hushed:
```

---
## \#6 Posted by: moon Posted at: 2018-10-05T14:39:42.512Z Reads: 168

```
Ill ask it here,

Is there a CAD file for this remote?

I want to make like CNC bamboo case, it will look awesome. Maybe a aluminium throttle.
```

---
## \#7 Posted by: StefanMe Posted at: 2018-10-05T16:12:42.645Z Reads: 155

```
GITHUB: https://github.com/StefanMeGit/nRF24-Esk8-Remote
THINGIVERSE: https://www.thingiverse.com/thing:3138533

@deucesdown
I don't have an diebiems.... maybe in the future :slight_smile:

@Yegmesh
I can do, but I made a special version with 963ZZ bearings... I also used a normal 6x6mm tactile switch instead the normal micro switch. Gives a much better feedback with the trigger.

![07|460x499](upload://tspQn1JEQPGq3wJb9Ybhyh5U6Ge.png)

@pjotr47
thanks!

@moon
please ask Solidgeek directly... I ll not give them away.
```

---
## \#8 Posted by: moon Posted at: 2018-10-05T16:30:51.486Z Reads: 132

```
Ok. I will ask him again :)
```

---
## \#9 Posted by: AreaKruzer Posted at: 2018-10-05T16:52:29.941Z Reads: 131

```
What screen size is it running on? I remember tried programming a 128x64 pixel screen on my Arduino nano and it is almost out of memory that it can hardly work with the VESC UART library that was developed by one of the members (I think he is SolidGecko) here. 

I was initially quite interested to port the codes over to use on a STM blackpill micro processor. But haven't have the time to do so
```

---
## \#10 Posted by: StefanMe Posted at: 2018-10-05T16:55:53.532Z Reads: 123

```
128x64 0,96inch
For me it working without any issues. The memory is a problem.... that’s true. I ll also try to port everything to a better chip. The feather m0 locks interesting. Build in Lipo handling and NRF transmitter. I have one at home. Maybe I ll give it a try in the future.

This Is only a bit modified version to make it more stable and handy for me.
```

---
## \#11 Posted by: brenternet Posted at: 2018-10-05T17:00:26.282Z Reads: 121

```
Bamboo case, I'm all over that bud. Hit me.
```

---
## \#12 Posted by: AreaKruzer Posted at: 2018-10-05T17:00:35.124Z Reads: 118

```
Yes. I just came across the feather m0. It looks to be a very good package size for what they have to offer. 

I am intending to add on a small rotary encoder so that one can use it to edit settings on the fly. Like changing the cruise control speed, the wheel size, and so on. 

But with the form factor being sleek, it is a little challenging to try and add any new stuff to it without compromising the sleek design of the firefly
```

---
## \#13 Posted by: moon Posted at: 2018-10-05T17:01:30.273Z Reads: 109

```
Yeah it will look beautiful - I just need to wait for files to make design changes
```

---
## \#14 Posted by: brenternet Posted at: 2018-10-05T17:02:18.096Z Reads: 106

```
Bamboo case with the single board and a larger screen is heaven.
```

---
## \#15 Posted by: AreaKruzer Posted at: 2018-10-05T17:02:46.009Z Reads: 104

```
U might need to add some counterweight at the bottom of the remote so that the throttle area will not be too heavy and feels alittle unbalanced in ur hands
```

---
## \#16 Posted by: moon Posted at: 2018-10-05T17:05:35.094Z Reads: 112

```
> "WE CHangeD ThE  RAptOr 2 haNDLe FOr BEtTer weigHt dISTRibUTION" - Jason, Enertion

Yeah your right. Good idea
```

---
## \#17 Posted by: AreaKruzer Posted at: 2018-10-05T17:07:25.056Z Reads: 108

```
Did Jason really said that?
```

---
## \#18 Posted by: moon Posted at: 2018-10-05T17:08:18.567Z Reads: 110

```
Yeah something along those lines
```

---
## \#19 Posted by: sanderfu Posted at: 2019-01-17T21:35:49.716Z Reads: 57

```
[quote="StefanMe, post:7, topic:70221"]
963ZZ
[/quote]

Did you mean 693ZZ bearings? Cant find any called 963ZZ :-)
```

---
## \#20 Posted by: StefanMe Posted at: 2019-01-17T22:02:13.260Z Reads: 53

```
Sorry... u are right! Its 693ZZ :slight_smile:
```

---
