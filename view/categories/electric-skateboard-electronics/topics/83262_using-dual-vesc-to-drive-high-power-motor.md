# Using Dual VESC to drive high power motor?

### Replies: 15 Views: 691

## \#1 Posted by: skaterscooter Posted at: 2019-02-05T16:46:07.074Z Reads: 137

```
I'm in the process of making an electric gokart and want to use a powerful brushless motor (Ideally 10kW but looking around might be limited to 5kW by VESCs). Obviously no single motor vesc can deliver the 200A continuous current needed for this however the dual motor VESC 6.6 can (although it comes with a £250 price tag :( ). Would it work simply connecting the outputs in parallel? Or is there some more complicated way to get this to work?
```

---
## \#2 Posted by: J0ker3366 Posted at: 2019-02-05T17:06:49.588Z Reads: 136

```
https://freeflyrobotics.com/products/arc200
```

---
## \#3 Posted by: FredrikHems Posted at: 2019-02-05T17:29:45.729Z Reads: 126

```
Well trampa’s vesc (7?) can do 300A at 75V. Thats 22kW. 
http://www.trampaboards.com/single-vesc-75v-300a-in-cnc-t6-silicone-sealed-aluminum-box--the-most-powerful-vedder-electronic-speed-controller-ever-p-26293.html
```

---
## \#4 Posted by: skaterscooter Posted at: 2019-02-06T11:04:01.585Z Reads: 102

```
Hmmm, this looks like a possible option. Back to my original question, would paralleling up  a Dual Vesc 6.6 be possible as they' have similar price and performance?
```

---
## \#5 Posted by: janpom Posted at: 2019-02-06T11:29:18.206Z Reads: 98

```
IMO it's unlikely that would work. Dual VESCs are typically two independent VESCs put into a single enclosure (focbox unity is the only exception I know). Motor phases synchronization would be a problem.
```

---
## \#6 Posted by: Vanarian Posted at: 2019-02-06T13:04:00.283Z Reads: 83

```
If you use a 6 phases motor, yea. If you use a classic 3 phases, hell no.
```

---
## \#7 Posted by: skaterscooter Posted at: 2019-02-06T14:20:53.714Z Reads: 77

```
With regards to the FOC Box, (this one https://www.unikboards.com/en/boutique/focbox-motor-controller/). The constant current is 60A and the peak is 300A. With enough cooling (how much?), how far could this be pushed? Would 100-150A continuous be possible?
```

---
## \#8 Posted by: skaterscooter Posted at: 2019-02-06T14:26:40.650Z Reads: 78

```
If not, I'll probably go for the Arc200
```

---
## \#9 Posted by: Andy87 Posted at: 2019-02-06T16:23:54.799Z Reads: 70

```
You can have a look on those too
https://www.electric-skateboard.builders/t/monster-build-need-a-monster-controller-be-one-of-the-first-to-try-the-maytech-6-6-200a-esc-at-the-lowest-price-you-will-ever-see/82697?u=andy87
There no reviews now, so it’s not confirmed how much current they really can handle.

Regarding focbox, @Kug3lis is running his at 100-150a (please correct me if i‘m wrong) with custom heatsink case.
```

---
## \#10 Posted by: Kug3lis Posted at: 2019-02-06T16:34:35.273Z Reads: 64

```
Yeah o run those motors in high current setting here is screenshoot from yesterday small ride

![image|230x500](upload://eZlOFAcK54hVwu2bgGwPCwv2CFe.jpeg)
```

---
## \#11 Posted by: skaterscooter Posted at: 2019-02-06T17:41:39.825Z Reads: 55

```
Oooh! Haven't heard of these before but they look very promising. Very good power output for not too much. Isn't this basically a VESC 4.12 with a big heatsink though?Any idea how I could get my hands on one or contact the maker?
```

---
## \#12 Posted by: Acido Posted at: 2019-02-06T17:51:17.743Z Reads: 50

```
just find a 20s controller, or something like that
dont expect it to be cheap though
```

---
## \#13 Posted by: Andy87 Posted at: 2019-02-07T02:09:44.406Z Reads: 47

```
No it’s a vesc 6 based design.
You can ask @hyperIon1 if he still have some fire sale. That would be definitely cheaper than buying it directly from maytech.
```

---
## \#14 Posted by: Fungineers Posted at: 2019-02-07T07:22:30.586Z Reads: 40

```
I was thinking of building an e-gokart too. 
What kind of motor are you using and where are you buying it from? 
Also are you using high discharge batteries? i though i could just use laptop batteries (with a looott in parallel) since a gokart doesnt have as high instantaneous acceleration as an esk8board, and theres plenty of space for the extra batteries.
```

---
## \#15 Posted by: skaterscooter Posted at: 2019-02-07T08:22:20.694Z Reads: 36

```
For the motor, (depending on what VESC i can get) I'm thinking of getting one of these high power outrunner motors.
https://hobbyking.com/en_us/turnigy-rotomax-50cc-size-brushless-outrunner-motor.html
https://hobbyking.com/en_us/turnigy-rotomax-100cc-size-brushless-outrunner-motor.html
https://hobbyking.com/en_us/turnigy-rotomax-150cc-size-brushless-outrunner-motor.html

They can be extremely powerful and should give some pretty insane performance. Fingers crossed! 
For the batteries, Li-ion would definitely be the ideal way to go. Only issue is the amount I would need to get some decent range. You could certainly try old laptop batteries but the quality can be a bit hit and miss as I found out when building my ebike! I've now switched to 4 li-po batteries in a 10s 2p configuration and although range isn't great, the discharge rates are more than enough. <110A!

Keen to hear how you get on
```

---
