# Speed vs. Range. Practical test results

### Replies: 39 Views: 3118

## \#1 Posted by: SimosMCmuffin Posted at: 2017-04-14T17:58:14.535Z Reads: 391

```
I have been keeping a log of all my runs on my board, which is using my own motor controller. I have been logging gps info, date, travel time, travel speed, # of teeth in motor gear, battery pack configuration, mAh/km, Wh/km and average power over the runs. Here's a link to the google sheet with all the results (https://docs.google.com/spreadsheets/d/1eorvXba_T8MIPB3ofDTwA8SjOiL4x7r-A7Iy1rNPU9M/edit?usp=sharing), select the "Gen2.1 deck" sheet from the bottom of the page.

I wanted to test the ratio of travel speed and energy spent per kilometer, so I decided to do 3 runs without any kind of duty cycle limitation, AKA full speed runs and then do another 3 runs with a 70% duty cycle limit. My battery pack is a 6S4P configuration made with LG MJ1 cells.

So in theory, with the 70% duty cycle limit the board should only go about 70% the speed than without the limit or simulate the motor seeing only a 4S battery. This test was meant to actually see how the results behave.

I have this benchmark route that I ride when I want to see how a board behaves over long distance. It is a there-and-back route, which means environmental effects such as wind have lessened effect and overall the terrain averages a flat plane (uphills become downhills on the way back and so on...). The route doesn't have any lights and is generally a very quiet piece of road. This allows me to keep my duty cycle at the maximum for about 99% of the run.

After I come home I then let the battery rest a bit and then charge it with a RC charger in balance mode and log the charged capacity and then interpolate the other variables from that based on the travel time and distance.

----------


Results are:
**non-limited runs:**
23.1 km/h avg; 13.1 km; 521 mAh/km; 11.6 Wh/km; 267 W avg power
23.1 km/h avg; 17.0 km; 509 mAh/km; 11.3 Wh/km; 261 W avg power
23.0 km/h avg; 18.0 km; 506 mAh/km; 11.2 Wh/km; 258 W avg power

**85% duty limited runs:**
20.5 km/h avg; 13.0 km; 445 mAh/km; 9.9 Wh/km; 203 W avg power
20.6 km/h avg; 14.5 km; 432 mAh/km; 9.6 Wh/km; 198 W avg power
20.4 km/h avg; 17.0 km; 422 mAh/km; 9.4 Wh/km; 191 W avg power

**70% duty limited runs:**
17.7 km/h avg; 13.0 km; 356 mAh/km; 7.9 Wh/km; 140 W avg power
17.5 km/h avg; 13.0 km; 400 mAh/km; 8.9 Wh/km; 156 W avg power
17.3 km/h avg; 18.0 km; 374 mAh/km; 8.3 Wh/km; 143 W avg power

**Averages:**
non-limited: 23.1 km/h; 512 mAh/km; 11.4 Wh/km; 262 W avg power
85% limited: 20.5 km/h; 433 mAh/km; 9.6 Wh/km; 197 W avg power
70% limited: 17.5 km/h; 376 mAh/km; 8.4 Wh/km; 146 W avg power

**Conclusions:**
Comparing the 70% duty limit to the non-limited results we can deduce some things.

_23.1 km/h * 0.7 = 16.2 km/h_; I went faster at 17.5 km/h, which I think can be explained by lower voltage droop across the battery, because lower continuous current and the non-linearly behaving aerodynamic drag (relatively lower drag at lower speed).

512 mAh/km * 0.7 = 358 mAh/km; I spent a bit more capacity per kilometer with 376 mAh/km, but I believe some of this can be attributed to the cold temperature, especially on the latter 2 duty limited runs when it was almost below freezing and most likely was if wind chill would be factored in. Taking a look at the LG MJ1 cells' datasheet (https://eu.nkon.nl/sk/k/Specification%20INR18650MJ1%2022.08.2014.pdf) they spec the temperature effects on the battery the following:

<img src="/uploads/db1493/original/3X/c/2/c2187db61887cb9a1d37d63dfa3476fa4e5f0e82.jpg" width="627" height="206">

I'm not 100% sure, but this might have had an effect on the result. Although it still shouldn't cause the cell to use extra energy. Or maybe it was because I did go a bit faster when comparing the average speeds then what was predicted and that's what caused the extra energy expenditure.

_11.4 Wh/km * 0.7 = 8.0 Wh/km_. 8.4 Wh/km This result follow the same conclusion logic as the mAh/km one, but clearly shows less energy spent per kilometer, meaning that **going at lower speed gets you more range**

_262 W * 0.7^2 (<- power needs to factored in this way) = 128 W_. 146 Watts average power shows that indeed my average power consumption was higher and therefore my mAh/km and Wh/km should have been a bit higher than the straight calculations show. Question is that what would the results have been if I had been traveling at the 16.2 km/h average speed rather then the 17.5 km/h I did with the 70% duty. Would the rest of the results fallen in line in that case? Are the results much more linearly linked to the speed rather than the duty cycle?

**Summary:**
The results were overall very close to the estimated values and show how much the travel speed impacts your energy expenditure. I'm pretty happy that the results were within 10% of the calculated values. I can use this information in the future to make a bit more educated decision on what kind of battery pack I'm going to build regarding speed and range.
```

---
## \#3 Posted by: Challlsss Posted at: 2017-04-18T20:22:03.123Z Reads: 271

```
@Stef you make good points. Just wanted to clear up, doubling speed wont necessarily cost 4x the power. This is because power expenditure isn't solely based on wind drag. It will _Octuple_ the power _that was used to combat drag_ This can be calculated using, <img src="/uploads/db1493/original/3X/e/a/ea6fbc619a3761c51f7b4425cba87000afece3d0.jpg" width="414" height="106">
Where: 
- P is the power lost from drag
- C_D is the coeficient of drag (around 1.0-1.3 for a person standing)
- p is the density of air (1.225 Kg/m^3 at sea level)
- v is velocity
- A is cross sectional area of person perpendicular to velocity vector (I've never measured this but found a person who has online and stated theirs was about 0.5 m^2

EDIT: Using these numbers:

At 17.7 km/h (4.92 m/s) there is a 47.3 Watt expenditure to combating air resistance
At 23.1 km/h (6.42 m/s) there is a 105.2 Watt expenditure to combating air resistance
```

---
## \#4 Posted by: SimosMCmuffin Posted at: 2017-04-18T20:26:05.157Z Reads: 237

```
Where did you get that equation?

I found this one (click for bigger picture):
<img src="/uploads/db1493/original/3X/e/f/ef6180b7f3882f037f1525b89a14bdc555470354.jpg" width="690" height="182">

And it has the velocity squared, not cubed.
```

---
## \#5 Posted by: Challlsss Posted at: 2017-04-18T20:28:02.039Z Reads: 214

```
@SimosMCmuffin That equation is for Force, with units in Newtons. We are looking for Power in Watts

EDIT: 
To get to watts you need to multiply Newtons by m/s i.e. velocity (this is why it goes to the third power)
```

---
## \#6 Posted by: SimosMCmuffin Posted at: 2017-04-18T20:30:52.306Z Reads: 203

```
Yep, just realized my mistake.
```

---
## \#7 Posted by: Challlsss Posted at: 2017-04-18T20:33:29.189Z Reads: 196

```
If I had to guess I'd say that the estimates for wind resistance are fairly close. You are probably spending a bit of extra power on friction in the bearings of your wheels and lost motor efficiency because it needs more torque to maintain a higher velocity.
```

---
## \#8 Posted by: SimosMCmuffin Posted at: 2017-04-18T20:35:43.453Z Reads: 195

```
It's just the squared works so nicely with my test results, but I agree that having only results at 2 different speeds might not reveal everything.

Avg power at 17.5 km/h -> 146 W
Avg power at 23.1 km/h -> (23.1/17.5)^2 * 146 W = 254 W (measured 262 W)
```

---
## \#9 Posted by: Challlsss Posted at: 2017-04-18T20:40:40.991Z Reads: 191

```
This is likely because the wind resistance is only accounting for about 1/2 of the power increase between these two tests. The other section is probably from friction in your bearings/motor and lost efficiency from higher torque. If I had to guess I'd say that the friction is much more significant than the efficiency change. Power expenditure from Kinetic (or static) friction measures as u*N*v. If this is accounting for exactly 1/2 of your lost power and you have only 2 data points it makes sense for it to seem as if it is v^2

EDIT: I'd assume that as velocity increases above 23 km/h you will see the wind resistance have a much larger impact than other factors, and at lower speeds below 17.5 km/h you will see the friction from bearings having the largest impact on power drain.
```

---
## \#10 Posted by: SimosMCmuffin Posted at: 2017-04-18T20:44:45.727Z Reads: 185

```
I think motor constant Km is the other major factor.

<img src="/uploads/db1493/original/3X/1/1/113bd1ff5e81e461246fa2565d97a03cc0f1b514.jpg" width="690" height="231">

To double produced torque, we need to quadruple the motor power (double current). So I think it's the aero drag + motor constant, which are the biggest power losses.

EDIT: I really need to add at least 1 more different speed to the results above.... Maybe do couple test runs with 85% limit and then figure out the trendline from there.
```

---
## \#11 Posted by: Stef Posted at: 2017-04-18T23:44:13.111Z Reads: 155

```
Ah I see, makes sense!
```

---
## \#12 Posted by: SimosMCmuffin Posted at: 2017-04-20T08:09:38.525Z Reads: 156

```
@Stef @Challlsss

I did 3 additional runs with 85% duty cycle limit and have updated the original post with the results, but they so far still lineup in the squared factor.

I propose that for now, we come to the conclusion that at lower speeds (<30 km/h) the aerodynamic drag is still small enough to not start influencing the results in the factor of velocity cubed?

I plan on doing a completely new set of higher speed tests in the future once I get my new board with the new motor controller running, but for now the results should be considered non-conclusive for higher speeds?
```

---
## \#13 Posted by: Challlsss Posted at: 2017-04-20T13:06:48.108Z Reads: 151

```
<img src="/uploads/db1493/original/3X/9/c/9ce213f2103bb86ed3383c94a544b7afffcace9d.png" width="668" height="499">

I'd say that a squared curve is definitely what the data seems to be indicative of so far. I'd be curious as to why that is, although I have a suspicion that it is due to the torque equation making it a force squared that drag is calculated, rather than power.
```

---
## \#14 Posted by: SimosMCmuffin Posted at: 2017-04-20T14:22:08.993Z Reads: 141

```
And the reason why the average continuous power rises in velocity squared and the energy consumption rises linearly with velocity is easily explained below:

Example values,
10 km/h, 100 W average power, 5 Wh/km
20 km/h, 400 W average power, 10 Wh/km

When traveling at double the speed and at quadruple the power as at half speed, you're only spending half as long traversing a kilometer at 20 km/h then at 10 km/h, so the energy consumption therefore only doubles.

----------

I'm trying to rationalize the drag force with the motor torque constant and figure out the power from there.

Example values:
-Motor has a torque constant Kt = 0.2 Nm/Amp and when factoring in gear ratio and wheel size, 
 comes to 1 N/Amp applied to the road. Power can be calculated with I^2*R, but let's say the R = 1 for easier calculation
10 km/h, 10 N drag force, 10 Amps of motor current to produce equal counter torque, 1x power
20 km/h, 40 N drag force, 40 Amps of motor current to produce equal counter torque, 16x power

Does this make sense so far?

Now let's apply this logic to our test results.
17.5 km/h, X N drag force, Y Amps of motor current to ---, 1x power
23.1 km/h,  (23.1/17.5)^2 = 1.74 X N drag force, 1.74 Amps of motor current needed, 3x power

But this isn't what the tests show. So somewhere I get confused and at the moment a can't figure out where.
```

---
## \#15 Posted by: Stef Posted at: 2017-04-20T14:33:49.287Z Reads: 128

```
I think I know what is going on here:

We are interested in the energy use per distance (Wh/km) to see how far(km) we can make it on a single charge(Wh) at different average speeds. We are not necessarily interested in the energy use(wh) per time(h) here, unless you ride for fun only and want to calculate your maximum ride time based on the speed.

Power needed to overcome drag goes up with the cube of velocity (v^3) as stated by @Challlsss, that is correct. However, the energy consumption due to drag -per distance- goes up with the square of velocity(v^2):

Example, going from A to B that are 10km apart with 10km/h avg speed and 20km/h avg speed:

Average speed 10km/h - power consumption due to wind drag 100W - time from A to B 1hr -> energy used 100W*1h=100Wh

Average speed 20km/h - power consumption due to wind drag 100W*2^3=800W - time from A to B 0.5hr -> energy used 800W*0.5h=400Wh (which is equal to 100*2^2 -> square relation)
```

---
## \#16 Posted by: Challlsss Posted at: 2017-04-20T14:43:08.202Z Reads: 122

```
So you said something important which I didn't notice. [quote="SimosMCmuffin, post:14, topic:21015"]
you're only spending half as long traversing a kilometer at 20 km/h then at 10 km/h,
[/quote]

Lets take a look at the equation again and balance it,


torque/sqrt(power) = torque/sqrt(power)


so we can get down to the obious:


Power = Power


Now we'll combine Mechanical (theoretical power) with Electrical (test results)


(Constant)(v^3) + Ff(Frictionforce)*Velocity = I^2R


*However this is only useful if we are, as @Stef said, measuring using time, so to get to Wh/m we will divide by meters (Because it's easier than Km ;)) 

We get:

(Constant)(v^2)/t + Ff/t = I^2R/t

To make your calculations easier it could be useful to do a few tests that are timed runs, rather than distance. For example do a 10 km loop and when you hit a nice number like 30 mins stop collecting data. Another consideration is voltage drop over time. I'm not entirely sure how it applies but your current will (I think) increase as your batteries run out of charge to maintain the power output.
```

---
## \#17 Posted by: SimosMCmuffin Posted at: 2017-04-20T14:59:20.135Z Reads: 119

```
<img src="/uploads/db1493/original/3X/b/c/bcfd549f3c1d025b614a46323ceb8e316b16a460.jpg" width="690" height="149">

I have a link to the google spreadsheet with the date, travel time, distance, charged mAh to battery and other info derived from those variables in the original post. You can also check the formulas used to calculate the derived info from the run.

here's a graph for speed at time, from the 85% limited 17 km run.
<img src="/uploads/db1493/original/3X/e/8/e881e2498efa57baf8204c8effd7c2c536ab3c14.png" width="690" height="388">

It's not super clear, but the speed clearly starts to drop towards the end of the run, which is normal as the battery voltage drops from being drained.
```

---
## \#18 Posted by: Challlsss Posted at: 2017-04-20T15:01:30.566Z Reads: 104

```
Ok so because the speed decreases with time we can assume that the voltage drop is fully accounted for in our power equation?
```

---
## \#19 Posted by: SimosMCmuffin Posted at: 2017-04-20T15:14:31.561Z Reads: 111

```
The power is calculated by first charging the battery and seeing how much charge is put back in to it, which is then multiplied by the _nominal_ voltage of 3.6V to give the total spent energy on the ride in Wh. This total energy amount is then divided by the ride time to calculate the average power.

Unfortunately that's the best I can do with the current setup, as the motor controller doesn't record anything.

Everything is averaged, is what I'm trying to say.
```

---
## \#20 Posted by: Challlsss Posted at: 2017-04-20T15:23:19.790Z Reads: 108

```
sure.

I'm having trouble understanding the picture of the sheet since I can't see headers. Seems like since you are doing averages you are gunna need to add time to the measurements. Not sure if you can do that accurately with current data.
```

---
## \#21 Posted by: Okami Posted at: 2017-05-19T16:10:14.589Z Reads: 97

```
Very nice thread! Someone should pin it to category 'Power consumtion / battery building / speed vs power'' or similar..

Im surprised I had missed it but this is not the first time this happens..

Anyways, nice info @SimosMCmuffin so you do prove that for about ~20kph speed. not more than 250w is usually needed, pretty close to what ebikes (bicycles) use since power consumtion is similar.
```

---
## \#22 Posted by: SimosMCmuffin Posted at: 2017-05-19T16:16:00.874Z Reads: 94

```
I'm going to be re-doing these tests once I get the new board up and running, because I'm interested how the pneumatics and the new FOC motor controller affect the numbers. I would believe that the FOC ESC is more efficient, but I don't know how much yet, I want to get field test data first. The pneumatics should decrease efficiency a little bit, because they will most likely have more rolling resistance, but that is also dependent on the tire pressure...

Will have to see once I get the board up & running.
```

---
## \#23 Posted by: Okami Posted at: 2017-05-19T16:42:06.443Z Reads: 95

```
Yeh, definately do this! We need more data like this - done in a decent and systematic (almost scientific :D ) way..

I had a real problems and pity designing mountainboard build since at that time not that many users had emtbs and information was very limited..

I think only after a while I found out about average consumtion of 20wh/km for mountainboard pneumatic wheels and there is still not a clear reference at what speed such consumtion is achieved.
```

---
## \#24 Posted by: Bataleon Posted at: 2017-05-19T17:03:47.360Z Reads: 91

```
Thanks for sharing, @SimosMCmuffin. These numbers are really interesting. Is your board powered by a single motor which drives both back wheels?
```

---
## \#25 Posted by: SimosMCmuffin Posted at: 2017-05-19T17:24:02.007Z Reads: 98

```
http://imgur.com/a/Mjodj
```

---
## \#26 Posted by: Maxid Posted at: 2017-05-19T18:05:10.061Z Reads: 94

```
[quote="SimosMCmuffin, post:22, topic:21015, full:true"]
The pneumatics should decrease efficiency a little bit, because they will most likely have more rolling resistance, but that is also dependent on the tire pressure...
[/quote]

On my skikes at high pressure (6 bars) I needed around double the energy per km than with kegels.
```

---
## \#27 Posted by: SimosMCmuffin Posted at: 2017-05-19T20:43:44.756Z Reads: 89

```
Hmm... Maybe to test the rolling resistance between PU and pneumatics: Just roll off of a small ramp and just see how far you can roll. Of course remove belts to remove parasitic friction from the drivetrain.
```

---
## \#28 Posted by: Okami Posted at: 2017-05-19T21:00:30.788Z Reads: 85

```
IF we find a constant value this way, we could tell people how to make their ramps to test rolling friction lol :D
```

---
## \#29 Posted by: Okami Posted at: 2017-05-20T21:47:30.496Z Reads: 86

```
[quote="Bataleon, post:24, topic:21015"]
Is your board powered by a single motor which drives both back wheels?
[/quote]

No, I think the second axle is just for support and he does not use it..

Maybe @SimosMCmuffin can answer on this one - why your board has 2 axles and how did you exactly made it longer?

I dont see that u would use adapter which came with the motor..to somehow extend it..

I assume maybe u changed the whole axle to make it happen? Or is it just a bigger motor which came this way (dual axle) ? Looks like turnigy aerodrive motor to me, so im not sure they even sell dual axle versions :)
```

---
## \#30 Posted by: SimosMCmuffin Posted at: 2017-05-20T22:40:04.011Z Reads: 81

```
It's just a longer single axle that I changed to from the shorter original one. The 3D-printed motor mount wasn't stiff or sturdy enough to leave the motor just hanging off one side, so I decided to add a support bracket for it on the other side.
```

---
## \#31 Posted by: Okami Posted at: 2017-05-20T22:40:48.507Z Reads: 78

```
hah pretty clever how u managed to do that with 2 axles and 'get away' with 3d printed mount! :D
```

---
## \#32 Posted by: SimosMCmuffin Posted at: 2017-05-20T22:47:46.019Z Reads: 76

```
I mean there is just a 1 single long axle that goes through the motor. No two axles.
```

---
## \#33 Posted by: Okami Posted at: 2017-05-21T00:22:34.609Z Reads: 75

```
yeh sorry for the bad wording.. I would say one long axle, which can mount 2 pulleys for example.
```

---
## \#34 Posted by: SimosMCmuffin Posted at: 2017-05-21T08:47:06.527Z Reads: 79

```
Then you run into the differential problem with the differing wheel speeds when turning. I did test his in the very beginning, mounting 2 pulleys on a single axle and both of them to the wheels, but it wouldn't had worked out for very long due to the aforementioned differential problem.
```

---
## \#35 Posted by: Okami Posted at: 2017-05-21T12:33:11.825Z Reads: 73

```
yeh I know, some sort of freewheel design is needed for this.

I think ive seen CarvOn have demonstrating something similar. Not even sure how they made it work.
```

---
## \#36 Posted by: Idle Posted at: 2017-11-21T06:04:35.088Z Reads: 62

```
[quote="SimosMCmuffin, post:34, topic:21015, full:true"]
Then you run into the differential problem with the differing wheel speeds when turning. I did test his in the very beginning, mounting 2 pulleys on a single axle and both of them to the wheels, but it wouldn't had worked out for very long due to the aforementioned differential problem.
[/quote]

Hi Simon :wave

Could you please elaborate on this? Specifically about the wheel scrub you had with the locked rear.
Under power, did it fight back and the rear made the front push when you turned sharp, or what? 

The world wants to know.

Oh, and that's a really nice build!
And nice work on the range testing, my head hurts now…too much maths for me.
```

---
## \#37 Posted by: SimosMCmuffin Posted at: 2017-11-22T13:06:59.046Z Reads: 56

```
I never went as far as to test it under power, because it did not feel nice even under dummy setup with an un-powered motor axle connected to both wheels. Regardless of speed, either one of the wheels will skip and skitter when turning and the worse it becomes the tighter the turn. It will also send a lot of reverse torque back to the motor, stressing the axle.

So unfortunately I can only speculate what it would have been like to test under power, but I did not feel like it would have been worth it according to my personal testing.

This video can give you some idea of the pros and cons associated with a locked diff
https://youtu.be/tuT-SZKZdAk?t=42s
```

---
## \#38 Posted by: PXSS Posted at: 2017-11-22T14:18:23.519Z Reads: 53

```
Again. A car has 4x tighter turning radius than a longboard. The equivalent car would have a 100ft turn radius
```

---
## \#39 Posted by: SimosMCmuffin Posted at: 2017-11-22T16:09:19.253Z Reads: 53

```
Fair enough.

All I can say that I did not personally find the idea to be worthwhile to keep testing further based on my short unpowered tests. I will absolutely admit that due to the shortness of my testing and not running it under power, it might have given me the wrong impression of how it would have turned out.

So if someones wants to go for... Go for it and share the results, both the good and the bad.

And also, in my setup the limiting performance factor is not the lack of grip with the tires, but rather the lack of motor torque, so this wouldn't really help my setup perform better.
```

---
## \#40 Posted by: Zilonis Posted at: 2018-05-11T00:56:49.416Z Reads: 38

```
![Knipsel|383x500](upload://li18QK52INjoyxOuWvBsStLS4m5.PNG)

Here you go I hope I could help. Ask if you want to know something.

BTW: you shouldn't think that if you have 10000watts at your disposal that you will go fast. You should consider KV of the motor. And other things. But this will give you a good estimate how much power you need to go a certain speed. Like if you need 1000watts going 45 km/h you need a double setup. Because at these speeds the rolling resistance will become relevant. And you'll have losses.
```

---
