# Project Commute &#124; Dual VESC &#124; Dual Hub Motors &#124; Custom Battery, Deck, and Enclosure

### Replies: 12 Views: 1701

## \#1 Posted by: JLabs Posted at: 2016-11-26T22:31:24.943Z Reads: 268

```
Well, I cant decide. I kind of need your guys help. A little back story; I have my original Alpha Build, running a 6s lipo, 190kv 6354, custom mount, and FVT esc. I know have 2 vesc's and 2 (fixed) non slip (Jacob) hubs on the way. 
**Option 1:**
Keep my original Alpha build and build Project Commute, using everything stated in the title. 
**Option 2:**
Modify my Alpha build with Hubs and VESC's, and build Project Commute with a satellite configed setup. I want to use a custom penny style board with a custom pack. So can I run hubs on 6s? I need to stay within airline regulations and want it to be grab and go. 

I also want to pick up the cells asap because of liionwholesale black Friday sale on cells. I am leaning towards the 25r, but just want them to be reliable and stay within airline guidelines.I of course want the max amount of range possible.

So what do I do? 6s on hubs? I cant decide. I will be sure to post updates when the VESC's and Hubs arrive.
```

---
## \#2 Posted by: lox897 Posted at: 2016-11-26T22:36:56.382Z Reads: 259

```
I would go with option 1 because I don't think hubs would be efficient on 6s.
```

---
## \#3 Posted by: Mark Posted at: 2016-11-26T23:24:35.798Z Reads: 249

```
You need higher kv hubs for 6s. Like the carvon v2. better go for 12s when using hubs :)
```

---
## \#4 Posted by: Hummie Posted at: 2016-11-26T23:38:54.471Z Reads: 237

```
I just was on the plane with my board. In my experience having a board was no problem with my three packs of 3s 8ah.  We checked out American's rules and from what we read I could have as many packs under 100wh as I'd like. They let me take it (has to be carry on) even though my board is much bigger than the size limit as well 

Motors run more efficiently on lower voltage if ur going to go slow anyway.  The esc needs to be able to handle the greater Amps though. Magic happens and it's all amps in the motor.
```

---
## \#5 Posted by: JLabs Posted at: 2016-12-04T21:11:42.883Z Reads: 202

```
VESC testing has commenced! XT90S added. Stay tuned for updates<img src="/uploads/db1493/original/3X/4/f/4f711a877c25102add44db09d35be0fb2d3f0095.jpg" width="375" height="500">
```

---
## \#6 Posted by: mccloed Posted at: 2016-12-04T21:32:47.734Z Reads: 194

```
These look like they are from Freerchobby? I usually update C51 and C37 to the correct 15uf, 100v caps. I also upgrade the wires to , at least 12 gauge before I use them.
```

---
## \#7 Posted by: saul Posted at: 2016-12-04T21:33:48.940Z Reads: 191

```
Yupp i'd go option 1 because those hubs have heat issues so high V is better than high A.

but its always fun to experiment.
```

---
## \#8 Posted by: Hummie Posted at: 2016-12-05T03:29:45.628Z Reads: 191

```
the high voltage thing being more efficient is the case for the battery and esc and overhead power lines but not the motor.  best to simple view the motor performance in relation to the motor kv, the supplied voltage, and the percentage of that max no-load speed you're traveling.  the most efficient way to run a motor is at roughly 80 percent of the no-load speed.  If you ride around with a high kv in a low speed it's inefficient.  If you ride around with a low kv at the same speed it will be more efficient, downside being you're max speed is low.  a compromise.  Or get a high kv motor and reduce it's no-load by reducing the voltage if you want to run slowly and efficiently and then increase the voltage when you want to be going faster.  this is assuming the esc can take the increased amps with a lower voltage
```

---
## \#9 Posted by: JLabs Posted at: 2017-01-29T00:05:58.882Z Reads: 158

```
Almost everything is gathered or is close to being here. I picked up some ShredLights and I decided on a compact 10s3p. 

Only thing I am looking for is a Potato like deck (similar to Unik). If anyone knows where to get one I would love a link! 

I will post build photos when everything arrives and I start to assemble it all together.
```

---
## \#10 Posted by: ajaynagra Posted at: 2017-01-29T00:20:56.490Z Reads: 151

```
http://www.jetskateboards.com/?room=spud-29-0-2
```

---
## \#11 Posted by: JLabs Posted at: 2017-03-25T03:42:48.040Z Reads: 119

```
Finally getting around to building this... I got the BMS installed on my 10s3p 25R pack.. 

Question: do I need a CANBUS cable? Or is a servo splitter good enough? I'm going dual hubs and VESC. Believe it or not, this will be my first build with a VESC... need some assistance.
```

---
## \#12 Posted by: surprisebirthday Posted at: 2017-03-25T19:49:59.914Z Reads: 105

```
A servo splitter is good enough if you just want to get going.  As you know, CANBUS will buy you traction control and will allow you to configure both VESCs without having to pull the USB cable from one and then plugging it in to the other.  Once you get your VESCs configured the way you like it, you probably won't be tweaking the parameters too much.

I tried CANBUS initially, but I couldn't keep a reliable CANBUS connection.  I had commitment issues, so I didn't want to solder or hot glue it in either, so I eventually just went with the servo splitter.  No complaints.  I haven't experienced a need for traction control.
```

---
