# Alanhunt123 &#124; 36&rdquo; Skateshred Deck &#124; Dual Racestar 5045 200kv Motors &#124; 10S4P 25r &#124; Dual FOCBOX

### Replies: 22 Views: 2618

## \#1 Posted by: Alanhunt123 Posted at: 2017-11-17T01:29:58.535Z Reads: 314

```
Hey guys, just thought I'd show off my latest build. Certainly not the fastest board out there, but I think it makes a decent cruiser.

<img src="/uploads/db1493/original/3X/d/c/dc46dc70c41ebd0bca3dec22a94b443e799c03ce.jpg" width="258" height="500">

Some of you may recall the crazy 8 wheel longboard I was making. Long story short, I kept running into issues with the 8 wheel all summer long, and it never felt like a finished product. So, I never posted anything about it. Now, the 8 wheel longboard can finally rest in peace. Here's a link to a post wrapping up that project. You can also see the process for making the recycled parts here: http://www.electric-skateboard.builders/t/8-wheel-build-36-kicktail-vesc-4-12-dual-om5065-200kv-2-2kw-10s-10ah-custom-enclosures/25708/24?u=alanhunt123

Many of the parts for this build came off of the 8 wheel, namely the deck (36" skateshred cheapy), the trucks (Paris 185mm), the battery ( custom 10S4P Samsung 25r), the custom sheet metal case I made for the batteries, and the FOCBOXs.

The FOCBOXs are housed in a custom enclosure that I milled out of aluminum. The inside has a copy of the original profile from the aluminum plate the ESCs came with built into the enclosure. This saves a bit of space and weight (also provides direct heatsinking to the environment. I'm sure that I could run 80A continuous if I ever wanted to).

<img src="/uploads/db1493/original/3X/5/4/545b2f5045a695bc82d77ffe9479f9bac2979e59.JPG" width="690" height="388">

The motors are the Racestar 5045s from Banggood, and they're pretty much the same thing as the 5065s from Ollinmotors, but with a shorter can. Banggood also sells 5065s for the same low price (around $41 each). I find these motors have plenty of power for a moderate speed setup for my 175lb. Certainly not going to win any races against some of the other builds on this site, but it's plenty of power for me. They're mounted to some custom CNC motor mounts that I made. They are a single piece that has a circle cut out that is the same diameter as the trucks. I drilled a small indent into the trucks, and put a set screw with red threadlocker to hold them in place. We'll see how long that lasts. If they move, I can always JB weld the set screws, or just come up with a better motor mount design (these were really simple to make, however, since there was only one crucial tolerance to hold, the circle cuts, which had to be made to fit each side of the truck individually).

<img src="/uploads/db1493/original/3X/d/2/d289ad92470c10b9cb734f38edd2f9a92fa2958f.jpg" width="303" height="500">
Yes I know I'm missing screws, heading to the hardware store tomorrow.

Here are my VESC settings, for those curious what works for these motors:

Motor Min/Max: -70/90 (gives a lot of startup torque!)
Battery Min/Max: -7/25

Currently running a 14/40 ratio, tops out around 23MPH. But there is endless torque for climbing hills! Easily does 25% grade at 15+MPH (haven't scientifically proven this).

Overall, I'm very happy with this build. Plenty of power, and so much lighter than my stupid 8 wheel... that thing weighed like 30 pounds. Plans moving forward are to redress the griptape on the top of the board (you'll get to see it when it's done!) and move up from 83mm to 97mm wheels. Should bring the top speed up to around 27MPH, which is perfect for me.

Cheers!
```

---
## \#2 Posted by: lrdesigns Posted at: 2017-11-17T01:35:52.944Z Reads: 284

```
Cool. I want to see some photos of the focbox's mounted in your custom enclosure, I think that is super interesting. Could even be something people would want to buy.
```

---
## \#3 Posted by: Alanhunt123 Posted at: 2017-11-17T01:58:38.833Z Reads: 284

```
Here's a photo. Kind of hard to see, since everything is packed in there so tight.

<img src="/uploads/db1493/original/3X/7/f/7f9f5eb71e25db2e3cffcc0835cfbae1709f0907.jpeg" width="690" height="388">
```

---
## \#4 Posted by: Alanhunt123 Posted at: 2017-11-21T03:56:21.543Z Reads: 264

```
Update on the motor mounts:

They don't work. For anyone trying to design their own motor mounts, a set screw is not enough to hold a motor mount in place. The set screw, being made of steel, will start to wear whatever hole (aluminum) you set it in, and become looser and looser over time because of it.

No matter, I have access to a machine shop, just means I need to come up with a better design. This time, I chose to use a two piece clamp design. This separates the functional requirements of the setscrew. Now, instead of having to hold the motor mount tight and at the correct angle, it now only has to hold the correct angle, while the clamp holds the motor mount tight.

Here's what I have for design. Ribs reinforce the plate on this design, improving its resistance to warping and fatiguing over time, while keeping its weight down. I'll probably get around to machining it next weekend after Thanksgiving.

<img src="/uploads/db1493/original/3X/5/9/59c0657196828cd82b65f00e5e48ab142973ca8d.JPG" width="690" height="388">

Cheers!
```

---
## \#5 Posted by: egzplicit Posted at: 2017-11-21T13:14:42.352Z Reads: 244

```
[quote="Alanhunt123, post:1, topic:38576"]
Motor Min/Max: -70/90 (gives a lot of startup torque!)
Battery Min/Max: -7/25
[/quote]

With 25A battery max will you ever hit 90A on the motor? I’m asking because the rated amps on these motors is 32A and you seem to push a lot more (probably less than 90A but more than 32). Do they heat up? 

I have dual 5065 140kv currently set at 40A motor max with 30A battery max and wonder if I should increase motor max at like 60A. It’s got plenty of torque but would want to see how it feels if I go higher.
```

---
## \#6 Posted by: briman05 Posted at: 2017-11-21T13:45:08.005Z Reads: 226

```
How did you connect the to focboxs to each other could you show a picture of that and did you use a those can bus cable?  Also I know these motors come with the xt30 plug and have three cables coming off did you just pop out the connectors and use a xt90 plug and what did you do with the 3rd wire I believe it is yellow?
```

---
## \#7 Posted by: Alanhunt123 Posted at: 2017-11-22T02:42:58.315Z Reads: 226

```
Motor max and battery max do very different things on VESC. The motor's rated current (32A in my case) refers to the average current flowing through it, or what is supplied by the battery. Motor max controls the maximum current flowing through the coils of the motor. Since current is only flowing some of the time, due to duty cycle, the average current will always be less than the maximum current.

So, if you have your motor max set to 32A, and your motor is running at 50% duty cycle (this is constantly changing depending on speed), there is actually only 16A flowing from your battery to run the motor, and you won't be utilizing the motor's full potential. At startup speeds with lower duty cycles, motor max will dominate. Once speed increases, your average current (battery current) starts to increase, up until it reaches battery max.

In short, this means you can run your motor max as high as you want, within reason. This is because motor max doesn't control the maximum amount of power running through it. Battery max is what caps the amount of power the motor has. Think of motor max as a way of controlling low speed torque.

I actually stepped it up to 100A motor max. This means that once I hit 25% duty cycle (100*0.25=25), motor max goes out of effectiveness, and battery max takes over. The motors never get hot, even when climbing hills.

I've heard of people on this forum going as high as 200A motor max, but this is approaching the limits of the MOSFETs on the board, I'd keep it around 100A as a maximum.

I had the 5065s, and when I used them 60A felt ok, but didn't give enough umph for starting from a stop without cogging. Stepping it up to 90A or 100A made them start flawlessly on flat ground sensorless.
```

---
## \#8 Posted by: Alanhunt123 Posted at: 2017-11-22T02:49:47.416Z Reads: 215

```
Are you talking about the MT30 connectors?

I don't use those, so I cut them off and used 3.5mm bullet connectors, which I had plenty of on hand. They handle plenty of current in a dual drive setup, but I probably wouldn't use them on a single drive where higher current is necessary.

To hook the FOCBOX together, I used a parallel XT60 Y cable that I made for power input. I originally used the CAN cable to sync both together, but when I accidentally powered on one FOCBOX but not the other while CAN was plugged in, I fried both of the CAN chips on the boards. I removed the CAN chips to get the boards working again, and now I use a split servo cable to bring the throttle signal to both machines. Works well enough.
```

---
## \#9 Posted by: briman05 Posted at: 2017-11-22T03:36:52.365Z Reads: 207

```
I’m doing a duel drive 5065 I weight the same as you but I figured if I can get a little extra out of it I might as well. I’m going to do dual motors on bear grizzlies(hopefully the fit both) with focboxs, with a 10s4p battery of 30q’s on kegels with a gearing of either 15:32 or 15:36. And motor mounts with idlers
```

---
## \#10 Posted by: Alanhunt123 Posted at: 2017-11-22T18:19:24.911Z Reads: 208

```
You won't be disappointed with the 5065s. In fact, I think the limiting factor will be your batteries. I wouldn't draw more than 40A-45A from a 10S4P 30q setup, even though the pack should handle 60A on paper. This is simply for longevity purposes. I notice almost no difference between the 5045s and the 5065s because my 10S4P 25r setup is the limiting factor, which I draw no more than 50A from (pack is nominally able to draw 80A continuous). I'd personally go with the 15:36, but that's because I live in a fairly hilly area, and acceleration and torque is more important to me than a few extra MPH on the top end.
```

---
## \#11 Posted by: Alanhunt123 Posted at: 2017-11-28T06:10:26.510Z Reads: 204

```
Finished machining the first half of some new motor mounts! One of my better looking designs, I really put in a lot of effort into getting all the chamfers right. Enjoy some CNC goodness

<img src="/uploads/db1493/original/3X/b/c/bcf3862d3cf5ef8b26a58fab5d8bf9c8290af80a.jpg" width="690" height="371">
```

---
## \#12 Posted by: lrdesigns Posted at: 2017-11-29T00:47:00.668Z Reads: 190

```
These look beautiful :heart_eyes: if you made a caliber version you could sell a few.
```

---
## \#13 Posted by: Sender Posted at: 2017-11-29T13:18:32.852Z Reads: 177

```
Those are for Bear Grizzlies?  If so, and they work well, I'd love to buy a set!
```

---
## \#14 Posted by: Alanhunt123 Posted at: 2017-11-29T14:13:56.503Z Reads: 181

```
They're for Paris Trucks. Unfortunately, I can't offer machining service to anyone since the machines I have access to are for educational purposes only.
```

---
## \#15 Posted by: Lobap Posted at: 2017-12-10T22:55:07.116Z Reads: 165

```
Hey Alan,

How do those motors perform? Did you ride them few more km?

I'm planning to use the same motors for my build to keep it compact on a Jet Spud with 90mm wheels and 36T.

Cheers,
Pablo
```

---
## \#16 Posted by: Alanhunt123 Posted at: 2017-12-13T14:41:02.255Z Reads: 151

```
Hey Pablo,

How many hills does your area have? These motors will probably struggle with 90mm amd 36t, I'd recommend 40t. If your area is fairly flat, you might be able to get away with 36t.
```

---
## \#17 Posted by: Lobap Posted at: 2017-12-13T14:58:38.470Z Reads: 150

```
Thanks for your reply!

Indeed Madrid is fairly flat except some areas, of course, so I hope to be ok. Otherwise I will follow your advise and change to 40T.

And I also got an extra pair of R-Spec 97mm from Enertion (besides the 90mm from @JLabs) so maybe it works better with 36T and bigger wheels.

Let's see, it's my first build so this kind of "failures" are expected.
```

---
## \#18 Posted by: Alanhunt123 Posted at: 2017-12-13T17:49:07.587Z Reads: 142

```
You'll definitely want 40t on the 97mm wheels. I run 14:40 ratio on my 97s, and on 10s, these motors will get me up to 27MPH (43kmh) on flat surfaces, and 30MPH (48kmh) on slight downhill. A lesser amount of teeth on the wheel (36t) will give you less torque (acceleration and uphill power) and even more top speed.

Good luck on your first build!
```

---
## \#19 Posted by: Lobap Posted at: 2017-12-13T17:50:42.068Z Reads: 143

```
Thanks!

How about battery life? How long do you ride with a single charge?
```

---
## \#20 Posted by: Alanhunt123 Posted at: 2017-12-13T20:39:16.665Z Reads: 142

```
I only charge to 4.1V/cell and discharge to 3.2V/cell and still get around 14 miles, and that is in my very hilly area.

Cheers!
```

---
## \#21 Posted by: Lobap Posted at: 2017-12-30T15:38:41.139Z Reads: 123

```
Hey Alan

Do you plan to eventually sell your FOCBOX enclosure? I'm interested!
```

---
## \#22 Posted by: Alanhunt123 Posted at: 2017-12-31T12:46:37.977Z Reads: 118

```
Hi Pablo,

I have no plans on selling it in the immediate future, since the CNC machines I have access to are for educational purposes only (can't make money off of them). Maybe someday when I get access to my own CNC!
```

---
