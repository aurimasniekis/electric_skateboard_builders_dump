# Li ion with no bms?

### Replies: 78 Views: 4001

## \#1 Posted by: willpark16 Posted at: 2016-08-08T03:40:49.643Z Reads: 212

```
is it possible to run li ion cells with no bms if so how many cells are neccessary?
```

---
## \#2 Posted by: Pantologist Posted at: 2016-08-08T03:50:26.623Z Reads: 210

```
Yes it is. I wouldn't recommend it though. 

Necessary for what?
```

---
## \#3 Posted by: willpark16 Posted at: 2016-08-08T03:51:15.349Z Reads: 207

```
to run without a bms
```

---
## \#4 Posted by: Pantologist Posted at: 2016-08-08T03:52:00.851Z Reads: 200

```
You can use any amount of batteries without a BMS. The more cell count, the more discouraged.
```

---
## \#5 Posted by: willpark16 Posted at: 2016-08-08T03:53:21.371Z Reads: 199

```
would basen 26650 cells in 8s3p work?
```

---
## \#6 Posted by: willpark16 Posted at: 2016-08-08T03:53:47.634Z Reads: 195

```
that would be 180a burst roughly and 120a cont
```

---
## \#7 Posted by: Pantologist Posted at: 2016-08-08T03:57:40.981Z Reads: 195

```
Your question isn't making sense. You can use any amount of cells. A BMS is an extra safety measure for your ESC, motor etc. You won't have Overcharge and overdischarge protection, not to mention no cell balancing.
```

---
## \#8 Posted by: willpark16 Posted at: 2016-08-08T03:59:07.353Z Reads: 191

```
no im saying can i use just the cells no bms when discharging the cells without damaging them and if so say an 8s setup how manys cells would i need for it to be safe
```

---
## \#9 Posted by: Michaelinvegas Posted at: 2016-08-08T04:01:46.451Z Reads: 189

```
I like this guy

Thinking the same thing @willpark16
 I think building a battery more than you need would allow you to use a pack without a bms safely 



 
https://youtu.be/pljSZcEwc8Q
```

---
## \#10 Posted by: willpark16 Posted at: 2016-08-08T04:03:10.928Z Reads: 181

```
thanks a ton for the link!!!!!!!!!!!
```

---
## \#11 Posted by: barajabali Posted at: 2016-08-08T04:24:02.160Z Reads: 166

```
Yes you can run without bms.
```

---
## \#12 Posted by: willpark16 Posted at: 2016-08-08T04:24:25.317Z Reads: 164

```
and how many cells would u suggest
```

---
## \#13 Posted by: barajabali Posted at: 2016-08-08T04:40:04.606Z Reads: 163

```
any amount is fine there is no wrong number.  

it doesnt matter
```

---
## \#14 Posted by: willpark16 Posted at: 2016-08-08T04:58:27.217Z Reads: 157

```
well i cant run 10s 1p no bms
```

---
## \#15 Posted by: barajabali Posted at: 2016-08-08T04:58:53.736Z Reads: 153

```
yes you can.
```

---
## \#16 Posted by: barajabali Posted at: 2016-08-08T04:59:33.812Z Reads: 156

```
why do you think you cant.
```

---
## \#17 Posted by: willpark16 Posted at: 2016-08-08T05:00:15.945Z Reads: 154

```
because no bms would over exaust the cells if say i try and go 30mph
```

---
## \#18 Posted by: barajabali Posted at: 2016-08-08T05:02:57.009Z Reads: 156

```
no thats not true.  the cells will always have the same amp output.  the bms may regulate that output lower and limit it.  But you wont over exhaust the cells if you dont run a BMS.  The cells will just discharge whatever theyre capable of discharging without a bms to limit it. 

running most Lion cells in 1p is not a good idea. bms or  not.   
 Unless youre going to 26650 cells.
```

---
## \#19 Posted by: willpark16 Posted at: 2016-08-08T05:05:21.529Z Reads: 153

```
so if im running basen cells in 2p with no bms at 10s id be fine? and if so why do people use a bms instead of just a normal charger
```

---
## \#20 Posted by: Pantologist Posted at: 2016-08-08T05:07:50.456Z Reads: 153

```
You'll be fine. At least have a fuse in case of a short. BMS with a laptop single plug style charger is a lot easier to charge and use. 

A "normal" charger in meaning a common lipo balance charger then the reason for not using them is that it requires a lot more effort to charge your battery. 

A BMS also monitors when the board is in use, not just while charging.
```

---
## \#21 Posted by: barajabali Posted at: 2016-08-08T05:08:10.631Z Reads: 146

```
yea 2p with basen will be a cake walk youll be fine.

we use bms for many reasons where do i begin. 

easy charging, plug and forget
cheaper than a 10s lipo charger (trust me i have one)
quicker charging
professionalism 
longer life for cells
over charge protection, over discharge protection
soft switches
thats basically it.
```

---
## \#22 Posted by: willpark16 Posted at: 2016-08-08T05:10:09.621Z Reads: 140

```
oh thats what i needed to ask whats the soft switch for exactly
```

---
## \#23 Posted by: Pantologist Posted at: 2016-08-08T05:11:16.441Z Reads: 135

```
I honestly don't see the point of not using a BMS. You can get one for arounf $35 that will be good enough. At 10S you should not draw more than 60A ever.
```

---
## \#24 Posted by: Pantologist Posted at: 2016-08-08T05:11:55.467Z Reads: 132

```
Turning the BMS PCB on and off. Basically turns off your board since your ESC/motor won't be powered.
```

---
## \#25 Posted by: barajabali Posted at: 2016-08-08T05:12:05.752Z Reads: 131

```
easy turn off and on
anti spark to save connectors life
professionalism
solid state skateboards ( dont have to open the enclosure everytime to turn on and off)


Bms's, soft switches, all these things are luxury's not needed if you dont want to use them. 

I use them though because i like to spend money and i love the features they offer
```

---
## \#26 Posted by: barajabali Posted at: 2016-08-08T05:12:28.830Z Reads: 127

```
I agree. I use them in all my builds.
```

---
## \#27 Posted by: willpark16 Posted at: 2016-08-08T05:13:23.916Z Reads: 133

```
ig ill just get a cheap bms for charging then
```

---
## \#28 Posted by: willpark16 Posted at: 2016-08-08T05:13:51.189Z Reads: 134

```
@Pantologist @barajabali @Michaelinvegas thanks guys!
```

---
## \#29 Posted by: zk8_builder Posted at: 2016-08-09T07:16:36.568Z Reads: 121

```
Is @whitepony most recent build without a bms
```

---
## \#30 Posted by: DilatedPupils Posted at: 2016-08-09T08:39:07.204Z Reads: 114

```
What charger do you use if you don't use bms?
```

---
## \#31 Posted by: Michaelinvegas Posted at: 2016-08-09T12:41:35.342Z Reads: 107

```
https://youtu.be/0Z5QWzSSvdI

DIY a charger for a battery pack without a bms 




https://www.amazon.com/gp/product/B01GFVI6R6/ref=as_li_ss_tl?ie=UTF8&psc=1&linkCode=sl1&tag=batter00-20&linkId=484a1902b5018199aa0604bc3078e670
```

---
## \#32 Posted by: lox897 Posted at: 2016-08-09T13:18:01.260Z Reads: 103

```
@whitepony doesn't use a BMS in any of his builds.
```

---
## \#33 Posted by: willpark16 Posted at: 2016-08-09T17:56:24.586Z Reads: 100

```
and this will still balance the cells?
```

---
## \#34 Posted by: mason Posted at: 2016-08-09T18:27:19.582Z Reads: 100

```
please, humor me and go the amazon page for it.

does it say anywhere on that page that it has balancing cababilities? 
either way, it doesn't have a balance plug!!
```

---
## \#35 Posted by: willpark16 Posted at: 2016-08-09T18:58:56.108Z Reads: 94

```
so is that a no kid?
```

---
## \#36 Posted by: Michaelinvegas Posted at: 2016-08-09T19:06:23.041Z Reads: 94

```
No it won't balance ..... But will allow you to choose an end voltage ... For example .... Is you have a 12s set up with out a bms ... You really wouldn't want to charge it to 50.4v.... You would want to end it @ 50v ...
```

---
## \#37 Posted by: willpark16 Posted at: 2016-08-09T19:07:37.915Z Reads: 93

```
ahhh thanks that clears it up
```

---
## \#38 Posted by: Michaelinvegas Posted at: 2016-08-09T19:09:48.952Z Reads: 92

```
If you have no bms...you need to give yourself a bigger range to play with so you don't over discharge and don't over charge ... Plus will extend the amount of cycles you can charge
```

---
## \#39 Posted by: Namasaki Posted at: 2016-08-09T23:18:40.068Z Reads: 88

```
I would never suggest or even think of running Li-ion or Lipo or Lifepo cells without at least balance charging them.
```

---
## \#40 Posted by: Namasaki Posted at: 2016-08-09T23:20:40.512Z Reads: 83

```
If you want to go 30+ mph, your gonna need all the power you can get. I would suggest 12s Lipos for that kind of power.
```

---
## \#41 Posted by: Namasaki Posted at: 2016-08-09T23:22:26.902Z Reads: 82

```
I went from 12s Lipo with 230kv motors to 10s Li-ion with 190kv motors and gave up a lot of power on the low end and abt 8mph on the top end.
```

---
## \#42 Posted by: Michaelinvegas Posted at: 2016-08-09T23:39:49.658Z Reads: 83

```
Shouldn't you have done the motors the other way? 190kv at 12s  etc...?
```

---
## \#43 Posted by: Jinra Posted at: 2016-08-09T23:45:54.856Z Reads: 84

```
I go 30mph on my 10s 200kv dual build :)
```

---
## \#44 Posted by: Namasaki Posted at: 2016-08-09T23:47:40.962Z Reads: 84

```
I was gearing up for the vesc's that I ordered. Thats why I went 190kv at 10s to keep the erpm at safe level.
```

---
## \#45 Posted by: Namasaki Posted at: 2016-08-09T23:49:00.408Z Reads: 84

```
I'm around 188lbs and I'm only getting a top speed of about 23mph with dual 190kv motors 10s li-ions and TB 12s Esc's
15/36 gears 90mm wheels
```

---
## \#46 Posted by: Jinra Posted at: 2016-08-09T23:49:44.220Z Reads: 81

```
What gearing? I'm not that much lighter at 175lbs. I'm sure i hit 190 with my backpack on, which I always have on. I'm running 16/36 83mm wheels.

EDIT: gotcha
```

---
## \#47 Posted by: Namasaki Posted at: 2016-08-09T23:50:19.533Z Reads: 79

```
are you using Vesc?
Li-ions or Lipos?
```

---
## \#48 Posted by: Jinra Posted at: 2016-08-09T23:51:03.338Z Reads: 78

```
Yep. I guess it might be because I'm using current control and you're using duty cycle.
```

---
## \#49 Posted by: Namasaki Posted at: 2016-08-09T23:51:51.492Z Reads: 78

```
I can't wait to try that current control!
```

---
## \#50 Posted by: Michaelinvegas Posted at: 2016-08-09T23:52:12.768Z Reads: 80

```
Oh so you haven't switched over to a vesc
```

---
## \#51 Posted by: Namasaki Posted at: 2016-08-09T23:52:29.676Z Reads: 83

```
haven't got um yet
```

---
## \#52 Posted by: Namasaki Posted at: 2016-08-09T23:53:06.364Z Reads: 84

```
are you using Lipos?
```

---
## \#53 Posted by: Jinra Posted at: 2016-08-09T23:53:37.242Z Reads: 82

```
I guess that explains why esk8 calculator isn't very accurate for you too!

I'm using the space cell pro 4, so Samsung 25R cells. VESC settings are 35A per VESC battery discharge max (70A total).
```

---
## \#54 Posted by: Namasaki Posted at: 2016-08-09T23:55:24.846Z Reads: 82

```
when I was running 12s lipos 16/36 gears 90mm wheels 230kv motors and TB12s esc's, I was only getting 28mph top
```

---
## \#55 Posted by: Namasaki Posted at: 2016-08-09T23:55:58.346Z Reads: 76

```
what motors are you running
```

---
## \#56 Posted by: Jinra Posted at: 2016-08-09T23:56:19.034Z Reads: 76

```
chaka's OM5065 200kv motors.
```

---
## \#57 Posted by: Jinra Posted at: 2016-08-09T23:58:24.518Z Reads: 82

```
This was high but not full battery.

<img src="/uploads/db1493/original/2X/f/f604159a9f53e855991774826c07c231e3d43d16.png" width="281" height="500">
```

---
## \#58 Posted by: barajabali Posted at: 2016-08-10T00:00:38.387Z Reads: 76

```
A BMS or lipo charger will balance the cells every time it charges it fully. 
Do cells need to be balanced every time it's charged? No but it is safer, makes them last longer and increases performance of the cells. 

That doesn't mean you never need to balance them if you go this route you'll prob need to manually balance them with the power supply once in a while
```

---
## \#59 Posted by: Namasaki Posted at: 2016-08-10T00:02:27.921Z Reads: 81

```
<img src="/uploads/db1493/original/2X/e/e3a3eedb8a8e8525c2d6439c15e4292e660a5bf7.png" width="281" height="500">
<img src="/uploads/db1493/original/2X/2/27ff18d4e1cbbcf5af40113215bde728f9e90c6b.png" width="281" height="500">
Looks like dropping 2s and 1 pulley tooth and 40kv cost me 10mph
Like when you go grocery shopping and get to the register. It really adds up.
Thats ok, I don't need to go 30mph anyway. I'm 58 and I need to start taking it a little easier.
Although my balance and reflexes are pretty good for an old guy. I've handled a couple situations going over 30mph including speed wobble and managed to stay on.
```

---
## \#60 Posted by: Jinra Posted at: 2016-08-10T00:07:23.776Z Reads: 73

```
That calculator doesn't seem accurate. I've done the math manually and toddy and makevoids calculators make sense to me. According to those youre 230kv 12s setup should get 47mph at full efficiency, but at that speed efficiency goes down the toilet. Either way you should be going VERY fast, faster than me. But again, this could be due to using duty cycle over current control as well, not sure.
```

---
## \#61 Posted by: Namasaki Posted at: 2016-08-10T00:08:38.745Z Reads: 75

```
Speed calculators never factor in rider weight or wind resistance . Thats what I use the trans ration for.
```

---
## \#62 Posted by: Jinra Posted at: 2016-08-10T00:09:39.201Z Reads: 73

```
Weight becomes less of an issue as motors get up to speed and start spinning at max efficiency. I find it not as big a factor as hills, especially on beefier motors like yours.
```

---
## \#63 Posted by: Namasaki Posted at: 2016-08-10T00:10:47.166Z Reads: 76

```
even when your full throttle on flat ground, weight and wind resistance are still extra load
```

---
## \#64 Posted by: Michaelinvegas Posted at: 2016-08-10T00:11:19.050Z Reads: 75

```
True....

But if you charge your pack just under voltage say on a 12s to 50v Max and only discharge let's say to 3v per cell.....then back on charge to 50v   ... Discrepancies in battery voltage will not really matter....plus you extend he life of your batteries....

If I was gonna do this myself ...id build a 12s3p pack but treat it like it was a 12s2p...id have pleanty of room on the top and bottom and would only periodically check the cells individually

Edit: on the condition each cell is working perfectly lol
```

---
## \#65 Posted by: Jinra Posted at: 2016-08-10T00:11:29.138Z Reads: 72

```
It is load, but most of it is already being taken away from the motor into momentum. I agree on the wind resistance part though.
```

---
## \#66 Posted by: Namasaki Posted at: 2016-08-10T00:12:50.624Z Reads: 69

```
try testing your speed with and without your backpack and see if it makes a difference. Put say 10 lbs in you pack.
```

---
## \#67 Posted by: Jinra Posted at: 2016-08-10T00:13:18.416Z Reads: 70

```
My pack is about 15 pounds, but I've ridden my board without it. Not much change on flats.
```

---
## \#68 Posted by: barajabali Posted at: 2016-08-10T00:13:28.697Z Reads: 69

```
All this capacity not being used just to avoid using a BMS. 

A BMS charger combo is like 115 bucks depending on sources. It's worth being able to use your cells fully and have them live longer
```

---
## \#69 Posted by: Namasaki Posted at: 2016-08-10T00:13:52.737Z Reads: 68

```
Wind resistance can be huge, once I burned up my hv switch because I was riding into a strong wind. everything got really hot
```

---
## \#70 Posted by: Jinra Posted at: 2016-08-10T00:14:25.582Z Reads: 68

```
For sure. My commute home has a ton of resistance and can make my motors burning hot, but on the way there it only gets a bit warm.
```

---
## \#71 Posted by: Namasaki Posted at: 2016-08-10T00:15:31.676Z Reads: 63

```
I totally agree with you. BMS is the only way to go.
```

---
## \#72 Posted by: Namasaki Posted at: 2016-08-10T00:18:46.737Z Reads: 63

```
I changed some settings on my Esc's. gonna go see if that helped.
went from normal timing and medium acceleration to
high timing and low acceleration.
on this esc, lowering the acceleration moves the power band to lower rpm.
on medium, I only had power at almost full throttle so I think It may have been set outside my rpm range.
```

---
## \#73 Posted by: Namasaki Posted at: 2016-08-10T00:21:19.908Z Reads: 65

```
gonna go cruise down to my daughter's house and see what my grandson is up to.
be back in little while with the results.
```

---
## \#74 Posted by: Jinra Posted at: 2016-08-10T00:22:25.266Z Reads: 68

```
Let me know! I have no experience at all with regular ESCs.
```

---
## \#75 Posted by: Namasaki Posted at: 2016-08-10T00:54:09.653Z Reads: 65

```
Seems like I had a little more power on the low end. But no more speed at the top end. 
It will be interesting to see how the Vesc does
My battery drops from 97% to 30% while going full throttle up 10% hill
Voltage sag blues
I had a lot more power with my Lipo setup.
```

---
## \#76 Posted by: Jinra Posted at: 2016-08-10T00:56:41.090Z Reads: 64

```
Wow that's a huge drop! Is this on your Basen setup? I imagine it's because of the low discharge rate at 2P.
```

---
## \#77 Posted by: Namasaki Posted at: 2016-08-10T01:32:44.411Z Reads: 65

```
Yes it is the Basen pack. It does fine on flat ground or slight inclines but chokes on steep hills. 
I've done the same hill with 6s x 2 in parallel and only pulled around 34a from the battery. 
So I thought that 10s 2p would be sufficient. 
Don't have room for 10 more cells to make a 3p. 
I might see about making a Lipo 10s flat pack.
```

---
## \#78 Posted by: Namasaki Posted at: 2016-08-10T03:18:15.332Z Reads: 65

```
Actually after cruising around the neighborhood for a bit,  I realize that this basen pack is just fine for cruising,  just not for storming steep hills.
```

---
