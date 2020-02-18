# Kickboard goes Electric (Micro Monster)

### Replies: 35 Views: 3560

## \#1 Posted by: Weberp7593 Posted at: 2016-12-05T00:10:16.698Z Reads: 409

```
Hey,
i am almost ready now and want to ask the ones who are advanced.

Do you think this will work...?

Board: (already bought)
<img src="/uploads/db1493/original/3X/d/7/d7e9a0a0eeccebc895ff4d79fe6d7164cba35c3e.JPG" width="356" height="500">

Vesc + SK3 9s Lipo

And:
<img src="/uploads/db1493/original/3X/d/a/da9d155314db730c229030601df05aae6cb6ea30.PNG" width="281" height="499"><img src="/uploads/db1493/original/3X/e/f/efbca0032157b28c098a34b4dd30fb725ec23200.PNG" width="281" height="499">

I calculated like this:
<img src="/uploads/db1493/original/3X/3/2/322a16fcb390a8d5f731b85229c1e624f5f9da31.PNG" width="281" height="499">
```

---
## \#2 Posted by: saul Posted at: 2016-12-05T03:09:47.371Z Reads: 326

```
that thing looks scary. plastic wheels?

also no idea where to mount anything or fit the pulley. but if you can figure it out i'd would just say gear ratio is a bit high. 16/40ish would give plenty of torque without loading the motor too much.

16/60 is usually for mtb wheels 6-9".
```

---
## \#3 Posted by: Michaelinvegas Posted at: 2016-12-05T04:30:36.447Z Reads: 313

```
Scary is a good thing lol
```

---
## \#4 Posted by: Weberp7593 Posted at: 2016-12-05T07:26:19.900Z Reads: 291

```
I think it's funny to ride it's an scooter for adults and it's very solid, the wheels are rubber.

What gearing ratio would you recommend?
```

---
## \#5 Posted by: saul Posted at: 2016-12-05T07:49:04.199Z Reads: 278

```
[quote="Weberp7593, post:4, topic:14188"]
What gearing ratio would you recommend?
[/quote]

My board has 14/36 on 97mm.
have also used 16/40 97mm wheels with the 149kv till it broke....twice... :weary:
```

---
## \#6 Posted by: Weberp7593 Posted at: 2016-12-05T07:59:56.401Z Reads: 253

```
@saul what board do you drive ;)?
And what did broke?
```

---
## \#7 Posted by: Okami Posted at: 2016-12-05T08:03:09.402Z Reads: 247

```
Do you have a real life pic of this ''beast''?

It does look it might be troublesome to mount the motor.. I think this is the problem with scooters that you have to make some sort of extensions to the chassis and then the motor usually stands out quite a bit.

As for the ratio.. I would recoomend to go with something close to 1:3. I think, the highest you might want to go would be 1:3.5

Also - for such wheels Im not sure you can easly get 60T pulley in such a small size.. not sure what size are these you showed in pics.. but for 6'' wheels, it is also easier to go with 45T or so (for htd5 belt), so that the cog is not larger than the hub)
```

---
## \#8 Posted by: Weberp7593 Posted at: 2016-12-05T08:15:04.508Z Reads: 215

```
Thanks for your advice! @Okami 
The Wheels are 120mm like I typed in, in the calculation.
But then I will go to 1:3...

And in the afternoon I will post some pics.
```

---
## \#9 Posted by: Okami Posted at: 2016-12-05T08:18:53.542Z Reads: 203

```
Cool.

Yeah, I've got 9''inch wheel monster.. and by running it with just 6s and 192kv I can start from a standstill! My ratio is 4.33, so I think you dont have to go with 3.7, if your wheels are almost twice smaller.

22.96cm / 12.00cm = 0.52. So, if we directly translate that to ratio - 1: 2.25 gearing
I think you would get quite good speed with 1:3, so that's where you should stay more or less, as some ppl with larger wheels also tend to use that ratio, I think. 

Though, perhaps someone has a better statistics and can recommend even better ratio..

---
```

---
## \#10 Posted by: Okami Posted at: 2016-12-05T08:26:45.165Z Reads: 200

```
Btw - **what's the optimal speed you would like to get?**

Im not entirely sure you need 149kv.. unless you plan to upgrade it or to move onto something else.. I think 192kv is totally fine, unless, you use 12s and get too much speed.. (but if it is related to vesc, then ok, not my deal, as I have not worked with it so far).

So, Im not entirely sure that you plan to dig ground with this thing you are planning to build..

I ran the numbers with this calc:
http://calc.esk8.it/#{"batt-type-lipo":1,"batt-cells":10,"motor-kv":192,"system-efficiency":85,"motor-pulley-teeth":10,"wheel-pulley-teeth":35,"wheel-size":120}|

Though, effiency set to 85%, and it showed, that with 192kv you could go even with 1:3.5 or 1:4 ratio and get quite good speed. Im not entirely sure it is safe to drive it up to 25mph.. but still :D

So, the conclusion, is that 1:3 should be optimal for 145kv motor.. especially, if the speed of ~20mph is totally okay for you.
```

---
## \#11 Posted by: Weberp7593 Posted at: 2016-12-05T08:41:28.807Z Reads: 192

```
I think for me also 25kph would be fine.
25mph would be very good and maybe a bit crazy :smiley:

But I think I would go on the ratio you recommend.
It sounds good.

I will try with that board and maybe go to an longboard if it will not work.
```

---
## \#12 Posted by: Okami Posted at: 2016-12-05T09:04:37.332Z Reads: 196

```
Depends on your mechanical abilities.

 It looks like that the space from wheel to the wheel brackets (which hold the wheel) is really tight. 

So there are a few scenarios I can imagine:

A) more narrow pulley if it fits in the existing space between the wheel and and bracket (chain pulley could be an option, as in some cases it is more narrow, I think)
B) A little bit worse scenario - you might need to change the wheel (to more narrow one), if none of the sprockets is easly attachable to the wheel
C) make the brackets wider (needs longer wheel axle and welding or screwing metal parts, probably the hardest step, if it needs to be taken)

When you can post pics of how the back wheel looks, what spokes it has (hub), also measure distance between wheel and the bracket in which the wheel is held. This way it should be a lot easier to help with the mechanical part, I believe
```

---
## \#13 Posted by: Weberp7593 Posted at: 2016-12-05T15:58:47.047Z Reads: 189

```
👍🏼@okami
<img src="/uploads/db1493/original/3X/2/c/2c861a043bfffef743cada33cf01e965b077e92c.JPG" width="666" height="500"><img src="/uploads/db1493/original/3X/5/6/56c7c4900c17ffbdb4ef2bab0d53b693196e2e8c.JPG" width="666" height="500"><img src="/uploads/db1493/original/3X/1/b/1be41ccb1411dd1566d6f58fb7138076da8d061d.JPG" width="666" height="500"><img src="/uploads/db1493/original/3X/c/a/cae2993998e2a76d26d2a38eb61c092789e1a273.JPG" width="666" height="500"><img src="/uploads/db1493/original/3X/9/b/9b2e34a2b6f58fe519fe9ccee1a276b105eb91a7.JPG" width="666" height="500"><img src="/uploads/db1493/original/3X/0/3/03dbea32c1a10f61cfc04d676ebaa963f6d760de.JPG" width="666" height="500">

It looks tighter then it's is on the pictures.
I must measure tomorrow but I think it's about 20mm space there. Maybe I should remove a part of the frame in the end but it looks good for placing an drive wheel with belt in the heck.
```

---
## \#14 Posted by: Hummie Posted at: 2016-12-05T16:04:16.891Z Reads: 171

```
Excited to see how this turns out please do some video of what it will do.  I've never seen that thing in action.  Hub motors on the front might be the easiest way to do it or maybe you could find one for the back.  They look like abnormally thin axles.  Back single hub I've seen stuff that would likely fit.
```

---
## \#15 Posted by: Okami Posted at: 2016-12-05T16:31:19.325Z Reads: 173

```
Is the axle rotating along the wheel or the wheel is seperate? If the axle is also moving,, it might be possible to mount the pulley directly on the axle,.. though some sort of method for fixating it in place might be needed..but at least you would not need to create a hub plate or put some sort of screws through the spokes..

For me it now looks like that there should be at least 10mm space.. so you might be able to fit 10mm pulley or perhaps a chain sprocket, if you have to go that direction (I think it was around 1/6.5'' / ~4mm in widht, so about 6mm more narrow or so than a 9mm belt pulley)

---

Hub motors would save you the hassle of figuring out how to place / position the motor in the right angle/place.. though Im not so sure how easy it might be to find it in the right size and also to suit your conditions..

perhaps @Hummie can recommend where to get ~80-50 sized motor and how to apply urethane to it.. I assume the diameter of the hub motor / wheel should be close to 120mm.. not to make the front higher up from the ground.


---


I am also quite interested in how this project of yours progresses.. I think this one could set a ''benchmark'' for other builders to go into more unconventioanal builds :slight_smile:

The last crazy 3 wheeled board I've seen here is called Frankenboard or similar.. it had more like a skateboard deck but also 3 wheels (only quite bigger than yours)
```

---
## \#16 Posted by: Hummie Posted at: 2016-12-05T16:39:14.420Z Reads: 149

```
I can't recommend or even direct you to a specific hub motor for the rear or the front as I don't really know what the situation is and if the axles spins even.  If you look on alibaba or google search in sure you can find a hub motor that size
```

---
## \#17 Posted by: Okami Posted at: 2016-12-05T17:12:20.532Z Reads: 144

```
ah, I think Im bad at searching china hub motors.. the closest I got is this:

https://www.alibaba.com/product-detail/5-inch-250w-electric-scooter-bicycle_501112624.html

It is really underpowered.. has really thick axles.. and im not even sure it is really 5'' (~120mm). From the sketch it looks like 130mm in size.

--

And custom made hub motor is probably out of the question for this build :D that just takes too much time and effort..
```

---
## \#18 Posted by: Weberp7593 Posted at: 2016-12-05T18:05:57.889Z Reads: 150

```
Thank you guys but I must say I already bought the SK3 and because of my budget I really want to use it.
Or maybe want to change with me and an Hub Motor? :wink: (SK3 6374 149kv).
The easiest way to do it would be an friction drive like they use in (endless sphere and co).
But I really want an "direct" drive and if I can I wish I can do it with an belt... so jeah your recommends are really good maybe I am using an 10mm belt system.

Also I will do an Build Thread when I am ready with planning so you can be up to date with the build :smile:
I think it will be a funny vehicle and with smaller motor and limited speed it would be perfect for kids...

But I will go professional with it :smiling_imp:

Oh and the axle is stare (don't know if this is the right word) I mean they are not spinning it's normal ABEC bearings on the wheels.

So in the next days I will measure a bit and will check if I can mount in in the front or rear...
Then I will check which Pulleys and co I will buy...
Or maybe someone want to change with me :wink:...

So let's see, I will open the thread the next days.
And of course I will do an video and upload it 👍🏼
```

---
## \#19 Posted by: Alken Posted at: 2018-05-08T05:49:11.937Z Reads: 133

```
Hi,
I had a similar project in the last months. 
Managed to make it work. 8 LIIONS in the steering tube and a hub Motor at the back. Works great now

![image|374x500](upload://vtDzpsbRbBT9aFt10yEq4h0D5lA.jpeg)
```

---
## \#20 Posted by: Alken Posted at: 2018-05-08T05:54:57.690Z Reads: 134

```
I have added a vesc, a BMS for charging and an on/off Switch.

![image|690x388](upload://dZqybtgDpAbp9502B89qb6exyuT.jpeg)
```

---
## \#21 Posted by: manu78 Posted at: 2018-05-11T08:43:08.056Z Reads: 120

```
hi Alken,

how did you managed the motor at the rear in term of axl lenght? 
How did you managed to maintain it to the fork?
Is it a 4 or 5 inches hub motor? Does it have enough power in uphill? 
Thanks for your response.
```

---
## \#22 Posted by: Alken Posted at: 2018-05-11T21:16:48.448Z Reads: 112

```
Hi,
It is a 4inch hubmotor. A 5 inch might also fit. I have extended the existing holes to fit the axle of the hubmotor. I had to secure the motor with nuts from in between the suspension points since the axle was not long enough. But it is mounted very safe this way. 
It could have a bit more power to go uphill.  The steering stick (which is a new aluminium profile) could provide space for two more batteries to have a 10S pack. ![image|375x500](upload://ogMC0UjuVAqkRl9zhjIwziRqjNc.jpg)
```

---
## \#23 Posted by: manu78 Posted at: 2018-05-14T14:10:25.041Z Reads: 104

```
Thank you Alken,

Have you got any video to show? 
i am hesitating because of the low power. I am also considering a different solution with a hobbyking motor. But the installation is much more complicated...
```

---
## \#24 Posted by: Alken Posted at: 2018-05-23T11:10:33.144Z Reads: 95

```
Hi,
Currently I am adding some features. As soon as I am finished I will post a video.
If you are more Interested in speed  instead of stealth, a separate motor might be the better option.
Or maybe there might be better hub Motors... with a bit more voltage, riding would be a bit more interesting.
```

---
## \#25 Posted by: Dmaxx Posted at: 2018-05-23T14:53:53.504Z Reads: 94

```
This was my take on the subject
![20180425_140456|690x388](upload://uLWYSwevew6GOXvOnHXOKONBSoV.jpg)![20180425_140449|690x388](upload://e3kbFA9EcCD2IDRAjyhr2llIijK.jpg)![20180424_085510|281x500](upload://gqsOcleY0BiR7UbyWBKuM0FG3eI.jpg)
10s3p i got for cheap from @GrecoMan, sealed 6374 190kv motor, focbox with case from @Kug3lis, Torqueboards motor mount, electric throttle and brake and lots of custom stuff. This is a frankenstein and it hauls ass!! (For my wifey😉)
```

---
## \#26 Posted by: mmaner Posted at: 2018-05-23T19:11:28.364Z Reads: 80

```
What did you do for a throttle?
```

---
## \#27 Posted by: Dmaxx Posted at: 2018-05-23T19:37:07.594Z Reads: 75

```
@mmaner, i used an ebike thumb throttle for the throttle and a second one for the brake. They use the adc pins in the uart plug and 3v3/gnd
```

---
## \#28 Posted by: mmaner Posted at: 2018-05-23T20:10:11.780Z Reads: 72

```
good info, thanks
```

---
## \#29 Posted by: Battosaii Posted at: 2018-05-23T21:05:13.200Z Reads: 73

```
I've heard you can wire in the thumb throttle to where the receiver usually goes on a vesc.
```

---
## \#30 Posted by: mmaner Posted at: 2018-05-23T21:06:43.776Z Reads: 74

```
Thats what Im trying to figure out.  I got my wife a segway ninebot, its anemic as hell.  I wanna replace the battery and ESC with 30q pack and VESC, maybe keep the existing hub motor, maybe not.  I need to tear it down and take look at the guts :slight_smile:
```

---
## \#31 Posted by: Alken Posted at: 2018-11-10T11:58:01.232Z Reads: 56

```
Hi there,
I have finally found some time to enhance my build. I have made some changes. Most importantly I have changed the case for the focbox and the BMS to a 3d printed case (I needed a bit more space). The design is not perfect but very simple and created in a way so I can mount the case to the deck using screws.  Additionally I have managed to add cables from the handle to the focbox to make an ADC control with a small joystick possible. Thereby a remote control is not required which has the advantage of a free hand and a bit more stealth.
A first measurement has shown a maximum speed of 21kmh. I hope to get it legally authorized in Germany with a few adaptations (lights and so on) when the new law for small electric vehicles is in place (maybe 2019).   I have attached some pictures of the build and the case.![E-Kickboard_Case|690x427](upload://lDUPNPGeqrJIZVd7lrRYQ4p8kIN.png) ![1|235x500](upload://jdkoWJQ0aSYeE8btr6W6WAU9exI.jpeg) ![3|690x260](upload://84pLP5Q2f40WWqJxxHLW8mrOy0K.jpeg) ![2|197x499](upload://vHU53S1be6q4wCSj5X3VOJJpWT7.jpeg)
```

---
## \#32 Posted by: Cuprani Posted at: 2019-09-03T14:55:05.239Z Reads: 38

```
I was looking into the same kind of build, but I actually wanted to mount the front end steering mechanisme onto my longboard.

But most important question.. how does it ride?
Is it more of a scooter or does it ride as a skateboard? How does it steer at higher speeds?
```

---
## \#33 Posted by: murdomeek Posted at: 2019-09-03T19:35:47.550Z Reads: 27

```
@Dmaxx
where'd you get the griptape?
```

---
## \#34 Posted by: Dmaxx Posted at: 2019-09-03T23:08:47.893Z Reads: 26

```
I cut it out on a cnc machine
```

---
## \#35 Posted by: manu78 Posted at: 2020-02-07T21:31:13.605Z Reads: 11

```
Hi there, here is my mod, it is very powerful and very pleasant to ride. 
I made several attempts, the goal was to improve the comfort especially when is road is not smooth. All wheels are air wheels. top speed is 35/40 km/h but acceleration is very strong so I lust be very careful 
![image|375x500](upload://gA8QINgU7QdOyq7yoEKv7eBLE41.jpeg)
```

---
