# Does increasing battery voltage increase torque?

### Replies: 30 Views: 3503

## \#1 Posted by: Zoomy Posted at: 2017-05-26T04:23:50.202Z Reads: 254

```
I currently have a 6s setup, soon to be 12s and am wondering if I need to adjust my gear ratio for this transition if the torque is affected by voltage. My intuition tells me it wont be but then I think this can't be true...

If this is not true then where does that extra energy go when hammering the throttle? As Voltage X Amps = Power
```

---
## \#2 Posted by: chuttney1 Posted at: 2017-05-26T04:51:22.173Z Reads: 250

```
Short answer, kind of. Long answer, a low motor constant and a short final drive ratio gives more torque at the expense of speed.
```

---
## \#3 Posted by: Janis Posted at: 2017-05-26T12:26:01.662Z Reads: 228

```
Overall you will be pulling more power which translates to increased torque.
You should setup your gearing based on how fast you want to go.
```

---
## \#4 Posted by: TarzanHBK Posted at: 2017-05-26T12:49:18.638Z Reads: 218

```
also depends on your system. Which motor kV, are you using a Vesc, gearing, wheelsize?
```

---
## \#5 Posted by: NickTheDude Posted at: 2017-05-26T14:34:20.233Z Reads: 199

```
Yes, if you gear it too.

If you had two boards that we're identical, one on 6S and one on 12S, the 12S board would have double the top speed, and presumably similar or identical torque.

However, if you adjusted the gearing (or kV) to make the top speed of the boards identical, the 12S board would have double the torque.

Theoretically I think that's how it would work out.
```

---
## \#6 Posted by: Challlsss Posted at: 2017-05-26T14:59:21.971Z Reads: 186

```
@NickTheDude That sounds right. 
Voltage = motor speed 
Current = torque
gear ratio is what allows you to change the balance between torque and speed.
```

---
## \#7 Posted by: t0m_r1dd1e Posted at: 2017-05-26T18:26:14.073Z Reads: 164

```
Sorry man but this isn't correct. 
As Janis stated above, POWER equals torque. So assuming all else equal, a 6s system running at 30 amps will be making half the speed AND half the torque as the same system on 12s at 30 amps. 

Source: https://electronics.stackexchange.com/questions/39387/how-are-current-and-voltage-related-to-torque-and-speed-of-a-brushless-motor

TL;DR: "For the same motor, ideally if you apply double the voltage you'll double the no-load speed, double the torque, and quadruple the power."

This is why people run higher voltage batteries. It lets you pull less current to make the same amount of power.
```

---
## \#8 Posted by: Challlsss Posted at: 2017-05-26T18:40:17.772Z Reads: 154

```
@t0m_r1dd1e Disagree. If we reference the webiste you linked...

 https://electronics.stackexchange.com/questions/39387/how-are-current-and-voltage-related-to-torque-and-speed-of-a-brushless-motor


<img src="/uploads/db1493/original/3X/c/c/ccca94fb4745bad91b3ac2c9bb80a9777eeea30f.png" width="686" height="177">

So Voltage = speed

<img src="/uploads/db1493/original/3X/7/f/7f401232cafa1dadc3edada7da1feedd41dc1b9b.png" width="690" height="169"> 

So Current = torque

IE if current is constant then torque is constant.
if voltage is constant then speed is constant.

The torque will likely be higher on a 12S system, _not because there is a higher voltage_ but because you will likely use a higher gear ratio to get the desired top speed. Assuming all gear ratios and current draws are constant then 12S and 6S are identical in terms of torque.
```

---
## \#9 Posted by: t0m_r1dd1e Posted at: 2017-05-26T18:50:40.883Z Reads: 139

```
lol well now I'm just real confused because that formula seems to contradict what he says later in that post. Going to do some more research.
```

---
## \#10 Posted by: Challlsss Posted at: 2017-05-26T18:53:20.824Z Reads: 135

```
@t0m_r1dd1e At the end of his post It looks like he forgot to say if you double the voltage _and current_  that you will double speed torque and quadruple power. If you just double voltage you will double power and speed. But not torque.
```

---
## \#11 Posted by: t0m_r1dd1e Posted at: 2017-05-26T19:05:24.878Z Reads: 132

```
Thanks for the explanation. I'm really trying to get my head around this. 

I found something else: On the wiki page for Torque, it shows various formulas involving torque and one of them is this:

Power = torque * 2pi * rotational speed. 

So where you said "If you just double voltage you will double power and speed." yes that's true, OR if you double voltage and keep rpm constant, you will have double the torque at that speed. 

And also like you said, if you double speed and torque, it takes 4 times the amount of power. 

At least that's what's making sense in my head right now. If I'm still wrong, please explain.
```

---
## \#12 Posted by: Challlsss Posted at: 2017-05-26T19:09:11.754Z Reads: 125

```
you can correct me if I'm wrong but in my experience that is not possible. When you double voltage you **will** double speed, assuming you dont load the motor. When I am riding my board it doesn't matter how little I press on the throttle, eventually the board reaches top speed. IE the controller only effects current and can't slow down the motor. It can only control how much torque the motor exterts. So unless there is a lot of friction/wind/a hill, double voltage == double speed.

This is personal experience though.
```

---
## \#13 Posted by: PXSS Posted at: 2017-05-26T19:20:45.584Z Reads: 119

```
[quote="t0m_r1dd1e, post:11, topic:23932"]
OR if you double voltage and keep rpm constant
[/quote]

You cant do this without switching to a motor with twice the kv. 
@NickTheDude is correct on everything so far
```

---
## \#14 Posted by: t0m_r1dd1e Posted at: 2017-05-26T19:32:48.907Z Reads: 117

```
Here's what I mean from the formula from wiki. 

Power = torque * 2pi * rotational speed

Let's say two identical boards, 6s and 12s, each travelling at a constant 10mph. If they're identical boards, with the same rider weight, on the same road surface with the same hill grade, wind etc, then torque is the same on both boards, right? Torque is however much rotational force is equal to the resisting forces of friction, gravity, wind resistance, etc.

So if torque and rotational speed are equal, then the boards power output is the same. 
Power of board 1 = Power of board 2

And since power = voltage * current:
12s * 0.5 current = 6s * 1 current
```

---
## \#15 Posted by: Zoomy Posted at: 2017-05-26T22:05:30.388Z Reads: 107

```
Would identical 12s and 6s boards be able to draw the same amount of current? This means that a 12s board on same gearing ratio, kv, wheel size would have more torque if the statement above is correct right? 

I will be making the conversion in a couple of weeks so I can put some practical tests behind this. Once I do this I will be excited to show off my first build!!
```

---
## \#16 Posted by: t0m_r1dd1e Posted at: 2017-05-27T17:23:01.514Z Reads: 101

```
If my statement is right, then yes. But I'm in no means certain about that. I'm still trying to work through and understand it. But yes, a 12s and a 6s should be able to output the same current, all other things (number of cells in parallel, type of cells, BMS fuse) equal. 

Very cool! Do you have a way of measuring current with your 6s setup before doing the conversion? If you have a VESC and a bluetooth module you can do it. I'd love to see how it compares to the 12s current draw on the same road at the same speed.
```

---
## \#17 Posted by: Zoomy Posted at: 2017-05-27T21:18:16.412Z Reads: 96

```
I've been having a bit of trouble with my Bluetooth module but I will do some tests!
```

---
## \#18 Posted by: mattfink Posted at: 2017-05-27T21:31:00.013Z Reads: 96

```
My understanding is that the theoretical maximum speed is voltage x KV which is where back emf balances out the battery voltage, and that as the motor accelerates towards that speed the current draw decreases and so does torque proportionally. From maximum current draw at stop and min at KV x voltage. 

So in the 6S / 12S example 
At any given speed the 12S motor is further from max speed and therefore drawing more current and therefore has more torque at any given speed. 

If the 12S didn't have more torque at the 6S max speed then it wouldn't be able to accelerate beyond that speed as the forces of resistance would be in balance with the torque produced. 

Further tho' as max available amps the motors can draw hasn't changed, at peek load, (starting from standstill, steep hill) the max torque may be the same for both. 

That's how I'd understood it but I'm learning myself
```

---
## \#19 Posted by: Namasaki Posted at: 2017-05-28T02:46:21.688Z Reads: 86

```
Early on I had a setup with 2 6s Lipos connected with bullet connectors and I could easily switch them from series to parallel.
12s 5ah  or 6s 10ah
The 12s option was a lot faster with a lot more torque than the 6s option which I only used for slow cruising on the board walk around lots of pedestrians.
These comparisons where made with same batteries, motors, gears, wheels and everything else.
So the answer to "Does just raising voltage render more torque", Yes it does!

I have no explanation or equations to back this up, just some real life comparison road testing.
```

---
## \#20 Posted by: PXSS Posted at: 2017-05-29T12:23:20.152Z Reads: 81

```
[quote="t0m_r1dd1e, post:14, topic:23932"]
So if torque and rotational speed are equal, then the boards power output is the same. 
Power of board 1 = Power of board 2
[/quote]

You do not need to go any further than this statement to get your answer. Specifically this: [quote="t0m_r1dd1e, post:14, topic:23932"]
torque and rotational speed are equal, then the boards power output is the same.
[/quote]

If your speed is the same, your torque at said speed is also the same. 

[quote="Zoomy, post:15, topic:23932"]
Would identical 12s and 6s boards be able to draw the same amount of current?
[/quote]

No. They can provide the same amount of **power**. So if you have a 12s that can do 30A and then place the halves in parallel, the resulting 6S can do 60A

[quote="t0m_r1dd1e, post:16, topic:23932"]
12s and a 6s should be able to output the same current, all other things (number of cells in parallel, type of cells, BMS fuse) equal.
[/quote]

In this example, you just doubled the number of cells. You doubled the number of cells in series and kept the number of cells in parallel the same. This means that the 12S pack has twice the power than the 6S because it has twice as much battery 

Sorry it took me so long to reply...
```

---
## \#21 Posted by: Zoomy Posted at: 2017-05-29T19:46:58.294Z Reads: 71

```
Since I will be adding batteries to my board instead of switching from parallel to series, this should mean that they will put out the same amperage. 

Can I conclude that my board should theoretically have more torque as well as top speed if I do not change anything else apart from battery voltage?
```

---
## \#22 Posted by: PXSS Posted at: 2017-05-29T19:52:02.398Z Reads: 68

```
If you double the battery, then yes, you double the power. 

E: @Zoomy It really has nothing to do with the voltage increase though as you could also just add the cells in parallel and double your power.
```

---
## \#23 Posted by: Zoomy Posted at: 2017-05-30T02:03:24.225Z Reads: 60

```
@PXSS however my motor can only handle 2x more voltage and not 2x more amperage.
```

---
## \#24 Posted by: Challlsss Posted at: 2017-05-30T14:23:58.126Z Reads: 56

```
Then do double the voltage, and change up your gear ratio, unless you want to go hekin fast.

<img src="/uploads/db1493/original/3X/7/3/73bbbf1fd49b028764334f62ae3716c5b7ca5822.png" width="500" height="341">
```

---
## \#25 Posted by: ugothakd Posted at: 2017-06-07T03:21:01.308Z Reads: 50

```
Here's a question...let's say you have one setup, 12s, 100kv motor, 2:1 gearing
then you have another setup, 6s, 200kv, 2:1 gearing
same size motor. Which has more torque? They have the same amount of **power** but one setup draws more amps at a lower voltage, one draws lower amps at a higher voltage.
```

---
## \#26 Posted by: PXSS Posted at: 2017-06-11T11:49:57.048Z Reads: 46

```
If you're going at the same speed,
Mechanical Power = Rpm*Torque always. 
So they would have the same torque
```

---
## \#27 Posted by: Zoomy Posted at: 2017-06-11T19:17:56.212Z Reads: 44

```
Would increasing the battery voltage not increase mechanical power?
```

---
## \#28 Posted by: ugothakd Posted at: 2017-06-12T02:57:46.006Z Reads: 41

```
With the same motor, yes it would. But if you have a motor of double the kv with the original voltage you draw more amps per volt, so the power is the same. It looks like this, given the motors are the same physical size.
300kv = 16.8 v x 80 amps = 1344 watts
150kv = 33.6v x 40 amps = 1344
```

---
## \#29 Posted by: PXSS Posted at: 2017-06-12T03:17:13.721Z Reads: 40

```
Given the same speed and battery size.
```

---
## \#30 Posted by: Challlsss Posted at: 2017-06-23T19:55:28.370Z Reads: 36

```
[quote="ugothakd, post:25, topic:23932, full:true"]
Here's a question...let's say you have one setup, 12s, 100kv motor, 2:1 gearing
then you have another setup, 6s, 200kv, 2:1 gearing
same size motor. Which has more torque? They have the same amount of power but one setup draws more amps at a lower voltage, one draws lower amps at a higher voltage.
[/quote]

provided we are assuming the 6S setup is capable of doing *double* the current. The torque would be the same and top speed would be the same.
```

---
