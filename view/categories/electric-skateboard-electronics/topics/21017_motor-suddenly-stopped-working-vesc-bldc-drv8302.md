# Motor suddenly stopped working (VESC,BLDC, DRV8302)

### Replies: 21 Views: 1718

## \#1 Posted by: TranxFu Posted at: 2017-04-14T18:19:27.602Z Reads: 127

```
Hey guys,

was working on my board when I noticed that the wheel pulley was grinding on the mount just a bit. Small sparks whenever I hit the throttle. Was putting it back together and hit the throttle again. Then it spun up and now it doesn't work anymore. 

Setup is a VESC/10s4p/Single motor 6374 190KV/FOC. The BLDC connects without issues. However I can't manually spin up the motor using the arrow keys or do a motor detection. Is there anywhere I should take a look at ? 

Phase wires didn´t come or are loose. I can still read all settings in the BLDC tool and the VESC connects just fine.
```

---
## \#2 Posted by: TranxFu Posted at: 2017-04-14T18:27:13.090Z Reads: 129

```
Oh well nvm. on the active sampling page it states DRV8302 whenever I pull the trigger... Damn, what a bummer. It was running so well the last days...
```

---
## \#3 Posted by: t0m_r1dd1e Posted at: 2017-04-14T18:32:29.614Z Reads: 124

```
Bummer. Any idea how it blew?
```

---
## \#4 Posted by: TranxFu Posted at: 2017-04-14T18:35:25.946Z Reads: 120

```
Mhmm.. It was running in FOC really well the last days. Maybe it could have sth. to do with the update I did today. I flashed the new 2.54 firmware and tool that ackmaniac released. First time doing watt w. reverse and his new mode. That is the one noticeable change I did :/ ... 

Just checked and the only service doing VESC repairs in Germany closed down because Vedder licensed his work. Does anyone here in Germany repairs DRV8302 errors ? 

I dont notice anything burnt or smelly from the VESC.
```

---
## \#5 Posted by: Guacamoleface Posted at: 2017-04-14T18:40:33.636Z Reads: 115

```
What Vesc are you using?

I "Blew" my vesc straight off when I went with default FOC settings, it works in bldc somehow tho.
```

---
## \#6 Posted by: TranxFu Posted at: 2017-04-14T18:42:40.795Z Reads: 112

```
Using a Axle VESC. 

I get the DRV8302 too, when trying to do anything in BLDC. :disappointed_relieved:
```

---
## \#7 Posted by: TranxFu Posted at: 2017-04-14T21:53:45.244Z Reads: 108

```
<img src="/uploads/db1493/original/3X/0/5/0572290455ac6ae30c609bd2aa2d3c52101121ae.JPG" width="375" height="500"><img src="/uploads/db1493/original/3X/1/2/12f49845598e93b0be51042595419e58aaca2043.JPG" width="375" height="500">
```

---
## \#8 Posted by: Guacamoleface Posted at: 2017-04-14T21:55:24.752Z Reads: 101

```
I recall Axle having a great warranty? could be worth contacting them, see what they say.
```

---
## \#9 Posted by: TranxFu Posted at: 2017-04-14T22:11:44.565Z Reads: 101

```
Yup, I've contacted @zmoney and he immediately offered me to take care of it! really great service. However they are located in the US... didn't even know as I have gotten this VESC from a forum member :pensive:
```

---
## \#10 Posted by: Guacamoleface Posted at: 2017-04-14T22:14:36.936Z Reads: 99

```
Nice of them to actually offer that especially since you didnt purchase it from them directly.

Yeah, I thought mine was toast aswell, and as you mentioned the german DRV repair is closed.. 

Considered(consider) getting myself a hotair solder station, some drv chips and futureproof myself abit. Wanna go Foc again but dont dare without any spare parts.
```

---
## \#11 Posted by: TranxFu Posted at: 2017-04-15T09:21:36.918Z Reads: 93

```
Did yours immediately work after putting it to BLDC again ? And you are not getting the DRV8302 error when running the motor in BLDC ?

Yea that would be great. I don't know about the learning curve compared to normal soldering tho. 
There are some local services here that offer SMD-Soldering and works. But I've read that most of the time it is not just the DRV8302 that needs to be replaced. And those guys did not work with VESCS before... 



----------
Another thing, I'd like to rule out that my motor is dead too. Is there a way to check up on the motor ? I don't have any other ESCs lying around. Is it correct that it does absolutely nothing(no stuttering,...) when trying to manually spin it via the arrow keys in the BLDC. It is just cold dead. Is that the way the motor behaves when having a DRV fault ?
```

---
## \#12 Posted by: Maxid Posted at: 2017-04-15T10:00:44.979Z Reads: 82

```
Oh wow I did not know that they stopped repairing VESCs. Seems a little off as only the name is trademarked, so I don't get why they have to stop repairs on already existing hardware. Have you contacted them and asked for an explanation?
```

---
## \#13 Posted by: TranxFu Posted at: 2017-04-15T10:04:55.528Z Reads: 82

```
I've wrote an email yesterday. Will update when I receive an answer.


----------
If there is anyone else doing VESC repairs in Europe/Germany, feel free to drop me an message ! :wink:
```

---
## \#14 Posted by: Guacamoleface Posted at: 2017-04-15T10:38:43.524Z Reads: 78

```
I did not try until day after as I was sure it was dead(even smelled burned). Reset default day after, did my motor detect and settings and it worked. Tried it outside aswell as on bench. No errors
```

---
## \#15 Posted by: XIII Posted at: 2017-04-15T15:43:16.007Z Reads: 75

```
https://ticket.lp-electronic.com/

If you need your vesc fixed in Germany. This is the one I am using. (esk8.de gave me his email )
```

---
## \#16 Posted by: Maxid Posted at: 2017-04-15T16:00:19.160Z Reads: 69

```
That is the one he means. On the website they say they stopped repairing vescs
```

---
## \#17 Posted by: XIII Posted at: 2017-04-15T16:02:17.092Z Reads: 68

```
I hope not because he should be working on one of mine ! :)
```

---
## \#18 Posted by: Maxid Posted at: 2017-04-15T16:05:49.939Z Reads: 70

```
Well maybe you got lucky

This is what they posted:

Update 28. März 2017

Mit sofortiger Wirkung bieten wir keine Services für das VESC Projekt an. Herr Vedder hat sich entschieden „VESC“ als Trademark zu führen und selber kommerziell zu vermarkten.
```

---
## \#19 Posted by: Fatglottis Posted at: 2017-04-16T21:53:53.681Z Reads: 65

```
Hi guys, I'm new here :) 

I had contact with LP Electronics the 27/3, telling him my VESC broke. I created a ticket in his system and got a message telling me to send the VESC which I did the 28/3. Asked him 10 days ago if he received the VESC but I haven't got a reply yet. I hope he is alright. 
He has helped me with three VESC repairs prior to this one. Great service!!
Did not know he was quitting :frowning: Hope I can get it back if he will not fix it. 
 
Unfortunately I broke my other VESC yesterday.. again.
Man, I have killed my two VESCs five times now and only ridden around 50km on my board :blush:
 
Yesterday I ordered two new VESCs.. different brand and I improved my HW design around the VESCs to prevent any more failures. 
Also ordered a hot air gun station and all the equipment needed so I can start doing my own repairs. This can only be a success haha! :smiley:
```

---
## \#20 Posted by: TranxFu Posted at: 2017-05-02T16:27:14.715Z Reads: 61

```
@Fatglottis any news on your VESC ?
@Maxid

Hey guys, just a quick update on this that might be of interest to you :) I've used the link @XIII posted and I've gotten a reply to send them/him the VESC including price details,... 

VESC has arrived a week ago and still awaiting an update to the status. 

Also the post on the original website is gone. I guess he changed his mind about servicing VESCS :smile: Well, good to know there is somebody in your country who can do the work for you.
```

---
## \#21 Posted by: Fatglottis Posted at: 2017-05-02T17:03:42.469Z Reads: 53

```
Yeah he fixed mine! :slight_smile:
It seems to run fine now. 

My vesc failures were most probably due to bad design made by me. Kept blowing STM32 all the time. I have now attached a 10awg ground wire between my two vescs. Soldered between the capacity boards so that the ground potential is more or less the same on both units. 
I also added transient protection with a resistor and a zenerdiode on each tx/rx on the UART-input to prevent killing the STM32 with voltage spikes. 
Have run 30km now and no failures yet.  Running UART with a teencyLC on the board and the remote is a wii nunchuck with arduino nano. 

Good to know he went back in business! :slight_smile:
```

---
