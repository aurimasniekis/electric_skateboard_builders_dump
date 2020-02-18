# Who has Experience ?,&hellip; Low KV vs High KV?

### Replies: 58 Views: 6720

## \#1 Posted by: Randyc1 Posted at: 2017-02-04T01:20:21.007Z Reads: 524

```
Who have experience With using Low KV vs High KV motors on their Skateboards?

What are your findings ? ,, preferences ??

- Low being 150-190  
- High being 190 and up .
```

---
## \#2 Posted by: JLabs Posted at: 2017-02-04T01:22:59.704Z Reads: 518

```
It all depends on the type of reduction ratio you use. On my first build I used a 290kv Tacon with 14/36 gear ration and have yet to find a hill it can't climb. So really it's all up to your preference, unless you go crazy high of course.
```

---
## \#3 Posted by: Luke Posted at: 2017-02-04T02:19:16.959Z Reads: 505

```
It's also restricted by your choice of battery. If you're using 10s then stick to under 200
If you're using 12s stick to below 190
```

---
## \#4 Posted by: LukeL Posted at: 2017-02-04T02:40:55.403Z Reads: 506

```
most places online in rc groups etc seem to say kv has no relation to torque and it's all about motor size

so just choose a motor big enough with enough torque, depending on dual/single drive and how heavy you are. Bigger motors tend to have lower kv that limits what you can pick.

Does the battery limit you? if you can just limit the erpm in the bldc tool there shouldn't be a problem, you could argue that you would be wasting money on extra battery, also isn't the vesc 6.0 supposed to be increasing the erpm limit?

i'm using 240kv 10S and weigh 180lb, it seems to have enough torque to get up any hill and have reached 24.8mph which i think is the max due to erpm limit
```

---
## \#5 Posted by: Randyc1 Posted at: 2017-02-04T02:44:28.864Z Reads: 478

```
I'm using a SK3 245 KV  on 10S, also,.. and works fine , just wondering how using a 190KV and Lower Ratio differs in real life use ??
```

---
## \#6 Posted by: willpark16 Posted at: 2017-02-04T02:47:25.072Z Reads: 463

```
I have used 190kv 260kv and 245kv on 6s 8s and 10s. 6s and 245kv is nice when just starting out east to control smooth and reliable. range is ok. 260kv on 6s is fast but at the same time I enjoyed 245 kv more because of torque. I find 8s with 245kv is the one of the better balanced for a motor like this. 190kv and 10s is nice too but it rewuires a large fear ratio for larger wheels but on 83mms it's nice
```

---
## \#7 Posted by: willpark16 Posted at: 2017-02-04T02:48:40.469Z Reads: 452

```
I also find that running 245kv on 10s at speeds over 25mph burns ur battery life much faster by a few miles even
```

---
## \#8 Posted by: Randyc1 Posted at: 2017-02-04T02:49:38.460Z Reads: 441

```
Have you tried Lower KV on the same 10S
```

---
## \#9 Posted by: willpark16 Posted at: 2017-02-04T02:50:34.419Z Reads: 433

```
Yes only li ion too
```

---
## \#10 Posted by: Randyc1 Posted at: 2017-02-04T02:51:27.617Z Reads: 427

```
Did you prefer the lower KV setup?
```

---
## \#11 Posted by: willpark16 Posted at: 2017-02-04T02:52:19.135Z Reads: 418

```
I honestly preferred 6s 245lv to be honest
```

---
## \#12 Posted by: Randyc1 Posted at: 2017-02-04T02:53:33.518Z Reads: 416

```
I'm thinking of a DR setup using 2x 6355 190kv on 10S with 15T 34T, 85-90mm wheels ?
```

---
## \#13 Posted by: willpark16 Posted at: 2017-02-04T02:56:16.350Z Reads: 409

```
It's faster but less controllable I think you will honestly prefer torque over speed so use a large gear ratio 40t
```

---
## \#14 Posted by: LukeL Posted at: 2017-02-04T02:56:48.868Z Reads: 411

```
[quote="willpark16, post:6, topic:17177"]
260kv on 6s is fast but at the same time I enjoyed 245 kv more because of torque
[/quote]

were these motors the same size?

if so then just changing the reduction ratio should give the same performance for both? i wish i could test this as it would show if kv really has anything to do with torque, by adjusting the ratios so that both boards have same top speed and seeing if torque is the same
```

---
## \#15 Posted by: willpark16 Posted at: 2017-02-04T02:58:55.620Z Reads: 393

```
it really depends on the motor so far 6s and a tacon has been my favorite compared to 10s and a 6355 r spec, 260kv was the sk3
```

---
## \#16 Posted by: Chris22 Posted at: 2017-02-04T02:59:32.282Z Reads: 391

```
I have built a few E-vehicles and I am currently working my first electric longboard.

In my experience it is better to have a Low KV motor since less gearing will be required. There is an easy way to calculate the amount of torque the motor will produce. Kv is the RPM constant, Kt is the torque constant. kt = 1355 / kv . Kt is in units of "Oz-In/A".

Here is an example. If your motor is a 150kv motor. Then it has a Kt of 1355 / 150 = 9 Oz-In/A (approximately).

Now you take your max amp draw, lets say 100A, and multiply that by the Kt.

9 Oz-In/A x 100 A = 900 Oz-In or about 4.68 ft-lbs for torque. This motor output torque is then multiplied by your gear reduction. 3:1 would be 3x the torque, 1/3 of the RPM.
Top speed of course is Kv x max voltage.


Side note:
For my electric skateboard I decided to use a higher KV motor (720kv) that pulls 128A and runs 12s. This will give me a lot of RPM. I have started to design a reduction system to drop the RPM from 30,000 rpm to around 5,000 rpm. With my gear reduction I should get around 7.5 ft-lbs for torque. The motor is over 5000 watts, and water cooled. Turnigy T20  .
```

---
## \#17 Posted by: willpark16 Posted at: 2017-02-04T03:02:02.097Z Reads: 357

```
Idk about this I can say that a better overall built motor In the long run can generate a nicer ride and better control. I also believe that is an incredibly inefficient system tbh
```

---
## \#18 Posted by: Randyc1 Posted at: 2017-02-04T03:10:48.148Z Reads: 368

```
Best experiment would be one using same Battery , same Moror (differnt KV's)

6364 260KV geared for Torque 14, 40
then   6364 190KV geared for Speed 16, 34 ,... then see the Difference ???
```

---
## \#19 Posted by: NickTheDude Posted at: 2017-02-04T03:17:23.759Z Reads: 375

```
To put it simply **kV is a trade off between torque and speed**, just like gearing is. Two motors that are identical other than their kV will preform the exact same assuming their each geared for the same top speed. This means a motor with **400kV and a reduction ratio of 4:1 will preform identically to a 200kV motor at a reduction ratio of 2:1.**

**HOWEVER, the VESC has an RPM limit of 8570.** Meaning the motor/battery you choose should not be capable of more than 8570 RPM at top speed. Thus, a 190kV motor at 10S would give you a max RPM of 190kV * 42V = 7980RPM and therefor be okay to use with a VESC. If you were to go with a higher kV motor, say 250kV, the maximum RPM would be 250kv * 42V = 10,500RPM which is too high and you would run the risk of blowing your VESC.

Also, BLDC motor are most efficient around 80% of their top no load RPM, therefore it is best to choose a motor that has the highest kV you can without exceeding the RPM limit. 190kV and 10S are common because they are close to the limit but allow for some headroom.
```

---
## \#20 Posted by: Randyc1 Posted at: 2017-02-04T03:33:01.067Z Reads: 379

```
What about if you think that most of our riding won't be done at 42-40V(10S) ,.. probably most will be done between (39-36V) ? , should that influence our KV choice ?
```

---
## \#21 Posted by: Chris22 Posted at: 2017-02-04T03:55:11.803Z Reads: 361

```
I don't think it should. The cruising speed that you will want to use most of the time should be below the max voltage of the motor.
```

---
## \#22 Posted by: Eboostin Posted at: 2017-02-04T05:15:47.492Z Reads: 347

```
You like 6S better than 10S? Or were you only talking about higher KV?
```

---
## \#23 Posted by: Namasaki Posted at: 2017-02-04T05:36:59.019Z Reads: 351

```
[quote="Chris22, post:16, topic:17177"]
For my electric skateboard I decided to use a higher KV motor (720kv) that pulls 128A and runs 12s.
[/quote]
What type of Esc are you planning to use?
```

---
## \#24 Posted by: willpark16 Posted at: 2017-02-04T05:47:36.030Z Reads: 342

```
Haha ik but yea I really did prefer the 6s
```

---
## \#25 Posted by: Namasaki Posted at: 2017-02-04T05:49:28.152Z Reads: 342

```
I'm running dual 190kv at 10s with 15/36 gears and 83mm wheels.
What I have noticed is that this combination seems to have a good balance between torque and speed while the motors never get hot, warm sometimes but not hot. Neither do I have any problem with the Vesc's over heating even when going up and down long hills.
```

---
## \#26 Posted by: NNGG Posted at: 2017-02-04T06:37:58.384Z Reads: 340

```
Don't lower KV motors have more copper in the stator?
```

---
## \#27 Posted by: E-Boarding Posted at: 2017-02-04T08:39:00.781Z Reads: 337

```
I've a tool to calculate things like this, just put in paremeters and see how speed etc. changes. It also shows motor RPM and max current for the given motor watts.
It doesn't show torque directly but it shows the force on the street. (torque is at the axle, but force depends on wheels size)
http://esk8-dresden.de/poe/v0.2/?tree=18650,Battery,Li-ion,1S1P,4S,5S,6S,Single,Dual,Belt,MotorP,WheelP,Wheels,70mm,75mm,80mm,83mm,90mm,&cellweight=45&kv=280
```

---
## \#28 Posted by: Okami Posted at: 2017-02-04T10:34:36.595Z Reads: 327

```
How to take into consideration the wheel size for this? 

I get about 45 'direct' kv, when I divide 192 / 4.33 (ratio). But im having 9in pneumatics + belt drive.

I assume, in general, pneumatic wheels will require a bit more torque compared to street wheels
```

---
## \#29 Posted by: NickTheDude Posted at: 2017-02-05T04:37:23.166Z Reads: 306

```
@NNGG I've heard the opposite from some people so I'm not really sure. I figure it probably changes for each type of motor. I suppose you could look at the weights of them to see if one has more copper than the other. For SK3s the 149kV weights 1265g and the 192kV weights 1288g so I don't think you'd be able to feel the difference.

@Okami Upgrading the diameter of your wheels would raise your top speed. If you compensated by increasing the reduction ratio in order to keep the top speed the same than theoretically the torque would be identical. However I think you're right in assuming that pneumatics would be less efficient so to keep the same amount of torque you'd have to increase the ratio a little more.
```

---
## \#30 Posted by: Randyc1 Posted at: 2017-02-08T22:29:36.644Z Reads: 276

```
Any of you who have used High vs Low KV noticed more DRAG on the lower KV motors....Does not coast as freely as higher KV,  probably lowering Range as well ?

Just heard about this on another thread and am curious about others experience ?
```

---
## \#31 Posted by: NNGG Posted at: 2017-02-09T00:18:28.604Z Reads: 269

```
Thats correct at higher speeds, coming from a 149kv @ 12S, But I don't notice it at sub 20 kph
```

---
## \#32 Posted by: Chris22 Posted at: 2017-02-25T21:20:09.317Z Reads: 260

```
Sorry for the late response, I am going to use Turnigy k force 120A hv esc that I have used to run this motor in the past. Mostly because I have it lying around.  I will eventually switch to the VESC because of the improved start up torque and more advanced setting for regenerative braking. 

We will see if it can handle the load. I will work out the electrical and mechanical efficiency to see how bad it is. I know with the added reduction I will have some mechanical losses but hopefully not a ridiculous amount.
```

---
## \#33 Posted by: Strange4209 Posted at: 2017-02-26T12:59:11.762Z Reads: 256

```
6374 190kv with a 12s is scary fast gold to the small amount of knowledge I have...
Motor only get slightly warm after some good abuse.
 Granted its only 40 or 50 degrees now, but I can tell it's a very fast, reliable setup for the short time I've gotten to man handle it. 

Latly im very interested in a higher KV lower Series battery, mono setup too.
Just really want to know what I'm getting into before I pull the trigger.  
The price of 6s-8s batteries are nice with a mono set up.
Is it just about the same sensation as my own setup? Without the high speed? A much more calm controlled ride all around?
Thanks 🤘
```

---
## \#34 Posted by: Strange4209 Posted at: 2017-02-26T13:05:56.936Z Reads: 248

```
Also in the process of building my dual motor 6355 190kv now on a 12s4p from Bara..
Got everything but the enclosure here or on the way..

So I want something different for my girl or a friend so they don't feel like they're on a rocket to outer space
```

---
## \#35 Posted by: Dornacht Posted at: 2017-02-26T22:28:12.468Z Reads: 240

```
Using a scorpion 5030 220kv at 10s and can reach 28mph easily on flats, don't recommend because it does cost $300 new
```

---
## \#37 Posted by: PXSS Posted at: 2017-02-27T04:42:17.952Z Reads: 235

```
That's assuming it's an out-runner with 14 poles.
The T20 he's using is 4 poles.
ERPM = (720KV)* (12S * 4.2V)*(2 Pole pairs) = 72,576 Max ERPM
```

---
## \#38 Posted by: Chris22 Posted at: 2017-02-27T05:17:40.202Z Reads: 236

```
PXSS is correct this is a 4 pole motor. 72576 ERPM
```

---
## \#39 Posted by: HTownBomber Posted at: 2017-02-27T16:45:42.019Z Reads: 239

```
720kv inrunner at 12s 128amps? What size? A 56mm+ inrunner geared down correctly would have stupid power, but would require some fancy gearing to harness that power at usable board speeds. I'd love to see you pull it off and I've been toying with a similar idea myself.

If you run 90mm wheels, you're gonna need to gear it down 7:1 or somewhere thereabouts to get proper torque off the line. With that kind of ratio you need a gearbox, or multiple reduction stages if you stick with belts.  What's your plan for gearing?
```

---
## \#40 Posted by: Chris22 Posted at: 2017-02-27T18:45:24.978Z Reads: 237

```
Hey HTownBomber,

Yes it is a 56mm inrunner that runs 12S @ 128A. I agree with you the biggest challenger is the gear reduction. I should be done and riding the streets by the time the snow is gone where I live.

I am running 90mm wheels. I would have liked to go to a 7:1 reductions but I am starting out with a 6:1 due to space limitations. I am using a two stage system. A pulley mounted on the wheel will be driven by a pulley mounted to a small 3/8" OD jackshaft bolted to the rear truck. I am using roller bearings to hold the shaft, which are rated at 650 lbs and 29,500 rpm. I will use a hardened shaft so it can take the load. The other side of the jack shaft will have my second reduction which I have already purchase. This reduction is a set of high load 20 degree pressure angle spur gears at 2:1 reduction (24 to 48 tooth). The 24 tooth is mounted to my motor, the 48 tooth is on the jack shaft.

I have to make sure I can still adjust the belt tension, or alternatively add a belt tensioner as an add on.

Thats basically my gearing plan. I might weld a small SS box around the gears after I am happy with it and fill this with grease or oil, otherwise my only concern is that the gears are going to get HOT.

The motor I think i can keep cool with the water jacket. I have used this motor on a BAJA 5T before and I still have the small radiator/fan and water pump i used as a closed loop cooling system on that project. I am going to use a similar system here.

Results from the spreadsheet I used for speed calcs below.
<img src="/uploads/db1493/original/3X/4/e/4edaf9666d21d5f8b34cc8b408ee4931cf6425aa.png" width="323" height="500">		

7.42 ft-lbs of torque at 104 km/h....crazy but not impossible. Iv gone that fast on my snowboard, never a longboard though. 104 km/h downhill seems sketchier then powered on a flat run.

Cheers,

Chris
```

---
## \#41 Posted by: Chris22 Posted at: 2017-02-27T18:55:26.627Z Reads: 204

```
I started my own thread on the build portion of this forum. I will be updating it tonight with some pictures.
```

---
## \#42 Posted by: HTownBomber Posted at: 2017-02-27T19:18:11.679Z Reads: 204

```
Sounds like a monster.  Can't wait to see how it works out.  I like the 2-stage reduction, a setup that e-bikes have gravitated towards (mid-drive e-bikes).  

Factoring voltage sag, motor and gearing inefficiencies, I'm calculating a weighted top speed closer to 73 kph, which is still dangerously fast but not ludicrous speed.  When you get up around those speeds, headwinds are gonna slow you down more than anything else.      

http://calc.esk8.it/#{"batt-type-lipo":1,"batt-cells":12,"motor-kv":730,"system-efficiency":80,"motor-pulley-teeth":1,"wheel-pulley-teeth":6,"wheel-size":90}|
```

---
## \#43 Posted by: Chris22 Posted at: 2017-02-28T00:42:12.812Z Reads: 198

```
Nice Tool! I never knew about this! I like how it tell me the weighted top speed. 73 km/h is pretty fast. I will post some videos of the build and first test when I am done.
```

---
## \#44 Posted by: ThinkChink Posted at: 2017-02-28T09:51:30.986Z Reads: 193

```
What if I am using an 8s? I am also curious about battery consumption on lower KV motors, do they consume less or more?
```

---
## \#45 Posted by: Luke Posted at: 2017-02-28T17:59:01.581Z Reads: 187

```
I don't believe that the difference is significant, however I haven't run any tests myself.
```

---
## \#46 Posted by: saul Posted at: 2017-02-28T18:09:17.502Z Reads: 188

```
i used 12s and 8s on various kv motors. gearing. wheels. with motors from 140-245kv.
either way you can get 20mph+, climb hills. and good range.

but theres always a torque/speed trade off. I haven't bothered testing anything that can't go at least 20mph because that is just boring now....:sweat_smile:

The real thing is the sound of the motors is different when using bldc/vesc and the torque band moves around. like off the line torque vs 12mph to 20mph.
```

---
## \#47 Posted by: Ryel Posted at: 2017-06-13T20:12:56.826Z Reads: 167

```
How's breaking on this board wand what's your max speed?
```

---
## \#48 Posted by: Namasaki Posted at: 2017-06-13T20:37:27.639Z Reads: 173

```
[quote="Ryel, post:47, topic:17177, full:true"]
How's breaking on this board wand what's your max speed?
[/quote]
At the time of that post I was running 83mm wheels and 15/36. 
Max speed was about 23 mph with my weight which is around 195
Braking is good but that's mostly because of the Vescs and also because of the dual drive. 

Currently I am running 90mm wheels with 15/40 gears. Bigger wheels = smoother ride. 
Top speed is about the same and braking seems even better.
```

---
## \#49 Posted by: lrdesigns Posted at: 2017-06-14T02:43:04.861Z Reads: 167

```
My experience is with 270kv 12s, 97mm wheel and 3:1 (15/48) gear reduction. It works but I don't like the large gear reduction. The wheel pulley is quite large and close to the ground and small motor pulleys wear out faster than large ones.  At first I had 4:1 ratio with a 12 tooth motor pulley. Those wore out super quickly. Im currently in the process of building a 140kv system, same size motors and everything else. Just so I can run a 2:1 ratio. 20/40 pulleys. Should be much more reliable on the pulley and belt side.
```

---
## \#50 Posted by: Carvetothemax Posted at: 2017-06-14T06:37:21.147Z Reads: 161

```
I  found an interesting project that I will try to replicate. 
**It uses 380kv motor and 6s and 3:1 gear ratio**. 
Of course is a budget build but I was amazed by the perforce reported and would be perfect for my needs.
Any concrete reason why I should not go this way?

If you want to look at the build the thread is called "300€ electric skateboard build" by never stop seeking
```

---
## \#51 Posted by: darkkevind Posted at: 2017-06-15T08:52:50.864Z Reads: 151

```
Will is that 6s Lipo or Li-ion? If Li-ion how many p?
```

---
## \#52 Posted by: Ryel Posted at: 2017-06-15T19:20:33.599Z Reads: 148

```
Awesome! Thanks for the info.
```

---
## \#53 Posted by: willpark16 Posted at: 2017-06-15T19:58:18.575Z Reads: 142

```
4p li ion celss
```

---
## \#54 Posted by: darkkevind Posted at: 2017-06-15T22:12:39.970Z Reads: 141

```
And that was enough for a single motor? What sort of range does that get?
```

---
## \#55 Posted by: willpark16 Posted at: 2017-06-16T17:22:36.417Z Reads: 132

```
10 miles????
```

---
## \#56 Posted by: darkkevind Posted at: 2017-06-16T19:25:46.168Z Reads: 130

```
Sounds perfect for me, I'll go 6s4p then I think with 30q Samsungs... :thumbsup:

Thanks!
```

---
## \#57 Posted by: Saturn_Corp Posted at: 2018-10-16T21:59:08.866Z Reads: 72

```
What would this mean for motors with a 1:1 gear ratio such as direct drive or hubs?

For example the Carvon Speeddrives are 110kv and the Torqueboard dd are going to probably be somewhere around 60-70kv.
```

---
## \#58 Posted by: SkateYS Posted at: 2019-06-10T16:07:12.169Z Reads: 47

```
Low KV consume less battery! they are slightly slower than high KV and arguably safer for your VESC. If you are using the Vedder ESC (VESC, I believe FOCbox or older), choose your KV according to your battery voltage. 10s you need a KV less or equal to 200KV, 12s you need a 170Kv or less. Note: your board will still work fine if you don't respect this, but know that you will be giving your VESC a hard time handling higher RPMs. High KV = faster, draws more juice form battery.
Low KV = slower, more torque, draws less juice. Note that the difference is not too small and that with a low KV motor you can still gain more speed by changing gear ratio (using bigger motor pulley and smaller wheel pulley, or vice versa to get more torque with high KV motors). In my experiments, there was a 5 MPH difference between my 192KV vs 168KV motors (Faster on 192kv) on the same setup.
```

---
## \#59 Posted by: DavidC Posted at: 2019-06-10T21:32:21.941Z Reads: 41

```
IMHO with mountainboard  : low kv = less amps = less heat = better efficiency maybe = less power = no fun

Anyway I don’t go beyond 192kv at 12S
```

---
