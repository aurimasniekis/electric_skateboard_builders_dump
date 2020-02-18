# VESC-X Lab test

### Replies: 13 Views: 1815

## \#1 Posted by: Blasto Posted at: 2016-11-04T16:56:51.993Z Reads: 233

```
Jason asked me to test out the Enertion Vesc-X in a lab environment.  http://www.enertionboards.com/?afmc=1o

TLDR here are the results:

was able to pull 40A at 50V before the motors would saturate and got a 30degC temperature rise. To go >40A @ 50V I would need to change up my motor jig to load up the system even more. So that's 2000W constant, and the Vesc-X temperature only raised to 50degC. That means there's another 50degC headroom and could probably handle up to 90-100A @ 50V constant!

Now my setup:

-15KW power supply
-Master-slave motor jig, slave motor has all phases shorted together (this motor was already burnt), the master motor drives the salve
-The slave motor will dynamically load up the master motor until it saturates, in this case the maximum load was 50V@40A

<img src="/uploads/db1493/original/3X/b/5/b56b13d74922ec51753b0237ac8d6473a7d41479.JPG" width="666" height="500"><img src="/uploads/db1493/original/3X/9/b/9b1d242563da7bf7481baf42a9a6cc9debc47451.JPG" width="666" height="500">

BLDC:
 https://youtu.be/hOnVNkxX694

FOC:
http://www.youtube.com/watch?v=C8nPuBvnVXM

I will try to find some bigger motors to ramp up the current even more... but do i really need to?
```

---
## \#2 Posted by: Michael319 Posted at: 2016-11-04T16:59:15.689Z Reads: 223

```
Check your video link.
```

---
## \#3 Posted by: Blasto Posted at: 2016-11-04T17:00:00.133Z Reads: 220

```
[quote="Michael319, post:2, topic:12461, full:true"]
Check your video link.
[/quote]

what do you mean? it's not working? give it 2-3 mins...

ok fixed, thanks
```

---
## \#4 Posted by: E-Boarding Posted at: 2016-11-04T19:03:44.863Z Reads: 195

```
Test in FOC-mode under heavy load please
```

---
## \#5 Posted by: treenutter Posted at: 2016-11-04T20:24:54.056Z Reads: 181

```
@Blasto I agree w @E-Boarding that an FOC test would be great. Even more helpful with a 6374-sized motor at 10S.

BTW @Blasto did you solder together the three motor wires to create resistance for the other motor to push against? That's a really clever testing jig!
```

---
## \#6 Posted by: SirDiff Posted at: 2016-11-04T20:28:25.226Z Reads: 175

```
I would like to see a 6374 at lower voltages, like 6-8s to see how does it manage more amps
```

---
## \#7 Posted by: JohnnyMeduse Posted at: 2016-11-04T20:28:25.712Z Reads: 171

```
He is already doing is test at 12S
```

---
## \#8 Posted by: Okami Posted at: 2016-11-04T20:31:47.797Z Reads: 166

```
if this vesc can take more amps I assume it would be now better suited for emountainboard use compared to the ''original vesc's'' since a lot of ppl not recommend them for mountainboard use ;)
```

---
## \#9 Posted by: SirDiff Posted at: 2016-11-04T20:35:01.924Z Reads: 163

```
Yeah, or single motor builds which happen to have some overheating problems at lower voltages with normal vescs, climbing hills or accelerating fast
```

---
## \#10 Posted by: treenutter Posted at: 2016-11-04T20:42:52.819Z Reads: 156

```
Oh ha, my mistake thanks @JohnnyMeduse
```

---
## \#11 Posted by: Blasto Posted at: 2016-11-04T20:43:13.136Z Reads: 155

```
@E-Boarding @treenutter
Foc mode, sorry i jumped in the video, i saturated the slave motor trying to go over 40A

  http://www.youtube.com/watch?v=C8nPuBvnVXM
```

---
## \#12 Posted by: Blasto Posted at: 2016-11-04T20:47:11.366Z Reads: 153

```
[quote="treenutter, post:5, topic:12461"]
BTW @Blasto did you solder together the three motor wires to create resistance for the other motor to push against? That's a really clever testing jig!
[/quote]

Yes, i had a motor with two shorted phases, so i didn't feel bad shorting the leads... up-cycling

@SirDiff i'm trying to show how much power it's able to handle. With my current motor jig i'm able to handle 2000W no problem

I won't start testting this and that motor... unless you guys send it to me. Next step would to crank up my motors on my jig... would it be necessary...

@Ackmaniac would your modified version of the bldc tool show the ouputted power in the real time data?
```

---
## \#13 Posted by: Ackmaniac Posted at: 2016-11-04T21:06:53.739Z Reads: 149

```
Sure, works as normal. So you can even verify that in watt mode the VESC only uses like 50% of the max watts at 50% throttle. But you only can see that when the motor has load which you are going to test as it seems.
```

---
