# Vesc options in plain english?

### Replies: 16 Views: 349

## \#1 Posted by: Jcammarata4 Posted at: 2019-05-17T14:58:45.954Z Reads: 146

```
has anyone ever took the time to decrypt the difficult vesc settings terms and made an easy to understand guide or translation.......for example:
Battery min= braking
motor min=brake force at low speed

this to me seems like it would be extremely helpful for people that are new to programming their boards.....the vesc tool is great but it is scary and very daunting to someone not used to using it.....let me know if anyone has a list like this or maybe we can just kinda put one together with input from anyone willing
```

---
## \#2 Posted by: Jcammarata4 Posted at: 2019-05-17T15:04:06.685Z Reads: 142

```
 the help buttons in vesc tool explain the settings but theyre still tough to understand to the average idiot like myself. i think a vesc for dummies translation sheet may be very helpful and cut down on the nonsense and amount of questions we all have
```

---
## \#3 Posted by: Wilsonliang777 Posted at: 2019-05-17T15:06:52.683Z Reads: 132

```
I think there is a few video on YouTube that explain some of the major settings.   Like your I don't understand like 75% of the settings therefore I don't touch what I don't understand.
```

---
## \#4 Posted by: Jcammarata4 Posted at: 2019-05-17T15:13:15.816Z Reads: 124

```
exactly ....i watched any vid i coud find most are ok but very specific or basic....if the vesc tool had a companion sheet maybe that we compiled thats in simple basic terms ..we would all be in a better smarter position.   i know i would greatly appreciate being able to understand the technical terms used to set these motors....
people must understand what im saying right?? or am i wrong and just not doing enough .....i dont want a electrical degree...just the ability to easily set my motors to the proper settings without consulting the pope daily
```

---
## \#5 Posted by: Jinra Posted at: 2019-05-17T15:14:46.484Z Reads: 116

```
If you have a Unity the Focbox UI or app is a simplified version of the vesc-tool. You still have to understand motor max/min battery max/min, but that's about it.

I wouldn't start equating battery min to braking even though it directly affects it because some people may want more braking and set it absurdly high and end up blowing up their boards.
```

---
## \#6 Posted by: Excess Posted at: 2019-05-17T15:30:07.946Z Reads: 111

```
Download the ackmaniac bldc tool and if you hover your cursor over the settings you get “tool tips” like these. 
![image|375x500](upload://cT90Nf7NRTu5YDVuAvIis31fmFv.jpeg) ![image|374x500](upload://funZEnoyl7vpdidf7MajfUfdRB1.jpeg) 

I hope that helps. 
It helped me. 
Good luck
```

---
## \#7 Posted by: Jcammarata4 Posted at: 2019-05-17T15:41:27.264Z Reads: 97

```
i do have that version. my problem with that is when you use that version ..the  ack version....i was told that it gave me some issues with firmware versions not being correct..like it gave me a firmware version of 3.103....which trampa explained isnt a real firmware number and is a problem ...but then i also heard that that version was made for boarding specifically versus all types of uses(drones planes)....so much info...not alot of uniform answers makes this tedious...i guess trial and error is ok for learning but dont want to burn the components out from trying to learn about it.
```

---
## \#8 Posted by: Jcammarata4 Posted at: 2019-05-17T15:41:48.181Z Reads: 96

```
thanks for the help
```

---
## \#9 Posted by: Excess Posted at: 2019-05-17T15:43:44.164Z Reads: 91

```
You don’t have to use the ack version to program if you’re not comfortable with it, you can just have it downloaded as a reference for simpler explanations of the settings.
```

---
## \#10 Posted by: Jinra Posted at: 2019-05-17T15:44:01.130Z Reads: 91

```
[quote="Jcammarata4, post:7, topic:94150"]
like it gave me a firmware version of 3.103…which trampa explained isnt a real firmware number and is a problem
[/quote]

3.103 is the custom firmware @Ackmaniac created. Don't listen to Trampa, he's just plain wrong..
```

---
## \#11 Posted by: trampa Posted at: 2019-05-17T15:53:55.565Z Reads: 89

```
[quote="Jcammarata4, post:7, topic:94150"]
but then i also heard that that version was made for boarding specifically versus all types of uses
[/quote]

The VESC FW is perfect for boarding, but you can also use it for many other applications. 
Motor max, Motor min, Battery max, Battery min is something you need to understand, since these values interact with another. 

Read this and you will understand it:
https://www.electric-skateboard.builders/t/vesc-6-cooling-and-max-current/61944/9?u=trampa

@Jinra : If you don't know what the issues was, don't post. @Jcammarata4 had FW problems and I helped him to sort it. The latest VESC-Tool has that new SWD Prog feature to rescue VESCs with messed up FW.
```

---
## \#12 Posted by: Jinra Posted at: 2019-05-17T15:59:34.948Z Reads: 80

```
3.103 is not a firmware issue lol. He didn't have an "issue" on this thread, he simply asked for tool tips.
```

---
## \#13 Posted by: Jcammarata4 Posted at: 2019-05-18T15:35:42.302Z Reads: 55

```
well thank you all for your input. not sure exactly what did it but reset vescs last night and today... just took a beautiful ride and all seems to be dialed in and working like it should. the sensorless 6374 149kv motors now take off from a standstill with little to 0 cog and have much more torque plus surprisingly i think my mileage has improved a little bit overall vs my older motors. thanks to all esp. scramboards for trying to charge me 140.00 per motor.
```

---
## \#14 Posted by: mmaner Posted at: 2019-05-18T15:46:52.384Z Reads: 52

```
[quote="Jcammarata4, post:7, topic:94150"]
trampa explained isnt a real firmware number and is a problem
[/quote]

Trampa thinks anything that isn't Trampa is a problem, just ignore it. Use Acks 2.54 and downngrade the firmware to 2.54. It's a simpler learning process
```

---
## \#15 Posted by: mmaner Posted at: 2019-05-18T15:49:09.337Z Reads: 51

```
[quote="trampa, post:11, topic:94150"]
@Jinra : If you don’t know what the issues was, don’t post.
[/quote]

To be clear, you have no authority here. You are a user just like everyone else. So stop giving order as if you have some authority.  Thank you
```

---
## \#16 Posted by: Gamer43 Posted at: 2019-05-18T20:23:59.306Z Reads: 32

```
Hey, just thought I would provide some input to help explain the settings. 

Motor current settings set torque limits, and also determine how hot the motors and ESCs will get under high throttle. Higher settings result in higher torque and higher temperatures. 

Battery current settings set the maximum power output of the ESC and motor, and determine how hot the battery pack and any antispark switches will get. Care must be taken not to exceed maximum charge and discharge ratings of the battery pack. 

Battery current will always be less than motor current, with the relationship being roughly proportional to speed. I.e. more speed means more battery current for the same motor current.

At higher speeds, battery current will start to throttle maximum motor current, resulting in less motor current at the same input level, and thus less torque. If torque seems to pick up as your board speeds up from low speed, that has to do with the control algorithm's performance at different speeds.

Battery soft cutoff voltage will throttle battery current, and by extension motor current, as the battery voltage starts to drop below the threshold.

Hope this helps!
```

---
