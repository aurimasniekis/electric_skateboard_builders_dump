# Removing FVT 120A ESC Fan?

### Replies: 24 Views: 3220

## \#2 Posted by: lowGuido Posted at: 2016-02-13T19:29:28.334Z Reads: 164

```
[quote="Mathieu, post:1, topic:1346"]
anyone used the EZRUN without a fan? I plan on integrating it in the enclosure with the heatsink mounted to the outside, it would work i guess?
[/quote]

I have used the HK150A for over a year without a fan with no issues. I think it is similar to the EZrun, should be fine
```

---
## \#3 Posted by: Mathieu Posted at: 2016-02-13T19:32:21.405Z Reads: 162

```
I think they're similar as well!
```

---
## \#1 Posted by: FlimFlamPhlegm Posted at: 2016-02-16T23:39:28.958Z Reads: 120

```
Hi there,

I put together my basic build, and it functions! Thanks for all your help!

However, I was wondering if it is possible to remove the fan on the FVT esc, as it is a bit too loud for my liking. If I just left a hole for the heatsink so air could circulate as I rode and removed the fan, would this prevent overheating?

Thanks!
```

---
## \#4 Posted by: FlimFlamPhlegm Posted at: 2016-02-17T00:31:08.179Z Reads: 112

```
I just tested it
After 10 minutes it's kinda warm is that ok? 
I just turned the board upside down and did random accel/brake
```

---
## \#5 Posted by: FlimFlamPhlegm Posted at: 2016-02-17T03:13:20.873Z Reads: 103

```
Never mind after riding it the motor had a bunch of cogging, heated up a lot and the fvt was burning to the touch, probably just gonna deal with the fan noise 

Do you think I can solve the cogging by reprogramming?
```

---
## \#6 Posted by: barajabali Posted at: 2016-02-17T04:29:43.921Z Reads: 102

```
@FlimFlamPhlegm  I ran 2 fvt 120 amp with no fans for 20 mile trips and it wouldnt heat up at all.  Just keep them in an area with alot of air flow!. and keep the heat sinks on
```

---
## \#7 Posted by: FlimFlamPhlegm Posted at: 2016-02-17T04:31:39.951Z Reads: 100

```
Maybe it's because it keeps cogging on startup? Would that be the problem?

I just tried it out again, and the urethane wheels had a burnout or something and now the house smells like plastic. The motor and ESC were all searing hot and the wires were warm. Is it just because of the large current draw caused by cogging?

If so, would reprogramming fix this? Im using 6s with a single hub carvon v2.
```

---
## \#8 Posted by: barajabali Posted at: 2016-02-17T04:35:13.031Z Reads: 100

```
no the cogging shouldnt have anything to do with it because when you first start up, whether the fan is on or not, it is at room temp.  

You might have a short or wires connected wrong.  Please upload pictures and exactly what kind of motors and battery youre using. 

Also how did you diconnect the fan? did you formally open the esc and un plug it? or just jam something in the fan blade?  (sometimes people do that lol)

Also when i used to have 270kv motos on that esc. when i pushed the throttle all the way down right away, the motors would cog up big time, i had to accelerate gradually (which is how you would accelerate when driving anyway) is this what youre talking about maybe?
```

---
## \#9 Posted by: FlimFlamPhlegm Posted at: 2016-02-17T04:40:03.323Z Reads: 98

```
<img src="/uploads/db1493/original/2X/5/5e46e44529a59d17fbac97d393c4d8e4eb72468f.png" width="690" height="358">

And yeah I unplugged the fan ( i did it too hard and broke the pins off, no shorts in the fan connector)

I also tried just going really slowly but it still cogged, even when i went really slowly on the acceleration
```

---
## \#10 Posted by: barajabali Posted at: 2016-02-17T04:42:12.247Z Reads: 95

```
it would really help if you posted a short video of it.  Im pretty good with these esc's if its a common issue i may be able to help
```

---
## \#11 Posted by: barajabali Posted at: 2016-02-17T04:43:36.192Z Reads: 93

```
also, depending on which wiiceiver youre using, it might be the problem.  try the system on a reguar 2.4 ghtz controller so eliminate any chance of it being a connection issue.
```

---
## \#12 Posted by: FlimFlamPhlegm Posted at: 2016-02-17T04:45:58.626Z Reads: 96

```
<img src="/uploads/db1493/original/2X/c/c8b19bfc574009e0bbadf41756cf49655073b696.jpg" width="675" height="500"><img src="/uploads/db1493/original/2X/8/8024dcf17d2339be2ac09fcdeda10410e923957e.jpg" width="675" height="500"><img src="/uploads/db1493/original/2X/a/a4d6a9294737a24f14c5c2f1c3f0cca39286e0c8.jpg" width="675" height="500">

I am using the newest wiiciever batch, 2.0B3
A video is probably going to have to wait until tomorrow, I left it in the washroom with the air extractor on to get rid of the smell.
```

---
## \#13 Posted by: barajabali Posted at: 2016-02-17T04:50:59.470Z Reads: 90

```
Okay you're not running sensors right? 

Do you have a pic of the motor?

Does the motor have bullet connectors soldered on?
```

---
## \#14 Posted by: FlimFlamPhlegm Posted at: 2016-02-17T04:51:47.234Z Reads: 89

```
the motor is the silver thing sticking out of the purple wheel in the 1st pic (it's a hub motor)
the motor is sensorless, and the bullet connectors are soldered and heatshrinked,
```

---
## \#15 Posted by: barajabali Posted at: 2016-02-17T04:53:15.659Z Reads: 88

```
Oh I'm sorry I didn't see the first pic as I'm on my phone! 


And hmm okay yea it all looks good... We'll have to wait for a video and/or trying with a different receiver (just in case) I had wiiceivers that were good in theory but terrible in practice
```

---
## \#16 Posted by: FlimFlamPhlegm Posted at: 2016-02-17T05:47:36.758Z Reads: 85

```
Aight yeah thanks for all the help so far! 

I'll try to get a video up tomorrow
```

---
## \#17 Posted by: lowGuido Posted at: 2016-02-17T07:57:12.450Z Reads: 80

```
Solder that dongle onto the wiiceiver while you are at it.

So yoy are using single motor? Maybe a 150A would have been better. Maybe 120A for dual motors without a fan.
I definitely dont get too warm with my 150A no fan. Even on hot days.
```

---
## \#18 Posted by: FlimFlamPhlegm Posted at: 2016-02-17T08:15:31.896Z Reads: 82

```
Yes I am using a single motor, could the heat be due to the 120A not being able to handle the amp draw? 
I'm planning to get a programmer to remove backwards cause I can't brake right now, going to see if tweaking timings and such helps with it. 

How would I go about soldering the dongle on? Do I have to take off the plastic housing?
```

---
## \#19 Posted by: lowGuido Posted at: 2016-02-17T10:30:22.579Z Reads: 77

```
yup you take it out of the housing and solder the wires directly.
otherwise you may die.
you have been warned.
```

---
## \#20 Posted by: barajabali Posted at: 2016-02-17T14:09:22.263Z Reads: 77

```
i have an extra programing card i can give you for cheaper than wherever you can buy it
```

---
## \#21 Posted by: barajabali Posted at: 2016-02-17T14:11:13.376Z Reads: 69

```
whats a dongle? the wii remote receiving block?
```

---
## \#22 Posted by: FlimFlamPhlegm Posted at: 2016-02-17T16:20:55.019Z Reads: 71

```
Yep the receiver from the nyko nunchuck

Could you ship to canada?
```

---
## \#23 Posted by: barajabali Posted at: 2016-02-17T16:34:44.216Z Reads: 73

```
I dont see why not. Ill just give it to you for free.  just pay for shipping. PM me your address and ill see how much shipping is.
```

---
## \#24 Posted by: FlimFlamPhlegm Posted at: 2016-02-17T20:12:12.868Z Reads: 69

```
Wow thanks so much! Hit you up with a PM
```

---
