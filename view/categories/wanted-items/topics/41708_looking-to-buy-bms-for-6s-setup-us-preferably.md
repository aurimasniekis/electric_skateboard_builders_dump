# Looking to buy bms for 6s setup (US preferably)

### Replies: 15 Views: 625

## \#1 Posted by: DevinG Posted at: 2017-12-22T15:22:47.590Z Reads: 66

```
Does any one stateside have a BMS i could buy that would be compatible with my two 3s 5000mah (6s) battery setup? Ive been reading a lot about them, I'm still not 100% sure I need one but would like to integrate one into my build sooner rather than later.
If anyone has one for sale or any advice in finding correct specs I would be grateful. feel free to PM me Thank you!
```

---
## \#2 Posted by: DEEIF Posted at: 2017-12-22T15:29:36.523Z Reads: 63

```
Uhhh are u going lipo?
```

---
## \#3 Posted by: DevinG Posted at: 2017-12-22T15:31:05.163Z Reads: 60

```
Yes atm I have 2 turnigy 3s 5000mah lipos
```

---
## \#4 Posted by: GrecoMan Posted at: 2017-12-22T15:35:14.001Z Reads: 62

```
we need more info...

cont. amps?
charging amps?
c rating?
charger?
space constraints?
discharge or bypass?
```

---
## \#5 Posted by: Namasaki Posted at: 2017-12-22T15:40:46.433Z Reads: 60

```
I run Lipos with a bms on my builds. 
They offer excellent power in a small lightweight package. 
As far as safety, I’ve never had a problem with them. 
You just need to protect them with an enclosure, not overcharge them or discharge them too low.

UPDATE:
Allow me to clarify.
I use and recommend Lipo's with a high C rating.  The higher, the better.
The Lipos I currently use are 5ah with 60/120C discharge and 5C charge.
Lipos with low capacity like 5ah and low C rating like 20/30C can have a tendency to heat up and bulge depending on the amount of load they are subject to.

Using Lipos with low capacity and low C rating can be risky.
```

---
## \#6 Posted by: DevinG Posted at: 2017-12-22T15:47:18.690Z Reads: 54

```
Im using a Turnigy E3 compact charger for 2s-3s lipos- for a first build I don't mind charging packs individually.
C rating for each pack is 20-30c
Space left in my enclosure is around 4x4x1.5 in inches so pretty narrow.
My esc is a quicrun 60A from hobby wing.
bypass would a require a anti-spark key right?

my goal is to have this be chargeable w/out taking batteries out ive seen builds on here that have charge ports on the enclosure. Am i mistaken in thinking that the bms is where this happens?
```

---
## \#7 Posted by: DevinG Posted at: 2017-12-22T15:49:16.526Z Reads: 52

```
Can you use a bms to add connection for charging batteries on board as opposed to taking packs out and charging them?
```

---
## \#8 Posted by: Namasaki Posted at: 2017-12-22T16:03:38.791Z Reads: 49

```
[quote="DevinG, post:7, topic:41708, full:true"]
Can you use a bms to add connection for charging batteries on board as opposed to taking packs out and charging them?
[/quote]

Yes, but if you use a bms to charge, you will need to buy a simple charger for 6s.
```

---
## \#9 Posted by: DevinG Posted at: 2017-12-22T18:26:32.455Z Reads: 40

```
that's interesting to me an kind of unfortunate because when I first started buying parts for my build I saw many that used the 20-30c 5000mah so I invested in a pair to start out. I that is indeed the case I may have to stop and reconsider weight an ride height, or even get a new deck altogether... My first impression about all this was terribly wrong in thinking it was fairly straight forward.
```

---
## \#10 Posted by: harveld9 Posted at: 2017-12-24T02:58:56.522Z Reads: 38

```
If don't use bms then?
```

---
## \#11 Posted by: Namasaki Posted at: 2017-12-24T03:32:52.774Z Reads: 37

```
[quote="harveld9, post:10, topic:41708, full:true"]
If don't use bms then?
[/quote]


For a 6s setup, you can just use a hobby balance charger.
They work better than a bms and brick charger anyway.

Just be careful to not discharge the packs too low.
Monitor with a voltage meter mounted through the deck or with battery alarms.
Or set the Vesc to back off at a conservative low voltage.
```

---
## \#12 Posted by: DevinG Posted at: 2017-12-25T15:00:10.186Z Reads: 34

```
https://www.amazon.com/dp/B01HEMGI6Q/_encoding=UTF8?coliid=I2DEEN1YXXGA0X&colid=2UGM4M2HJCPLG&psc=0

@Namasaki do you think that this should suffice for my 6s setup?
```

---
## \#13 Posted by: bartroosen12 Posted at: 2017-12-25T15:09:56.544Z Reads: 36

```
That bms should be fine if you only use it for charging.
I always use a bms for my lipo's and it works great.
For lipo's just make sure you got lipo's above 20C.
I got a 6S2P (with 5Ah 20C cells) so a 6S 40C pack.
```

---
## \#14 Posted by: Namasaki Posted at: 2017-12-25T16:10:11.768Z Reads: 33

```
[quote="DevinG, post:12, topic:41708"]
@Namasaki do you think that this should suffice for my 6s setup?
[/quote]

The balance current on that bms is only 42ma which is very slow.
 I honestly feel that you would be much better off using a hobby charger which will balance charge better and faster.
You can setup external ports for a hobby charger so that you won't have to remove the batteries to charge them.

The reason I used a bms on my system is because it's 10s and for protection during discharge.
I really see no point in using a bypassed bms on a 6s system.
```

---
## \#15 Posted by: DevinG Posted at: 2017-12-25T17:08:25.893Z Reads: 29

```
Links! Direct me to the links! what do you use? where do you get them?! :laughing:
```

---
