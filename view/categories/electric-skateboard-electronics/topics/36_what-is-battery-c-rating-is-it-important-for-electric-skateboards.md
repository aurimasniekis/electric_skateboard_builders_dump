# What is Battery &ldquo;C&rdquo; Rating &amp; Is it important for Electric Skateboards?

### Replies: 16 Views: 29909

## \#1 Posted by: onloop Posted at: 2015-07-16T02:30:02.899Z Reads: 2161

```
I remember *Fully-Stressing* about what parts to buy when I was building my first electric skateboard, mostly because I didn't have the money to make any mistakes. I wanted to make sure I bought all the correct & best suited parts for the job first time round. I was on a tight budget but I also didn't want to skimp on the important stuff.

One of the most important & expensive parts of your eSk8 build is the battery, so I started to research, I wanted the best bang for my buck based on my knowledge at the time.

**Here are some of my search queries**
"What is the best battery"
"Most powerful battery"
"Best battery chemistry"
"Peak power draw from electric skateboards"

*The problem is when you start researching stuff like this you end up with more questions than answers.... it's worth noting that after three years of reading & testing batteries I'm still learning... so maybe I'm just a slow learner! But let me tell you there is a lot of bullshit to filter through as well.*

Anyway, After a few weeks of reading  I decided to buy a Lipo because I learned that they have really high discharge rates & are high in power density. Meaning per gram they hold a lot of power. So they must be good!


----------


**So how can you determine the discharge rate of a battery?** 

Well fortunately this is clearly written on the label. **The 'C' rating of the battery below is 20C**. This means the the battery can peak output at 20X its capacity. 

So what is the Capacity? Thankfully it is also on the label of all batteries, this one below is 3000mAh or 3Ah. So this pack can output 20 x 3Ah making the rated **peak output for this battery 60Ah.** You can get Lipo batteries with much higher C rating and also batteries with much higher mAh. 

<img src='/uploads/db1493/original/1X/4701df3e4c64f6df95ed16a2b27bb2ac00148776.jpg'>

*My first battery for an eboard was an 8000mAh 30C Lipo, So 30Cx8Ah = 240A output! Wow! thats alot... so my board will be much better right?.... well not necessarily*

So now you know how to determine the output amount of any battery, but this information is useless unless you know what power an electric skateboard needs to function. 

**So how much power is actually required for an electric skateboard to move a human from a stationary position to ball tearing top speeds?**

The way to work it out is to buy a watt meter and install it onto your eboard, it goes in-line between the battery & the ESC, it gives you a real-time readout of how much power is passing through it.
<img src='/uploads/db1493/original/1X/a9ef665b4ef05153cb5f1d90fb75cdbb8c8b6cb7.jpg'>


It shows you peak amps & watts, also voltage. So you connect this to your board and go ride around to see how much power you are using.

>**BUILD TIP**  *You really don't need one of these permanently integrated into your eSk8. The info it displays is great to know initially but once you know the performance of your board the info really doesn't change so it becomes added weight and unnecessary wire bulk, also looking down at your feet when riding is dangerous!*

You will notice it will peak when starting from stationary, when you go up hills it will peak, basically when ever the motor has a load to push it will peak, But cruising around your board should only be using 15-20A of power. Actually you want low numbers you don't want high amps.

**So don't go brag to your mates about how awesome your 6KW (24V X 250AMPS) electric skateboard is!**

I can assure you that if your electric skateboard pulls too many amps you won't have an electric skateboard for long & your battery will likely get damaged from discharging too quickly & over heating. What you want to build is a skateboard that is power efficient when moving your mass, one that doesn't get hot even when hitting the big hills. Heat is power that got wasted!

Having an electric skateboard use too much power would be like bragging about how much black smoke pours out the muffler on your car. Its not that you have a really powerful eSk8, it's because you designed the drive train incorrectly. My design philosophy is **Powerful, Efficient & Robust**. These characteristics must be balanced otherwise failure will occur. Having the power & using it efficiently is two different things. So if your setup is under powered for your load (read "body weight") it wont be efficient. 

So yes your motors might be rated to 2400Watts (2.4kW) Each & Your Lipo might be able to out put 240AMPs and you might have a 150A Continuous ESC....  but you don't really want to reach the peak... its way to hot there & heat is bad!. 

**The best eboard will have an over engineered power system with safety features built in to prevent disaster**
.
Specifically when it comes to batteries, if you over discharge them, or discharge them too rapidly you will drastically reduce the life. So you need to be able to limit the power that is being requested by the motors & ESC. You can do this electronically or mechanically by reconfiguring the drive train gearing ratio.

Brushless Outrunner Motors are hungry little monsters... if you keep feeding them juice when a given load on them doesn't decrease they just want more juice. This could happen if you try riding up a big hill with a setup that is under powered for your mass. This appetite motors have for more power will rapidly convert to heat and your motor melts. So how do you stop this?

>**There are two electronic ways of managing how much power your system uses**
1. A Battery can have its own built-in battery management circuitry, commonly known as a BMS or PCB or PCM.
2. The Motor controller can have current limiting features built in.

I recommend both of the above. You might also consider using a fuse directly after the battery just in case things heat up melting the insulation on your wires & shorting out the entire system and destroying everything in a spectacular fire.

So the moral of the story is, you really don't need the highest "C" rated battery on the market. What you want is a battery that is specifically designed to easily deliver plenty of power up to the limit you require. Ideally you also want one that protects itself using a built in circuit, so if it is asked to deliver too much power it will limit the discharge. This will ensure your ESC & Motors are protected and also ensures your battery lasts a very long time.

I recommend that 60A Peak is enough for an electric skateboard. If you are constantly needing more then this amount of amps you should increase battery voltage & increase the mechanical reduction to lessen the load on the motor. Or go on a DIET!

**Higher Voltage = Lower Currents**
**Less Load = Lower Currents**
**Lower Current = Less Heat.**
**Less Heat = Longer Life & Improved Reliability of electronics.**
```

---
## \#2 Posted by: torqueboards Posted at: 2015-07-16T03:17:44.177Z Reads: 1761

```
Awesome post and well said.

I've also noticed the same discharge rates as well and it has been more then enough power to climb up hills here in SF.

Lipo's are fairly easier to get but 18650's are capable of higher discharge rates but are harder to get. Although, the added discharge rates most likely wouldn't be needed.

I think the key point is always having the correct gearing for the users intended use. If your motors are hot when riding = your setup is very inefficient and you should be most likely adding reduction to your current gearing setup and/or adding voltage to accommodate the lack of power. Of course, both would be better.

With a very efficient setup for your intended use - your setup should last 1,000 to 2,000 miles easy with no issues at all if not way more.

Do not stress the motors on purpose. You want to make things easy for the motors otherwise burned motors/escs = more money.

ESCs and Motors will only fail upon stress and overload which it wasn't designed to handle.

With that said 63mm are more forgiving in dispersing heat due to the larger motor (capable of more setup design mistakes) size versus 50mm motors which will get hot faster if your setup is highly inefficient.
```

---
## \#3 Posted by: ZachNYC Posted at: 2016-11-06T22:49:08.833Z Reads: 1051

```
Do you know by any chance if the wiiiciever has built in current limiting features?
```

---
## \#4 Posted by: Kstew70 Posted at: 2017-04-29T09:33:17.072Z Reads: 836

```
Okay so I'm making my own board with 4x 5000mah 4s 30c LiPos.  I will make 2 sets in series then 2 sets in parallel which will give me a total of 8s 10000mah 60c.  I want my board to have a great range.  I hope that will do it.  I'm also using dual 6354 sk3 260kv motors.  And 2 VESCs.  I weigh about 230 lbs though so I tried to compromise for more torque than top speed on my drive train with 72mm wheels.  But I'm using a 14:27 ratio from pinion to sprocket because I'm using a chain drive instead of a belt which will rip easier.  Do you think the board I am making will work? If not do you have any suggestions that could make it better? I love riding these boards, and it also stimulates the mechanical engineering student inside me!  Thanks a lot!!!
-Kurt
```

---
## \#5 Posted by: gee Posted at: 2017-05-23T05:23:22.991Z Reads: 704

```
Hello, I'm new here.I want to know is it possible to build a electric skateboard that can switch out battery with ease?
```

---
## \#6 Posted by: marcuscrackus Posted at: 2017-05-30T20:50:26.458Z Reads: 659

```
[quote="Kstew70, post:4, topic:36"]
5000mah 4s 30c
[/quote]

Kurt

Did you make the board in the end? if so how did you get on. my biggesrt concern at the moment is battery type. How are you going about charging the betteries?
```

---
## \#7 Posted by: wafflejock Posted at: 2017-07-06T18:55:09.091Z Reads: 554

```
Working on it https://cad.onshape.com/documents/15cd342c90ae1b0b6fd666bf/w/40780c7d8d67fd69a32fbf6e/e/fe1a99d1423c52e012228250  there are a few other e-skateboard swappable battery designs out there with various ways to clip a battery in and out but usually a proprietary battery pack.  It is yet to be seen if this will work in practice but my design should in theory keep things well connected while riding and still have the batteries be swappable (standard LiPos).
```

---
## \#8 Posted by: Snowi Posted at: 2017-07-14T18:28:10.064Z Reads: 513

```
do you think its safe and efficient to have two 5000mAh batteries, both with 6S and 20C? Do I need to it make a parallel or series?
```

---
## \#9 Posted by: the1515 Posted at: 2017-08-29T17:28:22.185Z Reads: 443

```
Hi Snowi, I just see your message "do you think its safe and efficient to have two 5000mAh batteries, both with 6S and 20C? Do I need to it make a parallel or series?" and I was wondering do you test this configuration, and did you do parallel or series, and even if you didn't test it, have you the answer ? Thanks
```

---
## \#10 Posted by: wafflejock Posted at: 2017-08-29T17:33:48.347Z Reads: 446

```
You'll be better off going in series and getting higher voltage in terms of electrical efficiency, but putting the batteries in series means adding the voltage and keeping the capacity mah and discharge rate the same.  So you'd have a 12S 5Ah at 20C or 100A max discharge, which should be fine because at 12S you're at 3.7V*12 = 44.4V * 100A = 4,440W which is more power than you'll likely ever draw through the system (even assuming you get dual drive this should be plenty).  That said higher C rating is always better (assuming it's a legit rating) the C rating effectively tells you the internal resistance of the battery and therefore how much it cooks itself during use and how much voltage dip it will have when under load (while drawing lots of current).  If you go in parallel you would add the mah and C ratings/max discharge of both batteries since half is coming from each but you stay at the 6S voltage of 22.2V and therefore need to dump twice the current to get the same power delivered.  Personally run two 5Ah 5S in series (20C but again higher is better) for a 10S setup on a 149kv SK3 6374 single drive setup.

http://calc.esk8.it/#{"batt-type-lipo":1,"batt-cells":10,"motor-kv":149,"system-efficiency":85,"motor-pulley-teeth":16,"wheel-pulley-teeth":36,"wheel-size":83}|

You can also roughly calculate your range in terms of Watt Hours, you get watt hours by multiplying amp hours by voltage.  If you go parallel or series you'll see you end up with the same Wh regardless of how you arrange (series or parallel) because watt hours is the actual energy in the cells (which is the same regardless of how you arrange).  The difference is at higher voltage you can deliver more watts with less loss through heat because heat loss increases as you increase amperage but not as you increase voltage (I^2*R).  Approximately 10Wh = 1km, and 1km = .6 miles if you're used to miles, with my (10*3.7*5 = 185) 185Wh battery 18.5km or about 11-12 miles.

---

A couple down sides with higher voltage just to balance this post out a bit :)

The higher voltage means you are getting higher top end which may be good or may be too much (12S felt like too much to me so I ended up at 10S after destroying the original batteries by accident over time).  Another thing is the VESC has an upper RPM limit (at least on the ones before the VESC 6 that one is new and I'm not so sure about yet) but if you have a high kv motor and 12S you could get above the 60,000erpm limit (8000ish regular RPM) and can fry the DRV chip on the VESC so make sure you either limit the eRPM or post your build plans to let others chime in if they know it will cause issues.

Also going at a higher top speed means that you're more likely to drain power more quickly (more wind drag more friction from parts moving against each other at a high speed and building up more heat, generally leading to more friction), but the gain in electrical efficiency through all the components before electrical power is converted into kinetic energy will generally more than offset these changes.
```

---
## \#11 Posted by: spearsgary74 Posted at: 2017-10-14T04:54:23.912Z Reads: 331

```
Check out the RC industry's solution to this question. Then use your imagination when designing your setup. With quick connects https://www.motionrc.com/pages/connectors-and-adapters. As well as an easy to open and close battery compartment you can extend range greatly while keeping the carrying weight down.
```

---
## \#12 Posted by: Kmanna Posted at: 2019-02-19T20:12:33.246Z Reads: 117

```
How much power of a battery for a mountain board with 8 inch wheels? 22000mah 20c would be fine?
```

---
## \#13 Posted by: draj2001 Posted at: 2019-07-01T03:04:17.241Z Reads: 79

```
Hey guys, quick question. I recently built an e-board with 2 batteries in series and just started riding it around since I have finished it. Sadly though, one of the batteries died out since I had been running it for a while to test it out. The problem is, the batteries are kind of expensive and I looked around for the one I used which was the ZIPPY Compact 5800mAh 5S 25C  18.5V Lipo Pack With XT90. The only problem is that this specific type seems to be discontinued. So I started to explore other options and found a 6S 25C 5800mAh 22.2V Lipo Pack from the same company. But I've read that there are risks of using different voltages, even in series, and different aged batteries. My biggest question is if the discharge and capacity is the same, then it shouldn't be much of a problem wiring the two in a series even if the voltages are differnet since they add up right?
```

---
## \#14 Posted by: Andy87 Posted at: 2019-07-01T05:46:22.846Z Reads: 70

```
depending on how old your ZIPPY pack is, it´s very likely that the internal resistance of the cells are different from the new pack you want to add.
this means that the old pack hold less capacity and the cells discharge faster what can result in an overdischarge of the older pack/cells while riding.
```

---
## \#15 Posted by: draj2001 Posted at: 2019-07-01T14:44:27.086Z Reads: 58

```
That's annoying. I have only used it for one cycle so far so I don't know how much that would increase the internal resistance, I'll look into it later. But since the discharge is the main concern that's good news cause it won't be hazardous since recharge is where the risk of fire is. So if I were to go with the ZIPPY 6S 5.8A 22.2V 25C battery, then it shouldn't limit by capacity and should give me more power due to the increased voltage but the main risk is wearing down the older battery right? Do you know if I can configure my VESC to prevent this?
```

---
## \#16 Posted by: TheEngineeredLife Posted at: 2019-10-15T21:29:46.435Z Reads: 28

```
What battery type/range would I want to choose for a short range but high torque and speed direct drive hub motor? I only want to use the electric part of the skateboard when I'm going up hills.
```

---
