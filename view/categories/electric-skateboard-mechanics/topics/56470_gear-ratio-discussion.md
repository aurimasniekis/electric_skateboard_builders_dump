# Gear Ratio discussion

### Replies: 8 Views: 606

## \#1 Posted by: epster Posted at: 2018-05-23T11:06:49.157Z Reads: 145

```
Dear eSK8`ers,
I have got some questions and some things i would like to discuss with you. 
To start with almost everyone off you recommends to take a minimum of 16T motor pulley with a 6374 190kv motor with a 15mm belt. 
But when i Calculate it i get this: ![image|690x436](upload://fj9mZDSC9kCgROc3rN4Zp5uxcHB.jpg)
As you can see i calculate it with 5mm pitch 15mm belts so x1.89 x0.7 because the belts are going to be arround 260mm long. Lets say we Calculate the max torque for arround 3000rpm and take a 16T pulley. You get 1.3Nm x 0.80 x 1.89 = 1,9656Nm max. 
How is that possible that you can easily run 16T with HTD5 Belts without getting belt slip? 
![image|313x259](upload://hBJCIwYz6NCmgg9SdPuuInvZHme.jpg)
Do you guys use a higher tensioning force then 12lbf about 53N?

My other question is about mounting motor pulleys to a diy electric motor. Is it possible to mount a eskating pulley to a diy electric shaft? (I am not that experienced in this field).
```

---
## \#2 Posted by: xilw3r Posted at: 2018-05-23T12:08:18.598Z Reads: 123

```
Firstly, I would like to commend you on actually doing things this way, I kind of miss the calculated approach on this forum as most of the decisions concerning drive design basically go the "mouth to mouth" sort of way... I do like this because that guy did like this and so on.

And now for slippage, this table you provided does not actually account for slippage, that depends on the looseness of the belt and the centrifugal force (rpm and diameter of the pulley being the major factors here). And the formulas for calculating that are rather big, im sure you can find them in some more serious belt drive design manuals.

In fact yes, since we are all running at high belt speeds (to be efficient you need to try and max out the motors rpm, which can easily reach 6k for 192kv), the actual torque our belts are rated for is less than we put through them, but it only impacts the lifetime of the belts. No wonder people (especially aggressive riders) need to change out their stripped belts rather often. And this table is most likely designed to calculate for some industry standard lifetime of x hours ... If you look at the actual tensile strength of the belts its quite high.

I am sure no one has ever calculated their belt tension force around here :) 

For your last question, I am a bit confused. What do you mean mounting eskate pulleys to a diy electric shaft? You mean the shaft of your diy motor ? (PICS PLEASE sounds really cool !! ) If so the of course .. there is no specific eskate pulley, you can buy pulleys with no hole, you just need to bore it to the size of your shaft, or turn your shaft to the size of your pulley if you already have it. Mounting is possible in many ways... shrink fit with a bit of glue, keyways with circlips, setscrews (please, dont use setscrews, its cringey as hell, but seems very popular here for some reason)
```

---
## \#3 Posted by: epster Posted at: 2018-05-23T13:01:14.061Z Reads: 102

```
First of all Thanks for the quick reaction. 

I just looked up some formulas for belt tension. These look quite trustworthy. https://www.engineersedge.com/mechanics_machines/two_pulley_connecting_belt_design_and_calculations_10226.htm 

I am now going to try to solve those. Looking at the formulas i can`t solve those precisely at the moment because I didnt order my pulleys yet :grin:. Is it possible that you give me a estimation of what the max torque rating before belt slippage would be off a 16T pulley so i can check my calculations.

About my second question now i read it back its really confusing. My bad. I was talking about the DIYelectric motors. As you can see there is a keyway of 3x3 at the top. But my question is if the motor shaft would fit these 8mm bore pulleys from eskating europe and even if it would fit would it be a good fit or do i risk it getting lose.  
https://eskating.eu/product/custom-htd-5m-12-to-20-teeth-steel-motor-pulley-in-9121520-width/ 

collections/electric-skateboard-motors/products/electric-skateboard-motor-6374-190kv 
![image|690x459](upload://oMuRHySFBb5aFpDwr6NmLdvHOIW.jpg)
```

---
## \#4 Posted by: Deckoz Posted at: 2018-05-23T13:59:23.276Z Reads: 76

```
[quote="xilw3r, post:2, topic:56470"]
No wonder people (especially aggressive riders) need to change out their stripped belts rather often.
[/quote]

I blame this on improper tensioning of the belts. People that tension belts with no idler. It's either

- too tight causing premature belt and bearing wear
- too loose for the load(weight of rider) without enough width to create surface friction/adhesion

If you want the proper tension without belt skip or pre mature wear you need:

- wide belts like 15 or 20mm run super loose
![com-resize (1)|210x118](upload://hq6QohzNMrDEIGeVfiR5uNxDdGZ.gif)
- or you run an idler. Put the idler at the inner most position. Extend the motor so the belt is tight. Loosen the idler screw enough to slide with pressure. Spin the wheel 1/4 turn in the direction of travel. The idler will move to the proper tension. Tighten the idler bolt.
```

---
## \#5 Posted by: epster Posted at: 2018-05-23T14:25:04.043Z Reads: 67

```
After 2.5 hours of researching and calculating I am not able to figure it out (the belt tensioning force calculated). 
@Deckoz thanks for the tips will run it that way when i get all my stuff. 

But i still dont know if i can put the eskating eu pulley on the diy electric motor shaft.
Does anyone know that? I see that you use another pulley @Deckoz how is it mounted to your shaft?
```

---
## \#6 Posted by: Deckoz Posted at: 2018-05-23T14:27:18.287Z Reads: 68

```
[quote="epster, post:5, topic:56470"]
eskating eu pulley on the diy electric motor shaft.
[/quote]

The link above has options for 8 or 10mm bore..

The Diyelectricskateboard aka torqueboards motors have 8mm shafts. So the motor pulley you buy will need an 8mm bore :) pretty much all motors you buy except APS will have an 8mm shaft. APS have 10mm.
```

---
## \#7 Posted by: epster Posted at: 2018-05-23T14:29:13.323Z Reads: 67

```
This is the link: 
https://eskating.eu/product/custom-htd-5m-12-to-20-teeth-steel-motor-pulley-in-9121520-width/ 
You are able to get the 8mm bore so thats fine. But you can chose 2 options 1 screw or 2 but i dont know if i should get 1 or 2 screws and if it even fits.
```

---
## \#8 Posted by: Deckoz Posted at: 2018-05-23T14:31:36.331Z Reads: 62

```
Those don't look to have keyways so go as many set screws as you can(2). 

As far as fitment if it is 8mm it should fit..

If you are talking truck width. And running a 10" truck with a single 6374. Run the widest belt you can(15mm).
```

---
