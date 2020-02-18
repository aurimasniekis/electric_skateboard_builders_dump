# Upgrading the motor on a bought skateboard

### Replies: 24 Views: 3184

## \#1 Posted by: Pickwick Posted at: 2017-04-29T18:52:34.695Z Reads: 138

```
Hello. I am pretty new at this, just so don't kill me if I make say something stupid :slight_smile:

I bought an electric longboard for a year ago. Now I am interested in an upgrade of the motor for a faster acceleration and top speed. 
I am not the greatest at electronics, but I now a little. I know I have a 25V battery on my skateboard, and I'm not really interested in replacing it (yet). 
I have been looking at this: 
https://hobbyking.com/en_us/turnigy-aerodrive-sk3-6374-192kv-brushless-outrunner-motor.html

If I have a 25V 8Ah lithium battery, and the max amp on the new motor is 80A, won't I get 2000W out of the motor then?
And will I run into trouble with my ESC because of the motor upgrade? (I know very little on the ESC) 

I now have a 1200W motor that runs about 20mph, and I hope it will get a bit faster

I hope somebody can help me learning. 
Regards Mikael :)
```

---
## \#2 Posted by: wmj259 Posted at: 2017-04-29T19:59:47.030Z Reads: 124

```
You will have to look into the ESC as companies provide barely enough headroom for personal upgrades.
```

---
## \#3 Posted by: Pickwick Posted at: 2017-04-29T20:27:25.963Z Reads: 110

```
But do you think it is necessary to open it up? 
Will it affect the ESC if I change to motor?
```

---
## \#4 Posted by: Namasaki Posted at: 2017-04-29T23:46:17.324Z Reads: 100

```
It would help if you told us what make of board you are trying to upgrade.
20mph is actually pretty good. In my opinion, if your wanting to go faster, you should consider building a custom diy board.
```

---
## \#5 Posted by: Pickwick Posted at: 2017-04-30T08:11:30.183Z Reads: 85

```
You are probably right. I am just interested in a few more mph. It doesn't have to be anything wild. Don't you think it would be possible if the current motor is replaced? 
Thank you 

https://www.amazon.com/Electric-Skateboard-Longboard-Falcon-Board/dp/B01ILZ7Q7U
```

---
## \#6 Posted by: XIII Posted at: 2017-04-30T08:58:40.050Z Reads: 78

```
you can upgrade the motor. But you could just add 3s battery in series and a better speedcontroller. 

My friend had this board and I had the speedcontroller laying around. Now it goes just over 40km/h.
Not the best torque (motor is small) but still decent!
```

---
## \#7 Posted by: Pickwick Posted at: 2017-04-30T09:06:11.410Z Reads: 71

```
Okay. That sounds Exciting. Do you know which speedcontroller he used?
```

---
## \#8 Posted by: XIII Posted at: 2017-04-30T09:11:37.287Z Reads: 66

```
It was mine :) 
It is a 12s AlienPowerSystem controller, it is the same one as the Torqueboards 12s I think.
A vesc would also work :) since it's almost the same price and probably the better choice
```

---
## \#9 Posted by: Pickwick Posted at: 2017-04-30T09:25:18.244Z Reads: 65

```
Okay. Thank you! :smile:
```

---
## \#10 Posted by: KTMinni Posted at: 2017-04-30T11:01:59.041Z Reads: 63

```
Get a higher kV motor because you have a lower voltage.
```

---
## \#11 Posted by: Pickwick Posted at: 2017-04-30T12:34:00.676Z Reads: 57

```
How much higher do you think?
```

---
## \#12 Posted by: Pickwick Posted at: 2017-04-30T12:44:16.308Z Reads: 57

```
https://hobbyking.com/en_us/turnigy-g160-brushless-outrunner-290kv-160-glow.html
?
```

---
## \#13 Posted by: KTMinni Posted at: 2017-04-30T12:51:39.882Z Reads: 55

```
That looks about right, you might want to double check with @chaka post on motor kv
```

---
## \#14 Posted by: XIII Posted at: 2017-04-30T13:12:42.550Z Reads: 55

```
you will decrease acceleration by just going for higher kv. If you want more topspeed AND acceleration you need to upgrade the Cells in series and change to a ESC which can handle the extra voltage
```

---
## \#15 Posted by: Okami Posted at: 2017-04-30T13:26:09.678Z Reads: 53

```
Have you considered just switching out to bigger wheels?

Im not sure will the setup / board deliver enough power, but if you can retrofit the pulley, you might get the desired speed..

Have you tried to ''play'' with the numbers here?

http://calc.esk8.it/#{"batt-type-lipo":0,"batt-cells":6,"motor-kv":245,"system-efficiency":87,"motor-pulley-teeth":16,"wheel-pulley-teeth":36,"wheel-size":83}|

If someone has 90mm to try and they are flywheel clones, the pulley might fit.. looks somewhat similar.

Though when running the thing through calculator, it looks like you would better be off with 97mm wheels but then again they might not fit onto your deck nicely because of the size. Though im not super sure.

IF the motor kv thing is somewhat right and gearing too, then you might get extra 3mph.

<img src="/uploads/db1493/original/3X/e/2/e20438ca45dd03b21380f89111a22a468f84902d.png" width="690" height="345">
<img src="/uploads/db1493/original/3X/6/0/60037b4cd849b0f874c81478819c15ad1e2ea6cd.png" width="619" height="350">
<img src="/uploads/db1493/original/3X/1/3/13da1b8e4baac3bb7ed9cb40e6149a301a769247.png" width="654" height="358">

--

If you do still want to ''change motor'' route, then yeh, you would be better looking at 260-290kv motors, if you dont replace the battery and controller..

**The calculation numbers does not decrease the efficiency.. so okay, it might be more like 2mph in the end because of the lost torque or something.. though if someone around you has the big wheels or you can get them just to test it out.. I would maybe start with the wheels as that would require the least modification, I think, if the pulley fits straight to the wheels..

When I put 6'' inch wheels (pneumatic) with the same gearing and motor I get only about 15mph, then with 9''inch wheels, I get 22mph.

Ive got a big different in wheel size, but if you go from 83mm to 97mm, then there's also a big improvement in speed, I think.
```

---
## \#16 Posted by: KTMinni Posted at: 2017-04-30T13:51:13.657Z Reads: 38

```
Yes I realize but I was just giving motor recommendations because he said he wanted to upgrade the motor for speed.  With the current capacity he should go with a higher kV.
```

---
## \#17 Posted by: Pickwick Posted at: 2017-04-30T14:24:25.115Z Reads: 34

```
Thank you guys. That helped a lot :)
```

---
## \#18 Posted by: Pickwick Posted at: 2017-04-30T14:44:57.122Z Reads: 31

```
I'm going for an ESC change and 3S battery. 
Maybe some other wheels as well. 
I was just wondering.. Now I get about 36V to do with.. What about the charger then? Do I have to replace that as well? 
And do it do anything that the one battery is Li-ion and the other is Li-Po?
```

---
## \#19 Posted by: Okami Posted at: 2017-04-30T18:12:38.614Z Reads: 31

```
U should avoid connecting Lipo and Li-ion in series.. The voltage profiles just dont match (and capacities too)..

You can connect them in parallel and get more power or more range.. but not the other way around..

You need precisely the same type of battery, to be connected in series,

--

You can just buy 3 x 3S batteries (Lipo) and then replace the current battery you have!

As I said, if you want it to do it cheaply and dont want to switch out too many parts, just replace the mechanical part or the motor and hope that current electronics can handle the higher load you will put on the system..

Change the gear of the motor.. that costs the least, just find out what type of gear you need.

That does not mean it wont start to slip.. but you will gain more speed, with just 5-10$ of purchase.. not 100usd or something as you would pay for esc / battery or higher speed motor.

--

If you want better range speed or power from the ground up.. then yes, invest in ''system of parts''.. 

Though, I would say that with better esc you might as well also get better speed or power.. at least Ive heard it has sometimes happened.
```

---
## \#20 Posted by: Pickwick Posted at: 2017-04-30T18:34:08.100Z Reads: 25

```
When you say "the gear of the motor" do you mean the pulley? 

I will not mind buying a new battery. I'm just afraid if I buy a new ESC because of all that programming. I have no idea how to do that, after I have done some research.
```

---
## \#21 Posted by: Okami Posted at: 2017-04-30T18:50:02.918Z Reads: 27

```
Yes, I mean the pulley.

There are some ''general to use'' settings, but you will need to watch a couple of videos or go through some pictures to truly understand which settings are best. (if u choose to use vesc)
```

---
## \#22 Posted by: Pickwick Posted at: 2017-04-30T19:06:16.499Z Reads: 26

```
Yeah okay. I will try to do that. 
Thank you for your help :slight_smile:
```

---
## \#23 Posted by: Okami Posted at: 2017-04-30T21:03:01.819Z Reads: 21

```
You should inspect what kind of belt u have.. is it HTD 5 or HTD3

Then you can inspect the ''axle'' of the motor..

Whenever it has a ''flat side'' or flange..

<img src="/uploads/db1493/original/3X/d/f/df613c58905a88022c1dd0b68ac560e3cce6bee4.png" width="384" height="272">

<img src="/uploads/db1493/original/3X/1/4/1454889f692c5850d3c962a1dd2164cc5a07ad16.png" width="436" height="351">

So there are 2 types of pulleys.. and you need to find out which one you need.. either with screw or that little metal piece

----
Take a look at this thread:

https://www.electric-skateboard.builders/t/help-me-take-apart-my-benchwheelcrap/10618/21

Sometimes they are stuck.. and that's all.. will be hard to take them off unless you buy the tool..

This one might also help:

https://www.electric-skateboard.builders/t/enertionboards-com-how-to-securely-install-a-pulley-onto-a-esk8-motor/22

--

Forgot to mention - before you take off anything, try to count how many teeth your pulley already has.. Pulleys are in different ''sizes''.. But just find out whenever you got 15Teeth one.. or smaller.. and then you can check out can you find 18T or even 20T pulley.. Though it might mess a bit with belt, so in the end, if you cannot move your motor around, you might end up buying a different size belt too..

So yes, these 2 things:

Teeth of the motor pulley right now
Motor position - is it possible to move the motor a bit to one side or another, while it is still bolted?
```

---
## \#24 Posted by: Pickwick Posted at: 2017-05-01T05:02:55.510Z Reads: 16

```
I'll go exploring. Thanks again, it helped a lot.
```

---
