# First Build- kicktail deck- paris 180mm trucks- 6364 190kv motor- 5000mah 3s- ESC/ VESC TBD

### Replies: 36 Views: 2885

## \#1 Posted by: potato Posted at: 2017-07-12T00:28:32.608Z Reads: 255

```
Hello,
I am looking to build my first electric long board. This being my first board, I am looking for advice on my build. I can solder, but can not weld, so I am also looking for advice on the best way to attach my motor mount to the board. I am looking for advice on my VESC/ESC. I also wanted to avoid actual drilling and welding all together, but will find a way if needed.  Mainly, I am looking for advice on the motor mount situation (**leaning towards two part epoxy**) and if all the parts seem like a good choice. If not, what parts are? Thanks so much!

**Build:**

**Longboard**

Atom kicktail deck (already had it)
Paris 180mm trucks
83mm flywheels
ABEC 7 Bearings

**Drive Parts**
Turnigy Aerodrive SK3 - 6364-190kv Brushless Outrunner motor
36T 9mm Enertion Drive Hub
15T 9mm Wide Motor Pulley
HTD5 9mm Timing Belt 265T
Electric Longboard Skateboard Motor Mount For 5065 5055 6374 6364 Motor-
<img src="/uploads/db1493/original/3X/b/c/bc9458a01dda711ed609b68b4f5a4dbea7068bee.jpg" width="690" height="283">

**Electronics**
Zippy Flight Max 5000mAh 20c 3S1P / 3 Cell / 11.1v
NEED ADVICE ON VESC/ESC
HobbyKing® ™HK-GT2B 3CH 2.4GHz Transmitter and Receiver\
All other necessary bits and pieces (thread locker, bannana jacks, wire, etc..)
```

---
## \#2 Posted by: pat.speed Posted at: 2017-07-12T02:02:48.771Z Reads: 230

```
I built a similar build to yours and I used a motor that was 190kv and it is very slow on 6s. I really wish that I had gone with a higher kv maybe around 245kv

https://www.electric-skateboard.builders/t/350-esk8-build/25252
```

---
## \#3 Posted by: pat.speed Posted at: 2017-07-12T02:05:43.659Z Reads: 216

```
Or you could use a Vesc and 9s which would give you more speed or even 12s. Just make sure to set the erpm limit on the Vesc if you use 12s because if your motor is slightly high kv like mine is it could blow the vesc
```

---
## \#4 Posted by: potato Posted at: 2017-07-12T02:10:09.076Z Reads: 210

```
Ok, I'm not looking for a board that is to speedy, just one that can get me from point A to point B at a reasonable time, about how slow was the 190kv motor on 6s. What 9s battery setup would you recommend, and do i need to worry about erpm on a 9s set up? I am guessing that a 245kv motor would work well with a 9s setup, am I wrong? Also, can you give me a link to an VESC you would recommend? Thanks.
```

---
## \#5 Posted by: potato Posted at: 2017-07-12T02:44:39.044Z Reads: 192

```
Hobbywing QUICRUN-WP-8BL150 will this esc work? I am not to comfortable programming a vesc... I will take your advice on a 245kv motor instead.
```

---
## \#6 Posted by: wafflejock Posted at: 2017-07-12T02:45:07.162Z Reads: 197

```
Can get a pretty good idea of top speed using the calculator here and punching in some numbers http://calc.esk8.it it's pretty accurate.  For the VESC I've got mine from DIY and no problems from what they delivered for me (I did fry one but was my own fault).  Seems anyone who carries them is pretty good apparently aside from Maytech (from what I've read).

Switching from 6S to 12S basically means the difference between 18mph max top speed to 36mph max top speed.  Also varying the kv by 50kv is pretty significant as well.  I tried both 6S and 12S I personally settled on 10S with a 149kv 6374 SK3 so top speed is about 21mph with my current setup.  Typically I cruise between 10-15mph and average 12mph on trips.

With 2 5S 5Ah in series, so 10S 5Ah effectively I get 12 miles range before I'm down to 3.6V per cell.

---

Strongly recommend the VESC it's worth the cost and time to go through a few configuration guides, Benjamin has a simple walk through video for some basic configuration as well.

https://www.youtube.com/watch?v=17CSl1iXYE8

http://www.electric-skateboard.builders/t/new-vesc-user-read-this-complete-walktrough-of-the-vesc/2980

https://www.youtube.com/watch?v=1TF8XARDa6U

The VESCs typically come preprogrammed with the firmware so you just use the configuration tool and a USB cable to calibrate it for your motor and configure your battery cut off limits and control settings.
```

---
## \#7 Posted by: potato Posted at: 2017-07-12T02:56:34.512Z Reads: 154

```
So in that case, what do you think of a 8s battery setup with the 190kv motor I put in my original build list,  along with the following VESC- diy-electric-skateboard-kits-parts/vesc-the-best-electric-skateboard-esc/
I will definitely need to do much more research on VESC's then.
```

---
## \#8 Posted by: korryh Posted at: 2017-07-12T02:57:08.788Z Reads: 146

```
You may want to go with caliber 2 50 trucks. Because of the shape you will have less issues with motor mount and will have more options. Also, VESC is your best bet, I went through  300.00 worth of ESCs (actial fire with HK and others just stopped working).
```

---
## \#9 Posted by: potato Posted at: 2017-07-12T03:01:00.135Z Reads: 143

```
Alright, sounds good, what kind of troubles will I go through if I decide not to use 250 trucks? (I already have 180mm trucks)
```

---
## \#10 Posted by: wafflejock Posted at: 2017-07-12T03:02:39.248Z Reads: 147

```
Looks pretty good in general agree with @korryh too though, also for mounting the trucks can get some JBWeld if there is any wiggle can use that to solidify the connection without really welding and is comparably strong (just make sure you have it all positioned how you want it before using JBWeld you can't remove it).

https://www.amazon.com/dp/B0006O1ICE/ref=asc_df_B0006O1ICE5071031/?tag=hyprod-20&creative=394997&creativeASIN=B0006O1ICE&linkCode=df0&hvadid=198093606370&hvpos=1o1&hvnetw=g&hvrand=11002247154439946818&hvpone=&hvptwo=&hvqmt=&hvdev=c&hvdvcmdl=&hvlocint=&hvlocphy=9021569&hvtargid=pla-320192516391

http://calc.esk8.it/#{"batt-type-lipo":1,"batt-cells":8,"motor-kv":190,"system-efficiency":85,"motor-pulley-teeth":15,"wheel-pulley-teeth":36,"wheel-size":83}|

Lower voltage means higher amperage to deliver the same wattage and more amperage means more heat and therefore energy loss in wires and components, so really ideal to go higher voltage for that reason (aside from higher speed) it also will affect the torque to some degree.
```

---
## \#11 Posted by: potato Posted at: 2017-07-12T03:20:42.640Z Reads: 130

```
So by mentioning lower voltage are you hinting that I should either increase cell count/ decrease motor size, or are just saying that for reference and the voltage on the 8s set up is fine?
```

---
## \#12 Posted by: wafflejock Posted at: 2017-07-12T03:27:39.157Z Reads: 135

```
Yeah just saying in general higher voltage means more power with less amperage so that's better, 8S I think should be fine with the setup you had described like in the link the calc in my previous post.
```

---
## \#13 Posted by: potato Posted at: 2017-07-12T03:28:53.088Z Reads: 133

```
Alright, Thanks so much! I have been wanting to build a board for a long time but had so many questions and didn't know where to start.
```

---
## \#14 Posted by: wafflejock Posted at: 2017-07-12T03:29:44.224Z Reads: 133

```
Yup we all start there and that's how we end up here :) all good nice that someone put that calculator together too helps to be able to do that without needing to crunch all the numbers yourself (and trust your own math).
```

---
## \#15 Posted by: korryh Posted at: 2017-07-12T05:02:05.773Z Reads: 128

```
The trucks I was referring to are the caliber2 (name of the truck) 50 is the angle of the truck. It comes in 45 or 50 degree options. This truck has a "D" shape profile that helps the mount stay in place. As opposed to the cylinder shape profile like the Paris trucks where the mount can spin around and around.
```

---
## \#16 Posted by: pat.speed Posted at: 2017-07-12T06:04:42.531Z Reads: 120

```
If your going with 8s what esc will you be using? I have heard that the Vesc can get a bit hot sometimes when going up hills on an 8s setup. I don't actually own a Vesc but I have only heard good things about them
```

---
## \#17 Posted by: potato Posted at: 2017-07-13T00:44:30.820Z Reads: 104

```
Oh, ok that makes so much more sense. (250mm trucks seemed crazy wide) and yes, I definitely will look in to those. Sorry for not responding earlier. (response limit for first time user was reached lol)
```

---
## \#18 Posted by: potato Posted at: 2017-07-13T00:45:13.267Z Reads: 110

```
I will most likely be using this VESC- diy-electric-skateboard-kits-parts/vesc-the-best-electric-skateboard-esc/
```

---
## \#19 Posted by: potato Posted at: 2017-07-13T00:46:41.564Z Reads: 104

```
Another question, spinning the motor the opposite direction works as a break right? If so, how effective is it at stopping when you are going down a hill. How do regenerative breaks work?
```

---
## \#20 Posted by: wafflejock Posted at: 2017-07-13T01:16:21.770Z Reads: 111

```
The regenerative brakes can be really strong.  I honestly probably couldn't explain it properly in terms of technical detail but the gist is the VESC is using the motor as a generator and allowing current to flow back into the batteries (basically applying a higher voltage than the battery itself to the leads the same way the chargers work).  So instead of pushing Watts/power into the motor from the battery to make it turn you're using the turning of the motor to drive power into the batteries (and creating drag).  There could be more to it but that's what I gather.

Biggest problems with stopping fast are:

1 It might throw you from the board.  If you don't have your feet locked in tight on the grip and don't have much concave or a nose or tail on the board then if you try to stop from 20mph+ to 0mph in a short time the board might stop but your inertia will pull you off of it and onto the street.

2 You can put as much or more stress on the pulley and belt while stopping as you do while accelerating so can tear up the belt more quickly.

3 If you have only one motor then only one wheel is being used to stop the whole board, if you are braking really hard you'll notice the tug to one side since the rest of the board wants to keep going (inertia again).  Also if that one wheel is off the ground you'll have trouble but doesn't take too long to get used to planting over the back trucks when you're going to accelerate hard or need to brake quickly.

Usually I try to slowly decelerate up to intersections and if I need to stop quickly I use the regen braking to get down to a speed I can run off the board and do that then use the brakes to get the ghost riding board to completely halt (not a good look but it works in emergencies).

In terms of hills there aren't a lot of them here really, but so long as you don't let yourself get over like 10-15 mph downhill the regen braking won't have a problem slowing you down, once you've got a lot of momentum it's more of a problem (again not just the regen braking itself but all the other components under stress like the pulley connection to the motor shaft and the belt).
```

---
## \#21 Posted by: korryh Posted at: 2017-07-13T02:25:15.509Z Reads: 85

```
Maybe get in on the focbox (Vesc updated in a case) group buy 115 shipped. I am still on the fence because I don't need them but will probably buy because it's a great price.
```

---
## \#22 Posted by: potato Posted at: 2017-07-13T03:29:17.242Z Reads: 85

```
Ok so just don't go to fast down the hills to avoid damaging the components, got it. 10000 mah should be good for 8s set up right? Also thanks for the lengthy explanation about the brakes.
```

---
## \#23 Posted by: wafflejock Posted at: 2017-07-13T03:49:22.048Z Reads: 96

```
No problem just lessons learned in real use.  Short answer is yes... details are below.

10Ah is just the capacity, for the batteries you basically need to know 3 parameters, capacity (expressed in Ah or mAh), energy potential (voltage, 8S in this case), and max amperage (current expressed in Amps A or as a C rating on LiPo packs).

10Ah means you could draw 10A from it for 1 hour continuously (or 5A for 2hrs).  Basically more Ah capacity means more volume/weight for batteries and longer range.  Personally I have a 10S 5Ah battery setup (2 5S 5Ah in series) and can get 12+ miles out of it (I draw about 5A on average, ride for about an hour including little stops).  To compare different battery capacities that have different voltages it's useful to look at them in terms of Watt Hours or Wh which you just calculate by multiplying the nominal voltage of the batteries by the Ah, so 10S*3.7V*5Ah = 185Wh, compare with 8S*3.7V*10Ah = 296Wh.  So you would get killer range with 10Ah but keep in mind if you stack 2 5Ah batteries in series it is still just 5Ah because the current flows through both batteries at the same time/rate (as opposed to if they are in parallel where you would add the capacity and max current throughput, but get no additional voltage).

The 20C on the battery is the max current rating and tells you how much you can "safely" draw from the batteries without rapidly killing them (due to their own internal resistance and overheating).  For example 20C * 5Ah = 100A max discharge, in reality having higher C rating helps to avoid voltage sag while the batteries are delivering power and will allow you to get a bit more range most likely (discharge graphs if you search google images can see how A draw on different C batteries affects how many mAh you can get out before the voltage dives).  Real world difference between say 20C or 30C or 40C though your guess is as good as mine, been using 20C 5Ah for a while without issue but imagine it could deliver more (unnecessary) power if I went with 30 or 40C.

---

Realize that was already a lot but a few other things to sort of keep in the back of your mind about all this, I'm drawing somewhere between 10-20A on accelerating and 3-6A (based on crappy ammeter measurements, getting a metr.at module soon hopefully) usually when riding continuously but these numbers will vary especially when you reduce voltage (it will need more amps to get the same kind of power/acceleration).  Also going faster means more wind resistance and overall more load on the components so they will run more/less efficiently depending on how/where you ride.
```

---
## \#24 Posted by: potato Posted at: 2017-07-13T06:18:03.677Z Reads: 77

```
 So if I hook up my batteries in series, then I will get more voltage (the full 8s), But in parallel, I will get the full Ah (10Ah) but only 4s of power. So you have two 5s 5aH batts, but they have 5Ah capacity since they are is series, but still supply 37V of electricity? Therefore I assume that I should hook my batteries in series to achieve the 29.6V of energy potential the calc says? (I have same Ah as you now yet more range because I use less voltage) Did I get that all right?
```

---
## \#25 Posted by: wafflejock Posted at: 2017-07-13T06:20:03.262Z Reads: 77

```
Yup all sounded right to me.
```

---
## \#26 Posted by: potato Posted at: 2017-07-13T06:25:02.792Z Reads: 75

```
Sweet! Can't wait to get the parts and start building! I will post pictures and problems I encounter here. (Probably mostly with the VESC) I will stick to the 20C batteries since you use them without issue and I don't need the "unnecessary power" of 30C and 40C.
```

---
## \#27 Posted by: wafflejock Posted at: 2017-07-13T06:58:42.240Z Reads: 78

```
Yeah I don't mean to downplay the benefit of higher C rated batteries when you are drawing a lot of amps, say a big guy trying to go fast up pretty big hills or a sizeable helicopter built for 3D acrobatics, but I just haven't ever seen a time I actually draw that many amps personally.

Again take with a small grain of salt since you have slightly lower voltage at 8S you'll have slightly higher amps to get the same Watts power to the motor. Seeing as how I've never actually seen my board draw that much current in any measurement I've done so far and my batteries seem to be doing fine after about a year I think it's fine.
```

---
## \#28 Posted by: potato Posted at: 2017-07-27T18:21:31.844Z Reads: 66

```
soooo......All the parts are arriving now, but I realized that I accidentally ordered a 5200 mah battery 4s, but it only has 10c discharge. How will this effect my board? Should I try to return it and get new batteries?
```

---
## \#29 Posted by: potato Posted at: 2017-07-27T18:27:46.821Z Reads: 69

```
However, I plan to set my motor max at only 40A, so it should be ok since I calculated the max discharge of my 5.2A 10c battery to be 104A?
```

---
## \#30 Posted by: wafflejock Posted at: 2017-07-27T18:37:44.225Z Reads: 75

```
Check lipo discharge charts to see for yourself but basically lower C means higher internal resistance in the cells so you consequently get more heat build up and voltage sag with lower C batteries and will likely shorten the number of cycles you can really use the batteries.  I use 20C 5Ah but really that's considered the low end of acceptable typically keep in mind manufacturers will rate their components in ideal situations (controlled pressure and temperature etc)

If your cells are in series they all experience the same continuous amperage flow and you only add voltage the Ah capacity doesn't get added since you are drawing electricity through both at the same rate.  Also C rating is per battery based on it's Ah in that scenario, if you instead put them in parallel the Ah and the C rating from both batteries get added since you're only drawing half the circuits total current from each battery when in parallel. In series you're looking at 52A max rating which is still above what you'll probably ever draw (can do Volts*Amps=watts or watts/volts = amps to work backwards from your motor max power to the max amperage given a voltage).  All that said higher is better.
```

---
## \#31 Posted by: potato Posted at: 2017-07-27T19:09:57.965Z Reads: 63

```
Ok, so my question is if I can run it on 10c by setting max motor to 40A without frying anything . I will switch to 10s with higher c in the future.
```

---
## \#32 Posted by: wafflejock Posted at: 2017-07-27T19:26:24.226Z Reads: 63

```
Pretty sure you can limit amperage both on the motor side and on the battery side so yeah basically as long as they aren't severely overheating should be fine (probably wouldn't do too much hill climbing and just monitor the battery temp on the first few runs keep in mind the heat builds up on longer cruises)
```

---
## \#33 Posted by: potato Posted at: 2017-07-27T19:48:51.179Z Reads: 61

```
Ok, so how would I limit amperage on the battery side? I know I can limit motor amperage through bldc for vesc . Also only the battery is in danger here right? Because I have insurance for my batteries if they break.
```

---
## \#34 Posted by: wafflejock Posted at: 2017-07-27T19:54:16.631Z Reads: 67

```
Yeah basically the ESC can deal with some max amperage but it will only draw as much power as it needs to drive the motor around.  So basically only issue here is the batteries can't really consistently supply that current without starting to get warmer (due to their internal resistance, also the warmth creates more resistance which isn't ideal).

The components on the ESC (MOSFETs are mostly dealing with delivering the power from the battery to the motor) have some max limit, pretty sure for the VESC the MOSFETs are rated for 50-60A continuous and 240A peak bursts but the higher amps it is drawing for any amount of time equals more heat build up in those components... this is mainly why higher voltage is better, since power is Volts*Amps if you can increase the voltage you can reduce the amps and keep the same power output (and by reducing the amps you reduce the heat loss and consequent voltage sag).
```

---
## \#35 Posted by: potato Posted at: 2017-08-14T01:42:24.506Z Reads: 59

```
Soooo, I finished the board and it works really well!!! However, I am having issues once I reach top speeds. I was riding the board and I pulled the remote trigger as far back as I could, reaching top speed. However, around 10 seconds after reaching the top, there was a sudden jolt in which the board went even faster and almost threw me off the board. Does someone know what it going on? I can send pictures of the programming and what not.
```

---
## \#36 Posted by: wafflejock Posted at: 2017-08-14T20:54:16.455Z Reads: 50

```
Not sure might be a loose connection between the receiver and ESC try to be sure everything is either soldered and/or mechanically secured with hot glue or whatever else so no connections can vibrate loose easily.  Check the ppm high and low values in the display after you're sure the connections are solid, you can disable control mode and still use the display to adjust the min and Max Ms values for the ppm input.
```

---
