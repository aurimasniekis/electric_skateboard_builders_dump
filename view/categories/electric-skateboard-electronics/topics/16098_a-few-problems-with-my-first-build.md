# A few problems with my first build

### Replies: 37 Views: 3275

## \#1 Posted by: JoJo Posted at: 2017-01-14T17:16:55.271Z Reads: 203

```
Hello electric skateboard builders! I have recently finished my very first esk8 build and have now taken it out for a few runs, however I am running into a couple of problems. 

The first problem i'd like to address is the acceleration from a full stop. I have noticed that my (dual) motors (sk3 260kv brushless-outrunners) jutter or stall when i try to slowly accelerate from a complete stop. I am not sure weather this is due to the (kv) of the motors being too high or something to do with my vesc settings. 
[Heres a video](https://youtu.be/RrN2our-DbI)

The second problem i have noticed is that whenever i connect the circuit in the board to turn it on, a blinding spark goes off. this is kind of discomforting, and i was wondering what could be causing the problem and if there are any solutions. 
[Here is a video](https://youtu.be/jWXkhEzjsqo) 
My hypothesis is that the voltage stored at the end of the connector is built up and when the connection is made, such a small surface area is initially touching, the electricity has nowhere else to go but out. using a volt meter i noticed that the energy at the connection is something like 30V and maybe it is because of the large amount of energy? I have no clue, this is my first time doing this... 

Here is a picture of my circuit diagram and the actual circuit 
<img src="/uploads/db1493/original/3X/f/0/f0d840279b42603e71b0e75b841cf9b00a0f2306.png" width="690" height="297">
<img src="/uploads/db1493/original/3X/f/2/f2288c7eb580e5934f10be152c7e881bb28b08ca.JPG" width="666" height="500">

On the bright side, i have achieved a top speed somewhere between 35 and 40km/h, and got a time of roughly 61 seconds for a full lap of a 400 meter track.

<img src="/uploads/db1493/original/3X/2/f/2ff400af094aa1093b47400d7d38cde5d73ba8c3.png" width="610" height="500">

Specs and Parts: 
2x sk3 260kv brushless outrunners
2x vesc v4.12
2x Zippy 8000mah 4S 30C Li-Po's (in series for 8S)

Loaded Vanguard Flex 1
Orangatang Kegels (orange)
Calliber II Trucks
2x Alien powers systems Drive kit

<img src="/uploads/db1493/original/3X/e/9/e9404de25b4d6f07b8d63acd97291d791e56426f.JPG" width="666" height="500"><img src="/uploads/db1493/original/3X/1/c/1c121b831ae3187a72ff50414cbeb93a374ec766.JPG" width="375" height="500">
```

---
## \#2 Posted by: wmj259 Posted at: 2017-01-14T17:21:24.752Z Reads: 180

```
For your spark, I think you need to get a Vedder anti-spark kit
```

---
## \#3 Posted by: JdogAwesome Posted at: 2017-01-14T17:32:13.440Z Reads: 176

```
Hey @JoJo nice build!  For your first problem with the stuttering, I'm not sure about because I don't have a geared setup, I have hub motors, but it might be do to your VESC settings. But your second problem is due to the capacitor banks on the VESC's. When you first plug it in there will be a large spark because it's drawing an immense amount of current but for an insanely short period of time. Like @wmj259 said you could use a Vedder Switch witch would solve your problem. You could also you XT90 connectors witch I guess have some sort of resistor inside of it to slowly charge the capacitors and prevent that initial spark. You could also take a look at my MOSFET switch thread were I have schematics on how to build yourself a switch as well.
```

---
## \#4 Posted by: goldenHusky Posted at: 2017-01-14T17:36:36.872Z Reads: 173

```
Or you could use a xt90 anti spark plug.
Anyway, the benefit of an anti spark switch is that you can use a good looking switch maybe even with a led (ring) to power your board.
The spark is basically the result of the requested charge current for the capacitors of your vescs

EDIT: @JdogAwesome was faster :grin:
```

---
## \#5 Posted by: JdogAwesome Posted at: 2017-01-14T17:41:00.353Z Reads: 165

```
This is what @goldenHusky means by an LED switch. And I guess I'm just a speed demon lol.
 <img src="/uploads/db1493/original/3X/c/9/c9b485e2301f231715901b6585e71077b3c5cb6e.jpg" width="690" height="388">
```

---
## \#6 Posted by: goldenHusky Posted at: 2017-01-14T17:42:29.612Z Reads: 161

```
[quote="JdogAwesome, post:5, topic:16098"]
And I guess I'm just a speed demon lol.
[/quote]

:smiling_imp: :imp: :smiling_imp:
```

---
## \#7 Posted by: mortorojo Posted at: 2017-01-14T17:44:17.569Z Reads: 155

```
The stuttering or cogging is a side effect of using BLDC, to prevent that kick off before you apply the throttle. Another option is to use FOC, though I wouldn't recommend without some research, since some people have had the DRV blowout on there VESC.
```

---
## \#8 Posted by: JoJo Posted at: 2017-01-14T18:20:57.310Z Reads: 157

```
Awesome! thanks for your suggestions! I'll check it out
```

---
## \#9 Posted by: JoJo Posted at: 2017-01-14T18:22:35.620Z Reads: 153

```
[quote="mortorojo, post:7, topic:16098"]
a side effect of using BLDC
[/quote]

Is there a way to fix this? i dont really want to mess with FOC since this is my first time trying
```

---
## \#10 Posted by: JoJo Posted at: 2017-01-14T18:24:06.237Z Reads: 150

```
[quote="goldenHusky, post:4, topic:16098"]
led (ring)
[/quote]
Do you know where i could get my hands on one of these?
```

---
## \#11 Posted by: goldenHusky Posted at: 2017-01-14T18:27:01.822Z Reads: 143

```
@JoJo this one of the cheapest out there: about 2,50€ including shipping worldwide
http://www.ebay.at/itm/16mm-12V-Car-Silver-Aluminum-LED-Power-Push-Button-Switch-Schalter-Latching-Heis-/191574665101?var=&hash=item2c9abd678d:m:maKEA89oJj02O53FBczkJ0g
```

---
## \#12 Posted by: JdogAwesome Posted at: 2017-01-14T18:36:22.639Z Reads: 138

```
You can get a nice one on Amazon Prime, it has a socket as well which makes installing it way easier. https://www.amazon.com/dp/B00ZR7MMXO/ref=cm_sw_r_cp_apa_U9MEybC6F1CDJ
```

---
## \#13 Posted by: Smorto Posted at: 2017-01-14T18:36:47.664Z Reads: 143

```
Let me just start out by saying that I am not 100% sure that what I know is correct but I'm going to give my 2 cents anyway. I completely agree with what @mortorojo said about preventing the cogging with a push start then hitting the throttle. The cogging could also be because you are using unsensored motors. These will often give a rough startup with a lot of cogging from a complete stop. I believe that sensored motors give a much smother start from a dead stop. That is just my opinion but as I said before, I could be wrong
```

---
## \#14 Posted by: JoJo Posted at: 2017-01-14T18:37:29.693Z Reads: 141

```
Does it include the circuit board like the one posted by JdogAwesome? Or its it the switch itself? Earlier I tried to use a 5-10v "garden bender" switch but I think it fried.
```

---
## \#15 Posted by: goldenHusky Posted at: 2017-01-14T18:39:26.971Z Reads: 139

```
Both @JdogAwesome and my link only provide the switch itself. This switch is intended for use with an anti spark switch (pcb).
```

---
## \#16 Posted by: JoJo Posted at: 2017-01-14T18:40:00.636Z Reads: 142

```
Great idea. I'll be sure to push start. Do you know there I could find some sensored motors for around the same price point as the ones I currently have as a future upgrade?
```

---
## \#17 Posted by: JdogAwesome Posted at: 2017-01-14T18:40:45.533Z Reads: 141

```
Yeah pretty much any conventional switch you find your going to kill because of the amount of current these boards draw, really your only option when it comes to EBoard switches are either MOSFETs or XT90's.
```

---
## \#18 Posted by: JdogAwesome Posted at: 2017-01-14T18:42:27.545Z Reads: 144

```
You don't need sensored motors, most people don't use them because the sensors break or cause other problems, any board you find pretty much is going to have cogging problems at the start, that's just how brushless motors work. And they can also cause problems at high speeds because the hall sensors can't reset fast enough. And sensored motors are a lot more expensive as well as very hard to find.
```

---
## \#19 Posted by: JoJo Posted at: 2017-01-14T18:46:28.590Z Reads: 136

```
That's good to know about the switches, I was just about to go buy another one 😂 
About the motors, just a small push at the start is all I need to fix the cogging?
```

---
## \#20 Posted by: JoJo Posted at: 2017-01-14T18:47:53.227Z Reads: 136

```
Could you possibly share a link to where I could purchase a PCB or vedder switch?
```

---
## \#21 Posted by: Smorto Posted at: 2017-01-14T18:51:26.373Z Reads: 132

```
Yes, as long as the board is moving you should be all set.
```

---
## \#22 Posted by: goldenHusky Posted at: 2017-01-14T18:53:05.988Z Reads: 134

```
@JoJo Well..lol.. I have some switches and pcb lying next to me up for sale
You can check out my sales thread here 
http://www.electric-skateboard.builders/t/vedder-anti-spark-switches-for-sale/15639

Since you are in Canada, you could also order one from ollinboardcompany.com which is based in the US
```

---
## \#23 Posted by: JdogAwesome Posted at: 2017-01-14T18:59:45.821Z Reads: 123

```
I do sell my switches normally, but I'm currently out of the country so I would go with @goldenHusky offer for the Vedder switch.
```

---
## \#24 Posted by: JoJo Posted at: 2017-01-14T19:01:26.931Z Reads: 121

```
Awesome! I'll check it out!
```

---
## \#25 Posted by: BoardfortheLord Posted at: 2017-01-15T01:10:03.198Z Reads: 112

```
hey man are you still looking for a way to fix the cogging?
```

---
## \#26 Posted by: BoardfortheLord Posted at: 2017-01-15T01:13:22.344Z Reads: 116

```
I have a way to fix that if your still interested
```

---
## \#27 Posted by: JoJo Posted at: 2017-01-15T01:23:29.515Z Reads: 123

```
For sure! What's your suggestion?
```

---
## \#28 Posted by: Pathaim Posted at: 2017-01-15T01:31:15.879Z Reads: 140

```
Im pretty sure using sensored motors would also help, it is normal, happens on my setup aswell, try pushing to start :slight_smile:
```

---
## \#29 Posted by: BoardfortheLord Posted at: 2017-01-15T01:35:03.369Z Reads: 141

```
I had the same issue as i just built a board myself and i too was testing yesterday. After hours of searching on youtube about a shakey start here is what fixed it for me.

1. Go into bldc tool
2. go to "motor configuration" tab
3. make sure you have "bldc" motor type checked
4. on the side tabs in motor config go into "advanced"
5. in the "advanced" tab there should be a section called "Current control"
6. in "current control" there is something called "startup boost" I think the default is 0.010 

startup boost acts like a clutch on a car, the lower the value on startup boost the longer it takes for the eboard to get going

7. I found that by changing my value to 0.060 it fixed the problem and there are no shakey starts anymore!

(I would recommend not going over 0.1 and your sweet spot, based on your gear ratio, batteries and motor, should be around 0.030 to 0.090

Let me know if this helps!
```

---
## \#30 Posted by: JohnnyMeduse Posted at: 2017-01-15T01:45:45.491Z Reads: 140

```
I Know that I'm late to the party... 

[quote="mortorojo, post:7, topic:16098, full:true"]
The stuttering or cogging is a side effect of using BLDC, to prevent that kick off before you apply the throttle. Another option is to use FOC, though I wouldn't recommend without some research, since some people have had the DRV blowout on there VESC.
[/quote]

You will get the same result (even worst) in FOC if your not sensor, the cogging is cause by the motor trying to find is position, or not enough current on the start... 

Best way to avoid any cogging is to give a push or use sensor motor.
```

---
## \#31 Posted by: JoJo Posted at: 2017-01-15T01:49:48.793Z Reads: 131

```
Awesome! I'll try this out tomorrow and tell ya how it goes
```

---
## \#32 Posted by: psychotiller Posted at: 2017-01-15T02:19:48.081Z Reads: 129

```
The only thing that will fix cogging is using a sensored setup. Then sensored FOC is a whole new experience. The spark can be fixed using xt90s plugs in a loopkey or a soft switch such as a vedder switch.
```

---
## \#33 Posted by: BoardfortheLord Posted at: 2017-01-16T03:23:57.014Z Reads: 115

```
did you test the new settings? did it work?
```

---
## \#34 Posted by: JoJo Posted at: 2017-01-16T05:46:26.050Z Reads: 112

```
Unfortunately not today some other things came up. I will check it out some time this week and will let ya know!
```

---
## \#35 Posted by: BoardfortheLord Posted at: 2017-01-17T00:31:10.510Z Reads: 107

```
sweet man!
```

---
## \#36 Posted by: JoJo Posted at: 2017-01-21T19:41:41.992Z Reads: 96

```
It worked! I did what you suggested in the BLDC tool and changed the startup boost value to 0.060 and while it is not completely gone, cogging off a start has been reduced. Thank you!
```

---
## \#37 Posted by: PDXroses Posted at: 2018-04-30T15:12:55.015Z Reads: 31

```
Hey Jdog. Interesting thoughts on sensored motors. I’ve been experiencing a sudden grab when I brake. It happens infrequently, but it’s scary. Do you think it could be the sensors malfunctioning?  What causes sensors to malfunction?  Thanks for any insights.
```

---
