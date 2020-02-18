# Creating battery

### Replies: 55 Views: 1008

## \#1 Posted by: curtis Posted at: 2018-11-04T17:14:35.590Z Reads: 263

```
Dear friends,
I want to create a battery that is 10s. How many 18650's cells are needed? I do not have a spot welder. Is their any way to make a battery WITHOUT a spot welder? My goal is simple, I want to make a battery as cheaply as I can that is safe.
```

---
## \#2 Posted by: Indiangummy Posted at: 2018-11-04T17:17:25.702Z Reads: 264

```
It's really not recommend to solder the batteries as it can damage them. Us the search function on the forum you'l find all the information you need. This topic has been covered throughly.
```

---
## \#3 Posted by: notepad Posted at: 2018-11-04T17:20:04.040Z Reads: 254

```
You can make a pack without a spot welder, but your iron needs to be Very hot to melt the solder as fast as possible so as little heat is transfered to the cell.

the minimum of cells for a 10s1p is 10.  so upgrade to 10s2p would be 20 ... and so forth.  

There are some very good resources on this forum, just search for it and youll be sorted.
```

---
## \#4 Posted by: Benjamin899 Posted at: 2018-11-04T17:23:01.337Z Reads: 235

```
you can use NESE packs. You can get them at [18650.lt](http://18650.lt)
I use them and no problem. There are also others who have made builds with these modules.
```

---
## \#5 Posted by: Andy87 Posted at: 2018-11-04T17:32:13.387Z Reads: 216

```
The cell count depends on how much cells you want to add in parallel.
10s x p cells = cells you need
```

---
## \#6 Posted by: curtis Posted at: 2018-11-04T17:39:14.048Z Reads: 204

```
I know 10s means I only need 10 cells, however I want to be able to ride my skateboard fast up hills. So I want to be able to supply enough power to go 35 mPh.
```

---
## \#7 Posted by: curtis Posted at: 2018-11-04T17:41:31.017Z Reads: 198

```
Yes that looks like a good option, but those configurations are so small. They are also not customizable. But, alas I wouldn't have to use a spot welder.
```

---
## \#8 Posted by: Andy87 Posted at: 2018-11-04T17:42:04.124Z Reads: 188

```
Which cells you plan to use?
```

---
## \#9 Posted by: curtis Posted at: 2018-11-04T17:43:29.286Z Reads: 183

```
What makes you think I have to put any in parallel? I can put them all in series
```

---
## \#10 Posted by: Andy87 Posted at: 2018-11-04T17:44:32.686Z Reads: 176

```
Because no any 18650 can output so much current that you can reach your required speed.
```

---
## \#11 Posted by: Benjamin899 Posted at: 2018-11-04T17:46:08.191Z Reads: 169

```
what? as andy said. There is no single 18650 that delivers enough power or capacity.
```

---
## \#12 Posted by: curtis Posted at: 2018-11-04T17:48:01.072Z Reads: 165

```
I am confused as to what you mean. It can't be done or hasn't been done?
```

---
## \#13 Posted by: wafflejock Posted at: 2018-11-04T17:48:13.725Z Reads: 168

```
Yeah you'd have a 10S 36V nominal, with about 2.5Ah so you'd get about five miles assuming you can get going without sagging the cells to 0 volts.

The amp draw is the problem no single 18650 can supply the power needed in terms of amps, the watts delivered to the components is the voltage times amps, most cells will have something like 20A max discharge so you need them in parallel to deliver enough amps.  Also 2.5Ah is not a lot of capacity for range.
```

---
## \#14 Posted by: curtis Posted at: 2018-11-04T17:49:01.340Z Reads: 161

```
When did I say I wanted a single 18650?
```

---
## \#15 Posted by: Andy87 Posted at: 2018-11-04T17:50:57.369Z Reads: 160

```
Look
Your 10s battery can max output 20-30a.
If you add cells in parallel the current they can output add up
2p 40-60a
3p 60-90a and so on
but for every p-group you need another 10 cells in series.
So a 10s4p would be 40cells 
Or 10packs in series which each 4cells in parallel
```

---
## \#16 Posted by: wafflejock Posted at: 2018-11-04T17:51:38.612Z Reads: 156

```
When you connect cells in series you increase voltage but the amps you can draw and the amp hours capacity can only be increased by putting more cells in parallel.
```

---
## \#17 Posted by: Andy87 Posted at: 2018-11-04T17:54:55.480Z Reads: 155

```
[quote="curtis, post:7, topic:73406"]
configurations are so small
[/quote]

Those not too small, it’s just one of the series packs. You need 10 of this packs to create your 10s battery you want to build.
Each pack connect the cells in parallel inside, not in series
```

---
## \#18 Posted by: Battosaii Posted at: 2018-11-04T18:22:58.998Z Reads: 156

```
Guys let him use the search function, spoon feeding him this info won't help him in the long run.

Making batteries is a serious matter and should not be attempted unless you have a basic understanding how they work and you clearly do not. 

Do your self a favor buy this book and read and study it as much as you can before you attempt to make a battery. These things have enough amps to kill you don't underestimate their power.
DIY Lithium Batteries: How to Build Your Own Battery Packs https://www.amazon.com/dp/0989906701/ref=cm_sw_r_cp_apa_i_ZIZ3Bb0EVR6E1
```

---
## \#19 Posted by: wafflejock Posted at: 2018-11-04T18:36:40.075Z Reads: 155

```
Yah fair point.  Regarding amps though we don't deal with high enough voltages for it to be a problem (unless you stab yourself with the probes your skin has pretty high resistance) except when it comes to vaporizing wires and blowing up cells if they over heat but agreed it's not something to just jump into without a good understanding of electricity.
```

---
## \#20 Posted by: curtis Posted at: 2018-11-05T06:03:48.329Z Reads: 142

```
Without a solder as well.
```

---
## \#21 Posted by: Schulerbible Posted at: 2018-11-05T06:10:57.583Z Reads: 134

```
You should really do more research on how to build a board that actually works and a battery that doesn't blow nek minnit.
```

---
## \#22 Posted by: mynamesmatt Posted at: 2018-11-05T06:16:50.348Z Reads: 132

```
dude, do some research.
that's all :)
```

---
## \#23 Posted by: curtis Posted at: 2018-11-05T06:17:20.021Z Reads: 132

```
I have I just wanted the opinion of the internet.
```

---
## \#24 Posted by: mynamesmatt Posted at: 2018-11-05T06:19:31.046Z Reads: 134

```
https://www.electric-skateboard.builders/t/series-or-parallel-battery/13422
```

---
## \#25 Posted by: legend27 Posted at: 2018-11-05T06:29:02.872Z Reads: 129

```
Before you order anything you should really read a lot about it. Batteries are dangerous if not handled correct and can potentially burn down a house. We don't want to hear about another battery fire. Please do some reading.
```

---
## \#26 Posted by: L3chef Posted at: 2018-11-05T06:40:43.552Z Reads: 129

```
Red flags. Be carefull mate
```

---
## \#27 Posted by: Nordle Posted at: 2018-11-05T09:01:26.744Z Reads: 124

```
:fire: :fire_engine: :derelict_house:  good look building a battery and not even knowing how many cells you need-.-
[quote="curtis, post:23, topic:73406, full:true"]
I have I just wanted the opinion of the internet.
[/quote]
you have a lot to read, seems thats the opinion of the internet
```

---
## \#28 Posted by: lrdesigns Posted at: 2018-11-05T09:05:42.437Z Reads: 125

```
Check here for safety tips 
https://www.electric-skateboard.builders/t/please-review-my-battery-pack-so-i-dont-make-a/70102?u=lrdesigns 

Its not really recommended to solder 18650's unless your very experienced, its much hard to do right then welding. 

For 10s most guys are using 10s5p so 50 cells. This gives good power and long range. 

Its much simpler to build a lipo pack if your just starting out. It can be done with no soldering if you have the right adapters.
```

---
## \#29 Posted by: curtis Posted at: 2018-11-05T15:31:59.089Z Reads: 117

```
The answer to that depends on what your doing. Do you want higher discharge, or do you want the battery to have more range?
```

---
## \#30 Posted by: Itsmedant Posted at: 2018-11-05T16:11:46.018Z Reads: 115

```
He wasn't asking you a question, he was posting a thread that you should read through.

There is tons of information on here about building batteries. It seems like you need to learn about the batteries a bit more before trying to make one. Or there are alot of people on here that build them for the community.

They aren't difficult things to make, you just need to follow the right protocols to make sure you are building something that is reliable and safe.
```

---
## \#31 Posted by: Itsmedant Posted at: 2018-11-05T16:14:21.454Z Reads: 112

```
Also, a 10s battery, you are going to be hard pressed to make one that truly will hit 35mph. You will ahve to play around with your gearing and motors at that point.

If you are trying to build a "cheap" board that hits 35 mph, I suggest you read through ALOT of build threads to see what other people are doing, you'll find very quickly that "cheap" and "over 30mph" do not go together very well.
```

---
## \#32 Posted by: pedro Posted at: 2018-11-05T17:41:08.048Z Reads: 113

```
you can buy batteries with tabs included, so you don't have soldered directly in the batteries,I build my pack in this way, but I don't recommend, because is too dangerous


like this

![imagem|400x300](upload://9Y0Hibkko9aPXcu4xJ2Brek3J4Z.jpeg)
```

---
## \#33 Posted by: Battosaii Posted at: 2018-11-05T19:39:59.812Z Reads: 108

```
That would work if you solder the tabs to a bus bar, won't exactly be cell level fusing but it would work
```

---
## \#34 Posted by: Acido Posted at: 2018-11-05T20:24:27.166Z Reads: 106

```
i would reccomend you not doing this unless you are 100% sure that you know what you are doing, and that your doing it properly
battery is the heart of your build if you want a cheaper option go with lipos
but if you want a li ion pack that has its advantages i would do it properly, because if its not it can end in a ugly way

im happy to assist you with your pack, I make them as a service so i know what im doing
but if you decide to pay someone to do it im one option, a spot welder is essential and it itself if around 100$+shipping

use as much insulation as you can, especially on the positive tab and between the p groups!
Either some 3d printed plastic or fishpaper
```

---
## \#35 Posted by: curtis Posted at: 2018-11-05T21:13:00.659Z Reads: 98

```
Who are you talking to?
```

---
## \#36 Posted by: curtis Posted at: 2018-11-05T21:42:02.160Z Reads: 95

```
I have gotten all the information I need for this thread. When using 18650 batteries I need  to use a ton of batteries if I want to be able to get my board to be able to go 35+ mPH. If I am going to be using a combination of 18650 cells  iI would make it make the capacity of the battery to last longer. 
.
```

---
## \#37 Posted by: Andy87 Posted at: 2018-11-05T21:46:24.393Z Reads: 95

```

Not a ton but min 40 you will probably need.
What exactly you mean with
[quote="curtis, post:36, topic:73406"]
If I am going to be using a combination of 18650 cells iI would make it make the capacity of the battery to last longer.
[/quote]

Sorry but didn’t understood
```

---
## \#39 Posted by: pat.speed Posted at: 2018-11-05T21:57:58.493Z Reads: 95

```
Hey mate, I don’t mean to be rude but at this point in time you are not ready to make a lithium ion battery. You need to know all of this stuff well before you start building. You also must know how to connect the cells safely, strongly and just correctly in general. Failure to do those things can lead to potentially catastrophic disasters, in order of not so bad to bad this is what might happen, cut yourself, you burn yourself, your batteries are ruined, your batteries smoke, they catch fire outside, they catch fire inside, your house gets burnt down, and worse of all every person in the house or building gets put at a sever risk when the battery is incorrectly built. 

So please do a lot more reading, I’m not saying you can’t do it, I’m just saying you need to know how to do it right first
```

---
## \#40 Posted by: Scream Posted at: 2018-11-06T00:07:57.346Z Reads: 98

```
I know it might seem like everyone is being killjoys but comments like this are why people are suggesting you go with a simple lipo set up or do a lot more reading.

Parallel vs series =/= range vs discharge.

There are a lot of nice people on this forum that would be happy to help you. I think what everyone is saying is that it seems like you need to start from learning the basics, and there are already a bunch of good online resources to increase your knowledge of electricity rather than someone on this forum writing you a personal electronics curriculum.
```

---
## \#41 Posted by: curtis Posted at: 2018-11-08T22:45:56.928Z Reads: 89

```
I agree with you about what you are saying about parallel and series. You do have to know exactly what you are doing.
 I am probably not going to go with lipo's simply because it defeats the purpose of having a DIY electric skateboard. That is my opinion.

I have done research and am in the position to move forward. I have been on with this forum for the past 2 years. I think using soldering in battery packs is very messy. I think my best bet would be getting vruzend solder less battery pack. Simply because of the versatility that it provides. I can make whatever connections I want without it being dangerous and it's customizable.

In my time here people have always told me the same types of things "you don't know what your talking about. Your going to build a bomb. " I could not disagree more.

I do know what insulation is and I understand the danger of using a spot welder. I know how the spot welder works. I know what series is and parallel. As well as how to combine them.

Curtis
```

---
## \#42 Posted by: curtis Posted at: 2018-11-08T22:52:27.991Z Reads: 92

```
I agree with you about what you are saying about parallel and series. You do have to know exactly what you are doing.
I am probably not going to go with lipo’s simply because it defeats the purpose of having a DIY electric skateboard. That is my opinion.

I have done research and am in the position to move forward. I have been on with this forum for the past 2 years. I think using soldering in battery packs is very messy. I think my best bet would be getting vruzend solder less battery pack. Simply because of the versatility that it provides. I can make whatever connections I want without it being dangerous and it’s customizable.

In my time here people have always told me the same types of things "you don’t know what your talking about. Your going to build a bomb. " I could not disagree more.

I do know what insulation is and I understand the danger of using a spot welder. I know how the spot welder works. I know what series is and parallel. As well as how to combine them. I am not saying I know everything, but I am saying I understand enough to move forward. I even understand how to create the vesc controller, however I think thats too much work.

I am going to use this forum and ask questions when I need to know more answers. I am at a good point right now. Thank you very much for everyone's input on this topic.

Curtis
```

---
## \#43 Posted by: curtis Posted at: 2018-11-12T03:44:41.121Z Reads: 85

```
Hello fellow e-skaters
 all, I was wondering if you truely need a bms? 
or would a hobby charger be a better option? to charge my battey system lets say 10s 4p
```

---
## \#44 Posted by: J0ker3366 Posted at: 2018-11-12T04:28:18.769Z Reads: 86

```
Bruv. You have been asked, directed and damn near begged to do some research. This site is full of the answers to your question. Everyone else won't say this but it needs to be said. @mmaner if I'm out of line tell me...

You are clearly uneducated in battery building. If you had the littlest of knowledge in it, you would have known about if bms is needed or not. And I'm not going to tell you cause all you're going to do it come back and ask which one you should get. It's redundant as shit as to how many people come here and expect to be handed all their answers by the PROs. Yeah I said it 😎 Seriously. Do some damn research. Stop asking us the questions that can be answered by using that search bar. I'm not saying you are lazy, but you're going about it the lazy way. No one will help you in life if you arent willing to help yourself.

Life lesson featuring Mista J. *Mic drop* @Sender lol
```

---
## \#45 Posted by: pat.speed Posted at: 2018-11-12T05:05:35.926Z Reads: 81

```
Ooooooooof he just got told. Lol
```

---
## \#46 Posted by: NewbieBoardBuilder Posted at: 2019-01-13T21:15:38.307Z Reads: 66

```
a balance of both...
```

---
## \#47 Posted by: Sebike Posted at: 2019-01-13T21:37:51.772Z Reads: 59

```
to build a battery for esk8, you just buy a ton of cells (if you want to go 35 mPh (sic! @b264 )). throw it in a bag with some solder, heat shrink and solder paste. zip it and shake. 

voilà! no need for search buttons!!
```

---
## \#48 Posted by: dareno Posted at: 2019-01-13T21:40:48.251Z Reads: 62

```
I bookmarked this thread because sometimes I just need a good laugh.  Everyone banging their respective heads against the wall so to speak and it just not getting through. :rofl:
```

---
## \#49 Posted by: Sebike Posted at: 2019-01-13T21:41:55.869Z Reads: 59

```
someone's trolling us for sure
```

---
## \#50 Posted by: mynamesmatt Posted at: 2019-01-13T22:50:48.986Z Reads: 52

```
[quote="curtis, post:42, topic:73406"]
I am probably not going to go with lipo’s simply because it defeats the purpose of having a DIY electric skateboard. That is my opinion.
[/quote]

good fucking Christ. sorry i have no sag, 30km of range and a top speed of 55kmh. get that for $250 with liion without burning your house down...
```

---
## \#51 Posted by: dareno Posted at: 2019-01-14T00:09:20.677Z Reads: 48

```
This is 2 months old this thread and pretty sure it was a pure trolling exercise.  Either that or he did indeed burn his house down lol
```

---
## \#52 Posted by: AlanZhou Posted at: 2019-01-14T02:57:42.080Z Reads: 43

```
@mynamesmatt geez


To kurtis:

What kind of earth defying logic and opinion is that? 
 
_"I am probably not going to go with lipo’s simply because it defeats the purpose of having a DIY electric skateboard. That is my opinion."_

Im gonna keep this in my quote book.

and a simple video on youtube could of explained everything..... :joy:

and why did i just notice this topic?
```

---
## \#53 Posted by: curtis Posted at: 2019-04-29T04:30:13.019Z Reads: 31

```
No I didn't burn anything down. However, I wasn't able create a battery at my college because they thought I was creating a bomb. Even kits like VRUZEND which. I don't have to solder anything. The same campus won't let you  borrow a 2 foot ladder because you are too much of a liability.
```

---
## \#54 Posted by: curtis Posted at: 2019-04-29T04:49:01.111Z Reads: 31

```
Easier and better are 2 completely different things. Yes it is a lot easier to set up with Li Po's. Some people enjoy the art that an electric skateboard can do. You can still mess up when setting up Lithium Polymer batteries. Most people don't want to acquire the knowledge and time required to create battery. It is much simpler to just go out and buy some Li Po's, but their is no fun in that. Some people enjoy projects putting things together and such. 

I want to make a battery. Now for 90% of people that is not something that they want to do. Their are pros and con's to doing each method.
```

---
## \#55 Posted by: Vero Posted at: 2019-04-29T04:57:28.938Z Reads: 31

```
You probably were making the equivalent of a bomb with the knowledge you seem to lack any battery you made i woukdnt touch with a 10 metre stick
```

---
## \#56 Posted by: curtis Posted at: 2019-04-29T05:16:16.943Z Reads: 30

```
Is that a challenge?
```

---
