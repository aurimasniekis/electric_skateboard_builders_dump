# Has anyone here tried using a gearbox/transmission on a belt and pulley eskateboard?

### Replies: 27 Views: 2528

## \#1 Posted by: ELREVENGE Posted at: 2017-04-01T06:00:41.968Z Reads: 289

```
I'm looking at building my first eboard. I've looked around and thought about going with a belt and pulley because of cost compared to a hub motor especially when it comes to repairs. While thinking about design I realized I'm basically building an RC car that I stand on. I have a friend who was into RC and robotics. He suggested a gearbox hooked up to a belt and pulley system because I wanted to not have to worry about 30% inclines but still be able to hit 30 mph or so as well as be able to use regenerative breaking on the way down hills. After looking at car transmissions I realized that it basically just changes the torque and rpm of the motor as needed. I looked around this site and only found a few posts about a [mountain board using a gearbox that you can change the gears of](http://www.electric-skateboard.builders/t/esk8-de-trampa-emtb-direct-drive-gearbox-2x-6374-200kv-sensored-10s-4p-vescs/10274) and a few posts about a [CVT (continuously variable transmission)](http://www.electric-skateboard.builders/search?q=cvt) from what I saw though those only work depending on the rpm so the regenerative breaking might not work or if it does it might be weird. I also found a post about a [2 stage gear box for getting higher torque.](http://www.electric-skateboard.builders/t/most-torque-for-the-money/17947)
I thought I could ether try for something with 2-3 different gear modes with different top speeds and hill climbing ability by changing gear ratio in the gearbox/transmission via remote control so you don't have to change the gears by hand. If I went with that I don't know if it would be safe to change gears while riding though. My other idea is making something more like a car transmission with 4+ gears with ability to change gears while riding. If I went with the car transmission idea I would probably try a [dual clutch transmission](https://www.youtube.com/watch?v=lFAtc-zOKZs)
Has anyone tried making/buying a gearbox and using it on a eskateboard? If so please explain how you made it and how it worked for you.
```

---
## \#2 Posted by: Smorto Posted at: 2017-04-01T11:11:21.458Z Reads: 268

```
Wow! This is an ambitious project for sure but i will love to see it if you get it working. I know @captainjez is using direct gears on their boards though I don't think they change gears on the fly/when they are out riding. Other than that I cannot help you, sorry :slight_smile:.
```

---
## \#3 Posted by: Tom1 Posted at: 2017-04-01T11:49:04.396Z Reads: 259

```
I haven't done it yet but I'm building a dual drive board with 3 different sized sprockets on the drive wheels, I want to keep a short chain and using solenoids to change the position of the sprockets will allow me to change speeds remotely and safely without breaking the chain, while riding. im using a dual vesc so I don't think it'll support regen breaking but the battery I'm making is gonna be a massive 10s 8p lithium ion so I wont need the regen breaking.
```

---
## \#4 Posted by: Okami Posted at: 2017-04-01T12:21:35.484Z Reads: 250

```

@Tom1  Will you have some sort of ''tensioner'' for the chain?

I saw a video of a ''kid'' building 2 speed transmission for his e-scooter, but he took the thing from bicycles.. Im not sure how easly it would be to mount it onto an eboard :slight_smile:

Non the less.. i really wish that you do make something and that you can encourage others later on to follow in your footsteps :)

--

Sorry for ''double post'', but this is the video for these, who have not seen it:
https://youtu.be/Vr6SIEmcQsE?t=342
```

---
## \#5 Posted by: Tom1 Posted at: 2017-04-01T12:39:27.777Z Reads: 233

```
I will need some sort of tensioner you're right, without it the chain wont leave the sprocket ha! I didn't think about that at first thankyou. what that guy has done with his scooter would be easier to make and easier to fix if something goes wrong, I don't have handlebars though so I gotta do it remotely and my chains wont be long enough to allow the chains themselves to change position. so my skateboard will change gears by first giving the chains slack and then activating/deactivating the solenoids.
my sprockets will have teeth on the inside which will match the teeth of the shaft they'll be on, the chain will spin the sprocket and the sprocket will spin the shaft which will spin the wheel, the bigger sprocket will spin the shaft slower but with more torque, the smaller one will spin faster with less and the smallest will spin fastest with the least amount of torque. I love how that guy used plumbing pipes XD thanks guys, I never considered how the chain was going to leave the sprockets
```

---
## \#6 Posted by: Okami Posted at: 2017-04-01T12:41:32.351Z Reads: 213

```
yeh, I ''updated'' the video, so that it starts from the part where he shows just the sprocket system and how he managed to use bicycle parts to make it work.. 

Basically he has the ''shifter'' from bicycle, to move the chain and then that 2 sprocket tensioner thing to keep it tensioned.
```

---
## \#7 Posted by: Tom1 Posted at: 2017-04-01T12:47:23.756Z Reads: 208

```
nice, that tensioner is exactly what I gotta make, I might make it shorter and ill make 2, I didn't notice that he had a tool box, I might put a custom one between the bindings. that's a really nice scooter though good on him
```

---
## \#8 Posted by: ELREVENGE Posted at: 2017-04-01T15:37:00.761Z Reads: 192

```
It sounds like a good idea, are you afraid of dechaing at all though? I wish you the best with your build it sounds nice.
```

---
## \#9 Posted by: Tom1 Posted at: 2017-04-02T01:04:26.165Z Reads: 177

```
Yup, pretty scared of it, I'll probably try out different gear changing methods, I think if the chain just stays straight it should be fine but I'll have to make a good tensioner thanks mate
```

---
## \#10 Posted by: saul Posted at: 2017-04-02T02:12:53.580Z Reads: 188

```
[quote="ELREVENGE, post:1, topic:20091"]
I wanted to not have to worry about 30% inclines but still be able to hit 30 mph
[/quote]

you can do this with a single speed, so theres no need to add the weight and complexity of multiple muti speed gearboxes.

There are also very few hills above 30% incline unless your off road.

either way the torque curve and rpm range of bldc motors means you can have torque and speed with a single speed setup thats easier and more reliable. so this would be creating more problems than it solves...
```

---
## \#11 Posted by: chuttney1 Posted at: 2017-04-02T02:15:09.900Z Reads: 178

```
There is a college team doing this for their Senior project. I do not have a link but have seen their stuff on the endless sphere forum. The use a differential.
```

---
## \#12 Posted by: RebellionBoards Posted at: 2017-04-02T22:13:30.960Z Reads: 170

```
<img src="/uploads/db1493/original/3X/5/7/5793d9bd36f5510f8af0c0836c87fc83ca80c3a1.PNG" width="281" height="500">
<img src="/uploads/db1493/original/3X/e/a/eae0f4f981a0675b7d8dc112d49e74c56900152e.PNG" width="281" height="500">
```

---
## \#13 Posted by: RebellionBoards Posted at: 2017-04-02T22:19:30.517Z Reads: 161

```
The belt stays the same size
The two pulleys change to the optimal ratio. 
Then for brakes add a kers flywheel. Then release the energy in the flywheel at startup. This would take most of the sage of the batteries.
```

---
## \#14 Posted by: ELREVENGE Posted at: 2017-04-03T02:43:14.515Z Reads: 152

```
You make some good points. However I would argue that a pretty simple [2 speed gear box](https://www.youtube.com/watch?v=OnLReFDz9B8) wouldn't cause too many problems (I would probably change some things about this set up but it shows how simple it could be) and would offer a higher top speed than a fixed gear ratio and maybe make it easier on the motor on hills for the heavier riders as well as let you keep the same battery voltage.
using [this calculator](http://calc.esk8.it/) 
changing nothing but the gear ratios will give you a higher top speed and maybe make it easier on the motor right?
[using a 15 to 36 or 2.4:1 gear ratio you only get a top speed of 14.58 mph](http://calc.esk8.it/#{%22batt-type-lipo%22:1,%22batt-cells%22:6,%22motor-kv%22:230,%22system-efficiency%22:70,%22motor-pulley-teeth%22:15,%22wheel-pulley-teeth%22:36,%22wheel-size%22:83}|)
[using a 15 to 15 or 1:1 gear ratio you get a top speed of 34.75 mph](http://calc.esk8.it/#{%22batt-type-lipo%22:1,%22batt-cells%22:6,%22motor-kv%22:230,%22system-efficiency%22:70,%22motor-pulley-teeth%22:15,%22wheel-pulley-teeth%22:15,%22wheel-size%22:83}|) 
both of these the motor will be spinning at the same RPM though. 
I'd like you to show me a build that can pull 250 pounds up a 30% incline at 30mph with a fixed gear ratio though.
```

---
## \#15 Posted by: ELREVENGE Posted at: 2017-04-03T03:32:23.941Z Reads: 138

```
CVTs are cool but 'Id rather be able to charge the battery from going down hills. Isn't KERS more of a boost system then a way of constantly putting energy back into the system?
```

---
## \#16 Posted by: saul Posted at: 2017-04-03T04:17:46.435Z Reads: 143

```
[quote="ELREVENGE, post:14, topic:20091"]
using a 15 to 36 or 2.4:1 gear ratio you only get a top speed of 14.58 mphusing a 15 to 15 or 1:1 gear ratio you get a top speed of 34.75 mph
[/quote]
This will get you that speed, I only know 1 hill > 30% and its not something Id want to ride....
[Build #3 Dual drive](http://esk8.today/guides/build-guide/)

A dual 10s/12s will go over 35mph **or** up crazy hills if you gear down with small wheels.

[quote="ELREVENGE, post:14, topic:20091"]
heavier riders as well as let you keep the same battery voltage.
[/quote]

this must be 6s. Higher voltage batteries and esc fix this without noisy heavy gears. that gearbox is cool, but just not needed.

I have 14/36 on 8s 245kv tops out at 25.5 mph.

I'm just trying to save you some time and money, I went through all this research already for an ebike, in the end for something you can actually use everyday its best to keep the mechanical side as simple as possible, cheap and reliable. 

Electric drivetrain and multiple speed gearboxes don't tend to work well, because the instant torque tends to break gears, a lot!
```

---
## \#17 Posted by: RebellionBoards Posted at: 2017-04-03T05:02:58.579Z Reads: 125

```
KERS could be used to put energy back into the system(like in F1). Or transfer the energy into a spinning weight(flywheel) to slow down. Then use the mass and speed of the flywheel to accelerate from a stand still or push start. Just a thought
```

---
## \#18 Posted by: saul Posted at: 2017-04-03T07:37:02.444Z Reads: 124

```
KERS = Kinetic energy recovery system

we already have that too. regenerative braking is a type of KERS since your motion is turned back into electrical energy.

Flywheel Mechanical KERS are really cool because they usually run at >90k rpm! but that means crazy expensive to develop and produce.
```

---
## \#19 Posted by: RebellionBoards Posted at: 2017-04-03T19:49:58.131Z Reads: 114

```
I know that I have burned out 4 motors in a year and a half of riding th hills of San Francisco. Heat is not a friend to the magnets and the rest of the parts inside. 


"Flywheel Mechanical KERS are really cool because they usually run at >90k rpm! but that means crazy expensive to develop and produce."

I am talking about a whole new drive train to help out the weakest link in the system. The battery. If you can take the stress off it using a cvt and kers, and have much more range and possibly a smaller battery pack saving weight, all makes for a better board. 
I think it would be worth the investment. 
Since esk8t boards are just the smallest rideable electric vehicle, that have similare systems to Teslas, formula e racing, LMP1 race cars. Let them do you r&d them make the same parts smaller and lighter.
```

---
## \#20 Posted by: Okami Posted at: 2017-04-03T20:40:55.084Z Reads: 110

```
@RebellionBoards So how exactly did you burn your motors? Did they become ''weak'' or were not working anymore? Or u just ''burnt'' the windings with too much amps maybe?

Im really curious.. as I was discussing about this with a friend that usually windings get burnt up.. and we werent sure how the magnets loosing strenght manifest in real life
```

---
## \#21 Posted by: RebellionBoards Posted at: 2017-04-03T21:02:05.862Z Reads: 103

```
I have a boosted 1 and a evolve gt bamboo. 
In the boosted there was a grinding noise out of both motors(they replace both for free and had the board back to me in less than a week).
The GT motors separated at the seems then made noise then locked up on me frying the motor controller. They sent me two new motors and a controller for free and I replaced the parts.
 I never found out what failed in all of those cases but I think it was braking down hill a lot and I mean sf a lot.
```

---
## \#22 Posted by: ELREVENGE Posted at: 2017-04-05T08:04:37.827Z Reads: 97

```
While I agree with you I do think multiple speed gearboxes if done correctly with strong materials would give worth while benefits. If an electric car uses a transmission I don't see why an eboard couldn't if using strong materials.
```

---
## \#23 Posted by: Okami Posted at: 2017-04-05T13:30:03.214Z Reads: 86

```
I think the most benefit would come for people with lots of hills and especially very steep ones.. on the second hand, probably the minority of eboard users have such hills everyday
```

---
## \#24 Posted by: mmaner Posted at: 2017-04-05T13:35:01.207Z Reads: 81

```
I am not saying one way or the other if I think this will work, but...

[quote="ELREVENGE, post:22, topic:20091"]
If an electric car uses a transmission I don't see why an eboard couldn't if using strong materials.
[/quote]

The basic tenet that all engineers have to learn over and over and over again is that correlation does not imply causation.
```

---
## \#25 Posted by: chuttney1 Posted at: 2017-04-05T14:59:29.163Z Reads: 78

```
[quote="mmaner, post:24, topic:20091"]
The basic tenet that all engineers have to learn over and over and over again is that correlation does not imply causation
[/quote]

This also fall under the science category.
```

---
## \#26 Posted by: ELREVENGE Posted at: 2017-04-05T22:46:45.310Z Reads: 74

```
You are right that correlation doesn't imply causation however, my point is that you shouldn't rule out it being possible just because it hasn't been done before. I'm saying they are so similar in how they function that I don't see why people aren't trying something similar because it already works on a larger scale.
```

---
## \#27 Posted by: mmaner Posted at: 2017-04-05T23:05:13.683Z Reads: 75

```
I totally dig what your saying.  I encourage you to try everything...hell, put bananas in it and see what happens :slight_smile:.  All I am saying is that because it works on something, that doesn't mean it will work here, even if the platforms are similar.  

Also, you gotta look at the law of diminishing returns.  Im not talking about cost, Im talking about energy (which is a kind of cost, just not $$$).  How much power/current is it going to take to operate it.  

Just tossing ideas is all.
```

---
