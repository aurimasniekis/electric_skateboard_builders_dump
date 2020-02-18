# Beginners Guide to building your own Electric Skateboard Drivetrain

### Replies: 57 Views: 98559

## \#1 Posted by: onloop Posted at: 2015-07-21T09:08:58.858Z Reads: 3285

```
> ## [NEW: 2019 Electric Skateboard Buyers Guide](http://www.enertionboards.com/ultimate-industry-insider-tips-buying-electric-skateboard-2017-buyer-guide-how/)

> ## [NEW ESK8 MOTOR TECH 2019: Liquid Cooled Hub Motors](https://www.youtube.com/watch?v=1l6hSPpUl6I)


Building your own electric skateboard is extremely enjoyable & also very challenging. One of the most complicated & very important elements of building a quality, high performance eSk8 at home is the Drivetrain or sometimes referred to as the Propulsion System or Powertrain

The **Drivetrain** of a an electric skateboard is the group of components that delivers power from the motor to the wheels. This excludes the motor that generates the power. So basically the Drivetrain of an electric skateboard consists of four key parts.
> 1. The Motor Pulley
> 2. The Wheel Pulley 
> 3. The Drive Belt
> 4. The Motor Mounting Plate and Truck Clamping Parts, referred to as the Motor Mount 

<img src='/uploads/db1493/original/1X/0597d0347b71e8b14b5a41e6d15064b1350e924c.jpg'>

The four parts listed above when grouped together with the motor, which provides the power or torque to move the Drivetrain components, is technically called the Powertrain Or Propulsion system. The motors with the best power to weight ratio for building an electric skateboard are Brushless Outrunners, that's why they use them on RC Planes! 

<img src='/uploads/db1493/original/1X/cc3af66ea0b9ff16af390ea7c0794166a1efb24c.jpg'>

Knowing the Revolutions Per Minute (RPM) of a Brushless Outrunner motor is critical to designing your Drivetrain, I will explain how to calculate that further down. Without knowing how fast your motor spins you cannot determine the required Gearing Reduction Ratio and therefore cannot build a system to reach your desired top speed. As the RPM of your motor is determined by the voltage being supplied from the battery we must also discuss the battery in this guide. Fortunately most motors have the kV (and RPM) rating noted and for this guide that is enough info to make our propulsion system.

We must also know the Diameter of the wheel you intend to use, With the diameter we can calculate the circumference of the wheel. Or you could just measure the circumference... ***C=2πr blah blah..***. This tells us the distance travelled per revolution. 

<img src='/uploads/db1493/original/1X/4ba664957589dda1f0283021be576920ee792cf8.gif'>
<img src='/uploads/db1493/original/1X/541911d5fa571fb3006b4d9da121297c7c5130b7.jpg'>


----------


!!! STOP !!! This is getting way too technical! OK so I promise no Algebra or Maths required.
---------------------------------------

--------------------------------------


----------



So now we know about the Six Key elements of a propulsion system that must work together to give you the performance you desire.
**Motor Pulley, Wheel Pulley, Drive Belt, Motor, Battery & Wheels**

Out of these six parts there are five variables that need to be determined so you can design & build your Drivetrain.
> 1. Gearing Reduction Ratio.
> 2. Motor KV.
> 3. Battery Voltage.
> 4. Wheel diameter.
> 5. Desired Top speed.

The top four variables are all related and if one is changed the top speed of your propulsion system will also change. That is why its is generally easiest to determine your desired top speed then work backwards to determine the others.


----------

> *SPEED KILLS - YOUR ELECTRONICS*
> -----------

> ***Now lets just be realistic for a minute!** How fast do you really want to travel on your powered-popsicle-stick? My balls a fairly large & I have bombed some narly hills in my time, but on the flats, in a suburban street, where shit can just appear out of nowhere, I start to get scared around 50kms/h. Or about 31mph - At this speed you are travelling at 13.8 meters every second. So I think this should be your absolute maximum for safety & longevity of components.*

> *But It is all about perspective... take for example if you ever get to ride on a race track that is open and smooth without unexpected obstacles appearing from behind cars 50 might seem a little slow now. If you want to go faster than this it becomes much more complicated to build a reliable system and probably needs to be discussed in a separate thread.* 

> *Personally I aim for about 45km/h which tends to be about 41km/h in the real world due to losses & resistance and gives you plenty of torque when you have a dual drive, generally speaking lower top speed = more torque.*


----------


So you want to travel at 45km/h?
----------------------------

Good choice! Now lets work out how to make this happen. I will assume you don't own any parts to make your electric skateboard. I will also assume your are on a tight budget as was I when I built my first eboard.

**The best thing to do is eliminate some of the variables! - Time to go shopping!** 
I suggest buying the wheels, battery and motor first. This will make it easier to calculate the other variables..

**Wheels** 
As you know when it comes to wheels it is the diameter that is important. Most commonly people use wheels between 80mm & 90mm diameter. 83mm Diameter is very common, mainly because you can buy nice wheels that have a hollow core that is perfect for passing bolts through & securing the wheel pulley. Like these wheels.

<img src='/uploads/db1493/original/1X/9e905bc4f7c518a0601878e25eba4aa0a1d70ff4.jpg'>
<img src='/uploads/db1493/original/1X/91ee38249289381d70748bcf82cba0cfa61a0952.jpg'>

You can go bigger or smaller wheels, however if you go too far outside this diameter range you will encounter some constraints that will make the system more expensive, more difficult to build or reduce performance. 

For example; **The bigger** you go in wheel diameter, without changing the drivetrain, the more your top speed increases but that is at the expense of torque. Lower torque output is not great, you want as much torque as possible. So if you must increase speed the best way is to increase voltage as the torque stays the same. Increasing the wheel diameter or increasing motor pulley increases speed and also increases current draw. If you must have bigger wheels or higher top speed you must design the drive train specifically for it. 

**The smaller** you go in wheel diameter, without changing the drivetrain, the lower the top speed & the more torque you get! But there is a limit of how small you can go. Mostly it has to do with ground clearance and pulley diameter limitations. You need to be able to fit batteries & motors under the deck. If the wheel is small the wheel pulley also must get smaller, because if it doesn't it will get damaged from contacting the ground. But you can't just keep making the wheel pulley smaller as this reduces the number of teeth & the reduction ratio you can achieve between the drive & driven pulleys.


----------


***

> *QUICK NOTE ABOUT PULLEY TEETH PITCH* 
> ------------------
> *There is a way to have a smaller pulley & also maintain high reduction ratios. The most common tooth pitch for electric skateboards is 5mm Pitch. Tooth pitch is the measurement between two teeth. So if I had a pulley with just 10 teeth at 5mm pitch the circumference would be 50mm. If I had a pulley with 10 teeth at 3mm pitch the circumference would be just 30mm. So what this means is you can use a smaller pitch & increase the number of teeth and have a pulley that is actually smaller in circumference. So I could have a 15 teeth pulley at 3mm pitch with 45mm circumference. This is advantagous as you can have much larger reduction ratios and have the pulleys fit onto a smaller wheel. But there is a trade off! the smaller teeth can't transfer the same amount of torque as the big teeth so you can get belt slipping issue. Running with 5mm pitch wheel pulley and keeping the wheel diameter at 83mm is enough to ensure you get good reduction ratio & good ground clearance, the maximum number of teeth I recommend for the wheel pulley on an 83mm wheel is 36 teeth. As the amount of teeth increases so does the diameter of the pulley making it closer to hitting the ground which is bad.*
> ***


----------

**Battery Voltage** 
The battery is a fairly easy choice, it is often determined simply by your budget, the more you spend the more watt hours they tend to offer. It will be no less then 6S and max of 12S (so lets say a range of 24 to 48 volts for simplicity). For this exercise lets say you go with 6S (24V) 
*If you want to read more about choosing a battery check this [Guide about battery 'C' rating][1]*


**Motor kV Rating**
The motor purchase is important. Get it wrong and it will be a problem that you can't easily fix. You can buy wheels & pulleys cheaper than you can buy motors, what I mean is you are better off experimenting by changing out some pulleys then buying a stack of motors to determine what one gives you the preferred balance of torque & speed.
You generally need to buy a motor between 200kV & 300kV but this is not always true. Remember the wheel diameter, battery voltage & motor kV all work together to determine the top speed you can reach. So today lets go with 245kV, this a fairly common rating and readily available from hobby shops. 


----------


> **Now we know the Wheel size, Battery Voltage, Motor kV rating & Top speed.** 
> 83mm Wheel Diameter
> 245Kv Motor 
> 6S Battery (24v for simplicity)
> 45km/h


----------


 
**With this information now you can more easily calculate your pulley sizes and determine the final reduction ratio.** As we want to achieve a top speed of 45km/h we can define the last variable, the gearing reduction ratio, to get the desired top speed we want. 

There are some important constraints in drivetrain design, when using pulleys & belts, that must be carefully considered. Firstly there is a minimum amount of teeth you should have engaged between the pulley & the belt. It is called teeth-in-mesh and you should have 6 teeth or more in mesh if you want to achieve the maximum torque transfer rates specified. Your ability to transfer maximum torque will be diminished if you have less than 6 teeth engaged. So it can still work just not to its full potential, so maybe the belt will skip over some teeth.


----------


> 15 to 36 teeth is the ideal configuration to achieve maximum torque transfer when using 5mm pitch pulleys
> -----------------------------------------


----------


Second constraint is your center distance 'C', it is best to have the shortest possible center distance. A shorter 'C' means less leveraging forces being applied onto the motor mounting hardware, it can help to reduce vibrations and minimizes the span of the belt. Basically the shorter it is the less chance the mount will flex, warp, bend or snap which is important when you are frequently accelerating & braking hard. 

However you cannot make it too short because you also need your motor to have some clearance from the truck hanger so you can make a turn. It is also worth noting that the longer your center distance the more the belt will wrap around the pulleys so it can actually result in more teeth in mesh, but it is probably better to keep your center distance short and go with a larger pulley to obtain more teeth in mesh. 

  
<img src='/uploads/db1493/original/1X/e26526eaf9426fd8ce029c6debf658f99d1b200d.jpg'>


**I recommend something around 60-70mm Center Distance. It's short & also offers good clearance for motors up to 63mm barrel diameter.** However If you wanted the motor to be mounted out the back of your electric skateboard you will need a longer center distance to give the motor additional clearance from the baseplate & pivot cup.


<img src="/uploads/db1493/original/1X/59de04e0cd2b857f5206610037eaac32e445d2aa.jpg" width="499" height="407"> 

You must also design your motor mount with a belt tensioning system, a method to increase or decrease the center distance, this is also useful if you like to change your motor pulley to modify performance. If you install a larger pulley to increase top speed, you want to be able to use the same belt, so you will need to be able to decrease/increase centrer distance enough to accommodate the size of your motor pulleys. With a set of motor pulleys you can fine tune your performance quickly & easily with very little cost.

<img src='/uploads/db1493/original/1X/7465408a6322c78f81ce808444e320525c8791be.jpg'>


When it comes time to choosing the pulley sizes for your system the easiest way to make the calculations is to use the [CENTER DISTANCE DESIGNER][2] You can enter the variables such as, Pulley teeth, Center Distance & desired Reduction ratio.
<img src="/uploads/db1493/original/1X/d8cab9d593fb8dc6b4702c8335fe4a599a0a8d1e.jpg" width="690" height="425"> 



> **HOT TIP:** The general theory of efficient drive train design is to aim for the highest possible reduction ratio, whilst keeping the motor in the 8000 - 9000rpm range where the motor losses are at minimum. 
So the most efficient propulsion system on paper that would work within the constraints of an electric skateboard would look something like this
> Drive Pulley: 17 teeth **3mm Pitch**
> Driven Pulley: 60 teeth **3mm Pitch**
> Battery Voltage (V): 42.0 V
> Motor Rounds per Voltage (kV): 215 kv
> Tire Diameter: 3.25inch (83mm)
> Final Reduction Ratio: 3.5:1 
> Motor rpms: 9 030 rpm
> Top Speed: 39.74 km/h (24.74 mph)
>
>This setup above is using a **3mm pitch pulleys & belt**, you would need to use a 15mm wide belt as a minimum to transfer the torque. However in real world testing under braking load this Drivetrain design will possibly skip/jump teeth as it is at the limit of its torque transfer capabilities. This can lead to reduced service life of the belts, Meaning ya' belts get shredded! On dual drive this system it can work slightly better, but only if the rider is under <70kg. Any heavier and the braking torque load is to high for the belts. 

**So the moral of the story is sometimes the most efficient build on paper is not actually the best choice in the real world, in this case I would prefer to lose some efficiency on paper to ensure drive train reliability is better. So for me I am sticking with 5mm pitch**


<img src='/uploads/db1493/original/1X/775a5095295f88dcd2ba049c87f33d8e75e7beab.jpg'>

----------


----------

But what if you need to change something? Different wheel sizes? Different Battery? How do I calculate everything together?
------------------------------------------------------------------------


What you need is a calculator that you type everything into & it spits out your answer! Well fortunately they exist. **So as promised there will be no Algebra!**

I suggest this app for android, its called [CalcRC][3] it's also available on your [PC][4]

Basically you enter your motor pulley teeth, wheel pulley teeth, battery voltage & Motor kV and it spits out your speed. 

**As you can see below the parts we chose only got our top speed to 38km/h**  :sob:


<img src="/uploads/db1493/original/1X/acb143bc2b667ae2d1e4224a27d638ddf80e972a.jpg" width="326" height="500"> 


----------


So your home work for the day is to reply in this thread explaining what you would do to increase your speed to 45km/h
------------------------------------------------------------------------


----------


**REMEMBER THESE KEY POINTS**

 - KEEP REDUCTION RATIO AS HIGH AS POSSIBLE
 - HIGH SPEEDS (OVER 50KM/H) EQUALS HIGH CURRENT DRAW & CAN DAMAGE ELECTRONICS
 - DUAL MOTORS = MORE TORQUE NOT MORE SPEED
 - HIGHER VOLTAGE IS ALWAYS BETTER

  [1]: http://www.electric-skateboard.builders/t/what-is-battery-c-rating-is-it-important-for-electric-skateboards/36
  [2]: https://sdp-si.com/eStore/CenterDistanceDesigner
  [3]: https://play.google.com/store/apps/details?id=cz.koubovo.calcRC.app&hl=en
  [4]: http://www.calcrc.com/
```

---
## \#2 Posted by: onloop Posted at: 2016-07-20T23:40:29.818Z Reads: 2015

```
I made a new video with a summary of all this information to further help people looking to build their own Esk8

https://www.youtube.com/watch?v=Ficvq9aLi2Q
```

---
## \#3 Posted by: Photorph Posted at: 2016-07-21T02:52:18.092Z Reads: 1883

```
Really appreciate what you are doing for the community!  Great info.  Hopefully it cuts down on your emails that ask silly questions.
```

---
## \#4 Posted by: onloop Posted at: 2016-07-21T03:08:11.107Z Reads: 1774

```
thanks mate!
```

---
## \#5 Posted by: PLEB Posted at: 2016-07-23T05:23:15.819Z Reads: 1669

```
Great video. Thanks for the info
```

---
## \#6 Posted by: Djupex Posted at: 2016-07-30T14:13:16.376Z Reads: 1573

```
Great video! I got one question Jason.
The motor pulley on one of my motors on the raptor isnt rotating smoothly and the belts not too tight. Therefore I wanted to fix it by taking the wheel and wheel pulley off and then disassembling the motor pulley I guess.
As I took the wheel off I felt something was loose in between the pulley and wheel (dont know the english word for it but its like the gapcloser I think lol.
Here comes the question: How do I get the damn pulley out of the wheel haha? 
I dont want to use brute force if there is an easy way, I am always over cautious because I didnt build an eskate yet.
Thank you or anyone else that can help out
```

---
## \#7 Posted by: onloop Posted at: 2016-07-30T14:30:07.826Z Reads: 1375

```
Are you talking about the pulley which is inserted into wheel?  

Is it the pulley version made from blue nylon?

The best way to get it out is knock if from to opposite side.
```

---
## \#8 Posted by: makevoid Posted at: 2016-07-30T14:37:17.375Z Reads: 1333

```
[quote="Djupex, post:6, topic:53"]
How do I get the damn pulley out of the wheel haha?
[/quote]

you should be able to push it out from the spaces in the wheel with something that fits in there and let you apply some force, it shouldnt require much force

Also it's normal that the motor itself has some resistance because of the magnets so that's completely normal. 

Instead to tighten the belt you need to loosen the three small bolt/nuts on the motor mounts, push the motor out and then re-tighten the three nuts ( Jason has a video where he shows how to do it https://youtu.be/J40FfVTBxVc?t=21m0s ). Don't tension it too much too, that can wear the belt and shorten your range because of the friction.

But before doing any of this check out belt alignment, see if its clearly off the wheel pulley or rubbing too much on one side (flange) of the motor pulley.

Anyway I think the best way is to post a short video (upload it on youtube unlisted) where you rotate the wheel/motor slowly recording from various angles.

edit: oops, I was too slow/late in writing this reply :)
```

---
## \#9 Posted by: Djupex Posted at: 2016-07-30T14:38:35.738Z Reads: 1137

```
Yeah it is and I tried knocking on it but it is stuck soo hard in there.
Thanks for the quick answer, Ill figure it out
```

---
## \#10 Posted by: Djupex Posted at: 2016-07-30T14:39:00.744Z Reads: 1109

```
Thanks men, needed that link and info for tightening the belt.
Video coming.
```

---
## \#11 Posted by: onloop Posted at: 2016-07-30T14:43:15.557Z Reads: 1106

```
Be careful not to over tighten the belt. 

When turning the wheel with hand you shouldn't be able to feel a difference between belt on or belt off.

There is a point during tightening at which you can feel the resistance in the wheel start to change. Just here is the correct tightness.  No more or less.
```

---
## \#12 Posted by: Djupex Posted at: 2016-07-30T15:07:31.854Z Reads: 1101

```
<img src="/uploads/db1493/original/2X/e/e5cb46aaea94d3c241e36fc1790715e41961b140.jpeg" width="375" height="500">
<img src="/uploads/db1493/original/2X/e/e08ca10726a942848d489ff121353abe85ff854a.jpeg" width="666" height="500">
<img src="/uploads/db1493/original/2X/9/996a691e00660df895a1c65736a1bc4a2f14ccb5.jpeg" width="375" height="500">
Alright!
Forget what I wrote before, I think I fixed it, one side might still be a bit too loose.
Question 1: Is the belt standing too far off of the wheel pulley?
Question 2: Arent the motors too close too each other?
Thanks!

EDIT: The video helped out a lot! I guess the video answered question #1 too, I just have to shift it a little bit
```

---
## \#13 Posted by: onloop Posted at: 2016-07-31T00:02:06.733Z Reads: 988

```

the motors look like they are touching, and your left side motor mount looks like it has shifted. Time for you to do some basic maintenance, perfect motor alignment is very important.....
```

---
## \#14 Posted by: ZeVinner Posted at: 2016-08-11T00:20:52.556Z Reads: 975

```
I'm using motors that have 10mm diameter shafts. The pulleys have 15mm spacers going around its 10mm bore (the hump on one side). I ordered enertion's motor mounts and was wondering if I would be able to make its center hole (where the motor shaft goes) on the carbon fiber motor plate any bigger by using a power drill. The current center hole diameter is 16mm, that only provides 0.05 mm clearance for the pulley to spin which is why I'm concerned.
```

---
## \#15 Posted by: Tdunn Posted at: 2016-09-30T14:56:42.290Z Reads: 874

```
What program do you use to open the free enertion open source mount
```

---
## \#16 Posted by: JLabs Posted at: 2016-09-30T15:34:40.516Z Reads: 867

```
On windows you use FreeCad and then export it to your liking.
```

---
## \#17 Posted by: Tdunn Posted at: 2016-09-30T16:00:33.681Z Reads: 878

```
How about for mac??
```

---
## \#18 Posted by: lox897 Posted at: 2016-10-01T02:40:43.087Z Reads: 875

```
You could download a free trial of fusion 360 or use autodesk 123D.
```

---
## \#19 Posted by: Kelan Posted at: 2017-01-08T14:18:24.437Z Reads: 808

```
Wouldn't something like this: http://www.ebay.co.uk/itm/DIY-Sprocket-Chain-Wheel-for-Electric-Longboard-8044-Skateboard-Repalcement-Part-/371827942388?hash=item5692ac23f4:g:aokAAOSwUKxYZ1sw

be more secure and have less chance of coming loose and also provide more rotational force to the wheels?
```

---
## \#20 Posted by: OskarCastrone Posted at: 2017-01-12T23:03:59.681Z Reads: 789

```
I have actually always wanted to try a chain system! Nice find! 
Belts works great as well though. I dont know if there is any downsides of using a chain system. Maybe you should make a thread about it
```

---
## \#21 Posted by: ewalks6 Posted at: 2017-01-12T23:53:29.602Z Reads: 732

```
I think chain is louder... I've never used it so if someone could chime in that has to confirm if that's true.
```

---
## \#22 Posted by: mmaner Posted at: 2017-01-13T01:51:12.645Z Reads: 705

```
I actually ordered one of those exact kits today, just wanted to try it out. I'll post back now it does.
```

---
## \#23 Posted by: Kelan Posted at: 2017-01-22T17:32:36.357Z Reads: 679

```
Any news with the sprocket drive chain?
```

---
## \#24 Posted by: mmaner Posted at: 2017-01-22T18:55:34.274Z Reads: 673

```
Not yet, they had stock issues and it just shipped saturday.  Ill update when I receive it.
```

---
## \#25 Posted by: OskarCastrone Posted at: 2017-01-26T15:56:04.799Z Reads: 676

```
Looking forward to it! :D
```

---
## \#26 Posted by: ciscotory Posted at: 2017-01-27T22:27:18.035Z Reads: 695

```
Hi there
Onloop thanks very much for detailed info, it gave me a good view on how things work :+1:

i would like to participate on how to increase the speed to 45km/h for that example
'' please correct me if i'm wrong as i'm new to all of the as well, i've ben reading you post all day :) ''
perhaps either 

changing the wheels size from 83mm to 87mm would incrase the speed..
or changing battery voltage from 24 to 42 if possible.
or using a 17 theeth pulley instead ofof 15theeth  
'' not sure if the diamater of these pulleys are that much of a diffrent '' 

quistion: if using a dual motor, how would you calcuate the voltage, is it simply adding both voltage or theres a diffretn way?

finaly i have a question if you could help me :)
i'm planning and preparing to build a back mounted dual motor long board, whit a slightly higher speed than your example, i also want to use circuit board like arduino for controlling the motors and other things making the board more light, less 
components and having many usable functions, is it possible to just use arduino for each motor and other stuff  or there , are more electronic part need to be used for a complete electric skateboard?       
thanks :+1:
```

---
## \#27 Posted by: Kubbur Posted at: 2017-05-06T16:44:53.105Z Reads: 558

```
But how do you calculate torque regarding all this
```

---
## \#28 Posted by: agent Posted at: 2017-06-05T01:40:43.549Z Reads: 555

```
Hey Guys i have made a electric skateboard using a 400kv prop drive motor by Turnigy,, it has 60A rating and  the drive train has 12- 36 Tooth pulley. and i have used it to reach speeds of 25kmph. i am not very good skateboard rider but i will try to push it to  max speed later.
It pushes my friend ahead who weighs 90kg From full stop.. but takes about 3 to 5 seconds to reach the 5kmph speed after which motor can move without much resistance..
My question is:
Will a 60kg person be able to go up a slope with elevation of 10degree?
```

---
## \#29 Posted by: briman05 Posted at: 2017-06-13T17:53:37.224Z Reads: 524

```
Where do you guys get your motors now that Enertion is not selling pretty much any parts now?
```

---
## \#30 Posted by: Dogman1247 Posted at: 2017-06-22T06:31:31.288Z Reads: 510

```
Love your videos watched literally all of them! So helpful and explain things in basic terms for us noobs,

I want to build a setup that will go 55kph or 34mph

Budget is no issues, money is no object, just want to build the best, Really love the new Evolve GTX would love to clone that board basically.

Wondering what parts kit I should buy for this, wondering motor and battery voltage I should run at, would love to use some wider than normal wheels if possible
```

---
## \#31 Posted by: Shahar9320 Posted at: 2017-07-01T17:42:52.284Z Reads: 469

```
hi jason , im new here to the esk8 community... can i have your opinion of my board? its mono drive 6374 190kv, 12s 18650 battery , 13/36 ratio, 83mm wheels. thank you so much and anyone who could also share their opinion please it would be much appreciated
```

---
## \#32 Posted by: memesupreme Posted at: 2017-07-02T08:30:11.580Z Reads: 459

```
that is literally my first build except with a little bit more speed due to higher battery voltage, I had to change my 83mm to 97 though to suit my roads which just shredded my 83s up, electronically though Id prefer your board over evolve or boosted ect
```

---
## \#33 Posted by: Shahar9320 Posted at: 2017-07-02T09:10:53.176Z Reads: 440

```
That's awesome to here! Didn't the 97 make the speed too fast? Do you recommend that in the future if the 83s won't work for me and I end up getting the 97s to change the gearing to 13/40?
```

---
## \#34 Posted by: Shahar9320 Posted at: 2017-07-02T13:14:56.355Z Reads: 429

```
To hear ** lol sorry
```

---
## \#35 Posted by: memesupreme Posted at: 2017-07-03T06:34:17.536Z Reads: 420

```
on paper the 97s would take the board 52km/h but in real world conditions it didn't have enough torque to fight the wind resistance so it never got over 47 for me. I think depending on how you ride and the terrain your wheels may last a lot longer than mine, I kinda murdered my wheels, but yeah that gearing would work nicely with 97s :ok_hand:
```

---
## \#36 Posted by: Shahar9320 Posted at: 2017-07-05T08:06:13.677Z Reads: 416

```
hi guys . because of shipping problems i could only get a 10s battery. (10s3p..)
would this setup still be good with 13/36? this really sucks but i guess i will still get 35 km/h.
```

---
## \#37 Posted by: memesupreme Posted at: 2017-07-05T08:13:18.785Z Reads: 423

```
shame, I currently use a 10s 3p space cell and I wouldn't mind a bit more power though. with 97mm wheels and that gearing ratio you can see about 45kmh which is nice, about the same amount of torque as a raptor mono I reckon, with 83 mm wheels itll be a bit slower but itll have way more torque
```

---
## \#38 Posted by: Shahar9320 Posted at: 2017-07-05T08:19:34.524Z Reads: 421

```
i would've bought a 90mm wheel set but the crapy service from diyes thought it would be appropriate to tell me they cant ship the battery after everything already arrived
```

---
## \#39 Posted by: memesupreme Posted at: 2017-07-05T08:24:15.110Z Reads: 432

```
egh, only stuff I've bought from them were mechanical parts like trucks and mounts, yeah 90 mm wheels seem like a good medium between 83 and 97, actually its exactly in between aha, there are other people on this forum who could possibly make and custom battery for you but I'm not sure how theyd go about shipping
```

---
## \#40 Posted by: Shahar9320 Posted at: 2017-07-05T08:37:15.698Z Reads: 430

```
Yea my problem is only shipping to here.. even hobby king couldn't
```

---
## \#41 Posted by: Smit Posted at: 2017-08-06T22:22:31.656Z Reads: 378

```
when I ride mine the belt tension keeps Coming lose does anyone know what could be the issue?
```

---
## \#42 Posted by: Smit Posted at: 2017-08-06T22:26:53.941Z Reads: 394

```
The belt only gets lose when I get on it, but when I tight the belt again and let it free ride without me being on it the belt doesn't get lose.
```

---
## \#43 Posted by: willpark16 Posted at: 2017-08-06T23:08:21.605Z Reads: 392

```
Motor mount isn't tightened or its moving or one of ur pulleys is moving
```

---
## \#44 Posted by: WARMAN Posted at: 2017-11-02T00:42:54.091Z Reads: 335

```
Just knocking about the forum researching 3mm pitch on 15mm pulleys and came across this goldmine! loads of in depth information,must have taken ages to write up..good work! @onloop
```

---
## \#45 Posted by: chuttney1 Posted at: 2017-11-02T05:39:00.195Z Reads: 332

```
I use 3mm pitch pulley with a 149 kV motor. I have stripped my belts using a 48:18 tooth ratio, but not at 48:32 ratio.
```

---
## \#47 Posted by: mynamesmatt Posted at: 2018-03-04T10:38:32.051Z Reads: 272

```
Hobbyking.com 
The sk3 models are quite popular for esk8
```

---
## \#48 Posted by: caffienatedinsanity Posted at: 2018-05-07T15:24:23.768Z Reads: 231

```
I know that this one is a basic guide but do you have a more technical version or know where I can find one?
```

---
## \#49 Posted by: Okami Posted at: 2018-05-07T19:16:17.834Z Reads: 227

```
How more technical? I think youtube videos also might be a good start.. or just lots of reading on forum..
```

---
## \#50 Posted by: caffienatedinsanity Posted at: 2018-05-07T19:21:46.019Z Reads: 226

```
I was looking for the math that he was talking about but I found it now thanks.
```

---
## \#51 Posted by: tex Posted at: 2018-07-22T15:55:16.218Z Reads: 187

```
Great video, really thanks for all the informations ;-)
```

---
## \#52 Posted by: ZaneKF Posted at: 2019-04-16T14:16:59.776Z Reads: 81

```
Thanks for sharing
```

---
## \#53 Posted by: Kingdom421 Posted at: 2019-04-16T15:03:39.966Z Reads: 81

```
@Kelan ok I bought those but the chain is too short where can I get a longer chain
```

---
## \#54 Posted by: thurbolt Posted at: 2019-06-14T08:02:08.763Z Reads: 60

```
Thanks for the animated info, there is a real effort here
```

---
## \#55 Posted by: Brad99 Posted at: 2019-07-19T22:50:44.207Z Reads: 49

```
![idler|375x500](upload://1iTlOVm966zGgs1KD2fesdJgKlE.jpeg) 

You just just send it and build your own.
```

---
## \#56 Posted by: Briholland83 Posted at: 2019-11-24T16:53:48.658Z Reads: 20

```
Man, after reading all that, I’m totally glad I already decided to build all of my boards with the Torque Boards 90kvdirect drive kits haha. I get it though. I’m a gear head.  I just like everything smooth and clean on the board.  I’ll try the belt thing sometime, but my first deck is definitely gonna be the integrated motors haha. Gonna do 110mm wheels I think. Mostly flatland in boston.  

Does anyone have any expuwith the Torque Boards parts?  The build quality and machining seems damn nice.
```

---
## \#57 Posted by: Tampaesk8er Posted at: 2019-11-24T17:10:25.183Z Reads: 22

```
TB products are top notch and customer service is great.
```

---
## \#58 Posted by: Briholland83 Posted at: 2019-11-24T17:24:54.642Z Reads: 23

```
^ just what I wanted to hear. I think this board I’m doomg is gonna be bad ass. I’m sorta modeling it after the M1 with the lights flushed into the corners.  I’m also gonna have working brake lights and high and low beam projector LED headlights made from motorcycle fog lights that I’ll control from my Apple Watch, or if a remote has aux functions. My cnc can cut all the nice little pockets and drill tunnels for wiring. I’ll 3d print a little removable door/cover for the battery. I’m gonna make my own charger from a local huge electronics warehouse. The battery life is gonna be in tiny led’s somewhere on the side or bottom of board. I don’t think anyone else has ever done that. I wanna go nuts on my first build. Sky is the limit. 🤘🏼 I def need to start a thread. It’ll be cool with all the cnc videos I’ll take and the wiring. You guys all know about the batteries and motors, but I’m a specialist in pro lighting engineering, so I’ll try to come up with some ridiculous new ideas for getting us all seen by cars and being able to see killer stones and sticks in the road at night LOL 😂🤣. Awsome. I’m glad I came across this forum last night. Lots of great info on here.
```

---
