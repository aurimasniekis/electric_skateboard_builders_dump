# 6S dual drive or 9S single drive?

### Replies: 23 Views: 3642

## \#1 Posted by: NNGG Posted at: 2015-11-07T08:42:50.785Z Reads: 189

```
So I bought a hobbyking outrunner thats like 168kv and am wondering if I should just buy a vesc and go for higher voltage on a single drive motor or buy two outrunners and two cheap 120amp escs each with 6S going in. 

I weigh like 160 pounds and will be going up light hills but mostly down hill. How will the two outrunners perform together at 6S each versus one motor at 9S with a vesc. 
What gearing should I have for each set up? 
Thanks for any ideas.
```

---
## \#2 Posted by: jacobbloy Posted at: 2015-11-07T10:05:52.771Z Reads: 188

```
Hey mate, higher voltage is always better! What is the motor you brought? As the power of a twin can some times not be any higher then a single as you only use what you need! 
It all comes down to how efficient your setup is

So twin 6s your motors will be slower or have higher kv but in both instances your motors arnt spinning at optimal rpm unless you hear down a lot with the twin the load is shared so less amps per motor but this could still be more more then a single drive on higher volts, with a 168kv motor at 10s you will get a good 35km/h to maybe 40km/h depending on your gearing but at that voltage will draw less amps so less heat!

the vesc from personal opinion makes your motors run more efficient! So more torque with less amp draw better motor timing.

I say 10s single drive vesc and plan on the upgrade when it's not enough power!
```

---
## \#3 Posted by: NNGG Posted at: 2015-11-07T22:14:15.467Z Reads: 172

```
Thanks for your input! But I do not have any need to go faster than 30 kph and I just  don't want my motor to overheat so I would think that having two of them would be less strain than if I have just one. How will the single 168kv motor perform at 6S?
```

---
## \#4 Posted by: chaka Posted at: 2015-11-07T22:36:30.947Z Reads: 166

```
Your motors in a dual configuration with a 6s voltage will be under the same current load as a single motor running 12s, the trouble is you will have trouble getting anything over 20mph unless you go with really large wheels and reasonably tall gearing.

If you are on a budget I offer the VESC as a "bare bones" option, it comes without any heatshrink, capacitors, or power cables attached. I only recommend it to people who are confident in their soldering skills or have access to someone how is.
```

---
## \#5 Posted by: NNGG Posted at: 2015-11-07T22:42:27.704Z Reads: 162

```
So I dont really want speed just. I just want the motors and the esc to stay cool.
```

---
## \#6 Posted by: onloop Posted at: 2015-11-07T23:52:00.784Z Reads: 164

```
Read this

http://www.electric-skateboard.builders/t/beginners-guide-to-building-your-own-electric-skateboard-drivetrain/53
```

---
## \#7 Posted by: jacobbloy Posted at: 2015-11-08T02:50:19.197Z Reads: 157

```
Vesc draws watts at start up so you have a 10s battery it will convert volts in to amps so you could even same a little money on a lower c rating battery! 
30km/h is good and where I sit alot of the time!
I still say single motor vesc 10s battery or even 8s

1:3 gear ratio is good, could go lower but then less torque more amps in turn to do the same job,
At 10s with a 168kv motor 1:3 ratio your looking at 30km/h with a nominal voltage of 3.7v 80mm kegel's

It sounds perfect for you!
```

---
## \#8 Posted by: NNGG Posted at: 2015-11-09T05:48:34.578Z Reads: 142

```
So what will be the negatives of using a DD set up with low kv and only 6S going into each motor?
```

---
## \#9 Posted by: cmatson Posted at: 2015-11-09T11:43:22.414Z Reads: 142

```
low top speed is the big one.. and it isn't as simple as just gearing them up to go faster-

it is kinda like a car transmission: it is always better to have high RPM's that get geared down, than to have low RPM's that get geared up. Sports cars don't cruise around in 7th gear driving 20kmh down the road at only 200rpm.. it'd probably blow up their engine. But, they could drive 20kmh in first gear with 1250rmp just fine. 

with 6s and 168kv, you are looking at low RPM- if you changed to 10s (like others have recommended) your motor would run cooler, faster, and be more powerful- not to mention you could go faster than like 15kmh. Higher voltage is always a win!
```

---
## \#10 Posted by: longhairedboy Posted at: 2015-11-09T20:27:46.279Z Reads: 136

```
i think everyone here has answered the question pretty well, but i'd like to also mention that you might want to go with a higher KV on a 6S. I've gotten as much as 30mph out of a 6S but i was running 270 kv motors at the time on a 14/36 pulley ratio. 

and yes, higher KV motors on a 6S will not be as efficient as a lower KV on a 10S or 12S. Things tend to run warmer and you don't quite get the range you would on higher voltage systems. But don't for a minute think they're slow. They're just less efficient. They're also cheaper to build around and the parts are more readily available. Everything has a trade off. 

but it sounds like based on what you want, a single drive 9S with a vesc would be better of the two choices.
```

---
## \#11 Posted by: psychotiller Posted at: 2015-11-09T21:39:19.041Z Reads: 139

```
To chime in here also,  the 290kv g160 motor rocks at 6s! Also had plenty of torque to climb and bust the 30mph Mark with ease on a single motor setup
```

---
## \#12 Posted by: cmatson Posted at: 2015-11-09T21:55:16.016Z Reads: 136

```
230-290kv would be nice for a 6s board, but he's got a 168kv- that's the dilemma.... I think higher voltage is the answer!
```

---
## \#13 Posted by: claudiofiore88 Posted at: 2015-11-09T21:58:16.411Z Reads: 131

```
I had more of setup in the middle. A single motor 8s lipo with an sk3 213kv outrunner. I got it to 25 mph. Keep in mind I weigh 265 lbs+, but sadly I fried it after slamming on the brakes going 25 mph.
```

---
## \#14 Posted by: NNGG Posted at: 2015-11-10T04:20:01.740Z Reads: 131

```
Ok, so I am looking at my options and I see either just get new motors and do a cheaper 6s DD boardwith higher kv motors, like a g160.
Or I can spend some coin and and go balls out with a 168KV 9S DD  drive setup. 
Lastly I could only go for a 9-12S vesc 168KV single motor drive set up. 
Which of these seems to be the most practical choice for me considering I have one 168KV motor and two 3S lipo batterie right now?
```

---
## \#15 Posted by: cmatson Posted at: 2015-11-10T11:44:43.289Z Reads: 123

```
a new motor and simple 6s setup would be the cheapest, but the higher voltage would be more powerful. 

If you don't have that many hills, and and don't need all the extra power(a lot of people don't...) then I'd just get new motors and go with a 6s setup.
```

---
## \#16 Posted by: longhairedboy Posted at: 2015-11-10T17:22:50.845Z Reads: 119

```
if you're basing it all around 3S packs, just do 9S with that single drive for now and if you want more power later you can drop in another 3S pack. 

unless there are decent sized hills, I think a single drive would be fine for you. Especially at those higher voltages.
```

---
## \#17 Posted by: lenineds Posted at: 2017-11-16T23:02:12.152Z Reads: 49

```
Hi there! I would like to know if you can help me. I'm building a e-board and I bought the parts with less information than I needed. My setup is very similar to yours. Torqueboard 4.12, G160 motor 290kv, 5000mah 6s (2 x 3s in series), 16/48 pulleys, 83mm wheels. My question is, will the vesc handle this in hills? Looks like it's for just 50A, and 6s can probably use more than that. It would be better put another 3s battery in serie or is it too much for a 290kv motor?
```

---
## \#18 Posted by: lenineds Posted at: 2017-11-16T23:07:22.399Z Reads: 52

```
I just posted this question up. I think you can help me. This setup you used had a vesc or car esc? I'm afraid the 50A vesc is not enough.
```

---
## \#19 Posted by: psychotiller Posted at: 2017-11-16T23:10:55.259Z Reads: 50

```
People have done it. But 290kv @ 6s is asking for trouble amps wise. All you need to do is get up to 8 or 9s and it'll work in bldc
Or buy one of those cheap dual escs on ebay.
```

---
## \#20 Posted by: lenineds Posted at: 2017-11-17T00:00:02.106Z Reads: 44

```
Thanks for replying. Do you think 9s is to much for 290kv on 16/48 gears? Do you think It would use the same amount of amps?
```

---
## \#21 Posted by: psychotiller Posted at: 2017-11-17T00:03:37.195Z Reads: 43

```
I've run 290kv on 8s.
```

---
## \#22 Posted by: lenineds Posted at: 2017-11-17T00:07:49.049Z Reads: 41

```
Vesc? Do you have idea of how much amps is using? What gears and wheels size?
```

---
## \#23 Posted by: psychotiller Posted at: 2017-11-17T00:23:03.422Z Reads: 38

```
Enough to burn it out if you set it up wrong.
```

---
