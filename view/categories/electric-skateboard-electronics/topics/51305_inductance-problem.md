# Inductance problem?

### Replies: 13 Views: 506

## \#1 Posted by: BooYA Posted at: 2018-04-05T14:37:25.474Z Reads: 104

```
Hi everyone,
I need a bit of advice building a 12s setup with a focbox.
I'm concerned about an inductance issue that might occur due to the length of the wires. 
I read that I should avoid cables longer than 30cm,
But in my case there is only one polarity which has to be quite long ( 50cm).  
Also it worth mentioning that I'm using large flat copper tape, 5cm by 0.065mm thickness.
And I know using flat cables next to one another will prevent huge inductance. 
Still, what do you guys think about that? 
Thanks for you inputs 
![Screenshot_2018-04-05-16-27-22|281x500](upload://6blyBVHILZacCxAjHG8I24cM7dI.png)
```

---
## \#2 Posted by: koralle Posted at: 2018-04-05T14:53:48.839Z Reads: 84

```
1. Inductance does not discriminate when it comes to polarity so I dont thing that is relevant.
2. All the copper inlaid boosted inspired people use wires that are longer than 50cm and I have not heard of any problems so far.
```

---
## \#3 Posted by: fraannk Posted at: 2018-04-05T15:06:22.071Z Reads: 84

```
I built a Boosted clone with fairly long wires, and I have never had a problem. They seem to have more influence when running FOC, and I'm currently upgrading it to FOC, so we'll see. :)
```

---
## \#4 Posted by: rok Posted at: 2018-04-05T15:17:57.557Z Reads: 74

```
Thats what im afraid of. I also have a boosted like board and the thing ran perfectly fine on bldc with 4.12 vesc. I switched to FOC and all of a sudden the vesc was overheating.
I'll report back when i test it with FOCBOX.
```

---
## \#5 Posted by: Hummie Posted at: 2018-04-05T15:23:25.158Z Reads: 63

```
I didn't do the math but thickness of the wire effects the inductance too    what size equivalent cylindrical wire would you be using?
```

---
## \#6 Posted by: Exiledd_Top Posted at: 2018-04-05T15:24:36.711Z Reads: 66

```
I've never incounterd  that problem with my 4wd and it's a 39inch deck and from one end to another  running foc with no problem but I think this because am using 10awg
```

---
## \#7 Posted by: rok Posted at: 2018-04-05T15:29:15.642Z Reads: 66

```
Did you ran 4.12 vescs at any point? I'm also using 10 awg.
```

---
## \#8 Posted by: Exiledd_Top Posted at: 2018-04-05T15:30:48.218Z Reads: 62

```
Am running 4x focbox 
With 10awg and a battery of 12s6p 30qp
![20180224_214610|374x500](upload://jXSU11O84h0qLgVrv7mVpUSmort.jpg)
Here's a basic layout without the cables
```

---
## \#9 Posted by: rok Posted at: 2018-04-05T15:32:49.695Z Reads: 61

```
Good to know. My hopes are high. :grinning:
```

---
## \#10 Posted by: BooYA Posted at: 2018-04-05T15:35:29.901Z Reads: 59

```
6mm2 so basically very big wire XD cause I'll double each wire
```

---
## \#11 Posted by: BooYA Posted at: 2018-04-05T15:43:13.796Z Reads: 57

```
Also is there any issue with 50cm canbus wires?
You guys are truly helpful!
```

---
## \#12 Posted by: Exiledd_Top Posted at: 2018-04-05T15:54:05.103Z Reads: 53

```
I steer away from canbus in my opinion don't like the fact that if one vesc dies u have another perfectly fine vesc that is useless if it happens while riding. I always use ppm y splitters, with my 4wd it was a no brainer that ppy y splitter for 4 vesc far away from each other was impossible to do I did 2 receivers and 2 ppm y splitters but I have then switched to 4 receivers one per vesc for more redundancy.
```

---
## \#13 Posted by: Grabacr Posted at: 2019-09-05T01:13:11.597Z Reads: 10

```
Hi everyone,

I've recently received my Unity and I've been trying to get everything set up for the past few weeks, but I keep running into the same error and haven't found a solution. When running the motor detection I keep getting the error "L is 0. Please measure it first." Has anyone had a similar issue or know of a solution? Any help would be greatly appreciated. I've been working on this project for more than six months and am desperate to get out and ride.
```

---
