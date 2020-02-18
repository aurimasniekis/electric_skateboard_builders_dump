# How do you calculate for a dual motor setup?

### Replies: 12 Views: 1530

## \#1 Posted by: sub6ix Posted at: 2018-03-19T21:29:07.645Z Reads: 241

```
I am trying to come up with accurate calculations for my board by using this calculator and by using pen and paper. On this [calculator](http://calc.esk8.today/advanced/) , how would I account for their being dual motors?

Edit: Not too sure which section to post this in.
```

---
## \#2 Posted by: RedEagle Posted at: 2018-03-19T21:40:47.555Z Reads: 235

```
The main advantage of dual is traction. Your setup wil be a bit heavier than single drive, but your system will run cooler because the load is shared between two motors instead of one.
Not sure what you're trying to calculate. Mind elaborating?

Edit: I think I see what you mean. There is no way to add a second motor in the calculator. Nevertheless, the difference is negligible.
```

---
## \#3 Posted by: sub6ix Posted at: 2018-03-19T22:41:19.667Z Reads: 207

```
Yeah I am trying to calculate distance and speed for the most part. My original thoughts were that it is a negligible difference but I just want to make sure of that.
```

---
## \#4 Posted by: RedEagle Posted at: 2018-03-19T22:44:03.420Z Reads: 200

```
I think if you calculate for single the same result is true (or close) for dual. Can someone else reading this confirm?
```

---
## \#5 Posted by: NickTheDude Posted at: 2018-03-19T22:47:44.801Z Reads: 180

```
I think it might be the case that you'd have a slightly higher top speed with dual since you have more torque and it might be able to pull closer to that max ERPM. That being said you also have less efficiency since you got twice the belts.

Overall, with equal power outputs I would expect the differences to be pretty small though.
```

---
## \#6 Posted by: sub6ix Posted at: 2018-03-19T22:51:22.168Z Reads: 169

```
Ok that makes sense to me. Is there anywhere I can find the formulas so I can do the calculations by hand? I am trying to have evidence of my calculations and compare it to the real world performance of the board for a school project.
```

---
## \#7 Posted by: NickTheDude Posted at: 2018-03-20T03:09:47.219Z Reads: 144

```
Calculating top speed isn't too difficult but range can be a lot more complicated.

For speed you need to first understand kV. Basically it just means how many RPM your motor will spin at per volt supplied to it. So a 100kV motor will spin at 100RPM when at 1V, 200RPM at 2V and so on.

So to determine the maximum RPM of you motor you multiply the kV of the motor by the maximum voltage of the battery. For something like a 10S battery at full charge it would be 42V. I don't know what your setup is but max voltage * motor kV will give you the max RPM of your motor. You then need to multiply that number by the reduction ratio you have in your gearing. For example a 18T motor pulley and 36T is 18/36 which is 0.5. After you multiply this will be the RPM of your wheel.

You then need to take into account the distance your wheel is going to travel in one rotation. This is going to be the circumference of the wheel. So 2pi*radius, radius being the diameter of your wheel divided by 2.

You then multiply that distance by the rpm, which will give you the distance traveled in one minute. If you used mm units for your circumference calculation the this figure will represent top speed in mm/minute. Convert that to km/hour and you have your top speed.

Sorry if that was overly simplistic or patronizing but idk where your at in terms of mathematics so I tried to make it relatively simple. 

For range you need to understand watts and watt hours, estimate your boards average watt consumption over time and compare that too the watt hours of your battery pack.
```

---
## \#8 Posted by: trancejunkiexxl Posted at: 2018-03-20T03:52:14.966Z Reads: 119

```
physics A trauma.. seems so fresh in my mind
```

---
## \#9 Posted by: sub6ix Posted at: 2018-03-20T17:01:02.929Z Reads: 107

```
Yeah I'm taking calculus and physics so I'm not afraid to learn a little because it can only help. I did those calculations already a couple weeks ago. The part that really stumps me is calculating the torque with my weight on the board. Any idea how to go about doing that?
```

---
## \#10 Posted by: NickTheDude Posted at: 2018-03-20T18:06:46.846Z Reads: 100

```
That one I'm not entirely sure about. However I do know that theres another motor constant called kT that has something to do with current and torque in a motor. This might be helpful: https://en.wikipedia.org/wiki/Motor_constants

One thing to keep in mind is that at all points while accelerating your torque and power figures are going to be different. The VESC is really good since it can log all of these values and people have made apps that let you get a readout of them while riding. There are some nice videos that have these values overlaid on them.

The torque is going to be at its peak when you're first taking off and it lowers as you accelerate faster. If you watch one of these videos and pay attention to the motor amps figure, or log these values yourself you should be able to figure out your motors kT and use that to calculate how much torque you're using while taking off, as far as peak possible torque goes, it would depend on your VESC settings as you can tune the maximum motor amps there.

https://www.youtube.com/watch?v=vNNcW0CIh5Y&t=15s

https://www.youtube.com/watch?v=Y8QkQTsjO6Y
```

---
## \#11 Posted by: sub6ix Posted at: 2018-03-20T18:17:17.331Z Reads: 89

```
Wow I didn't know about that feature. I'm going to have to try that out. Thanks for the help!
```

---
## \#12 Posted by: NickTheDude Posted at: 2018-03-20T18:36:14.275Z Reads: 87

```
No problem. Good luck on the project!
```

---
