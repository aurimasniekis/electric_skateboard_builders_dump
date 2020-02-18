# Looking for FOC settings for smooth start-up/braking

### Replies: 36 Views: 2063

## \#1 Posted by: thatguy614 Posted at: 2017-05-07T00:12:45.006Z Reads: 231

```
Just got my board running today, and after being dissapointed with BDLC on startup I switched to FOC. I can get a decent start up on flat ground but I am looking for a little more power so I can start on hills and more smoothly on flat ground.

I have a VESC-X from Enertion and I am running a 6S pack with a Tacon Bigfoot 110 motor. If anyone has suggestions or experience im open to try them! Below are my current settings and the board.
<img src="/uploads/db1493/original/3X/e/e/ee25c9bda317d34aa31dac47a96085fe59d9ccc3.png" width="690" height="396"><img src="/uploads/db1493/original/3X/b/f/bf6a95d8b7fe4b638af70cd2956031b8f7c538b2.png" width="690" height="391"><img src="/uploads/db1493/original/3X/8/e/8eb88f27935a651d6d128c24b87878f60d5fd41f.png" width="690" height="396">

 <img src="/uploads/db1493/original/3X/6/d/6d0e5ddc705c8d15fd4b75b8b2c5098671fa6c46.jpeg" width="375" height="500">

Also huge shoutout to everyone on this forum, theres no way this board would be running without yall. Ride on!!
```

---
## \#2 Posted by: Smorto Posted at: 2017-05-07T00:14:48.421Z Reads: 213

```
First off, I know nothing about the setting so I can't help you there but  dang thats a long belt lol. Why such a long belt? And do you have any more pics about the mount? It looks interesting :slight_smile:.
```

---
## \#3 Posted by: saul Posted at: 2017-05-07T00:42:52.625Z Reads: 211

```
small high kv motor, and low 6s voltage, all the things you don't want for smooth startup and torque. :joy:

but good luck....
```

---
## \#4 Posted by: thatguy614 Posted at: 2017-05-07T00:59:33.178Z Reads: 213

```
I had the long belt because of the way my trucks were set up. The Enertion 55 tooth belt was too short and the motor wouldn't fit, so I had to guesstimate and went with an 80 tooth just to be safe, I could probably work with a 65 tooth, but I had to get it done because its a semester project for school. As for the mount, its nothing fancy just some angle iron and a U bolt. Ill probably upgrade to a machined mount in the future. 
<img src="/uploads/db1493/original/3X/d/a/da8b8b33225dce7629011fc11c7af6548c8fecf2.jpg" width="375" height="500"><img src="/uploads/db1493/original/3X/7/b/7bce71bb22440f263b2ef20ad13f9b7fe0cb86b5.jpeg" width="375" height="500">
```

---
## \#5 Posted by: Smorto Posted at: 2017-05-07T01:00:48.583Z Reads: 200

```
Ahh I see, good work!
```

---
## \#6 Posted by: Eboosted Posted at: 2017-05-07T02:19:59.006Z Reads: 197

```
Those trucks a perfect for rear mounting motors, outwards. Shorters belt anf more stable mounting points.

I guess you are runing sensorless, try runing hybrid mode on BLDC is pretty good, nos as good as sensored FOC, but with more power
```

---
## \#7 Posted by: willpark16 Posted at: 2017-05-07T02:28:21.081Z Reads: 197

```
That mount is your issue buy new trucks and a new mount and ur belt is wayyyyy too lomg
```

---
## \#8 Posted by: thatguy614 Posted at: 2017-05-07T02:28:43.196Z Reads: 195

```
Ahh I didn't even think of doing that, Ill give it a shot! Also Ill try the BDLC hybrid and just up the boost factor and see how that fares
```

---
## \#9 Posted by: Eboosted Posted at: 2017-05-07T02:30:58.909Z Reads: 197

```
Did you wire the hall sensors?, you need to do tha before attempting to try hybrid mode
```

---
## \#10 Posted by: Hummie Posted at: 2017-05-07T02:46:46.769Z Reads: 192

```
Motoramps.com http://motoramps.com  This site was made to explain the math details by Devin who I think might be the sole person booted/banned from the forum!   Motor and battery amp settings are the way to control your power and at what speed you have access to it. You are far from the power you could have and smoothness with that esc on foc with good settings for low speed power
```

---
## \#11 Posted by: thatguy614 Posted at: 2017-05-07T02:49:37.090Z Reads: 181

```
Nope, I honestly don't know if it has hall sensors, is that a position sensor?
```

---
## \#12 Posted by: thatguy614 Posted at: 2017-05-07T02:53:06.286Z Reads: 180

```
Looking at the site, some of the equations he gives are circular, how do you find duty cycle %? He definitely sounds like he knows what he's doing but i'm a tad lost there.
```

---
## \#13 Posted by: Hummie Posted at: 2017-05-07T02:58:42.874Z Reads: 173

```
Yup  haha.  whats ur motor resistance?  U can get it off your plugged in vesc doing the tests.   Give me that and whats your desired wattage when pulling full throttle power and He could give u the numbers that will do that
```

---
## \#14 Posted by: laurnts Posted at: 2017-05-07T03:06:26.526Z Reads: 173

```
No wonder you get disappointed with BLDC startup mode. You have 0.070 startup boost. If I am not mistaken, it should have been 0.70. If you have 0.070 that means your outputting 10x less what you should be getting lol.
```

---
## \#15 Posted by: thatguy614 Posted at: 2017-05-07T03:07:07.053Z Reads: 171

```
Heres my resistance R: 0.01196 Ω and as for watts, I can pull 22 volts but I don't want to kill the battery every time I hit the gas (5000mAh pack). What would you suggest? maybe 300 watts? Sorry I don't know my stuff super well, just trying to keep up with the learning curve.
```

---
## \#16 Posted by: thatguy614 Posted at: 2017-05-07T03:07:51.759Z Reads: 164

```
That only applies to BDLC correct? Im currently running it in FOC
```

---
## \#17 Posted by: Hummie Posted at: 2017-05-07T03:18:38.578Z Reads: 161

```
What battery pack is it or what's the c rating.
```

---
## \#18 Posted by: thatguy614 Posted at: 2017-05-07T03:27:27.883Z Reads: 160

```
its a 6s, Ill probably make it 8 soon but uhh college budget here :confounded:
```

---
## \#19 Posted by: Hummie Posted at: 2017-05-07T03:29:27.647Z Reads: 161

```
What's the c rating of the 6s 5ah battery
```

---
## \#20 Posted by: thatguy614 Posted at: 2017-05-07T03:39:48.919Z Reads: 162

```
Oh! sorry, they're 20C
```

---
## \#21 Posted by: Jinra Posted at: 2017-05-07T03:42:49.257Z Reads: 149

```
Startup boost is minimum duty cycle in current control mode. Setting this to .7 would result in insane acceleration as that's 70% duty cycle. This shouldn't affect acceleration as much as it does prevent cogging from non-sensored setups.
```

---
## \#22 Posted by: thatguy614 Posted at: 2017-05-07T03:48:18.090Z Reads: 147

```
Ok good to know. The BLDC tool is pretty epic, just trying to get a handle on how to really use it to its full potential. Thanks!
```

---
## \#23 Posted by: Hummie Posted at: 2017-05-07T04:00:52.712Z Reads: 151

```
startup boost seems kind of the opposite of smoothness in a way as it skips the ramp up of the duty cycle.    What's it good for?

with 20c and 5ah batteries the math says you can do 100 amps continuous but it's over-advertised and maybe 50 more realistic.  You'll want all of it on 6s.  plug in your vesc and see what it's set at and maybe you could show us your screen shots.
```

---
## \#24 Posted by: Jinra Posted at: 2017-05-07T04:05:00.127Z Reads: 145

```
Like i said, useful for preventing cogging when starting up in non sensored mode
```

---
## \#25 Posted by: thatguy614 Posted at: 2017-05-07T04:09:54.671Z Reads: 142

```
50 Amps for motor max? The screenshots at the top are what i'm currently set at which is 60. I do want a smoother start but more power could be an answer as the current issue is jittering when im not over 50% throttle
```

---
## \#26 Posted by: Hummie Posted at: 2017-05-07T04:29:03.641Z Reads: 135

```
i meant battery max but I see you already posted your screen shots.  I'd increase both motor and battery since you're on 6s especially.    i could give you answers if you figure your motor's resistance and you decide what power you want when you pull the throttle fully.
```

---
## \#29 Posted by: thatguy614 Posted at: 2017-05-07T04:33:53.466Z Reads: 132

```
Ok, here's the motor resistance I have right now, also I upped my motor and battery max to 70 and 55 respectively and didn't see too much of a change. <img src="/uploads/db1493/original/3X/c/5/c53bd46b582491aab4104e9985fed46f54111753.png" width="690" height="308">
```

---
## \#30 Posted by: thatguy614 Posted at: 2017-05-07T04:36:30.783Z Reads: 136

```
Upped the boost in BLDC and it does give way more torque starting but its really abrupt power. Also I'm a fan of how much quieter FOC is.
```

---
## \#31 Posted by: Hummie Posted at: 2017-05-07T04:55:19.208Z Reads: 135

```
youre especially limited by the software as far as how many watts you can do at low speeds because youre only doing 24 volts and the max motor amps is 200.  you have two options i came up with as far as wattage since you didnt say.


motor amps at 160 is said to be safe here on this forum but in other parts of the world 200 motor amps is good so you chose.  i like 200

360          watts continuous
13 battery amps
160 motor amps   and max max of 200

478 watts
20 battery amps
200 motor amps  max max of 200
but you could add more battery amps all the way up to 100 according to the battery manufacturer.  youre at the max of motor amps and that's the low end power and the battery amps category is for higher speed power generally.  so you can fiddle just wont have even power at all speeds which isn't important.

motor amps aren't really amps and you'll still only pull a max of the battery max from the battery, and that's the math part you want to skip
```

---
## \#32 Posted by: thatguy614 Posted at: 2017-05-07T05:15:44.521Z Reads: 123

```
Ok this is fantastic! Thanks a bunch! Ill mess around with those settings and let you know how it does. Just to be sure, settings that high shouldn't cause too much strain on the VESC will it?
```

---
## \#33 Posted by: Hummie Posted at: 2017-05-07T06:08:54.017Z Reads: 119

```
  try the 160 at least and then there's no one who will say it's too high.
```

---
## \#34 Posted by: thatguy614 Posted at: 2017-05-07T16:28:04.183Z Reads: 111

```
Bumping the motor max helped a bit, its still not perfect, but I think my next step is to rear mount the motor so I can get better torque and  more clearance.
```

---
## \#35 Posted by: Hummie Posted at: 2017-05-07T16:31:26.231Z Reads: 115

```
if youre still at 48 battery max that's going to limit a lot on 6s.  I'd bump that way up too.   your battery is good for many more and as long as it's not getting warm it should be good.  maybe do 100 battery and 200 motor!

you can get really good power...it's possible with what you have

you likely willl start to heat your batteries though.  with the 20c and 5ah it's supposedly good for 100 continuous like said but they exaggerate, like said, and people will assume half, but that's conservative and you could definitely do more and just reduce the lifespan of the battery.  the battery will possibly puff a bit and get warm but that happens sometimes in such a situation.
```

---
## \#36 Posted by: Ackmaniac Posted at: 2017-05-07T20:58:23.916Z Reads: 109

```
@Hummie even after the guys in the Vedder forum told you that you are wrong with the 200 amps theory (standard VESC can only detect 165A maximum) you still continue to give the wrong advice's.
```

---
## \#37 Posted by: Hummie Posted at: 2017-05-07T21:37:18.159Z Reads: 110

```
 I explained above that there are people who will say the vesc can only do 160 or 165 motor amps.    There are other people who will say it's fine.   Im not sure what's possible and have asked on vedder's forum as mentioned.   The only reason presented as to why it wont work is the sensor can't sense that high.  I've ridden at least 200 miles on 200 motor amps.  (now back to two motors and tamed it down).  Why it worked fine for me I don't have an answer but I will do it again on another single drive for sure in maybe a month or two and see what the results are again.   It was the quietest smoothest ride I've ridden besides having no problem with low speed power or cogging.
the  vesc software, and the 200 or possibly 160 amp motor limit reduces the possible power at low speed especially on lower voltage as the wattage numbers I posted above show.  
It's worth getting to the bottom of
```

---
## \#38 Posted by: thatguy614 Posted at: 2017-05-07T22:19:02.647Z Reads: 104

```
Good to know, I currently have it set at 160, but I will probably back it down to 150 just to keep away from the max of what the VESC is rated at. Definitely want this thing to last as long as it can.
```

---
