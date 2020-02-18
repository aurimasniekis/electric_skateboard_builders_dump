# Dynamic truck angle based on current speed for stability

### Replies: 39 Views: 946

## \#1 Posted by: Noah Posted at: 2019-03-29T02:51:00.105Z Reads: 260

```
Has anyone brought up the idea of dynamically changing the angle of the truck to increase the radius of the maximum turning capability as speed increases in order to increase stability at high speeds and retain a good turning radius at low speeds?
```

---
## \#2 Posted by: morrisxyz Posted at: 2019-03-29T03:03:19.213Z Reads: 256

```
I'm just imagining hydraulic skateboards with huge subwoofers bouncing down the street. 😅
```

---
## \#3 Posted by: Noah Posted at: 2019-03-29T03:04:40.822Z Reads: 251

```
I feel like your insulting me but the image is so cool I'm going to let it slide.
```

---
## \#4 Posted by: MoeStooge Posted at: 2019-03-29T03:43:00.490Z Reads: 235

```
This needs to be made.
```

---
## \#5 Posted by: Dirt_Bag Posted at: 2019-03-29T03:58:51.912Z Reads: 234

```
ive never heard of something like that, but this topic might help you if your looking for stability and speed balancing

https://www.electric-skateboard.builders/t/split-truck-angles-wtf-are-they-and-why-should-i-care-and-other-stuff-about-trucks/57929
```

---
## \#6 Posted by: Noah Posted at: 2019-03-29T04:03:33.018Z Reads: 227

```
thank you i will read that
```

---
## \#7 Posted by: meesie Posted at: 2019-03-29T08:51:59.162Z Reads: 211

```
that is a fecking amazing idea. i've always tried to make a board that has a decent turning radius whilst aso being stabe at high speeds. i've used wedges and intricate bushing combo's and i kinda succeeded, but damn this idea is amazing.
```

---
## \#8 Posted by: Okami Posted at: 2019-03-29T08:56:53.097Z Reads: 206

```
I think ackermann steering / steering rods and so on is better direction. Or just simple dampener.
```

---
## \#9 Posted by: lrdesigns Posted at: 2019-03-29T09:00:09.508Z Reads: 203

```
One of these base plates. 

![image|690x363](upload://1yNUy397AJfymmJCgKSMjTePIus.png) 

Connected to a large servo

![image|484x450](upload://suzJbSJ5SzBNA2NXGkXKZk40oRK.jpeg) 

Connected to an arduino

![image|413x181](upload://8SzF4qA0VYUZeTWHviangBJPTME.jpeg) 

Connected to a vesc to read the speed could work. :thinking: 

![image|690x372](upload://2zaS7XXXLCg3yhWx6IrW2zgDipH.jpeg)

***plus a high amp regulator for the servo
```

---
## \#10 Posted by: meesie Posted at: 2019-03-29T11:12:51.534Z Reads: 183

```
you'd have to take your motormounts in consideration too though. if you turn the truck your motormount will move along too. i think this will work best with directdrive or hubs.
```

---
## \#11 Posted by: sk8l8r Posted at: 2019-03-29T11:36:42.794Z Reads: 178

```
[quote="morrisxyz, post:2, topic:88645"]
hydraulic skateboards
[/quote]

hmmm..... hydraulic assisted ollies :smile:
```

---
## \#12 Posted by: Noah Posted at: 2019-03-29T13:03:10.790Z Reads: 172

```
I was thinking it would make sense to have the pivot point on the board itself just behind where the trucks are mounted because then it would slightly bring the board lower to the ground as speed increased as well.
```

---
## \#13 Posted by: AlanZhou Posted at: 2019-03-29T13:19:56.720Z Reads: 168

```
Maybe surfrod adjustable baseplate with a motor?

It takes a lot of force to move a base plate with a human on top
```

---
## \#14 Posted by: ducktaperules Posted at: 2019-03-29T15:18:24.565Z Reads: 167

```
rather than switching truck angle you could just switch to electronic steering.
This is how most modern cars work by making the steering less responsive at higher speeds, if done well no one can even notice. This would mean that you would not need to lean as for to get sharp turns whilst going slowly. 

Additionally there could be the option to transition to 2 wheel steering at higher speeds for increased stability.
```

---
## \#15 Posted by: Darkie02 Posted at: 2019-03-29T16:06:15.853Z Reads: 158

```
Think a liner actuator instead of a servo might be better suited to a tilting hanger. But if you want really tight terns a vertical pivoting base plate on a tilt senser that only activate below say 5kmh might work. I think there will be a lot of play in any system like this and that will be counterproductive to any high speed stabalastion you gained by a lower truck angle. Going to need machining with super low tolerances. Interesting idea pleas keep us posted with pictures of how you get on.
```

---
## \#16 Posted by: Okami Posted at: 2019-03-29T16:39:03.159Z Reads: 156

```
https://www.electric-skateboard.builders/t/trampa-truck-steering-dampening/38970

@Nowind also used one and a few others as well.. though someone should jump in who has first hand experience on this

I know someone even mounted linear dampener on street board
```

---
## \#17 Posted by: Ckarg Posted at: 2019-03-29T17:25:40.973Z Reads: 144

```
I feel like @MoeStooge NKP 3-link trucks would be a great base for this idea. You could have a rod between the link and move that to achieve the desired angle. The tricky part would be software side and determining the desired angle to speed.
```

---
## \#18 Posted by: CHAINMAILLEKID Posted at: 2019-03-29T17:52:06.613Z Reads: 150

```
This is something I've wanted to do for YEARS, actually been meaning to make this topic for a while too.

I think more than stability the advantage could be just extreme maneuverability at low speeds, because I don't think you'd really want to cut your pivot angles at speed as much as you'd think.

The main thing is you'd need to have it so the roll axis stays at the same height so that you're not lifting the rider up/down, which would greatly reduce the torque needed.
But you'd also want a system with very little lashback.

OR, maybe you do want the roll axis to change for some reason. You can change more geometry than just the pivot angle if you want. But for starters better to keep it simple.

I would also want to just make it a standalone system, and not part of a normal eskate, again, just to keep it simple.
```

---
## \#19 Posted by: Noah Posted at: 2019-03-29T18:49:15.428Z Reads: 140

```
Another consideration is the fact that if your lowering the deck and changing the angle as speed increases you could probably figure out a way to utilize all of the braking energy to bring the board back up and change the truck angle back at low speed instead of not being able to send all the power back to the battery because of amperage limiting for battery health.
```

---
## \#20 Posted by: Flexboardz Posted at: 2019-05-12T11:34:33.053Z Reads: 120

```
Why not making a bold step out of the box and dump the old trucks and its horrible lean/steer relationship + rigid axle which are instable by design.

You won't bring an horse cart to the moon, even with hydraulic and electronic assistance !!
```

---
## \#21 Posted by: MD84 Posted at: 2019-05-12T12:37:48.816Z Reads: 113

```
@skatardude10 uses a hydraulic steering dampener. How about a speed regulated spool valve that dynamically changes the hydraulic resistance of the dampener based on speed. Only on the back truck.
```

---
## \#23 Posted by: Flexboardz Posted at: 2019-05-12T14:00:43.505Z Reads: 105

```
sorry, let's call it a board, on wheels, to make the difference with toys.
```

---
## \#25 Posted by: Flexboardz Posted at: 2019-05-12T15:58:52.811Z Reads: 93

```
Agree 100% for the board definition, you lean to turn....and not to slide or wobble.

And it doesn’t need to be on skate truck + wooden plank.
```

---
## \#27 Posted by: rusins Posted at: 2019-05-12T16:49:54.712Z Reads: 93

```
[quote="Deckoz, post:26, topic:88645"]
ya know move the location of the axles
[/quote]

This is genius! We just make the board out of stretchy urethane, and put the drive chain in front. When you accelerate, the board stretches, giving you a longer wheel base and thus more stability, and when you brake the board shrinks and gives you good maneuverability! Someone, quick, patent this!!!
```

---
## \#29 Posted by: rusins Posted at: 2019-05-12T18:00:58.699Z Reads: 81

```
Ya win some ya lose some ¯\\\_(ツ)_/¯
```

---
## \#31 Posted by: Tangent Posted at: 2019-05-12T18:45:43.006Z Reads: 79

```
You hit on something here, and I'd love it explained to me, as I see it, currently we run positive caster and positive trail on the front end, which is good for stability, but negitive castor and leading trail on the rear, which is bad for stability. Would running rkp up front, and a tkp in the rear address this? @Deckoz
```

---
## \#32 Posted by: Flexboardz Posted at: 2019-05-12T18:52:06.602Z Reads: 78

```
Agree but skate trucks have non linear steering (relationship between lean angle and steering radius)

...and sadly, it's very reactive around 0 degre, which is the main wobble cause.

Making a truck "under reactive" around 0 degres (to swallow small feet mistakes or ground irregularities without steering too much) and yet able to turn tight at strong leaning angle would be a great idea.
```

---
## \#33 Posted by: treenutter Posted at: 2019-05-12T18:55:37.601Z Reads: 83

```
A long time ago there was some discussion about dynamically adjusted bushing durometers. I went as far as searching for a material that has similar properties to urethane, but could change duro with electrical input. I could never find anything like that. 

[quote="treenutter, post:1, topic:389"]
A system that identifies high acceleration and automatically stiffens the bushings would be an ideal solution.
[/quote]

from:
https://www.electric-skateboard.builders/t/speed-wobble-is-real/389
```

---
## \#34 Posted by: RedBaron Posted at: 2019-05-12T19:07:33.260Z Reads: 80

```
I think this is a cool idea, but the added weight and complexity let alone the maintenance costs are too much. I got into esk8 because of how simple the concept was and relatively cheap to have reliable alternative transportation. Not that there wouldn't be a market for your idea though.
```

---
## \#35 Posted by: Tangent Posted at: 2019-05-12T19:11:06.240Z Reads: 79

```
This ties in with what @Flexboardz is saying, but he put it wrong, the steering is definitely linear, i.e. for x amount of lean you get x degrees of turning, but the force required to initiate the change in turning increases with angle, with the least amount at force required at zero degrees, also with the least amount of damping.
There are electrically changeable fluids that could be used in a damping system, and are used in some car systems, but that would mean switching to a spring and damper solution.
```

---
## \#36 Posted by: Flexboardz Posted at: 2019-05-12T19:41:31.069Z Reads: 75

```
Sorry but no, the skate truck lean/steer relationship is not linear at all ( there is an Atg in the lean/steer formula) otherwise, trucks would be much better.

Ideally, a non linear lean/steer would be better if non reactive around 0 degre and more reactive at higher angle to get the necessary turning radius.
```

---
## \#37 Posted by: Tangent Posted at: 2019-05-12T19:55:25.449Z Reads: 75

```
No, you're right, what I meant was that the steering response is mappable by single function. I'd love to see that lean/steer formula, got a link?
```

---
## \#38 Posted by: Flexboardz Posted at: 2019-05-12T20:39:02.258Z Reads: 72

```
It's a bit late here but I will dig in my files to find and post it tomorrow ( and please, remember than I'm not a truck passionate )
```

---
## \#39 Posted by: CHAINMAILLEKID Posted at: 2019-05-12T20:42:15.007Z Reads: 73

```
Steering is not exactly linear.
Depends on how nitpicky you want to be.
I would definitely describe it as linear to 95% of people.

But in reality, its not.
For one thing, slop. It eats away turning so you don't get that perfect relationship.

Also, slightly related but not exactly. a 5 degree wedge doesn't affect turning the same amount on a 45 degree baseplate as it does on a 30 degree plate. I'm not the best at applied math like I wish I was, so I can't go into detail about that, but making a dynamic angle truck would have to have that relationship all mathed out.

Also, here's a link which has maths.
https://nelsonlongboards.com/blogs/blog/80421639-different-wheelbase-same-turning-radius-dial-in-your-next-setup-with-the-power-of-math#ihatemath
```

---
## \#40 Posted by: Leonhart Posted at: 2019-05-14T08:19:31.340Z Reads: 65

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#41 Posted by: Flexboardz Posted at: 2019-05-14T18:05:22.122Z Reads: 67

```
Thanks !! This site should be the holly bible of all skaters as it tells everything about truck technology!!

And you can see on screen capture below how non linear it is (over reactive, indeed). 

For a 50 degree pivot angle, 1 degree lean causes a 50ft radius curve (ie a medium curve), 2 degrees cause a 25 ft curve (tight if you are fast), 3 degrees for 18 ft, 4 degrees for 12 ft (ie a Uturn radius).... and .... visualize that 1 degree angle, on a 10" wide deck means moving our toe tip by 2mm on deck edge!! Touchy! 

In addition, if someone want to design the "ideal truck", it's better to have a non linear behaviour, ie non-reactive around zero degree (fast speed) and more reactive at deeper angle to be turny enough at low speed.

Last, a +-10 degrees tilting range is very "narrow band"  to transmit all ours riding information through feet...

![Capture%20du%202019-05-14%2019%3A08%3A23|685x500](upload://gjFtkfHWlSNElhtMib61XcP4AIS.png)
```

---
## \#43 Posted by: rusins Posted at: 2019-05-14T20:24:46.322Z Reads: 56

```
While split angle trucks are definitely an option, a lot of people prefer the center of the turning radius being in line with the middle of the board, rather than the back. Having the front truck angle too big in order to compensate is especially problematic when pushing, because it's too easy to accidentally steer to one side.
```

---
## \#46 Posted by: MoeStooge Posted at: 2019-05-15T19:45:44.750Z Reads: 54

```
I'd hit the solved button if their was one available.
```

---
## \#47 Posted by: taz Posted at: 2019-05-16T05:44:43.459Z Reads: 45

```
Like riding a  bike :rofl:
```

---
