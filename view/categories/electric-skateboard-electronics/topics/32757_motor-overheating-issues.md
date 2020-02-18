# Motor overheating issues

### Replies: 25 Views: 3057

## \#1 Posted by: ndwallick Posted at: 2017-09-09T23:50:03.488Z Reads: 230

```
I have been riding my board a lot recently between classes and noticed it was cogging randomly a few times. (it would randomly feel like it's braking and make a loud sound) Then I was riding it pretty hard once and checked the motor with a heat gun and it read 300 degrees F! I even dripped water onto it and it steamed off. It has since stopped working completely. It just cogs and shakes when I push the throttle. 

motor: OM 5065 200kv
esc: Ollin vesc
batteries: 10s LiFe
[my build log](http://www.electric-skateboard.builders/t/build-log-waterproof-longboard-10s-life-with-vesc/7157/93)

Possible causes:
1) It is hot right now where I live (110 degrees when I am riding)
2) I tried @ackmaniac's vesc firmware with watt control mode a few months ago and noticed it got kinda hot, so I immediately switched back to the regular firmware (maybe once the magnets start to demagnetize it just keeps getting hotter and worse)

Anyone else have issues like this, maybe I need a 63mm motor for the AZ heat?
```

---
## \#2 Posted by: Boardnamics Posted at: 2017-09-10T00:02:56.103Z Reads: 223

```
Oh no...if it is so hot it boils water then you can pretty much guarantee the thing is shot. BLDC motors we use don't like anything hotter than 180f. Because you are in such a hot area the ambient air does a lot less good of a job keeping the motor cool. A 63 size would likely solve the issue if it is just the motor that is undersized. If you're over geared you will also have overheating issues caused  by the immense amount of amps that are required to sustain the torque needed.
```

---
## \#3 Posted by: Cobber Posted at: 2017-09-10T00:41:10.640Z Reads: 210

```
Sounds cooked dude :rage:

yeah 63mm will be cooler but so would going for a longer motor, plenty of 6374's around for fair money atm ;)

what's your gear run out?
```

---
## \#4 Posted by: ndwallick Posted at: 2017-09-11T02:07:02.016Z Reads: 192

```
@cobber My gearing is 16 to 36. My actual top speed is 20 mph, so nothing crazy. I guess I will try a longer 63mm motor. Maybe on my next board I will go 12S so it won't pull so many amps.
```

---
## \#5 Posted by: ndwallick Posted at: 2017-09-11T02:18:03.361Z Reads: 188

```
Anybody know of any good long 63mm motors that work well with the vesc and 10s LiFe?

Also I realized the new motor bolt spacing has to be 27 mm (or 38 mm measuring diagonally) to fit my current motor mount. Otherwise I will have to get/make a new mount :sweat_smile:
```

---
## \#6 Posted by: Clonkex Posted at: 2017-09-11T04:39:21.712Z Reads: 179

```
The [SK3 6374 192kv](https://hobbyking.com/en_us/turnigy-aerodrive-sk3-6374-192kv-brushless-outrunner-motor.html?___store=en_us) is a good popular motor. It's what I've got at 6S on my board and while I haven't ridden it for very long yet, and not in any kind of heat, after about 15 minutes of hard acceleration and braking and some longish continuous runs at full speed it was only barely warm. Once I've got my enclosure done so the ESC stops trying to fall off the underside I'll take it for a proper test run from full battery to none :P
```

---
## \#7 Posted by: Cobber Posted at: 2017-09-11T05:33:46.837Z Reads: 175

```
yeah I'd try a 6374, or there are some 6085's getting around too.
Certainly the 6374 is the popular choice:
[Hobbyking](https://hobbyking.com/en_us/turnigy-aerodrive-sk3-6374-192kv-brushless-outrunner-motor.html)
[Dymond](https://www.horizonhobby.de/en/p/dymond-gtx-6374.htm?a=article&ProdNr=03121773&p=43793)
Kaly also has some if you look him up on the boards I think

or a 6374 sensored
[Alien](http://alienpowersystem.com/shop/brushless-motors/alien-6374-sensored-outrunner-brushless-motor-170kv-3200w/)
[Psychotiller](https://psychotiller.com/product/sensored-6374-190kv)

or a 6384 at 955g it is single beast. I think weight equals reliability for motors...
[Alien](http://alienpowersystem.com/shop/brushless-motors/alien-6384-sensored-outrunner-brushless-motor-200kv-3500w/)

or the 6085
[Ollin](http://www.ollinboardcompany.com/product/om-6085-200kv)

you could also try searches on fleabay, alibaba or banggood...

anyway a few options to get you started
```

---
## \#8 Posted by: guyguy Posted at: 2017-09-11T13:41:42.778Z Reads: 155

```
Your motor may be under warranty if you contact ollin. 

I had a motor burnout like this due to a seized bearing.
```

---
## \#9 Posted by: ndwallick Posted at: 2017-09-22T00:04:26.682Z Reads: 141

```
@Clonkex @Cobber Thanks for all the suggestions!

@chaka Have you ever heard of an OM5065 getting to 300 F like this? The motor still spins freely so I don't think it's a seized bearing. I may have just been way overworking it lol. (with the AZ heat + the weight of me plus my backpack)
```

---
## \#10 Posted by: chaka Posted at: 2017-09-22T11:07:48.217Z Reads: 138

```
You have really tall gearing for a single 50mm motor. You need two of these of you want to use something as tall as 16:32 tooth. We can replace it but it will not like your current setup. 

If you are riding heavy with a pack you might want to think about going dual.
```

---
## \#11 Posted by: ndwallick Posted at: 2017-09-22T15:21:56.497Z Reads: 132

```
Ya that's what I figured :sweat_smile: My setup doesn't have room for another vesc or motor mount so will just try a larger motor

@chaka does your OM6085 have the same bolt spacing as the OM5065?
```

---
## \#12 Posted by: chaka Posted at: 2017-09-23T13:28:34.089Z Reads: 124

```
No, the spacing is larger. What type of motor mount are you rolling with? I also have some 15 tooth pulleys if you wanted to have another go with a 50mm motor with more gear reduction.
```

---
## \#13 Posted by: ndwallick Posted at: 2017-09-25T18:06:15.787Z Reads: 120

```
I have an aluminum mount I made for the spacing of your smaller motors. [my mount](http://www.electric-skateboard.builders/t/build-log-waterproof-longboard-10s-life-with-vesc/7157/24)


I don't wanna to lose any speed so I think I'm ready for a bigger motor. I guess I will have get a different mount and sell this one. It worked well for me for a solid year

What exactly is the spacing of your larger motor?
```

---
## \#14 Posted by: ndwallick Posted at: 2017-09-28T22:05:35.864Z Reads: 115

```
I’m currently deciding between the alien 6374 and the Ollin 6085. 

@chaka, instead of replacing my OM5065, could you discount me that price on the OM6085? That would be awesome if you could! 

Then I just have to find another mount and I will be riding again :slight_smile:
```

---
## \#15 Posted by: chaka Posted at: 2017-09-29T01:47:33.445Z Reads: 107

```
Sure, as long as you don't mind sending the the 50mm motor back. Let me know when you are ready and I will generate a coupon for you!
```

---
## \#16 Posted by: ndwallick Posted at: 2017-09-29T18:05:21.677Z Reads: 93

```
Yup I can send it back, just pm me the address to send it too. And I'm ready to buy!

Also what mounts will fit this? is the bolt spacing the same as most 63mm motors?
```

---
## \#17 Posted by: chaka Posted at: 2017-09-30T14:54:28.659Z Reads: 88

```
Ollin Board Company
PO Box 3391
Truth or Consequences, NM
87901


Yes they are the common spacing for 63mm motors.
```

---
## \#18 Posted by: dickyho Posted at: 2017-09-30T14:57:56.492Z Reads: 85

```
[quote="ndwallick, post:1, topic:32757"]
tween classes and noticed it was cogging randomly a few times. (it would randomly feel like it's braking and make a loud sound) Then I was riding it pretty hard once and checked the motor with a heat gun and it read 300 degrees F! I even dripped water onto it and it steamed off. It has since stopped working completely. It just cogs and shakes when I push the throttle. 

motor: OM 5065 200kv
esc: Ollin vesc
batteries: 10s LiFe
my build log

Possible causes:
1) It is hot right now where I live (110 degrees when I am riding)
2) I tried @ackmaniac's vesc firmware with watt control mode a few months ago and noticed it got kinda hot, so I immediately switched back to the regular firmware (maybe once the magnets start to demagnetize it just keeps getting hotter and worse)

Anyone else have issues like this, maybe I need a 63mm motor for the A
[/quote]

Even reached 300C, the motor still will not damage.    check all wires and connectors to see if the tin got melted
```

---
## \#19 Posted by: ndwallick Posted at: 2017-10-02T16:47:56.293Z Reads: 74

```
I just bought Chaka's larger motor and the Torque boards mount for it!
```

---
## \#20 Posted by: Bataleon Posted at: 2017-10-03T10:40:43.956Z Reads: 73

```
Awesome. Please keep us posted on how performance compares to the 5065.

@chaka, I'm currently running an OM-5065 so it would be really interesting to get a "postmortem" of what went wrong with @ndwallick's motor :)
```

---
## \#21 Posted by: chaka Posted at: 2017-10-03T14:00:24.282Z Reads: 66

```
Gear ratio was too tall for a single 5065, need a dual setup or a bigger motor if you want to run tall gear ratios.
```

---
## \#22 Posted by: ndwallick Posted at: 2017-10-03T21:36:23.948Z Reads: 60

```
@chaka Also interested to see what the inside of that motor looks like haha
```

---
## \#23 Posted by: Bataleon Posted at: 2017-10-04T13:36:04.032Z Reads: 60

```
Did some of the enamel coating on the copper wire melt due to the heat?
```

---
## \#24 Posted by: chaka Posted at: 2017-10-04T13:53:30.826Z Reads: 59

```
As soon as it arrives I will pull it apart and check it out!
```

---
## \#25 Posted by: ndwallick Posted at: 2017-10-06T15:23:21.010Z Reads: 50

```
Just installed the new parts! http://www.electric-skateboard.builders/t/build-log-waterproof-longboard-10s-life-with-vesc/7157/97
```

---
