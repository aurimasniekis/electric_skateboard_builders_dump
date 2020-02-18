# BMS question! Noob alert

### Replies: 43 Views: 598

## \#1 Posted by: MrDGOrman Posted at: 2018-09-23T19:25:30.023Z Reads: 138

```
Hi everyone,

I'm in need of some advice. I'm looking to buy a BMS which I can use with my current LiPo batteries (3 batteries with 3 cells each) and then use again with my Li-ion setup which I plan to do in a few months time. I've found this one from eskating.eu and I'm confused how everything will work.

Is it compatible with my 3s3p lipo setup and will it be compatible with a 10s4p setup after?
Bestech website says its for a LiFePO4 (?) setup?

https://eskating.eu/product/10s-bestech-bms-80a-10s4p/

Thanks,
Daniel
```

---
## \#2 Posted by: Andy87 Posted at: 2018-09-23T19:54:09.080Z Reads: 121

```
You mean 3s3p or you will put the 3x 3s in series to get 9s?
Why not only get a lipo balance charger like this one 
hengda iMax LiPo/NiMh 1s-6s Akku Multifunkt. Ladegerät Balancer Adapter inkl. 5A Netzteil https://www.amazon.de/dp/B00FF6DA0G/ref=cm_sw_r_cp_api_J6-PBbK3T8QXQ
For the time you use your lipos?
Use a fuse and a antispark loop key in your board set up and you also good to go.
The only down side is that you need to take out the packs and charge them separated from each other
```

---
## \#3 Posted by: MrDGOrman Posted at: 2018-09-23T20:08:20.374Z Reads: 108

```
They're in series already. 3 batteries, in series, each with 3 cells in.

I'm currently taking the batteries out to charge them already. I thought I'd be fine with it but I'm not. It's annoying having to remove my enclosure each time.i want to charge the batteries. I just want to plug the board in and away I go.

Is there a way I could makeshift this BMS to work with the LiPos? If not then what smart BMS could I use?
```

---
## \#4 Posted by: Andy87 Posted at: 2018-09-23T20:19:00.504Z Reads: 105

```
[quote="MrDGOrman, post:3, topic:68993"]
They’re in series already. 3 batteries, in series, each with 3 cells in.
[/quote]
Yes i undetstood, but if you put them all in parallel you will still have only 3s which is 11v only...🤔

Unfortunately I can’t recommend you any smart bms as I don’t have experience with them.
But put it in the search function here. There some guys already using it.

[quote="MrDGOrman, post:3, topic:68993"]
just want to plug the board in and away I go.
[/quote]
Don’t want to be the  ☝️ ☝️ ☝️ guy, but it’s never good to go away from a charging board... 
https://www.electric-skateboard.builders/t/eu-sickboards-caliber-truck-sale/59110/10?u=andy87
```

---
## \#5 Posted by: MrDGOrman Posted at: 2018-09-23T20:46:27.189Z Reads: 87

```
Is 11v bad? People always said to link them in series rather than parallel.

I always charge my batteries with a balance charger to prevent over charge etc. They automatically cut off when they reach full charge (4.2v). My understanding is that the BMS is effectively the same as a balance charger. When the power goes in from the wall it is then balanced through the BMS?

In short, a BMS isn't going to be suitable for a LiPo battery setup unless I have 10 of them in series?
```

---
## \#6 Posted by: mynamesmatt Posted at: 2018-09-23T23:00:21.876Z Reads: 82

```
all your lipos are most likely 3s packs. or do you have a 1s3p pack? i doubt that
```

---
## \#7 Posted by: Jake2k17 Posted at: 2018-09-23T23:47:54.023Z Reads: 82

```
Aren't diebyms smart bms?
```

---
## \#8 Posted by: AreaKruzer Posted at: 2018-09-24T02:52:25.979Z Reads: 76

```
Not that 11v is bad. But the voltage is generally too low to power the motor. 

At bare minimum, people are running 6s. Lower voltage means higher current is needed. And higher voltage will result in lower current.
```

---
## \#9 Posted by: MrDGOrman Posted at: 2018-09-24T13:19:11.269Z Reads: 68

```
@mynamesmatt @AreaKruzer

My battery setup is on the right, so series. Each battery has 3 cells. They're Zippy Flightmax 5000mah.
https://i.stack.imgur.com/OmK0c.jpg

I've been running my setup like this for ages and it works fine?

@Jake2k17 I'll check out diebyms. I think I saw a thread on the forum about them.
```

---
## \#10 Posted by: AreaKruzer Posted at: 2018-09-24T13:51:55.271Z Reads: 61

```
Yup. Running them in series will give u 6s. Almost a bare minimum setup
```

---
## \#11 Posted by: MrDGOrman Posted at: 2018-09-24T15:26:03.632Z Reads: 54

```
I've got 3 so it's 9s..

![Battery%20setup|455x500](upload://608USQKINEOj75gjoCXQLZlM9xA.png)
```

---
## \#12 Posted by: Jake2k17 Posted at: 2018-09-24T17:48:29.652Z Reads: 46

```
Yes this is correct. Are you running a bms?
```

---
## \#13 Posted by: MrDGOrman Posted at: 2018-09-24T18:05:11.119Z Reads: 50

```
Not currently because it was to my understanding that the BMS is to manage the charging aspect of things. Also allowing you to keep everything in the enclosure rather than removing it all the time.

Currently I have the batteries connected to the FOCBOX. Inbetween the two is a fuse and XT90S anti spark loop key.

I'm wanting a BMS that I can use to charge the batteries so I don't need to remove the enclosure. Plug a lead in and boom, it charges. Also have an on off switch to remove the antispark I currently have. But I also want to have a BMS I can use for the LiPo setup and then again for when I purchase the Li-Ion batteries to make my own pack. I to avoid paying for the BMS twice.

My understanding would be getting a 10s or 12s battery and splicing the additional wires into a single cell wire so it gathers the data that way. Because that's all it's doing, right? Grabbing the voltage reading to determine the max cut off. If I had a BMS that was suitable for a 12s setup then surely splicing the wires will be fine because it's doing the exact same thing? The BMS would think those cells are exactly the same voltage.

Please correct me if I'm completely wrong!
```

---
## \#14 Posted by: Jake2k17 Posted at: 2018-09-24T19:16:16.030Z Reads: 40

```
You can use the same bms for both liion and lipo, but a 9s bms is pretty hard to find. Unless you have purchased the batteries already, I really suggest using 2x 5s batteries, they are much easier to charge and find a bms for.
```

---
## \#15 Posted by: b264 Posted at: 2018-09-24T19:39:01.714Z Reads: 39

```
[quote="Andy87, post:2, topic:68993"]
Why not only get a lipo balance charger
[/quote]

Don't do that.  Use a BMS
```

---
## \#16 Posted by: b264 Posted at: 2018-09-24T19:40:12.674Z Reads: 40

```
[quote="Andy87, post:4, topic:68993"]
Don’t want to be the :point_up:️ :point_up:️ :point_up:️ guy, but it’s never good to go away from a charging board…
[/quote]

When I get home from work, I can't watch my board charge for two hours.  If I did, I would spend my ENTIRE LIFE watching boards charge.  Do you watch your car sit in the garage for two hours every time you get home?
```

---
## \#17 Posted by: b264 Posted at: 2018-09-24T19:42:18.769Z Reads: 41

```
That BMS will work for 9S and 10S but if you're going to use a loopkey and bypass the BMS for discharge, I would get the ["D190" 10S BMS by bestech](http://www.bestechpower.com/32v10spcmbmspcbforlifepo4batterypack/PCB-D190.html) and since you have to buy 2, sell the other one on the forum after you get it and finish your battery.

To use a 10S BMS for 9S always make sure the most-positive balance lead is the one left unhooked.  Start at negative and go from there
```

---
## \#18 Posted by: Andy87 Posted at: 2018-09-24T19:47:49.062Z Reads: 40

```
Yes i do...what else to do in my free time...
I didn’t say sit and wait till it finished charging.
But leave it alone while charging is simply not good. 
I had a fire in my home and i‘m happy that i was close to stop it from burning down everything around.
I does not need to happen with everybody, but just some days ago it happened with one of our member... so I think it’s not that worst suggestion to be as min near or to have a fire alarm close to the charging place.
```

---
## \#19 Posted by: Andy87 Posted at: 2018-09-24T19:48:46.369Z Reads: 36

```
What’s the difference between bypassing a bms for charge only or balance charge with a hobby charger?
```

---
## \#20 Posted by: b264 Posted at: 2018-09-24T19:49:07.719Z Reads: 33

```
I think the solution for that is to buy batteries already made by professional.  Heavy vibrations make things fail in the most unusual ways that you don't think about ahead of time.
```

---
## \#21 Posted by: b264 Posted at: 2018-09-24T19:53:02.377Z Reads: 34

```
[quote="Andy87, post:19, topic:68993, full:true"]
What’s the difference between bypassing a bms for charge only or balance charge with a hobby charger?
[/quote]

With one, you plug in one barrel plug and forget it
![s-l300%20(17865)|300x300](upload://wDqkg9lNUCw5McEjdlYCno6nn05.jpeg) 

With the other, you take your board apart every time you need to charge it and you can only charge half your board at a time and you're more likely to run the battery all the way down because it's a pain in the neck to charge it, which increases the chances of early battery failure and getting stranded and reduces the amount of time you spend riding the board.  Plus your board can die if you hit one puddle of water.
```

---
## \#22 Posted by: Andy87 Posted at: 2018-09-24T20:02:16.617Z Reads: 31

```
That‘s relative. For sure it’s more easy to just plug a laptop brick charger and good.
But for my mtb for example, i have a easy to open case. I have a dual balance charger, so I can charge two lipos in one.
It’s not a pain in the ass to plug the one more charging plug plus two balance plugs inside of my charger though 😅 and I even can take the lipos out and charge them in a safe lipo charging box.
I think it all just depends on how the lipos integrated into the board.
That’s why I didn’t understood that you said my suggestion with the balance charger is stupid and than suggest to use a bms for charge only.
```

---
## \#23 Posted by: b264 Posted at: 2018-09-24T20:04:02.151Z Reads: 32

```
I guess it's the difference between making a "toy" or a "tool".

You can't really use it as a tool if it doesn't have a BMS

If you just want a big boy toy, that will work fine
```

---
## \#24 Posted by: Jake2k17 Posted at: 2018-09-24T20:05:14.105Z Reads: 30

```
To answer @Andy87 question about which charger is better, I think that for most people, the bms is better, but the imax charger is more fool proof
```

---
## \#25 Posted by: MrDGOrman Posted at: 2018-09-24T20:05:21.124Z Reads: 29

```
This was my logic.

The current setup is 9s which we all seem to confirm on. This setup is LiPo batteries and as you mentioned in another post - I want to get a BMS to avoid having to remove the enclosure all the time to charge them. I think that's pretty fair.

When I get a BMS I'll be getting a e-switch aswell which, to my knowledge, will mean I can get rid of the antispark key altogether. Is this correct?

My theory is to get a 10s (or even a 12s?) BMS and wire it so that the BMS thinks there's 10 (or 12) batteries to charge. If I can do that buy simply leaving wires unplugged (closest to positive) then that's fine, otherwise joining the wires together will surely bring the same effect.

Regardless, it is possible to use a 10s BMS for 9s LiPos. But why would I need to get a second one when I change my battery setup altogether? Could I not remove the connections and join them back up?

I didn't realise this would be so difficult to understand :laughing:. Can you recommend a BMS for me please (10s and 12s)?

Cheers,
Daniel
```

---
## \#26 Posted by: Andy87 Posted at: 2018-09-24T20:06:24.116Z Reads: 26

```
You probably right.
For me it’s also just a hobby 😜
So I guess I see some things from a other point of view than you
```

---
## \#27 Posted by: Jake2k17 Posted at: 2018-09-24T20:06:27.685Z Reads: 26

```
Yes the e switch would get rid of your anti spark. I like the Bestech bms, they are reliable for charging and discharging
```

---
## \#28 Posted by: MrDGOrman Posted at: 2018-09-24T20:07:47.198Z Reads: 27

```
Perfect. There seems to be so many BMS options on the bestech website. Which one should I go with?
```

---
## \#29 Posted by: Jake2k17 Posted at: 2018-09-24T20:08:43.105Z Reads: 27

```
Check out Build Kit Boards, they have a good selection for bestech bms

https://buildkitboards.com/
```

---
## \#30 Posted by: Jake2k17 Posted at: 2018-09-24T20:09:27.578Z Reads: 24

```
By the way, you need to discharge through the bms to use the e-switch
```

---
## \#31 Posted by: MrDGOrman Posted at: 2018-09-24T20:12:11.616Z Reads: 23

```
I just want to have a switch on the outside that I turn on to use the board and then a laptop style plug to out my charger in. I presumed the charge and discharge works through the BMS anyway?
```

---
## \#32 Posted by: b264 Posted at: 2018-09-24T20:12:35.524Z Reads: 24

```
[quote="MrDGOrman, post:25, topic:68993"]
When I get a BMS I’ll be getting a e-switch aswell which, to my knowledge, will mean I can get rid of the antispark key altogether. Is this correct?
[/quote]

Yes, it will replace the loopkey.  You can still bypass a BMS and use the BMS for charging only.  Or, you can use a full high-current BMS like that one you linked and discharge through it.  There are pros and cons to that, I would not.

I'd use:
a BMS for charge only and a loopkey
OR
a BMS for charge only and an antispark switch
```

---
## \#33 Posted by: b264 Posted at: 2018-09-24T20:13:07.132Z Reads: 22

```
[quote="MrDGOrman, post:25, topic:68993"]
My theory is to get a 10s (or even a 12s?) BMS and wire it so that the BMS thinks there’s 10 (or 12) batteries to charge. If I can do that buy simply leaving wires unplugged (closest to positive) then that’s fine, otherwise joining the wires together will surely bring the same effect.
[/quote]

Yes.  Don't join the wires, leave the extra ones unhooked on the most-positive end
```

---
## \#34 Posted by: MrDGOrman Posted at: 2018-09-24T20:14:59.868Z Reads: 24

```
Perfect. So I can get a 12s BMS and still be able to use it with 9s, 10s or anything up to 12s for that matter. 

Why do you suggest not using a BMS for charge and discharge? Surely that's the purpose of them?
```

---
## \#35 Posted by: Jake2k17 Posted at: 2018-09-24T20:16:58.296Z Reads: 26

```
Uhh, I would go with the 10s Lipo bms
```

---
## \#36 Posted by: b264 Posted at: 2018-09-24T20:18:45.730Z Reads: 25

```
[quote="MrDGOrman, post:34, topic:68993"]
So I can get a 12s BMS and still be able to use it with 9s, 10s or anything up to 12s for that matter.
[/quote]

Yes

[quote="MrDGOrman, post:34, topic:68993"]
Why do you suggest not using a BMS for charge and discharge? Surely that’s the purpose of them?
[/quote]

Yes, it is.  But you have a balance to make.  If you go down a big hill with a full battery, and you hit the brakes, in an emergency situation would you rather slightly damage your battery by a tiny overcharge, or cut off the charge to keep the battery perfectly healthy, but leave you with no brakes?  In the choice between battery and face, face wins every time

Also the VESC ESCs have the ability to cut off throttle on a fully-discharged battery but keep brakes and controls working.  The BMS isn't designed to do that, and while it might work under some circumstances, it's not as good and creates a lot of heat in it.

Essentially, the VESC has software to handle those situations better than a generic BMS that cares only about battery health first and foremost whereas the VESC is designed to care about human health first and foremost.

Not using a BMS for discharge has cons too, though.  If you get a short-circuit between the VESC and battery, the BMS will not help prevent a fire...

Also heavy vibration makes things fail in the most unusual ways
```

---
## \#37 Posted by: MrDGOrman Posted at: 2018-09-24T20:50:34.712Z Reads: 22

```
Okay now I'm majorly confused. Of course I would rather have brakes as apposed to none.

My understanding is that charge is coming from the wall to charge the battery pack and discharge is to power the FOCBOX which in turn moves the motor.

I'm getting confused here. My understanding is that I would connect the cells in a 10/12s 4p fashion, connect the BMS to the cells to allow for me to charge via a wall plug. It would then have a FOCBOX connected to it with an e-switch inbetween which acts as the on off switch. The FOCBOX is connected to the motor.

I think I'm starting to misunderstand things. Sorry to appear stupid. Can you explain in a different way?
```

---
## \#38 Posted by: b264 Posted at: 2018-09-24T20:59:31.858Z Reads: 24

```
Charge comes from the wall and the braking system.  When you brake, it dumps the energy into the battery.
```

---
## \#39 Posted by: Jake2k17 Posted at: 2018-09-24T23:15:00.312Z Reads: 24

```
So, this is hard to explain to someone who is just learning all of this stuff, but read this all the way through, Here we go...

The VESC has a setting that when enables regenerative breaking. This means that everytime you brake, the vesc somewhat turns the motor into a generator, and puts small amounts of energy back into the battery. The bms's purpose is to balance all the cells, but also to protect the battery from over charging. What @b264 is saying about the no brakes is true, but highly unlikley. So if you charge your battery to 100%, and then immedietly go down a hill with your brakes on, the vesc is trying to recharge your batteries, and the bms is protecting your cells from over charging, so it disables the regenerative brakes. This mean that you have no brakes (duh). 

Also, you can use your bms in two ways, bypassed and non-bypassed. Bypassed means that you connect the bms only for charging, and that the energy goes straight from the batteries to the vesc when driving. Non-bypassed is the same connection for charging as bypassed, but the energy goes from the batteries through the bms to the vesc when driving. The brakes being disabled would only happen during non-byassed, but like I said, that is very unlikely. What you said above was all correct. If I were you, I would go with the 12s LiPo Bestech BMS from BKB. Hope this wasn't confusing.
```

---
## \#40 Posted by: MrDGOrman Posted at: 2018-09-25T06:09:12.769Z Reads: 22

```
@b264  @Jake2k17

I understand now. I programmed my FOCBOX for regen braking so that's what it's doing already. It seems like something that shouldn't be worried about too much because the likelihood of something going wrong would be slim. If it was high, no one would have these boards.

Okay so I'm going to get a 12s BMS and then do the no connect thing with the wires. I could even buy another zippy battery to bring my LiPo pack up to 12s.

Thanks for all the help,
Daniel
```

---
## \#41 Posted by: MrDGOrman Posted at: 2018-09-25T06:39:41.108Z Reads: 21

```
My next question is antispark. I like the LED push button switch that eskating.eu does but it's an additional product to fit in. The BMS would need to be switched on all the time. Is this okay? Would leaving the BMS on cause issues?

If it were you, would you have an antispark switch inbetween the BMS and FOCBOX or would you just have the normal switch on the BMS as your on/off method?
```

---
## \#42 Posted by: b264 Posted at: 2018-09-25T07:00:21.166Z Reads: 23

```
The BMS should always be on, that is correct.  It's in charge of the battery... except of course the connection you make to the VESC around it (in a "bypassed" system, which I recommend)

What the BMS actually does is connect a dummy load (a resistor) to any cell (or P-group) that's over 4.20V to bring it down to 4.20V

Thus if you charge a whole 10S pack to 42V and keep it there, it will bring all the cells up to 4.2V by bleeding the higher ones so the lower ones get more charge and eventually you have ten times 4.20 and not, say, nine at 4.21V and one at 4.11V for example
```

---
## \#43 Posted by: MrDGOrman Posted at: 2018-09-25T07:51:29.993Z Reads: 22

```
Okay perfect, thank you. I think I've got it all now. Thanks so much for the help!
```

---
