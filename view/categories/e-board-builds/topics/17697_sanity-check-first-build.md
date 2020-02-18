# *SANITY CHECK* First build

### Replies: 8 Views: 866

## \#1 Posted by: faithfulpuppy Posted at: 2017-02-14T18:14:49.652Z Reads: 133

```
just want to make sure my board won't catch fire under my feet.  Ive already ordered my battery (some price-glitched floureon lipos that i got (12 4s 5000mah batteries, not gonna use them all obviously but i want to do a 12s config)), BMS (60a 12s), power supply, ESC (vesc), wheels (83mm flywheel clones), trucks (sidewinders because fuck the status quo), and motor mount/pulleys/belt (generic kit from ebay that i'm gonna modify)

i was planning on running a 190kv sensored 6374 motor but apparently that's waaaayyyy too much for my build. this would be fine if i limited the rpms in the VESC settings though, right?

the other two components i havent ordered yet are the remote (either a nyko kama with wiiceiver or a modded GT2B)  and the deck (i was thinking a generic ebay deck)

I'm not sure im doing everything right. what am i doing wrong.
```

---
## \#2 Posted by: ewalks6 Posted at: 2017-02-14T18:26:44.527Z Reads: 133

```
as long as you modify the mount to fit your trucks you will be good I believe. What pulley configuration are you doing?
```

---
## \#3 Posted by: faithfulpuppy Posted at: 2017-02-14T19:11:06.659Z Reads: 115

```
my pulley config is 36t wheel 12t mototr
```

---
## \#4 Posted by: NickTheDude Posted at: 2017-02-14T19:51:20.478Z Reads: 95

```
12S and 190kV shouldn't go above the 60k ERPM limit, even fully charged so you should be fine there. Most people go lower to leave some headroom.
```

---
## \#5 Posted by: Iceni Posted at: 2017-02-14T20:02:25.750Z Reads: 88

```
Nyko kama is really hit or miss when it comes to reliability, usually miss from what I've seen here and tested myself.
So I'd really suggest going for the gt2b.

And with a 12t motor pulley you should think of using an idler pulley to get more teeth in gear.
Otherwise you run the risk of the belt skipping a lot.
```

---
## \#6 Posted by: ewalks6 Posted at: 2017-02-14T20:43:15.413Z Reads: 78

```
I suggest you use a skateboard bearing to lower the belt. This is because the teeth in mesh (the amount of teeth from the belt in motor pulley I believe) will be under 6, the recommended amount. I can't quite explain it but people have done it.

 [quote="lowGuido, post:30, topic:406"]
well I just finished my belt tension idler pulley.Its pretty simple, just like you described @psychotiller. I drilled a 8mm hole and put a bolt with a bearing on it.My theory is that it will force more teeth in mesh on the small pulley.the traditional method of tension by moving the  2 pulleys apart doesn't give optimal amount of teeth in mesh on the small pulley. sure making the pulley bigger will give you more teeth in mesh, but then you lose your gear reduction, and acceleration/torque/hill climbing etc..
[/quote]

He talks about it here.
```

---
## \#7 Posted by: ewalks6 Posted at: 2017-02-14T20:44:08.858Z Reads: 70

```
and @Iceni talked about it as well above
```

---
## \#8 Posted by: faithfulpuppy Posted at: 2017-02-15T00:29:04.887Z Reads: 55

```
good call on the belt tensioning.  should be an easy modification.  Thanks for the pointer man.
```

---
