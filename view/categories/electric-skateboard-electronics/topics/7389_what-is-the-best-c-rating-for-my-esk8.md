# What is the best c rating for my esk8

### Replies: 10 Views: 2402

## \#1 Posted by: gmcgaffey Posted at: 2016-08-09T20:31:07.126Z Reads: 201

```
when I was building my board the batteries sat around for a long time and 2 of 5 cells are dead I have tried to bring them back but nothing works. I am looking for new batteries and I found these. is the c rating on these good or should it be higher.<img src="/uploads/db1493/original/2X/2/2e10d79015e37ade3b52d2e0276bcbae58beeea1.png" width="281" height="500"><img src="/uploads/db1493/original/2X/8/8ed424ac06f2cca5d02abda9570253ec359174a6.png" width="281" height="500">
```

---
## \#2 Posted by: lox897 Posted at: 2016-08-09T20:42:03.304Z Reads: 192

```
Should be higher. You need roughly 120+ continuous on lipos because they are often over stated.
```

---
## \#3 Posted by: gmcgaffey Posted at: 2016-08-09T20:47:47.906Z Reads: 187

```
right now I'm running 2 5s 5000mah 25c packs but I'm looking for 6s should I 2 of these.<img src="/uploads/db1493/original/2X/0/041e1c5c505912e9fbe0d6fd611e97194ab5c9f0.png" width="281" height="500">
```

---
## \#4 Posted by: lox897 Posted at: 2016-08-09T22:03:08.534Z Reads: 167

```
That's better. Here is the calculation: 5ah x 20c = 100 amp continuous. Which should be alright. Try and get 25c if you can.
```

---
## \#5 Posted by: maxz Posted at: 2016-08-09T23:16:55.465Z Reads: 162

```
Ive always wondered... is there to much c?? or is it what your esc/vesc can handle??
```

---
## \#6 Posted by: paragon Posted at: 2016-08-10T00:54:27.596Z Reads: 157

```
The more the merrier (generally higher "c" batteries are heavier and more expensive though).
Put really basically, c rating tells you the continuous amp discharge that a battery can provide;
having a c rating that is too low will make a lipo sag, heat up, and/or puff.
The "c" just means capacity, so 10c means that your max continuous discharge rate is 10 times the pack's capacity. For example, a 10c 5000mah (5ah) pack, would have a continuous discharge rate of 50 amps (50000mah)*.

*Keep in mind that lipo manufacturers (very) often overstate their c ratings.
```

---
## \#7 Posted by: pcbacon Posted at: 2016-08-10T01:07:55.245Z Reads: 140

```
yes I bought two of those batteries but I am running them in parallel so its fine if you are only going to run one then no don't get those or if your running two in series then no don't get them
```

---
## \#8 Posted by: gmcgaffey Posted at: 2016-08-10T01:13:51.306Z Reads: 133

```
ok thank you
```

---
## \#9 Posted by: maxz Posted at: 2016-08-10T01:40:59.042Z Reads: 126

```
but say if you have an 120 amp esc and you are putting 150 amps through it (5ah 30c), would the esc heat up or blow??
```

---
## \#10 Posted by: paragon Posted at: 2016-08-10T01:48:06.534Z Reads: 124

```
The 150a is the max your battery can handle continuously. You are almost never pulling that amount on an esk8. You'd likely have 150a momentary spikes, but only pull something like 20a continuous (all depending on your setup), so having a battery that can handle 150a shouldn't heat up (the battery) much, if noticeably at all.

120a esc with a 5ah 30c battery would work well for most setups (your amp draw depends on what your motor demands from your esc, and how much of that your battery can supply)

rule of thumb: more amps = more heat
```

---
