# Foc brakes cutting out with drv error

### Replies: 32 Views: 374

## \#1 Posted by: 12meterkuk Posted at: 2018-12-25T06:52:31.945Z Reads: 92

```
![image|374x500](upload://j3U1vsjtjKugiparBED2YSCKRTx.jpeg) 


Been getting these errors in foc mode, anyone knows how to solve it? Brakes would cutout. 

Tried halving and doubling observer gain with no difference in results.

Does the same thing with different motors
```

---
## \#2 Posted by: Andy87 Posted at: 2018-12-25T06:58:35.245Z Reads: 90

```
vesc4, 6, dual, focbox ?
```

---
## \#3 Posted by: 12meterkuk Posted at: 2018-12-25T06:59:25.863Z Reads: 89

```
Single 4.12
```

---
## \#4 Posted by: Andy87 Posted at: 2018-12-25T07:01:26.254Z Reads: 86

```
which brand, with heatsink?
hw4.12 doesn´t like FOC usually (as min the cheap versions)
it´s only while braking, just to double check that, right?
what´s your max min settings?
```

---
## \#5 Posted by: 12meterkuk Posted at: 2018-12-25T07:02:25.430Z Reads: 85

```
Yes with heat sink. Maytech made. I’ve just been turning the wheel by hand while braking and this happens.
```

---
## \#6 Posted by: 12meterkuk Posted at: 2018-12-25T07:02:54.377Z Reads: 83

```
90 and 60 motor max and min, 40 and 40 batt max and min
```

---
## \#7 Posted by: 12meterkuk Posted at: 2018-12-25T07:03:13.414Z Reads: 82

```
Current in when braking cuts out at about 15a
```

---
## \#8 Posted by: Andy87 Posted at: 2018-12-25T07:04:09.050Z Reads: 81

```
switch to bldc and check if it´s happening there too.
did you check that there no bad/cold solder points and that all connections properly? bullet connectors pluged together totally, xt90 plugged in 100% etc.
```

---
## \#9 Posted by: 12meterkuk Posted at: 2018-12-25T07:04:55.149Z Reads: 80

```
Yeah everything is solid, BLDC works great, been riding on it but hall sensors only detect in foc so I want to switch to that.
```

---
## \#10 Posted by: Bjork3n Posted at: 2018-12-25T08:21:37.417Z Reads: 76

```
You can't run foc on maytech vesc, they are super unstable in Foc. 
Bldc mode and you'll be fine.
```

---
## \#11 Posted by: 12meterkuk Posted at: 2018-12-25T12:03:26.624Z Reads: 63

```
So went back to BLDC, getting drv errors on instantaneous full throttle. What the hell. 

Any ideas?
```

---
## \#12 Posted by: Andy87 Posted at: 2018-12-25T12:11:04.052Z Reads: 62

```
maybe you already broke your DRV during the time you was playing with FOC.
```

---
## \#13 Posted by: Friskies Posted at: 2018-12-25T12:14:03.075Z Reads: 60

```
Your settings are way to high. Lower them to 30 and 20 motor min max and try again. Do this in bldc unless you have Enertion or ollin vescs.
```

---
## \#14 Posted by: 12meterkuk Posted at: 2018-12-25T12:22:51.008Z Reads: 60

```
Don’t think so, it works fine if I don’t full throttle instantly. If I give it 80% doesn’t cut out.
```

---
## \#15 Posted by: 12meterkuk Posted at: 2018-12-25T12:23:40.058Z Reads: 57

```
It was running these settings fine before with an unsensored motor. I guess it didn’t  throw this fault since I physically couldn’t throttle all the way instantly from a standstill without cogging
```

---
## \#16 Posted by: Andy87 Posted at: 2018-12-25T12:25:26.774Z Reads: 56

```
which motor and voltage you running_
if its 12s at 190/200kV it could be your problem if you didn't set an erpm limit.
```

---
## \#17 Posted by: 12meterkuk Posted at: 2018-12-25T12:26:34.045Z Reads: 55

```
9s 210kv. I think erpm should be ok. Old Motor was 210kv too it cuts out long before I hit full speed. Like half a second after throttling to full from a standstill
```

---
## \#18 Posted by: 12meterkuk Posted at: 2018-12-25T12:29:38.670Z Reads: 57

```
Right now I’m thinking it might just be a bad VESC from the start, just that I didn’t catch the problem before when using an unsensored  motor
```

---
## \#19 Posted by: Bjork3n Posted at: 2018-12-25T12:32:11.131Z Reads: 56

```
From my testing maytech vesc can only handle around 30A on battery max. If you do over this it will cut out on full throttle. At least this was the case for me.
```

---
## \#20 Posted by: 12meterkuk Posted at: 2018-12-25T12:33:35.365Z Reads: 53

```
I’ve seen 40a on my telemetry before, albeit not instantly throttling to full from a stop before. No errors then.
```

---
## \#21 Posted by: Bjork3n Posted at: 2018-12-25T12:36:04.357Z Reads: 51

```
When i used maytech dual vesc i used the following settings with no issues.
Motormax : 60A
Motormin : -40A
Batterymax : 30A
Batterymin -8.

I found these settings was reliable with the maytechs.. as soon as i went over 30A on battery max i had cutouts and problems as soon as i pushed hard.
```

---
## \#22 Posted by: 12meterkuk Posted at: 2018-12-25T12:37:03.441Z Reads: 51

```
I’ll try 30a later, thanks!
```

---
## \#23 Posted by: Friskies Posted at: 2018-12-25T13:15:58.933Z Reads: 51

```
If you run these it should work fine. I would probably increase battery min to about 20 or so but that depends on what batteries you are using. With vescs you pretty much get what you pay for. If you want to run higher limits you will need to "invest" in it.
```

---
## \#24 Posted by: 12meterkuk Posted at: 2018-12-25T22:47:40.099Z Reads: 40

```
So I did 30 and 25 for batt current and it still cuts out. Feels bad man.
```

---
## \#25 Posted by: 12meterkuk Posted at: 2018-12-25T22:48:53.067Z Reads: 40

```
As I said earlier this seems to be a dud vesc as I’ve been running 40a with no issues on an unsensored motor. . Issue only happens when I peg the throttle instantly which I couldn’t do with an unsensored motor instead of slowly ramping up to full
```

---
## \#26 Posted by: 12meterkuk Posted at: 2018-12-25T22:54:45.665Z Reads: 40

```
Going to try another firmware now
```

---
## \#27 Posted by: 12meterkuk Posted at: 2018-12-25T23:31:30.415Z Reads: 39

```
Went from 3.38 to ackmaniac and still having the same problem. I think it’s just a hardware issue now.
```

---
## \#28 Posted by: YungDaff Posted at: 2019-06-04T17:27:52.341Z Reads: 22

```
Burying up this old thread while searching for any answer to why I got this error. Running FOC on a maytech VESC will probably not work at all and could lead to permanent damage on the VESC. So to anyone reading this be aware of this before attempting it.
```

---
## \#29 Posted by: mixedcreation Posted at: 2019-06-04T18:35:27.064Z Reads: 18

```
Not true.  I have a Maytech VESC that I have run on FOC for over 4 months.  BLDC ran it for 2 months.  

60,-60,40, -12.

on a 10s3p battery. 

Don't put a blanket statement as all Maytech VESC's aren't created equally.  My 100a has been solid from day 1.
```

---
## \#30 Posted by: Sn4pz Posted at: 2019-06-04T21:48:30.330Z Reads: 14

```
you should edit your post to reflect the specific hardware / version of the VESC you are talking about, as there are multiple maytech VESCs
```

---
## \#31 Posted by: YungDaff Posted at: 2019-06-04T21:50:28.446Z Reads: 14

```
@Sn4pz @mixedcreation My bad. I meant the single 50A one. The 100A might be more solid. Also I might have gotten a bad unit, I regret making that statement.
```

---
## \#32 Posted by: Sn4pz Posted at: 2019-06-04T21:54:51.623Z Reads: 14

```
all good my dude. Whether a 4.xx VESC can run FOC is entirely up to chance. My TB 4.12 VESCs (sold to me around December 2017) ran FOC perfectly, yet people who bought them before and after I did, struggled with FOC and blown DRV chips. 

It feels very 'silicone lottery'-ish to me, unless there is difference in the precision of soldering / manufacturing that no one has noticed yet
```

---
