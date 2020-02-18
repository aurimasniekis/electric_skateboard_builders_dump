# First build, still a few questions

### Replies: 36 Views: 1984

## \#1 Posted by: ShakeNBake7000 Posted at: 2017-06-23T11:31:52.247Z Reads: 140

```
so after posting here I got most of my answers but I still have a few questions:
will this mounting kit work by itself? don't I need to buy another part to mount the motor?
the mounting kit:
https://www.banggood.com/Electric-Skateboard-Belt-Motor-Mount-Bracket-Pulley-Screws-For-839097MM-Wheel-p-1105929.html
my trucks and wheels:
http://www.ebay.com/itm/90mm-78a-Neon-Green-Longboard-Wheels-and-Blue-Reverse-Kingpin-Truck-Combo-Set/182587344126?ssPageName=STRK%3AMEBIDX%3AIT&_trksid=p2057872.m2749.l2649
and another question, how do i turn the board on and off? do i have to make the cord loop that starts the board or is there an easier way mabye a button on the esc?
im buying two 3s 8000mAh that i want to connect in series and charge together but the problem is i dont understand what side of the cable goes to what battery and i was told it will ruin the battery if i dont put it correctly.
this is the cable:
https://hobbyking.com/en_us/6s-battery-pack-balance-charge-adapter-lead.html?___store=en_us
and last, do i only need the balance cables connected to the board to charge or do i also need to + and - to be connected? if so, can someone explain what do i do with the  + and -?
sorry for so many questions im just really confused and thanks in advance to anyone thats answers!
```

---
## \#2 Posted by: Challlsss Posted at: 2017-06-23T14:23:34.147Z Reads: 121

```
Hi! You have good questions. Most of them have already been answered in other posts so I'll add a link or two. 
As far as the motor mount... I'd say it looks good. However you know ahead of time that it is not the best way to mount the motor as using grub screws to fasten it to the truck typically isn't enough to keep it in place.

https://www.electric-skateboard.builders/t/how-to-anti-spark-xt-90-loop-key/204

<img src="/uploads/db1493/original/3X/8/9/892c7c5b03ab2b2f893c22e21d71609baf68ea3a.png" width="380" height="500">
```

---
## \#3 Posted by: ShakeNBake7000 Posted at: 2017-06-23T18:20:51.403Z Reads: 102

```
thanks for the reply! so to charge i need to connect both the red and black and the balance cable?
```

---
## \#4 Posted by: Challlsss Posted at: 2017-06-23T18:39:23.496Z Reads: 98

```
The balance connector you have linked above does that for you
```

---
## \#5 Posted by: pjotr47 Posted at: 2017-06-23T19:15:48.585Z Reads: 94

```
Hi, i have ordered the same mount but i am waiting for delivery. If you want i have some 6s parts for selling, they are all new... https://www.electric-skateboard.builders/t/be-seller-charge-adapter-6s-25-2v-4a-2x-lipo-3s-to-6s-adapter-ubec-lipo-alarm/25765
```

---
## \#6 Posted by: ShakeNBake7000 Posted at: 2017-06-24T12:57:20.428Z Reads: 81

```
so all I need to do is connect the balance cable to the charger and charge?
```

---
## \#7 Posted by: gee Posted at: 2017-06-25T00:32:40.553Z Reads: 79

```
Yes, the balance cable should fit in to the side of your balance charger. If you still have question on how to charge it, let me know. I can take pictures. I still don't know why you need the 6s balance charger adapter. Like you trying to charge two batteries in series at the same time? 
BTW you are running a 6s so I don't know if that would be enough to run your motor and your weight. I have 190kV motor and 6s doesn't really get it going. I hook up 3 batteries in series so 9s. And so far it runs smoothly.
```

---
## \#8 Posted by: Challlsss Posted at: 2017-06-26T13:12:45.549Z Reads: 69

```
[quote="gee, post:7, topic:25984"]
I still don't know why you need the 6s balance charger adapter.
[/quote]


I Gatchu **FAM SQUAD** 

<img src="/uploads/db1493/original/3X/d/d/dd253418f289184163999d3a449dd40dc348abce.png" width="690" height="305">

Ok so there is a very simple explanation why you need to balance charge your lipo's / liion cells. It is because you have more than one cell in series. When multiple cells are in series it is very difficult to hook a charger up to the circuit and charge each *individual* cell to its max voltage of 4.2 some odd volts. Because of this we getttt balance charging! Basically As you can see from the image above the balance charger allows the charger to apply voltage and current at different levels along the circuit to balance out any changes that happened while discharging. If you don't balance charge and you have cells in sereies eventually one of them is going to get over charged - over discharged and your battery will fail.

On the other hand.. When you charge in parallel you basically are taking both positive ends of the batteries and both negative ends and sticking them together. As a result (as long as the batteries have the same nominal voltage) they will "push" against eachother and there will be a rush of current and they will automatically balance out as they become one **big** battery. So if you had 3, 1S1P 1000 mAh batteries and put them in series, you'd have a 1S3P, 3000 mAh battery. Be careful with parallel charging however, because if the voltages between the two batteries is too far apart; when you plug them into each other the current to balance them will generate way too much heat.

EDIT* One other thing.. When you balance charge you will want the balance charge cable aaaaand the regular charging wire (thick 10 gauge one) because then the majority of current is running through the thicker wire. (I think I read somewhere that this wasn't necessary but I like to play it safe)
```

---
## \#9 Posted by: ShakeNBake7000 Posted at: 2017-06-26T14:02:17.687Z Reads: 56

```
yes, im connecting two 3s in series

and if ill want to upgrade ill just add another 3s

i connect them in series not in parallel, didnt understand the last part about the thicker cable, can u explain?

can u mabye take a picture of how u connected the charger to the batteries?
```

---
## \#13 Posted by: Challlsss Posted at: 2017-06-26T14:13:30.594Z Reads: 58

```
@ShakeNBake7000
Woah easy there cowboy. Try to keep your thread tidy. Could you please consolidated these four posts into 1?
I posted about parallel just to highlight the differences between it and series. If you read through again it is mostly an explanation for Gee. 
 [quote="ShakeNBake7000, post:11, topic:25984, full:true"]
i connect them in series not in parallel, didnt understand the last part about the thicker cable, can u explain?
[/quote]

The balance wires are really thin. Most balance chargers will have a connection for the charging (thick wire) and a connection for the balancing (thin wire) If you look at the diagram I posted earlier you can see. Balance on top. Main charge wires on bottom. you will use both when you balance charge.

EDIT* if you are trying to get photos of charger and battery configs I urge you to look up previous threads. You will find tons of info readily available from people who have had the same questions as you.
```

---
## \#14 Posted by: ShakeNBake7000 Posted at: 2017-06-26T15:54:11.395Z Reads: 56

```
yeah sorry about that, thanks for the help, ill try to find some pictures
```

---
## \#15 Posted by: ShakeNBake7000 Posted at: 2017-06-26T16:00:36.381Z Reads: 55

```
<img src="/uploads/db1493/original/3X/d/4/d480cd3b812b94b80817183d2724313d9fc1f375.png" width="690" height="388">
hey, i found this picture and it shows exactly what im planning to do but some people said it wont work and some said it will.
can u confirm it will work? ill use xt90's on the - and + cables
```

---
## \#16 Posted by: Challlsss Posted at: 2017-06-26T16:04:25.268Z Reads: 55

```
The balance charging is incorrect (small wires) 
Everything else is fine.
Basically if the batteries were charged it would work, but when you plug it into a charger you will melt the charger almost instantly.
Refer to the image at the beginning of your post for correct balance wire setup. If you compare the two you will see two important differences,
1) which battery has the positive end of balance vs negative
2) how the two balance wires (red and black) in the middle are connected.
```

---
## \#17 Posted by: ShakeNBake7000 Posted at: 2017-06-26T16:21:58.402Z Reads: 47

```
cant understand whats the diffrence between his pic and yours, I wouldn't bother u any more thanks for all the help, its aprecciated
```

---
## \#18 Posted by: Challlsss Posted at: 2017-06-26T16:33:17.649Z Reads: 51

```
Oh no. Lets keep looking at it. This is important stuff. Gimme a sec...
So on the first photo we notice that the pack one positive lead for the main power is the one used as well in the balance charge and the negative lead for the main power is used for balance as well. This is **good**.
<img src="/uploads/db1493/original/3X/7/3/73049aa162a5068a07420b3687f0647d120693a9.png" width="481" height="500">
(forgive my shitty drawing skills)

It the other pic... the "bad" one...
<img src="/uploads/db1493/original/3X/9/5/95a84d7e4c9470130e4c741613841d567acd05c1.png" width="690" height="296">

It is super sloppy but does this help? @ShakeNBake7000
```

---
## \#19 Posted by: ShakeNBake7000 Posted at: 2017-06-26T17:00:55.346Z Reads: 49

```
Oh.. the balance cable has a negative and a positive.. didn't realize..
So to fix the problem on the bottom picture he only needed to switch the balance cables between the batteries? looks so simple now..
Thank you so much for taking the time to explain it in depth it's really aprecciated!
and sorry for bad english it's not my first language (:

EDIT: i forgot one last thing, the antispark loop key goes in the xt90 port thats used for charging? so when i want to turn it on i connect the loop key and when i want to charge it i connect the charger instead of the loop key?
```

---
## \#20 Posted by: Challlsss Posted at: 2017-06-26T17:06:03.779Z Reads: 50

```
Yes. Make sure you really have this locked down before you try to charge your batteries. A good way to practice is to look at other peoples diagrams and see if you can figure out if there is anything wrong. Then see what other people said. If everyone always says the same thing as you then you are good. Not to put pressure on but if you mess it up it gonna cost ya a new battery charger and possibly new batteries too.

In regards to your edit: ***NO!!!*** **If you plug the antispark loop key into the charge port you will *short circuit* the batteries and they will die**

The loop key only goes where the "switch" is
and the charger only goes where the "charge port" is
```

---
## \#21 Posted by: ShakeNBake7000 Posted at: 2017-06-26T17:19:53.989Z Reads: 47

```
lol u just saved me with that, thanks
so i need to make three holes out of the encloser, one for the balance and charging xt90 and one for the anti spark xt90 loop key?
```

---
## \#22 Posted by: Challlsss Posted at: 2017-06-26T18:24:05.400Z Reads: 42

```
Right! and you'll need a way for the phase wires from the VESC to the motor to get through as well
```

---
## \#23 Posted by: ShakeNBake7000 Posted at: 2017-06-26T18:48:25.510Z Reads: 44

```
ill use xt90 for those aswell.
thank you very much for all the help i wouldnt have understood how to charge my skateboard without your help
```

---
## \#24 Posted by: Challlsss Posted at: 2017-06-26T18:49:52.620Z Reads: 41

```
ehhhh you probably won't. There are 3 phase wires
<img src="/uploads/db1493/original/3X/2/2/22cb88cec724f5e7962a5f138cde38a9cd124223.png" width="554" height="500">
```

---
## \#25 Posted by: ShakeNBake7000 Posted at: 2017-06-26T21:15:15.183Z Reads: 39

```
oh yeah i got confused, do i need to buy a connector for those or is it ready to use? im using and esc not a vesc btw
```

---
## \#26 Posted by: gee Posted at: 2017-06-27T00:17:49.197Z Reads: 35

```
Yeah I know you need balance charge for 2+ cells in series. I'm wondering why he needs the 6s balance adapter. Like he's trying to charge two 3s batteries in series? Why not just cut the cost and charge them individually? I have 6 batteries now and I'm charging them individually until I make enough to afford the parallel board and learn how to hook them up. I'm trying to help him as well as learning for my own sake. Thanks for correcting though. 12 years of school and 3 years of college doesn't teach me SHIT. LIke I'm so clueless about electricity that 2 months of researching for my build taught me more.
```

---
## \#27 Posted by: ShakeNBake7000 Posted at: 2017-06-27T00:38:49.092Z Reads: 35

```
how will i go about charging them individually? just courius
```

---
## \#28 Posted by: Challlsss Posted at: 2017-06-27T04:53:49.034Z Reads: 42

```
[quote="gee, post:26, topic:25984"]
12 years of school and 3 years of college doesn't teach me SHIT.
[/quote]

LOL Same. 
@ShakeNBake7000 You would probably be better off just spending the money on a charger. I guess you could get a 4.2V power supply or use some sort of transformer to step down another supply, I mean hell at that point you might be able to make an arduino do it. (It would take years to charge though ;))  Point is, if you charge each cell individually you'd have to plug and unplug the charge to each cell 6 times each time you wanted to fully charge the board. Since a typical charge is going to be 1-2 hours I'd say that that would mean you would be changing which cell would be charging every 15 minutes, 6 times, per charge. I'm not sure it's worth the extra work (especially since one you build it you are going to want to do multiple full rides every day) I actually  go out of my  way to make excuses to ride it... (grocery shopping, drive through food, need to see a view etc)
```

---
## \#29 Posted by: ShakeNBake7000 Posted at: 2017-06-27T11:11:29.096Z Reads: 38

```
lol yeah I think ill find excuses too
about the 3 pin between to motor and the esc do i need to buy connectors for those or do they come ready to connect?
my ESC: 
https://hobbyking.com/en_us/hobbykingr-tm-x-car-beast-series-esc-1-8-scale-150a.html
my Motor:
https://hobbyking.com/en_us/turnigy-aerodrive-sk3-6364-245kv-brushless-outrunner-motor.html
```

---
## \#30 Posted by: gee Posted at: 2017-06-27T12:48:20.463Z Reads: 33

```
hmm it doesn't tell you what kind of connector the esc has so I'm guessing it doesn't have any so you have to solder yourself. The motor has 4 mm bullet connector though.
```

---
## \#31 Posted by: ShakeNBake7000 Posted at: 2017-06-27T13:10:35.947Z Reads: 31

```
so i need to buy those 4mm connectors or just solder the motor and esc cables together?
```

---
## \#32 Posted by: gee Posted at: 2017-06-27T13:14:59.141Z Reads: 30

```
Yeah I don't think you should solder the motor wires to the esc. Other people might say otherwise though. 
If I were you, I'd get the female 4 mm bullet connector and solder them to the esc so later if you change your mind about the motor or the esc you can swap them out.
```

---
## \#33 Posted by: ShakeNBake7000 Posted at: 2017-06-27T13:19:57.575Z Reads: 27

```
can u link me some? I can't find it on hobbyking, is it used for a lot of things? because if it is I can probably buy it here instead of ordering online
```

---
## \#34 Posted by: Challlsss Posted at: 2017-06-27T13:23:41.264Z Reads: 26

```
just go to an rc store with your motor and find the ones that work and buy it there.
```

---
## \#35 Posted by: gee Posted at: 2017-06-27T13:25:20.322Z Reads: 30

```
https://www.amazon.com/Generic-Plated-Bullet-Connector-Battery/dp/B01CJMAMT0/ref=sr_1_10?ie=UTF8&qid=1498569708&sr=8-10&keywords=4mm+bullet+connector
Honestly though spending 8 bucks for these which you gonna use 3 of them is not worth the money. But if you trying cut the cost might as well solder the shit together but get your motor the run the RIGHT direction first.
```

---
## \#36 Posted by: ShakeNBake7000 Posted at: 2017-06-27T13:31:32.671Z Reads: 28

```
yeah i thought that was a better solution but im not sure they will have the connector
ill check and then see what ill do
```

---
## \#37 Posted by: Challlsss Posted at: 2017-06-27T13:34:09.550Z Reads: 28

```
they will have it
trust
```

---
## \#38 Posted by: ShakeNBake7000 Posted at: 2017-06-27T14:04:44.713Z Reads: 27

```
thank you so much for the help guys
```

---
## \#39 Posted by: ShakeNBake7000 Posted at: 2017-06-27T15:58:02.494Z Reads: 27

```
really man, i cant thank you enough, i gave up but u kept explaining until i understood
```

---
