# Gathering Electronics from scratch

### Replies: 118 Views: 7404

## \#1 Posted by: noushi Posted at: 2015-12-16T23:50:05.350Z Reads: 126

```
Hi
I would love some help on the motor,esc and battery
I am thinking of buying this motor http://www.hobbyking.com/hobbyking/store/__18126__Turnigy_Aerodrive_SK3_5065_236kv_Brushless_Outrunner_Motor.html 

However I am very confused about the ratings. Will this motor always output 1850W (Rated Max Wattage) and draw current equal to 1850/Supply Voltage and then I use this current value to calculate my ESC. Or does the motor wattage output equal 60A(max amps) x Supply Voltage and therefore as it only draws 60A max I only need maybe a 70A ESC

Also I've heard people use 125A ESCs but the motor's max current is only 60A so what is the point of this?

I really appreciate any help!
Thanks very much
```

---
## \#2 Posted by: NNGG Posted at: 2015-12-17T00:06:58.104Z Reads: 122

```
The motor wont always give 2.5 horse power, it has a burst rating. The 125amp esc is so it can survive a burst.
```

---
## \#3 Posted by: noushi Posted at: 2015-12-17T00:21:02.549Z Reads: 126

```
Ok
But on general cruising which of the 2 options is correct as ultimately I would like to know what esc to get and what the normal output power will be.
```

---
## \#4 Posted by: Sharkface Posted at: 2015-12-17T00:49:53.895Z Reads: 127

```
The output of your motor will varry a lot depending on a multitude of variables: rider weight, gearing, wheel size... i think there might be more but that could be it. 

Overall that 1850w is the max yes... but we have science somewhere on this forum that shows you are actually never drawing more than like 400w. A lot of people use a motor very similar to the one that you have linked, then they put a 6s battery and the VESC (Vedders ESC) to keep the motor spinning and get a respectable 20mph on average.  Again, this can vary based on weight, wheel size.... blah blah blah.

[quote="noushi, post:1, topic:743"]
Also I've heard people use 125A ESCs but the motor's max current is only 60A so what is the point of this?
[/quote]

put simply: safety. If you get a car ESC from hobby king and get it all set up, you are putting weight onto a motor that was meant for an RC car/airplane.... itll do it, but she will get super pissed. Mise' well have a lot of wiggle room so that you always have that safety ceiling. If you get lipo batteries and have a short.... you risk having a nice fire that looks a lot like thermite welding. The only ESC that was made specifically for our boards, both long and short, is the VESC.

If you search around on this forum and check out others builds you will find that a lot of people follow the same pattern, get a VESC, get a LiFe battery (like the space cell) throw on a 36 tooth wheel pulley to some 83mm abec flywheels, throw a 14T pulley to that motor you linked, mount it with one of the many motor mounts out there, strap it all under the board, and ride happily for days. Usually they have two motors no less lol

If you can spend the ~$100 on an ESC get either the VESC or torqueboards 12S ESC. you will have to do some learnings regarless though. have fun!!!!!!
```

---
## \#5 Posted by: cmatson Posted at: 2015-12-17T01:08:52.937Z Reads: 110

```
I second on either buying a VESC or torqueboard's esc. 

Torqueboard's for simplicity 

VESC for tinkering

Both are the best options, just for two types of buyers! Good luck on your built!
```

---
## \#6 Posted by: noushi Posted at: 2015-12-17T17:16:29.783Z Reads: 105

```
Hi

If I don't want to purchase a VESC (high cost) what size amp car/airplane esc would i need.
Is a high esc used just to cope with the burst current upon startup and then when cruising the motor pulls less than 60A and will provide power equal (actually less as it is not 100% efficient) to that current x supply voltage?

thanks
```

---
## \#7 Posted by: Sharkface Posted at: 2015-12-17T19:32:35.706Z Reads: 103

```
The VESC sits comfortable at a 60 amp draw, but since its made for electric boards you dont need to have that rated comfortable amp draw nearly as high. 

Since you are trying to use an RC ESC you will 100% want to ensure that its:

 1. a car ESC as its got breaks typically
 2. can take the beating you will throw at it for making it do something it wasnt 100% meant to do. (a 100+ amp draw, and programmable are the two things that come to mind)

Its like taking a basketball player and telling him to play soccer. Sure he can run up and down the field, probably can even dribble the ball some. But he will really shine when you get him back on the basketball court. An ESC is an ESC yes, but by using a car ESC you will be running a much higher risk of getting the ESC to:

 1. fry itself
 2. give you lots of engine cogging and therefor not a smooth ride
 3. require tinkering to get it to not overheat the motor
 4. pull more power and run less effeciently

the car ESC will work, but the money you save means that you will be researching hard to ensure that you dont end up having to buy 2 or 3 car ESCs (you should just expect to fry one). So, a car esc will work, but you are going to want to put a loootttt of time into searching around online.
```

---
## \#8 Posted by: noushi Posted at: 2015-12-18T08:42:18.853Z Reads: 92

```
That makes it clearer
However i still dont understand why i would need a 100Amp rc car esc. Wont that supply the motor with 100A but then fry the motor as its max current limit is 60A?
```

---
## \#9 Posted by: lowGuido Posted at: 2015-12-18T09:01:03.651Z Reads: 97

```
look at it this way.
the numbers printed on cheap ESC's are probably all fat anyway.
a "200A" ESC is probably pretty unlikely to actually reliably handle 200A for any sustained period of time. (if at all)
so by buying a "120A" ESC you are more likely to see an actual 60A current though.

also you wont fry your 60A motor with a 200A ESC. these numbers are purely "ratings" not actual currents. so its not as if you turn on a "200A" ESC and there is 200A coming out the back of it.. in fact there's nothing coming out at all.

the motor actually DRAWS current from the ESC. so its the relationship between the motor and the battery that makes the current flow through the ESC.
```

---
## \#10 Posted by: noushi Posted at: 2015-12-18T10:07:56.000Z Reads: 94

```
Right thanks a lot for that explnation
One thing though, if the motor is put under load I assume it will draw more current. However will the motor keep drawing current until roughly 60A and then just stop turning. Or will it carry on and burn out
```

---
## \#11 Posted by: lowGuido Posted at: 2015-12-18T10:30:47.441Z Reads: 91

```
the motor is a "dumb" component it doesn't have any limiters or anything smart.. its just a pile of copper and magnets. so it will try to keep going until it burns out.
```

---
## \#12 Posted by: noushi Posted at: 2015-12-18T10:55:04.018Z Reads: 92

```
So do i just have to gear the motor to make sure it doesnt draw more than 60A
```

---
## \#13 Posted by: lowGuido Posted at: 2015-12-18T11:20:03.623Z Reads: 92

```
60A is a lot of amps. all the motors I have used are 60A max and never blown one.
I think you'll be fine.
```

---
## \#14 Posted by: noushi Posted at: 2015-12-18T14:53:35.438Z Reads: 94

```
Ok so i just need to buy a 120A rc car/airplane esc only because the amp rating is not entirely correct and probably more like 60A

And the motor realistically wont draw more than 60A and therfore the max power i can expect with a 4s lipo (14.8V) is 60x14.8 W

Is this all correct?
```

---
## \#15 Posted by: lowGuido Posted at: 2015-12-18T15:37:25.700Z Reads: 98

```
don't get a plane ESC get a car ESC.
```

---
## \#16 Posted by: psychotiller Posted at: 2015-12-18T15:51:31.217Z Reads: 98

```
Car esc. Not plane, not boat, not helicopter. CAR.
Another thing to note is you are absolutely going to get out of your board what you choose to spend on it.
```

---
## \#17 Posted by: Sharkface Posted at: 2015-12-18T15:54:11.867Z Reads: 105

```
With that car RC you wont be able to tell how kuch amperage you are rolling with. Howver 4s is way slow. Do 6s at mins. Im rolling 12s on hills. 

The car esc is cheap and thisly dont expect the world of it. It was MEANT for an rc car that weighs maybe 10 pounds. Your board alone will easily get up to 15 pounds. Thusly you make the ESC as beefy as you can so it can handle as much current as you drop through it. Then you just let the motor draw what current it needs. Due to the weight the current will need to do a high amp load for a long period of time (like riding up a hill) so rather than risk frying a component you beef it up. I can guarantee you that if you get a 60a esc for you 60a motor, you will fry your esc and risk shorting out lipo batteries. 

My torqueboards esc can do like 180amp continuous and then do 1000amp burst. Ill never get 180 amps to glow through that motor... yet ive already burned through one esc... 

If you short a lipo it can explode. I would hate for you to end up frying yourself alive because you wanted to buy the cheapest CAR esc you could find. Get a car esc
```

---
## \#18 Posted by: psychotiller Posted at: 2015-12-18T16:10:13.148Z Reads: 101

```
Every castle esc I've used is still in action except for one). No programming issues. No fault codes,  No drv blah blah to replace. And the xe runs and ez runs are pretty much Bomb proof from hobbywing. The only reason everyone here believes differently is marketing for higher voltage setups. And, also note that the torqueboard's esc is a car esc.
```

---
## \#19 Posted by: psychotiller Posted at: 2015-12-18T16:13:38.948Z Reads: 100

```
The fact is though, to get  a reliable CAR esc you will spend more money on it than on a vesc anyway. And if you cheap out on a smaller boat or plane esc you may hurt yourself.
```

---
## \#20 Posted by: noushi Posted at: 2015-12-26T10:54:33.136Z Reads: 101

```
ok
does anyone have any car ESCs they can recommend or think will probably work?
Thanks everyone
```

---
## \#21 Posted by: noushi Posted at: 2015-12-26T11:32:16.489Z Reads: 99

```
Also on a side note what is the average current going through a motor whilst cruising so I can calculate my  rough battery life duration so I know what capacity lip to buy
```

---
## \#22 Posted by: noushi Posted at: 2015-12-26T11:46:44.662Z Reads: 94

```
an esc like this - http://www.hobbyking.com/hobbyking/store/uh_viewitem.asp?idproduct=77155 
will it work?
```

---
## \#23 Posted by: claudiofiore88 Posted at: 2015-12-26T17:22:02.222Z Reads: 94

```
People here usually recommend the hobbyking 150a or hobbywing xerun 150a. You could also use @torqueboards esc or the vesc which can handle up to a 12s Lipo.
```

---
## \#24 Posted by: NIK Posted at: 2015-12-26T17:26:21.570Z Reads: 92

```
Yep, @claudiofiore88 right, it also gives you more 'room' for upgrading your board for the long run. But its all up to you. Have fun and good luck
```

---
## \#25 Posted by: lowGuido Posted at: 2015-12-26T22:05:53.980Z Reads: 91

```
I have used plenty of the old HK 150A ESC's and they were great, but unfortunately limited to 6S and no longer sold. 
I have bought a new X-car series that replaces them (in @noushi 's link above) but havent finished my hack board for testing yet. again its still limited to 6S.
```

---
## \#26 Posted by: mccloed Posted at: 2015-12-27T01:46:45.206Z Reads: 92

```
I'm running the 150a xbeast on a dual motor board. They're pretty much the same as the old HK 150a. Just as much brake noise, but they work good. Definitely buy the led program card if you get one of these.
```

---
## \#27 Posted by: lowGuido Posted at: 2015-12-27T02:05:37.311Z Reads: 94

```
interestingly enough the trackstar ESCs have a LOUDER breaking noise than the HK ones.
I know right. 
the HK ESC's are actually pretty quiet comparatively.
```

---
## \#28 Posted by: noushi Posted at: 2015-12-27T09:59:19.284Z Reads: 94

```
So either of the xbeast or hobbywing xerun/ezrun 150A car escs are recommended?

And also mccleod where do you find the hobbyking xbeast 150A esc? I can only find the 120A version from my original link
And can a car esc actually brake a skateboard to a stop/very low speed? Or does it just slow you down slightly
```

---
## \#29 Posted by: mccloed Posted at: 2015-12-27T15:57:23.714Z Reads: 92

```
Here is a link to the HK 150a: http://www.hobbyking.com/hobbyking/store/__77145__HobbyKing_174_8482_X_Car_Beast_Series_ESC_1_8_Scale_150A.html

The brakes are pretty good on these.I usually set them from 80 - 100%.
```

---
## \#30 Posted by: lowGuido Posted at: 2015-12-27T20:41:37.728Z Reads: 89

```
I generally set my brakes to 50%. I find any more to be too much. Stop so quickly you land on your face.
```

---
## \#31 Posted by: noushi Posted at: 2015-12-27T21:56:42.700Z Reads: 92

```
Thanks for the replies
Do you think the 120A HK car esc will be enough (as it is half the price of the 150A HK esc)?
```

---
## \#32 Posted by: noushi Posted at: 2015-12-31T12:32:04.548Z Reads: 91

```
Thanks for the replies @lowGuido and @mccloed and everyone else  
Do you think the 120A HK car esc will be enough (as it is half the price of the 150A HK esc) to drive a single motor skateboard?
```

---
## \#33 Posted by: lowGuido Posted at: 2015-12-31T13:16:50.893Z Reads: 97

```
I have only ever used the 150A so i can't comment on the 120A version.
```

---
## \#34 Posted by: mccloed Posted at: 2016-01-01T05:00:50.483Z Reads: 96

```
I too have only used the 150a version. I do use the FVT 120a and it works just fine, so I'm assuming the X beast 120a should be fine also.
```

---
## \#35 Posted by: psychotiller Posted at: 2016-01-01T05:17:24.252Z Reads: 91

```
The 120a mamba monster worked really well.
```

---
## \#36 Posted by: cmatson Posted at: 2016-01-01T14:46:57.446Z Reads: 95

```
I second that @psychotiller

I absolutely love castle esc's even if they are slightly more money.
```

---
## \#37 Posted by: mccloed Posted at: 2016-01-01T17:34:42.871Z Reads: 96

```
They are definitely good quality. I am using the XL2 on my 8s board. Unfortunately, they do not have a sensored option.
```

---
## \#38 Posted by: noushi Posted at: 2016-01-02T09:35:24.294Z Reads: 90

```
Hi
Do you think a 120A boat esc will work as I have read (https://endless-sphere.com/forums/viewtopic.php?f=35&t=52759) that they are quite good and better than car escs in terms of braking noise but im not sure if it will actually work properly?
```

---
## \#39 Posted by: psychotiller Posted at: 2016-01-02T13:21:03.730Z Reads: 90

```
If you read further you will find they don't work well enough to deal with the hassle.  I know it's been said many times, but I'll stay it again.
Car esc!
```

---
## \#40 Posted by: noushi Posted at: 2016-01-02T13:47:31.991Z Reads: 84

```
ok thanks a lot. I think I will use the 120A HK Car ESC
```

---
## \#41 Posted by: noushi Posted at: 2016-01-03T14:45:27.448Z Reads: 85

```
If I use a 6s 5000Ah lipo does anyone know **roughly** how long it will last on a 1 motor electric skateboard. I know it depends on the speed but just for an average trip with some stopping, slowing down and fast speeds. 
Thanks
```

---
## \#42 Posted by: psychotiller Posted at: 2016-01-03T15:37:59.953Z Reads: 83

```
Maybe 5 miles @noushi
```

---
## \#43 Posted by: lowGuido Posted at: 2016-01-03T23:38:59.370Z Reads: 84

```
I get about 13km, on my single motor 6S 5000mah board.
(that's about 8 miles for the Americans)
```

---
## \#44 Posted by: noushi Posted at: 2016-01-04T07:56:45.479Z Reads: 84

```
What size wheels does everyone use? Is 70mm wheels enough as then there is also the trucks amd riser pads which add even more clearance?
```

---
## \#45 Posted by: lox897 Posted at: 2016-01-05T06:50:17.902Z Reads: 84

```
Seeing as @onloop is busy shipping stuff I'll repost this in all the threads that don't follow the guidelines quoted by onloop here:

In order to make the "E-board Builds" category really easy to search & locate specific builds i am asking that you change your title to something descriptive that better expresses the makeup of your build.
Most of the new build threads tend to end up with a name such as 
"new- noob - noobie - beginner - first - build - help - newb" this becomes hard to keep track of.
I would like to see each build thread with a descriptive title, such as;
Project Name | Deck Name | Trucks | Motor type | Mounting method | Voltage/Battery | ESC
Example
The Samurai | Custom Deck | Paris Trucks | R-SPEC | Custom Mount | 10S | VESC
```

---
## \#46 Posted by: treenutter Posted at: 2016-01-05T15:59:23.813Z Reads: 85

```
@noushi same here as @lowGuido. I get about 9 miles with 5000mah using 8S. Terrain and speed impact this by about 30%.
```

---
## \#47 Posted by: noushi Posted at: 2016-01-05T16:11:40.394Z Reads: 86

```
But what size wheels do you all use @psychotiller @treenutter @lowGuido @mccloed ?
Are 70mm wheels fine when considering the riser pads are like 12mm?
```

---
## \#48 Posted by: treenutter Posted at: 2016-01-05T16:13:42.202Z Reads: 81

```
@noushi I'm using 127mm pneumatics but you don't need wheels that are that large; that was a choice based on my environment. I'll let others weigh in on the size of their urethane wheels, 83mm flywheels, or their clones, seem to be standard.
```

---
## \#49 Posted by: noushi Posted at: 2016-01-05T16:14:33.657Z Reads: 81

```
@treenutter would 70mm be too small. 83mm just seems big!
```

---
## \#50 Posted by: treenutter Posted at: 2016-01-05T16:19:13.226Z Reads: 83

```
@noushi as the wheel gets smaller, you lose the opportunity to create a useful reduction ratio with your gearing. That's the ratio between your motor pulley and your wheel pulley. A greater ratio allows you to create torque, which you need to start moving and to power up inclines. in DIY anything is possilble! So it is possible to use 70mm wheels, but I think it's smaller than what most use in this community. Take a look at the measurements of the available wheel pulleys from @onloop and @torqueboards, this should help you to figure out if it will work.
```

---
## \#51 Posted by: noushi Posted at: 2016-01-05T16:54:07.387Z Reads: 83

```
Yes @treenutter but doesn't a smaller wheel diameter increases the torque so i dont need such a high gearing, which will also mean the speed will increase so overall wont my torque and speed be the same as an 83mm wheel board
```

---
## \#52 Posted by: psychotiller Posted at: 2016-01-05T16:58:12.011Z Reads: 80

```
I would say minimum you should use would be 75mm. Smaller than that and you are going to run into several speed bumps in your build. I hate risers and won't use them.  Being up high on a longboard feels retarded and is avoidable with the right parts. I have builds with 75, 80, 85 , 105 and 150mm wheels right now.
```

---
## \#53 Posted by: chaka Posted at: 2016-01-05T16:58:38.556Z Reads: 83

```
It is all about clearance. On 83mm wheels even a 30 tooth pulley will be extremely close to the asphalt.
```

---
## \#54 Posted by: treenutter Posted at: 2016-01-05T19:43:00.887Z Reads: 82

```
@noushi you're right in theory, but as you shrink down the pulleys and wheel, you need to also shrink down the teeth on them. There is a limit to how small the teeth on the pulleys and belt can be and still transfer the required torque without slipping. That's why 5HTD is the standard that most settle on. Like @psychotiller said, 75mm is about the smallest you can get without some unique engineering (which I heartily endorse!)
```

---
## \#55 Posted by: lowGuido Posted at: 2016-01-05T20:45:10.174Z Reads: 83

```
I have 70mm wheels on all my builds.
I only have 2mm risers on my daily.
```

---
## \#56 Posted by: noushi Posted at: 2016-01-05T21:14:54.889Z Reads: 81

```
@lowGuido what size pulleys and belts do you use
```

---
## \#57 Posted by: lowGuido Posted at: 2016-01-05T21:17:45.304Z Reads: 81

```
30t and 12t pulleys.  The 30t is pretty close to the ground.  Id say i have hit it on small rocks plenty of times.
```

---
## \#58 Posted by: noushi Posted at: 2016-01-05T21:29:44.010Z Reads: 84

```
@lowGuido what speeds and torque do you get? Can you go up some moderate hills?
```

---
## \#59 Posted by: lowGuido Posted at: 2016-01-05T21:52:58.391Z Reads: 85

```
top speed on flat 35km /h and handles hills so long as you have a bit of momentum.
```

---
## \#60 Posted by: noushi Posted at: 2016-01-26T19:26:51.298Z Reads: 80

```
So could someone (@lowGuido @treenutter @psychotiller @mccloed or anyone else) please tell me if the this setup will work:
Turnigy aerodrive 236kv motor
120A HK X Car beast ESC
6s 5000 mah lipo
76mm wheels
12T to 30T pulley system

Thank you VERY MUCH for your help
```

---
## \#61 Posted by: lowGuido Posted at: 2016-01-26T19:28:18.831Z Reads: 77

```
Yes. that will work.


----------
```

---
## \#62 Posted by: psychotiller Posted at: 2016-01-26T19:35:08.214Z Reads: 76

```
Yes. You'll be looking at a 16-18mph top speed.
```

---
## \#63 Posted by: noushi Posted at: 2016-01-26T19:37:10.279Z Reads: 74

```
and do you (@lowGuido @psychotiller)  think it is safe to buy a 5000Ah 30C 3s lipo. So the lipo can safely discharge 150A? or do i need a higher amp discharge?
```

---
## \#64 Posted by: lowGuido Posted at: 2016-01-26T19:44:08.916Z Reads: 73

```
30C is fine.
I have used 20C, 30C, 35C, there is no noticeable difference.

I have found on average i discharge at 1C.
```

---
## \#65 Posted by: noushi Posted at: 2016-01-26T19:45:43.526Z Reads: 75

```
oh cool. but the C rating of a battery determines how much current can be drawn. Is 20C fine because the motor never draws above 100A?
And a 120A esc is enough correct?
```

---
## \#66 Posted by: lowGuido Posted at: 2016-01-26T19:47:02.379Z Reads: 77

```
[quote="lowGuido, post:64, topic:743"]
I have found on average i discharge at 1C.
[/quote]

so thats about 5A average discharge on my 6S setup.
I use a 150A ESC but many other people are using a 120A ESC with no dramas.
```

---
## \#67 Posted by: noushi Posted at: 2016-01-26T19:47:51.271Z Reads: 75

```
so your motor only ever draws 5A??? isn't that low
```

---
## \#68 Posted by: lowGuido Posted at: 2016-01-26T19:49:51.682Z Reads: 76

```
Average.
obviously it draws higher and lower. but average is 5A
```

---
## \#69 Posted by: noushi Posted at: 2016-01-26T19:53:01.534Z Reads: 76

```
woah ok. thanks a lot lowGuido. I really appreciate your help along with everybody else's
```

---
## \#70 Posted by: lowGuido Posted at: 2016-01-26T19:59:06.870Z Reads: 75

```
I think the problem is that everyone gets caught up in numbers. particularly PEAK values.
if you were to ask anyone here how long they skate for on one battery they would probably say 30 mins to an hour. (this obviously will differ with different peoples battery sizes etc.) if anyone was to discharge their battery at ~30C their skate would last a few MINUTES. (obviously again depending on batteries)
I don't think anyone draws that much current consistently.
```

---
## \#71 Posted by: noushi Posted at: 2016-01-26T21:40:57.472Z Reads: 74

```
but when the current does peak don't you need to ensure the battery can supply a large enough current or else it will catch on fire? Or is the peak duration so short it doesn't make much of a difference?
```

---
## \#72 Posted by: NNGG Posted at: 2016-01-26T22:46:38.743Z Reads: 72

```
Are you going for a single or dual setup?
```

---
## \#73 Posted by: noushi Posted at: 2016-01-26T22:47:51.874Z Reads: 71

```
single motor (236kv) setup
```

---
## \#74 Posted by: NNGG Posted at: 2016-01-26T22:48:36.593Z Reads: 69

```
I would go for a bigger motor just because its only $20 extra dollars but depends on how many Volts you are going to put through it.
```

---
## \#75 Posted by: noushi Posted at: 2016-01-26T22:52:43.380Z Reads: 69

```
im was going to use 6s lipo (22.2V) with the 236kV motor with 76mm wheels and a 12T:30T pulley ratio. Apparently it should go at 18mph
```

---
## \#76 Posted by: NNGG Posted at: 2016-01-26T22:57:01.086Z Reads: 66

```
I dont have a need to go faster than 20mph and so I choose more torque
```

---
## \#77 Posted by: noushi Posted at: 2016-01-26T22:57:54.112Z Reads: 68

```
yh me too so isn't a 236kV motor enough? How steep hills do you think it can go up?
```

---
## \#78 Posted by: NNGG Posted at: 2016-01-26T22:58:33.104Z Reads: 73

```
I have heard that my 149 kv on 12S can go up 20% as a single
```

---
## \#79 Posted by: NNGG Posted at: 2016-01-26T22:59:05.818Z Reads: 71

```
I have Lots of 10% hills and a few 15+
```

---
## \#80 Posted by: Sharkface Posted at: 2016-01-26T23:01:15.267Z Reads: 75

```
[quote="NNGG, post:78, topic:743, full:true"]
I have heard that my 149 kv on 12S can go up 20% as a single
[/quote]

I really wish I had a way that I could measure the degree incline of the hill i take every day on the way home. these 149kv motors have just so much darn torque. 20% incline on a 15mm belt is nothing for these motors. fooorrr sssuuurreeee
```

---
## \#81 Posted by: NNGG Posted at: 2016-01-26T23:06:18.144Z Reads: 75

```
findhills.com m8 Its a good site
```

---
## \#82 Posted by: NNGG Posted at: 2016-01-26T23:07:58.443Z Reads: 72

```
I might go dual 149kv @8S each with two 9mm belts
```

---
## \#83 Posted by: noushi Posted at: 2016-01-26T23:17:10.731Z Reads: 69

```
what about 236kv how steep can that go?
```

---
## \#84 Posted by: noushi Posted at: 2016-01-26T23:18:15.935Z Reads: 72

```
@lowGuido what motor are you using and how many lipo cells to get these results.
```

---
## \#85 Posted by: NNGG Posted at: 2016-01-26T23:22:09.043Z Reads: 73

```
A 236kv motor is only 5065 size can and has a higher rpm than a 149kv. I would say It can easily do 5-10% maybe 15%
```

---
## \#86 Posted by: noushi Posted at: 2016-01-26T23:29:23.166Z Reads: 74

```
thanks and 120A esc is fine yh?
```

---
## \#87 Posted by: NNGG Posted at: 2016-01-27T00:33:05.935Z Reads: 75

```
I would spend some money and get a vesc. If you are already gonna send $300+ I would do it right so I do not have to spend anymore on escs. Just my opinion. I would do a fvt120A ESC only if doing a budget dual drive with four 3S batteries and some 215KVs, or in your case two 236KVs
```

---
## \#88 Posted by: lowGuido Posted at: 2016-01-27T02:11:14.504Z Reads: 76

```
I have 6s with a aerodrive 280kv.
<img src="/uploads/db1493/original/2X/c/cb8274d55c693799af81f251898aa55d2946b48f.jpg" width="583" height="500">
```

---
## \#89 Posted by: lowGuido Posted at: 2016-01-27T02:44:07.954Z Reads: 78

```
this setup above is almost identical to the setup you are considering.
https://youtu.be/TTiKzhJQBk8?t=1m
here is a video of that same setup easily cruising 20~30km/h
```

---
## \#90 Posted by: cmatson Posted at: 2016-01-27T03:44:22.699Z Reads: 75

```
using a Garmin VIRB by any chance? I know it can record all that sensor data and the gauge overlay looks oddly familiar..
```

---
## \#91 Posted by: lowGuido Posted at: 2016-01-27T03:46:44.721Z Reads: 76

```
its the virb overlay, but was a gopro camera. I don't have a virb but I really like the software for the speed overlay etc. (and its free!)
```

---
## \#92 Posted by: NNGG Posted at: 2016-01-27T04:12:50.132Z Reads: 76

```
What wheel pulley do you have? It makes the motor shaft look tiny.
```

---
## \#93 Posted by: noushi Posted at: 2016-01-28T19:56:15.034Z Reads: 76

```
@lowGuido please could you tell me if you know roughly what degree/% incline hills it can go up.
And you said your pulley hits the ground sometimes? Can you just keep going or do you have to slow down, and is the pulley still fine or does it get damaged?
Also what size belt do you use 9mm or 15mm? Do you experience any belt slippage with 12:30 when going up some hills?

Thanks a lot :smiley:
```

---
## \#94 Posted by: lowGuido Posted at: 2016-01-28T22:55:39.828Z Reads: 75

```
[quote="noushi, post:93, topic:743"]
said your pulley hits the ground sometimes? Can you just keep going or do you have to slow down, and is the pulley still fine or does it get damaged?Also what size belt do you use 9mm or 15mm? Do yo
[/quote]

I use a 9mm belt, and I have made my bracket the same hight as my pulley so it will hit the ground before the pulley does. (although over time it has worn down anyway) I came to the conclusion that the pully is moving the same speed as the wheel and will roll over things easier than the bracket thats stationary anyway.
after over 700km of travel the damage is just a few scrapes, nothing more that you would expect on a skateboard truck.
<img src="/uploads/db1493/original/2X/c/c8bad6a0200fc166d020c720a418d0f74bf2933e.jpg" width="281" height="500">
it can go up slight hills but anything too steep will slip the belt.
I dont know if you can see the gradient of the hill in this video? it doesnt really show.
https://youtu.be/Xe_WowHbwmE?t=1m31s
```

---
## \#95 Posted by: laurnts Posted at: 2016-01-28T23:17:57.476Z Reads: 73

```
@noushi Just small input, if you really think to do uphill alot then you really need to refine your choice of motor again. I would recommend getting somewhere around 200 KV value, it would help alot already in climbing uphill by 15 - 30 degree incline taking average of 15A - 20A draw. Like @lowGuido mentioned, even if your motor could draw so much up to 65A or 120A you will probably slip the belt / pulleys also combined with cheap 120A chinese RC ESC that are not meant for pulling 60kg uphill 20km/h for 10km you will definitely going to destroy them quicker. And personally what you will experience when climbing an even stepper hill is your motor probably still keep drawing more amps and turn but your wheel is loosing traction to the ground. Hence the pulley combination you choose wouldn't matter so much.

It's always recommended from my personal experience to get single big motor for "normal commute" and dual drive for climbing and speedy mode. The traction is really one of the biggest point in uphill despite of motor, esc and pulleys. If you want to be on the safe side, start buying the right motor and configuration as you would like to have only to purchase 1 motor and many pulleys instead of many motors with single pulley combination setup.
```

---
## \#96 Posted by: lowGuido Posted at: 2016-01-28T23:34:08.124Z Reads: 72

```
I have to admit that my dual motor board eats hills for breakfast. if you have lots of hills around i would go for a dual setup.
i ride my single as a commuter, where there aren't many hills
```

---
## \#97 Posted by: noushi Posted at: 2016-02-21T18:57:23.509Z Reads: 67

```
@mccloed and @lowGuido  how do you program your 120/150A hobby king car beast ESCs?
I can't seem to find any manual. Do you have to buy a programming card or can you do it via a remote (I know it is harder)?

Thanks
```

---
## \#98 Posted by: lowGuido Posted at: 2016-02-22T00:44:43.088Z Reads: 66

```
I use the programing card.
```

---
## \#99 Posted by: noushi Posted at: 2016-02-22T18:25:22.129Z Reads: 64

```
@lowGuido Do you know if you can use a remote to program it instead?
```

---
## \#100 Posted by: lowGuido Posted at: 2016-02-22T18:28:05.848Z Reads: 66

```
apparently you can use software. but I haven't done that before.
this is what I used:
<img src='/uploads/db1493/original/2X/1/1c8d6de71de8be488a8ed05b099d306bfbf6d0c8.jpg'>
```

---
## \#101 Posted by: noushi Posted at: 2016-02-22T18:33:36.129Z Reads: 63

```
@lowGuido  ok thanks. And do you know if the 120A esc has a manual? I can't seem to find one.
And do you know what cable I need if i where to program it using software?

Sorry for all the questions. I really appreciate your time and help!
```

---
## \#102 Posted by: lowGuido Posted at: 2016-02-22T18:38:36.598Z Reads: 62

```
mine came with a manual, a pretty basic one, its pretty much the same as all the other ESC manuals I have seen
```

---
## \#103 Posted by: noushi Posted at: 2016-02-22T18:56:42.487Z Reads: 61

```
and do you know if I can use a cable to program it?
 I looked at the this hobbyking cable (http://www.hobbyking.co.uk/hobbyking/store/uh_viewitem.asp?idproduct=31858) but i'm not sure if it will work with the 120A BEAST esc? What do you think?
```

---
## \#104 Posted by: lowGuido Posted at: 2016-02-22T19:38:44.867Z Reads: 62

```
I believe that is the correct cable, but I have never used it so I cant comment.
the cost of the cable is close to the same as the cost of the program card so.. six of one, half a dozen of the other.
```

---
## \#105 Posted by: noushi Posted at: 2016-02-22T20:51:32.054Z Reads: 64

```
yh i'm asking because the led programming card you used is not in stock at the moment and don't know how long it usually takes for hobby king to restock.
```

---
## \#106 Posted by: noushi Posted at: 2016-02-23T19:36:32.742Z Reads: 61

```
@lowGuido the programming card you used is on backorder from hobby king
Do you know what else I can do to program it??? Can you check for me if you can use the remote control or if there is a button on the esc
Many thanks

P.S.I think the cable I posted was for the 120A 1:10 esc 2-3s lipo and not the 120A beast 1:8 2-6s lipo esc we both have.
```

---
## \#107 Posted by: noushi Posted at: 2016-03-02T18:38:06.943Z Reads: 56

```
Hi @lowGuido @psychotiller @cmatson @NNGG @treenutter     
Do you all have to kickoff and get the board moving before starting the motor, or does the motor accelerate from rest. I am using a 236v motor with a ratio of 12T : 30T

Thanks
```

---
## \#108 Posted by: lowGuido Posted at: 2016-03-02T18:42:04.450Z Reads: 54

```
I kick off first.
As I have said in other posts I find it super awkward to step onto the board without kicking off anyway
it only takes a very small kick to get it rolling.
```

---
## \#109 Posted by: treenutter Posted at: 2016-03-02T19:22:06.150Z Reads: 54

```
@noushi I can kick if I want to, but I don't have to. Generally I prefer to stand on the board and take off using the motor, it feels more satisfying to me. Unless I'm facing uphill from a dead-stop, in which case I'll give a small push to get going.
```

---
## \#110 Posted by: NNGG Posted at: 2016-03-02T22:05:53.772Z Reads: 53

```
I always push my board at low speeds because its good exercise, but I use the throttle for anything 5+ mph
```

---
## \#111 Posted by: cmatson Posted at: 2016-03-02T22:41:49.871Z Reads: 53

```
[quote="lowGuido, post:108, topic:743"]
As I have said in other posts I find it super awkward to step onto the board without kicking off anywayit only takes a very small kick to get it rolling.
[/quote]

agreed; it is just more natural to have a small amount of momentum. 

Like riding a bike- you don't just hope on when it's sitting still; give yourself a push, and then off you go!
```

---
## \#112 Posted by: psychotiller Posted at: 2016-03-02T22:48:56.897Z Reads: 52

```
Kicking off is natural. Not an inconvenience. Can't imagine I would ever not kick off.
```

---
## \#113 Posted by: noushi Posted at: 2016-03-02T22:52:17.984Z Reads: 51

```
@psychotiller @cmatson @lowGuido @treenutter @NNGG     And do you find if you kick (which will spin the motor) doesn't that generate some backward current. Does it damage the components or is the current produced just negligible it makes no difference
```

---
## \#114 Posted by: psychotiller Posted at: 2016-03-02T22:56:12.784Z Reads: 52

```
Maybe an unmeasurable amount. Doesn't matter any more than you braking down a hill and then hitting forward throttle.
```

---
## \#115 Posted by: NNGG Posted at: 2016-03-02T23:59:30.923Z Reads: 51

```
I would believe there would be more stress on the motor/esc with takeoff from a stand still.
```

---
## \#116 Posted by: mccloed Posted at: 2016-03-03T01:44:58.446Z Reads: 54

```
I love the sensored feeling of not having to kick off but I still do. One of my friends kids kicked off on a board with the castle xl2 on 8s before the loopkey was inserted and the board powered up from the motor spinning. It, of course immediately shut down after the motor stopped. Very unexpected.
```

---
## \#117 Posted by: treenutter Posted at: 2016-03-03T20:40:55.580Z Reads: 52

```
@noushi, @psychotiller is right, the amount of current it generates isn't harmful.
```

---
## \#118 Posted by: mccloed Posted at: 2016-03-04T01:59:27.305Z Reads: 52

```
@treenutter, Agreed.
```

---
