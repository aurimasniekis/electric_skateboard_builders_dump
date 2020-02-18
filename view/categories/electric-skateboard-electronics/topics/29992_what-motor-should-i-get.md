# What motor should I get?

### Replies: 11 Views: 1049

## \#1 Posted by: taycro Posted at: 2017-08-07T21:54:12.275Z Reads: 123

```
I am fairly new to the ESK8 community and I am working on building my first board. I am having a hard time deciding what motor to get?

I am only going to have 1 motor. It needs to be able to handle hills with ease. I would like it to get my boards to 25mph+. Can anyone give me suggestions or point me in the right direction.

Thanks for reading this. I could really use some help.
```

---
## \#2 Posted by: gliz5714 Posted at: 2017-08-07T22:00:17.673Z Reads: 121

```
I would highly recommend reading up on a BUNCH of build threads to know what goes into making up that speed.  However, once you kind of have a general build idea (in terms of wheel size, gearing, motor) check it here:

http://calc.esk8.it/

This will give you the final output numbers you are wanting.  I saw you posted in another thread about batteries, so I can give you a general rule that if you want to go with 6s (6 batteries in series) you will have to go with a HIGH kv (250-300) to reach anywhere near 25mph.

Basically put, speed is combo of MANY different parts ranging from pulleys to wheel size to motor size to battery output.

Read up and use the calculators to see what other people are doing to make sure it works!
```

---
## \#3 Posted by: rich Posted at: 2017-08-07T22:40:28.989Z Reads: 108

```
We were all in the same boat in the beginning.:wink:
Like @gliz5714 mentioned, you should read a lot about everything before starting to buy THE RIGHT things. The worst you can do is to rush. I lost a lot of money because of buying wrong or cheap parts in the beginning without enough knowledge.

At least for little help:
- If you wanna climb hills get a 6374 motor e.g. 190kv (with 10s)
- good motor pulley size is 15T, for 80-90mm wheels get something between 32-40T
- get a motor/pulley with keyway
- my top speed with 190kv motor and 15/32 pulleys on 80mm wheels and 10s was about 28-30 mph.
- get a quality V4.12, no cheap one (I bought six and can use the 2 quality ones only)
- think about 10s battery and get a bypassed bms + li-ion charger (is together even cheaper than a balance charger from hobbyking and much easier to charge) You can put lipos in parallel to reach 10s.
The problem with 6s is that it sucks much more ampere from your battery than with 10s so you get less watt from the motors and heat up the V4.12's much quicker. With 6s you would need a motor with more kv to reach 25 mph+
- with 10s and 5000maH your range would be about 12-13 miles or a liitle less depending on hills and the way you accelerate.

But to make a proper build you need more knowledge before starting, have fun!
```

---
## \#4 Posted by: taycro Posted at: 2017-08-10T23:34:22.245Z Reads: 73

```
Is this a good V4.12? diy-electric-skateboard-kits-parts/vesc-the-best-electric-skateboard-esc/
```

---
## \#5 Posted by: jammin Posted at: 2017-08-11T01:06:23.285Z Reads: 71

```
I'm running the Torque VESC with BLDC with zero issues so far.
```

---
## \#6 Posted by: taycro Posted at: 2017-08-11T01:07:44.579Z Reads: 70

```
That's what I sent you right?
```

---
## \#7 Posted by: jammin Posted at: 2017-08-11T01:12:41.425Z Reads: 69

```
tbh not sure, I just got back from my travels :confused:
```

---
## \#8 Posted by: gliz5714 Posted at: 2017-08-11T01:49:38.291Z Reads: 65

```
Yes, torqueboards is what you sent.  They make a fine standard VESC.  Not sure if it is updated with more beefy parts but I haven't heard anything bad about them.
```

---
## \#9 Posted by: jammin Posted at: 2017-08-11T01:54:38.657Z Reads: 61

```
definitely a standard VESC (nothing like the FOCBOXes). FWIR they're essentially maytech VESCs with the bootloader.
```

---
## \#10 Posted by: Ulfberht Posted at: 2017-08-11T02:39:03.007Z Reads: 55

```
I have my eyes on this beast. It's pretty bad ass. You would really only need a single drive with this monster...
http://www.ollinboardcompany.com/product/om-6085-200kv
```

---
## \#11 Posted by: taycro Posted at: 2018-05-10T04:21:10.767Z Reads: 33

```
@onloop can you delete this thread of mine.
```

---
