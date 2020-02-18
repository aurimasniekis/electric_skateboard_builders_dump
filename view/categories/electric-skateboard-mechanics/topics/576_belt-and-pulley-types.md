# Belt and Pulley Types

### Replies: 18 Views: 8453

## \#1 Posted by: claudiofiore88 Posted at: 2015-11-24T23:29:54.847Z Reads: 599

```
What are the advantages and disadvantages of certain pitches and belt widths (eg. 5 mm htd 9 mm width vs  3 mm htd 15 mm width)?  Why use htd at all?  There are other pitch types, why are those not used (eg gt2, xl etc.)? Has anyone on the forum experimented with different pitch sizes and/or types or do people just blindly follow the norm.  Sorry, my curiosity must be getting the better of me.
```

---
## \#2 Posted by: onloop Posted at: 2015-11-24T23:46:06.032Z Reads: 597

```
Yes, I have tested this fairly extensivley....

The size of the tooth & the width of the belt is proportional to the amount of torque it can transfer...

Basically, it boils down to the surface area of the belt meshing with the surface area of the pulley teeth. The greater the surface area the more torque it can transfer.

greater surface area = more traction between belt & pulley

If you want to use 3mm pitch the belt needs to be a minimum 15mm wide for a reasonable result. Any less and you will have the belt skipping along the teeth when accelerating & braking... Mostly the problems occur under braking as it requires much more force to stop the momentum. Accelerating is more of a gradual lowering of the load on the belt, braking is a rapid increase in load.

So basically if the belt is underrated for the desired load it will shred into pieces.

I wrote a little bit about this in my article about designing a drivetrain.

http://www.electric-skateboard.builders/t/beginners-guide-to-building-your-own-electric-skateboard-drivetrain/53


here is the snippet:

> QUICK NOTE ABOUT PULLEY TEETH PITCH
> There is a way to have a smaller pulley & also maintain high reduction ratios. The most common tooth pitch for electric skateboards is 5mm Pitch. Tooth pitch is the measurement between two teeth. So if I had a pulley with just 10 teeth at 5mm pitch the circumference would be 50mm. If I had a pulley with 10 teeth at 3mm pitch the circumference would be just 30mm. So what this means is you can use a smaller pitch & increase the number of teeth and have a pulley that is actually smaller in circumference. So I could have a 15 teeth pulley at 3mm pitch with 45mm circumference. This is advantagous as you can have much larger reduction ratios and have the pulleys fit onto a smaller wheel. But there is a trade off! the smaller teeth can't transfer the same amount of torque as the big teeth so you can get belt slipping issue. Running with 5mm pitch wheel pulley and keeping the wheel diameter at 83mm is enough to ensure you get good reduction ratio & good ground clearance, the maximum number of teeth I recommend for the wheel pulley on an 83mm wheel is 36 teeth. As the amount of teeth increases so does the diameter of the pulley making it closer to hitting the ground which is bad.
```

---
## \#3 Posted by: claudiofiore88 Posted at: 2015-11-25T00:16:48.297Z Reads: 504

```
Hmm, interesting.  You did mention that you're coming out with 12mm belts soon.  I'm guessing they're 5 mm htd pitch.  Would a 5 mm htd 12 mm belt have better torque transfer than a 3 mm htd 15 mm belt?  What do the boosted boards use?  It looks like a 3 mm pitch to me, not sure of the width.
```

---
## \#4 Posted by: onloop Posted at: 2015-11-25T00:22:53.982Z Reads: 495

```
I think boosted is 3mm pitch, their belt is 15mm or maybe 18mm wide.

yes, I have come to realise that 5mm pitch is the best option. It's much more durable and can handle the torque we are driving with the big motors.
```

---
## \#5 Posted by: claudiofiore88 Posted at: 2015-11-25T00:28:34.723Z Reads: 481

```
Are there disadvantages in going with a 12 or 15 mm belt vs 9mm?
```

---
## \#6 Posted by: onloop Posted at: 2015-11-25T00:31:39.368Z Reads: 465

```
 1. Increased cost of belt & pulleys
 2. Increase friction / rolling resistance 
 3. Can't mount DR motors easily / need very short motors as 6355 won't have the space on a standard 184mm wide truck hanger
```

---
## \#7 Posted by: claudiofiore88 Posted at: 2015-11-25T00:34:08.204Z Reads: 440

```
Yikes!  Lots to think about.  Thanks, Jason.
```

---
## \#8 Posted by: onloop Posted at: 2015-11-25T01:11:48.776Z Reads: 427

```
YEP... lots to think about when building an eboard!...
```

---
## \#9 Posted by: trbt555 Posted at: 2015-11-25T07:07:36.118Z Reads: 416

```
Here is a very good belt selection guide to give you some insight:
[belt selection guide][1]


  [1]: http://www.sdp-si.com/D265/PDF/D265T146.pdf
```

---
## \#10 Posted by: torqueboards Posted at: 2015-11-25T08:07:18.600Z Reads: 407

```
15mm belts are nice riding def add to the resistance and harder to fit things with as well.
```

---
## \#11 Posted by: ElectrikSK8 Posted at: 2015-11-25T20:39:52.699Z Reads: 390

```
Ooo thanks for that belt selection guide! Great for a n00b like me.
```

---
## \#12 Posted by: willpark16 Posted at: 2016-05-24T05:28:33.196Z Reads: 326

```
so an XL pulley can work or cant?
```

---
## \#13 Posted by: lowGuido Posted at: 2016-05-24T06:13:42.365Z Reads: 319

```
XL pulleys work mate. even a 9mm XL will do an alright job on flats, but will struggle with hills.

noted that a HTD belt is superior...
```

---
## \#14 Posted by: 91Seconds Posted at: 2016-06-18T11:08:14.662Z Reads: 293

```
I was wondering about all this different belt specs but every resource seemed to be a super technical spec sheet endorsing a particular brand.  
http://file.lasersaur.com/docs-thirdparty/The_World_of_Timing_Belts.pdf
still pretty technical but explains stuff really well for example why are htd 5m different from 5.08mm XL belts is not only the pitch but the htd can carry more torque due to optimized tooth profile.  

interesting read for people who are interested.

TL;DR
if this post was too long to read prob not the right resource for you anyway
```

---
## \#15 Posted by: Lizardking0069 Posted at: 2016-06-19T13:46:24.772Z Reads: 271

```
This made me look for htd pulleys instead of xl.
```

---
## \#16 Posted by: b264 Posted at: 2017-12-28T18:29:26.729Z Reads: 123

```
What is HTD?
```

---
## \#17 Posted by: b264 Posted at: 2017-12-28T18:36:09.636Z Reads: 122

```
Apparently it means "High Torque Drive"

https://www.pfeiferindustries.com/documents/Timing%20Belt%20Tooth%20Profiles%20and%20Pitches.pdf

https://www.pfeiferindustries.com/documents/Timing%20Belt%20Tooth%20Profile%20and%20Pitch%20(Interchangeability).pdf
```

---
## \#18 Posted by: Wilsonliang777 Posted at: 2017-12-30T05:30:05.651Z Reads: 109

```
I began with htd3m belts and went to XL belts but at the end I ended up using htd5m belts.  I washed a lot of money and time buying  htd3m and XL belts and pulleys
```

---
