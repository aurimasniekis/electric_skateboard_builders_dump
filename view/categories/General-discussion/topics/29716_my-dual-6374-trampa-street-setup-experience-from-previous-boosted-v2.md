# My Dual 6374 Trampa Street Setup experience (from previous Boosted v2)

### Replies: 29 Views: 2250

## \#1 Posted by: pshaw Posted at: 2017-08-04T19:18:25.247Z Reads: 261

```
Well.... to start. It's fast. Like REALLY fast. This thing from a power perspective makes the v2 boosted board see like a joke. However there are some things that I miss about the Boosted board which are as follows....

1) Silent operation. These 6374 are super loud as I'm running them in BLDC hybrid mode (@Ackmaniac watt mode no reverse). From what many have said FOC mode is a gamble on 12S from a reliability perspective. 

2) Smoothness on acceleration. With the boosted board it was unbelieveably predictable. If you moved the thumbwheel 20% it would immediately jump up to speed and stay exactly that speed until you have it another input. In watt mode on this new board it is like the speed just keeps ramping up as you give it an input. Then you will be accelerating progressively then out of nowhere I guess you get into the area where the motor becomes really efficient and it rockets you forward. so hard and abrupt it is hard to stay on the board...
```

---
## \#2 Posted by: NickTheDude Posted at: 2017-08-04T19:40:52.606Z Reads: 254

```
Dual 6374s are just awesomely insane. If your VESCs can handle it you could probably set it up for 6000W which is 3x the power of a dual+. Personally I wouldn't gamble with FOC but I like the sound anyways so it's not a big deal.

For the smoothness I've heard that you can fine tune the acceleration curve with ackmaniacs firmware but I've never tried it so maybe someone else can chime in.

Also, post some pictures :stuck_out_tongue:
```

---
## \#3 Posted by: t0m_r1dd1e Posted at: 2017-08-04T19:56:18.800Z Reads: 241

```
Check out Ackmaniac's extended VESC firmware. It will let you set a throttle curve to be more sensitive at the lower end of input. Should help with your issue of holding speed constant.
```

---
## \#4 Posted by: pshaw Posted at: 2017-08-04T20:40:00.744Z Reads: 233

```
[quote="t0m_r1dd1e, post:3, topic:29716, full:true"]
Check out Ackmaniac's extended VESC firmware. It will let you set a throttle curve to be more sensitive at the lower end of input. Should help with your issue of holding speed constant.
[/quote]

Yeah but the problem is how do I determine exactly where I'm getting those non linear ramp ups? These places where the throttle curve has to be mellow will have to be very exact 

Best way I can' describe it is on my boosted car when you floor it everything is nice and linear then when full boost hits you jump a few hundred horsepower in just a tight RPM window..... so when that happens you have to VERY precisely lift throttle the perfect amount to continue moving forward without having a smokehsow .....
```

---
## \#5 Posted by: t0m_r1dd1e Posted at: 2017-08-04T20:53:47.101Z Reads: 219

```
Ohhhhh you're talking about when the motors hit their higher efficiency point I think. I have dual 6355's and I can feel that too but I've never tried to correct it. I imagine it's a bigger issue with your much larger motors. Yeah sorry, I don't have an answer to that one.
```

---
## \#6 Posted by: Jinra Posted at: 2017-08-04T21:05:49.688Z Reads: 212

```
watt control is still current control. This is just how the control mode works. You will always ramp up to full duty cycle if given current overcomes load. I wouldn't call it a downside of the mode, however, just a different way of accelerating. While Boosted's controller controls' speed, watt/current mode controls acceleration.
```

---
## \#7 Posted by: pshaw Posted at: 2017-08-04T21:45:36.401Z Reads: 210

```
Gotcha so there's is no getting around that really? I'm ok with adapting but this hard hit around 22mph is really brutal and uncontrollable even....[quote="Jinra, post:6, topic:29716, full:true"]
watt control is still current control. This is just how the control mode works. You will always ramp up to full duty cycle if given current overcomes load. I wouldn't call it a downside of the mode, however, just a different way of accelerating. While Boosted's controller controls' speed, watt/current mode controls acceleration.
[/quote]
```

---
## \#8 Posted by: trampa Posted at: 2017-08-04T21:47:04.390Z Reads: 208

```
The new VESC-Tool isn't far away and three different types of throttle curves will let you adjust the setup perfectly.
For FOC on a 4.xx hardware you want much lower KV. Personally I never had a single issue with FOC, using our low KV motors.  Welcome to the club of high performance beast board riders. I hope you like the Carver as much as I do.

Frank
```

---
## \#9 Posted by: Jinra Posted at: 2017-08-04T21:50:03.475Z Reads: 206

```
Build your foot muscles, and just keep riding, you'll eventually get used to it. Then you'll want even more speed.
```

---
## \#10 Posted by: Rob69de Posted at: 2017-08-04T21:59:19.682Z Reads: 198

```
I have a Kaly built urban Trampa with two ailen 6564 170kv runningAckmaniac's watt control on high torque settings in order to stay on the board i use ratchet strap bindings..
```

---
## \#11 Posted by: Ackmaniac Posted at: 2017-08-04T22:25:36.145Z Reads: 198

```
The kick you are talking about doesn't come from the control mode. It is noise on the current sensors at around 85% duty cycle. So the current reading isn't correct. Which Vesc Do you use? The Focbox for example improves that a lot. And it shouldn't exist anymore on the Vesc 6.
```

---
## \#12 Posted by: pshaw Posted at: 2017-08-05T00:30:58.567Z Reads: 189

```
[quote="Ackmaniac, post:11, topic:29716, full:true"]
The kick you are talking about doesn't come from the control mode. It is noise on the current sensors at around 85% duty cycle. So the current reading isn't correct. Which Vesc Do you use? The Focbox for example improves that a lot. And it shouldn't exist anymore on the Vesc 6.
[/quote]

Torque VESC
```

---
## \#13 Posted by: Ackmaniac Posted at: 2017-08-05T00:34:15.820Z Reads: 179

```
That's the standard VESC 4.12. Think it also depends on the motors and maybe also wire length and wire routing. But i could be wrong. On my single drive with a old 4.10 VESC it is very noticable. And the duals it is less. But maybe check if the outing of our phase wires makes a difference.
```

---
## \#14 Posted by: Aggdaddy Posted at: 2017-08-05T00:52:03.468Z Reads: 178

```
The "boost" feature/issue seems like it is vesc related.  I get it from vesc 4.12 and FOC box and from two different motors.  6355 / 190kv and a monster 300kv motor.   When I used a torqueboards 12s esc on the 6355, no turbo effect, just regular old v8 naturally aspirated speed.
```

---
## \#15 Posted by: pshaw Posted at: 2017-08-05T01:35:50.534Z Reads: 180

```
[quote="Aggdaddy, post:14, topic:29716"]
it
[/quote]

@Ackmaniac any chance there is a way to mitigate this? Can you set the board up to stay under 85% duty cycle so tmwould never hit the area that would induce the noise into the system?
```

---
## \#16 Posted by: pshaw Posted at: 2017-08-05T02:01:07.021Z Reads: 176

```
Also @trampa got any suggestions for setup to do high speeds? I'm 185lbs and have the 15ply street carver with the springs in the outer position on both front and back.
```

---
## \#17 Posted by: Namasaki Posted at: 2017-08-05T04:10:36.795Z Reads: 177

```
There is a thread by @Jinra on adjusting acceleration with the max current ramp step.
the default setting is .04. You can increase acceleration by increasing this value so I'm thinking that you could soften acceleration by lowering the value.
But before doing anything, please read about it here: 
http://www.electric-skateboard.builders/t/better-throttle-performance-through-more-responsive-ramping/29356
```

---
## \#18 Posted by: trampa Posted at: 2017-08-05T09:54:33.020Z Reads: 162

```
Ad Dampas in the back. If its still not perfect, ad Dampas in the front. "Speed" is very subjective.

Frank
```

---
## \#19 Posted by: pshaw Posted at: 2017-08-05T11:05:56.293Z Reads: 162

```
[quote="trampa, post:18, topic:29716, full:true"]
Ad Dampas in the back. If its still not perfect, ad Dampas in the front. "Speed" is very subjective.

Frank
[/quote]

How are the dampas different than just tightening the springs in the back?
```

---
## \#20 Posted by: trampa Posted at: 2017-08-05T12:23:23.409Z Reads: 159

```
The springs should always have pre-tension. 
Usually you wind in the adjuster till it sits flush with the deck. The Dampas are absorbing shocks and sudden movements. It's like in a car.

Frank
```

---
## \#21 Posted by: pshaw Posted at: 2017-08-05T14:27:34.167Z Reads: 149

```
[quote="trampa, post:20, topic:29716, full:true"]
The springs should always have pre-tension. 
Usually you wind in the adjuster till it sits flush with the deck. The Dampas are absorbing shocks and sudden movements. It's like in a car.

Frank
[/quote]

Very good to know. I had some pretension on the back but ZERO in the front. Hopefully once I get all 4 pre tensioned and put the dampas in the back it'll be even more stable at~30mph. 

Checked the @kaly motor mounts today after my first ride and to my disappointment they had both been broken free. Unfortunately these trucks make it nearly impossible to securely mount motor mounts. I had put the infinity trucks on a drill press and used an end mill bit to cut 4 "pads" as square as possible for the set screws to be able to bite on a flat surface. Followed the torquing pattern by the book as well per Kaly (inner finger side, outside opposite that, bottom, then finally the top side). Not sure where to go from here now.
```

---
## \#22 Posted by: trampa Posted at: 2017-08-05T14:51:38.657Z Reads: 137

```
We have zero issues with our mounts. Rock solid!
No milling needed + reversing the hanger is possible.

Frank
```

---
## \#23 Posted by: Kaly Posted at: 2017-08-05T15:06:46.360Z Reads: 134

```
Hi man 

Let's do this send me the hanger with the motor mount base attached and I'll send you a hanger with the mounts base properly installed. 

You have my address. 
This way you'll get it by Tuesday or Wednesday.
```

---
## \#24 Posted by: Kaly Posted at: 2017-08-05T15:10:24.456Z Reads: 131

```
And for the acceleration just change the USE MAX WATT value to 900. This will take the power until you can get use to it. 

Something to have in mind this is not boosted territory, a lot of power on this type of setup, we are not in Kansas anymore :wink:
```

---
## \#25 Posted by: pshaw Posted at: 2017-08-05T16:05:57.960Z Reads: 139

```
[quote="Kaly, post:23, topic:29716, full:true"]
Hi man 

Let's do this send me the hanger with the motor mount base attached and I'll send you a hanger with the mounts base properly installed. 

You have my address. 
This way you'll get it by Tuesday or Wednesday.
[/quote]

Damn dude that would be super helpful. I'm sure you guys know Kaly well around these forums but it is so damn refreshing to have such amazing support out there, especially when you are relatively new to all this. He got me everything expedited initially so that I could get this build together quickly, as well as helping me over the phone multiple times. 

Take DIY on the other hand... I order 2 antispark switches and both of them fail in the first use on two separate setups (which virtually eliminates anything weird/wrong on my end). I do some research and find a thread here where my exact isssue is happening to multiple people. The fets blow immediately which keeps the power essentially stuck open making the board impossible to turn off via power button. I contact them and they make me upload a video on a website to show the exact problem. I do that and then they request that I ship both units back on my own dime (despite just seeing my uploaded video of their faulty product mind you) for them to inspect them. So their customer service puts me out a week or more on my build, costs me more money to ship, all for getting replacements which will more than likely fail as well. 

Sorry for the rant... I just realize this is a very small community, so in industries such as this where there isn't much competition it can be easy to not have to go the extra mile (or hell even just do what is right haha). This makes it even that much more pleasant that there are people out there like Kaly that are just super psyched to get people up and riding. 

Can't wait to get this thing sorted out. I'm already crazy addicted to the power!
```

---
## \#26 Posted by: pshaw Posted at: 2017-08-05T20:39:07.703Z Reads: 121

```
@trampa just curious how your motor mounts are fixed? Seems that it is inevitable to have to use a set screw on the 2 curved surfaces no?
```

---
## \#27 Posted by: trampa Posted at: 2017-08-05T21:24:01.698Z Reads: 123

```
They use specially shaped M8 flat spotted, rotatable ball tip stainless set screws in combination with a 12mm thick bracket from 6061T6 alloy. The screws are made to our specification by a German precision manufacturer.

http://www.trampaboards.com/m8-x-16mm-grub-screw-mgst-shape-b-with-flat-ball--connects-street-urban--mountaniboard-mounts-to-hangers-35-p-12956.html

Frank
```

---
## \#28 Posted by: pshaw Posted at: 2017-08-07T14:43:31.869Z Reads: 115

```
So a little update: I realized that I might not have max watts limit box checked and set. According to my friend he thinks that this means I won't actually be in watts mode, but current mode. 

If this is true this explains A TON. haha

Update update: apparently watt mode was still active (@jinra confirmed) but with no limit. I checked and the settings weren't identical between the two escs and I had zero throttle curve (I thought I saved it but must've not hit write).

The board is now smooth as can be. @Ackmaniac sorry man! Your software is freaking smooth as butter. Just have to have the right settings ... and more importantly the same settings if you have multiple escs lmao.....

Update update update lol: I spoke too soon once again. The turbo boost happens where there is noise on the current sensor at the higher end of duty cycle. So I know there is a way to limit duty cycle... but if I do that I'm limiting top speed correct?
```

---
## \#29 Posted by: Darby Posted at: 2017-08-21T17:34:00.775Z Reads: 86

```
Yup Kaly is the best.. and I made the DIY antispark switch mistake too... DO NOT BUY from DIY.
```

---
