# No battery, super fast charging

### Replies: 14 Views: 1629

## \#1 Posted by: im-done Posted at: 2016-10-22T21:14:02.228Z Reads: 190

```
So i was wondering if you could make a super capacitor based board. The encloser would have two tabs so you just dock the board and the caps charge in under 5 mins. The only thing is you would have little range, but the way i see it when you buy your coffee plug it in kinda thing. It would charge so fast you wouldnt need to wait long. 

So does any one have any experice with super caps? I have basic knoledge of caps and their benifts/dangers. I was thinking of about 1,000-2,000f at 36 v.
```

---
## \#2 Posted by: Monte Posted at: 2016-10-22T21:20:12.223Z Reads: 186

```
Doesnt capacitors loose its energy if they are not plugget in?
```

---
## \#3 Posted by: im-done Posted at: 2016-10-22T21:22:21.282Z Reads: 186

```
Wrong they have a super low internal residence. The problem is that when they run they drop volts faster than lithium, but you can run them to 0v with no issue and they have the highest discharge ever.
```

---
## \#4 Posted by: Monte Posted at: 2016-10-22T21:24:52.720Z Reads: 185

```
I actually have just basic knowledge of capacitors :sweat_smile: But its sounds like it should work.
```

---
## \#5 Posted by: whitepony Posted at: 2016-10-22T21:30:51.256Z Reads: 176

```
well, yea, the energy stored in a cap is 0.5*C*U^2, i.e.1F cap at 36V stores just 650watt.

a rather small skateboard battery has 100Wh (boosted), i.e. to store that kind of energy means, you need 100Wh = 3600*100Ws = 360.000Ws, i.e. 360.000/650 = 500-600F. so you got that number halfway right, but I think you dont know how large these caps actually are. this here is the 2F cap Im using for spot welding - its about as thick as my lower arm and it nearly has its length :sweat_smile:

http://www.alternative-4.com/evolvecarbon/spotwelder1.jpg
```

---
## \#6 Posted by: smurf Posted at: 2016-10-22T21:31:49.342Z Reads: 167

```
The electric power motorcycle speed record was set with a bike that used super capacitors. While ideal for a quarter mile run their cost prohibitive.
```

---
## \#7 Posted by: SimosMCmuffin Posted at: 2016-10-22T21:54:29.914Z Reads: 160

```
Aside from the huge energy capacity difference between solid state capacitors and chemistry based energy storing batteries weight and volume wise.
Caps don't have a steady output voltage like normal batteries do, which usually for example with Li-Ion and Li-Po is about 3.6 - 3.7. Your capacitors voltage would slowly drop from 36 V towards 0 V. When you have spent half of the capacitor's stored energy you would have only ~25.5 V left.

[quote="smurf, post:6, topic:11705, full:true"]
The electric power motorcycle speed record was set with a bike that used super capacitors. While ideal for a quarter mile run their cost prohibitive.
[/quote]

I couldn't find anything with a google search about this. Care to link to a source?
```

---
## \#8 Posted by: smurf Posted at: 2016-10-22T22:38:23.913Z Reads: 150

```
http://www.nedra.com/build.html

https://youtube.com/watch?v=3ErAqgNI58Q
```

---
## \#9 Posted by: Pablo_702 Posted at: 2016-10-22T22:41:41.548Z Reads: 146

```
At one point inwas going to do a vape box mod with this concept
```

---
## \#10 Posted by: SimosMCmuffin Posted at: 2016-10-22T22:50:42.344Z Reads: 139

```
I wouldn't exactly call their results record breaking and that is ignoring the fact that most of their battery setups had both batteries and capacitors in parallel.

> TCC EV Capacitor Testing History:
> Fall of 2008 - 32V @ 25F in parallel with 24V Pb.
> 2010 - 32V @ 54F switched in/out with 70V LiFePO.
> 2013 - Capacitor only 75V @ 50F followed with
> switching in a 120V @ 54F bank (1/4 mi 16sec).
> 2014 – Switched to a capacitor hybrid PS:
> 144V Pb and a 163V @ 10F bank switch in/out
> (best 1/4 mi 13.7s). Bike weighed 550lbs w/Pb.
> 2015 – LiPo’s+Pb

Also that video, doesn't tell what that particular bikes power system is comprised of, probably normal batteries and caps as well.
```

---
## \#11 Posted by: im-done Posted at: 2016-10-23T02:28:33.516Z Reads: 111

```
A lot of number + just got off work = confused.

But i do see your point about size and farads.
```

---
## \#12 Posted by: im-done Posted at: 2016-10-23T02:33:18.691Z Reads: 111

```
https://www.ebay.com/itm/171875095563 

Whats about these caps it would be over $300 to make a 36v pack but it would be 1,400F so it would get some range correct?
```

---
## \#13 Posted by: saul Posted at: 2016-10-23T02:46:25.203Z Reads: 110

```
actually @monte is right, caps have a leakage current, but its usually days to weeks so not a problem in this case because you would charge quick and go ride right away.

The problem is like whitepony said super caps are just TOO BIG.

li ion have a specific density of about 100-250wh/kg
Super/ultra cap 5-10wh/kg.
thats 10-50x the power for the weight.

you can see from the caps you posted they are about 1.2whr each x 15(37.5V) = 
18wr = = 1-2 miles? or **one really high power speed run!?**
----------

The reason is when you add caps in series to get higher voltage the capacitance is 
1/c = 1/c1 + 1/c2

it actually shows on the page
6 capacitors of 1400F/2.5V in series connection
C=1/(1/1400+1/1400+1/1400+1/1400+1/1400+1/1400)=233F
V=2.5V*6=15v

hopefully someday soon carbon nanocapacitors will blow away liion density but till then....
```

---
## \#14 Posted by: drangboards Posted at: 2018-11-12T13:11:42.510Z Reads: 32

```
Check out Stephane Fife.  I’m sending him some carbon and associated materials for testing. https://youtu.be/CvCw3OeNUZk
```

---
