# To ESC or not to ESC. That is the question&hellip; (A freakin annoying one)

### Replies: 20 Views: 1709

## \#1 Posted by: CalinStalin Posted at: 2016-10-21T00:05:47.120Z Reads: 335

```
Ok, is it true that the reliabilty of escs are highter to that of a vesc's? I've been trying to decide for ages now and I just can't make my mind up. If I buy a vesc, I know there's a good chance I'll short it within the first 5 mins of unpacking it. There's also the fact that I live in the UK and I can't find a reliable dealer for a good quality vesc.

With the ESCs, I've found two options. 

http://www.hobbyking.com/hobbyking/store/__106585__HobbyKing_Red_Brick_125A_ESC_Opto_Ver_2_0_UK_Warehouse_.html?strSearch=Red%20brick

http://www.hobbyking.com/hobbyking/store/__74073__Turnigy_Marine_120A_BEC_Waterproof_Speed_Controller_with_Water_Cooling.html

I really like the simplicity of them and the fact that I don't need to configure anything. Apparently, they're less prone to shorting than vescs. However, I've heard that braking is just plain awful.

I'd really appreciate some help deciding because this is starting to do my nut in (:
```

---
## \#2 Posted by: Jinra Posted at: 2016-10-21T00:09:00.903Z Reads: 319

```
The VESC is generally regarded as more reliable, but not idiot-proof. Regular ESCs are simple and easy to use, but lack in customization and options. If you know what you're doing with a VESC, you'll likely be much happier with it.
```

---
## \#3 Posted by: saul Posted at: 2016-10-21T00:17:07.700Z Reads: 304

```
most issues with shorting vesc were from early batches...slightly longer wires and heatshrink are mostly standard from the popular suppliers...

you could always try the vescx it seems a bit more friendly with the case.


vesc have much better brakes and failsafes. and allows custom limits!
```

---
## \#4 Posted by: Namasaki Posted at: 2016-10-21T06:33:28.654Z Reads: 270

```
I also was afraid to try the vesc at first because of all the horror stories.
I used car esc's for months. And thought, there good enough, even though I had to constantly deal with jerky acceleration  and unpredictable and often grabby brakes.
The Vesc has adjustable brakes that are always linear, smooth and predictable. Acceleration is also linear and smooth.
When I found out that the vesc delivers full voltage to the motor at all speeds and regulates current flow unlike car esc's that only regulate voltage so that you have to go full throttle to get full efficiency. Where the Vesc is efficient at all speeds.
I just had to try it. So I bought 2 Vescs with heat sinks from Chaka (the best that money could buy at that time) and I am so glad I made the jump. There performance is way beyond my expectations. Iv'e been using them for several months now with no issues at all. I ride fast and I do a lot of hill climbing. I have not had any problem with overheating or the vesc shutting down.  All of the main Vesc vendors are now realizing that the original vesc needed improvement and they are stepping up. Chaka was the first to address this and to sell a quality reliable vesc.
Believe me, If you get a quality Vesc, you will not regret it. 
Just stay with a safe erpm range like 190kv with 10s voltage and stick with BLDC.  FOC is a gamble. I run BLDC, I would not even try to run FOC.
I use quality precision motors from Alien Power And have my Vescs inside a sealed enclosure and its quiet enough.
Even if my Vesc failed, I could not go back to using a car esc. I would have to buy another vesc. There just 100 times better than even the most expensive car esc.
```

---
## \#5 Posted by: CalinStalin Posted at: 2016-10-21T10:05:36.624Z Reads: 243

```
Thanks from that, i guess I'm going with the vesc then! Would you recommend a reliable  UK dealer? I looked at www.vesc.co.uk who have a couple good reviews.
```

---
## \#6 Posted by: Namasaki Posted at: 2016-10-21T12:33:04.485Z Reads: 226

```
It looks like there's doesn't come assembled or programmed. And they did not mention having important and nesesary upgrades. 
I would recommend goaxle.com 
Or ollinboards
There's have upgrades and come assembled, programmed and tested with a warranty.
```

---
## \#8 Posted by: Namasaki Posted at: 2016-10-21T15:38:21.531Z Reads: 201

```
Took me a while and a lot of arguments before I could get my head around the concept but the Vesc is completely different. 
Where a normal Esc adjusts voltage via throttle and current is determined by the amount of load applied. 
The Vesc delivers constant full voltage and adjusts current via the throttle. "Current Control"
```

---
## \#10 Posted by: Namasaki Posted at: 2016-10-21T16:50:09.131Z Reads: 181

```
I am very familiar with ohms law. 
P=I E
It is my understanding that the Vesc delivers full voltage as soon as you press the throttle which is evident when bench testing as the motor or motors spin up to full rpm as soon as you press the throttle and that rpm stays constant regardless of how much throttle is applied. 
Where with a regular esc, the rpm varies depending on the amount of throttle applied. 
I will however, run some test later with a voltage meter on the phase output of the Vesc to prove wether this theory is correct or not. 
I'll post the answer here as soon as I have it.
```

---
## \#12 Posted by: Namasaki Posted at: 2016-10-21T17:43:57.407Z Reads: 164

```
P= I E
The product is power in watts. 
40v x 10a = 400w
10v x 40a = 400 w
if you need 400w power to handle a load. 
You can do it with high voltage and low amps 
or low voltage and high amps.
If you raise the voltage to a motor under a given load, the current goes down not up. 
I have proven that with real life tests.
Oh, and there is no V in ohms law. 
Ohms law: I=E/R  the formula you posted I don't know how you came up with that. 
I= current
E= voltage
R= resistance 
P=power
```

---
## \#15 Posted by: Namasaki Posted at: 2016-10-21T18:07:21.625Z Reads: 153

```
I learned ohms law in 1969
P=IE was part of ohms law. 
I=E/R 
This is how it was taught in 1969
Of coarse, that was way before your time
```

---
## \#17 Posted by: Jinra Posted at: 2016-10-21T18:13:50.088Z Reads: 148

```
[quote="IDVert3X, post:16, topic:11593"]
higher the voltage, the higher the current,
[/quote]

With less load, you run full voltage with low current, so I'm not sure why you're saying higher voltage = higher current. If you have a lot of load, it's then you'll pull higher amps. I think back EMF has a part to play in this that you're not considering.
```

---
## \#19 Posted by: Jinra Posted at: 2016-10-21T18:27:21.032Z Reads: 146

```
I feel like you're being needlessly aggressive toward @Namasaki. For all intents and purposes, you can consider the VESC to be running full input voltage when running current control mode. The motor will always run at the input voltage given it has enough current to overcome load.
```

---
## \#21 Posted by: Namasaki Posted at: 2016-10-21T18:37:17.116Z Reads: 143

```
When you reach your current limit with the Vesc, you just don't go any faster. And if the load increases like going up hill, you'll slow down.
```

---
## \#25 Posted by: CalinStalin Posted at: 2016-10-21T21:12:38.119Z Reads: 141

```
Lol, you guys basically just hijacked this post... xD
```

---
## \#26 Posted by: CalinStalin Posted at: 2016-10-21T21:24:36.509Z Reads: 135

```
"There's also the fact that i live in the U̲K̲" Those dealers are not UK based...
  Also, may i point out that the vesc on www.vesc.co.uk has a drop down menu with the premium option for the vesc      which comes with all cables attached and ready to go. It even has a nice wooden box for it! (:

Thanks anyway,
Cal
```

---
## \#27 Posted by: Namasaki Posted at: 2016-10-21T21:56:01.102Z Reads: 130

```
Sorry your thread got hijacked. But I don't think that was my fault. I tried to answer your question  when that guy who is by the way a newbie on this forum, jumped in and hijacked your thread to try to show off how smart he thinks he  is.
And I didn't notice the drop down menu on that website.
Btw, This is a little off topic but I have been to Sussex Downs south of London. Such a beautiful place to esk8
```

---
## \#28 Posted by: CalinStalin Posted at: 2016-10-21T22:00:43.254Z Reads: 126

```
To be honest, i didn't understand a word you two were going on about xD. Probably because i'm still in high school and i didn't take physics...
```

---
## \#29 Posted by: IDVert3X Posted at: 2016-10-21T22:14:28.657Z Reads: 123

```
@CalinStalin 
Sorry about that,
we were talking about electrical-engineering related side of the thing, nothing you really need to know.
Again, sorry, I shoul've really talked about it in the PM.

I deleted my posts as they really shouldn't be there, they will disappear after 24 hours.
If Namasaki will do the same it's up on him.

@Namasaki
 > to try to show off how smart he thinks he is.

This is just your opinion, that's really not what I'm trying to do.
I just wanted to explain that what you said is wrong ( partially ) and why.
I've never planned it to end up like so ( many posts me trying to explain you something ).
```

---
## \#30 Posted by: DIY4Life Posted at: 2016-12-09T12:46:46.733Z Reads: 102

```
Guys,
Could some-one please help me out for a sec.

I have this ESC laying around, its a badass ESC, super solid and reliable
http://rctimer.com/download/HW-SM013_PL100A-HV-en.pdf

And i would like to use it as an eboard ESC.
But it actually isnt a car ESC(brake mode and stuff included) , but a HELI ESC... with flight modes

First i thought i wasnt able to use it, and have to buy a new one :-(, but when reading the manual, 
i can set it to have a brake mode?? Correct?

And i can set the flight mode as 'HELI GOVERNOR OFF' and then it will have a straight throttle curve (check the throtthle curves in the manual please...), this is what an eboard ESC would offer me to right??
Or wil it just have a forward and reverse with that curve? 

is setting forward and brake mode possible? (no reverse, straight throttle line,...)
Please help me out, i know a lot about building and electricity but nothing about programming ESC's.
```

---
## \#31 Posted by: Namasaki Posted at: 2017-05-07T04:41:19.961Z Reads: 65

```
I had completely forgotten about this thread until today when I got a like notice.
Now that I read some of my posts I'm am totally shocked and ashamed for being such a rude jerk.
I would delete my posts now if I could. That option is no longer available so all I can do now is apologize.
to @IDVert3X @CalinStalin @saul @DIY4Life @Jinra  and anyone else who reads this thread.     
Because disrespecting others is unacceptable regardless of who's wright or wrong.
```

---
