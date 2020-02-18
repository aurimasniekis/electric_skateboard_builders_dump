# How many batteries do i need?

### Replies: 11 Views: 3378

## \#1 Posted by: Zimbombe Posted at: 2017-07-16T15:04:34.603Z Reads: 248

```
At first of all i have to apologize if there are any threads where to ask this kind of Questions, i couldn´t find it.

Am i correct by ordering 18 x Samsung INR18650-30Q 3000mAh - 15A ?
Also how much max Discharge would this pack have ? 90A ?
And my last question would be do i need these BMS Things ? what do they do and would this one do the job ?

https://www.banggood.com/PCB-BMS-6S-15A-24V-Battery-Protection-Board-For-18650-Li-ion-Lithium-Battery-Cell-p-1162772.html
( it thems like it outputs only 15A ?! but my motor needs 34A )

I´m building my first electric board (small budget) and have already : 

RACERSTAR 5065
RPM/V: 140KV
Cell Count: 6-12S
 
Tested with 36V voltage:
No load current: 0.6A
No load speed: 5200rpm
Max current: 34A
Max power: 1200W

https://www.banggood.com/Racerstar-5065-BR5065-140KV-6-12S-Brushless-Motor-With-Gear-For-Scooter-p-1110304.html?rmmds=myorder

FVT 120A SENSORLESS ESC

Specification:
 Output:Continuous 120A, burst 640A.
 Input: 2-6S LiPo.  
 BEC:6V/3A . 
. Size:56.5mm* 37.5mm * 36mm.
.Waterproof:Yes
.Supported motor:>5.5T  sensor and sensorless brushless motors.

https://www.banggood.com/FVT-CBWI120A-ESC-Brushless-Speed-Controller-For-110-and-18Series-RC-Cars-Skateboard-ESC-p-985970.html

My Plan is to build a 6s 9A Battery and here comes the question.
I want to build 3 "packs" ,6 cells each.

Thank you guys in addition
```

---
## \#2 Posted by: anorak234 Posted at: 2017-07-16T15:31:36.400Z Reads: 205

```
Please... do some more research. There are plenty of threads answering any questions that you may have on batteries. I'm not trying to be an ass, just trying to make sure everyone can use the proper tools on this forum. Clicking on the search button in the top right corner of your screen is never a bad idea.
```

---
## \#3 Posted by: karma Posted at: 2017-07-16T15:59:50.018Z Reads: 199

```
Like @anorak234 said, do research! You need to learn about how batteries setup affect you're build, like how many in series/parallel. Search around on the forum or visit ebikeschool on youtube, he is a great resource for learning about 18650 cells.
```

---
## \#4 Posted by: Zimbombe Posted at: 2017-07-16T20:14:26.220Z Reads: 192

```
Thx for the help, hope it was worth wasting your time to write this :+1:
```

---
## \#5 Posted by: oyta Posted at: 2017-07-16T21:28:22.173Z Reads: 183

```
There are several threads you can read. Search and you will find. A thread with some basic info and some discussion is this one: http://www.electric-skateboard.builders/t/new-user-looking-for-battery-read-this-complete-walkthrough-of-batteries/26010

😊

Edit: typos
```

---
## \#6 Posted by: wafflejock Posted at: 2017-07-16T21:49:14.108Z Reads: 182

```
You question shows a lack of understanding.  A battery with 6 cells in series and 3 cells in parallel are typically referred to as 6S3P, the 3 parallel you can add the max amperage (ampacity) and the capacity but the voltage is fixed, the 6 in series you add the voltage but don't add the max ampacity or amp hour capacity.

$4 BMS you might as well just light the cells on fire with a lighter :slight_smile:  The battery can be connected directly to the ESC and the BMS can just be used for charging IMO better off buying LiPo packs and a regular charger if you don't know what you're doing yet.  If you are getting or building a custom Li-Ion 18650 based pack then BMS can make sense but don't get the cheapest thing available to manage the charge on your most expensive part.

 140kv is pretty low the 34A is the max, if you had 36V at 34A you have  1224W.  Motor I have is a Turnigy sk3 149kv 6374, max watts 2200 or so.  Likelihood of actually needing to draw that much power is low unless you are accelerating up hill or towing something, but also much better to go with higher voltage and therefore lower amperage to get the same power.  That ESC will work but you are limited to 6S with that so no room to upgrade the battery without buying a new ESC as well (I had a similar one that worked fine for a while when waiting on a VESC, the programming and regenerative braking and room for upgrading made me go with a VESC eventually, been happy with it running between 6S and 12S).
```

---
## \#7 Posted by: Zimbombe Posted at: 2017-07-17T12:24:44.616Z Reads: 152

```
It´s really neat how i´m getting flamed for beeing not "informed" enough. 

Since 2-3 months im checking on a daily basis all kind of threads about new builds, Batteries, Vesc/Esc and  Esk8 compatible Parts. Maybe its because i´m not native speaker maybe not, but some things are difficult to understand for me.

Thats the reason i created a new Thread, hoping to find some Help. Hoping to clear some things up before i can order
my batteries.
And yeah i did research, just minutes before i´ve opened this thread i went through these to give you a small 
collection of what i´ve read.

http://www.electric-skateboard.builders/t/new-user-looking-for-battery-read-this-complete-walkthrough-of-batteries/26010

http://www.electric-skateboard.builders/t/acceptable-diy-6s3p-bms-and-battery-setup/6114

http://www.electric-skateboard.builders/t/how-do-bmss-work/7719?source_topic_id=17645

http://www.electric-skateboard.builders/t/need-help-understanding-batteries/5406

http://www.electric-skateboard.builders/t/how-to-choose-batteries-for-your-project-info-guide/27160

http://www.electric-skateboard.builders/t/what-is-battery-c-rating-is-it-important-for-electric-skateboards/36?source_topic_id=215

FUN FACT in one of these threads i found @karma willingly aswer questions without implying Op to have not read enough .
```

---
## \#8 Posted by: SirDiff Posted at: 2017-07-17T12:48:04.769Z Reads: 111

```
The problem is not about you, that simply don't understand what you've read, but the huge amount of people who want to have everything served without doing any research. It actually looked like you didn't read enough from the first post. I didn't understand what you were saying and it didn't look like you did either (6s 9A battery, you meant 9Ah, 15A discharge, but for a single cell, which means 45 in a 3p, and so on) 
What I can tell you is: you're not ready to assemble a pack by yourself, the battery - motor combination is not ideal, 140kv is very low for that voltage, I would go for a 10s at least. If your budget is too low, go for lipos and a balance charger, otherwise study a bit more about the best battery combination, how to build one, which bmss are the best etc. 
English is not my native language either, and I'm young and didn't know anything about this stuff before building. My first thread was kinda like this one, and I regret. Then I read thousands of posts and I can finally help you
```

---
## \#9 Posted by: DavidBanner Posted at: 2017-07-17T13:56:26.499Z Reads: 99

```
you might want to dial the attitude back. no one here owes you anything, they are helping out of kindness alone.

i managed to figure what u are asking by research alone.

folks here are giving you really good advice that will stop you making a very expensive mistake which could also set fire to your home and cause life changing injuries....
```

---
## \#10 Posted by: bartroosen12 Posted at: 2017-07-17T14:52:51.942Z Reads: 96

```
In my opinion a 6S build is good to start, I have made 3 builds until now with a 6S battery and it has enough power for me max speed 40kmh so fast enough.

I have used several esc's but the FVT 120A is really very good for it's price, just buy the programcard also so you can adjust some things like brakes and acceleration.

So your pack will output max 45A by 22,2V, maybe that will will be enough if you don't do any hills but I should try lipo cells if you wanna make a 6S build otherwise if you wanna make a 6S pack with 18650 cells you need like double the Amps like 90A for you pack otherwise your cells will have to work very hard with 45A max.

I think they also have a 200kv motor on banggood, but you can also buy from hobbyking. Just find out what max speed you want, which wheels you wanna use (I should go for flywheel clones), the pulleys you gonna use and calculate the motor kv which you need.
After this you know which motor kv you need to look for ;)

https://www.instructables.com/member/bartroosen/instructables/
Here are 2 of my 6S builds and they are strong enough for me (weight with backpack around 100kg)
```

---
## \#11 Posted by: wafflejock Posted at: 2017-07-17T16:23:45.144Z Reads: 89

```
Saying things like "my motor needs 34A" and talking about batteries in terms of "packs" instead of parallel and series connections just raises some flags that despite having a pretty good idea of what you're talking about you maybe aren't at the 95-100% knowledge level you should have about the details here to be building your own battery.  I'm not an electrical engineer either (my Dad is and I'm a programmer, CS degree)... I don't trust myself to put together one of those batteries really and I was trying to give you feedback about the components I do know well (ESC since I basically have that one in a drawer and am now using a VESC).

Understand there are tons of noobs that come through here and post a list of parts without using the calculators available or reading up on builds using similar components, it's a bit of knee jerk reaction here to be sure people actually searched around instead of posting first.  Good to see you're doing research, but I would focus in more on the BMS and battery pack building threads if you plan to do that yourself, it's a pretty serious endeavor and if you mess up you're likely to start a fire either burning your board up or worse.

With a BMS you are basically putting a balance charger onto the board.  Things to consider:

1.  What is the total wattage it can charge at, given your battery voltage how many amps will it be driving the current in with and therefore how many hours is it going to take to charge?

2.  What does the AC->DC transformer that you need to go with it look like, how many watts can it handle, needs to be more than what the charger will need to draw?

3.  How much do you care about the charge time?

4.  Does the BMS actively discharge cells in order to keep things balanced?  If so this will lead to more cycles on the batteries.

5.  Does the BMS bring all the cells up to 4.2V or whatever the charged voltage is for the cells you're buying?  Does it just advertise that or have people reviewed/tested it?  Does it do a good job balancing the cells? How long does that take on average?

6.  Are you relying on the BMS for cutting off the power to the ESC to save the cells from low voltage, if so the power will need to flow through it and it needs to be able to deal with the full amperage the motor will pull (what happens when you draw more than that?)  This could be in part solved by using a VESC then you can bypass the BMS and use the low voltage cut off in the VESC (not sure with the ESC there can be programmed for low voltage cut offs where it ramps down the power like the VESC).

7.  What parts do you need to change out if you decide you want to upgrade?  Is it going to require a new BMS new ESC and new battery pack?  If so is that the best choice for your first build?  How much more does it cost to upgrade all these things than to get a VESC, balance charger, and LiPo packs (which in total are probably cheaper in the first place)?
```

---
