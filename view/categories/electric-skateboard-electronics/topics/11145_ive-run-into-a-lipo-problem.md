# I&rsquo;ve run into a LiPo problem

### Replies: 24 Views: 1889

## \#1 Posted by: minimorris77 Posted at: 2016-10-14T22:06:44.480Z Reads: 133

```
After I rode my board, I took off the enclosure because I needed to charge up my 2 Turnigy 5Ah 3s Lipos.

I immediately noticed only one of the 3s batteries was puffy. What would cause only one to puff up? Could it have to do with the fact that I charge them separately as 3s packs? The cells on the puffy one are at 2.8v/cell but when I plugged the not puffy one into the charger it showed 3.6v/cell. I am using an FVT120a ESC with the e-board firmware which doesn't let you select the LCV

Isn't this theoretically impossible in a series circuit like the because the ESC pulls from the cell with the highest potential?

Also, now I don't know what to do. I probably shouldn't use this battery anymore, but can I just go buy 1 3s pack, or do I have to have a matching set? The set only has about 8 cycles on them :(
```

---
## \#2 Posted by: michaeld33 Posted at: 2016-10-14T22:08:22.688Z Reads: 131

```
Many things can cause a puffy battery, manufacturing defects, shorting, pushing the battery too much, unbalanced cells, etc.
```

---
## \#3 Posted by: SimosMCmuffin Posted at: 2016-10-14T22:13:32.095Z Reads: 120

```
Are you sure they were both charged up fully or to an equal state before you started your set? 
Maybe the now puffed one was at a lower SoC (State-Of-Charge) when you started and therefore got ruined.

Asking because you said you charge them separately and therefore seems the likeliest reasons I could come up with.
```

---
## \#4 Posted by: Namasaki Posted at: 2016-10-14T22:14:58.059Z Reads: 115

```
Also, did you balance charge them? Or fast charge?
Where both packs same age?
There's nothing wrong with charging them separately but you need to always balance charge them.
```

---
## \#5 Posted by: minimorris77 Posted at: 2016-10-14T22:31:01.878Z Reads: 98

```
They were both the same age, and they were both balance charged... kinda. I usually charge them until at 4.4Ah for about 100 minutes. The reason I say about 100 minutes is it charges for 80-90 minutes at like 4.4Ah then I let it balance as it goes between 0-.1 for another 10-20 minutes till I stop it (all the cells are within 0.01V) If I don't stop it, it goes on for another 30 minutes being completely anal about the cell balance. Yes, I realize that makes me sounds ignorant. 

I was under the impression that they will all equal out and drain equally because the battery will pull from the highest cell. Is this not correct?
```

---
## \#6 Posted by: minimorris77 Posted at: 2016-10-14T22:38:36.547Z Reads: 88

```
Is it possible to instead hook up the balance plugs as 1 6s battery so I don't have to charge separately? 

So charge them at 6s, 4.4Ah.
```

---
## \#7 Posted by: Namasaki Posted at: 2016-10-14T22:39:25.475Z Reads: 83

```
[quote="minimorris77, post:5, topic:11145"]
I was under the impression that they will all equal out and drain equally because the battery will pull from the highest cell. Is this not correct?
[/quote]


I don't think that is correct. That's why it's so important to charge on balance mode and let the charger run its full cycle until it says it's done.
```

---
## \#8 Posted by: minimorris77 Posted at: 2016-10-14T22:43:45.252Z Reads: 77

```
Well shit.. Guess I learned a $60 mistake. I guess it could have been worse and blown up, and been a $200 mistake.

So I should probably buy two more packs?
```

---
## \#9 Posted by: Namasaki Posted at: 2016-10-14T22:44:59.415Z Reads: 75

```
[quote="minimorris77, post:6, topic:11145"]
Is it possible to instead hook up the balance plugs as 1 6s battery so I don't have to charge separately?
[/quote]

Yes, you can charge them in series as a 6s.
Your battery puffed because you drained it too low.  I did that once with 2 brand new 6s packs.
better not go below 3.6v when riding.
The lower your battery gets the lower its voltage goes and the more amps you pull out of it so the faster it goes.
Its like a vicious cycle. and voltage sag makes it even worse because the closer your amp drain is to the battery's capability, the lower the voltage sags under load.
```

---
## \#10 Posted by: minimorris77 Posted at: 2016-10-14T22:48:25.858Z Reads: 77

```
How can I monitor this when I cant set the LVC of the esc.. Just keep an eye on it with the little balance plug meters?

I don't know what LVC is set to nor how to change it.
```

---
## \#11 Posted by: Namasaki Posted at: 2016-10-14T22:49:42.157Z Reads: 73

```
get an alarm meter that plugs into the balance harness and monitors each individual cell.
```

---
## \#12 Posted by: Namasaki Posted at: 2016-10-14T22:51:58.224Z Reads: 73

```
https://www.amazon.com/gp/product/B0064SHG0Y/ref=oh_aui_detailpage_o06_s00?ie=UTF8&psc=1
```

---
## \#13 Posted by: minimorris77 Posted at: 2016-10-14T22:52:24.348Z Reads: 68

```
The problem with that is the batteries are in the enclosure so if/when it goes off I can't really turn it off.
```

---
## \#14 Posted by: Namasaki Posted at: 2016-10-14T22:53:27.036Z Reads: 63

```
you set the alarm for 3.4v and if it goes off you stop riding
```

---
## \#15 Posted by: minimorris77 Posted at: 2016-10-14T23:00:13.880Z Reads: 61

```
So if I'm far from home I can just turn the board off and push back and it won't make a peep?

Will it go off from voltage drops while I'm going up hills because the batteries are only 20C/30C 

I'll probably get this basic one from HK because I gotta get my new packs from there.

http://www.hobbyking.com/hobbyking/store/__58827__HobbyKing_8482_Lipoly_Low_Voltage_Alarm_2s_6s_AR_Warehouse_.html
```

---
## \#16 Posted by: Namasaki Posted at: 2016-10-14T23:06:08.847Z Reads: 61

```
If going up a hill sags the voltage below 3.4 then it would go off and you would want it to go off.
```

---
## \#17 Posted by: Namasaki Posted at: 2016-10-14T23:07:43.583Z Reads: 60

```
The one from hobby king looks good. as long as the alarm is loud enough
```

---
## \#18 Posted by: minimorris77 Posted at: 2016-10-14T23:08:25.381Z Reads: 58

```
I just checked the cells on my puffy pack:

Cell 1: 3.54V
Cell 2: 1.89V
Cell 3: 3.10V

There's something terribly wrong with this pack. :astonished:
```

---
## \#19 Posted by: minimorris77 Posted at: 2016-10-14T23:14:51.715Z Reads: 57

```
This also means it would always be plugged into the pack under the enclosure and it would drain the packs eventually then just go off and scare the crap out of me.
```

---
## \#20 Posted by: Namasaki Posted at: 2016-10-14T23:21:25.707Z Reads: 58

```
You could run your balance leads to a series adapter cable and run it outside to enclosure and mount the alarm on the bottom of your deck outside the enclosure
```

---
## \#21 Posted by: minimorris77 Posted at: 2016-10-14T23:33:17.018Z Reads: 55

```
Thanks for your help dude!
```

---
## \#22 Posted by: Namasaki Posted at: 2016-10-15T00:14:59.643Z Reads: 55

```
your welcome
```

---
## \#23 Posted by: SORRENTINO Posted at: 2016-10-15T01:24:46.494Z Reads: 54

```
Could also check the IR of the individual cells if your charger is capable of that. Looks like you had a bad cell and could have possible noticed it earlier if you periodically checked the IR. Like Namasaki said  if you set it to 3.4 it will beep but the lipo is almost always sagging alittle when your riding and if you stop when it beeps volatge should raise up to "resting voltage" and the alarm will go off. Cells with high IR will drain faster (sag more) then lower IR cells and will make your charger work double time to try and balance that bad cell. Just my 2 cents
```

---
## \#24 Posted by: tueboard Posted at: 2016-10-15T08:27:23.927Z Reads: 49

```
i had the same puffy problem and i had to throw the battery, i think that i over discharged it too much :(

I created some threads to better understand the lipo batteries:
http://www.electric-skateboard.builders/t/i-broke-two-lipo-batteries-and-i-dont-know-why/9684
http://www.electric-skateboard.builders/t/tips-for-the-lipo-batteries-to-last-longer/9683
```

---
