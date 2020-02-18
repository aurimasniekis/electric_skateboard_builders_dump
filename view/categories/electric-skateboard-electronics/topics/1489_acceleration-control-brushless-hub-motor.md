# Acceleration Control brushless hub-motor

### Replies: 9 Views: 2159

## \#1 Posted by: John12121 Posted at: 2016-02-21T17:30:59.390Z Reads: 102

```
Hey there! 

I have built a very short electric skateboard using a brushless hub-Motor with sensors a thumb-throttle and this Controller for the Speed-controll: http://de.aliexpress.com/item/Free-shopping-24V-250W-Brushless-DC-motor-controller-E-bike-speed-controller-for-lithium-battery/2027719724.html

My problem is, that because the skateboard is very short, it is very hard to stay on the board while accelerating. When I push the thumb throttle to one point, it accelerates quickly and then stays at the same Speed. So here's my question: Isn't it possible to Control the acceleration of the Motor through the thumb throttle instead of the Speed of the Motor? That would make it mouch easier to ride. 

I don't have any Knowledge in electronics, so sorry if thats a stupid question.

Thanks a lot in advance! Regards, John
```

---
## \#2 Posted by: John12121 Posted at: 2016-02-22T20:05:55.543Z Reads: 80

```
Can no one help? You would realy help me..
```

---
## \#3 Posted by: evoheyax Posted at: 2016-02-22T21:07:59.486Z Reads: 78

```
This problem can be solved in multiple ways.

The nyko wii controller by my understanding works the way you are describing.

A tradition controller works the same as a car would. You pres forward and you go forward, you let go and you coast. And when you press again, you have a small amount of pressing the pedal that does little to move you forward until you hit the spot where you accelerate again (In an automatic car, this is hard to notice, but much easier to see in a manual car).

The nyko wii controller has a cruise control function that at neutral, keeps you moving at the same speed, and when you press up, you accelerate. When you let go back to neutral, it stays at that new speed. When you go to slow down, you press back on the joy stick, and it decelerates. When you let go, it keeps going the same speed you were going when you let go (that's completely stopped if you let go after you completely stopped.

The issue with this controller is that its plagued with drop outs. I'm not sure how cross compatible it is also, and you do need to modify (i.e solder) the cables of the receiver, so this option is not for everyone.

I think some of what your feeling is also the problem of having a single drive system. You get a pull to one side while accelerating which wants to throw you off the board if you don't counter the pull by shifting your weight towards the side with the motor.Its not fatal, as I have use a single drive system for the last 6 months, but you do have to keep it in mind while riding or you will fall every now and then from it.

I can't speak to the quality of the speed controller or motor you are using. A lot of people use hobby grade parts, but that speed controller is 1/6 the cost of the cheapest esc I've seen others use on this forum, so some of the issues could be with the speed controller not having a good acceleration graph or other issues.

Also, there's no such thing as a stupid question. Most of us had no experience with this kind of stuff when we started, and ask many "stupid" questions. So don't feel bad, and keep striving for more information :)

Can you describe how short your board is also? Most normal trick skateboards are around 29" long, my eboard is 28" long, which is far short than most electric boards. I don't have Issues with instability due to shortness.

Other factors could include your trucks (are they regular skateboard trucks, longboard trucks, ect. they have different turn radius and geometry which affect stability), and the hardness of the bushings your using. The harder the bushing, the more stability you have. The downside you hard bushings is that you can turn less. But you need to find a  middle ground between super hard and super soft that is comfortable for you by trying different hardness of bushings.
```

---
## \#4 Posted by: lowGuido Posted at: 2016-02-23T09:21:58.043Z Reads: 65

```
so let me get this right? are you using a bike speed control for your board?
```

---
## \#5 Posted by: John12121 Posted at: 2016-02-23T22:25:34.337Z Reads: 61

```
@evoheyax: Thanks a lot for this Information! I think I will do some more Research based on our remarks. The pull to one side isn't too bad. The nyko wii Controller sounds interesting, but I couldn''t find it online.

@lowGuido: Actually yes, I do.
```

---
## \#6 Posted by: evoheyax Posted at: 2016-02-24T02:26:03.213Z Reads: 53

```
nyko controller can be found on amazon - http://www.amazon.com/Nyko-Wireless-Kama-Black-Nintendo-Wii/dp/B0047SFGDW/
```

---
## \#7 Posted by: claudiofiore88 Posted at: 2016-02-24T03:41:45.465Z Reads: 51

```
Wow! The price went up a lot. I think I paid like 10 bucks for mine.
```

---
## \#8 Posted by: evoheyax Posted at: 2016-02-24T03:44:33.823Z Reads: 49

```
You can get it cheaper other places with enough searching. This higher because its amazon prime, and it has become harder to find. Thus the reason I just ordered one to test with.
```

---
## \#9 Posted by: Namasaki Posted at: 2016-02-24T08:43:50.688Z Reads: 43

```
Hey John, I took a look at the speed controller your using and I'm thinking that it is the cause of the problems your having with uncontrolled acceleration. I recommend that you try a different speed control first.
There are some fairly inexpensive RC car speed controllers that work well in this application because they are programable using a simple programing card. 
Here is one in particular that I liked because you can download a free iphone app and program the esc from your iphone connected to the esc via an optional wifi module and If I'm not mistaken you can leave the wifi module connected to the esc all the time so that you can just pull over and make adjustments. 
and it will let you fine tune the throttle and braking curves.
http://www.rcjuice.com/toro-ts150-brushless-sensored-150a-esc/
There are also less expensive controllers than this one.
Just shop around for a ⅛ scale RC Car Esc  150 amp should be heavy duty enough.
```

---
