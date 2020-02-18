# Scooter motors on Mountain board - Build Report

### Replies: 17 Views: 602

## \#1 Posted by: Iuliu Posted at: 2019-07-18T15:39:12.334Z Reads: 175

```
Hi, inspired by @Martin hub motor build, I decided to go with two scooter hub motors.  
I used two 350w [Motor](https://www.ebay.com/itm/8-Electric-Scooter-24V-36V-48V-DC-Hub-Wheel-Motor-Toothless-Brushless/323712797255?ssPageName=STRK%3AMEBIDX%3AIT&var=512706536086&_trksid=p2057872.m2749.l2649) on this [truck](https://www.aliexpress.com/item/32896745192.html?spm=a2g0s.9042311.0.0.44364c4d0MNI4w) .
![IMG_20190718_151312|666x500](upload://6u2qDbx4xh3mXR4DOZu8ptLuu3u.jpeg) ![IMG_20190718_151317|666x500](upload://spHVh81ro99sYh0EIpX2ncdUwUe.jpeg) 

The ESC is a Chinese substitute [board](https://www.ebay.com/itm/6S-24V-Electric-Skateboard-Controller-Dual-Motor-Drive-w-Remote-ESC-Substitute/173674345348?_trkparms=aid%3D111001%26algo%3DREC.SEED%26ao%3D1%26asc%3D20160908105057%26meid%3D3780139cddb041f68ada4b43a45f3f7f%26pid%3D100675%26rk%3D3%26rkt%3D15%26sd%3D323712797255%26itm%3D173674345348%26pg%3D2481888&_trksid=p2481888.c100675.m4236&_trkparms=pageci%3A6cbbd3d1-a974-11e9-baa2-74dbd18092c8%7Cparentrq%3A05cb65a916c0acc7c67fc5c5ff6d3716%7Ciid%3A1), I am currently waiting for my [odrive ](https://odriverobotics.com/) to arrive. Since I am a robotics engineer and doing my master in computer vision, I am trying to get an intelligent board, self balance+aid in lining on the bike road+ control the speed for each motor by a joystick for a smoother control.

The battery case is 3d printed, I am currently working on a non-tape involved build with double the amount of 18650, but should be good enough for a few days.
I tried placing the motor directly on the truck, then remove the rubber from the wheel and connect it to the mountainboard original wheels, but my skills of working on the metal lathe suck, so it's I left it for a later version
```

---
## \#2 Posted by: AlanZhou Posted at: 2019-07-18T16:06:29.392Z Reads: 160

```
That looks like it has really bad wheelbite.
```

---
## \#3 Posted by: esk8snith Posted at: 2019-07-18T17:29:26.363Z Reads: 153

```
good stuff man, I'd be interested to know how this build turned out.

top speed?
acceleration?
Are these motors sensorerd?
```

---
## \#4 Posted by: Iuliu Posted at: 2019-07-18T20:03:45.418Z Reads: 132

```
So far i can't measure them, i need to upgrade the battery to a 11s12p 18650 instead of current 10s4p 18650. The motors have a hall sensor, rated for 36V 350w. My esc currently barely can output more then 430 for both motors, still, i get a quite high speed, more then i can handle at this point since i am just a beginner.
```

---
## \#5 Posted by: Iuliu Posted at: 2019-07-18T20:05:31.509Z Reads: 123

```
Yea, they are close, but never touched. It should be fixed with a modified 15.5 trampa truck
```

---
## \#6 Posted by: esk8snith Posted at: 2019-07-18T23:06:22.108Z Reads: 118

```
ahh I see. I think 11s12p is over kill. If you use 30Q/25R you should be good with 4p or max about 6p if you want the range. More than that is really unnecessary

how many mi/h or kmph are you getting?
```

---
## \#7 Posted by: Martin Posted at: 2019-07-19T00:31:24.896Z Reads: 111

```
Hi friend, you made it. 
How about the torque and the max speed ?
It seems a little heavy.
```

---
## \#8 Posted by: Iuliu Posted at: 2019-07-19T05:37:44.048Z Reads: 103

```
Yea, i managed to get the first version and it's is indeed quite heavy, maybe 9-11kg. Based on what i can see, i can get easy over 25 km/h but some uphills are up to 10km/h. I am using a cheap esc that gives only 215w per motor at max and quite weak batteries which might limit it to ~150w, since it was just a cheap build to see how well everything fits tougher. The breaking is incredible strong though. 

My next step is to upgrade the battery, since these are some reusable 18650 and not rated for high current, i am getting an 11s 12p pack. 
Then in 2-3 weeks my odrive should arrive, so i can go with 13s12p.  
Next is to use some raspberry pi 3 and control odrive with a joystick (i already made the python code for joystick inputs.).
Then is to use 3 10axis IMU from another project and add some smooth controler+ balancing on the back wheels like a this - https://www.youtube.com/watch?v=jp_vRK7mbwY
Then finish it with a custom 15.5 trampa truck and remove the rubber wheel and connect them to my own wheels similar to yours.

The build is quite heavy, that's why i need joystick control so i can easier control then i turn and hoverboard like self balancing so it's easier for transportation- just follow me.
```

---
## \#9 Posted by: Iuliu Posted at: 2019-07-19T05:40:54.972Z Reads: 98

```
I am using some very low quality 18650 refurbished from laptops in my 10s 4p. Which give me a good drive for the first 3-5 km, but then uphills is just slow. The 11s12p is with better quality batteries and more in parallel  for less voltage drop since my area is mostly hills and downhills.
```

---
## \#10 Posted by: Okami Posted at: 2019-07-19T08:28:41.036Z Reads: 85

```
Very nice project/build. Im intrigued. I like the part about joystick control. As I understand u should be able to make turns with remote control?
```

---
## \#11 Posted by: Iuliu Posted at: 2019-07-19T12:31:13.607Z Reads: 81

```
Yea, by changing the speed of each of the motors, i didn't receive my odrive yet. But i have been working on voice control using google api, so voice control could also be used to tweak drive parameters . There is a very nice python library for reading inputs from joystick. I will go with a generic joystick game pad, but i test few other joysticks i have and all of them seems to work.
```

---
## \#12 Posted by: Iuliu Posted at: 2019-07-21T19:43:14.989Z Reads: 65

```
I will keep with updates on the post below - https://forum./t/scooter-motors-on-and-inteligent-mountain-board-control-with-odrive/4689/14
```

---
## \#13 Posted by: wireload Posted at: 2019-07-25T21:24:19.865Z Reads: 46

```
Hey I'm interested to build a three wheeled longboard/scooter with this motor. How many amps are you running with them? do they have enough torque? Would you change them for any other motor if you have to buy again because I saw a lot of sellers selling xioami m365 motors?
```

---
## \#14 Posted by: Dog Posted at: 2019-07-28T16:38:25.838Z Reads: 40

```
I always wanted to do that!!

But I’ve always thought that the hub motors are designed for a different weight distribution, aka in a “bike” type fork and attaching them to a truck only from one side would eventually bend the axle in the hub.

What are your thoughts on that?
```

---
## \#15 Posted by: Iuliu Posted at: 2019-07-30T17:11:36.162Z Reads: 31

```
They are quite strong. I was driving at about half of their power, but all the hills i have encountered seems not to be a problem. I have a dual setup
```

---
## \#16 Posted by: Iuliu Posted at: 2019-07-30T17:14:32.762Z Reads: 32

```
The bearings are quite strong though. The issue i am having is that the truck is designed for a wider axle, i did a quick fix, but i am not sure how safe it is.
```

---
## \#17 Posted by: Dog Posted at: 2019-07-31T20:14:36.712Z Reads: 20

```
Could you please take a few pics of the trucks and how you mounted motors on them? Also the maximum lean without a wheelbite.

I had this project in my head for months and I abandoned it because I thought the motors will be ruined, but now I’m inspored again.

I want to do a 4 wheel drive with mijia x365 10” 250w motors
```

---
