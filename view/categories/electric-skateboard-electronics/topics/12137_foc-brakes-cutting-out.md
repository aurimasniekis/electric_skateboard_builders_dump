# FOC brakes cutting out

### Replies: 5 Views: 764

## \#1 Posted by: Brando Posted at: 2016-10-30T02:40:30.579Z Reads: 121

```
I set up my vesc in FOC mode and I love how smooth and quiet it is, but the brakes are acting a little weird. If I start to pull back the throttle on my nano remote, it will slow down, but if I brake all the way the motor screeches a bit before cutting out and coasting. 
any idea how to fix this? It is a safety hazard and an annoyance
```

---
## \#2 Posted by: Mrmoonlight Posted at: 2016-10-30T03:19:55.065Z Reads: 115

```
Is your battery fully charged? If not, post your settings.
```

---
## \#3 Posted by: Brando Posted at: 2016-10-30T04:52:52.227Z Reads: 106

```
I'll post my settings tomorrow. Hopefully we can find something.
```

---
## \#4 Posted by: flatsp0t Posted at: 2016-10-30T21:23:50.035Z Reads: 72

```
i think @longhairedboy had the same problem on his boards, maybe he can tell you why and how he fixed it.
```

---
## \#5 Posted by: longhairedboy Posted at: 2016-10-31T19:21:23.467Z Reads: 52

```
i'm not running in FOC, still BLDC. I'm about to switch to sensored hybrid BLDC though as soon as some sensored motors arrive that i want to try out.  

I ended up bumping the absolute batt max up a little and for some reason that mitigated most of this effect for me, but it still happens on occasion on my test board. I think something else is going on in that board though. I'm about to have some wireless real time diagnostics happening on that board though so maybe i can figure it out some more.
```

---
