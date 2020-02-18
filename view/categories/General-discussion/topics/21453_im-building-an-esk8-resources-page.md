# I&rsquo;m building an Esk8 Resources Page

### Replies: 18 Views: 1315

## \#1 Posted by: longhairedboy Posted at: 2017-04-20T17:23:11.780Z Reads: 155

```
I'm creating a section on my website for listing good informational resources and tools for DIY Esk8 Builders. 

I'm not really trying to make it a vendor list as i plan to make a seperate collection of links for that, so i'm looking more for forums and calculators and site that have how-tos for making parts and comparison charts and things like that. I could spend a lifetime compiling this so since i think this would be a good use of time but don't have a lot of it, i thought i would ask you guys to help. My starting list is short because i literally just started on this last night. 

So far i have the following listed on my new page at https://longhairedboy.com/pages/esk8-resources :

[THE ESK8 CALCULATOR](http://calc.esk8.it/)
Figure out rough estimates of top speed and range for your build. 

ELECTRIC-SKATEBOARD.BUILDERS FORUM (this website)
a forum filled with builders. this place is literally overflowing with good information and community support. 

[ESK8 COMPARISON CHART](http://compare-skateboards.com/)
an excellent way to compare damned near every model of electric skateboard available for purchase from anywhere. Complete with specs, links to vendors, the works. 



Also, i figure this would be a great way to compile the list for this site as well. 

Thanks for the help!
```

---
## \#2 Posted by: mmaner Posted at: 2017-04-20T17:26:50.785Z Reads: 139

```
http://esk8.today/2016/12/28/how-far-can-i-ride/
```

---
## \#3 Posted by: longhairedboy Posted at: 2017-04-20T17:36:26.453Z Reads: 121

```
thanks! I just updated my page. That's a really good one.
```

---
## \#4 Posted by: mmaner Posted at: 2017-04-20T17:37:07.938Z Reads: 116

```
I like it, its ugly but works great...kind of like me :slight_smile:
```

---
## \#5 Posted by: mmaner Posted at: 2017-04-20T17:46:27.222Z Reads: 115

```
Here's the formulas I use for everything from Range and ERPM to Max Current and Constant DC Rate.

_* a note to all readers..._
I did not discover these, I am not Pythagoras or Pascal, this is just what I have discovered and collected (mostly from posts on this forum) over the months that I've been building boards (said main-lining powered boards).

**WATT HOURS**
  mAh * V / 1000 = Wh
  _example:  7500 * 37 / 1000 = 277.5_
  
**RANGE**
  wh / 5 * 0.31(miles) = range in miles
  _example:  277.5 / 5 * 0.31 = 17.2_
  
**ERPM (Electrical RPM)**
  KV * MAX Voltage * 7 = ERPM
  _190 * 42 * 7 = 55860_

**RPM**
  MAX Voltage * KV = RPM
  _example:  42 * 190 = 7980_

**MAX KV**
  8600 / MAX Voltage = MAX KV
  _example:  8600 / 42 = 204.76_

**MAX VOLTAGE**
  8600 / Motor KV = MAX Voltage
  _example:  8600 / 190 = 45.26_

**MAX WATTS**
  MAX Battery Amps * Volts per Cell * Cells = MAX Watt
  _example:  60 * 3.7v * 10 = 2220 Watts_

**MAX CURRENT**
  C Rating x Capacity (AH) = Max Current
  * C Raiting = Disharge Rate
  * Capacity = mAh Rating
  _example:  30 * 80000 = 240a MAX CURRENT_

**CONSTANT DISCHARGE RATE**
  AH * C = Maximum Constant Discharge Rate
  * 1000mAh can deliver 1 Ampere (1000mA/1000) for 1 hour(s) or 1AH
  * 8000mAh can deliver 8 Ampere (1000mA/1000) for 8 hour(s) or 8AH
  _example:  8AH (8000mAh) * 30c = 240.000 mAh Discharge Rate = 240 Ampere Constant Discharge Rate_
```

---
## \#6 Posted by: longhairedboy Posted at: 2017-04-20T17:54:01.788Z Reads: 96

```
oh that's good. I think i might do a page for this kind of thing too. Thank you.
```

---
## \#7 Posted by: mmaner Posted at: 2017-04-20T17:54:33.618Z Reads: 93

```
no worries brudda.
```

---
## \#8 Posted by: rwxr Posted at: 2017-04-20T19:12:49.240Z Reads: 87

```
Maybe snatch some diagrams from the diagram-thread? With authors permission of course.
Like wiring diagrams for BMS, Parallell, Series, Loop-key etc.
```

---
## \#9 Posted by: Okami Posted at: 2017-04-21T10:13:55.825Z Reads: 71

```
The idea about creating nice infographics has floated in my head for a while but for this we firstly need a source or a 'block' of info, everyone agrees about (more or less)

Then we would need a designer, who would make all that in picture format.

--

Im not against reading and reading and researching in gerenal, i just think some of the info could be "compressed" to be more easly found and 'read'.

Maybe im wrong and i would be happy if someone would prove why infographics are bad idea and why we would loose info because of using them
```

---
## \#10 Posted by: Jebe Posted at: 2017-04-21T11:07:53.793Z Reads: 69

```
This kinda stuff ?
http://www.instructables.com/howto/vacuum+pump/

http://www.instructables.com/id/Bare-Bones-Vacuum-Forming-Box/
```

---
## \#11 Posted by: longhairedboy Posted at: 2017-04-21T11:14:12.525Z Reads: 65

```
I like this idea.
```

---
## \#12 Posted by: Okami Posted at: 2017-04-21T13:11:44.954Z Reads: 77

```
@longhairedboy  Yeh, I agree, now we just need these ''2 parts'' to emerge.. ''a person who sources/compiles the info'' and the ''designer''

I even have some topics which could be covered there:

---
**Regular (car, heli, boat) ESC's VS VESC** - 

_Which is better?_

_Which offers more features / safety?_

_Does the features justify the price?_

_Or Is it worth it to pay less and get less, when you can get way more for a bit higher investment?_

----
**LIPO vs Li-Ion (18650 / 26600)** - 

_Which to choose?_

_Which one is better?_ 

_What about the size?_

---

**Mountainboard building ABC**

_Deck stifness? Soft or hard?_

_Trucks? Either Spring or Skate? Benefits/cons of each?_

_Tire size and profile? Which and when better?_

_Binding types. Strapped or not-Strapped?_

---

**Designing battery power requirements / range.**

_Should I choose more ''powerful'' battery or more range? Why?_

_Battery cost related to size / power / energy density and other factors_

_How to charge batteries? How much time will it take to charge my battery?_

_Do I need any additional connections for my battery? What about BMS?_

----

**Power consumtion, hills, esc's that overheat, motors that get hot etc (everything that does not fit in previous parts)**

_Will my board be able to go up this hill?_

_Electronic brakes. Are they reliable enough?_

_Most common failures of esk8_

_How much power my motor can produce? Will it overheat when riding in general conditions?_

---

I could perhaps go and go.. but I will stop for now, to be honest, I agree to take one topic, compile info and then post it here (or in a new topic) for others to ''review it''. 

After info has been reviewed by more than a few people, I think it could be made in picture format and posted in ''ESk8 bulletin / message board'' section for others to view!
```

---
## \#13 Posted by: Okami Posted at: 2017-05-02T19:54:47.314Z Reads: 56

```
No more new replies?

Im still sticking to the idea someone should make ''info page'' .. at least a little bit of guidance into esc's / batteries .. motor configs.. etc

I do know that Enertion has covered a lot of these topics in his videos.. but I still think textual / graphic information in such format is also needed..

--
@KTMinni

This is a good ''snip'' I got from Maxid about some Vesc's with which extra caution should be taken:

[quote="Maxid, post:19, topic:16764, full:true"]
Maybe we should add who is selling Maytech VESCs without a bootloader. Seems like that problem pops up quite often now.

e-greenmotion, michobby, protoboards and alien resell Maytech VESCs as far as I can tell
[/quote]

@ https://www.electric-skateboard.builders/t/worldwide-vesc-directory/16764/18
```

---
## \#14 Posted by: tueboard Posted at: 2017-05-02T20:27:33.675Z Reads: 55

```
hi,

i made this esk8 directory a few months ago, where people can share their esk8 builds and specs :)
http://esk8builds.com/
```

---
## \#15 Posted by: Okami Posted at: 2017-05-02T20:30:37.409Z Reads: 48

```
@tueboard  Maybe your page could be used as a base to 'host' some of the info..

I dont mind creating some tuts on the forum.. but on a webpage everything just might look a bit better..

When thinking about this.. im not even sure there is a page which lists all sources where to get Vesc in the first place..

After that would come some other sources + Car escs and what we know about them so far..
```

---
## \#16 Posted by: saul Posted at: 2017-05-03T07:56:42.477Z Reads: 44

```
sorry I'll make the next one prettier! lol

thanks for linking.
```

---
## \#17 Posted by: mmaner Posted at: 2017-05-03T11:48:04.178Z Reads: 46

```
Lol, it's all good brother 😀
```

---
## \#18 Posted by: longhairedboy Posted at: 2017-05-03T11:55:58.013Z Reads: 48

```
[quote="tueboard, post:14, topic:21453"]
i made this esk8 directory a few months ago, where people can share their esk8 builds and specs :slight_smile:
[/quote]

Added! that's exactly the kind of thing i'm looking for since i'm mostly just trying to build a sort of link list / directory.

[quote="Okami, post:15, topic:21453"]
Maybe your page could be used as a base to 'host' some of the info..

I dont mind creating some tuts on the forum.. but on a webpage everything just might look a bit better..
[/quote]

That would be great too. Then i can link to them. Also, i could host things like that (tutorials etc) as well.  I have a domain i just recently registered that might be perfect for it. esk8.build. If there was enough content compiled for it i would be willing to host it and even flesh out the site. just an idea. I grabbed a few "esk8" domains recently in order to capture them for the community to use in some way, and i'm willing to host on them for free and set up blogging platforms or whatever for articles so people can write things like that.  I'm on Dreamhost, and i've been with them for almost 10 years, so i have accrued a vast amount of bandwidth and hosting space. Hosting informational sites on these domains and paying to keep them hosted would be my pleasure. And i'll be happy to keep the designs fresh too.  

The domains i recently got are:

**esk8.build**
possibly for tutorials, instructional videos, articles on building. Not a forum, but maybe comments)

**esk8.me** 
i was thinking about some kind of community driven buyer's guide.

**esk8.racing**
obviously an esk8 racing blog with multiple writers and parts reviews

**esk8.life**
lifestyle blog about esk8ing life stuff, i don't know. I saw it and thought of hipsters on boosteds with $9 coffees and images of boards leaning against walls next to flowing curtains. I was drunk. 

At the moment they're all pointed to my stuff since i didn't want to put up a bunch of squatter pages. 

if something gets started and looks like its gaining traction on one of these domains i would consider running ads to pay the writers and possibly improve hosting if needed, but to start it would have to be a volunteer/community type thing and run in the space i have already. 

Also, i'm not building forums. This is the forum. I'm just trying to help flesh out some places to put good article type info where it can easily be found and maintained by the community.
```

---
