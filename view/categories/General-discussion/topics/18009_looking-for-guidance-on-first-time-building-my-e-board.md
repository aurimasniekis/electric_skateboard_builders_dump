# Looking for guidance, on first time building my e-board

### Replies: 9 Views: 1220

## \#1 Posted by: ciscotory Posted at: 2017-02-21T00:16:22.326Z Reads: 124

```
Hello every one 
recent member in esk8 forms and fist time crating new topic  :grin:  hop it's in the wright place
Ben reading / gathering info for my build, wanted to get your advise and guidance on my planed/aims/setup for this project.. 

i want to build an e-long-board for every day us, going to work or college or just simply buying groceries 
my aim:-
1)  Dual motors long-board, Arduino drive and  remote controllered.
2) is to have reach 50 km/h
 '' I know some of you might say that's extremely fast :fearful: but i would like to experience and feel that speed"
  I'm aware that i wont be always going that fast but still would love to have that option when i have the chance '' and on             papers calculation would be 50 but in real life it wont reach that speed 
  of course safety comes first so Protective gear will be in my list :eyeglasses:
 3) Range wanted to be, i would say about 10 - 20 km '' is that possible or is that reasonable? / can it be more?''

What i have at the moment is the board was on sale booth it at a local store 
drop trough long board 
drop through pairs truck ''i believe''
72mm wheels with ABEC-7 bearings
BRUNOTTI BOBO LONG-BOARD 
https://www.brunotti.com/en/summer/boards/longboard/bobo-longboard-24432.html

This's my list to buy so far '' would this work for what I'm aiming for? ''

1) 2- 2 x 50mm 270KV motor's
2) Caliber 184mm trucks replacing  the pairs trucks that comes with the board
 ''it's hard to find motor mount's that can work with pairs trucks, it's unfortunate and i cant make DIY no access to tools'' 
3) Enertion's Motor Mount '' any recommendations for EU shipping ? avoiding paying Duty  ''
4) Motor Pulley 15t Pulley '' not sure of diameter?  perhaps depends on the motor shaft ''
5) Drive Hub or wheel Pulley 36t 
6) 2x  Arduino Uno board '' or one Arduino can be enough for two motor's ? ''
7) 2x ESC's '' any recommendations ? ''
8) SPACE cell 10s3p lion Battery 
'' not sure if this Battery would work as i got very confused on how to calculate the total power demand by all of the electrical components while reaching power need to my aims  ''
9)  9mm Belt i would say ?
10) RunPlayBack's Sulaco v1 Enclosure
11) I'm sure i need some sort of cables to connect all of the components?

That's all i can think, I need and required to start working 
sorry if i semis to be asking a lot from you guys but i really need your help and guidance on how to approach my desired e-board ..


Thank you all in advanced
looking forward chatting and connecting with all of you :sunglasses:
my salute to all 
Ciscotory
```

---
## \#2 Posted by: sl33py Posted at: 2017-02-21T01:18:33.563Z Reads: 104

```
Welcome Ciscotory!

I would try to stick to 190kv or less if you want ot use a 10s battery.  50 or 63mm

Your ESC needs to be picked before you pick battery.  VESC is my suggested and will handle 10s if you stay below 190/200kv motor (avoiding >60k ERPM).

Enertion mount is really simple and works really well.  I also like the DIYes.  More adjustable angles as a bonus.

I like 14/36 or 14/40 - but since you want speed, you might go with 15/36.  Definitely stick to 8mm motor shafts so you can easily get gears to fit.  I have one 10mm shaft motor and it's a PITA to find gears w/o custom from online places for $$.

Definitely dual 9mm belts or even better dual 12mm (more contact area and less skipping under hard acceleration/braking).

I'm kinda "old school" and would suggest the GT2b over Arduino.  Much more proven, and when going fast - last thing you want is to lose connectivity/control!

know how to solder?  have a decent adjustable soldering iron/station?  making your own custom length cables really helps keep it clean w/o "spaghetti" wiring being a clutter underneath or in your enclosure (also restricts airflow for cooling).

HTH - GL!
```

---
## \#3 Posted by: rpn314 Posted at: 2017-02-21T03:47:30.718Z Reads: 95

```
You're definitely on the right track!
I would second @sl33py: 190kv motors and VESCs to drive them. We're pretty biased towards the VESC around here cause it works pretty well once set up.

I'm not sure I understand what you're planning on doing with the Arduinos, but I think trying to use them will just complicate things. If you were hoping to use them as your remote as @sl33py mentioned, I would caution against that even more, at least on your 1st board. The GT2B (any any of the modifications for it) are the most reliable. If you want something a little different, I think the most I can recommend is the NunchuckRF (what I went with personally).

With your top speed it will really come down to gearing. How steep are the hills around you? There's some tradeoff between top speed and torque (which affects your hill climbing ability and your acceleration). I'd personally recommend that you aim for a bit lower speed and then later on change your gears and possibly belt if you're really craving more. That's just me :)

You're battery should be fine. I _think_ you'll be able to get 10-20km of range with that, but if you have the budget, I'd get a larger parallel count like 10s4p. That will secure that range a little better.
```

---
## \#4 Posted by: ciscotory Posted at: 2017-02-21T21:20:14.613Z Reads: 74

```
[quote="sl33py, post:2, topic:18009"]
12mm
[/quote]

sl33py thank you very very much :+1: you really helped me a lot :ok_hand: 
this's the first time i found out that ESC and VESC are not the same thing :stuck_out_tongue:

If it's not asking to much, I have few more questions :sweat_smile:
 
1) my chose of 2x 50mm 270kv motors's was that an over-overkill  :smile:? 
is it perhaps they require more volt and would drain out the battery fast? and if i'm going to us them is that too much, and  would it required a bigger battery?

2) I forgot to mention that i do have access to 3D printing machine, perhaps i can search and try to make DIY mount
but not sure how it would be durable and last for long time? and i found it takes a long time to design parts.. 

3) I think ill change to your recommendation on pulleys of  14/36 or 14/40, i believe this would give more torque with reasonable speed, and i can change gears to increase speed when ever i want :thumbsup: grat tip thansk.

4) using dual belts would that might cause the belts to tangle over each other when operating, do you know if there are belts that are more wide to increase concoct area?

Thanks again for your help and time 
really appreciate it ..
```

---
## \#5 Posted by: jaykup Posted at: 2017-02-21T21:59:05.915Z Reads: 63

```
1 - Overkill?  No, I actually think you would get equal or better performance with two 6355s 190kv or a big 6374 190kv motor.

2 - [my 3d printed mount experiment](http://www.electric-skateboard.builders/t/just-got-a-3d-printer-what-can-cant-i-print-for-esk8-parts/17991/8)

3 - so there are a few speed calculators out there, but here are some examples:

190kv 10s 16/36 80mm kegels
<img src="/uploads/db1493/original/3X/3/4/34ae7224d29e6c5a768c2d35a79cbde80a5828e5.png" width="474" height="320">

190kv 10s 16/36 73mm wheels
<img src="/uploads/db1493/original/3X/8/2/82f532b275eac70f4bcd3c7b70ac70a4588ce4bf.png" width="448" height="300">

So a single 6355 190kv 10s 16/36 with 80mm+ wheels will give you 50kph (I've personally hit 45kph on a 12s version of this setup while at 70-80% duty cycle, still room to go!)

You might have clearance problems with 14/40 on 72mm wheels - a 40t pulley is around 65mm in diameter so that's getting pretty close to the ground there.  14/40 on 190kv 10s 72mm will only give 38kph, 14/40 on 260kv and 73mm wheels will give you 50kph, but the VESC can't handle the high RPMs.  That's why a lot of guys go for 190kv or lower motors with taller gearing.  It's the same thing really - in the end it's the wattage of the motor that matters and a 63xx will put out more total power than a 50xx motor.

4 - Dual belts, one on each wheel, not together.  9mm wide belts were popular but broke somewhat frequently so a lot of guys switched to 12mm wide htd5 belts and they handle the power nicely.  15mm is standard but two 6355s wont fit side by side on standard 180mm trucks with 15mm belts, so that's where the 12 comes from.

5 - range - I've been averaging 10 watt hours per kilometer, so you can easily hit a 10-20km range with a moderate size battery.  I went 40 kilometers on a full charge last weekend and still had some charge left.
```

---
## \#6 Posted by: ciscotory Posted at: 2017-02-21T22:12:18.256Z Reads: 51

```
rpn314 

Thank you also for the great info and help :v: you guys are the best 
ill give you some info on me i'm 172 cm and 85 kg in wight, in the heavy category :sweat_smile:
regarding how steep are the hills i'm not sure but don't think it would be gradient of more than 15% even a bit less..

i'm differently going to use your tip of aim for bit lower speed and change when desire :wink: :point_left: 
that's a great advice thank you..

If it's not asking to much, I have few more questions for you as well :sweat_smile: 

1) the reason i wanted to you Arduinos because i thought i can fully control my e-board with out using VESC  or ESC as this will reduce electric components, do you think that's possible? 
and to answer your question  yes i want also to us it to connect the Controller receiver  

I've been searching and still looking online for builds with Arduinos or other  micro-controllers like raspberry pi
i believe these micro-controllers have a lot of functions and advantages, for example i want to add LED lights for front and tail lights to my board at a later stages as extra as this could be a possible feature or any fun :wink:

2) can it be possible to increase the board rang to more than 20? and how this could be done ? so to make long rids 
 
Thanks again for your help and time 
really appreciate it .. :pray:
```

---
## \#7 Posted by: sl33py Posted at: 2017-02-21T22:22:13.103Z Reads: 48

```
[quote="ciscotory, post:4, topic:18009"]
first time i found out that ESC and VESC are not the same thing :stuck_out_tongue:
[/quote]
Vedder's ESC = VESC.  An amazing creation and really cool he built this.  As an option to the car ESC's...

[quote="ciscotory, post:4, topic:18009"]
1) my chose of 2x 50mm 270kv motors's was that an over-overkill  :smile:? is it perhaps they require more volt and would drain out the battery fast? and if i'm going to us them is that too much, and  would it required a bigger battery?
[/quote]

Good question.  It's not overkill, but the higher kv won't work well for e-sk8.  You want lower kv if possible.  It's not really about drain and volts - more about limitations of the VESC and it's ERPM limits.  Your motor ERPM needs to stay below 60,000 ERPMs to avoid damaging the DRV chip on the VESC.  So as a general rule you want to stay <200kv - but you can use 270kv motors if that's what you have - it's less ideal, but you'd have to use a lower voltage battery setup (maybe 6s - and possibly up to 8s (running speed calc)).

[quote="ciscotory, post:4, topic:18009"]
2) I forgot to mention that i do have access to 3D printing machine, perhaps i can search and try to make DIY mountbut not sure how it would be durable and last for long time? and i found it takes a long time to design parts..
[/quote]

a 3d printed motor bracket will not work.  Yes i know someone somewhere has gotten one to work... but let's just skip to making one from aluminum/metal, or purchasing one from a vendor or fellow builder here.

I've used 3d printed wheel pulleys... they work pretty well and if you can make your own as they wear - a great option!

[quote="ciscotory, post:4, topic:18009"]
3) I think ill change to your recommendation on pulleys of  14/36 or 14/40, i believe this would give more torque with reasonable speed, and i can change gears to increase speed when ever i want :thumbsup: grat tip thansk.
[/quote]

If you want to gear down, i would go with a lower kv motor first, before lower gears like this.  14/36 or 14/40 should work really well.

[quote="ciscotory, post:4, topic:18009"]
4) using dual belts would that might cause the belts to tangle over each other when operating, do you know if there are belts that are more wide to increase concoct area?
[/quote]

the belts are on each side, so don't cross - no issue with them tangling.  Dual 9mm will work, but i'd suggest dual 12mm.  The kits from both Enertion and DIYes both are 12mm i believe, but please double check.
```

---
## \#8 Posted by: sl33py Posted at: 2017-02-22T00:18:16.194Z Reads: 41

```
[quote="ciscotory, post:6, topic:18009"]
1) the reason i wanted to you Arduinos because i thought i can fully control my e-board with out using VESC  or ESC as this will reduce electric components, do you think that's possible? and to answer your question  yes i want also to us it to connect the Controller receiver
[/quote]

I would still caution you to stick to an ultra-reliable GT2b or similar.  You can them move into 3d printed enclosure pretty easily (I have an old writeup you can look at to see complexity - not too bad):
http://www.electric-skateboard.builders/t/how-to-hack-build-compact-controller-using-gt-2b-badwolf-v2-enclosure/114

When you are going 30-50kmh you do not want to have any control issues (loss of acceleration/braking), because at those speeds your reaction times are so fast and any error could be a serious injury (wear protective gear appropriate for the speed you intend to go).

[quote="ciscotory, post:6, topic:18009"]
i want to add LED lights for front and tail lights to my board at a later stages as extra as this could be a possible feature or any fun :wink:
[/quote]
Easy to add on.  Several folks have LED's including some addressable LEDs.  Do some searching and you'll find some options.


[quote="ciscotory, post:6, topic:18009"]
2) can it be possible to increase the board rang to more than 20? and how this could be done ? so to make long rids
[/quote]

the easiest way to increase range is add capacity (more battery Wh).  A general rule of thumb - for every 10Wh you will get 1km.  To get Wh, take your Ah x voltage = Wh.  Easy math example - 10s (36v) 5000mAh = 5 * 36 = 180Wh.  /10 = 18km

I had to check the SPACE cell specs, but it looks like 270Wh / 10 (every 10 = 1km) = 27km.  Now this is an estimate - and hills, or a heavier rider, or even hard acceleration will decrease your range.  Also kicking to start, not accelerating super hard, etc - can all extend it slightly too.

HTH - GL!
```

---
## \#9 Posted by: JeanDublin Posted at: 2018-04-26T15:19:00.839Z Reads: 11

```
@ciscotory I'm very impressed with the way you all guys build your own electric skateboards, it is definitely the best way to customise it to your needs :slight_smile:

Off-Topic: Will you be joining the meetup in Dublin for a ride the 13th of May or any other future rides? Check out my profile for the link :slight_smile:
```

---
