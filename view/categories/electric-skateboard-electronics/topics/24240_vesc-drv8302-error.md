# VESC DRV8302 error

### Replies: 12 Views: 1276

## \#1 Posted by: Dalton_Dom Posted at: 2017-05-31T00:10:06.049Z Reads: 131

```
I was wonderning why my motor wasn't turning when i pulled the throttle. So I went and connected my vesc to the bldc tool and discovered that I recieved a DRV8302 error, when ever i pull the throttle on my remote. I currently use a 245kv motor with an 8S liion setup.I can provide pictures with my vesc configurations if needed.
```

---
## \#2 Posted by: sl33py Posted at: 2017-05-31T00:13:35.766Z Reads: 131

```
Sounds like a dead DRV chip most likely.  They are very sensitive to exceeding 60k ERPM and sometimes fail for no real reason (MTBF).

You can post pics of your settings for some of the gurus to check an comment on.

Might also include your wheel and gearing info (83mm - 245kv - 8s - 15/36 ?).  Run that on a speed calc to see how close to 60k ERPM you were - sometimes you are under the limit riding, but going downhill... and braking can be a killer.

GL!
```

---
## \#3 Posted by: Dalton_Dom Posted at: 2017-05-31T00:15:45.295Z Reads: 126

```
Yep those are my exact gearing info. Do you have a recomendation of what to do to prevent next time, because im assuming i will need to buy a new vesc. Who has the best vesc.
```

---
## \#4 Posted by: psychotiller Posted at: 2017-05-31T00:22:29.863Z Reads: 118

```
Best thing you can do if you are going to stay 8s:
Buy a lower kv motor
Best thing to do if you keep your motor:
Buy a 6s battery. 

Otherwise you are going to blow more drv chips.
```

---
## \#5 Posted by: sl33py Posted at: 2017-05-31T00:25:14.133Z Reads: 112

```
good guess (a standard "kit" setup helps)...  Running that on a calc i have, i see it as 50k ERPM - so not super close, but again if you were heading downhill braking it could've cooked the DRV.

I'd go for warranty fix first if available, then repair (if you can find someone), then new ESC.

Best?  I'd say VESC 6 as it's looking like it's removed the 60k ERPM issue and less likely to kill DRV chips from Ben's testing.  But $$$ relative to most 4.12 VESC's, and only available during the BETA from @Trampa / Frank.  Shoot him a PM and perhaps he has a spare if you don't mind the price.

Next i'd suggest a direct FET variant from @Chaka, or Enertion (VESC-X).

If you go with another 4.12 VESC, or even one of the direct FET variants - you might want to get a lower kv motor to avoid in the future.  

Where are you located - this might help us steer you towards vendors in your neighborhood?

GL!
```

---
## \#6 Posted by: psychotiller Posted at: 2017-05-31T00:37:19.839Z Reads: 103

```
Johnnyrepairservices@gmail.com for drv repair! $45
```

---
## \#7 Posted by: Dalton_Dom Posted at: 2017-05-31T00:39:25.998Z Reads: 105

```
Who is this person and how reliable or how long does this take? And even if I do this wont my DRV fry again?
```

---
## \#8 Posted by: JohnnyMeduse Posted at: 2017-05-31T00:46:08.575Z Reads: 104

```
I think... I Know who that guy might be :wink: And for reliability I guess it is pretty good... :stuck_out_tongue_winking_eye:

And it always depend on the quality of your VESC. 

https://www.electric-skateboard.builders/t/johnny-vesc-repair-services-now-with-soldering-tips/11267/18
```

---
## \#9 Posted by: Dalton_Dom Posted at: 2017-05-31T01:06:13.552Z Reads: 99

```
The vesc that I bought was from DIY Electric skateboard.
```

---
## \#10 Posted by: psychotiller Posted at: 2017-05-31T01:45:46.352Z Reads: 90

```
You repair fuckboxes? Sweet!
```

---
## \#11 Posted by: JohnnyMeduse Posted at: 2017-05-31T02:01:16.506Z Reads: 83

```
Yep... but don't mix them with BoxeOfFuck, I don't repair these, since they are too cheap.
```

---
## \#12 Posted by: sl33py Posted at: 2017-05-31T02:05:21.328Z Reads: 79

```
Can't speak to turnaround time, but he has a good reputation from what i've seen on the forum.  at 1/2 the cost of a new... a great option.

I'd take the $ saved from new VESC and get a lower kv motor, or go to 6s batteries like @psychotiller suggested.
```

---
