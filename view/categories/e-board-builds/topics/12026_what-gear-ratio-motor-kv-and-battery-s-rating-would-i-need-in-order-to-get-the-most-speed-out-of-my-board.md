# What gear ratio, motor KV and battery &lsquo;S&rsquo; rating would i need in order to get the most speed out of my board?

### Replies: 30 Views: 2225

## \#1 Posted by: CalinStalin Posted at: 2016-10-27T21:14:30.524Z Reads: 188

```
I'm currently in the process of gathering parts for my build and i've practically got everything i need. However, there's one thing that's bothering me, and that's the speed of a single drive board. I've been browsing YouTube looking at various speed tests but in my opinion it doesn't look like they're actually going at a decent speed. It may just be the camera angle that messes with the perspective but i want to be absolutely sure that what i'm buying is going to work how i want it to work. So here's the question, what would the specs of my motor, gear ratio, battery etc have to be in order to go at almost double the speed of the board in this video: https://www.youtube.com/watch?v=m3ySmFGMGzw without having to go with dual motors? Is it possible? I currently have decided to go with an 192kv Turnigy SK3 motor and two 5s lipos in series which from what i've read seems to be the best i can get. I might have missed something.
```

---
## \#2 Posted by: ArmandR Posted at: 2016-10-27T22:18:30.129Z Reads: 181

```
12s lipo, 280 kv, 12s ESC, 107 mm, 16/36 gearing. That will probably get you extremely fast speeds.
http://calc.esk8.it/

You could use a different gearing to get even more speed. But you will have barely any torque, i would not recommend this for an offroad build.
```

---
## \#3 Posted by: CalinStalin Posted at: 2016-10-27T22:34:55.903Z Reads: 170

```
Why do you need torque when you have speed? For example, if I saw a hill about 200meters in front of me couldn't I just accelerate to a speed that will gather enough momentum to get me up the hill?
```

---
## \#4 Posted by: CalinStalin Posted at: 2016-10-27T22:35:43.448Z Reads: 154

```
Also, wouldn't this setup fry my ESC?
```

---
## \#5 Posted by: ArmandR Posted at: 2016-10-27T22:36:36.172Z Reads: 155

```
Well not always, if you do not have enough speed or torque the motors might not even have the capability to take you up a hill. Torque is also important in acceleration. Without torque your acceleration will be slower. With the setup I gave you should go faster then you will ever want.
```

---
## \#6 Posted by: CalinStalin Posted at: 2016-10-27T22:45:38.592Z Reads: 147

```
So would you say that the setup I have currently (190kv, 10s, etc) is a good combination of torque and speed?
```

---
## \#7 Posted by: Jinra Posted at: 2016-10-27T22:48:05.971Z Reads: 154

```
[quote="CalinStalin, post:3, topic:12026"]
if I saw a hill about 200meters in front of me couldn't I just accelerate to a speed that will gather enough momentum to get me up the hill?
[/quote]

If you have inadequate torque, you'll eventually slow down and overheat your motors, if not kill them. You also might have a hard time accelerating at a decent rate after lights and stop signs. Keep in mind the amount of current required increases exponentially as you go faster. You should aim for 30-35mph tops if you want speed to be efficient. 97mm wheels + 200kv motor + 10s + 16/36 will get you near 35mph.

[quote="CalinStalin, post:6, topic:12026, full:true"]
So would you say that the setup I have currently (190kv, 10s, etc) is a good combination of torque and speed?
[/quote]

190kv 10s is pretty much a gold standard in esk8 ;)
```

---
## \#8 Posted by: ArmandR Posted at: 2016-10-27T22:55:30.563Z Reads: 143

```
Yes, probably one of the most successful setups.
```

---
## \#9 Posted by: caustin Posted at: 2016-10-27T22:55:38.964Z Reads: 145

```
Would fry your VESC not ESC, like TB 120A Opto esc
```

---
## \#10 Posted by: caustin Posted at: 2016-10-27T23:00:35.570Z Reads: 142

```
@ArmandR and @Jinra both right. One to optimize speed exclusively, i.e. Overly at cost of torque. The other plenty of speed and better torque trade off. You can always tweak the pulleys gearing ratio, wheel size, battery spec, rider weight (harder lol) to increase speed or torque or whatever but best practice to start with proven build foundation like @Jinra specifies!
```

---
## \#11 Posted by: CalinStalin Posted at: 2016-10-27T23:20:27.146Z Reads: 137

```
And I take it if I had 7 inch mountain board wheels I would get as much speed if not more?
```

---
## \#12 Posted by: caustin Posted at: 2016-10-27T23:23:36.012Z Reads: 133

```
You would think so, but no. Shift to pneummies changes the equation.
```

---
## \#13 Posted by: CalinStalin Posted at: 2016-10-27T23:25:07.727Z Reads: 131

```
What would the equation be? I should have probably made it clear that I'm building a mountain board (for mainly flat canal paths)
```

---
## \#14 Posted by: Jinra Posted at: 2016-10-27T23:29:48.124Z Reads: 127

```
you'll want a bigger pulley for pneumatics which will decrease top speed given the same settings in other places. For example, Evolte GT uses 66T pulleys on pneumatics I believe.
```

---
## \#15 Posted by: caustin Posted at: 2016-10-27T23:30:39.571Z Reads: 123

```
There is a separate thread on this. Search forum, and ask @Kaly @psychotiller @trampa etc.

(Edit). Actually remembering that thread was more about "why is my pneummie battrery consumption 2x my uro?" Lol
```

---
## \#16 Posted by: caustin Posted at: 2016-10-27T23:31:54.860Z Reads: 121

```
Correct sir, resulting in serious gearing ratio given same motor pulley!!
```

---
## \#17 Posted by: CalinStalin Posted at: 2016-10-27T23:33:28.140Z Reads: 123

```
66T for both motor and wheel pully?!
```

---
## \#18 Posted by: Jinra Posted at: 2016-10-27T23:33:52.104Z Reads: 121

```
no 15T for motor on the GT
```

---
## \#19 Posted by: CalinStalin Posted at: 2016-10-27T23:35:33.185Z Reads: 127

```
Yet the evolve gt goes much faster compared to the speed of the board in the video I linked!
```

---
## \#20 Posted by: psychotiller Posted at: 2016-10-27T23:38:45.320Z Reads: 126

```
Current build I'm working on has 6" pneumatics, 16/60 gearing, 170kv motors, 10s and vescs running sensored FOC. Super torquey. Top speed is around 25mph. My wheels can easily change to 42t pulleys which will net 35mph, but torque will suffer a little.
<img src="/uploads/db1493/original/3X/9/6/961df3db467849987b8265408337e5f7cbab0684.jpeg" width="690" height="389">
```

---
## \#21 Posted by: Jinra Posted at: 2016-10-27T23:38:48.649Z Reads: 112

```
Depends on a large number of factors, though the GT with AT wheels only go 22mph I think, not too fast.
```

---
## \#22 Posted by: caustin Posted at: 2016-10-27T23:42:49.521Z Reads: 106

```
Yes I have GT and tried all wheel sizes uro and pneummie. EXCEPT @psychtiller best of the best famous billet wheels.  Which he is sending me now though I picked the 60T gearing to start with!! 

Mountain board?  Me thinks torque over flat level ground speed anyway lol.
```

---
## \#23 Posted by: Photorph Posted at: 2016-10-28T01:59:15.291Z Reads: 102

```
You can always just get dual hub motors with 12s and 97mm fly wheels, the carvon V2 were 149 kv...would get some serious speed with that set up.  Or the 116 kv V3 that are still to be released.
```

---
## \#24 Posted by: Kaly Posted at: 2016-10-28T02:44:48.114Z Reads: 102

```
@CalinStalin
For speed and usable toque you'll need to go to 12S or minimum to 10S with a high discharge battery preferably A123 or lipo and use a TB120A ESC. (The VESC in its current iteration is no good for eMTB). Then Gear it to 16/65 or 18/65 using 8 in wheels and we are talking about 30-35 Mph with torque to tackle any circumstances.  

This set up have work incredibly well for me and I weight 208 lb at 6'2".

The setups with batteries less than 10S you'll have to compromise either in speed or torque and don't have the dirt bike feeling that I really love about eMTB. 

Good luck with your built :-)
```

---
## \#25 Posted by: caustin Posted at: 2016-10-28T02:46:49.204Z Reads: 100

```
@kaly advice is gospel!
```

---
## \#26 Posted by: psychotiller Posted at: 2016-10-28T03:22:45.015Z Reads: 99

```
Here's a video of 10s, sensored FOC and 16/42 with 170kv 6355's on 6" billet Pneumatics.
GPS on this was 30mph. @mccloed  has the screen shot.

https://www.facebook.com/SiLo.socal.e.longboard.group/videos/pcb.1898805307013695/1898805250347034/?type=3&theater
```

---
## \#27 Posted by: caustin Posted at: 2016-10-28T04:06:40.014Z Reads: 90

```
Haha, now that's what I'm talking about. Killing it on 10s. I have that same setup on an old evolve gen 2 carbon deck I am modding. Same except for 12s and 100mm MBS ATLB wheels until I get your 6" billet pneumies!
```

---
## \#28 Posted by: caustin Posted at: 2016-11-04T02:12:33.790Z Reads: 77

```
Haha, early Christmas. Finallly rocking these new @psychotiller 6" billet pneummies 55psi!!<img src="/uploads/db1493/original/3X/5/2/528144e6c375b5296d2da76b7cf8beb948ff6bf4.JPG" width="375" height="500">
```

---
## \#29 Posted by: psychotiller Posted at: 2016-11-04T02:41:53.568Z Reads: 75

```
Nice! Was hoping you'd get them today. What board are they going on?
```

---
## \#30 Posted by: caustin Posted at: 2016-11-04T02:46:39.758Z Reads: 70

```
Haven't decided yet, want to toy around with then first and see how they might fit in an evolve carbon gen2 I am modding. Who knows maybe they will also somehow fit on my evolve carbon GT, that would be interesting!
```

---
