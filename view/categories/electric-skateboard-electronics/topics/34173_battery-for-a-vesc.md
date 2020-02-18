# Battery for a VESC

### Replies: 6 Views: 640

## \#1 Posted by: Greenie Posted at: 2017-09-28T13:27:45.364Z Reads: 93

```
I tried looking up info but haven't really gotten the answer I looked for.
My knowledge about batteries is not the greatest. My uncle helps me a bit with my first build, he claims that VESCs will require a very strong battery to work because they draw a lot of current. It sounded weird to me, I understand that I can use whatever battery and the VESC just controls everything. It doesn't really have demands, does it? I'd appreciate some clarification.
```

---
## \#2 Posted by: DeathCookies Posted at: 2017-09-28T13:39:45.172Z Reads: 92

```
The VESC can only perform in a certain range (6V - 60V?). In this range the VESC itself will manage how much current and voltage goes through to the Motor (VESC BLDC-Setup). It will only get what the battery can deliver.

Your application (single/dual Motor + weight + desired topspeed + desired range) tells you how much Juice your battery will Need.
If your battery is too weak you will harm your battery or wont drive as fast / Long as you want.
So better overbuild the battery to get what you want.
```

---
## \#3 Posted by: Greenie Posted at: 2017-09-30T10:39:08.143Z Reads: 60

```
Thanks for the reply mate. That's what I thought. The VESC manages the current and get what the battery can deliver. My uncle sort of thinks the VESC got this requirement, as if feeding it a weak battery won't even power it up. By weak I do not mean some toy battery. Range is most important to me, any tips for that?
```

---
## \#4 Posted by: DeathCookies Posted at: 2017-10-04T07:41:38.112Z Reads: 44

```
Many batteries in parallel for increased range
```

---
## \#5 Posted by: GrecoMan Posted at: 2017-10-04T11:26:09.547Z Reads: 39

```
[quote="DeathCookies, post:2, topic:34173"]
6V - 60V?
[/quote]

While the vesc will power on at 6v, it won’t have enough power to move anyone over 75 pounds and climb decent sized hills until about 24v (6s). For range, get maybe 6 3s 5000mah batteries, make each into a 6s pack.  You will be able to get over 20 miles if you use all 3 in one ride
```

---
## \#6 Posted by: Greenie Posted at: 2017-10-18T13:48:02.070Z Reads: 27

```
What if I wanna make the 18650 configuration? Any recommendations for that type of thing?
```

---
