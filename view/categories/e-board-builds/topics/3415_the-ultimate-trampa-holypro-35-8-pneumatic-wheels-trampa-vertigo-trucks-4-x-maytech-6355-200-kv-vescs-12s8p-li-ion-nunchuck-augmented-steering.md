# The Ultimate &#124; Trampa Holypro 35 &#124; 8&rdquo; pneumatic wheels &#124; Trampa Vertigo Trucks &#124; 4 x Maytech 6355 200 Kv &#124; VESCs &#124; 12s8p Li-Ion &#124; Nunchuck Augmented Steering

### Replies: 22 Views: 4457

## \#1 Posted by: makepeace Posted at: 2016-05-17T20:29:34.020Z Reads: 524

```
So I've been wanting to build an eMTB for a while, and this is going to take a while. It's still a concept in my head at this stage, and it's going to take a while to settle on some designs for motor mounts, motor protection and an electronics enclosure. As well as to save up the cash for this MONSTEROUS build.

Anyway. The main feature of this build will be the augmented steering. What I plan to do is to incorporate the x-axis of the Nunchuck to augment the steering. Basically, when you angle the toggle left and right, you will get an appropriate amount of acceleration of the motors on the outside of the turn and a corresponding deceleration of the motors on the inside of the turn. This will compensate for the increased turning resistance that a 4wd implementation forces, as well as make for a far more stable and manueverable MTB, as the turning capability is already compromised in comparison to a street board based on the geometry. There will be a similar effect with braking. The 'bias' so to speak will be adjustable on the fly, so you will be able to reach down to the board to adjust the sensitivity based on the trail you're on.

Gearing will be selected for a top speed of about 60km/h, but will be easily adjustable by switching out pulleys down to a 30km/h max for increased run time. Pulleys will be 15mm width HTD 5.

The idea behind this board will be to provide a long fast ride that will enable the user to ride mountain bike trails. Highest performance possible over the longest range possible. I want to start the sport of eMTB racing in South Africa with this board. People down here love outdoor sport and race culture, and I believe this to be the next big thing. 

This will be a fully open source project, and I will be publishing all mechanical, electrical/electronic and software components for this build as I want to create a sport culture designed around the DIY experience. Because skate is punk like that.

And ideas/suggestions and collaborations welcome. All the financial help possible will be greatly appreciated and needed.

This is going to be extreme.
```

---
## \#2 Posted by: claudiofiore88 Posted at: 2016-05-17T21:08:54.414Z Reads: 481

```
You're crazy, but I love it!
```

---
## \#3 Posted by: JLabs Posted at: 2016-05-17T22:59:20.339Z Reads: 484

```
This sounds great! I REALLY like your idea about the steering! I want to know how well it will work for you!! Start the build!!!
```

---
## \#4 Posted by: makepeace Posted at: 2016-05-18T00:33:11.143Z Reads: 484

```
This is the Trampa setup I'll be going for with this build:

<img src="/uploads/db1493/original/2X/5/593bfb4b5b24c6fd11fbcdba7d9a2c1cbdf4b930.jpg" width="690" height="308">

I still need to settle on the deck and damper specs, but at the moment I'm leaning towards the 16 ply deck (because I'm a light guy at 75kgs, but those batteries are going to add some dynamic mass), and stiff dampers due to the fact that the steering would be augmented and it would be good to have some straight line stability.

I'll also be going for the heel straps to improve steering on the toe-side.
```

---
## \#5 Posted by: barajabali Posted at: 2016-05-18T00:37:40.258Z Reads: 450

```
I don't know much about mtb how do you attach the motor mount ? Or which mounts are you gonna use on them?
```

---
## \#6 Posted by: willpark16 Posted at: 2016-05-18T01:45:08.641Z Reads: 429

```
I would advise against the 12s 6p just because those cells probably wont have a very long life for such a large investment
```

---
## \#7 Posted by: makepeace Posted at: 2016-05-18T06:09:22.836Z Reads: 421

```
*8p (probably). I want about 20-40km range out of this thing, depending on how you ride. And that's not the point. They will last about a year with hard wear, but the expense to replace will be less than the the fuel to your MX/Enduro bike over that period. So it's all good.
```

---
## \#8 Posted by: makepeace Posted at: 2016-05-18T06:10:31.453Z Reads: 431

```
Patience. We'll get there. 😉. It will be very similar to how we normally mount the motors.
```

---
## \#9 Posted by: whitepony Posted at: 2016-05-18T06:16:31.044Z Reads: 446

```
i built the very same trampa with a diy 10s6p liion battery: https://endless-sphere.com/forums/viewtopic.php?f=35&t=78970

<img src="/uploads/db1493/original/2X/7/751e0ac83558a39db957111d6924929a4829300e.jpeg" width="690" height="498">

its quite heavy already, not sure if 20 more cells and 2 more motors will actually add more fun - my educated guess is: theyll take some fun away.

not that I wouldnt wanna see quad motor steering ... :smiley:
```

---
## \#10 Posted by: makepeace Posted at: 2016-05-18T08:19:04.106Z Reads: 423

```
Awesome build @whitepony. The single tracks in South Africa are pretty knarly and hilly, and a 30km ride time out in the open with no need for pitstops will be awesome. Could also be cool to find a 10k loop or so and have an 'Enduro' type of race with pitstops to swap out a smaller battery pack. Maybe 12s2p. Will do some experimentation with setups to see where the break-even point for fun is.

@whitepony, what's the range on that 10s6p with that setup? Oh and at what average speed or so. You done these tests yet?
```

---
## \#11 Posted by: DilatedPupils Posted at: 2016-05-18T15:58:50.678Z Reads: 385

```
This would be interesting. Controlling the speed with a little joystick on a bumpy curvy hill seems challenging enough. Add the turning to that little thing, might not be for everybody. And the mechanics of the skateboard, you lean to where you wanna turn. :neutral_face:
```

---
## \#12 Posted by: barajabali Posted at: 2016-05-18T16:05:38.651Z Reads: 375

```
Haha true. I'm thinking about doing a mountain board build but I just don't know if I'll have to make a custom mount or if I can buy one.  

I don't mind making a mount I've done it before it's just a lot of work
```

---
## \#13 Posted by: makepeace Posted at: 2016-05-18T16:38:08.376Z Reads: 378

```
@DilatedPupils, Yeah, I've given that some thought. Basically, the idea here is to augment the steering. It is not to be used as a replacement for using your body to ride the board.

It will probably be progressive, so the more you steer, the less the change in the differential effect. It will also probably compensate for jolts by ignoring changes in toggle position occurring over less than a certain time period.

It will also probably be progressive relative to your speed. So the faster you go the less the change in differential effect

The main idea here is to get over the hurdles that a 4wd board faces, most importantly the increased turning resistance. 

It will probably also have VESC controlled general differential, because that's generally a good idea on 4wds.
```

---
## \#14 Posted by: makepeace Posted at: 2016-05-18T17:05:28.977Z Reads: 344

```
I know that a couple of companies are involved in developing mounts for Trampa boards. As far as I know there is nothing yet on the market.
```

---
## \#15 Posted by: bbq870 Posted at: 2016-05-18T17:09:53.358Z Reads: 333

```
Jenso aka nowind has a motormount 
check the Endless Sphere forum in "skateboards"
```

---
## \#16 Posted by: Tarzan Posted at: 2016-05-18T17:53:06.791Z Reads: 345

```
The website of nowind is
http://www.e-toxx.com
His mounts are well made and tested.
Just write him and he will let you know what his is calling for it.
```

---
## \#17 Posted by: barajabali Posted at: 2016-05-18T18:08:47.569Z Reads: 385

```
Any reason you're going for the advanced/pro model? 

I'm thinking about getting this one 

http://www.trampaboards.com/35-long-trampa-deck-on-vertigo-trucks-with-hypa-wheels-ratchet-bindings--689-mountainboard-p-12349.html

Edit: never mind realized the difference in price is minimal.

Here is what I'm looking into 
<img src="/uploads/db1493/original/2X/8/8c1d177b35a8af1626e872c81f7fe7c5854e5735.png" width="281" height="500">
```

---
## \#18 Posted by: makepeace Posted at: 2016-05-18T19:16:31.674Z Reads: 375

```
The reason I'm going for the 685 is because I don't want to pay for the slight mass difference of the titanium trucks over the Vertigos and the Vertigo trucks are substantially lighter than the Infinity series trucks. Best cost/performance decision in my view.

The reason I'm going for the Holy Pro deck is the small price difference for a much lighter and performance driven deck. The additional weight of the electro-mechanical components requires everything else to be as light as possible within a reasonable cost to maximise fun.

Oh yeah and the star wheels because of ease of mounting a pulley to them.
```

---
## \#19 Posted by: Kaly Posted at: 2016-05-19T11:28:35.463Z Reads: 362

```
I've eMTB for little over a year now and light weight is a most.  http://www.electric-skateboard.builders/t/esk8tube-video-thread/47/17?u=kaly

a AWD system sounds good but in practice the added weight will harm your maneuverability. In my experience maneuverability it's top priority a lot of the obstacles on a off-road trail can be overcome with a little hop of the board. 

Besides the power consumption of the 2 extra motors and controllers will force you into a large battery pack that will not be use efficiently. 
IMO I think for your goal you'll be better serve by motors 150 kv at the back for maximum torque and maneuverability. 
And a detachable battery pack for quick refueling on the trail. 

About the argumented steering this boards don't need it, with the right suspension set up and once you get to trust the bindings this boards can steer really well you'll be surprise. 

Best regards  :-)
```

---
## \#20 Posted by: makepeace Posted at: 2016-05-19T18:36:27.657Z Reads: 348

```
@Kaly, thanks for your comments. With no disrespect, what most eMTBs are capable of that I've seen so far (at least with video evidence) comes nothing close to what I want to do with my proposed board.

I want to do stuff like the downhill mountain bikers do, but uphill. And provide a platform for others to do so too. And I don't want to be limited by what the board can do. The sportsman's skill needs to be the limiting factor. Because one day people will be doing things with these boards that we can only dream of.

As far as I'm concerned AWD is a must, and I'm confident that with concept of augmented steering manoeuvrability will not be an issue and will most likely be better than the current skateboard offers with a bit of dialing in and getting used to.

I do value your suggestion if a lower Kv. I will have to do some calculations when I get into the kitty gritty to see what's viable.

Thanks for your opinions!
```

---
## \#21 Posted by: cesargrimmelprez Posted at: 2016-10-08T16:31:44.242Z Reads: 239

```
Is this still continuing or am i missing something?
```

---
## \#22 Posted by: barajabali Posted at: 2016-10-08T19:57:33.061Z Reads: 237

```
12s7p is as much as I can fit in my battery box how are you gonna fit 12s8p? Box is gonna be huge
```

---
