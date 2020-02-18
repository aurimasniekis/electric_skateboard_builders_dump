# What KV rating should I choose?

### Replies: 19 Views: 6410

## \#1 Posted by: Driftwood Posted at: 2016-11-12T17:13:49.900Z Reads: 452

```
Hi guys hope someone can give me advice...I want to get two alien 6355 motors...there are 2 options...one has a kv of 190 and 230. I weigh 90kg's...what should I choose, they both same price.
Thanks.
```

---
## \#2 Posted by: Hillso Posted at: 2016-11-12T17:22:52.155Z Reads: 448

```
It depends on your personal preference. low kv = hige torque low max speed, high kv = low torque high max speed.
(for the same gearing and wheel size and weight and voltage and amperage and stuff)
```

---
## \#3 Posted by: NickTheDude Posted at: 2016-11-12T17:23:23.858Z Reads: 435

```
Which ESC are you planning on using? And what voltage?
```

---
## \#4 Posted by: Driftwood Posted at: 2016-11-12T17:45:51.889Z Reads: 423

```
was thinking on getting ESC from enertion and using 24volt 5000Mah Lipo...i gues i should go with a low KV then as i want power over speed...or just a good balance between the both.
```

---
## \#5 Posted by: Driftwood Posted at: 2016-11-12T17:47:40.292Z Reads: 407

```
thanks Hillso, you just cleared that up for me...the difference between KV of motors.
```

---
## \#6 Posted by: itsmikeholland Posted at: 2016-11-12T18:17:31.902Z Reads: 399

```
I got the 6373 149kv from Turnigy and am easily able to get over 25mph. Not sure how fast you want to go, but lower kv usually means more efficiency and less heat.
```

---
## \#7 Posted by: Hillso Posted at: 2016-11-12T19:17:17.094Z Reads: 391

```
kv is rpm per volt, this helps http://calc.esk8.it/
```

---
## \#8 Posted by: Namasaki Posted at: 2016-11-12T20:09:39.169Z Reads: 375

```
I don't know how much range your wanting to get but 6s/5000 Lipo will only get you about 5 miles.
You can double that range by using 2 of those Lipos in parallel for 6s/10000 or in series for 12s/5000
Voltage x capacity = watt hours 
Watt hours divided by load = range
The Vesc has an RPM limit of 8571 and can fail if you go too high with voltage and KV. 
RPM= volts x KV
More voltage will increase torque and acceleration more noticeably than lowering the KV while also increasing top speed and reducing current flow. 
10s and 190kv is a proven combination delivering good torque and speed while being very dependable. 
6s is ok if your riding mostly flat but if your planning to do much hill climbing then I would recomend 10s and 190kv. 
If you decide to stick with 6s then I would recommend the higher 230kv motor.
The Alien power hev precision motor are great(I'm currently using them myself) but there shaft is non standard 10mm and you'll have to get pulleys from Alien power to match them. Also if you go with this motor, you will be limited to using 9mm belts. 
As far as motor size, 6355 is good for a dual drive setup but if your doing a single drive, then I would recomend considering the larger 6374 motor which should produce more torque because of its longer stator and magnets. 
I have personally used dual 6355's 230kv with 6s and 12s
Top speed was about 15mph with 6s and 28mph with 12s. These numbers depend on gear ratio and rider weight.
```

---
## \#9 Posted by: Mobutusan Posted at: 2016-11-14T08:49:44.871Z Reads: 299

```
@Namasaki Just out of curiosity, were you using the TB mini remote when you got those results? I ask because when I ran those same two 230kv motors on 12s with TB 12s esc's and 14/36 gearing on 83mm wheels with a **GT2B**, I hit 30mph on a full charge and still had a little extra throttle left (I got scared and backed off, but I'm guessing it could have gotten up to 32+mph, at least). When I swapped the GT2B out for the TB mini remote, making no other changes, on a freshly charged battery, I had the throttle pegged and only got up to 28mph. This is using the same two gps speed/tracking apps on the same stretch of flat bike path, and the only change/variable was the different remote. I fiddled with the trims, re-paired the mini remote many times and same result. And I'm around 75-80kg fully loaded when I ride.
```

---
## \#10 Posted by: darkkevind Posted at: 2016-11-14T10:51:59.184Z Reads: 278

```
I would go with the 230kv option, that's what I'm running and the speed is just about fast enough for me, and it pulls my weight no problem, I'm about 85kg and hills aren't a problem for my board. 190kv will be too slow I think.
```

---
## \#11 Posted by: Driftwood Posted at: 2016-11-14T12:08:01.836Z Reads: 268

```
Are you running dual motors?
```

---
## \#12 Posted by: darkkevind Posted at: 2016-11-14T12:15:26.822Z Reads: 258

```
Nope, just one!

http://kevindark.co.uk/Blog/Read/7
https://www.youtube.com/watch?v=UOuKlUChD8g
```

---
## \#13 Posted by: Namasaki Posted at: 2016-11-14T16:32:33.775Z Reads: 240

```
Is it a 230/6355 or 230/6374?
```

---
## \#14 Posted by: Namasaki Posted at: 2016-11-14T16:37:32.123Z Reads: 237

```
I was using the mini. And I noticed that moving the trim on the remote would decrease or increase top speed. 
I've never tried a GT2B but it sounds like you've got a lot more throttle with it than the mini.
```

---
## \#15 Posted by: Mobutusan Posted at: 2016-11-14T18:27:38.399Z Reads: 227

```
Interesting. What's even more odd is that switching from channel 2 (trigger) to channel 1 (steering wheel) resulted in about 250rpm increase at the wheels, measured with a hand held tachometer.

I'll investigate further and start a new thread on this subject. Sorry for threadjacking.
```

---
## \#16 Posted by: darkkevind Posted at: 2016-11-14T18:53:42.533Z Reads: 218

```
I noticed that too, also the step-ups in speed are more smooth with the wheel than with the trigger...
```

---
## \#17 Posted by: bwosei17 Posted at: 2017-02-26T00:46:01.821Z Reads: 195

```
hey guys so I'm building my own board and i'm kinda stuck trying to understand what exactly the kv value means. I'm about 185 lbs and I'm debating between a 192 kv motor with 2750 W of power and 149 kv motor with 2250 W of power. How low does the power have to get before I have to start worrying about it being too low and also I heard lower KV is better because it give more torque but you guys are talking about using 200 kv and up so I'm confused
```

---
## \#18 Posted by: itsmikeholland Posted at: 2017-08-17T22:08:37.042Z Reads: 168

```
if you havent already, go with 149kv. Ive used 12s, 10s, and 6s with my 149kv and have no idea how people think its slow. ive done 28mph with plenty of throttle to spare and have popped wheelies twice in the past three days when my receiver wires came loose and triggered the full throttle.
```

---
## \#19 Posted by: claphamska8er Posted at: 2019-06-19T23:58:15.368Z Reads: 39

```
Hi, I was just wondering what battery pack you used with this motor and ESC?
```

---
