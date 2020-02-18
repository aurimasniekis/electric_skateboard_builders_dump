# Wiring 6s BMS for 2x 6s LiPo&rsquo;s in parallel (sorry for making 2 topics)

### Replies: 5 Views: 1013

## \#1 Posted by: Orin635 Posted at: 2017-11-28T21:57:07.379Z Reads: 79

```
Hi,
I'm in quite a pickle here I have bought 2 6s LiPo's (wiring in parallel) and a 6s BMS (bypassing discharge) this was how I was originally going to wire (when I was going to buy 2x 3s)<img src="/uploads/db1493/original/3X/2/d/2de4c9ceeef2862c85f4d371df747ca4f9e0b5fa.PNG" width="690" height="345">

but now that I have got 2x 6s LiPos I do not know how I will wire everything  
Here is my pathetic excuse of making a diagram<img src="/uploads/db1493/original/3X/0/7/07f87ee6ad53b724faed330904a692cede7cf99f.PNG" width="690" height="345"> could someone help, thanks
```

---
## \#2 Posted by: krloz Posted at: 2017-11-28T22:32:07.559Z Reads: 74

```
I think you kind of have it right.  You are bypassing ok. And you are paralleling the thick wired and the balance wired of the batteries.  If your bms is for 6s and only had 5 pin for balance connector it means it doesn't carry the positive or negative on the balance.  So ignore the red and black from the balance wire on the batteries (they should be that colour.  One on each end) 
Pro tip when not sure about writing Lipo batteries and asking.... wait to have a bunch of people agreeing on an answer before you run to wire...
```

---
## \#3 Posted by: Orin635 Posted at: 2017-11-28T22:33:23.065Z Reads: 72

```
OK thank you very much :)
```

---
## \#4 Posted by: OBone Posted at: 2018-10-23T08:57:24.796Z Reads: 39

```
Noob question. Please clarify what you mean ignore? Does it go nowhere? 

To confirm the 6s BMS balances both packs, you simply splice the matching colors together?
```

---
## \#5 Posted by: krloz Posted at: 2018-11-08T17:32:44.107Z Reads: 34

```
In a 6s pack you havea thick ref for positive, a thick black for negative and 7 small wires for balancing.  Of those 7 wires one is connected to the thick red (and is usually also red) for the positive balance and another one is connected inside the battery to the thick black (usually also black) and thus this 2 are not always necessary if your bms already had positive and negative through the thick wires.  So in occasions bms have connection for Less  than  the expected 7 balancing wires. 
The other 5 balance wires are the between cell connections. 
You can paralell batteries by combining colours if the are same model because they should respect the colour coding but I wouldn't risk if.  Better measure voltage between negative black thick wire and each balance wire.  If should be something like. 0》3.8》7.6》11.4》15.2》19》22.8
```

---
