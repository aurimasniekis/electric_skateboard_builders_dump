# Space Cell PRO 3 Screen help

### Replies: 38 Views: 2266

## \#1 Posted by: roonydagoony Posted at: 2016-07-08T14:15:02.185Z Reads: 164

```
Hi,
I setup my The Space CELL 10sp3 with DIY's ESC and DIY's 6374 230KV 3200W motor
Initially, it had a voltage reading on it before riding. (40.8 V i think)
However after riding my 1st mile, I noticed the screen changed to "L 3" and once I think I even saw "L 4"

Any idea what those things mean? I was not able to find a manual for the space cell.

Also, my board went up to 25-28 mph at first, but after 3 miles it doesn't go more than 4-6 mph.

Any idea what could be wrong?
```

---
## \#2 Posted by: Jinra Posted at: 2016-07-08T15:22:27.910Z Reads: 152

```
It looks like it's on the screen to choose what battery type the meter is reading. You should talk to enertion support on how to change it.
```

---
## \#3 Posted by: quanze Posted at: 2016-07-08T15:30:34.600Z Reads: 147

```
I remember someone else having the same problem. Apparently there are buttons on the back of the screen which you would have to get to.
```

---
## \#4 Posted by: roonydagoony Posted at: 2016-07-08T16:07:13.160Z Reads: 143

```
ah, that makes sense. But also seems a bit silly to have controls inside the enclosure
```

---
## \#5 Posted by: rpn314 Posted at: 2016-07-08T22:17:36.276Z Reads: 127

```
As I understand it that should have been set by Enertion before putting the space cell together, and shouldn't have to be set again. So my best guess is that something hit that button on the inside and somehow reset it. I think it's a similar LCD to [this one](http://www.ebay.com/itm/262492361627), and you can see the button the back used to change the configuration (how many and what kind of cells, so it gives the correct percentages) in one of the pictures.
```

---
## \#6 Posted by: lox897 Posted at: 2016-07-09T07:16:08.557Z Reads: 123

```
@EnertionSupport @onloop It seems like your battery manufacture forgets to de-solder the buttons before they put it in the space cell. A few people are having this problem.
```

---
## \#7 Posted by: roonydagoony Posted at: 2016-07-10T22:27:00.081Z Reads: 108

```
UPDATE: The screen automatically fixed itself and I'm able to see the voltage.

Another weird observation: Now when I turn it off, it takes 4-6 seconds to shut off the screen. And in the process you see the voltage dropping from where you were to 3 or 4 v, after which it finally shuts off.
Does this seem normal?
```

---
## \#8 Posted by: quanze Posted at: 2016-07-10T23:35:32.253Z Reads: 100

```
Probably a capacitor discharging in the battery pack I guess?
```

---
## \#9 Posted by: c4Lvin Posted at: 2016-07-11T02:55:28.066Z Reads: 96

```
When you switch it on, what do you see now? I have a Space Cell Pro 3 and it shows L10 (perhaps for 10S) and then stays on the % of the pack.
```

---
## \#10 Posted by: Mrmoonlight Posted at: 2016-07-11T05:00:37.827Z Reads: 97

```
There's a button on the back of the screen and the BMS is on top of it. On mine if you pushed the screen or area around the screen, it would press the button. I slapped some velcro on the bottom of the BMS and moved it right in front of the screen. That solved the problem.
```

---
## \#11 Posted by: roonydagoony Posted at: 2016-07-11T05:48:14.023Z Reads: 91

```
Yeah if I press above the screen area, it goes from L 3 to L16 and then till P48 or something followed by L 3 again.
Weird thing is, I saw the 100% sign after riding 7 or 8 miles....Super weird that it's at 100% and super weird that it's finally showing up. 
And when riding it goes through all the numbers...I'm worried I'll damage the cells or bms entirely.

On top of cutting down power to 5mph after going a few miles, this is another issue I have to deal with...smh
```

---
## \#12 Posted by: roonydagoony Posted at: 2016-07-11T05:49:21.800Z Reads: 89

```
I see L 3 when I turn it on.
```

---
## \#13 Posted by: roonydagoony Posted at: 2016-07-11T05:49:40.629Z Reads: 88

```
Is that bad for the battery?
```

---
## \#14 Posted by: lox897 Posted at: 2016-07-11T05:53:18.563Z Reads: 85

```
I'd get that button fixed ASAP if I were you. It may be showing you the wrong percentage if it thinks your battery is a different voltage. @onloop
```

---
## \#15 Posted by: Mrmoonlight Posted at: 2016-07-11T06:08:07.861Z Reads: 86

```
Not sure what problems this could cause, but either way, it's probably best to move your BMS to start. Then you can see if your power cutting issue persists.
```

---
## \#16 Posted by: c4Lvin Posted at: 2016-07-11T06:11:41.225Z Reads: 85

```
If it's L3 it would be 3S that's why I think he said it's at 100% for all those miles he rode. I read somewhere that the L"x" was for the series programming on the bms on eBay.
```

---
## \#17 Posted by: Jinra Posted at: 2016-07-11T06:16:38.221Z Reads: 84

```
This is another popular battery meter. It's not exactly the same, but I imagine the programmings codes are similar. You should scroll to Li10/L10/LiA and try to confirm it.

https://drive.google.com/file/d/0B8UWKkPeL6BbVXlIUUJrRkV5aGs/view?pageId=101385600508154334539
```

---
## \#18 Posted by: c4Lvin Posted at: 2016-07-11T06:25:09.425Z Reads: 84

```
Look at eBay 172018886570 and follow those steps. And see if you get a proper reading after that. Good luck.
```

---
## \#19 Posted by: roonydagoony Posted at: 2016-07-11T06:30:08.537Z Reads: 86

```
Ok, might need to shop for a few things.
I'll definitely try those steps and see if it fixes it
```

---
## \#20 Posted by: Aleendis Posted at: 2016-07-11T09:32:55.081Z Reads: 83

```
Had some similar problems. After the battery arrived it only shows the voltage and not the percentage value. Wrote to Jason in a thread here. He asks me to explain the behavior to the support. I decided that Iam good to go with the volts-values. But a few days ago I switched the pack on one more time (want to see if there is any voltage drop over the time) and the pack fixed itself. 

Oh Iam talking about the space cell for raptors. After I have received my board I'll have an eye on the readings.
```

---
## \#21 Posted by: philipp Posted at: 2016-07-11T12:01:19.500Z Reads: 79

```
When you turn your battery on and "L3" shows and stays => The button on the back of the display is being pressed by the bms wich is glued on top of the display. This starts the display in configuration mode everytime you turn on your battery.

Is your battery mounted to your board already? (the battery could be under some stress, wich causes the button to stay pressed)

You could lift off the bms from the battery, then turn the battery on while having the button on the backside of the lcd pressed (white small smd button), then press the button a few times till "L10" shows on the display, then turn battery off and on again without pressing the button.
After this, you could desolder the button to prevent it from being pressed again.
```

---
## \#22 Posted by: roonydagoony Posted at: 2016-07-11T14:16:12.270Z Reads: 77

```
Ah, ok. I'll check it out. A bit annoyed with @onloop that he'd sell such a buggy expensive piece : /
But I'm sure he's doing his best
```

---
## \#23 Posted by: roonydagoony Posted at: 2016-07-11T23:31:19.400Z Reads: 72

```
@onloop Will I void warranty if I try to fix the BMS myself?
```

---
## \#24 Posted by: Haick Posted at: 2016-07-12T06:36:24.781Z Reads: 74

```
I had the same problem and found that if i firmly press hard right above the top left side of the meter reading it will press the button. Clearly something is pressing on it and needs to be fixed. @onloop , this is something worth looking into
```

---
## \#25 Posted by: onloop Posted at: 2016-07-12T07:26:04.821Z Reads: 74

```
try not to attach the case too firmly to the deck, it is meant to be "hanging" from it.

However, i will look at relocating the parts to ensure the minute deck flex doesn't put pressure onto these parts.

thanks for the feedback
```

---
## \#26 Posted by: Haick Posted at: 2016-07-12T07:34:46.917Z Reads: 75

```
Quick question, My board keeps starting up on l3 mode. Ive loosened the case substantially and press the button to cycle up  to L 10 but each time when i turn the board on it turns back on to L3. Do you know why this is? I've ridden the board for about 6 miles so far and havent noticed any difference in speed or power when it says its on the L 3 mode
```

---
## \#27 Posted by: philipp Posted at: 2016-07-12T07:53:09.599Z Reads: 76

```
[quote="Haick, post:26, topic:5776"]
...but each time when i turn the board on it turns back on to L3.
[/quote]
Sounds like the button is still pressed on start-up of the board.
If it's not pressed on startup, it should show L10 for a second, then switch to the percentage display.
I'd still recommend to desolder the button on the back of the LCD, but first I'd ask for onloops permission.


[quote="Haick, post:26, topic:5776"]
I've ridden the board for about 6 miles so far and havent noticed any difference in speed or power when it says its on the L 3 mode
[/quote]
The voltage meter only acts as a charge indicator, it doesn't do anything else other than showing how full your battery is. Even if it's broken, your battery would work fine.
```

---
## \#28 Posted by: Haick Posted at: 2016-07-12T07:56:10.352Z Reads: 71

```
Thanks for the advice @phillipp . I'll look into it when I get a chance
```

---
## \#29 Posted by: Mrmoonlight Posted at: 2016-07-12T11:51:38.654Z Reads: 70

```
Mine was held on by just a piece of tape and a little by the foam padding on top. So it was pretty simple to move it. It only needs to be moved about a cm to be away from the button.

For mine, it pressed the button when I placed the board on the deck, before I screwed it on. Probably had a wire or something that happened to be right over the button. Once I figured it out, it literally took 10 seconds to fix the issue.
```

---
## \#30 Posted by: roonydagoony Posted at: 2016-07-12T15:15:12.604Z Reads: 68

```
I think I successfully fixed mine. I lifted the bms module and clicked on the white button until L 9.
Then pressed it and held it and turned it off while the button was held (it turned to L 10 and then you turn it off)
I haven't mounted it back yet, I just need to make some adjustments there before I can do that.

HOWEVER, at some point the power adapter got fried or something. I no longer see a light on the adapter.
And when I tried to connect to the battery, it sparked at the power connector. @onloop Can I still use the battery or did I mess something up there? When I try to turn the battery on, I see 0%(I definitely used up all the juice) with no backlight (after seeing L 10 for a second). Do I need a new power adapter?
```

---
## \#31 Posted by: Haick Posted at: 2016-07-12T16:14:20.973Z Reads: 70

```
@Mrmoonlight Just noticed mine had the same problem. Thanks for the advice

@roonydagoony My charger also occasionally sparks when connecting to the port. I have found that if you turn the battery off and wait a few seconds before you connect the plug, it tends to avoid that issue.
```

---
## \#32 Posted by: roonydagoony Posted at: 2016-07-12T17:33:35.167Z Reads: 68

```
@Mrmoonlight 
If you connect your charger only to the wall, not the battery....does the adapter LED turn on?
If so, mine's screwed.
If not, does it light up when you connect it to the battery?
If so, does it charge?
If not, does it charge?

Thanks
```

---
## \#33 Posted by: c4Lvin Posted at: 2016-07-12T17:41:49.871Z Reads: 69

```
I just noticed that the PRO 3 is different than the original Space Cell (30A). I think the original's LCD was always on while charging. And now the PRO 3 when the power button is switched off, it won't show it and only can tell if it's fully charged from the LED of adapter.
```

---
## \#34 Posted by: Mrmoonlight Posted at: 2016-07-12T19:41:06.271Z Reads: 66

```
Plug the power supply in and the light is green. Plug it into the battery and it turns red.
```

---
## \#35 Posted by: roonydagoony Posted at: 2016-07-12T20:19:33.523Z Reads: 64

```
Damn, so I definitely busted the adapter :disappointed:
```

---
## \#36 Posted by: Kaly Posted at: 2016-07-12T21:09:06.737Z Reads: 67

```
@EnertionSupport can you give a hand here ?
the silence is unbearable :no_mouth:
```

---
## \#37 Posted by: roonydagoony Posted at: 2016-07-14T02:48:09.006Z Reads: 60

```
Thanks for all the help guys.
@EnertionSupport reached out to me. I'm gonna send it down to Damon

Hopefully it works out!
```

---
## \#38 Posted by: j.archibald01 Posted at: 2016-08-24T01:10:29.537Z Reads: 48

```
Hi Guys. I had the same problem as most of you so I decided to make a video of how to fix this problem. Have fun riding with an awesome battery :) [Space Cell Pro screen Fix](https://www.youtube.com/watch?v=bhkjJXx33Ik)
```

---
