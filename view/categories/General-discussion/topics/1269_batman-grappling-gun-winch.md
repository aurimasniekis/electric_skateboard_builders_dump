# Batman Grappling Gun Winch

### Replies: 21 Views: 3102

## \#1 Posted by: SufficientlyAdvanced Posted at: 2016-02-07T22:16:35.800Z Reads: 96

```
Hi Everyone!

This isn't an E-Board build, but it is an interesting challenge and this forum seems to have the most knowledgeable peeps when it comes to high powered brushless drive design. If this topic has no place here, let me know and I'll delete it!

Anyways, I'm trying to build a winch that fits on a co2 propellant grappling gun that can pull me up 7-10 meters at least .33 m/s. So far I've settled on using an SK3 6374 149 Kv motor on 12S, driving a 12mm diameter reel through a 12:50 timing pulley transmission. The rope is a 3mm Nylon cord used for spearfishing, breaking strength 1050 lbs.

149 Kv gives a Kt of 0.064, which at the max current rating of the motor (70 A) gives a max torque of 4.48 Nm. The theoretical load being pulled up is 100 kg, or 981 N. On a 12mm diameter reel, that requires a torque of 981*0.006= 5.886Nm. So through the 1:4.167 reduction, the motor has to supply 1.41 Nm torque. Assuming a max theoretical angular velocity of 687.5 rad/s at 44V and a max theoretical torque of 4.48 Nm and assuming a linear torque-speed curve, when the motor is providing 1.41 Nm torque it is spinning at 473.33 rad/s, which means a reel speed of 113.59 rad/s, which means on a 12mm reel an ascending velocity of 0.68 m/s. So I figure even after tossing out losses and efficiency and such that should still give me at least 0.33 m/s, while consuming at least 22 A, which doesn't seem that bad!

I've got a BS in electrical engineering but I'm a total noob when it comes to these high powered outrunners, so I was hoping I could get some opinions on this set up. Does the math above make sense? There's a ton of assumptions being tossed around there. And what's your gut feeling about this kind of performance? I've never even held a 63mm brushless outrunner before, so I have no feel for what they *realistically* can or can't do.

Also, I'm trying to finish this build ahead of Batman V. Superman, so I don't know if I can wait the 3-4 weeks for the legendary VESC. I've also got concerns about the VESC max 50 A spec, since once the 3mm Nylon rope gets reeled up the effective diameter doubles, which means the motor will likely be drawing over 50 A. Do you guys think the Torqueboards 12S ESC would do? Or should I chance using the VESC?

Thanks for reading! This board really looked like it had some of the smartest dudes around, and if this is too off topic I sincerely apologize!
```

---
## \#2 Posted by: psychotiller Posted at: 2016-02-07T23:12:57.354Z Reads: 89

```
Math isn't my strong suit but I can say parts and numbers look good. you are going to have to strap your hand or arm to the gun. I honestly don't think you'll be able to just hold onto it. From what I've experienced with the VESC compared to other esc's the 50a mark sets a red flag for me. My best performing setups have been with Castle or Hobbywing ESC's and were @ 6s or 8's. Both had the torque and punch to pull my boards into the high 30's as well as high 40's (mph) without blowing any fuses or drv chips.

The vesc's got some programming skillz though I'm thinking duty cycle would be good if you go this route. I don't think it will handle the amps you'll pull though.

PICTURES! :open_mouth:
```

---
## \#3 Posted by: laurnts Posted at: 2016-02-07T23:15:24.111Z Reads: 90

```
Theoretically your math could be right by numbers, since you have figured out this far. I am not an electrical engineer my-self and this question are not really easy to answer by just many of us in this thread due to the differences and our lack of experience in grappling gun.

But I have 1 fact that i could tell you, based on my opinion I don't think brushless motor of SK3 149 KV would pull 70A to pull you up. It has max 70A rated rating but, it's a peak Amps. It possibly run 1 - 3 seconds before it got destroyed. Brushless outrunner has excellent torque when it already starts rotating, hence you will need to get that motor spinning on certain level of speed before it could pull you up. You could expect 149KV motor to draw about 30A - 40A which is already quite high before it start cogging / jittering and so on if it doesn't have proportional speed to it.

VESC has great startup torque speed but again, this is horizontal kinetic direction and not vertical. Even on horizontal mode you can already hear some smooth cogging / modulating occur. You might wanna use an additional hall sensor to that 149KV SK3 motor to be better at low speed, I would recommend this if you try it anyway. Also you need to know that VESC has current limit of Peak 60A I believe, which you could run for several seconds before burn / shorts.

Last but not least even if you have all of this worked out, mechanically it's still quite impossible. SK3 Motor are made for high speed and not so much torque. It doesn't even have a flat spot for pulleys to grip on the shaft that well. Many of us experience spin outs if not installed with grub screw combined with flat spot. Yet the bearings would be under great stress even if you manage to setup with a gear / belt if your mechanical design is not perfectly suited for the condition.

There are many aspects that could go wrong here, but if you like the risk and chance you should try them. I wouldn't recommend to build this with SK3 149KV at least, you might even need 2 or 3 of them to get it working. And so you would also need 3 VESC to get descent power with quite complex mechanics. Your battery also need the one that has mega high discharge / burst to handle the power required by 3 motors. Overall this would also add quite some weight in the overall build, hence it's not quite as streamline as what batman has. I would like to see this works, but from my opinion, this is going to be a quite expensive build which the fun factor and the succeed rate is lower than just building an electric longboard :smiley:
```

---
## \#4 Posted by: SufficientlyAdvanced Posted at: 2016-02-07T23:23:31.348Z Reads: 78

```
Thanks for the replies! The plan is to connect the gun to a climbing harness, so while I'll be holding onto it, almost all my weight will be supported by the harness. Glad to hear good a good experience with Hobbywing, at 12S I'm really concerned about the ESC quality. I have a Youtube channel where I build these sorts of gadgets, so that's where the results will go if it works!

Yup, while the max rated current of the SK3 6374 149 Kv is 70 A, I don't plan on putting enough load on the motor to get quite that high. Thanks for the heads up on the smooth shaft, I suppose I'll have to grind a side flat. Your cogging anecdote also concerns me, is that something that happens often with E-Boards going up hill/other high load situations? I'd like to avoid a sensored set up, but if it's necessary that's not such a big deal.
```

---
## \#5 Posted by: SufficientlyAdvanced Posted at: 2016-02-07T23:32:06.961Z Reads: 76

```
Ah hit the wrong reply button, but this video is what gives me some hope for the idea: https://www.youtube.com/watch?v=ESFewdU0JcA

An 18V cordless drill has enough oomph to pull about 80kg up, albeit slowly. Of course the gearing on the drill is going to be much better than my plan, but I figure if you put a kilowatt into a brushless motor, something ought to happen right? :stuck_out_tongue:
```

---
## \#6 Posted by: psychotiller Posted at: 2016-02-07T23:39:29.066Z Reads: 74

```
-Not 12s with castle or hobbywing. 8s max. I know first hand that an XL2 esc can handle 80a continuous @8s. 
12s builds took off with the knowledge higher voltage pulls less amps. Then the vesc took off. Problem is the vesc doesn't handle high amps for very long. It was designed for high voltage/low amps. Cogging occurs primarily only at start up without a sensored set up. If it happens anyother time after spin up there are other problems to look for. Inefficient gearing and an under powered system would more likely be to blame. If your gun has enough slack to allow your motor to spin initially you may find sensorless sufficient. If not, talk to @mccloed. He's been getting good results putting sensors on that specific motor.
```

---
## \#7 Posted by: SufficientlyAdvanced Posted at: 2016-02-08T00:03:26.377Z Reads: 69

```
Ah ok, I'll be sure to allow the motor to spin up first without load. I do really like everything people have been saying about VESC, but yeah, the lowish amp rating might keep me away. It seems the second best might be the Torqueboards 12S ESC, but I haven't found many reviews or first hand accounts.
```

---
## \#8 Posted by: psychotiller Posted at: 2016-02-08T00:06:50.134Z Reads: 63

```
I haven't used a Torque 12s esc so I can't give a worthy review. Believe they are made by FVT though.
```

---
## \#9 Posted by: laurnts Posted at: 2016-02-08T00:16:14.001Z Reads: 63

```
I have experience with Turnigy Sentilon 100A HV ESC. This ESC have been tested by an MIT master student to have the amazing low speed torque that are able to draw 90A - 100A stable continuously in open air box. But again having abit of slack in the rope as well as getting it descent speed help boost the power can be output by the motor.

Brushless motor definitely has the ability to output more power than drill which is brushed motor with lower voltage and battery burst. So if one person could made it with brushed motor electric drill, theoretically it's possible to do with big brushless motor without problem. Drill uses planetary gear with quite high gear ratio. Just make sure you tune down your ratio, would be fine to go.

Rotating / going with full speed (12S) on brushless motor help brushless motor draw more amps easier, hence it helps burst the power of the motor.
```

---
## \#10 Posted by: SufficientlyAdvanced Posted at: 2016-02-08T00:47:12.674Z Reads: 60

```
Awesome, I had read mixed things about the Sentilons, but the price is pretty nice. I'll read up some more.
```

---
## \#11 Posted by: laurnts Posted at: 2016-02-08T03:20:57.454Z Reads: 57

```
Well Sentilon are straight forward robust ESC. No fancy features. It doesn't even have nice slow brake. Either brake or not braking at all. Personally I think it's quite perfect for your test since it's not as expensive as VESC (but again it's your choice and I don't want to be blame if it doesn't work). You dont need regen braking, you don't need FOC (silent operation, but not optimized yet), you don't use nunchuck control, etc. The only thing that I am worried about the build (from your youtube video) is that when you start climbing up / down, there is no way of stopping in the middle. You will need to have mechanical brake to lock your self at certain position, it's because electronic brake are not powerfull enough to get you a static full stop.
```

---
## \#12 Posted by: Hummie Posted at: 2016-02-08T05:09:21.478Z Reads: 53

```
I skipped all the math not understanding but looking to find out what you need.  You need torque. 2 Newton meters is within the motors abilities without any gearing but putting a big load on it without it already spinning sounds bad.  Maybe you could put a planetary gear on it and keep under the amp max of the vesc and also you have the stealth factor of the vesc, which any super hero using such a device would appreciate.
```

---
## \#13 Posted by: trbt555 Posted at: 2016-02-08T08:23:19.676Z Reads: 51

```
Basic feasibily from a physics standpoint: to lift a mass of 100kg up 10m within a 30sec timespan (0.33m/sec) you need a theoretical power of 327W. E-board sized brushless motors are an order of magintude more powerful so it should certainly be feasible, even if you take all losses into account.
I think your detailed math checks out. Your username is fitting ;-)
One caveat: your entire logic is based on a "Chinese" max current rating of 70A and nobody knows how reliable this figure is.
I don't think you'll be hitting max Amps, your 22A estimate seems about right with the figures you posted. 
A VESC with a decent heat-sink would probably do the job.
Basically the cogging happens when commutation is off due to the unknown position of the rotor when starting from standstill. In order to determine the position of the rotor you need BEMF so it needs to be moving...
The VESC has pretty advanced algorithms to cope with this. 
A sensored motor is better in this respect, because your controller knows where the rotor is at any given point.
I think you could get around the cogging/spinup issue by allowing the motor to take op slack in the line before lifting off.
If I were you I'd definitely design a ratchet system onto the winding pulley, just in case anything fails.
```

---
## \#14 Posted by: SufficientlyAdvanced Posted at: 2016-02-08T08:51:10.549Z Reads: 48

```
Thanks! It's the name of my Youtube channel, after the Clarke quote of course. I've been lucky enough to have a couple viral hits now, so hopefully this grappling gun continues the trend (and I can continue paying rent!)

I'm still playing around with the gearing, but I think I'm pretty settled on the 149 Kv motor and a 100 A Sentilon. With 30 ft of line, I should have enough slack to reel unloaded line in for start up. A ratchet might be a good idea, I was sort of hoping that braking would slow down my descent, but if the ESC blows I suppose I won't have that...
```

---
## \#15 Posted by: trbt555 Posted at: 2016-02-08T11:05:02.703Z Reads: 45

```
Just a quick sanity check: are you really willing to use cheap Chinese hobby electronics to lift yourself to a height that will kill you if you fall ? Will you have any other form of safety line ?
```

---
## \#16 Posted by: SufficientlyAdvanced Posted at: 2016-02-09T20:10:50.370Z Reads: 40

```
For the first few tests I'll probably set up a belay line, but ideally I'll be able to manage with just a crash pad. That ratchet idea is starting to sound better and better :smile:
```

---
## \#17 Posted by: locktight Posted at: 2016-02-09T20:20:55.405Z Reads: 41

```
hey @SufficientlyAdvanced, are you the sufficiently advanced from youtube who made the light saber and the mjolnir?
```

---
## \#18 Posted by: SufficientlyAdvanced Posted at: 2016-02-09T20:44:26.957Z Reads: 40

```
Yup, that's me! Hopefully this build does as well as those did!
```

---
## \#19 Posted by: lowGuido Posted at: 2016-02-09T20:57:39.820Z Reads: 39

```
Did you see the episode of mythbusters where they did this?
make sure you don't do what Jamie did and not include a release/reverse. He winched himself to the ceiling and couldn't get down!
then he had to cut the line and he clocked himself in the face with the winch as it released from the cut line!
```

---
## \#20 Posted by: locktight Posted at: 2016-02-09T21:12:30.578Z Reads: 40

```
https://www.youtube.com/watch?v=4OyoWAZEcIE this guy did something simmilar to what you want using parts from a cordless drill. he goes over in detail what he did to make it in the video.

Hope it helps, Hans
```

---
## \#21 Posted by: Hummie Posted at: 2016-02-10T22:31:02.916Z Reads: 38

```
Super cool. You're famous with your lightsaber.  I'm very disconnected and still saw a bit of that video.  I think it's a giant butane torch.  And the hammer is awesome!  
youre viral. Hope they're paying more than the rent.  Steve Harvey apologies again in your lead-up commercial. That's also about the only thing I know about in the news. Can't believe they employed him to do the pageant...he is a comedian foremost and his "blunder" seems to be paying off for him.
```

---
