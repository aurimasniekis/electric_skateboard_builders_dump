# Please, help with project. 2 x 6354 260kv/2 x X-Car Beast/6 x 4.2Ah 2S 25C Lipo.First eSk8 build.Starting to make a great board

### Replies: 30 Views: 1441

## \#1 Posted by: jeffreyrash Posted at: 2017-04-25T13:12:14.440Z Reads: 184

```
Hello everybody!My name is Vlad, I'm from Russia. I'm a student of MEPhI. A few weeks ago I planned to build my own electric skateboard. It's my first experience in construction like this.
Well two days ago I wrote to a great builder called Tom @Idea , saw his works here. He advise me some of the parts for my project.

So, I plan to make E-board with this parts:

-Turnigy SK3 Aerodrive - 6354-260kv x 2
-HobbyKing® ™ X-Car Beast  x 2
-Turnigy 4200mAh 2S 25C Lipo x 6 (I will make two paralleled stripes 6S each)
-Caliber II 184/10/50
-Abec 11 Flywheels 83mm (Duro: 78A ) 
-Pulleys 15t/36t

Going to do regenerative brakes, but don't know what ESC will be better for it.

I will be very pleased if you advise something good, what parts I need and what has to do in this project.

Really inspired on this project by @Idea and @Namasaki  

P.S. Here my own 4-layer deck, 43""(109cm)
<img src="/uploads/db1493/original/3X/b/1/b11bcda98f8f1503b0087fe4c17367859b730403.jpg" width="281" height="500">
```

---
## \#2 Posted by: SyrusB Posted at: 2017-04-25T13:18:11.977Z Reads: 168

```
Also what remote do you plan on using. Alot of people suggest using a vesc over a car ESC becuse they are designed for esk8. Also a good remote to use is a Gt2b they are very reliable and if you have a 3d printer you can make a smaller case for it. How do you plan on charging and turning it on and off. A cheap and efficient way to turn it on and off is to use a anti spark switch.
```

---
## \#4 Posted by: jeffreyrash Posted at: 2017-04-25T13:26:46.319Z Reads: 162

```
I'm going to use standard remote 2.4 GHz like the way you wrote for the start  .
I'm planning on make something like compact smart remote with all the necessary information in it, think it will be based on arduino.Well, for the first time I will charge batteries separately, cause i don't have system with enough energy for the whole pack(However, I know that is silly) and I don't think about switching    -_-...thanks for the reminder.
```

---
## \#5 Posted by: SyrusB Posted at: 2017-04-25T14:21:14.410Z Reads: 149

```
You could get a bms I am doing a 12s1p with a bms we have a whole post about it then all you have to do is get a laptop charger with the same voltage as your batteries and you can keep them in the case at all times. I used to charge them sepertaly but I am getting annoyed and adding a bms.
```

---
## \#6 Posted by: Marko Posted at: 2017-04-25T19:16:00.447Z Reads: 135

```
Hi vlad, cool project.
i have the same motor running it with the same ESC on 6s. But i`m first trying it in a kart i am building for my kinds. now the Problem i have is that the motor is to weak. It´s not possible to get the tires rotated. I can even stop the motor with my hand, and then it stops and beeps.
Here i have a video: 
https://www.youtube.com/watch?v=vdF0QNTBGhs
is your motor also so wake, that you can stop it with your hand? (i just can stop it wearing gloves, cause it gets very hot :) )
hope you can give me your feedback, because it makes me crazy, that a 2500w motor isn`t able to get the tires spinning.
Thanks, Marko
```

---
## \#7 Posted by: halifax21 Posted at: 2017-04-25T23:31:29.563Z Reads: 127

```
If you can get vesc, you will be better off with the application to configure them to your specifications in the future.  Definitely try to get a BMS on your batteries - the hassle of taking out the batteries to put them on a parallel board to charge will become annoying after a week.  Toms mounts are awesome, good purchase.  The motors are good, I weigh 280# and the push me around at 10s voltage.

Are you using xt90 connectors?
```

---
## \#8 Posted by: jeffreyrash Posted at: 2017-04-26T08:57:20.201Z Reads: 118

```
Hi, Marko!
Thank you.Woow, you know I haven't ordered electronic parts yet.I just learn and read about these to select the better way.

I saw you video, I have not so many variations of the reason of this problem.So it can be:

-Problem with pulleys, may be you should increase  the transfer function of you pulleys(but this is only in theory, cause I have not got so much experience in mechanics).
-Batteries, but I think you checked it.
-ESC, more precisely, settings of your ESC.
-Problem in motor, like spoilage, defect during the production of it. I saw a lot videos and examples where people use these motors and there are no problems.

Here the man using the SK3 - 280kv - https://www.youtube.com/watch?v=4tHmGSwrgxA
```

---
## \#9 Posted by: jeffreyrash Posted at: 2017-04-26T09:02:17.763Z Reads: 112

```
Hello, Halifax!

Yeeeah, VESC will be better, but it is problem to me find vesc's that suits to me, cause there is 70A on motors.And BMS I will buy, definitely.
Wow, you have the same motors?And what about torque?How about acceleration from zero?
```

---
## \#10 Posted by: Tuomalar Posted at: 2017-04-26T11:00:40.515Z Reads: 104

```
You should read another users builds and learn what parts they did use. For example dual 260kv with car escs is very unusual. What is your budget?
```

---
## \#11 Posted by: jeffreyrash Posted at: 2017-04-26T11:19:33.514Z Reads: 102

```
Think that ESC or VESC should be under 75$
```

---
## \#12 Posted by: Tuomalar Posted at: 2017-04-26T11:29:33.924Z Reads: 99

```
You can't get vesc under 75$ so you have to use escs.. But i meant what is your budget with this whole build?
```

---
## \#13 Posted by: halifax21 Posted at: 2017-04-26T12:37:43.650Z Reads: 96

```
These motors are unsensored so you will get cogging, meaning, the motor will skip a couple of times before it engages to drive the belt, I haven't tried to gun it from zero because I don't want to flip off.  The motors are rated to take only 70A in a burst, but the vesc can be configured not to deliver that amount of power continuously.  I've configured my vesc to allow kick starts to over come the cogging and strengthen my legs for days when the batteries are low.

You can use car Esc, lookup E-Toxx builds to see what they did.
```

---
## \#14 Posted by: TarzanHBK Posted at: 2017-04-26T12:54:38.423Z Reads: 92

```
What we do here normally:
On budget: 6s Lipos + RC Charger + Car ESC 6s + Motor about 245KV
Fck my money, I wanna nice thing: 10S - 12S custom Liion + BMS + 2x Vesc + 2x 149KV - 200KV

If you wanna dual Car ESC, check out @lowGuido builds
```

---
## \#15 Posted by: jeffreyrash Posted at: 2017-04-26T20:30:07.940Z Reads: 89

```
So, about 530$.
```

---
## \#16 Posted by: jeffreyrash Posted at: 2017-04-26T20:37:50.516Z Reads: 89

```
Well, Halifax, there is a question: I'm gonna lose a lot of power if I restrict VESC to 50A or is it not critical in practice?And how about regenerative brakes, does it work good, does it feel?
```

---
## \#17 Posted by: halifax21 Posted at: 2017-04-26T20:56:07.500Z Reads: 84

```
If you restrict the flow that just means your not using up the power as fast.  My weight makes regen brakes is a non value added feature - you'll have to get that from a lighter rider
```

---
## \#18 Posted by: saul Posted at: 2017-04-27T17:23:27.131Z Reads: 76

```
your battery setup is too complicated. get larger cells instead of doing 2p. 
that esc makes the worst sound while braking, and you get very little tuning.

the vesc is only 50a but it can do 12s so power is similar. fine tuning is 10000x better with vesc. 

at that budget  I think a single drive with vesc will beat out a dual drive with car esc.
```

---
## \#19 Posted by: jeffreyrash Posted at: 2017-04-28T06:20:17.000Z Reads: 75

```
So, guys, @saul, @halifax21  @TarzanHBK @Tuomalar@SyrusB, FCK the fckin budget! I will get 2xVESC, 2x260KV,BMS ,and better batteries.Well, with batteries and motors it's all the good, I'll buy them on HK. So where I can order good VESCs? I'm afraid of counterfeit.Is it a good idea to take it here http://m.ebay.com/itm/Maytech-Benjamin-Vedder-Electronic-Speed-controller-VESC-for-electric-longboard-/302200711613 ? And what BMS will be better?
```

---
## \#20 Posted by: saul Posted at: 2017-04-28T07:12:41.661Z Reads: 78

```
[quote="jeffreyrash, post:19, topic:21744"]
FCK the fckin budget!
[/quote]

lol in that case.
10s3p hg2 + bestech bms.
[dual ollin vesc](http://www.ollinboardcompany.com/product/vedder-s-speed-controller)
200kv or lower motors

that'll get you 15miles range and > 30mph top speed.
```

---
## \#21 Posted by: jeffreyrash Posted at: 2017-04-28T08:45:39.936Z Reads: 74

```
It will be too expensive(
```

---
## \#22 Posted by: halifax21 Posted at: 2017-04-28T12:25:35.071Z Reads: 71

```
Search the forum for vesc's, I bought mine on eBay - Maytech Vesc
A motor choice under 200kv is good, if you are planning on mounting them on the rear of a regular skate truck Sk3 6355 will fit, you'll have to measure the space used by the motor mount, leave at least 1cm of space between the motors.
BMS and Lipo batteries is a fickle beast. You want range so that means a high Mah > 8k mah, but then you want speed which means 10 ~ 12s. with that kind of lipo you won't find a BMS suitable and that's because there will be too many cells.

Here comes the problem: my setup is 4 x (4s 5000mah) wiring that in series will make a 16s 5a battery pack which will blow your vesc, then if you wire 2 x (2 batteries in series) and then wire those two in parallel, you will have an 8s 10a - now you get speed and range, I haven't seen a BMS on that kind of
```

---
## \#23 Posted by: mmaner Posted at: 2017-04-30T01:46:21.209Z Reads: 62

```
@halifax21 I've never owned an 8s BMS, but I've got 2 packs with series lipos to make 10s where I'm.using s BMS.  Be glad to help if you wanna give it another shot.
```

---
## \#24 Posted by: jeffreyrash Posted at: 2017-05-16T09:17:58.630Z Reads: 56

```
Hi,guys! I have some problems, hope that you can help me. I have ordered 4 x LiPos 3S1P 5000mAh to build 6s and what **BMS** I can use for it and how to connect it?Please see it https://hobbyking.com/en_us/6s-li-ion-10a-pcm.html - is this BMS suit for my build? @TarzanHBK  @saul   @Tuomalar @mmaner
```

---
## \#25 Posted by: TarzanHBK Posted at: 2017-05-16T09:26:20.609Z Reads: 54

```
Only fits for charging, due to the 10A Limit, so if you wanna go with that, you have to bypass it for discharging - several threads therefore on this forum you´ll find.:frog: (<- Yoda)
If you wanna use a BMS for discharging too, you´ll need much more discharging current, so get at least a 80A BMS for 6s (we buy our BMS here: http://www.batterysupports.com/ or here: http://www.bestechpower.com/)
```

---
## \#26 Posted by: jeffreyrash Posted at: 2017-05-16T10:47:41.253Z Reads: 48

```
So,this BMS will not suit for work in the system with VESC?
```

---
## \#27 Posted by: Tuomalar Posted at: 2017-05-16T11:02:04.226Z Reads: 49

```
It does and it doesn't. You can use it only for charge your battery. It can't can handle discharge current. I personally don't know why people use bms between battery and vesc. I personally like super small bms only for charging but seems like there isn't anything really reliable on a market.
```

---
## \#28 Posted by: Tuomalar Posted at: 2017-05-16T11:04:03.412Z Reads: 47

```
Btw i'm not sure how you should connect you batteries. Someone else can help you with that. I wonder if bms can balance 6s batteries in parrallel?
```

---
## \#29 Posted by: Jellybean Posted at: 2017-06-08T09:08:28.048Z Reads: 38

```
Why do you need 1cm of space between the 2 motors? For airflow or magnetic reasons or just general tolerance reasons? I'm wanting to use dual 6354 260kv motors, but I'm not sure I'll have 1cm between the motors on my 183mm trucks.
```

---
## \#30 Posted by: Tuomalar Posted at: 2017-06-08T09:32:41.051Z Reads: 37

```
i have 2mm space between motors and works great.
```

---
## \#31 Posted by: halifax21 Posted at: 2017-06-08T11:46:27.878Z Reads: 32

```
As long as they are not touching and I may have meant mm instead of cm
```

---
