# One motor at 60amps or 2 at 30A?

### Replies: 44 Views: 970

## \#1 Posted by: robthebuilder Posted at: 2019-03-29T20:36:16.355Z Reads: 226

```
Hi guys! :slight_smile:

I need help from someone with more experience!

I have a board atm with a single 6374 190kv TB motor on it. I'm running a 12S3P battery pack with 30Q cells.

I'm thinking of adding a second motor to it, but.. Right now I have to limit my ESC at 60A from the battery as the pack can't handle more current. If I add a second motor I will have to limit the ESC's at 30A each. Right?

Do you think I will notice a difference or will it be the same apart from the added traction? I want some extra power for the steepest hills :sunglasses:

I know I should upgrade the battery pack also, but right now I'm on a tight budget as I'm studying for another year.

Thanks guys!
```

---
## \#2 Posted by: taz Posted at: 2019-03-29T20:42:06.398Z Reads: 216

```
The difference will be night and day.

@dareno I don't need to say it, do I?:rofl:
```

---
## \#3 Posted by: dareno Posted at: 2019-03-29T20:42:07.815Z Reads: 214

```
You will notice a difference going from one motor to two and yes you are correct in the assumption that you have to split the amp draw across both vescs.
```

---
## \#4 Posted by: dareno Posted at: 2019-03-29T20:42:39.133Z Reads: 207

```
I was waiting for you just to make you feel good lol
```

---
## \#5 Posted by: taz Posted at: 2019-03-29T20:43:34.935Z Reads: 206

```
Old geezer fight, lol
```

---
## \#6 Posted by: Bjork3n Posted at: 2019-03-29T20:44:13.713Z Reads: 200

```
The diffrence is huge on a dual compared to single.. HUGE!
```

---
## \#7 Posted by: nirurin Posted at: 2019-03-29T20:45:04.373Z Reads: 196

```
Not the OP, but I honestly can't tell if all these answers are sarcastic or not lol
```

---
## \#8 Posted by: robthebuilder Posted at: 2019-03-29T20:45:41.167Z Reads: 194

```
Thanks for all the replies! I can't understand how the diffrence would be so dramatic with the same power tho'. But I will probably try it out and see :slight_smile:
```

---
## \#9 Posted by: dareno Posted at: 2019-03-29T20:47:21.866Z Reads: 189

```
[quote="robthebuilder, post:8, topic:88728"]
But I will probably try it out and see :slight_smile:
[/quote]

Best answer anyone gave ever.  True builders spirit.
```

---
## \#10 Posted by: robthebuilder Posted at: 2019-03-29T20:48:12.025Z Reads: 186

```
Haha! Experience is knowledge :smile:
```

---
## \#11 Posted by: taz Posted at: 2019-03-29T20:50:32.183Z Reads: 184

```
Scientia est lux lucis
```

---
## \#12 Posted by: Mich21050 Posted at: 2019-03-29T20:53:10.038Z Reads: 180

```
https://www.electric-skateboard.builders/t/one-motor-at-60amps-or-2-at-30a/88728/11?u=mich21050

For everyone who can't speak Latin. :slight_smile:
https://en.wikipedia.org/wiki/Scientia_est_lux_lucis
```

---
## \#13 Posted by: Superflim Posted at: 2019-03-29T20:53:44.767Z Reads: 169

```
Slightly off topic question. 

But would a for example 6374 motor ran on 40% load more efficient or a 5056 at 75% load
```

---
## \#14 Posted by: robthebuilder Posted at: 2019-03-29T20:54:07.832Z Reads: 165

```
The 6374 would be cooler at least :slight_smile:

It would probably also last longer since it has to do less work
```

---
## \#15 Posted by: taz Posted at: 2019-03-29T21:02:44.183Z Reads: 162

```
This. Lower temperatures also mean less power losses.
```

---
## \#16 Posted by: wafflejock Posted at: 2019-03-29T21:07:10.227Z Reads: 157

```
https://www.electric-skateboard.builders/t/torque-curves-for-sk3s-6354-260kv-6374-149kv-6374-192kv/19721 <-- can see some efficiency charts here but agree with others in general more overhead is a good thing and keeping heat losses and amperage low is ideal.
```

---
## \#17 Posted by: b264 Posted at: 2019-03-29T21:07:28.924Z Reads: 157

```
[quote="dareno, post:3, topic:88728"]
yes you are correct in the assumption that you have to split the amp draw across both vescs.
[/quote]

But you only split the "battery" current numbers, not the "motor" current numbers
```

---
## \#18 Posted by: dareno Posted at: 2019-03-29T21:11:54.797Z Reads: 155

```
We were talking about the battery.  Now share some knowledge about the difference using 2 motors and the advantages of motor amps.  Share the love Brian.  I love it when you go all techie
```

---
## \#19 Posted by: Pedrodemio Posted at: 2019-03-29T21:14:46.458Z Reads: 157

```
First things first

Motor current ≠ Battery current

Right now you are using 60A on the motor and the battery

With two motors you will set 30A on each VESC but you can and should set 60A on each motor, this way you have 120A in the motor total, meaning you will have double the torque

Now to the catch, to limit the battery current to 30A, the VESC wont go above 50% duty cycle, what that means? In the hill that will require each motor to keep at 60A you will climb at half of your top speed for a given battery voltage

* If you can't climb some hill at 60A motor and battery, you will be able to climb it with dual motor

* If you can climb a given hill right now, you won't climb it faster by going dual motor

In the first case you would be torque limited, it doesn't matter at what speed, your motor at 60A simply doesn't have enough torque

In the second case you are power limited, and what constrains it is the battery max
```

---
## \#20 Posted by: Eboosted Posted at: 2019-03-30T02:48:48.752Z Reads: 134

```
Dual motors will give you more stability on full acceleration, you will feel safer and might ride with more confidence, braking two wheels is way more effective than a full brake on one wheel. Acceleration will be more powerful as you are already increasing efficiency on motors by reducing the current and accumulating less heat. 

Go for it and report back with your findings, thank us latter
```

---
## \#21 Posted by: Dirt_Bag Posted at: 2019-03-30T06:19:35.635Z Reads: 119

```
30a is still alot of current.  You will notice huge difference in performance. I made a board that i teach other people to ride on and its dual 6355 set at 25a each. Its still way more power than most people can handle. Certainly more than a boosted.
```

---
## \#22 Posted by: taz Posted at: 2019-03-30T06:29:01.780Z Reads: 121

```
I don't think I have ever drawn over 70A battery on my dual 6374 street setup with pneumatic tires and that is climbing some serious hills.

Welcome to the dark side :sunglasses:
```

---
## \#23 Posted by: robthebuilder Posted at: 2019-03-30T08:06:43.115Z Reads: 115

```
Great information! Thank you for helping me understand it all :grinning:
```

---
## \#24 Posted by: robthebuilder Posted at: 2019-03-30T08:09:07.836Z Reads: 112

```
Thank you for all the great help :grinning: Looks like I will add a 2nd motor then :sunglasses:
```

---
## \#25 Posted by: Wilsonliang777 Posted at: 2019-03-30T08:48:31.530Z Reads: 107

```
I am  the same boat now.  I have a board running on a 6264 190kv motor with vesc setting of 50amps and I am thinking of switching it to 2x 5365 200kv.  I running 10s lipo so I think I can pull 70 to 80amp.  

Today while I was going up some hills  and I noted  that not have enough tractions is the problem with single drive system.  My single 6364 had enough power but it was slipping because lack of traction and perverting effective hill climb.
```

---
## \#26 Posted by: robthebuilder Posted at: 2019-04-02T11:00:47.260Z Reads: 91

```
The snow here in the north of Sweden hasen't melted yet, but I went for a short ride today and recorded the VESC status.

With my single 6374 motor, the maximum amp draw from the battery pack was only 15A and the max motor amp was at 45A. With that knowledge I will surely throw another motor on there and check the difference :sunglasses:
```

---
## \#27 Posted by: Superflim Posted at: 2019-04-02T13:34:15.361Z Reads: 83

```
What setup and you running?

How can you draw so low?
```

---
## \#28 Posted by: robthebuilder Posted at: 2019-04-02T14:35:03.076Z Reads: 80

```
I have no Idea why.. my setup is a One Wheel drive, 90mm wheels, 16/36 teeth pulleys, 6374 190kv TB motor, VESC 4.12, Samsung 30Q 12S3P battery pack.
```

---
## \#29 Posted by: Superflim Posted at: 2019-04-02T14:37:18.951Z Reads: 80

```
What are your settings?
```

---
## \#30 Posted by: robthebuilder Posted at: 2019-04-02T16:12:05.560Z Reads: 77

```
60A on motor and battery and I run BLDC mode
```

---
## \#31 Posted by: Superflim Posted at: 2019-04-02T16:13:54.343Z Reads: 76

```
Your measurements must be wrong....You must be very very light or you're very conservative on the trigger.

I'm 70 kilos myself almost same setup and drawing 35 bat amps max.
```

---
## \#32 Posted by: robthebuilder Posted at: 2019-04-02T16:40:18.393Z Reads: 69

```
They might be wrong ofc. I'm 70 kilos and i'm not light on the trigger at all :joy: I always kick my board when I start tho'. I never use the motor to start from a standstill.
```

---
## \#33 Posted by: robthebuilder Posted at: 2019-04-02T16:41:51.950Z Reads: 70

```
An as I said, there is still snow in places here so I could't ride fully normal today. I will try again when the conditions are better and see :)
```

---
## \#34 Posted by: wafflejock Posted at: 2019-04-02T19:22:23.193Z Reads: 66

```
I would check to see if you have anything adding friction to the wheels (bad belt alignment something overtightened etc.) I typically get much lower amperage (I am light on the trigger and light weight, but still 35A on the battery is quite a bit unless you're gunning it/racing or hill climbing) <<-- granted this is a chill cruise to the convenience store and back but still got up to 16mph and at most 6.5A on the battery.  Would be curious to see your data (ideally elevation changes too since I think this plays a pretty big role but just acceleration/velocity vs amperage would be interesting too)
```

---
## \#35 Posted by: Superflim Posted at: 2019-04-02T19:27:25.772Z Reads: 61

```
extra friction might be my suck ass bearings. need to replace those. Belt is aligned fine. I guess it could be slightly tighter. I draw many amps when I jam full throttle to top speed. But maybe it's my riding style too. I like to ride aggressively. I almost always ride on flats.
```

---
## \#36 Posted by: wafflejock Posted at: 2019-04-02T20:24:54.888Z Reads: 64

```
Yah I'm sure slamming the throttle I could get higher values, but generally speaking I'm just using the board for cruises similar to the one recorded to run to local stores not using it as a thrill ride, but different strokes for different folks and all, just wouldn't expect to get that high of draw when jumping on the board to go and riding flats for light riders (I also typically set some amp limit on the motor to avoid accidentally punching it out from under my feet, has happened once before, luckily just landed on my backpack and felt stupid for a minute).  Most ebikes are limited to 600W so really that's typically enough and at 15A with 50V it's 750W so it's enough power to keep you moving but really depends on how fast your accelerating what peaks you'll hit.
```

---
## \#37 Posted by: robthebuilder Posted at: 2019-04-04T08:47:20.592Z Reads: 57

```
I just made an order for a second 6374 motor so I will keep you posted on the result :) I'll have to figure out how to make one VESC a master and the other a slave and things like that but I think it'll be alright! In one or two weeks I should have the parts so we'll see how it goes :sunglasses:
```

---
## \#38 Posted by: robthebuilder Posted at: 2019-04-04T11:19:14.013Z Reads: 52

```
If anyone knows or can link a video for how to setup dual VESCs via a CAN-bus please hit me up :) I use the old BLDC-tool as I like this the best. If it's the only option, I can ofc use the new VESC-tool also!
```

---
## \#39 Posted by: sk8l8r Posted at: 2019-04-04T11:44:35.082Z Reads: 53

```
https://www.electric-skateboard.builders/t/how-to-program-canbus-properly-video-tutorial/52606
```

---
## \#40 Posted by: lrdesigns Posted at: 2019-04-04T11:59:28.232Z Reads: 52

```
I have dual setup and if one is down it feels like 30% as much power. I rode a friends single setup and it was easy to break traction.
```

---
## \#41 Posted by: robthebuilder Posted at: 2019-04-16T15:25:11.526Z Reads: 47

```
My parts should be here tomorrow so I hope to report my findings after the weekend :blush:
```

---
## \#42 Posted by: robthebuilder Posted at: 2019-04-17T18:49:28.256Z Reads: 41

```
I got all my parts today but I have a problem..

My new VESC doesn't want to upgrade it's firmware. I did this last week on my old VESC and it was not a problem. But on the new VESC it says that the firmware is too old so I upgrade it, but still when reconnecting after a successful firmware write, it still tells me the firmware is too old. The firmware on it is 3.50 both before and after upgrade.

Can anyone help me with this? :)
```

---
## \#43 Posted by: robthebuilder Posted at: 2019-04-19T06:43:36.871Z Reads: 36

```
Problem solved! One VESC can help program the other. Thanks to Trampa for helping me out :)
```

---
## \#44 Posted by: robthebuilder Posted at: 2019-04-19T13:06:42.932Z Reads: 26

```
I've been riding a bit today and, my lord.. This is awesome! :sunglasses:

Dual motors is waaaay more powerful than one, even with the same battery power. The steepest hills is not a problem at all! And even better, the traction is perfect. I rode on really loose gravel without a problem. I can recommend this to everybody! Even if you don't need more power, the traction makes the ride feel so much safer. The brakes are ofc also much, much better.

The only thing that's better with a single motor is the lighter weight and the slightly longer range, tho' range has never been an issue for me so that's not a problem.

Thanks everyone for your help and for pushing me over the line with the purchase :joy:

Have a great day! :grinning:
```

---
