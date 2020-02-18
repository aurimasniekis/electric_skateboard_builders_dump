# Custom Ram Air for cooling

### Replies: 80 Views: 4114

## \#1 Posted by: oldguy Posted at: 2017-07-09T20:21:29.870Z Reads: 444

```
Traditional Ram Air dama and systems  function to feed more air to a combustion engine to increase output. In my case, it is a little different… 
So... my old enclosure was about 1/4 inch shorter than this new one. Apparently the old one allowed just enough air to flow over top of the motor to keep it from getting too hot. The new enclosure blocks that airflow and the motor heats up pretty good. So, I had to develop a ram air system to restore airflow to the motor. Here is this afternoon's invention…

<img src="/uploads/db1493/original/3X/7/b/7bf5c465d8943b5bb795c24b1f22254c444319f9.jpg" width="281" height="499">
```

---
## \#2 Posted by: oldguy Posted at: 2017-07-09T20:22:39.017Z Reads: 423

```
 Does anyone else do something to help keep their motor cool?
```

---
## \#3 Posted by: Okami Posted at: 2017-07-09T20:26:40.336Z Reads: 419

```
yeh, ive seen people printing a fan for it and then attaching it on outside.. 

I printed it but it didnt fit.. later on I concluded the motor barely needs colling unless going up hill constant.

https://www.thingiverse.com/thing:1705363

--

Though I totally dig your 'solution'.. looks very unique, sort of like steam punk design :D im sure if you added some paint to the tubes it might look badass
```

---
## \#4 Posted by: Michaelinvegas Posted at: 2017-07-09T22:15:56.475Z Reads: 401

```
Add ice for extreme conditions 

https://youtu.be/Vx5-3M0hvTc
```

---
## \#5 Posted by: oldguy Posted at: 2017-07-09T22:27:21.487Z Reads: 383

```
I think I'm going to start experimenting with some peltier devices
```

---
## \#6 Posted by: bbq870 Posted at: 2017-07-10T00:12:30.516Z Reads: 383

```
wow! this looks awesome! if you would 3D print a funnel to combine the pipes it would have a larger area of AIR-INTAKE.


 my concerns:
if there are no internal fans involved, this rather blocks the airflow, than increasing it. - air is a tricky thing.

my guess here:
-the whole construction itself is shielding the motor from the natural airflow. 
-the air will not be collected and directed to the motor. with all those windings it might NOT even FLOW through the hoses and rather stop inside
(just guessing)
<img src="/uploads/db1493/original/3X/4/7/47a413329d6d991a6d8ebbc74b0f01df4807f54f.png" width="690" height="401">
```

---
## \#7 Posted by: oldguy Posted at: 2017-07-10T00:37:55.413Z Reads: 360

```
 I think you are pretty spot on. I have begun looking for something very similar to exactly what you drew. I would mount it at the tip of the board on top and then run it to a T-junction  below. I was also looking for some small fans I might be able to mount in front of the openings, or even a fan and  Peltier  Device that would generate cooling at 12 V DC. 
 It is also conceivable that the only reason I am experiencing heat issues over the last two days is because it's hotter than hell outside. Almost 100.
```

---
## \#8 Posted by: oldguy Posted at: 2017-07-10T01:15:03.263Z Reads: 339

```
I do believe that my enclosure is already blocking airflow, which is why I only started having this problem after installing it.
```

---
## \#9 Posted by: Okami Posted at: 2017-07-10T05:31:11.954Z Reads: 334

```
An orthodox solution would be to run the board with motor in front.. though the braking then is a bit tricky, if you apply too much braking force..

Otherwise.. if heat really is an issue, and you got time to remake enclosure, maybe I would have made it in a way there is a 'channel' for air to travel to the motor. This would require that there are 2 parts of enclosure probably but if you are using lipo bricks, I think this should not be as a big problem as it would be, if you had one flat li-ion pack installed.

And yes.. to be honest, a direct fan at the motor of some sort does not sound like a bad idea to save some time by not modifying enclosure but by a burning off a few watts in battery life for cooling.
```

---
## \#10 Posted by: TarzanHBK Posted at: 2017-07-10T09:07:24.819Z Reads: 320

```
before you spend more money in new parts for cooling, simply buy a bigger motor.
It´ll stay cooler and you don´t need to put on strange looking toilet tubes ;)
```

---
## \#11 Posted by: lowGuido Posted at: 2017-07-10T09:52:42.321Z Reads: 314

```
I think you would be better of making a fan that bolts to the motor can. Something like this. 

<img src="/uploads/db1493/original/3X/2/4/2414129a373acd1981e80e06bb711105eaf925de.jpg" width="200" height="200">
```

---
## \#12 Posted by: mwkeefer Posted at: 2017-07-10T10:38:36.989Z Reads: 311

```
Come on.... just strap on a 2.5 pound tank of liquid nitrogen, that'll do the trick :)

-Mike 

(Sorry had to)
```

---
## \#13 Posted by: Cobber Posted at: 2017-07-10T11:36:24.751Z Reads: 298

```
A front brake is maybe twice as effective as a rear brake. So if I only had one, id rater a front brake. Front wheel drive over rear wheel drive sucks but...
```

---
## \#14 Posted by: longhairedboy Posted at: 2017-07-10T11:54:46.725Z Reads: 306

```
[quote="oldguy, post:5, topic:27172, full:true"]
I think I'm going to start experimenting with some peltier devices
[/quote]

make sure you have somewhere for the heat to go. Peltiers get really, really warm on the hot side. I've got some coming in at some point, i ordered them a couple months ago. We were going to tie the cold side to the focbox and the hot side to a heatsink that's exposed to outside air and see if we couldn't crank up the output a little. 

SK3s have a built in fan. Maytech, R-Spec and my motors blow quite a lot of air due to the centrifugal fan behavior of the mag wheel looking end caps. They get warm and even hot on occasion but it seems to have little effect on anything. 

We put a scoop on them once but ended up getting crap clogged in it. 

I'm pretty sure its totally not worth it though to do peltiers, but it will be fun to try and come up with something. 

I'm interested in heatpipes actually as a more realistic ESC cooling solution. Scoops and fans though.. there's defeinitely something there for the motors. Yuneeq had that fan on thier e-go motor.
```

---
## \#16 Posted by: oldguy Posted at: 2017-07-10T14:51:23.163Z Reads: 288

```
Yeah - I've wanted the peltiers for a home-made cooler anyhow, so while I don;t expect to find a very practical use for them on the board, I was ordering anyway.
 I also thought that for $15 I might give this a shot as a way to push air into the pipes...

It's only 42mm.

http://www.ebay.com/itm/Performance-Air-Box-Filter-Motorcycle-Scooter-Go-Kart-GY6-49cc-50cc-RED-H-AF32/380675288367?ssPageName=STRK%3AMEBIDX%3AIT&_trksid=p2055119.m1438.l2649
```

---
## \#17 Posted by: oldguy Posted at: 2017-07-10T15:00:59.435Z Reads: 282

```
Unless I can get some serious airflow pushing through there and can make a noticeable difference in the temp of my motor after a 5-mile run I may disassemble the whole works. This is just what I did as an afternoon project tinkering with what I had lying around. I'm not even sure that the temp the motor is getting to is dangerous for it, I just know it is hotter than it used to get when I was using my slightly shallower temporary enclosure. The normal operating temp for my motor is 120-130 degrees. Mine doesn't get too hot for me to touch it, but if I left my finger there for more than about 6 seconds it would start to hurt. 
  I guess there is also a little plastic fan inside this motor? I suppose I should see if that stopped working somehow (or is turning in the wrong direction)...I don't know exactly where it is, but I'll look for it tonight before I ride.
```

---
## \#18 Posted by: evoheyax Posted at: 2017-07-10T17:11:19.713Z Reads: 272

```
I've been toying with an idea of water cooling for a while now. For example, a sealed hub motor with water cooling... But it's risky, so... Might be a while before I try that one, haha.
```

---
## \#19 Posted by: jaymu86 Posted at: 2017-07-10T17:15:13.093Z Reads: 263

```
Oh man had a flash back to how we used to keep the grow room cool haha
```

---
## \#20 Posted by: longhairedboy Posted at: 2017-07-10T17:32:00.903Z Reads: 253

```
just keep a squirt gun handy and crouch down and spray the motors now and then while you ride.
```

---
## \#21 Posted by: evoheyax Posted at: 2017-07-10T18:53:35.452Z Reads: 243

```
haha, one solution. I might need a really big squirt gun, cause I get motors HOT.
```

---
## \#22 Posted by: longhairedboy Posted at: 2017-07-10T18:54:08.798Z Reads: 216

```
single drives? heavy rider? or both?
```

---
## \#23 Posted by: evoheyax Posted at: 2017-07-10T18:57:23.700Z Reads: 228

```
I ride 4wd, but hills, I weight around 205 these days + a 20 pound backpack (textbooks, laptop, ect.), I ride aggressively... Did I mention hills? lol. I also like to stay above 25 mph as much as possible, which with GG park, that could be a few miles at a time. And we saw recently how wind resistance really is a huge factor at high speeds.

It's also cause these motors are just too damn small, as much as I like the fact that I have a motor fully enclosed in an 80mm wheel that to most people who ask, have no idea my board is electric. They mostly ask why my boards so thick, lol.
```

---
## \#24 Posted by: longhairedboy Posted at: 2017-07-10T19:00:34.234Z Reads: 221

```
what size are your motors? 50's or 63's? What voltage are you running?

Just curious because no matter how fast i go, i can still hold my hand on my motors, they're never too hot to keep my hand on. Even in 101 degree weather. To be clear i do not try to hold them while travelling at 25+ mph. I usually wait until i stop to grab them.
```

---
## \#25 Posted by: evoheyax Posted at: 2017-07-10T19:06:49.838Z Reads: 213

```
50mm. They are hummies small motors. New one's will have a stator twice as long, and heat shouldn't be as much of an issue. But they won't have as simple of a look IMO.
```

---
## \#26 Posted by: longhairedboy Posted at: 2017-07-10T19:12:31.920Z Reads: 208

```
ahhhhhhh now it makes sense. I was wondering why your motors were working so hard. 

hubs man. That mechanical disadvantage generates a fuckload of heat. But they do look clean on a board.
```

---
## \#27 Posted by: evoheyax Posted at: 2017-07-10T19:16:54.264Z Reads: 205

```
I think the 24 tooth stator might be the real solution. Need to do more testing, but it might be why enertions and jacobs hubs ran much cooler, at least at slower speeds.

I know your still on belt and pulleys, but I think one day soon, they'll be real solutions to the problems hubs have today, some of which I'm sure the raptor 2 hubs have already fixed.
```

---
## \#28 Posted by: longhairedboy Posted at: 2017-07-10T19:25:56.694Z Reads: 207

```
true. But untill i can change ratios on a hub, i'm not doing it. 

When i come up with my hubs, swapping KV will be a feature. Hopefully i can have modular hubs that let me swap stators. That's the real dream right there. 

I deal with people who write me and say "i'm 220 pounds and i want to climb hills in virginia." that guy doesn't need hubs unless i can drop them down to maybe 60kv and have a stator as long as my dick or steal somebody's raptor two hubs. Belts? no problem. 14/36 or 15/37 will get him up a damn hill all day long on 6355s and all i have to do is swap a pulley. 

Its hard sitting here waiting for what i need. Building customs is a challenge because of shit like this.
```

---
## \#29 Posted by: evoheyax Posted at: 2017-07-10T19:30:58.193Z Reads: 191

```
It's true. Theres less convenience on hubs. I think 4wd with hubs is really a great option. Expensive, but VESC prices are dropping ,and will continue to drop. And considering I can get a motor little motor for less than $100, I could in theory build an a small 4wd hub board for around $1000 USD, without labor and the other BS involved like taxes.

With 80 kv and 4wd, I climb 20% grade hills at 20 mph. Tons of torque, and I can still get up to almost 30 mph.
```

---
## \#30 Posted by: longhairedboy Posted at: 2017-07-10T19:44:58.251Z Reads: 184

```
listen to me talk smack about hubs when i just sent a home wrecking sized wire transfer to Slovenia for an NGV system for a customer's build.
```

---
## \#31 Posted by: Jinra Posted at: 2017-07-10T19:48:09.800Z Reads: 185

```
Unless you're skidding, a front brake is not twice as effective as rear brakes. Under very hard braking you may skid though, making a front brake a tad more effective.
```

---
## \#32 Posted by: Cobber Posted at: 2017-07-10T20:03:10.082Z Reads: 186

```
for a simple test you can try at home hope on a motorcycle or push bike and measure your stopping distance using either brake...

I see you quoted the first reference from google on the topic, funny how the second reference states that: " The front brake assumes around 75-90% of the braking power"

It is simple physics you just can not get your weight behind the rear wheel to optimize traction.
```

---
## \#33 Posted by: Jinra Posted at: 2017-07-10T20:06:30.375Z Reads: 179

```
I didn't quote anything. This is based off real world experience
```

---
## \#34 Posted by: t0m_r1dd1e Posted at: 2017-07-10T20:07:50.060Z Reads: 170

```
Front brakes on motorcycles are physically much larger....
```

---
## \#35 Posted by: Okami Posted at: 2017-07-10T20:23:11.034Z Reads: 176

```
Yep, agree, I also read about this and it seems like even regular bicycles with disk brakes incorporate this feature - the front wheel brake disc is just physically larger too.. I heard it somehow takes up more heat also = more braking force/power.
```

---
## \#36 Posted by: t0m_r1dd1e Posted at: 2017-07-10T20:28:45.779Z Reads: 176

```
Yep. And you need more braking power up front on a motorcycle where you don't have as much weight on the rear and the tire can lock easily. But I've never had the rear wheels on my longboard lock... Maybe if you had a single 6374 on a 15mm belt it could be an issue.
```

---
## \#37 Posted by: jrpwit Posted at: 2017-07-10T21:36:05.222Z Reads: 183

```
This is so funny that this thread popped up just now. I actually accidently killed my vesc last week because of the heat. I live in Arizona and rn is like 115° F in the afternoon. Anyways I decided to ride to work (14 mile trip) and my board started to cut out on my about 6-8 miles in. 

I have had to stop and let the esc cool off before on long trips. I assume that the esc gets so hot that it limits the current running through it.

So after stopping a couple times I decide to take off the back half of my case where the vesc is to possibly let it get some air cooling. However I thinks some of my sweat fell on the vesc and I heard this pop and there was a flash from underneath esc. Anyways it won't turn back on and I am looking into the vesc 6 despite its high price tag. 

BTW I run single drive with a tacon 245kv and 10s4p. Also I was very late XD
```

---
## \#38 Posted by: jrpwit Posted at: 2017-07-10T21:37:53.630Z Reads: 174

```
Also my front truck gets pretty hot and there isn't even a motor attached to it
```

---
## \#39 Posted by: Jinra Posted at: 2017-07-10T21:39:44.871Z Reads: 171

```
[quote="jrpwit, post:37, topic:27172"]
I live in Arizona
[/quote]

That's the first problem I'd fix.
```

---
## \#40 Posted by: jrpwit Posted at: 2017-07-10T21:41:32.862Z Reads: 170

```
Lol maybe when I finish hs
```

---
## \#41 Posted by: Okami Posted at: 2017-07-10T22:03:08.451Z Reads: 169

```
hah bad luck, man .. wish you a good start with the new vesc  / controller once you get it.. so is your board now just sitting at home or something?
```

---
## \#42 Posted by: jrpwit Posted at: 2017-07-11T00:30:05.926Z Reads: 150

```
Yeah in the garage. Will be happy to try foc with a focbox. It has a heat sink which is awesome. Vesc 6 is just crazy expensive. Literally the same price as a good Kelley controller. Overall I was happy with my old enertion vesc worked great despite all the controversy when it came out.
```

---
## \#43 Posted by: oldguy Posted at: 2017-07-11T01:34:21.943Z Reads: 153

```
I would "like" that post, but that really sucks. Survived the heat and got killed by  your sweat. Believe it or not, here in Florida, I worried about that while working on my board a couple of times. It would just fall off my forhead and land on the board. A little to the left, or to the right, and right into a battery connector.  The threat is real.
```

---
## \#44 Posted by: oldguy Posted at: 2017-07-11T01:37:06.540Z Reads: 153

```
 I have come to accept that riding during the day in the summer defines most of my problem. Even if there is air passing over the  Motor, I don't know how much good it does when it is a stream of hot air.  For now, I have equipped whiteboard with lots of light and I do my daily rides after the sunsets. You know, when it is only 88°.
```

---
## \#45 Posted by: wmj259 Posted at: 2017-07-11T02:24:40.812Z Reads: 157

```
I'll try to design a stick on fan like the one posted earlier in the thread. Either way SK3's have a internal fan, mostly the 6374, maybe the 6364, but I didn't see one in the 6355s.
Also on my 6374, the motor gets warm. I can hold it and it won't burn but you'll notice it's warm.
```

---
## \#46 Posted by: oldguy Posted at: 2017-07-11T02:49:45.167Z Reads: 150

```
Mine's a 6354. It gets hot, but at a certain point it doesn't keep getting hotter. It's just a difference I noticed after putting on the enclosure. It is also conceivable that there are other variables at work. I am starting to become more confident and comfortable and I am probably riding a little harder and a little faster than before.
```

---
## \#47 Posted by: Cobber Posted at: 2017-07-11T02:55:04.851Z Reads: 154

```
Ok lets take the modern sport bike as a example. A super-sport bike is based on a racing motorcycle and entire categories are based on racing stock bikes. Don't you think they have squeezed every ounce of performance out of the bike as possible? If larger rear brakes would pull the bike up faster don't you think some one would have mounted a 330-300mm disk on the rear with a twin piston caliper like is used up front?
Rear brakes are 170-150mm with a single piston. Ant more and you lose modulation and just lock up the rear. The front on the other hand has 2 x 330-300mm disks with twin piston (thats 4 pistons all up) radial calipers. These are mounted in a radial orientation from the axle because so much force can be applied that a traditional mount to the fork leg binds and twists giving you brake chatter. 
Lets take another example, through the 60's disk brakes began to be used on cars as they were more powerful but expensive. They were only used on the front... by all means find even one example of a production motor vehicle that has a more powerful rear brake?
It is simple physics, there is just no weight behind the rear wheels to aid braking unless you are going backwards.
```

---
## \#48 Posted by: JdogAwesome Posted at: 2017-07-11T03:05:21.621Z Reads: 150

```
@oldguy @longhairedboy Peltier units are cool, no pun intended, but they are just so stupidly inefficient. Your only going to end up creating vastly more heat than if you just used a larger heatsink. Though it never hurt to try something new out, so why not! 

@evoheyax when I was originally designing my board I thought water cooling would be awesome as well, just overly complex lol.  Would love to see someone do that, may even try doing it as well one day. 

@jrpwit I was having some over heating issues with my VESc as well, after a long burst of acclearting or going fast my VESC would start to thermal throttle quite a lot and it was a problem especially when I wanted to go fast or get going. My solution was to add some small heatsinks to the MOSFET's on both sides as well as a small fan blowing right on them. The fan just blows the air around inside the enclosure, theres no port for ventilation, but it works plenty well and I haven't had any throttling problems since!
```

---
## \#49 Posted by: longhairedboy Posted at: 2017-07-11T03:08:28.024Z Reads: 145

```
[quote="JdogAwesome, post:48, topic:27172"]
Peltier units are cool, no pun intended, but they are just so stupidly inefficient.
[/quote]


Well of course they are. I'm going to put the hot side up top so i can keep my tea warm.
```

---
## \#50 Posted by: JdogAwesome Posted at: 2017-07-11T03:09:41.449Z Reads: 143

```
Your a genius! Never mind this is now incredibly efficient! Who has the noble prize in physics, give it to him now!
```

---
## \#51 Posted by: oldguy Posted at: 2017-07-11T03:10:47.251Z Reads: 147

```
 I would have to do some studying up on liquid cooling. I know very little beyond the physical concept. I'm assuming there would need to be a pump, and that the liquid is not just water but some kind of gel or anti-freeze type of chemical.  Then there is circulation and the biggest challenge of all, as it concerns the motor, is the fact that 90% of the body is rotating rapidly so afixing things to it is pretty much out of the question.  Still, philosophically speaking I am not opposed to  innovation for innovations sake.
```

---
## \#52 Posted by: JdogAwesome Posted at: 2017-07-11T03:14:01.980Z Reads: 145

```
Well for liquid cooling, at least in PC's which is im guessing what you'd adapt most of the parts from you usually just use water with some additives. Yeah the main can of the motor is moving, but not the ends of it, or how else could you mount the motor lol. And yes you just use a small 12v pump with a radiator somewhere. Not entirely sure were you'd want to put the rad cause they are very fragile.
```

---
## \#53 Posted by: oldguy Posted at: 2017-07-11T03:19:14.163Z Reads: 149

```
 I am wondering what kind of transfer I could expect by running it over the bracket and how likely  keeping that cool would translate to the motor. Particularly when I believe the majority of heat resides in and around the copper coils in side.  Now if I could invent a way to transfer temperature control across a magnetic field, then I would make a play for that Nobel prize myself!
```

---
## \#54 Posted by: oldguy Posted at: 2017-07-11T03:21:18.785Z Reads: 157

```
 I should probably mention that I do not possess a single molecule of engineering aptitude anywhere in my body. Give me a keyboard and I can accomplish almost anything. Give me tools and the best I could hope to accomplish is an eventual trip to the emergency room.  I only mention this because if my questions indicate I am not thinking about this in the correct way, it is probably because I am not.
```

---
## \#55 Posted by: lock Posted at: 2017-07-11T03:22:54.950Z Reads: 165

```
I did see this [on the APS website](http://alienpowersystem.com/shop/brushless-motors/wc80100-outrunner-brushless-motor-180kv-7000w-watercooled/) the other day.
> WC80100 Outrunner brushless motor 180KV 7000W **water cooled**

<img src="/uploads/db1493/original/3X/1/a/1afe50b61c001cef4ae651cc5af85c1003c62a5b.png" width="400" height="400">

80100 size, go on you know you want too 😉.
```

---
## \#56 Posted by: oldguy Posted at: 2017-07-11T03:23:56.001Z Reads: 159

```
Damnit. 
10 chars
```

---
## \#57 Posted by: JdogAwesome Posted at: 2017-07-11T03:24:10.550Z Reads: 158

```
I think you would see a decent temp drop as the coils are mounted to the stator and in turn the motor case which is mounted to the bracket that holds the motor in place. I would see how hot the bracket gets during a ride and if its quite hot I could see it being worthwhile. I think your best bet would be using some type of generic heat block from like eBay or AliExpress and mounting it to the motor mount.
```

---
## \#58 Posted by: oldguy Posted at: 2017-07-11T03:25:18.850Z Reads: 159

```
 I have felt, not measured with any kind of accurate device, the bracket at the same time as the motor and I would say it is nearly as hot, maybe a fraction less.
```

---
## \#59 Posted by: jrpwit Posted at: 2017-07-11T03:52:41.404Z Reads: 166

```
This talk of water cooling XD
"I'm going to overclock my esk8"
Not too difficult to setup for an esc but I don't know where you would put the radiator with it getting gunked up with dirt.

Cut up an old heat sink and found some paste. Hope to use them when I get my focbox!
<img src="/uploads/db1493/original/3X/7/6/76ba026f2fad7dcd9fc337753e2c7084d1eecb52.jpg" width="375" height="500">
```

---
## \#60 Posted by: Jinra Posted at: 2017-07-11T04:13:04.551Z Reads: 165

```
Glue one of those things on the lateral side of a motor and you gotta yourself a two in one solution. A heatsink for the motor AND wheel spikes to spike everyone else on the road.
```

---
## \#61 Posted by: JdogAwesome Posted at: 2017-07-11T04:37:21.828Z Reads: 165

```
You could in theory just use a length of copper tube instead of a radiator, would server the same purpose and be a lot more durable, seen people do it before with PC's.

Those heatsinks are pretty tall, this is what I use and they fit perfectly on my VESC.
<img src="/uploads/db1493/original/3X/8/4/8464a690c8b9a8da615467adb9dba93f16a3b33c.jpg" width="690" height="389">
```

---
## \#62 Posted by: wmj259 Posted at: 2017-07-11T05:02:57.775Z Reads: 162

```
Some laptops have copper tubing that's glued to the heat sink of the cpu and heat is transferred over to the exhaust fans. You could take those pipes and attach to the FETs.
```

---
## \#63 Posted by: hornet90 Posted at: 2017-07-11T05:08:33.059Z Reads: 159

```
Thats not bad just like a water cooled pc computer
It might work......
```

---
## \#64 Posted by: Jinra Posted at: 2017-07-11T05:14:22.817Z Reads: 163

```
Pic for anyone interested

<img src="/uploads/db1493/original/3X/3/8/3868a274a23b1a93274da4726e2bdceea9bde407.jpg" width="668" height="500">
http://www.electric-skateboard.builders/uploads/db1493/original/3X/7/e/7edfe1aa4a36c03f050b5af209779da3022fd546.jpg
```

---
## \#65 Posted by: JdogAwesome Posted at: 2017-07-11T05:27:39.095Z Reads: 159

```
Lol we use practically the same heatsinks, id through a little 30 or 40mm fan in there, helped a lot for me.
```

---
## \#66 Posted by: Jinra Posted at: 2017-07-11T05:30:33.956Z Reads: 154

```
pretty sure they're exactly the same! 30 pc "raspberry pi" heatsinks on ebay for like $2
```

---
## \#67 Posted by: JdogAwesome Posted at: 2017-07-11T05:31:18.488Z Reads: 154

```
idk I order SOOO much shit off eBay its nearly impossible for me to find anything lol.
```

---
## \#68 Posted by: Jellybean Posted at: 2017-08-29T06:12:38.280Z Reads: 147

```
A lot of those have liquid inside of them to make them heat pipes. They work by heating up the liquid with the cpu/gpu and then the liquid moves to the other end where the fan is to be cooled. The liquid then returns to the cpu/gpu and the process begins again. But because of how they work, they basically can't be modified in any way.
```

---
## \#69 Posted by: wmj259 Posted at: 2017-08-29T16:01:54.290Z Reads: 145

```
It basically depends of size and application, they can be reused but without bending or modification of the pipes. It would require making your build around this cooling system rather than having your cooling system built around your build.
```

---
## \#70 Posted by: darkkevind Posted at: 2017-08-29T16:05:09.050Z Reads: 144

```
Only fluid cooled laptops would have that and they require a separate pump to circulate the fluid.

Most laptops have passive cooling copper tubes with an active fan to extract internal heat.
```

---
## \#71 Posted by: Jellybean Posted at: 2017-08-30T00:13:39.199Z Reads: 143

```
I agree about the pump if we're talking about water-cooled. Most laptops that have the cooper tubes have a liquid inside of them that passively moves heat to the fan, no pump required. How they do it? I don't know, magic I guess. I just know they can't really be messed with and like @wmj259 said, the board needs to be built around the cooling system.
```

---
## \#72 Posted by: wmj259 Posted at: 2017-08-30T01:21:07.554Z Reads: 144

```
<img src="/uploads/db1493/original/3X/9/6/966df71122ab8f220ae8b21c7c71d003fd859809.png" width="281" height="500">
```

---
## \#73 Posted by: ugothakd Posted at: 2017-10-07T22:59:07.057Z Reads: 126

```
How hot are your motors actually getting? Brainstorming a bit, water is pretty much everywhere, you could device a small water drip into the motor. Basically exactly how sweat cools our bodies with evaporation you could cool the motor. It all might fling off at the speeds the motor goes
```

---
## \#74 Posted by: GhettoFab.rictation Posted at: 2018-02-27T06:56:56.994Z Reads: 100

```
I'm in AZ too, but I use 6374 sk3 192kv on 12s with vesc and I'm putting heatsinks on each mosfet with a fan on both sides of the vesc. The motor, I am trying to figure out airflow of and see if a fan is redundant or not because of resistance. The 6374 sk3 has a cooling system, but hard to tell if it is cooled using centrifugal force or by sucking up very little resistance and cooling the motor conserving the energy by reducing the heat with little resistance.
```

---
## \#75 Posted by: banjaxxed Posted at: 2018-02-27T07:29:19.611Z Reads: 100

```
You could vary the airflow with one of these
![IMG_8567|500x500](upload://jVY5uOKjawdGQCfmcys6HCTnjtq.JPG)
```

---
## \#76 Posted by: TarzanHBK Posted at: 2018-02-27T07:30:03.358Z Reads: 97

```
flush if too hot - easy
```

---
## \#77 Posted by: banjaxxed Posted at: 2018-02-27T07:33:33.515Z Reads: 99

```
The possibilities are endless![IMG_8569|500x500](upload://tjzpmjyuXBlMuuoqiCExN08eZXL.JPG)
```

---
## \#78 Posted by: TarzanHBK Posted at: 2018-02-27T07:35:07.815Z Reads: 97

```
take a small hub motor on this and you´ll have a automatic toiletpaper dispenser!
```

---
## \#79 Posted by: banjaxxed Posted at: 2018-02-27T07:37:58.858Z Reads: 98

```
Now that's an idea..and you can reroll if you take too much
```

---
## \#80 Posted by: pakue Posted at: 2018-02-27T09:47:53.150Z Reads: 93

```
Think bigger – you could motorise the wipe too ...
```

---
## \#81 Posted by: banjaxxed Posted at: 2018-02-27T11:41:08.930Z Reads: 90

```
Seriously though I have to agree with others, that motor is too small alone and that's very much contributing to the problem, either a second motor (meaning a second motor controller and pulleys/mount etc) or a bigger motor like a 6374 will take care of business.

But if you insist on this at least make it look nice :joy:

http://r.ebay.com/9EJial
```

---
