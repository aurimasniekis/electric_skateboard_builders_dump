# (x4) Zippy 3S 5000mAh, Turnigy Aerodrive SK3 - 6364-245kv, Enertion VESC, Help please

### Replies: 30 Views: 5614

## \#1 Posted by: karan.basnet Posted at: 2016-05-20T06:27:47.928Z Reads: 308

```
Hey guys this is my first time building anything electric. Ive done quite a bit of research and according to what I have learnt I came up with this set up to best fit my needs which are:

* 10 miles plus range
* good torque 
* 20 mph speed (according to http://toddy616.blogspot.com/2013/07/electric-skateboard-calculator.html?m=1)
* easy to build (no soldering or adjusting the VECS software)

The build: 

<img src="/uploads/db1493/original/2X/3/3ae6b8627d2bfa35ef1aa5af86ccb6f5c28a1ca1.png" width="331" height="316">

Few questions

1. Can any one please let me know if this build is right for me, considering what I said above? I had a hard time calculating my top speed because every site I used told be something different.
2. Which would be better, series then parallel or the other way around?
3. Do I need any type of heat protecters? if so, recommendation? 
4. Recommendation for cheap but efficient charger?

Thank you!
```

---
## \#2 Posted by: Michaelinvegas Posted at: 2016-05-20T06:45:32.170Z Reads: 277

```
Hello and welcome ....

Let's have you start here:

http://toddy616.blogspot.com/2013/07/electric-skateboard-calculator.html?m=1

........
```

---
## \#3 Posted by: Michaelinvegas Posted at: 2016-05-20T06:46:47.512Z Reads: 282

```
After you figure out how fast you really wanna go ....

See here......


http://www.electric-skateboard.builders/t/new-builder-list-of-known-and-commonly-used-parts/2983?u=michaelinvegas



.....
```

---
## \#4 Posted by: shred Posted at: 2016-05-20T06:47:15.060Z Reads: 265

```
I use this calculator, I prefer this one because it is also telling you the theoretical max current flow in your circuit. 

http://217.118.128.188/tests/ev_calc.html

With 4x3S and with the 149kv you will probably go for a 12S. With 12S you get higher Voltage and lower current and as well more rpm out of your 149kv Motor. Especially with the VESC you don't like to do much more than 50A continuous. 

Whats your planned wheel size? (to be added in inch, e.g. 3.27 for 83mm)

Assuming you have a 15/36 transmission and 83mm wheels: 

S6 / 22.2 Volt / 2250W / 149KV = 100A = 3308RPM = 13.41 mph / 21.59 kph (without losses) 
S12 / 44.4 Volt / 2250W / 149KV = 50,6A = 6616PRM = 26.83 mph / 43.17 kph (without losses)
```

---
## \#5 Posted by: Michaelinvegas Posted at: 2016-05-20T06:48:48.874Z Reads: 246

```
Keep this shit simple...get complicated later...
```

---
## \#6 Posted by: Michaelinvegas Posted at: 2016-05-20T06:50:16.506Z Reads: 234

```
And if you wanna build an electric skateboard ... You better learn how to solder .... This ain't Legos
```

---
## \#7 Posted by: shred Posted at: 2016-05-20T06:53:57.645Z Reads: 225

```
sorry! 

202020202202020
```

---
## \#8 Posted by: Michaelinvegas Posted at: 2016-05-20T07:19:51.504Z Reads: 215

```
Lol no sorrys in eboard building

Just learn...it will put hair on your chest
```

---
## \#9 Posted by: susplus Posted at: 2016-05-20T08:37:47.498Z Reads: 205

```
the calculator has some problems..for a 260kv motor on 8s it list more than 200 km/h
```

---
## \#10 Posted by: shred Posted at: 2016-05-20T08:59:26.651Z Reads: 206

```
sounds like you mixed up Hub Teeth and Pulley Teeth
```

---
## \#11 Posted by: susplus Posted at: 2016-05-20T09:14:42.128Z Reads: 198

```
thought so too, but no. i am still getting some ridiculous numbers...
```

---
## \#12 Posted by: thisrealhuman Posted at: 2016-05-20T09:15:25.946Z Reads: 205

```
I keep [this calculator](https://howtomakeanelectricskateboard.wordpress.com/2013/05/09/calculating-speed/) on my desktop for calculating everything I plan. So far it hasn't been wrong with any builds I've put through it.

@karan.basnet Your motor is rated for 37V, with those batteries you will need to do 6s or 12s, but 12 will kill the motor. With a 6s setup you're limited to 12mph but will have a 10 mile range running at top speed. 

The batteries are a fine choice,but that charger needs to be (Genuine) rather than (copy), but if you get (Genuine) Imax B6, the 50w limit will only allow 2.2A charging, which means two packs will charge in about 2 hours, or charging all four packs with two 6s in parallel will take 4 hours. Those batteries are 1c and can be charged at 5A, so you should look into a 100w charging solution. Slower charging is better for the battery though.

Your motor is your weak spot. If you change batteries to 10s and change motor to 190kv It'll be 25mph assuming you're using 83mm wheels, and you can get a sub $100 motor that'll handle 10s, but if you want 12s go with a higher quality motor. I spent $160 on [my first motor](http://www.e-fliterc.com/Products/Default.aspx?ProdID=EFLM4160A) to make sure I can't kill it with voltage. It's survived two mounts so far but I'm about to upgrade to an R-spec.

18mph with 149kv isn't a bad start. It'll have enough torque to rip itself out from under you when you're already going 10mph and bump the trigger when switching hands. You could use an 18t motor pulley to get up to 22mph but you'll pull more amps that way.
```

---
## \#13 Posted by: WeeChumlee Posted at: 2016-05-20T11:10:01.558Z Reads: 196

```
Just my 2 Cents.
The SK3 6374 motors can handle 12S voltage without an issue - many people use 12S on these motors.
```

---
## \#14 Posted by: hamminitup Posted at: 2016-05-20T11:45:33.814Z Reads: 190

```
Huh pretty interesting. This is almost exactly my first build that I just ordered. Except mine is 6s instead of 10s or 12s. Really interested to see how yours goes.
```

---
## \#15 Posted by: Foster382 Posted at: 2016-05-20T14:28:06.920Z Reads: 182

```
Why push 44v through a motor that has a max voltage handling  of 37... so much for having head room lol
```

---
## \#16 Posted by: Trademarc Posted at: 2016-05-20T20:50:33.262Z Reads: 176

```
I don't know where the original 37v came from. I have the same motor and it's definitely rated at 44... See for yourself:
 <img src="/uploads/db1493/original/2X/b/b3a9f8604ec10a3e3fc0fc67c9761cdc15e2fc6b.png" width="251" height="182">
```

---
## \#17 Posted by: Foster382 Posted at: 2016-05-21T00:58:59.530Z Reads: 171

```
The spec sheet he posted says the max voltage is 37<img src="/uploads/db1493/original/2X/5/5b3b62ec10ecde0ffe1b7c646c990528409fac4d.png" width="281" height="500">
```

---
## \#18 Posted by: Trademarc Posted at: 2016-05-21T06:53:57.187Z Reads: 155

```
I realized that, which is why I said "I don't know where the original 37v came from" :P
```

---
## \#19 Posted by: claudiofiore88 Posted at: 2016-05-21T07:15:20.729Z Reads: 152

```
[quote="susplus, post:9, topic:3541, full:true"]
the calculator has some problems..for a 260kv motor on 8s it list more than 200 km/h
[/quote]

You're probably putting the wheel diameter in millimeters instead of inches.
```

---
## \#20 Posted by: karan.basnet Posted at: 2016-05-21T16:16:31.926Z Reads: 142

```
I really wanted to but I live in dorms and they told me its a fire hazard
```

---
## \#21 Posted by: karan.basnet Posted at: 2016-05-21T16:23:31.560Z Reads: 138

```
That was really helpful thank you!
```

---
## \#22 Posted by: karan.basnet Posted at: 2016-05-21T16:24:53.269Z Reads: 133

```
wow thats good to here, how did yours go?
```

---
## \#23 Posted by: karan.basnet Posted at: 2016-05-21T16:26:17.643Z Reads: 131

```
The 37v came form me contemplating if I should use the 245kv motor or the 149kv and i forgot to change it.
```

---
## \#24 Posted by: hamminitup Posted at: 2016-05-22T12:36:11.237Z Reads: 125

```
Well actually the parts are still arriving. Did you end up going with the 149kv or 245kv?
```

---
## \#25 Posted by: susplus Posted at: 2016-05-23T10:58:35.916Z Reads: 125

```
done that too, still getting some weird numbers. Here's a picture to see what i mean


 <img src="/uploads/db1493/original/2X/2/2bb8da8900b5ea0c2a83730725dc49b4ab9de9e4.JPG" width="571" height="500">
```

---
## \#26 Posted by: shred Posted at: 2016-05-23T12:53:35.939Z Reads: 114

```
looks good, just change "Hub Teeth == 36" and "Pulley Teeth == 15", that should to the trick ;)
```

---
## \#27 Posted by: susplus Posted at: 2016-05-23T13:23:37.975Z Reads: 111

```
hmmmm...this feels awkward. thanks for the heads up. If the stats are going to be true even at 50% efficiency i  will be one happy rider
```

---
## \#28 Posted by: karan.basnet Posted at: 2016-05-24T03:17:15.601Z Reads: 107

```
I see.... I have decided to stick with the 149 because Id rather have more torque, and according to all the calculators i have been using, my top speed is around 20mph and I am happy with that :) in addition the max voltage is 44 rather then 37
```

---
## \#29 Posted by: hamminitup Posted at: 2016-05-24T11:34:06.125Z Reads: 101

```
Cool. I got the 149kv too. That top speed is pretty good. I'll have to eventually go from 6s to 12s.
```

---
## \#30 Posted by: William_Trojel Posted at: 2017-08-16T04:52:48.267Z Reads: 20

```
can u link the site you used
```

---
