# Has anyone amped up the meepo board hub?

### Replies: 45 Views: 3383

## \#1 Posted by: onepunchboard Posted at: 2018-04-09T15:51:19.132Z Reads: 268

```
As the title says,...
Original cheepo esc can only go like 20 each, but anyone tried amping up those 500w motor to like 1000w to each?

Shouldn't be too hard with vesc, but haven seen anywhere.
```

---
## \#2 Posted by: Blitz Posted at: 2018-04-09T15:51:57.768Z Reads: 269

```
Meepo 1.5 runs 40A but that's on a dual setup..
```

---
## \#3 Posted by: onepunchboard Posted at: 2018-04-09T15:54:35.432Z Reads: 266

```
yeah that's 20 each. it suffer from hill.
```

---
## \#4 Posted by: Blitz Posted at: 2018-04-09T16:00:47.660Z Reads: 259

```
You can try ask someone here, maybe the topic author will ask Ownboard.  
https://www.electric-skateboard.builders/t/group-buy-upgraded-ownboard-esc-hub-motor-remote/49783/83

this is the info I found on meepo, It would seem the esc won't pull more than 24A
"This ESC is for dual motor.   Max Current 24Amps. Sinusoidal wave."

https://meepoboard.com/collections/parts-accessories/products/electronic-speed-controller

You could run 100a lipos but It won't pull more than 24A.
```

---
## \#5 Posted by: onepunchboard Posted at: 2018-04-09T16:09:33.340Z Reads: 235

```
I meant with vesc not the riginal esc.but Thanks!
```

---
## \#6 Posted by: evoheyax Posted at: 2018-04-09T16:16:10.674Z Reads: 231

```
You are simply limited by the stator size. Their stators are so small that they will become oversaturated very quickly and overheat. The stator simply can't handle a larger magnetic force than it already is, which is what would happen by pushing more amps into it. This is why hummie stopped producing small hubs like this and stepped it up to a double sized hub motor.
```

---
## \#7 Posted by: PredatorBoards Posted at: 2018-04-09T17:03:10.991Z Reads: 225

```
+10 for this once again. Motor construction isn't magic. All that really matters is the stator size. Stator size indicates copper and iron content, which indicates magnetic saturation, which indicates efficiency, which indicates heat production, which indicates the motor's true max amperage.
```

---
## \#8 Posted by: evoheyax Posted at: 2018-04-09T17:13:11.148Z Reads: 215

```
It's not magic, but their is a geometry between the magnet width and stator teeth width also. They create a trapezoid, which affects motor kv and ultimately, efficiency and heat generation. But the stator is the beginning of everything.  Start small and your limiting your self. And you fit into a normal skate wheel, means your stator has to be on the smaller side.

There's other factors too... Ultimately, you want a large enough stator with a super low resistance. The resistance tells you a lot about how much heat your going to generate once you have a big enough stator ;)
```

---
## \#9 Posted by: PredatorBoards Posted at: 2018-04-09T17:43:47.635Z Reads: 200

```
Yep. The magnets are pretty significant as well, however I excluded mentioning them simply to focus on the bigger picture in this discussion.
```

---
## \#10 Posted by: ElskerShadow Posted at: 2018-04-09T17:58:17.507Z Reads: 190

```
I run them at 50A each with vesc...
Jason told me that the max they could take is 50A
```

---
## \#11 Posted by: onepunchboard Posted at: 2018-04-09T18:03:02.427Z Reads: 182

```
Thats 1800w+ @ 10s That's actually good.

Does it go 25% hill?
```

---
## \#12 Posted by: ElskerShadow Posted at: 2018-04-09T18:09:03.664Z Reads: 186

```
Clearly. 
You can only be amazed by the performance of these hubs with Vesc considering what they are. 
The torque is very good and no hill would stop me if I am already launched ! I’m 90 kg. 
But the fact it’s a design made to be trashed and rebuy... i don’t like it 
I have the old version With bad quality urethane tho. 
They are not very comfortable as well. But they perform great for the price. 
I’m really looking forward recieving my hummies so I can try some « real » hubs, still sceptic with comfort but the reflex urethane they are developing seems promising. 
I use carvon daily so I am a used to use full 97 mm flyweel that are as smooth as the 107’s to me.
```

---
## \#13 Posted by: sayekim Posted at: 2018-04-09T19:35:00.687Z Reads: 182

```
Been running the Meepo hubs with vesc since February.
100
-60
25
-12

With Sanyo 10s2p. No complaints and tackles hills easily. 

https://metr.at/r/I3Hje
```

---
## \#14 Posted by: sayekim Posted at: 2018-04-19T22:57:10.727Z Reads: 162

```
I have ran these suckers today and It seems I overheated them because they went into full brake and acted weirdly in either full brake, unresponsive, or full throttle without me touching the remote. 

It has been the warmest day yet riding them with average speed of 27 kph or 17 mph. It was 27 C or 80 F. 

Anyone else have experience or know why these hub motors would go into braking when overheated @Hummie @evoheyax  ?
```

---
## \#15 Posted by: evoheyax Posted at: 2018-04-19T22:58:59.138Z Reads: 161

```
If you burn up the enamel protecting the wire, they short together and the motor locks up. But this is permenant. They don’t get better if you let them cool off again.
```

---
## \#16 Posted by: sayekim Posted at: 2018-04-19T23:00:53.678Z Reads: 157

```
Mine were working again after they cooled down. Any other ideas?
```

---
## \#17 Posted by: evoheyax Posted at: 2018-04-19T23:15:08.698Z Reads: 159

```
I would say try another esc. Sounds more like an electronic thing than a motor thing.

Unless, it was your bearings that locked up. Bearings are usually the weakest point in hubs motors in terms of heat. I have had bearing lock up from over heating with hummies v1 motors, since they were also very small hub motors.
```

---
## \#18 Posted by: sayekim Posted at: 2018-04-19T23:32:49.102Z Reads: 156

```
I’m using focboxes. 
Never had this when it was colder. Also the motors were too hot to touch and hold. I could touch them but not hold my finger on them. 
You can see here I was going forward but the motor was pulling negative amps. 

![image|690x387](upload://fRA5p4E3g2OFG0BMIRXZ9sXN94u.jpg)
```

---
## \#19 Posted by: evoheyax Posted at: 2018-04-19T23:51:20.552Z Reads: 151

```
Well it’s normal for motors to get too hot to the touch and hold. Anything over 100f is really too hot to touch and hold, and they should be good to at least 150f.

It seems to me like the bearing might be overheating. Metal balls expand under heat and the grease cooks out and they lock up. Then when they cool, they shrink again and are fine.

If that is the problem, then the bearings will break after you do this a few times as they lose their lube and it’s just metal on metal rubbing at that point.
```

---
## \#20 Posted by: onepunchboard Posted at: 2018-04-20T00:01:55.524Z Reads: 153

```
isn't this temp cutoff problem? I cooked a motor few times but usually it just stops moving with smoke comming out. u shouldnt even touch it, you will have blister,

but could be bearing as well due to expension
```

---
## \#21 Posted by: ElskerShadow Posted at: 2018-04-20T00:04:52.154Z Reads: 144

```
I never had this issue and I m running the same set up. I ll tell you if I notice the same thing it's getting warmer in Paris as well. 
One weird thing tho is that I've done motor detection again on foc and now I have much less torque.do u run them in foc?
```

---
## \#22 Posted by: goldrabe Posted at: 2018-04-20T00:40:43.234Z Reads: 139

```
Dis I understand you correctly, they are also accelerating without you touching the remote?
If that is the case it sounds more like a problem with your remote and reciever or a failing esc as said before.
```

---
## \#23 Posted by: sayekim Posted at: 2018-04-20T05:51:04.344Z Reads: 138

```
No load they spin fine. Under load they just brake as in regenerative braking. When they cooled down they work as normal again. 

This is so weird. I’ll see if it happens again today.
```

---
## \#24 Posted by: sayekim Posted at: 2018-04-20T05:52:39.395Z Reads: 134

```
Hmm I ride them unsensored. That can’t be it then can it?
```

---
## \#25 Posted by: sayekim Posted at: 2018-04-20T06:02:55.650Z Reads: 135

```
I ride them in foc. 3.1

Perimetr should have an export function. @rpasichnyk
```

---
## \#26 Posted by: sayekim Posted at: 2018-04-20T06:03:57.766Z Reads: 132

```
Yeah perhaps but I doubt it since no such problem when they cool down.
```

---
## \#27 Posted by: goldrabe Posted at: 2018-04-20T06:35:13.346Z Reads: 131

```
I see, did you soldered bigger connectors on them?
Those clear rubber covers from the original connectors are melting easily once i had one of them getting brown and touching another phase wire under vibration.
I tried this hubs with 15 amps, 20 amps and 30 amps , so for dual setup 30, 40 and 60 amps. I could not feel a difference in torque beyond 20 amps but i noticed that they get way hotter with 30 amps.
```

---
## \#28 Posted by: onepunchboard Posted at: 2018-04-20T06:35:19.710Z Reads: 129

```
maybe possible heat increase resistance and those motor use thinner wire than it may affect foc try sensored. they do get saturated with amp as other says so that could be it
```

---
## \#29 Posted by: sayekim Posted at: 2018-04-20T09:10:48.260Z Reads: 130

```
I did replace a few connectors since some of them felt loose over the past few days and when one of them had a loose connection it also definitely make it sound wierd and also brake until it caught up with speed again with the other hub motor. 

I will replace all the connectors. 

I wish there was a consistency with the faults of the motors I am experiencing now. 

This morning I went out to commute to work with them and something did not feel right. It did not sound weird but it did feel like one of the motors was hesitating in acceleration and yet I went to test ride yesterday evening and it felt absolutely fine again.

Damn it. It was reliable af before the connector loss issue and colder weather.

I'm leaning to the connectors now as the problem. This is the only consistency I have with my problems that started.

Also one of the fricking connectors of the Focbox side broke off earlier which I resoldered with a new one.

Thanks for the input guys, and perhaps gals no?
```

---
## \#30 Posted by: goldrabe Posted at: 2018-04-20T12:57:59.715Z Reads: 117

```
Broken connectors doesn't sound good man.
You could have damaged your vesc with shorting the phase wires. Look in the BLDC tool for faults.
I am still at no clue why your motors accelerated without you pushing the trigger.
```

---
## \#31 Posted by: sayekim Posted at: 2018-04-20T13:11:18.462Z Reads: 114

```
The metr app, eskate vesc app don't show any faults. Would the bldc tool show them otherwise?

I have the whole event on tape. I'll see if I can find the time with my lazy ass to upload it.
```

---
## \#32 Posted by: goldrabe Posted at: 2018-04-20T13:17:21.223Z Reads: 113

```
I never used the metr. app and have no knowledge about what it can do and not can do. But why would your motors accelerate with bad phase wire connections?
```

---
## \#33 Posted by: onepunchboard Posted at: 2018-04-20T13:21:12.786Z Reads: 112

```
maybe time for video!
```

---
## \#34 Posted by: sayekim Posted at: 2018-04-20T21:32:08.469Z Reads: 117

```
Here is where it starts. I go up this hill and it throws me off.

https://youtu.be/0coHSCX3Zlc

This second one is 12 min showing the throttling without remote input. You can also see that when I let go it brakes immediately.

https://youtu.be/S70Al_dAgFg
```

---
## \#35 Posted by: goldrabe Posted at: 2018-04-21T01:44:40.467Z Reads: 106

```
Your wiring is a mess in that tupper 😜

Is your reciever located close to your battery or phase wires? Try to get the reciever as far as possible from wires carrying high currents.
I am leaning towards problems with your remote\reciever when your apps are not showing any DRV faults.
```

---
## \#36 Posted by: onepunchboard Posted at: 2018-04-21T01:53:46.165Z Reads: 105

```
it looks like u cooked the motor half way,
or the receiver is broken.
```

---
## \#37 Posted by: sayekim Posted at: 2018-04-21T07:43:58.293Z Reads: 93

```
Receiver is under the master phase wires bottom left.
```

---
## \#38 Posted by: sayekim Posted at: 2018-04-21T07:45:00.961Z Reads: 90

```
Alright I’ll try the nano x see what that results to.
```

---
## \#39 Posted by: goldrabe Posted at: 2018-04-21T08:39:23.292Z Reads: 95

```
Also check your phase wire plugs again, that strange stuttering might come from bad connections too.
```

---
## \#40 Posted by: sayekim Posted at: 2018-04-21T20:11:45.296Z Reads: 97

```
It was the location of the receiver. Haven't tried anything else but as soon as I relocated it the problem was gone. Also the motors were cold this time since I just went out and it happened instantly.

What is weird is that for the whole ride from the last ride until about a km from my house it started doing this, so that small chance that the receiver antenna I guess was moved to interfere with the signal during the ride is what happened to cause the interference. 

https://youtu.be/RZ4leM5d2LI
```

---
## \#41 Posted by: onepunchboard Posted at: 2018-04-21T20:55:40.059Z Reads: 93

```
wow that is awesome!
```

---
## \#42 Posted by: sayekim Posted at: 2018-04-25T21:41:38.750Z Reads: 91

```
Just figured it out why the interference did not start until the end of the ride last time.

I have the focboxes and receiver fastened via velcro tape which is stuck with the adhesive layer on the back of the velcro. 
At the end of the ride the focboxes get hot enough or have been hot enough for long enough to let the adhesive melt and release from the focboxes which in turn moves them around in the enclosure and get in the way of the receiver which caused the interference.

Do not place your receiver near the phase wires. That is where I notice the interference starts to happen.
```

---
## \#43 Posted by: murdomeek Posted at: 2019-11-18T22:23:37.519Z Reads: 27

```
[quote="sayekim, post:13, topic:51715, full:true"]
Been running the Meepo hubs with vesc since February.
100
-60
25
-12

With Sanyo 10s2p. No complaints and tackles hills easily.
[/quote]

100a/-60a motor amps?
100a each?
or 50a per hub?
```

---
## \#44 Posted by: Sn4pz Posted at: 2019-11-19T04:19:17.602Z Reads: 25

```
Most vescs can't do 100a motor, or if they can not for long... 

I bet he uses vesc 6 🤔
```

---
## \#45 Posted by: sayekim Posted at: 2019-11-19T12:51:42.131Z Reads: 21

```
25 batt amps each and 100 motor amps each. 

Focboxes.
```

---
