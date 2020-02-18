# Would this ESC be enough?

### Replies: 8 Views: 228

## \#1 Posted by: matfrags Posted at: 2019-07-09T13:33:05.227Z Reads: 108

```
im trying to build my first electric board this summer(because ive got nothing better to do) and i was planning to use turnigy's Turnigy SK8 6374-192KV Sensored Brushless Motor (14P) coupled with their Turnigy SK8-ESC V4.12 For Electric Skateboard Conversion w/BEC, the only problem is that some of the reviews have commented on the ESC'S tendency to throttle power output to avoid overheating
i think that this problem would be worsened in my case as im planning to run 4kw through this tiny board.
my question is:is it up to the task or should i search for somethinng else?
```

---
## \#2 Posted by: Chemlut Posted at: 2019-07-09T16:23:08.399Z Reads: 90

```
No not really, the esc only supports up to 50 amp continous, and i wouldnt recommend pushing much higher than that. I have the same motor with a vesc 4.12 and power wise the 2kw that vesc allows is plenty for a beginner though the braking power is a bit lackluster. So if you really wanna get the 4kw out of the motor you will have to get i vesc 6 i guess ;D
```

---
## \#3 Posted by: Dirt_Bag Posted at: 2019-07-09T17:57:29.385Z Reads: 78

```
A better option is to go with the flipsky vesc 4.20 mini.

Its very reliable and cheap
```

---
## \#4 Posted by: leroy Posted at: 2019-07-09T23:01:21.153Z Reads: 62

```
I have that motor, I used it with a 50 amp vesc and it was good, 
then I used it with an 80 amp Graupner ESC, and it is amazing. 

If you are going to use a VESC, get one made by one the guys here, 
there are several that make them very well.  

Don't be an dumb ass, cheap should not the primary criteria for a speed controller.
```

---
## \#5 Posted by: Schulerbible Posted at: 2019-07-09T23:03:55.653Z Reads: 52

```
I have that vesc on the old Enertion RSpec motor (6354) and it's great. If you don't have a battery which dumps out a lot of amps, you also don't run the Vesc at its limit!
```

---
## \#6 Posted by: matfrags Posted at: 2019-07-10T06:09:28.929Z Reads: 40

```
The set of batteries I'm planning to use will be dumping about 150 amps into the circuit so it's probably not ideal
```

---
## \#7 Posted by: meesie Posted at: 2019-07-10T08:15:28.309Z Reads: 32

```
[quote="Dirt_Bag, post:3, topic:98125, full:true"]
A better option is to go with the flipsky vesc 4.20 mini.

Its very reliable and cheap
[/quote]

i back this. i bought them for about $55 bucks a piece on aliexpress and i run them on 12S in FOC without any problems. they handle 50 amps which in my opinion is more than enough.

[quote="matfrags, post:6, topic:98125, full:true"]
The set of batteries I’m planning to use will be dumping about 150 amps into the circuit so it’s probably not ideal
[/quote]
 your battery can handle these loads, but will you be using all that energy? if i accelerate *hard* with my board i pull about 45 battery amps max. which relates to about 90 motor amps with my setup.

[quote="matfrags, post:1, topic:98125"]
ESC’S tendency to throttle power output to avoid overheating
[/quote]

this is a setting that you can adjust in every VESC
```

---
## \#8 Posted by: Sn4pz Posted at: 2019-07-10T13:26:56.119Z Reads: 21

```
[quote="matfrags, post:1, topic:98125"]
commented on the ESC’S tendency to throttle power output to avoid overheating
[/quote]

In my experience this has only happened at around 80c-85c... And that's hella hot. If you use some sort of cooling for your vescs you probably will never see those types of numbers, but even then the throttling is to preserve hardware... Do you want to constantly be replacing melted vescs? :p
```

---
