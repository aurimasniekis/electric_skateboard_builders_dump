# Vesc tunning help

### Replies: 17 Views: 116

## \#1 Posted by: Forklift Posted at: 2019-05-16T05:49:49.798Z Reads: 35

```
Hello Everyone

My name is Dylan and I am building an electric mountain board.  I have a dual 6374 190kv motors with 2 vesc connected to 3. 4s 6000mAh 14.8v 50c lipos so, 12s total in parallel.  The reason for the post is i wanted some help because my wheels spin but, i want to get the most out of the board.  I have a 12t pinion gear and a 48t sprocket. So any advice that would be great thanks.
Dylan
```

---
## \#2 Posted by: taz Posted at: 2019-05-16T05:54:07.666Z Reads: 35

```
The size of you wheels (200mm , 250mm something else?),  the type of transmission (chain, belts, gears), your terrain (flat, hilly) etc would help in order to provide better suggestions.
```

---
## \#3 Posted by: Jinra Posted at: 2019-05-16T05:55:50.879Z Reads: 32

```
[quote="Forklift, post:1, topic:93997"]
12s total in parallel
[/quote]

I think you mean series.

What are you asking for? settings? something else?
```

---
## \#4 Posted by: Forklift Posted at: 2019-05-16T05:56:14.259Z Reads: 30

```
Hey Taz 
They are 200mm and it is chain driven.  Mostley flat.
```

---
## \#5 Posted by: Forklift Posted at: 2019-05-16T05:56:47.633Z Reads: 29

```
Looking mainly for setting.
```

---
## \#6 Posted by: Jinra Posted at: 2019-05-16T05:59:42.430Z Reads: 28

```
What VESCs are you using? If you're using something with decent heatsinks you could try this as a baseline (per VESC) and go from there.

60/-60/50/-10

motor max/motor min/battery max/battery min
```

---
## \#7 Posted by: Forklift Posted at: 2019-05-16T06:01:55.634Z Reads: 26

```
Im using Torque boards bdlc vesc
```

---
## \#8 Posted by: taz Posted at: 2019-05-16T06:02:45.456Z Reads: 28

```
You have 4:1 gearing which although a little tall for 200mm wheels, if you ride in flat terrain it should be fine.

Do you want us to suggest vesc settings? If so then you need to provide more details on the components, cooling etc.

Some base figures are 80A bat / 60A motors -40A bat /-40A motors
```

---
## \#9 Posted by: Andy87 Posted at: 2019-05-16T06:04:11.733Z Reads: 27

```
[quote="taz, post:8, topic:93997"]
80A bat
[/quote]

[quote="Forklift, post:7, topic:93997"]
Torque boards bdlc
[/quote]

I wouldn´t go higher than 35A batt max on tb vesc without any additional heat sink or cooling.
```

---
## \#10 Posted by: taz Posted at: 2019-05-16T06:05:23.541Z Reads: 27

```
True. I had the total battery amp draw in mind when I wrote this, the way unity is setup.
```

---
## \#11 Posted by: Forklift Posted at: 2019-05-16T06:06:08.926Z Reads: 29

```
Cool I have to give these settings a try.  I currently have no cooling at the moment.
```

---
## \#12 Posted by: Andy87 Posted at: 2019-05-16T06:08:03.692Z Reads: 29

```
[quote="taz, post:8, topic:93997"]
70A bat / 60A motors -40A bat /-40A motors
[/quote]

than take this settings and set the half of the batt value in each vesc. the vescs are in parallel so they the totall batt amps add up, keep that in mind.
```

---
## \#13 Posted by: Forklift Posted at: 2019-05-16T06:09:10.873Z Reads: 27

```
Will do. Thanks Andy87
```

---
## \#14 Posted by: Andy87 Posted at: 2019-05-16T06:12:00.273Z Reads: 26

```
sorry,small edit....
only the batt amps are half half.

the motor amps are for one side :sweat_smile:

so to not confuse you, it´s like this in each vesc:

batt max 35A

batt min -20A (would start with -15A)

motor max 60A

motor min -40A (if brakes too weak set it to -50A)
```

---
## \#15 Posted by: taz Posted at: 2019-05-16T06:15:30.248Z Reads: 25

```
To help you further adjust keep in mind the following:

If your high speed brakes are too strong increase regenerative battery value (eg go from -35A to -20A).

If your low speed brakes are too strong increase the negative motor value.
```

---
## \#16 Posted by: Forklift Posted at: 2019-05-16T06:16:02.764Z Reads: 23

```
Cool thanks
```

---
## \#17 Posted by: Forklift Posted at: 2019-05-16T06:16:52.452Z Reads: 21

```
Thanks Andy87
```

---
