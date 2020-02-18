# A true BMS - does it exists, should it be designed?

### Replies: 36 Views: 2827

## \#1 Posted by: tomtom13 Posted at: 2017-04-09T01:08:43.929Z Reads: 253

```
Hi,

I've been wrestling with an idea of actually building my own electric long board (not many drop decks around there and I like that sort of board flex points arrangements).

But (of course I might be blind, to not see those) it became apparent to me that most of people concentrate a lot on motor controllers and actual motors but there is very little improvement in terms of BMS.

So from my experience a BMS will be responsible for:
- energy counting coming in and out of battery to have a full knowledge of current SOC,
- continuous monitoring of each cell voltage
- continuous measurement of cell temperature 
- provoding balancing durring charging 
- imposing a drive and regen current for motor controllers based on SOC, cell min / max voltage and temperature.
- dictating charge current for charger connected to battery pack 

Common practice is to blend BMS with distribution unit, distribution unit is usually responsible for:
- measuring current coming in and out of battery pack
- comparing current current against BMS imposed limits and if those are exceeded perform a controlled shutdown (bus isolation)

Another problem that I've seen is that any isolation units that exists (or distribution units) are fairly limited in max current. I was considering a build with 10S running at 200A drive and 100A regen and as far as I can tell I'm on my own. 

Please correct me if unit like that does exists, and please don't try to deteriorate this topic for no reason. 

I've also noticed that there is fair amount of people that do complain about their range and other aspects that do indicate that they smash their battery because some cells have different impedance to others (heat spots can cause that as well). Decent 18650 will give you 5000 cycles for capacity drop of 20% if used within current / voltage / temp limits. From our tests of batteries you can kill bests cells quicker than 20 cycles (drop them more than 50% of capacity), without even touching region of thermal run away. Also there seems to be not much concern about batteries going for runaway among some users ... and scary is that they chose polymers that we know that those can go with decent fireball. 

Now recently I was doing a small design work that included a set on nice mosfets that can do 43 amps and provide current measurement within single package and small footprint (and verrrryyyyy low ON resistance resulting in low loss).

So my intention was to actually create a BMS that allows all mentioned functionality. Now if using a right chip, there could be additional functionality include: 
- providing it with 4 can busses it could be connected to 4 separate VESC motor and dictating current limit PER wheel.
- reading realtime wheel speed from each vesc separately
- dictating torque request independently to each wheel
- implementing a speed control where a central unit is reading wheel speeds and computing whenever we are in turn or not and altering torque based on those parameters. 
- implementing a simple 4 wheel control with drive and regen torque bias, still not exceeding base battery limits. 
- if one would be veeerrrryyy advantageous, by controlling each wheel separately there is a way to implement stability program that would allow driving a softer suspension setup downhill, and having motors eliminate potential of tail oscillation. 

FYI, I don't fancy changing it into any form of business and would prefer for it to be open source so more people can benefit (I like the vesc initiative !)
```

---
## \#2 Posted by: Pantologist Posted at: 2017-04-09T03:27:56.125Z Reads: 223

```
Have you checked these BMS designs from members of this community? I am pretty sure they offer most of this features. Just to let you know they exist. 

[Batman BMS](https://www.electric-skateboard.builders/t/raphael-chang-bms-and-esc/8952/13?u=pantologist)

[DieBie BMS](https://www.electric-skateboard.builders/t/diy-6s-to-12s-bms-with-can/2639?u=pantologist)
```

---
## \#3 Posted by: Okami Posted at: 2017-04-09T03:50:51.132Z Reads: 223

```
Im definately up for more ''open source'' / customizeable bms designs out there!

Raphael Chang's one seems to be promising.. but the work developing these seems a bit slow and im not sure when we will see them more openly available to everyone.. so as i said earlier, the more options we have, the better!

--

The idea about individually controllable wheels also sound nice.. Though for start a bms which can do some ''coulometer'' functions and display energy spent/received would be nice itself
```

---
## \#4 Posted by: Pantologist Posted at: 2017-04-09T04:11:23.380Z Reads: 199

```
[quote="Okami, post:3, topic:20647"]
The idea about individually controllable wheels also sound nice.. Though for start a bms which can do some ''coulometer'' functions and display energy spent/received would be nice itself
[/quote]

That is one of the easier functions and most of these smart bmses can do that. 

DieBie is not being manufactured by a company, you have to use the open source files and print and assemble it yourself. 

BatMan is in a beta production run right now.
```

---
## \#5 Posted by: Stef Posted at: 2017-04-09T06:16:02.092Z Reads: 174

```
How about combining the functionality of a soft switch, (smart)BMS and VESC on one PCB with shared heatsink?

Ideally being able to configure all functionality through one piece of software through bluetooth...
```

---
## \#6 Posted by: smurf Posted at: 2017-04-09T06:26:42.215Z Reads: 173

```
Take a look at this BMS

http://www.chargery.com/BMS16.asp
```

---
## \#7 Posted by: tomtom13 Posted at: 2017-04-09T10:58:32.017Z Reads: 163

```
[quote="Pantologist, post:2, topic:20647, full:true"]
Batman BMS

DieBie BMS
[/quote]
Thanks a lot for that, I seen not only me seen the problem :slight_smile:

[quote="Pantologist, post:4, topic:20647"]
That is one of the easier functions and most of these smart bmses can do that.
[/quote]
From my experience coulometer is the worst possible solution - When we passed our daily battery data through coulometer we got SOC drift of 35% ... unfortunately more complex computation of energy flow is required (and a rough value of internal impedance of cells has to be known)

I'm not saying that they don't do it - just bringing up that coulometers are very unreliable in real world. 

[quote="Stef, post:5, topic:20647"]
How about combining the functionality of a soft switch, (smart)BMS and VESC on one PCB with shared heatsink?
[/quote]

So in 4x4 skatebords one would have 4 bms units ? who provides ESP then ?
I see possibility of having 4x50A continous BMS units with isolation units that somehow synchronise, which will simplify design by not having to use large components for 200A, BUT then one will be hit with 4 x single bms cost + 4 x failure modes + you still need master unit .... design would be messy here UNLESS you have some brilliant idea (not the first time I've not seen obvious and simple solutions so go for it!)

[quote="smurf, post:6, topic:20647, full:true"]
http://www.chargery.com/BMS16.asp
[/quote]
I'm not sure, but stuff that I've seen on this link is far from being "skateboard ready" .... could you please elaborate how you see use of their stuff here ? 


So far I see that 100A continuous is max so far.
Mostly a single CAN buss ... just to make people realise the problems with esp : good abs has separate inputs from each wheel ( analog so there is no problems with max bandwidth ) and if you've looking for active suspensions - most manufacturers use FlexRay - which gives 100x the bandwidth of CAN ... 

(and I know how some will approach it "it's a overkill" "you're nuts" etc ... but I would rather implement eps the right way, because it's not a car with a lot of body panels around you and a tinny error means that your face becomes a crump zone :/ )

Thanks to everyone for their input and not taking down the thread with usual "why would you numbty" or "use search". Cheers guys !
```

---
## \#8 Posted by: Stef Posted at: 2017-04-09T18:09:50.396Z Reads: 140

```
[quote="tomtom13, post:7, topic:20647"]
So in 4x4 skatebords one would have 4 bms units ? who provides ESP then ?I see possibility of having 4x50A continous BMS units with isolation units that somehow synchronise, which will simplify design by not having to use large components for 200A, BUT then one will be hit with 4 x single bms cost + 4 x failure modes + you still need master unit .... design would be messy here UNLESS you have some brilliant idea (not the first time I've not seen obvious and simple solutions so go for it!)
[/quote]

Less than 3% of builds on this forum are 4WD, in that case it wouldnt be practical indeed.

I dont think ESP should be applied through the BMS, but through the motor controllers. CAN-bus connected vescs can already apply traction control, so ESP is only a bit of coding away.

Design would be much less messy with integrated BMS+softswitch+VESC on a single PCB as it becomes one big plug and play device. Plug in your switch, receiver, batteries, balance leads, motor leads and sensor leads, done! Then connect through bluetooth to set all parameters in one PC app.

On dual drive builds you will have one BMS too many, though you could also make a version with dual vesc + bms +switch. 

Im not going to try designing this, but i'm just sharing what I would want to buy as a perfect electronics solution.
```

---
## \#9 Posted by: JTAG Posted at: 2017-04-09T19:48:05.743Z Reads: 125

```
Why on earth would you like 10*3.7*200=7.4KW passing trough a BMS? You should really considder external means of current measurement (hall based) for these powers. My BMS can do up to 120A discharge but that is really maxing it.

Why would you need 4 times a CAN bus? Do you know how a CAN bus works :stuck_out_tongue:?

ESP sounds coowl but I think its to complex for esk8 application.....
```

---
## \#11 Posted by: tomtom13 Posted at: 2017-04-09T20:38:17.297Z Reads: 118

```
@Stef only 3% ? that's a pitty ... but I guess people don't want to spend to much on their eskate hobby. "Oh well".

Anyway in terms of ESP, I strongly disagree with it being implemented by motor controller (at least in current shape of vesc) to do this you need to shift a lot of data on CAN (2 might be OK but 4 on same buss will be to slow). Also for esp or any decent traction control you need at least a most crude yawn sensing ... even ESR does use gyro. Another thing is a processing power ... current STM32 that is used on vesc is a nice bit of kit but I would not go below 300MHz for any meaningful computing - specially that vecs is pretty busy with phase control and sensing! 


For a late joiner @JTAG
I think you are slightly wrong with your assumptions.

First of all 3.7V is a static nominal (100% saged) voltage for kobalt cells, when heavy loaded those will drop to 3V easily - so it's actually 6kW. If we are talking about polimer cells this voltages will go down under load even more :* climbing over a 25% will give you rather amazing power drain

Second, hall sensors are cheap and crap and nobody in automotive that cares about their name uses it :) Using transistors of a soft switch for current measurement is not by any means perfect but it does simplify design, reduces bom, and provides a better measurement than hal effect :) 
[and before you will go into proving me that some people do, most of controllers for EV that used hal is DEAD because on high noise buses it's just not functioning properly - and nobody in motor controller business is looking and stoping using batteries as noise dump]

Third - no, I did not know how CAN works up until now, I always assumed that you can put infinite amount of nodes, with infinite bandwidth, no noise caused "tripple message cascade" problems (error -> error frame -> resend) 
(that is single handedly cause a rule of thumb not to create systems with bus content of more that 30%). I just design vehicles using kw2000 over VPW ... you know to show that I'm "a pro"

Fourth - sorry for throwing out my toys out of pram :P anyway point of 4 CANs was to create any meaningful esp, for simple max current propagation one CAN is more than enough 

Fifth - your bms is something I would go for with RWD setup where no other means (like esp) are neaded :) 



But I see that there is more emerging problem for eskate people - a increasing complexity that leads to harder setup and has more failure points. 

Anyway anybody could ask a creator of vesc this two simple questions
- how is he coping with switching noise on his system - what if 2 (or even 4) controllers would occupy same PCB
- what is a max cable length for 3 phase between controller and motor ?

maybe there would be a way to kill multiple birds with one stone and get everything merged into a singular design (that way heat rejection would be less of a problem, less cabling ... as @Stef points out a easier setup.
```

---
## \#12 Posted by: JTAG Posted at: 2017-04-09T21:07:27.993Z Reads: 99

```
Dajum, didn't expect this for a reply. Your type of arrogance makes me feel sick, goodbye :sunglasses: .
```

---
## \#13 Posted by: Okami Posted at: 2017-04-09T21:09:33.593Z Reads: 104

```
Hi! Im seeing a wide list of topics adressed here in one reply @tomtom13 
So im really starting to wonder from which ''industry'' are u coming and how many years of experience you are having into it ;)

Non the less, I found 2 topics of interest from what you pointed out: 

[quote="tomtom13, post:11, topic:20647"]
second, hall sensors are cheap and crap and nobody in automotive that cares about their name uses it :slight_smile: Using transistors of a soft switch for current measurement is not by any means perfect but it does simplify design, reduces bom, and provides a better measurement than hal effect :slight_smile:
[/quote]

Can you describe this more precisely. How exactly transistors are used for measurement? To my understanding this means that the process you describe is what Vesc does.. measurent shunt current etc... but then again, if you use sensored setup, the halls are still in the magnets.. so this part is a bit unclear to me..

[quote="tomtom13, post:11, topic:20647"]
First of all 3.7V is a static nominal (100% saged) voltage for kobalt cells, when heavy loaded those will drop to 3V easily - so it's actually 6kW. If we are talking about polimer cells this voltages will go down under load even more :* climbing over a 25% will give you rather amazing power drain
[/quote]

Why do you say that polimer cells 'sag' even more heavy under load?

I always though that li-ions are the ones which sag, while lipo cells maintain higher output.

Accounting for voltage drop and power decrease seems smart, im sure not everyone is accounting for this.
```

---
## \#14 Posted by: tomtom13 Posted at: 2017-04-09T21:11:47.014Z Reads: 91

```
Sorry for offending you ( I did said sorry for throwing my toys out of pram :* ) but I guess if that is so easy for you to get offended than you will be not willing to change your desing. FYI I definitely don't see that as a negative trait!
```

---
## \#15 Posted by: tomtom13 Posted at: 2017-04-09T21:54:09.831Z Reads: 88

```
Hall efect sensors don't limit to measuring magnetic field in motor / or "noticing a passing magnet". There were at some point measuring systems (not invasive) that would measure a current by having a coil winded over a wire in which you were measuring current (like current clamp meter - just cheaper) their accuracy was god awful when used in EV because motor controller produces a lot of noise and it will _always_ produce way off measurement. 

using a trnsistor - mosfet in ON position has a fairly linear Rdson, lets say 16mOHM. When you pass current through transistor it will give you a voltage drop - you measure this voltage drop and apply a simple formula: V/R = I. So if you had a 16mV drop on your transistor with 16mOHM Rdson - than current between drain and source will be 1A. 

There are transistors that have this measurment units build into them ! Case point:
VN5T016AHTR-E
http://www.st.com/content/ccc/resource/technical/document/datasheet/f9/c7/ff/ce/de/e0/43/ab/DM00064519.pdf/files/DM00064519.pdf/jcr:content/translations/en.DM00064519.pdf

so why complicate ? sink sense output through resistor to ground and connect high side of resistor to ADC of you choice and you've got a very accurate current measurement for a penny (yes you can do it even better but for eskare down to 0.01A is enough !)


Polimers are a slightly different beast to what people think of them. Reason people use polimers are price / weight / power to energy ratio. Polimers also have a different chemistry to usual kobalt 18650, so for like to like test (discharging both chemistries with 1C) polimers will sag far less than kobalt. Now as we know reality of polimer cell is that they always quote astounding C discharge rating - 165C was highest that I've seen but it still means that 6000mah battery will discharge with roughly 900A within 20 seconds. Battery will survive that without significant degradation or going into thermal run away so everybody is happy, but what nobody actually measures is that cell voltage at this discharge rate can drop down to 0.5V. So yes you've got a brilliant current but not as much power output that you've expected. 

So bottom line is that when reaching a genuine max C discharge rating of cell, kobalt cells because those are not rated to cosmic levels will always give higher load voltage than polimers. 

If you want to get a decent source of current measurements under load for 18650:
http://lygte-info.dk/review/batteries2012/Common18650Summary%20UK.html

here for example is a briliant sonny cell ( on of the best )
http://lygte-info.dk/review/batteries2012/Sony%20US18650VTC5A%202600mAh%20(Green)%20UK.html

Cell was fully loaded and taken _STRAIGHT_ off the charger (no time to sag to nominal standby) and you can see that straight of the bat within first minute battery is at 3.3V at discharge of 30A ... then it collapses down to 2.8 which bloke uses as a cut of point for kobalt cells (vise)
```

---
## \#16 Posted by: tomtom13 Posted at: 2017-04-09T22:16:52.357Z Reads: 82

```
@Okami (just a supplementary stuff, didn't wanted to edit previous one .... it had only so many edits)

What you have to think of as well is that if you load cell:
- with 20A (for lets say 3.7V cell) you have to provide 0.185 ohm resistance on output. 
- with 200A (for lets say 3.7V cell) you have to provide 0.0185 ohm resistance on output.

If internal resistance of the cell is arround 0.02, a 20A load does mean that internal resistance is that significant - but when internal resistance makes up a _half_ of total loop resistance that your voltage will sag dramatically !!!

This is why I was keen on separate cell voltage measuring and adjusting a max discharge current (and letting motor controllers know) so voltages don't drop to low. People are not aware of that but kobalt cells if depleted to low will dramatically decrease life span. Of course polimer "calendar" cells require compression so they don't swell ... so each chemistry / design has it's downsides !
```

---
## \#17 Posted by: Okami Posted at: 2017-04-09T22:17:52.116Z Reads: 80

```
Thanks for all the great info!
@tomtom13

Basically, do you refer to 'coulometers'  as 'devices'' which exlusively use hall sensors?

When I pointed out to BMS with coulometer integrated, I meant more that it has current sensing integrated, has some form of a display / data output and that it replaces the need to install 'exterior' current sensors / power meters, for analyzing / measuring or displaying data.

Im not so sure is this super needed as there might as well be 'ready-made' modules for this reason but I still think it might be nice, if you could see all the energy / battery related data using bms itself. 

----

I will get to 'battery topic' asap, as I saw you made a new reply and im still pondering the idea on why do you refer to 'cobalt' 18650 as the battery type - chemistry, which 'handles' load better.

it still seems to be that lipos 'can bear' higher load / energy output than 'cobalt' li-ions.
For example.. the same vtc 5 cell can bear a current of about 10C (2.6 ah x 10C = 26 A )

While some lipo's can go to the ''sky-limit'' you mentioned.. even over 100c per cell.. it does seem logical that voltage will drop dramatically.. but does it mean that in some way VTC 5 cells can output higher watts? 

**In reference to what are you then comparing 18650 li-ion vs lipo packs?**

Typically, it seems like vtc5 can output about = ~93.6W per cell (3.6v nominal x 26A) or about 108w max (30A).

In which case.. lipo pack, if outputting 25c..of let's say 3ah capacity.. will output way more..maybe the size will be bigger.. so **maybe you refer to the energy density per volume here ..**
```

---
## \#18 Posted by: tomtom13 Posted at: 2017-04-09T22:23:25.429Z Reads: 79

```
[quote="Okami, post:17, topic:20647"]
coulometers
[/quote]


I would assume that coulometer here is a "culomb meter" which only measures current IN / OUT of battery. Now if you look at physics of battery - if you charge it with 50A you actually put more energy into the battery than if you would discharge battery with 50A and it's all to do with voltage sag / increase. Some folks like to think of battery as a current storage (you know a magical Ah marking) but in reality those are a chemical energy storage ... so you need to measure how much energy you put IN (amps * volts) and how much you take out ( amps * volts ) and on top of that you need to account for cell internal resistance that will always convert current into heat (energy heat loss). So if you discharged 100W and charged 100 you may still end up with battery slightly less charged because you lost some energy to heat through internal cell resistance.

as I stated before we did that for fun on one BMS and we got 35% drift over a course of day of vehicle driving. It was even more funny when BMS opened contractors on our test guy in the middle of the motorway because cell voltage got to low while thinking it was 35% :))))))
```

---
## \#19 Posted by: tomtom13 Posted at: 2017-04-09T22:29:23.339Z Reads: 79

```
@Okami 
Maybe you understood me wrong:

[quote="tomtom13, post:15, topic:20647"]
Polimers also have a different chemistry to usual kobalt 18650, so for like to like test (discharging both chemistries with 1C) polimers will sag far less than kobalt
[/quote]

polimers handle discharge far better than cobalt. BUT they are rated to insane ratings at which they actually sag far more than cobalt cells at their max rating. So lipo at max current of 300A will sag more than 18650 at max current of 15A. Still lipo handles discharge better (due to mainly lower internal resistance). Still people strust max rating as a golden bullet for having a nominal voltage.
```

---
## \#20 Posted by: Okami Posted at: 2017-04-09T22:29:30.305Z Reads: 85

```
[quote="tomtom13, post:16, topic:20647"]
People are not aware of that but kobalt cells if depleted to low will dramatically decrease life span.
[/quote]

So which 'amplitude'' of battery voltage do you recommend to use?

I've seen this chart, I think this is somewhat smart on how to prolong battery lifetime/runtime in the long run.

<img src="/uploads/db1493/original/3X/c/9/c9cc55bef81e241e1feedb1dc0deae8eba6ac36e.jpg" width="570" height="195">

---

[quote="tomtom13, post:19, topic:20647"]
polimers handle discharge far better than cobalt. BUT they are rated to insane ratings at which they actually sag far more than cobalt cells at their max rating. So lipo at max current of 300A will sag more than 18650 at max current of 15A. Still lipo handles discharge better (due to mainly lower internal resistance). Still people strust max rating as a golden bullet for having a nominal voltage.
[/quote]

Ah okay, then I can agree.. yes I somehow thought you want to tell me that li-ions sag less than lipos.. even if lipos are capable of way higher discharge rate.

I think if you read around, smarter people on this forum have already pinpointed out this 'fact' to downrate lipo batteries.. and refer to C rating as maximum possible (sometimes maybe for short amount of time)

--

This is the ''coulometer'' to which im referring to and which would be cool, if it could be integrated into the bms circuit already:

http://www.ebay.com/itm/Battery-Capacity-Tester-Indicator-Coulometer-Lithium-Lead-Acid-8-65V-150A-BI668-/232282362560?hash=item36151b92c0:g:tw8AAOSwSlBY1ek8

http://www.ebay.com/itm/35-80V-50A-Capacity-Tester-Indicator-Coulometer-Lithium-Lead-Acid-Battery-Meter-/272018674496?hash=item3f55939340:g:~6IAAOSwYHxWH3Zg

--

Maybe code could be open, so that users could make their own data output displays,, in a way they wish to see the info.

Basically, it has a shunt / current sensor to measure passing through current and some microprocessor drivign everything and of course measurement of voltage.. then after the mcu has calculated all data, it gets output to lcd.
```

---
## \#21 Posted by: tomtom13 Posted at: 2017-04-09T22:43:00.818Z Reads: 76

```
That graph is not that much wrong, Tesla was giving you 30 - 40% more capacity so after a 5 years you would still enjoy the same range. 

So if you allow batteries to be drained at full "quoted by manufacturer" current (cobalts of course)
- at 2.9V you start decreasing their life by 20%
- at 2.8V you start decreasing their life by 30%
- at 2.7V you start decreasing their life by 50%
- anything below 2.7 and you are effectively asking for it. 

You know, some of 18650 are rated to 80% capacity loss over 10000 cycles (f*** expensive) but when those loose capacity they will increase internal resistance -> voltage sags further -> you create more cristals in side of battery -> magic circle. so if you plan to ride you eskate only 300 times whach them down to 2.7V but be warned that battery might melt underneath you.

I'll explain it from my perspective: I'll got for a run on my long board -> come back -> toss it to a boot of my car. If battery is at the point of thermal runaway I will loose my car and I surely love more my beaten up old 3 series more than a long board. So i would prefer to build more expensive BUT safe eskate. That's why safety matters to me. Personally @jtag bms looks promising but this need investigating (I seriously don't fancy redesigning a wheel)
```

---
## \#22 Posted by: tomtom13 Posted at: 2017-04-09T23:11:34.186Z Reads: 73

```
I see your culometers ... I would personally advice against using china stuff, but if there is nothing else available or price difference is of an order of magnitude .... than I understand the motive. 

Now, how much you care about this garbage on the screen ???? I mean if you have a precise measurmen of true energy in the battery than silly LED digit display is enough (like that one)
https://www.google.co.uk/search?q=digit+segment+display&client=safari&rls=en&source=lnms&tbm=isch&sa=X&ved=0ahUKEwi7vJelv5jTAhXoKMAKHWKFAR0Q_AUICCgB&biw=1920&bih=1112#imgrc=gmqKAojLHRKcsM:

I means what else you need ??? if ti's charged it's 100% if it's balancing it's not 100%, if you are at 10% you have 10% energy = range left ...
```

---
## \#23 Posted by: Okami Posted at: 2017-04-09T23:15:50.120Z Reads: 72

```
Well, I still like to see the wattage / amps.

Also, percentage is not always enough.. I hate to do the calculation in my mind each time, knowing that 10% maybe corresponds to 2.7km for example. (if max range is 27km)

Plus, voltage drifts, so for precise reading you always need to let the voltage to rest a bit to return to steady state.

--

With ''coulometer'' - Wh / Ah shown, I know that my battery is 400wh total, for example, then I see 50wh consumed and I know I still got 350wh to go.. 

With percentage there is no way to accurately measure this as the energy use might change.

--

Basically, with smart enough bms / coulometer, a ''precise'' tool for range estimation could be created..

If riding at steady speed consumes 300w, then it would calculate the max range based on capacity left in the battery.. **now tell me, how can i achieve the same with percentage display?**
```

---
## \#24 Posted by: tomtom13 Posted at: 2017-04-09T23:22:02.829Z Reads: 69

```
Well actually if you have a BMS with a precise measurement and true energy calculation you don't have to wait for voltage to settle ... problems you describe are from devices that are crap (or have a crap firmware). 

As a comparison, some folks produced a pretty awesome calibration for us and over a long drive test when we used a range extender and consumed total of 350KWh, SOC reading was off by less than a 0.7kW (tested by charging pack to max and balancing it).

So if firmware is done properly and none of measuring devices are bad - a SOC reading should be more than enough.


ahhhhh the old "range" question .... well your range depends on how you drive, drag, how fat you are, incline, driving style  ... so it's never the same ... but I can precisely tell you how much real energy you've got in a pack ... over time you will automatically know - 10% get's me that far ...

still voltages, watages etc are redundant in my opinion.
```

---
## \#25 Posted by: tomtom13 Posted at: 2017-04-09T23:32:48.082Z Reads: 70

```
Ok, this would be an overkill but there is a way of doing range based on "last X miles driven" so what you do is look at how much power you used per mile (km) in last 1000 miles (km) and you build a profile out of that ... considering how much energy you've got left in pack it becomes academic ... but you need to know wheel size, rpm etc.
```

---
## \#26 Posted by: IsTalo Posted at: 2017-04-09T23:44:37.299Z Reads: 68

```
They are nice, but very difficult, it uses a lot of small pieces to solder and need a lot of experience on programming
```

---
## \#27 Posted by: tomtom13 Posted at: 2017-04-09T23:47:22.162Z Reads: 65

```
[quote="IsTalo, post:26, topic:20647, full:true"]
They are nice, but very difficult, it uses a lot of small pieces to solder and need a lot of experience on programming
[/quote]

I would assume that those come in pre assembled and provider uses a pick a place machine ... right ?
```

---
## \#28 Posted by: IsTalo Posted at: 2017-04-09T23:50:49.819Z Reads: 58

```
Right, but I mean, make one at home, I couldn't do it without contacting a factory of pcbs! And I (and a lot of people) don't have that programming skills, I just know Arduino Code!
```

---
## \#29 Posted by: Stef Posted at: 2017-04-09T23:52:15.976Z Reads: 65

```
[quote="tomtom13, post:11, topic:20647"]
only 3% ? that's a pitty ... but I guess people don't want to spend to much on their eskate hobby. "Oh well".

Anyway in terms of ESP, I strongly disagree with it being implemented by motor controller (at least in current shape of vesc) to do this you need to shift a lot of data on CAN (2 might be OK but 4 on same buss will be to slow). Also for esp or any decent traction control you need at least a most crude yawn sensing ... even ESR does use gyro. Another thing is a processing power ... current STM32 that is used on vesc is a nice bit of kit but I would not go below 300MHz for any meaningful computing - specially that vecs is pretty busy with phase control and sensing!
[/quote]

Good luck with your project, it seems you definitely dont need our input, looking forward to seeing the results.
```

---
## \#30 Posted by: tomtom13 Posted at: 2017-04-10T00:04:09.646Z Reads: 64

```
Let me get this straight - those bms come not populated ? 

Also why you worry ? once somebody writes a code you can replicate it without a hassle :) Also if you use arduino studio you already write code in C .... that's a lot more than some of self proclaiming software engineers that I've seen in my time :D
```

---
## \#31 Posted by: IsTalo Posted at: 2017-04-10T00:11:08.777Z Reads: 64

```
Populated you mean assembled? If yes, the answer is no, it will come assembled. But I think they don't have producing date

Yeah, Is easy copy the code, but both projects don't shows the code, so we're blind 

I would love to make my owm Bms (Also because mine don't arrived, Brazil isn't a good place to buy things on Ebay) but there are somethings that is better buy manufactured, like the lipo packs, it is cheaper to make one with 18650 cells but it is harder! I will buy a Imax b6 this week, but want to buy other Bms on the future, because my power supply arrived (Man, really, don't mind living in Brazil and building e-boards)
```

---
## \#32 Posted by: tomtom13 Posted at: 2017-04-10T00:18:26.575Z Reads: 58

```
Well @Stef I did take on board your input about overtly complex designs in eskate world, and it there are things that can be done with that to make end user life easier ... also it's not my "project" it's a general thread on what's there and how stuff can be done / improved .... might be a need to design something / implement it ...
```

---
## \#33 Posted by: tomtom13 Posted at: 2017-04-10T00:22:08.305Z Reads: 53

```
Wow, Ok ... look at least you know that they will emerge at some point ... also you choose a right attitude - don't complain where you live just get on with it ! Keep it up !
```

---
## \#34 Posted by: IsTalo Posted at: 2017-04-10T00:29:48.806Z Reads: 55

```
I didn't want to be anti-patriotic, but it is just the truth
```

---
## \#35 Posted by: tomtom13 Posted at: 2017-04-10T00:31:05.797Z Reads: 55

```
That's cool !
```

---
## \#36 Posted by: PXSS Posted at: 2017-04-10T03:39:14.642Z Reads: 60

```
Eeek so much arrogance it hurts...
A little piece of advice, humbleness takes you a long way in life and with people.

[quote="tomtom13, post:7, topic:20647"]
From my experience coulometer is the worst possible solution - When we passed our daily battery data through coulometer we got SOC drift of 35% ... unfortunately more complex computation of energy flow is required

I'm not saying that they don't do it - just bringing up that coulometers are very unreliable in real world.
[/quote]

Then you're using it wrong. I get SOC within 3% by simply using coulometer data in real world scenarios.

[quote="tomtom13, post:15, topic:20647"]
Polimers also have a different chemistry to usual kobalt 18650
[/quote]

Wrong, the difference is in packaging not chemistry, and it is spelled Cobalt.

[quote="tomtom13, post:15, topic:20647"]
Now as we know reality of polimer cell is that they always quote astounding C discharge rating - 165C was highest that I've seen but it still means that 6000mah battery will discharge with roughly 900A within 20 seconds. Battery will survive that without significant degradation or going into thermal run away so everybody is happy, but what nobody actually measures is that cell voltage at this discharge rate can drop down to 0.5V. So yes you've got a brilliant current but not as much power output that you've expected.
[/quote]

Reputable Lipo makers do take this into account. A Lipo is not meant to ever be under 3V. I have run several LiPos at full 60C and they never dropped below 3.2V/cell although they do not discharge 100% capacity, they normally do 85-90% which is expected, given losses due to heat etc.

[quote="tomtom13, post:16, topic:20647"]
If internal resistance of the cell is arround 0.02, a 20A load does mean that internal resistance is that significant - but when internal resistance makes up a half of total loop resistance that your voltage will sag dramatically !!!
[/quote]

If your Lipo internal resistance is that high then you should replace it.

[quote="tomtom13, post:16, topic:20647"]
People are not aware of that but kobalt cells if depleted to low will dramatically decrease life span.
[/quote]

And the same thing doesn't happen with LiPos... right.

[quote="tomtom13, post:18, topic:20647"]
if you charge it with 50A you actually put more energy into the battery than if you would discharge battery with 50A and it's all to do with voltage sag / increase
[/quote]

If you discharge a cell from full to empty at 50A, and then charge that same cell from empty to full at 50A you will get mighty close results... The difference is that the reaction is slightly endothermic during discharge and exothermic during charge. The voltage sag/rise almost cancel each other out.

[quote="tomtom13, post:21, topic:20647"]
So if you allow batteries to be drained at full "quoted by manufacturer" current (cobalts of course)- at 2.9V you start decreasing their life by 20%- at 2.8V you start decreasing their life by 30%- at 2.7V you start decreasing their life by 50%- anything below 2.7 and you are effectively asking for it. 

You know, some of 18650 are rated to 80% capacity loss over 10000 cycles (f*** expensive) but when those loose capacity they will increase internal resistance -&gt; voltage sags further -&gt; you create more cristals in side of battery -&gt; magic circle. so if you plan to ride you eskate only 300 times whach them down to 2.7V but be warned that battery might melt underneath you.
[/quote]

Errr. no. just no...
```

---
## \#37 Posted by: tomtom13 Posted at: 2017-04-10T14:59:59.466Z Reads: 57

```
[quote="PXSS, post:36, topic:20647"]
Eeek so much arrogance it hurts...A little piece of advice, humbleness takes you a long way in life and with people.
[/quote]
So when your mate asks me "Do you know how a CAN bus works ?" and then replies with "Your type of arrogance makes me feel sick, goodbye" you don't call him hypocritical for being arrogant and then calling somebody else being arrogant.  

[quote="PXSS, post:36, topic:20647"]
Then you're using it wrong. I get SOC within 3% by simply using coulometer data in real world scenarios.
[/quote]
Can you provide data for that ? because we tested in real world environment and spend ~20k on this test just to eliminate bms that use pure culomb counters out of equation ... 

[quote="PXSS, post:36, topic:20647"]
Wrong, the difference is in packaging not chemistry, and it is spelled Cobalt.
[/quote]
I could change cobalt to kobalt but it nicelly highlights the spelling guild here. And no, you're wrong - 18650 use different substrate to be able to roll those without cracking, calendar cells don't have that requirement so use different substrate to give more power density. Those are part of battery chemistry unfortunately. 

[quote="PXSS, post:36, topic:20647"]
Reputable Lipo makers do take this into account. A Lipo is not meant to ever be under 3V. I have run several LiPos at full 60C and they never dropped below 3.2V/cell although they do not discharge 100% capacity, they normally do 85-90% which is expected, given losses due to heat etc.
[/quote]
Let me put it this way:
Please tell me which 60C max rated cell when discharged at 60C is giving you 3.2V ... I'll plug it into our digatron, I'll even compress it so there is no substrate de-lamination, I'll even drop it to climatic chamber to keep it at perfect temperature (that I'll let YOU chose) and I'll provide you with discharge graph at full 60C and corresponding voltage. Hey I'm dumb and all people that I work with are dumb and we would love to see that battery in action.

[quote="PXSS, post:36, topic:20647"]
If your Lipo internal resistance is that high then you should replace it.
[/quote]
And did I say anywhere in that post that I'm talking about lipo ?

[quote="PXSS, post:36, topic:20647"]
And the same thing doesn't happen with LiPos... right.
[/quote]
So you are telling me that you've done accelerated life cycle test of a 18650 and lipo over a 5000 cycles and you found different data than a whole industry dealing with batteries and spending billions on it - is just wrong ??? 

[quote="PXSS, post:36, topic:20647"]
If you discharge a cell from full to empty at 50A, and then charge that same cell from empty to full at 50A you will get mighty close results... The difference is that the reaction is slightly **endothermic** during discharge and exothermic during charge. The voltage sag/rise almost cancel each other out.
[/quote]
endothermic batteries ? you want to tell me that you've got battery that converts (any significant) heat energy into electricity ? that actually cools down while discharging ??????

[quote="PXSS, post:36, topic:20647"]
Errr. no. just no...
[/quote]

soooooo this 2 packs of 18650 that we've killed for reference data with that test are imaginary ? 
<img src="/uploads/db1493/original/3X/8/7/87322f381e762f6c8c25cd1079cb004d715ec89b.jpg" width="666" height="500">

This cylidricals that we've killed for undisclosed_super_car_manufacturer are imaginary ?
<img src="/uploads/db1493/original/3X/e/7/e7f5442afa22cc0244f3f185408c7930d3639ee2.jpg" width="375" height="500">

So far I'm trying to provide data to users that was achieved through lots of resources and time put into testing - not a hobby equipment with multimeter, if you don't find it useful that you get this without signing NDA - maybe this thread is not for you. Also if you don't have anything to bring into this thread in terms of answering my bms questions - thanks for participating and don't point into arrogance if you intend to be arrogant your self. 

And don't throw users under the bus with statements that stressing batteries under a certain voltage does not decrease their life span - it's plain malice.
```

---
