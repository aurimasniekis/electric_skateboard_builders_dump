# New ESK8 Calculator in wild

### Replies: 140 Views: 5620

## \#1 Posted by: Kug3lis Posted at: 2018-11-13T02:12:45.294Z Reads: 863

```
Got really sad then my favourite calculator which I was opening more than once a day got closed so I spent today's evening trying to my own small implementation which I will try to add lots of features.

### Todo List:

* Shareable URL which would save your inputs
* Recommended VESC current ratings based on inputs
* Add many style graphs for e.g. (motor/bat current duty cycle relationship), (battery voltage/speed relationship)

https://calc.3dservisas.eu/

If someone has some more ideas hit them up I will try to implement them all :)
```

---
## \#2 Posted by: skatardude10 Posted at: 2018-11-13T02:19:55.318Z Reads: 591

```
Nice! I too got very sad to see it go down, thanks for putting in the work for a replacement! 

Some feedback, Your watt hour calc looks wrong though, shouldn't you use nominal voltage instead of full charge voltage?

Second, it would be nice to be able to input max amp charge rate instead of just C rating... And choose A or mAh on capacity.
```

---
## \#3 Posted by: Kug3lis Posted at: 2018-11-13T02:22:21.876Z Reads: 535

```
[quote="skatardude10, post:2, topic:74497"]
Your watt hour calc looks wrong though, shouldn’t you use nominal voltage instead of full charge voltage?
[/quote]

I always counted Wh with max voltage as it's still usable watt hours :slight_smile:

[quote="skatardude10, post:2, topic:74497"]
Second, it would be nice to be able to input max amp charge rate instead of just C rating… And choose A or mAh on capacity.
[/quote]

I will implement this later on, this was quick iteration :) I wanted to keep simple. I don't know many other 18650 cells which allow more than for e.g. 2C charging current and lipos are all C rated :)
```

---
## \#4 Posted by: skatardude10 Posted at: 2018-11-13T02:26:39.636Z Reads: 457

```
What does the currents section mean? My 10S4P 20A 2500mah cells are saying 350A constant discharge? I think that should be 80? Something to look at there? 

Same with the power, the numbers seem off by a power of ten, but if corrected still slightly lower than I'd expect.
```

---
## \#5 Posted by: Kug3lis Posted at: 2018-11-13T02:33:29.070Z Reads: 419

```
Opsy :sweat_smile: copied bit too much code from wrong place :) Fixed should work correctly :)
```

---
## \#6 Posted by: skatardude10 Posted at: 2018-11-13T02:38:00.967Z Reads: 409

```
Nice, looks just right now! 😎😎
```

---
## \#7 Posted by: Jake2k17 Posted at: 2018-11-13T02:46:52.968Z Reads: 392

```
@Kug3lis
My hero! :smile:
```

---
## \#8 Posted by: Kug3lis Posted at: 2018-11-13T02:48:54.414Z Reads: 390

```
This is how my crazy 2 x 80100 setup looks :) Looks pretty accurate... :D 72Nm drive train... Polo 1.2 has 107Nm iirc :D 

![image|315x499](upload://ljUMmozzEC1EtAN6HLuUb9Zm5S3.png)
```

---
## \#9 Posted by: Bor.inc Posted at: 2018-11-13T08:40:20.279Z Reads: 330

```
Wow well done already
I have it that the numbers of the results are cut in half because the borders are very little (if you understand what i say) I see that you don't have that so how can I fix it? or is it a bug
```

---
## \#10 Posted by: martijntje42 Posted at: 2018-11-13T08:55:06.151Z Reads: 324

```
Looking awesome, battery options are really nice and understandable. Just a quick question, I'm guessing motor wattage is per motor?
```

---
## \#11 Posted by: Maxid Posted at: 2018-11-13T08:56:25.894Z Reads: 318

```
[quote="Kug3lis, post:3, topic:74497, full:true"]
I always counted Wh with max voltage as it's still usable watt hours :slight_smile:
[/quote]
Seems wrong to me - Wh is the total energy in your pack. You don't use the pack at 42V all the time. The reason to use the nominal voltage is that it gives a good estimate for the average voltage the pack will be at. Some time will be at higher than nominal while around the same time will be spent below the nominal voltage.
See this for a quick and dirty illustration of what I mean.

Edit2: Even more obvious: an actual Wh graph from [lygyte](https://lygte-info.dk/review/batteries2012/Samsung%20INR18650-30Q%203000mAh%20(Pink)%20UK.html)
![image|690x345](upload://t2iozqkZDZD9kOamQ5bzg7AdVwP.png) 
so we see a single 30Q has around 10 to 11 Wh - which can be estimated quite well with 3.6*3000mAh.
```

---
## \#12 Posted by: nuttyjeff Posted at: 2018-11-13T08:58:43.219Z Reads: 271

```
This. 10char
```

---
## \#13 Posted by: pat.speed Posted at: 2018-11-13T09:49:02.588Z Reads: 263

```
I don't think the lipo selection is working, I can't seem to get data to work while using a lipo set up. I did just change to 18650 and put in the correct values and it's great. Love how it displays torque output, that would be fun for comparing. IDK how you are making 72Nm mine says 7Nm lol

Great work man
```

---
## \#14 Posted by: Sebike Posted at: 2018-11-13T09:55:23.539Z Reads: 255

```
Nice work! It would be nice to be able to set the exact kv value though
```

---
## \#15 Posted by: pat.speed Posted at: 2018-11-13T09:58:38.348Z Reads: 254

```
It does, does it not? isn't it called speed/volt
```

---
## \#16 Posted by: Pedrodemio Posted at: 2018-11-13T10:02:32.002Z Reads: 257

```
Nice work @Kug3lis

I think the range estimation is wrong by a factor of 2, maybe something do with the number of motors, a 370Wh battery is only giving me 19km of range using 10 Wh/km

I would like to have maximum grade and what speed it can climb that maximum grade based on the maximum duty cycle that respects the battery maximum current proportional to motor max current

If you want I have the formulas ready in my own spreadsheet
```

---
## \#17 Posted by: Sebike Posted at: 2018-11-13T10:03:26.721Z Reads: 241

```
you can set it to 170, 180, 190 aso. Typing in other values highlights the box as if it's not an accepted value (?)
```

---
## \#18 Posted by: Sebike Posted at: 2018-11-13T10:05:04.539Z Reads: 246

```
Wh consumption is for one motor, so even if you have 2 motors, you should enter value for one motor only. Range looked right to me anyway
```

---
## \#19 Posted by: Gustdd Posted at: 2018-11-13T10:24:44.493Z Reads: 244

```
Would you consider opening the source code for the calculator? I could help you implement somethings.

For example, a toggle for metric/imperial instead of having both at all times.
```

---
## \#20 Posted by: Pedrodemio Posted at: 2018-11-13T10:26:48.599Z Reads: 242

```
That makes no sense, consumption is a variable of the system, you don’t say your car does 10 mpg per piston
```

---
## \#21 Posted by: Kug3lis Posted at: 2018-11-13T10:42:38.675Z Reads: 206

```
What size is your screen?
```

---
## \#22 Posted by: Kug3lis Posted at: 2018-11-13T10:43:06.515Z Reads: 200

```
Yes, its just to calculate max current and torque of the motor :)
```

---
## \#23 Posted by: Kug3lis Posted at: 2018-11-13T10:43:25.968Z Reads: 203

```
Will change it, I always used my top voltage :)
```

---
## \#24 Posted by: Kug3lis Posted at: 2018-11-13T10:43:58.472Z Reads: 200

```
Can you send me PM with some pictures what are you trying to type?
```

---
## \#25 Posted by: Kug3lis Posted at: 2018-11-13T10:44:47.394Z Reads: 197

```
Ahm, I added it to be steps of 10kv as it usually the case will change it :)
```

---
## \#26 Posted by: Kug3lis Posted at: 2018-11-13T10:45:27.046Z Reads: 192

```
If you would like to share the formulas I would implement it, after quick search I didn't found anything online.
```

---
## \#27 Posted by: Kug3lis Posted at: 2018-11-13T10:46:16.116Z Reads: 188

```
I will open up after I have done basics which I want to implement. Also I will fix how units work. I have done this in 3h evening so don't expect much from first iteration :D
```

---
## \#28 Posted by: Kug3lis Posted at: 2018-11-13T10:47:31.682Z Reads: 185

```
well there weren't any calculators which would calculate more than one motor :) I added avg. consumption per motor as you only have access to one vesc usually to get info about consumption you enter that and I multiple by motor configuration.
```

---
## \#29 Posted by: nuttyjeff Posted at: 2018-11-13T10:47:46.919Z Reads: 186

```
Great job. Thanks loads for the calc btw.
```

---
## \#30 Posted by: Kug3lis Posted at: 2018-11-13T10:48:22.213Z Reads: 185

```
Haha thanks no worries :) calc.esk8.today was my homepage basically :D
```

---
## \#31 Posted by: Pedrodemio Posted at: 2018-11-13T10:50:42.841Z Reads: 186

```
I can put them individually later

here is my old spread sheet that has them, sorry but they are kind of a mess, the new one is much better but doesn't have this peak grade part since it's build in the graph, maybe there is something you can use

Old one:

https://drive.google.com/file/d/0B64MF1WJuj0yQUdTcEpSNGJzLVk/view?usp=sharing

New one:

https://drive.google.com/file/d/15gsz0LiEjiuLc3wVriNmjd10ry1jlA7j/view?usp=sharing
```

---
## \#32 Posted by: Gustdd Posted at: 2018-11-13T11:08:19.792Z Reads: 175

```
If you need any help I would be glad to. I'm profiting from your work afterall.
```

---
## \#33 Posted by: Komamtb Posted at: 2018-11-13T11:32:11.240Z Reads: 168

```
Can the average 63km/h be realistic with 190kv 16/38 on 12s with 97mm wheels?
```

---
## \#34 Posted by: pat.speed Posted at: 2018-11-13T11:35:33.369Z Reads: 167

```
Was it average weighted speed?
```

---
## \#35 Posted by: Kug3lis Posted at: 2018-11-13T11:36:22.595Z Reads: 178

```
![image|447x500](upload://sl9qFXNJ5OzGmAQiPoimZN6xd0D.png) 

old calc

![image|278x499](upload://4xJbNVe9k2fH4RiDx5HIY2SYmgQ.png)
```

---
## \#36 Posted by: Bor.inc Posted at: 2018-11-13T12:03:05.558Z Reads: 158

```
13inch?
10char
```

---
## \#37 Posted by: esk8jpn Posted at: 2018-11-13T12:37:41.403Z Reads: 158

```
Wow, Nice work!!! :+1: :+1: :+1:
I like that site and always used it.
```

---
## \#38 Posted by: Kug3lis Posted at: 2018-11-13T12:48:43.133Z Reads: 164

```
@Gustdd here you go made it public :) https://github.com/aurimasniekis/esk8_calc

@Pedrodemio @Maxid  added avg Wh and max Wh :)

@Bor.inc fixed the the issue with smaller screens now should be better

@pat.speed added total torque :)

Next is to make shareable urls :)

http://calc.3dservisas.eu
```

---
## \#39 Posted by: Kug3lis Posted at: 2018-11-13T14:48:46.087Z Reads: 169

```
Added some features:

* Browser history now after each change you can go back to previous and see difference.
* Now you can share your calculation result with all inputs preserved by copying url

For e.g. this is my build:

https://calc.3dservisas.eu/?Nc6xDsIwDATQf_HMkDRtKawBMSFFqkR36FAkokTqWPHv-M50e3acszd5xkXO8nnXIgdZ46iFb8ikbKmoCs45FhdUvjNjprE-c7yyIiMAmOztX03jP66mtL8zKnQkmj1pQeBrsc3kVXkK5ANbW7QzBnBu5uEDe6nALak62gU5lv3YeVpJpM23u3qgJpzIAS5z8v0B
```

---
## \#40 Posted by: FredrikHems Posted at: 2018-11-13T14:55:19.254Z Reads: 165

```
[quote="Kug3lis, post:8, topic:74497"]
This is how my crazy 2 x 80100 setup looks :slight_smile: Looks pretty accurate… :smiley: 72Nm drive train… Polo 1.2 has 107Nm iirc :smiley:
[/quote] 
This is the torque after reduction, right? Afaik torque in vehicles are measured at the engine shaft, not wheel axle. Still impressive though
```

---
## \#41 Posted by: Kug3lis Posted at: 2018-11-13T14:55:40.313Z Reads: 152

```
[quote="FredrikHems, post:40, topic:74497"]
This is the torque after reduction, right? Afaik torque in vehicles are measured at the engine shaft, not wheel axle. Still impressive though
[/quote]

Oh right... :( NVM means my board can spin car engine shaft :D
```

---
## \#42 Posted by: Pedrodemio Posted at: 2018-11-13T16:33:09.793Z Reads: 133

```
On the subject of torque, you could the force that the wheels put to the ground, way more meaningful when comparing board with different wheel sizes
```

---
## \#43 Posted by: Kug3lis Posted at: 2018-11-13T16:34:18.520Z Reads: 130

```
I have some thoughts regarding comparison between multiple things but that's for later on :)
```

---
## \#44 Posted by: Maxid Posted at: 2018-11-13T17:13:40.587Z Reads: 129

```
But there is no such thing as average or max watt hours. The pack has a defined amount of total available energy.
```

---
## \#45 Posted by: Kug3lis Posted at: 2018-11-13T17:15:53.068Z Reads: 128

```
Yes, but you know that fully charged on will discharge more Wh than your Wh rating on nominal cell voltage?

EDIT: that's especially the case with lipos ;) As nominal cell voltage is 3.7V but dead is at 3.4V ;)
```

---
## \#46 Posted by: Maxid Posted at: 2018-11-13T17:17:29.261Z Reads: 126

```
No it will not - wh is energy what you are talking about is power (at least I think that's what you mean) - that's a different thing.
Also you'd have to look at a lipo discharge like I showed above which will show you that the energy inside your battery will be estimated very well with the formula nominal voltage*capacity.
```

---
## \#47 Posted by: Kug3lis Posted at: 2018-11-13T17:21:12.681Z Reads: 128

```
Yes, I understand but why then I consume more Wh from battery according logs than Wh calculated according to you?
```

---
## \#48 Posted by: Maxid Posted at: 2018-11-13T17:35:11.825Z Reads: 129

```
Thats interesting - How big of a difference are we talking about?
I am just saying that the wording is not right with max and average Wh for a battery - there can only be one total energy the pack has. About the topic whether nominal voltage*capacity actually represents the energy in a Lipo well, is a different story and I am happy to discuss and learn.
```

---
## \#49 Posted by: Kug3lis Posted at: 2018-11-13T17:36:50.862Z Reads: 132

```
If you have suggestion for wording I can change as I am not specialist in naming things :D But regarding capacity I am usually getting near 900Wh so according nominal voltage another whole hundred 100Wh :)
```

---
## \#50 Posted by: Pedrodemio Posted at: 2018-11-13T17:43:43.386Z Reads: 129

```
There is something wrong somewhere then

What cells are you using and what configuration? Energy is simply work integrated over time, what could be wrong is your nominal voltage, for example, 3.6V volts works well with Li-Ion, but if you use that with Lipo to do a roughly energy estimation your result will be less than what actually the battery can store
```

---
## \#51 Posted by: Kug3lis Posted at: 2018-11-13T17:45:21.239Z Reads: 121

```
nah I use 3.7V for nominal and Turnigy Graphenes :) Maybe it's Graphene making magic don't know :) I just wanted to add that number for myself as I planning to use the same packs in future projects too :)
```

---
## \#52 Posted by: Maxid Posted at: 2018-11-13T17:49:40.748Z Reads: 125

```
My guess is that your capacity is just slightly higher than what is printed on the box. 100Wh at 900Wh is roughly 10% - not unheard of that a say 5000mAh Lipo actually has 5500mAh especially considering you are using the more expensive graphene ones. I'd say that the formula still holds and with brand name Liions we can be sure that the capacity is not 10% above the rated one. For HK Lipos etc. capacities might be a bit off.

I'd just use the nominal*capacity calculation in your calculator and simply call it energy (or battery energy or total pack energy or whatever you want that gets the point across).
```

---
## \#53 Posted by: professor_shartsis Posted at: 2018-11-13T18:02:40.285Z Reads: 129

```
https://image.ibb.co/inPuKf/course-1.jpg

^suppose i'll be climbing 1.8miles on a steady 5% grade... 

i have 4x 190kv 0.05ohm motors &amp; 83mm tires, 120a motor current and 60a battery current limit per motor, & 13S (48.1v)

what's my maximum top speed up slope and what gear ratio gives this top speed assuming 0.6m^2 frontal area, 0.75 drag coefficient & 200lbs?
```

---
## \#54 Posted by: Kug3lis Posted at: 2018-11-13T18:05:10.196Z Reads: 127

```
[quote="professor_shartsis, post:53, topic:74497"]
^suppose i’ll be climbing 1.8miles on a steady 5% grade…

i have 4x 190kv 0.05ohm motors &amp; 83mm tires, 120a motor current and 60a battery current limit per motor, &amp; 13S (48.1v)

what’s my maximum top speed up slope and what gear ratio gives this top speed assuming 0.6m^2 frontal area, 0.75 drag coefficient &amp; 200lbs?
[/quote]

?

1000char
```

---
## \#55 Posted by: professor_shartsis Posted at: 2018-11-13T18:06:54.732Z Reads: 119

```
i have no idea! :smiley:
```

---
## \#56 Posted by: psychotiller Posted at: 2018-11-13T18:08:31.576Z Reads: 113

```
This looks great!! Thank you
```

---
## \#57 Posted by: Kug3lis Posted at: 2018-11-13T18:08:44.347Z Reads: 118

```
[quote="professor_shartsis, post:55, topic:74497"]
i have no idea! :smiley:
[/quote]

I have no idea too? Did you post it as a question?
```

---
## \#58 Posted by: pat.speed Posted at: 2018-11-13T20:08:43.254Z Reads: 126

```
Maybe this could help

Taken from a go kart forum

**Force Hill = Weight Go Kart * SIN(Angle Hill)**

The typical hill is 10 degrees and the sin for 10 degrees is .17

So the Balancing force to just hold the go kart in place on the hill is for example:

(228 (gokart) Lb + 185 (person)lbs )*.17 = 70.21 lbs

The next step is to calculate what the go kart will do with the horsepower it has.  So we go through the calculations covered in Go Kart Building 201 and come up with a force that is pushing the go kart:

Force Go Kart  = (Te* Rd/Re*Rw)

Te = Torque Engine = 59 in-lbs
Rd = Radius Drive Sprocket = 4.3 inches
Re = Radius Clutch Sprocket = .60 inches
Rw = Radius Wheel = 6.5 inches

Force Go Kart = 48.41 lbs

**As you can see the force that the engine**  will push the go kart is 65 lbs, to climb a hill it must put out 70.21 lbs.  The go kart will actually go backwards down the hill with this set up, because the amount of downhill force is greater than the engine can deliver.

The go kart to be exact will go down the hill at – 5lbs/12 slugs = .41 ft/sec^2 which  **would appear like a slow crawl backwards.**
```

---
## \#59 Posted by: Battosaii Posted at: 2018-11-13T20:31:01.442Z Reads: 118

```
Says my max speed loaded would be 58mph but I'm expecting 50mph in reality.
```

---
## \#60 Posted by: Kug3lis Posted at: 2018-11-13T20:31:55.853Z Reads: 120

```
[quote="Battosaii, post:59, topic:74497, full:true"]
Says my max speed loaded would be 58mph but I’m expecting 50mph in reality.
[/quote]

Depending on capacity but by the time you reach your top speed your voltage will be probable down a bit which would limit your speed :)
```

---
## \#61 Posted by: pat.speed Posted at: 2018-11-13T20:51:00.528Z Reads: 116

```
Also voltage sag
```

---
## \#62 Posted by: dg798 Posted at: 2018-11-13T21:54:02.731Z Reads: 120

```
I think this thread should be pinned.
Anyone agree
@mmaner @Namasaki @treenutter
```

---
## \#63 Posted by: professor_shartsis Posted at: 2018-11-13T22:21:50.932Z Reads: 130

```
[quote="professor_shartsis, post:53, topic:74497"]
^suppose i’ll be climbing 1.8miles on a steady 5% grade…

i have 4x 190kv 0.05ohm motors &amp; 83mm tires, 120a motor current and 60a battery current limit per motor, &amp; 13S (48.1v)

what’s my maximum top speed up slope and what gear ratio gives this top speed assuming 0.6m^2 frontal area, 0.75 drag coefficient &amp; 200lbs?
[/quote]

[quote="Kug3lis, post:54, topic:74497"]
?
[/quote]

i went ahead and solved this:

60a battery limit / 95% duty = **63.1578a motor current at peak mechanical power**

63.1578a^2 * 0.05ohm = **199.445385042w copper loss per motor at peak mechanical power**

60a battery limit * 48.1v battery = **2886w electrical power at peak mechanical power**

2886w peak electrical - 199.445385042w copper loss = **2686.554614958w peak mechanical power per motor**

2686.554614958w peak mechanical power per motor * 4 motors = **10746.218459832w peak mechanical**

60 / (190kv * 2 * pi) = **0.05025945571323010603228Nm per motor amp**

63.1578a * 0.05025945571323010603228Nm per motor amp = **3.174276652045044390766 Nm torque at peak mechanical power**

2686.554614958w peak mechanical / 3.174276652045044390766 Nm = **846.3517548878964569933rad/sec @ peak mechanical**

(60 / (2 * pi)) * 846.3517548878964569933rad/sec = **8082.063923094534641801 motor rpm @ peak mechanical power**

**^peak mechanical power is 10746.218459832w @ 8082.063923094534641801 motor rpm**

A = meters per second = XX.XXX
B = drag coefficient = 0.75
C = frontal area = 0.6m^2
D = fluid density of air = 1.225kg/m^3
E = wind drag force in watts
F = sine of 5% slope = sin(atan(5/100)) = 0.04993761694389223373491
G = acceleration of gravity = 9.80655m/s^2
H = vehicle mass in kg = 90.7184kg = 200lb / 2.20462lb/kg
I = mechanical watts required for constant speed up slope with no wind drag
J = mechanical watts required for constant speed up slope including wind drag
K = H * G * F
L = (1/2) * D * C * B

E = ((1/2) * D * C * (A^2) * B) * A

I = H * G * A * F

J = E + I

J = (((1/2) * D * C *(A^2) * B) * A) + (H * G * A * F)

J = (1/2) * D * C * B * A^3 + H * G * F * A

J = (L * A^3) + (K * A)

^this can be rearranged to:

A=(sqrt(3) * sqrt(27 * J^2 * L^4 + 4 * K^3 * L^3) + 9 * J * L^2)^(1 / 3) / (2^(1 / 3) * 3^(2 / 3) * L) - ((2 / 3)^(1 / 3) * K) / (sqrt(3) * sqrt(27 * J^2 * L^4 + 4 * K^3 * L^3) + 9 * J * L^2)^(1 / 3)

we know:

J = 10746.218459832w peak mechanical
L = 0.275625 = (1/2) * D * C * B
K = 44.42622815547907982077 = H * G * F

therefore:

A=(sqrt(3) * sqrt(27 * 10746.218459832^2 * 0.275625^4 + 4 * 44.42622815547907982077^3 * 0.275625^3) + 9 * 10746.218459832 * 0.275625^2)^(1 / 3) / (2^(1 / 3) * 3^(2 / 3) * 0.275625) - ((2 / 3)^(1 / 3) * 44.42622815547907982077) / (sqrt(3) * sqrt(27 * 10746.218459832^2 * 0.275625^4 + 4 * 44.42622815547907982077^3 * 0.275625^3) + 9 * 10746.218459832 * 0.275625^2)^(1 / 3)

A=**32.32551993764664323864 meters per second**

**^therefore the peak velocity up slope is 32.32551993764664323864 meters per second**

**72.31024856931928212624mph** = 32.32551993764664323864 meters per second * 2.23694 mph per m/s

**^72.31mph is the maximum possible top speed up 5% slope w/ 200lbs, 0.75 drag coefficient, 0.6m^2 frontal area, 4x 190kv 0.05ohm motors & 120a motor current limit & 60a battery current limit per motor w/ 48.1v battery**

therefore we need:

8082.063923094534641801 motor rpm @ peak mechanical power @ 72.31024856931928212624mph w/ 83mm tires

83mm * pi = 260.7521902479528387924mm per rotation

1mph = 0.44704 meters per second

72.31024856931928212624mph * 0.44704 meters per second per mph = 32.32551993764664323864 meters per second

32.32551993764664323864 meters per second * 1000mm per meter = 32325.51993764664323864mm per second

32325.51993764664323864mm per second / 260.7521902479528387924mm per rotation = 123.9702719540260136714 tire rotations per second

123.9702719540260136714 tire rotations per second * 60 seconds per minute = **7438.216317241560820284 wheel rpm required for 72.31024856931928212624mph @ 83mm tire diameter**

8082.063923094534641801 motor rpm / 7438.216317241560820284 wheel rpm = **1.086559408652925905457 gear ratio**

^**1.08:1 gear ratio is needed to obtain maximum possible 72.31mph top speed up 5% slope w/ 200lbs**, 0.6m^2 frontal area, 0.75 drag coefficient, 4x 190kv 0.05ohm motors, 83mm tires, 120a motor current limit, 60a battery current limit per motor & 48.1v (13S) battery

answer:

**72.31mph & 1.08:1 gear ratio**
```

---
## \#64 Posted by: Kug3lis Posted at: 2018-11-13T22:23:58.071Z Reads: 114

```
In ideal world ;)
```

---
## \#65 Posted by: professor_shartsis Posted at: 2018-11-13T23:16:30.169Z Reads: 119

```
https://image.ibb.co/inPuKf/course-1.jpg
https://image.ibb.co/cnoVQL/70mph-5percent-1.jpg
https://image.ibb.co/ndAzKf/70mph-5percent-2.jpg
https://image.ibb.co/c86H5L/70mph-5percent-3.jpg

^graphed out it looks about like this 25T wheel & 23T motor = 1.088:1 ratio for ~72mph up 5% slope w/ 4x 190kv 0.05ohm, 83mm tires, 120a motor current and 60a battery current limit per motor, 13S (48.1v) w/ 200lbs, 0.6m^2 frontal area and 0.75drag coefficient.
```

---
## \#66 Posted by: pat.speed Posted at: 2018-11-14T04:52:01.977Z Reads: 101

```
I don’t really know what I just witnessed as I lost you at the point where the legend ended but great work. It seems like based on those calculations the NGV board has pretty similar specs with 170ish kv quad hub motors running at either 6s or 12s
```

---
## \#67 Posted by: professor_shartsis Posted at: 2018-11-14T05:02:55.186Z Reads: 120

```
[quote="pat.speed, post:66, topic:74497, full:true"]
I don’t really know what I just witnessed as I lost you at the point where the legend ended but great work. It seems like based on those calculations the NGV board has pretty similar specs with 170ish kv quad hub motors running at either 6s or 12s
[/quote]

[quote="professor_shartsis, post:63, topic:74497"]
J = (L * A^3) + (K * A)

^this can be rearranged to:

A=(sqrt(3) * sqrt(27 * J^2 * L^4 + 4 * K^3 * L^3) + 9 * J * L^2)^(1 / 3) / (2^(1 / 3) * 3^(2 / 3) * L) - ((2 / 3)^(1 / 3) * K) / (sqrt(3) * sqrt(27 * J^2 * L^4 + 4 * K^3 * L^3) + 9 * J * L^2)^(1 / 3)
[/quote]


^the hardest step was this... 

i'll admit i cheated...

https://www.wolframalpha.com/widgets/view.jsp?id=3d613c498715c870be91ed38004abc81

https://image.ibb.co/dXmjLL/rearrange-1.jpg

https://image.ibb.co/kkNPLL/rearrange-2.jpg
```

---
## \#68 Posted by: pat.speed Posted at: 2018-11-14T05:05:39.075Z Reads: 105

```
Haha, I use something like that in maths class when I can’t solve the answer and there isn’t an answer for me to check with. It’s called maths papa and it goes through all the steps, it’s rather helpful for rearranging things like that too
```

---
## \#69 Posted by: Kug3lis Posted at: 2018-11-15T13:31:36.714Z Reads: 103

```
Fixed some minor issues, I know people with Microsoft Edge has some issues I will try to address them later on :) In mean time use real browser :D

https://calc.3dservisas.eu
```

---
## \#70 Posted by: rusins Posted at: 2018-11-16T22:06:23.166Z Reads: 102

```
Really cool tool @Kug3lis! One suggestion I have is to add the formulas for how things are calculated either on the side, or as tooltips.

Specifically, I'm still confused as to how the estimated range is calculated. Reading this thread has made me no wiser on how much usuable WH a battery pack might have, and none of my guesses have matched the answer I get from the calculator :D
```

---
## \#71 Posted by: Kug3lis Posted at: 2018-11-16T22:12:45.576Z Reads: 102

```
[quote="rusins, post:70, topic:74497"]
Specifically, I’m still confused as to how the estimated range is calculated. Reading this thread has made me no wiser on how much usuable WH a battery pack might have, and none of my guesses have matched the answer I get from the calculator :smiley:
[/quote]

Ur battery Wh / (avg consumption next to motor * motor configuration)
```

---
## \#72 Posted by: rusins Posted at: 2018-11-16T22:20:46.379Z Reads: 100

```
Yup! Checks out! If that's true, then pretty crazy that having dual motors reduces range in half! Too bad I don't have a bluetooth module to test this myself. Thanks!
```

---
## \#73 Posted by: professor_shartsis Posted at: 2018-11-16T22:21:42.346Z Reads: 105

```
[quote="rusins, post:70, topic:74497"]
Specifically, I’m still confused as to how the estimated range is calculated.
[/quote]

[quote="professor_shartsis, post:63, topic:74497"]
A = meters per second = XX.XXX
B = drag coefficient = 0.75
C = frontal area = 0.6m^2
D = fluid density of air = 1.225kg/m^3
E = wind drag force in watts
F = sine of 5% slope = sin(atan(5/100)) = 0.04993761694389223373491
G = acceleration of gravity = 9.80655m/s^2
H = vehicle mass in kg = 90.7184kg = 200lb / 2.20462lb/kg
I = mechanical watts required for constant speed up slope with no wind drag
J = mechanical watts required for constant speed up slope including wind drag
K = H * G * F
L = (1/2) * D * C * B

E = ((1/2) * D * C * (A^2) * B) * A

I = H * G * A * F

J = E + I
[/quote]

@rusins 1st solve for J to calculate the mechanical load...
```

---
## \#74 Posted by: Kug3lis Posted at: 2018-11-16T22:22:57.164Z Reads: 95

```
Do you count this way your car tank mileage too? :D

Normally people use their average miles/galon Wh/mi or etc number to determine their range as that average number is based on their driving style and hardware :)
```

---
## \#75 Posted by: professor_shartsis Posted at: 2018-11-16T22:35:30.370Z Reads: 96

```
[quote="rusins, post:72, topic:74497"]
pretty crazy that having dual motors reduces range in half!
[/quote]


@rusins ...we can say that dual motors extends the range at constant speed for a given mechanical load (compared to single) because the total copper losses are cut in 1/2 (each motor needs half the motor current, which equates to ((1/2)^2 * 2) = 1/2 the losses...
```

---
## \#76 Posted by: rusins Posted at: 2018-11-16T23:02:23.873Z Reads: 97

```
Yeah, that's what I would have expected. I guess riding style from dual motors is what does the opposite?
```

---
## \#77 Posted by: professor_shartsis Posted at: 2018-11-16T23:09:09.581Z Reads: 98

```
@rusins what speed and quantity of mechanical watts are required for the range you want to calculate? and what is your kv, gear ratio, wheel size & # motors?
```

---
## \#78 Posted by: rusins Posted at: 2018-11-16T23:15:37.406Z Reads: 102

```
Why you need to know? :D I was just playing around with the calculator, I don't know the mechanical load off the top of my head.
```

---
## \#79 Posted by: neiru37 Posted at: 2018-11-17T01:18:24.182Z Reads: 104

```
Can the left side build config module be sticky when you scroll down in desktop mode? I want to be able to see stuff on the motor module for example, and modify the config to see what changes without having to scroll up again.

That or could you compress the right side modules so that we don't have to scroll.
```

---
## \#80 Posted by: pat.speed Posted at: 2018-11-17T05:34:07.109Z Reads: 98

```
I like this idea, would make it easier to see how things affect the outputs
```

---
## \#81 Posted by: mutantbass Posted at: 2018-11-17T12:57:02.440Z Reads: 94

```
I second the left hand side container to be sticky. Its annoying to scroll up to make changes and then go down to see the results and on and on.

thanks. good work :)
```

---
## \#82 Posted by: Kug3lis Posted at: 2018-11-17T15:46:04.365Z Reads: 92

```
@neiru37 @pat.speed @mutantbass I implemented the sticky left side should work in all latest normal (edge/ie will suck probably)
```

---
## \#83 Posted by: ankjaers Posted at: 2018-11-17T16:04:57.310Z Reads: 91

```
Awesome work! Wish I had this when planning my build last spring.
```

---
## \#84 Posted by: professor_shartsis Posted at: 2018-11-17T20:26:14.760Z Reads: 97

```
[quote="professor_shartsis, post:53, topic:74497"]
^suppose i’ll be climbing 1.8miles on a steady 5% grade…

i have 4x 190kv 0.05ohm motors &amp; 83mm tires, 120a motor current and 60a battery current limit per motor, &amp; 13S (48.1v)

what’s my maximum top speed up slope and what gear ratio gives this top speed assuming 0.6m^2 frontal area, 0.75 drag coefficient &amp; 200lbs?
[/quote]

[quote="professor_shartsis, post:63, topic:74497"]
72.31mph &amp; 1.08:1 gear ratio
[/quote]

what's the watt hours per mile?
```

---
## \#85 Posted by: pat.speed Posted at: 2018-11-17T21:58:52.454Z Reads: 94

```
You need to find battery current. Then you should be able to work out watt draw.  Then travelling at 72mph it would take 0.0139 hours or 50 seconds. So multiply the watts by 0.0139 to give wh/mi.

Lol you probs already know how to do that bit
```

---
## \#86 Posted by: skatardude10 Posted at: 2018-11-18T01:26:48.393Z Reads: 96

```
Can you consider adding the option for selecting a custom battery chemistry? A123 nominal voltage for example is 3.3v and that LTO battery is <3v nominal. It would be nice to be able to select custom battery chemistry and enter in your own nominal voltage so you don't have to select one of way too many other chemistries, just the most common esk8 ones or enter a custom nominal value.
```

---
## \#87 Posted by: luis99945 Posted at: 2018-11-18T02:26:39.584Z Reads: 102

```
you could put something to tell you what earrings can go up and something to select between pneumatic and urethane wheel
```

---
## \#88 Posted by: makevoid Posted at: 2018-11-20T02:19:23.205Z Reads: 102

```
Great calculator
```

---
## \#89 Posted by: Kug3lis Posted at: 2018-11-24T12:25:19.604Z Reads: 96

```
Added overview screen and some more freedom units thanks for contributing (@b264)

![image|690x450](upload://cYXKrxpJuPSXb8xAXt0PxichSr0.png) 

https://calc.3dservisas.eu/
```

---
## \#90 Posted by: Jc06505n Posted at: 2018-11-25T18:03:25.279Z Reads: 84

```
So for a 10 Wh system I should put 5 wh to get accurate measurement?
```

---
## \#91 Posted by: sharky Posted at: 2018-12-12T20:40:28.623Z Reads: 90

```
Hey hey @Kug3lis thx for the great new calc 👍👍
So the range calc is correct?
Do i need to select 1wd even when i got a dual system ir not?
Kr
```

---
## \#92 Posted by: Kug3lis Posted at: 2018-12-12T20:45:55.873Z Reads: 94

```
Range calculator depends on your average Wh/km 1wd is for single drive, 2wd is for dual motors and 4wd is for 4 wheel drive.

Average Wh/km I took from old calculator its how much one motor consumes power so the range is calculate **Battery Wh**  / (**Motor Count** * **Avg Consumption**)
```

---
## \#93 Posted by: sharky Posted at: 2018-12-12T21:09:40.295Z Reads: 88

```
Ok got it thx
```

---
## \#94 Posted by: rusins Posted at: 2018-12-23T17:37:55.845Z Reads: 83

```
Feature request: acceleration!

Or rather, since everyone's weight differs, force of acceleration, calculated from the max torque and wheel diameter. F = torque / radius. That way people can mix and match combinations to find a suitable one for their desired acceleration.
```

---
## \#95 Posted by: pat.speed Posted at: 2018-12-23T20:25:44.210Z Reads: 84

```
Wouldn’t a=f/m work too? I honestly have no idea that’s just how I’ve been shown got to calculate acceleration from force (Nm) and individual mass (kg)

Using that formula my acceleration (m/s^2) would be a =16.2/60

a = 0.27m/s^2

What’s yours?

Edit: Idk if the max torque shown is wheel rotational force or forward movement. Now I think I get why you used that equation. Would you need to do that one before doing the equation I did?
```

---
## \#96 Posted by: Sn4pz Posted at: 2018-12-23T20:44:30.639Z Reads: 81

```
[quote="Sn4pz, post:2693, topic:9559"]
Im sure its a simple explanation, but why do the torque values go down in the esk8 calculator when series count of cells is increased?

10s:

[![image|392x361](https://www.electric-skateboard.builders/uploads/db1493/original/3X/1/d/1da236543e0be5d62563fa4cb63c9faee7329665.png)
image.png928x855 38.7 KB
](https://www.electric-skateboard.builders/uploads/db1493/original/3X/1/d/1da236543e0be5d62563fa4cb63c9faee7329665.png)

12s:

[![image|392x348](https://www.electric-skateboard.builders/uploads/db1493/original/3X/e/8/e8a3874c43ccfb9918f5f63268b177f6e595d41d.png)
image.png948x842 38.1 KB
](https://www.electric-skateboard.builders/uploads/db1493/original/3X/e/8/e8a3874c43ccfb9918f5f63268b177f6e595d41d.png)

I was under the impression that the builds only got ‘punchier’( wouldnt this mean more torque) as the series number increased, as well as other benefits :thinking:
[/quote]

Any input :thinking:
```

---
## \#97 Posted by: pat.speed Posted at: 2018-12-23T20:47:23.864Z Reads: 68

```
Because higher voltage means less current needs to flow to reach the same amount of watts. Thus less current means less torque. You must adjust the watts up to the new amount based on your voltage 🙂
```

---
## \#98 Posted by: Sn4pz Posted at: 2018-12-23T21:04:10.690Z Reads: 70

```
Ah, so if I was planning for 30a on each motor for 10s, would you recommend 35a on 12s? 

I was speaking to @deucesdown and (please, anyone, if I'm wrong, don't heckle deuce) he made a comment where range seems to benefit off of increased series numbers, but wouldn't the need to readjust the values to achieve the same amount of torque effectively negate the effect of increasing the series number?

Thanks for the answer Pat
```

---
## \#99 Posted by: pat.speed Posted at: 2018-12-23T21:06:00.495Z Reads: 72

```
It’s only on this calculator that you must adjust the watts because the max current is not something we can just enter it is calculated from max wattage and pack voltage. 

In the vesc tool however you just enter 30a and it will only pull 30a

Example 

2000w /36v = 55a

2000w/44.4 = 45a
```

---
## \#100 Posted by: Sn4pz Posted at: 2018-12-23T21:06:20.899Z Reads: 72

```
Roger Roger, thank you
```

---
## \#101 Posted by: pat.speed Posted at: 2018-12-23T21:07:32.274Z Reads: 72

```
Just added an example, hope that makes it crystal clear
```

---
## \#102 Posted by: Sn4pz Posted at: 2018-12-23T21:08:23.795Z Reads: 79

```
Oooh

Cool, ok. I had it inversed in my head :P
```

---
## \#103 Posted by: deucesdown Posted at: 2018-12-23T21:23:42.467Z Reads: 77

```
[quote="Sn4pz, post:98, topic:74497"]
range seems to benefit off of increased series number
[/quote]

Looks like I got into your head. :) I was referring to this specific post:

https://www.electric-skateboard.builders/t/why-run-12s-on-a-vesc/7246/132

Please don't take it as a broadly general thing. I don't understand what's happening, but in this specific instance,
- adding 4 cells (12s4p -> 13s4p, 8% more cells) increased range 29%
- adding 17 cells (12s4p -> 13s5p, 35% more cells) doubled the range

It's hard to generalize this, and 12s is already a bit risky so it's hard to recommend 13s.
```

---
## \#104 Posted by: rusins Posted at: 2018-12-23T23:53:10.920Z Reads: 74

```
Yeah, changing wheel size doesn't change the torque value in the calculator, so I guess it's rotational torque that's being shown. So yeah, you would first need to divide the torque (Nm) by wheel radius to get the force pushing you forward (N), and then you divide by your mass to get acceleration.

My stats:
Torque: 12Nm
Radius: 42.5cm
~~Acceleration force: 28.24N~~
My weight: 80kg
~~Acceleration: 0.353 m/s^2~~
_Edit:_
Actually acceleration force is 282.4N, and acceleration is 3.53 m/s^2

~~:thinking: which means I've made a mistake somewhere, because that is super low.~~

Another thing I noticed is that the torque displayed in the calculator doesn't change when you change your battery cell discharge rate, which is bad. Means the max motor wattage is used, even if your battery cannot drive them at that rate. However, I guess that's OK, because I'm guessing just from max W and KV alone (+ motor efficiency) it calculates the motor torque per amps, and when starting from zero voltages are low, so you'll be able to drive enough amps easily.

If what I'm saying is true, then I guess you'll have good startup acceleration irregardless of what battery you have – what matters is motor wattage (well, torque, but usually correlated) and your drive train ratio. Would love for someone to either confirm this or correct me :smiley:
```

---
## \#105 Posted by: pat.speed Posted at: 2018-12-24T03:33:57.643Z Reads: 68

```
I think you got the wrong wheel radius, well unless you use 850mm wheels

Mine is about 2.75m/s/s with 97mm wheels, 16Nm torque and 60kg mass

Edit: I think the wheel radius also must be used in Metres so mine was 0.097m
```

---
## \#106 Posted by: rusins Posted at: 2018-12-24T05:04:06.220Z Reads: 67

```
Yup! That's where I messed up. Thank you! Now I get 3.53 m/s^2, which seems correct to me.
```

---
## \#107 Posted by: b264 Posted at: 2018-12-24T05:22:11.245Z Reads: 75

```
[quote="pat.speed, post:105, topic:74497"]
wheel radius also must be used in Metres
[/quote]

Everything needs to be in base units, yes
```

---
## \#108 Posted by: skatardude10 Posted at: 2019-02-03T00:56:51.816Z Reads: 78

```
Why does it say a 12S8P will have less torque then my current 10S4P?

[12S8P](https://calc.3dservisas.eu/?Tc-7DsIwDAXQf8mMkJs05bEG1AkUCYnulCFIlFTqiPrv-F7CYzu27BvnaS4hma253_LDLLQ4auGWjXoKJ3VlyahcUwEDIsJih8oWx5-ZWSlHZDjgb2-M6NYUlyBGOU-i2ZDfoD6FktSnPY4R8swT4SGUpIFnb9iLGa5JrFv_Hs2fn127CZQV3B5gT3YcB_Gaps0v) - 13.8nm after reduction 

[10S4P](https://calc.3dservisas.eu/?Rc-9DsIwDATgd8mMUEqa8rOaiglkqRLdKUOQKI3UseLd8R0RbJ8d-5Is7ibJHdzzMb3cyoqLFWHdmGfpzJUn1VhTYtpE_20fWRXr38ysjBkZAcBk8NzL2pW4rFyCGBUiiWZD_oKGJCVpSK1p58krjnnpKCVp5LP37OkE1yTW7eEcZRvD937mJ7fw6QxHsuc4iNss7f0B) - 16.6nm after reduction

When I increase motor max wattage from 3250, the torque goes up as expected. But right now on 10S4P I'm not even pushing 2880+W at 10S-80A battery max(40A/40A)... Which, with voltage sag under full load and charge down to 36 volts, that's expected- 36v*40A=1440W *2 = 2880W. 

By increasing to 12S8P and pushing 120-160A battery max (60-80/60-80), that would be 43.2v(nominal or full charge under load w/sag)*60A = 2592W *2 = 5184W. 

How is 5184W less torque than 2880W, from just going from 10S to 12S? 

Would it make more sense to be able to input your intended vesc battery and motor max/min values to calculate this better?

What it seems like though, is that the calculator is taking the motor max wattage and not multiplying it by however many motors you have, instead setting a hard wattage limit regardless of number of motors entered.

Then again, if I enter 9999999999 on the motor power rating, the torque goes up to some craaaaaazy number... Shouldn't the torque be based off your battery max, with the motor rating * # of motors being the absolute wattage limit, and calculating primarily based off your battery and efficiency, with the motor rating acting as a ceiling?
```

---
## \#109 Posted by: rusins Posted at: 2019-02-03T03:09:47.702Z Reads: 78

```
Yeah, the calculator just assumes the max current your motor can handle is watts divided by voltage of your battery. It is very misleading imo. @Kug3lis, please fix :smiley:  

P.S. Would be nice if motor kV didn't have to be a multiple of 10. TB direct drive is 75kV, so it would be useful to enter such values.
```

---
## \#110 Posted by: b264 Posted at: 2019-02-07T01:30:36.355Z Reads: 78

```
[quote="rusins, post:109, topic:74497"]
the calculator just assumes the max current your motor can handle is watts divided by voltage of your battery
[/quote]

What formula do you suggest it should use instead?
```

---
## \#111 Posted by: rusins Posted at: 2019-02-07T11:47:29.508Z Reads: 74

```
People should just have the option to input their motor's / ESC's max current that it can handle.
```

---
## \#112 Posted by: Kug3lis Posted at: 2019-02-07T14:06:38.495Z Reads: 75

```
Those torque values should matter least as they are best ever condition without anything affecting it. In reality I would be happy if you have at least half of it. So I don't see a point of changing that. Plus your ESC current limit is nothing in reality as your motor can draw up anything it wants until ESC detect over current and limits it. that's why I use power rating of the motor as manufacture measures how much it can draw.
```

---
## \#113 Posted by: rusins Posted at: 2019-02-07T14:13:21.096Z Reads: 72

```
In that case, perhaps it would be best if instead of dividing motor's power by the volts of the battery, you should always divide by 50.4V (because that's what most of our motors are rated to)? I just think something needs to be done so that people can somewhat accurately compare acceleration of different setups.
```

---
## \#114 Posted by: b264 Posted at: 2019-02-07T18:09:28.668Z Reads: 64

```

Why always divide by that, when we already know the battery voltage?  That seems even less useful than the way it is now.
```

---
## \#115 Posted by: skatardude10 Posted at: 2019-02-07T18:21:12.965Z Reads: 66

```
When riding, I see up to 2880 watts on max settings. This doesn't take into account motor amps, just battery amps and battery voltage. 

My motor amps are double my battery amps (80A motor / 40A battery). If ESC / battery amps don't matter much compared to motor amps, does that mean I'm realistically seeing (80A+80A)*36v = 5760W and not (40A+40A)*36v = 2880W according to my ESC? 

In my time riding and changing settings, it feels to me like increasing battery max has the biggest impact on increasing torque. It seems odd that if I set my motors max watts to 4000 from 2880 that it has such a huge impact on the torque calculation. I might be off base here, but I feel like the limit should be what your battery can output, and if your motor max is the limiting factor, that should be the limit. Basically, not whatever is higher (motor or battery) but whatever is lower should be the limit to max wattage being taken into account for max torque calculation. 

Again, if a motor is capable of 180A * 2 motors * battery voltage for max watts for each motor, should torque be super high if your battery can only output a max of 30A total? Just asking the question, not saying I'm right, just confused.

Also, does the calculator take into account voltage drop? It'd be neat to be able to enter expected or observed voltage drop under full load, and have that subtracted from the voltage used in various calculations.
```

---
## \#116 Posted by: rusins Posted at: 2019-02-07T19:18:31.896Z Reads: 62

```
Say I have a generic esk8 motor and a 6s20p battery. The voltage of the battery is pretty low, but that doesn't mean the ESC cannot drive the motor at an insane current when starting from stationary position. More current -> more torque -> more acceleration.

@skatardude10 Hopefully this answers your questions as well. If you have dual 80A motors, then the max you can have the ESC push them to is 160A in total. With only 40A coming from the battery, that means you can get that insane torque/acceleration only from standing still to about 1/4th of your max speed, which is the voltage at which the ESC would require more power (power = current * voltage), but that it cannot get because of the battery's limit.

Basically, two identical boards, but one with a 40A max cont. battery, and one with a 20A max cont. battery, will have the same startup acceleration, but the stronger one will be able to maintain that acceleration for precisely twice as long, until it (acceleration) starts going down due to lack of power.

Currently the calculator shows torque while driving at full speed according to your specs (when motor voltage = battery voltage). I personally don't care what my torque is like when I'm already traveling at high speed, so I think it's a bit useless at the moment.
```

---
## \#117 Posted by: b264 Posted at: 2019-02-07T19:23:49.017Z Reads: 60

```
[quote="skatardude10, post:115, topic:74497"]
Also, does the calculator take into account voltage drop?
[/quote]

It does; it's based on the nominal voltage.  This was a change from version 1.

[quote="skatardude10, post:115, topic:74497"]
It’d be neat to be able to enter expected or observed voltage drop under full load, and have that subtracted from the voltage used in various calculations.
[/quote]

You can already edit that.
```

---
## \#118 Posted by: b264 Posted at: 2019-02-07T19:26:20.632Z Reads: 60

```
What formula do you suggest it should use instead?
```

---
## \#119 Posted by: rusins Posted at: 2019-02-07T19:31:51.875Z Reads: 64

```
Since motor manufacturers usually say "up to 12s", X many watts of total power, then I'm assuming that at 12s voltage and X watts of power the current through the motors is the hottest they can handle safely for extended use. Therefore, even at lower voltages (because heat is purely dependent on current in the motor, not voltage), I think that most of our motor's max current could be estimated as 

Current = X Watts / 50.4Volts

Of course, there are some exceptions, like TorqueBoards, that list their 6355 motor as handling 80A, despite its stated power being only 2500W. (Maybe through testing they just found that 80A is fine when accelerating for a short while, but not permanently, or something) That's why ideally I'd like to plug in my ESC's / motor's max supported current, and if not, then at least calculate motor current by always dividing by 12s voltage. Current method isn't very useful imho.
```

---
## \#120 Posted by: b264 Posted at: 2019-02-07T19:43:04.130Z Reads: 60

```
Anything involving magic numbers is an almost definite "no".  At least, I'm not going to code that.

So then you are indirectly suggesting to add a "Motor Max Voltage" box and then calculate based on that?  Please elaborate

Formulas = good

Walls of text = bad
```

---
## \#121 Posted by: rusins Posted at: 2019-02-07T19:47:45.013Z Reads: 58

```
Haha, sorry. Just want to explain my thinking.

A "Motor max current" box would be ideal.
```

---
## \#122 Posted by: b264 Posted at: 2019-02-07T19:51:44.323Z Reads: 62

```
So remove the Motor Max Watts box and add a Motor Max Current box?

I think, but I'm not sure, that most motor manufacturers give max lithium Series count (12S etc) and maximum wattage.  Though I don't trust the maximum wattage numbers too much.

So “Motor max current” would be difficult for some users, I think
```

---
## \#123 Posted by: rusins Posted at: 2019-02-07T19:53:31.805Z Reads: 60

```
Very true. I just don't know of an easy way to find a compromise between "difficult for some users" and "no magic constants" :smiley:
```

---
## \#124 Posted by: Mich21050 Posted at: 2019-02-07T19:54:20.047Z Reads: 67

```
[quote="b264, post:122, topic:74497"]
So “Motor max current” would be difficult for some users, I think
[/quote]
You only need to know one formula.. P= U * I or P= V* I
...
```

---
## \#125 Posted by: b264 Posted at: 2019-02-07T19:58:52.737Z Reads: 68

```
That's kind-of true

First, expecting the next n00b to know that is pushing it a tad far.

But the other thing is what happens when you start adding duty cycles and it's not "on" 100% of the time
```

---
## \#126 Posted by: Mich21050 Posted at: 2019-02-07T20:01:51.003Z Reads: 68

```
Yep, you are right. But if you were to replace the wattage with the current box it would be the easiest formula... :slight_smile:
```

---
## \#127 Posted by: evoheyax Posted at: 2019-02-11T20:10:47.800Z Reads: 65

```
Site is down. I get an https certificate expired error. Won't let me bypass it.
```

---
## \#128 Posted by: Mich21050 Posted at: 2019-02-11T20:12:28.415Z Reads: 70

```
@Kug3lis your https/Let's Encrypt certificate expired... :slight_smile:
```

---
## \#129 Posted by: Schulerbible Posted at: 2019-02-19T12:41:18.360Z Reads: 66

```
Something with the distance calculation is seriously off. A 12s3p lipo @12Wh/km gives me only ~16 km of range and a 10s4p (same Wh/km) doesn't perform much better????
```

---
## \#130 Posted by: pat.speed Posted at: 2019-02-19T19:19:14.023Z Reads: 61

```
That sounds about right to me as your lipos are probs around 5ah so a 12s3p should get better range than a 10s4p
```

---
## \#131 Posted by: Deckoz Posted at: 2019-02-19T19:41:16.841Z Reads: 62

```
12s3p = 36 cells
10s4p = 40 cells


range is likely within a mile of one another..
```

---
## \#132 Posted by: pat.speed Posted at: 2019-02-19T20:44:08.581Z Reads: 63

```
[quote="Schulerbible, post:129, topic:74497"]
12s3p lipo
[/quote]

He’s using lipos in the 12s3p tho so it should really have better range

@Schulerbible are you talking about figures the calc gives or real world? The calculator divides your range by how many motors you have so it’s not very accurate
```

---
## \#133 Posted by: Deckoz Posted at: 2019-02-19T20:56:16.288Z Reads: 66

```
maybe... 

Li-Ion
(3p * 3Ah)(12s * 3.7v)=399.6wh
(4p * 3Ah)(10s * 3.6)=432wh

LiPoly
(3p * 5Ah)(12s * 3.7v)=532wh

LiPoly hold 60% of their charge above nominal, 10% more below nominal, and the last 30% being cell damage territory under load. so 70% usable

.7 * 532 = 372wh usable

Lion hold 60% of their charge above nominal, but can be discharged down to about 20%. or 80% usability

.8 x 432 = 345wh

differece of 37wh. Which gives you

[quote="Schulerbible, post:129, topic:74497"]
doesn’t perform much better???
[/quote]
```

---
## \#134 Posted by: 3DServisas Posted at: 2019-02-19T21:22:18.910Z Reads: 68

```
[quote="pat.speed, post:132, topic:74497"]
The calculator divides your range by how many motors you have so it’s not very accurate
[/quote]

Depends what you call accurate. You enter your ESC avg. Wh/km value you get from most apps and it multiples it by 2 if it runs dual setup and technically ur motors shouldn't consume more than 5% difference from each other then it uses it to divide battery Wh capacity for avg. range.

[quote="Schulerbible, post:129, topic:74497"]
A 12s3p lipo @12Wh/km gives me only ~16 km of range and a 10s4p (same Wh/km) doesn’t perform much better???
[/quote]

3P lipo of what kind capacity 10Ah 1Ah or 1kAh? There are options to specify the capacity of the pack which multiples it by cell count in pack and how many are in series and how many in parallel. If you don't enter correct input values don't expect correct results.

This calculator is just to give general idea, u will never have that torque neither u will have exact ranges or any other values.
```

---
## \#135 Posted by: Schulerbible Posted at: 2019-02-19T21:43:57.595Z Reads: 61

```
I am talking about the values the calculator spits out. 
I get about 15-18 km real world range on my Raptor 1 DIY (16/36 gearing, 6354 motors, 10s3p 7.5ah). Hence, with a 10s4p pack (12.4 ah), I'd assume  to get somewhere around 25 km real world range.

For my new build, I am using a 12s3p (3x3.7ah ~11 ah) lipo battery. I would expect, this should get me bit more than 20 km at 12 Wh/km? The specs for this build are:

- dual motors 170KV
- 18/36 gearing
- 100 mm wheel size
- 12s3p (11ah) lipo battery
```

---
## \#136 Posted by: Deckoz Posted at: 2019-02-19T21:57:08.169Z Reads: 63

```
10s3p 7.5Ah
((3p * 2.5Ah)(10s * 3.7v)) *.7 = 194.25wh usable

10s4p 12.4Ah
((4p * 3.1Ah)(10s * 3.7v)) *.7 = 321.16wh usable

12s3p 11Ah
((3p * 3.7Ah)(12s * 3.7v)) *.7 = 344.98wh usable

I think it would be helpful to have a page on the tool, to calculate and compare usable watt hours between batteries setups, so when someone questions range on different setups regardless the rest of the setup, they can see how just the battery stacks up..
```

---
## \#137 Posted by: b264 Posted at: 2019-02-19T22:10:01.131Z Reads: 64

```
[quote="pat.speed, post:130, topic:74497"]
so a 12s3p should get better range than a 10s4p
[/quote]

Negative, 10S4P has better range
```

---
## \#138 Posted by: pat.speed Posted at: 2019-02-20T01:21:06.180Z Reads: 65

```
I was assuming 5ah lipos and 30q cells
```

---
## \#139 Posted by: sharky Posted at: 2019-03-25T11:18:48.379Z Reads: 49

```
Just want to thank you @Kug3lis for the new cool calc
im using it several times per week but never thanked you 
Great work:+1:
```

---
## \#140 Posted by: rusins Posted at: 2019-09-05T12:44:03.368Z Reads: 21

```
@Kug3lis Just thought I'd mention that by default ublock origin (my ad blocker) is blocking content from `sentry-cdn.com`, and that stops the calculator from working. That didn't use to be the case previously, so either you made some change that introduced this bug, or sentry just wasn't counted as a malicious tracker before :man_shrugging:
```

---
