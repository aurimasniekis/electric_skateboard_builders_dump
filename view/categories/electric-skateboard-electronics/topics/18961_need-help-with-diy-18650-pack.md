# Need Help With Diy 18650 Pack

### Replies: 14 Views: 1122

## \#1 Posted by: Gmoney Posted at: 2017-03-12T19:56:47.513Z Reads: 153

```
Now that I have done some research I am almost ready to start my build. But there is one problem, I have no clue what I'm doing when it comes to batteries and BMSs. I plan on making a single motor build with 190kv. I want to go at least ten miles on a charge and reach 25mph. I have heard Samsung 25Rs are good so I will most likely use them in a 10s3p. That's about all I know for sure. Laptop style charging with a BMS would also be great, but I don't know what kind is the best for a 10s3p pack. My main issue for now is the BMS. If you could answer any questions or help in any way that would be great.
```

---
## \#2 Posted by: OskarCastrone Posted at: 2017-03-12T21:07:45.289Z Reads: 141

```
Hi

I have a spot welder and some BMS units on the way. I can make a battery for you if you are interested? If you choose the BMS with discharge function, I can also include a LED power switch. A 2a charger and power outlet could also be included. If you want lights I am also cabable of doing that. If you just want the possibility to install lights in the future, I can just make an outlet supplying you with 12v. 
If you want more info or pictures. Just let me know.
```

---
## \#3 Posted by: Gmoney Posted at: 2017-03-12T22:26:46.801Z Reads: 130

```
How much would something like that cost?
```

---
## \#4 Posted by: Guacamoleface Posted at: 2017-03-12T22:43:59.845Z Reads: 131

```
Hey from across the bridge!
What kind off BMS are you getting? I'd love to know more about that! Currently running my 10s4p without bms(just got it together today and went on my first testride outside). 

Sorry Gmoney for abit offtopic!
```

---
## \#5 Posted by: Guacamoleface Posted at: 2017-03-12T22:46:10.274Z Reads: 129

```
I currently have a 10s4p with thoose(samsung 25r) batteries, Im pretty sure it does 25mph ++, tried it today at 35kmh but had alot of throttle left. 25mph = 40kmh ish as for comparing. 

also its single drive 190kv!
I have no bms but I would recommend having one. I will most likely get one  soon aswell.

I heard supower have some great bms!
```

---
## \#6 Posted by: Eboosted Posted at: 2017-03-12T23:16:31.462Z Reads: 123

```
I have a supower bms, it resets if the battery is fully charged and you brake. I really hate that. 

The battery becomes unbalanced every once in a while even if you leave it plug it overnight. 

Not extremely happy with this bms, might try the Bestech one soon
```

---
## \#7 Posted by: Guacamoleface Posted at: 2017-03-13T12:30:40.061Z Reads: 115

```
Now that you say so, I recall reading someone having that problem at full charge aswell. but the fact that it gets unbalanced...Thats the main reason I'd want a bms - to keep it balanced.
```

---
## \#8 Posted by: PXSS Posted at: 2017-03-13T13:45:48.127Z Reads: 114

```
* Use Samsung 30Q cells instead (Sourced from Nkon) - 25Rs aren't that good (You can look up plenty of threads where I explain why)
* BMS from Bestech or Supower is the standard, people have been having issues with the one from Supower so I would only recommend Bestech, they have a moq of 2 units though.
* You can either solder to your batteries or spot weld them. Spot Welding is better but if you don't have the equipment and you are good at soldering, you might want to explore that route. There are a few threads that explain how to do this.
* There are plenty of laptop chargers for 10S available in aliexpress, I have one that charges 10S at 5A that I'm most likely going to get rid off once I get my new variable voltage one if you want it (and are in the USA). 
* To determine what current you want to charge the batteries at, I recommend that you look up the spec sheet of whatever cell you use, find their standard charge rate and then multiply that by however many cells you have in parallel.
* There are several people that offer their battery assembly services but IMO it is way overpriced, 10S3P battery materials would cost $200 including all required materials, an antispark switch and BMS, while they would charge upwards of $350, some as high as $450.
```

---
## \#9 Posted by: OskarCastrone Posted at: 2017-03-13T19:20:22.456Z Reads: 98

```
I have not figures that out yet... But, I can promise you that it will not be very expensive if you are willing to post some feedback / review on this forum in return. I will soon begin to offer this service, so I will need some advertising :-) 

Please write me a pm with your prefered specifications. Then I can give you a price.
```

---
## \#10 Posted by: OskarCastrone Posted at: 2017-03-13T19:25:50.534Z Reads: 94

```
I would really recommend a BMS! 
I have some on the way from Bestech. One with 80a discharge (perfect for your battery with 10s4p Samsung 25r cells), and one with 20a discharge, where you will bypass the BMS and use the VESC to set the battery amp limit. With the last model you will also need some sort of switch, since it does not come with a build in power switch... 
Please send me a pm if yu are interested! :)
```

---
## \#11 Posted by: Eboosted Posted at: 2017-03-14T04:31:57.623Z Reads: 85

```
Oscar, are you going to have a spare Bestech 80A BMS? when do you extect to receive them? are you in USA?
```

---
## \#12 Posted by: OskarCastrone Posted at: 2017-03-14T11:04:17.847Z Reads: 78

```
Unfortunatly I am from Denmark... I believe that shipping to US would make it too expensive for you?
```

---
## \#13 Posted by: longhairedboy Posted at: 2017-03-14T11:35:41.782Z Reads: 75

```
The braking/resetting issue with the Battery Supports BMSs can be mitigated with settings in the VESC. I keep my Batt Min (regen) set to -4 and no longer have this issue, and i still get stiff brakes. I've yet to have one of these fail in a situation that wasn't my fault, but I've had a few BesTechs arrive DOA.
```

---
## \#14 Posted by: Eboosted Posted at: 2017-03-14T17:09:37.951Z Reads: 63

```
I've tested -4 A on batt min regen and I still got the reseting issues consistently.

Braking was also not as safe as -8 or -10A
```

---
