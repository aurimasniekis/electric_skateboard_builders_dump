# Mixing belt drives and hub motors

### Replies: 15 Views: 962

## \#1 Posted by: pigeonic Posted at: 2018-01-28T16:38:43.068Z Reads: 187

```
So, this random thought I had.

Would it be feasible to fit hub motors and belt drives in one board?

Belt drives have certain slip to it, so acceleration wont be instant (unless its dual diagonal drive, but i still think it slips slightly)

What if the hub acts as its initial pull to accelerate, and maybe during the rest of the ride, it lays off to the belt to let it handle speed etc, and the hub can do the regen to the battery. 

Does this even make sense?
```

---
## \#2 Posted by: ducktaperules Posted at: 2018-01-28T16:51:11.174Z Reads: 182

```
[quote="pigeonic, post:1, topic:44880"]
Does this even make sense?
[/quote]

. . . . no
```

---
## \#3 Posted by: krloz Posted at: 2018-01-28T17:10:26.139Z Reads: 174

```
That was harsh...

I'm not sure how this would work out. But I'm sure I've seen a 4wd here that had two hubs and two belt or chain, can't remember.  So it is possible. Search for it and I'm sure you will find it here. 
If you are proposing to use regen on the hubs while the belt motors are pushing that won't work for sure.  Your belt motors will have to use much more power while pushing than the hubs will be able to regenerate
```

---
## \#4 Posted by: lennylogs Posted at: 2018-01-28T17:12:54.937Z Reads: 167

```
Idk if it’s possible/practical or not, but if it is, I think it would make more sense to do it the other way around: belts initially for acceleration and the hubs for higher speeds
```

---
## \#5 Posted by: jdnicholson Posted at: 2018-01-29T02:53:54.387Z Reads: 120

```
You know when you're about to fall asleep and your mind comes up with some wacky and very impractical ideas. Well I had basically the same thought last night.

I have a terrible single hub drive spare in the workshop and was thinking if you could pair it with a belt drive. So on the rear you have one hub and one belt. The hub would provide the extra power on flats but the belt would do all the work on hills. If you ran a loose 9mm belt so you didn't get too much drag. 

I assume the extra weight and drag from the belt would make it useless. But an interesting idea.
```

---
## \#6 Posted by: b264 Posted at: 2018-01-29T02:55:12.136Z Reads: 115

```
[quote="pigeonic, post:1, topic:44880"]
Belt drives have certain slip to it, so acceleration wont be instant
[/quote]

citation needed

(citation from someone other than a cheap hub motor board seller)

Also, cars usually weigh less than 5kg until they hit 30km/hr then they are usually around 1500kg
```

---
## \#7 Posted by: Rayce Posted at: 2018-01-29T03:26:00.524Z Reads: 101

```
The 4wd concept sounds interesting 2 hubs upfront 2 belts in the rear. I wonder how that would play out. Or maybe hubs in the back for sliding.
```

---
## \#8 Posted by: lennylogs Posted at: 2018-01-29T03:29:38.214Z Reads: 99

```
Does this design mean 2 remotes?
```

---
## \#9 Posted by: pat.speed Posted at: 2018-01-29T03:30:38.002Z Reads: 100

```
This is an old concept and has been done many times. Carvon has a board like this single large motor on one end and dual hubs he other
```

---
## \#10 Posted by: ShutterShock Posted at: 2018-01-29T03:31:07.530Z Reads: 102

```
Honestly it is kind of a weird idea?  I don't think the hubs would stand any chance against the belt drive.  I think that the belt would overpower it every time.

The only things that have come close to the torque of the properly configured belt setups are the Raptor 2 massive hub motors, Carvon direct drives, and the new hummie drives that he is currently working on.  

Most of the China hubs (Landwheel, Meepo, Benchwheel, etc etc) are all hard to compare to.  For example, my landwheel L3-x, the new one, is like a Prius, and my DIY board with dual 6355 motors is like a Tesla. 

Also just another note, as far as I am concerned, a properly setup belt drive should have zero "slip", if you have belt slip, you gotta set up an idler or tighten it up a bit.
```

---
## \#11 Posted by: ShutterShock Posted at: 2018-01-29T03:32:18.424Z Reads: 96

```
Lol maybe the other way around (hubs in front), the hubs thane would get destroyed in the back xD

50 miles and my Landwheel is already chunking like crazy
```

---
## \#12 Posted by: pigeonic Posted at: 2018-01-29T13:28:13.281Z Reads: 70

```
This. This was EXACTLY what happened.
```

---
## \#13 Posted by: pigeonic Posted at: 2018-01-29T13:30:09.307Z Reads: 70

```
Totally forgot what my brain was going through. But it shouldn't be 2. (I know it doesn't make sense, stop telling me it doesn't make sense.) 

Like some cpu inside it to switch around from hub and belt in one remote. AGAIN, no sense whatsoever. 

ITS JUST A RIDICULOUS IMPRACTICAL IDEA CONCEIVED BEFORE SLEEPING. 

sheesh
```

---
## \#14 Posted by: laurnts Posted at: 2018-01-29T14:36:36.404Z Reads: 63

```
Heres the thing, its possible. One of the moderators here have tried it before with unbalanced dual drive. Technically how it works is the other way around of how you describe it. The belt drive have more initial torque due to reduction, so it will be the driving force from static stop. Hub drive is best played during high speed as the way BLDC motor works (requires movement in the magentic flux to determine which phase wire to be electrified). Therefore the hub will perform the pull well to the higher speed than the belt drive. As so this is the hypothesis.

In practice, this works too. Belt will give higher torque and smooth start while the hub will pull you up in speed. But what you're trying to achieve, the difference, is not significant. It will just be all in all smooth transitions.

If you have proper dual sensored hub or dual unsensored belt in what ever combinations, it works quite well and efficient. So to say, its doable but no significant impact (just more cost).

---

So how 2 different speed works? it comes back to the rules of electricity works with load. Basically each motor and each esc / vesc will share the load. Just like if you're on downhill road, you still roll but use less electricity. Same goes by with dual uneven motor or drive.

---

This should end your questions and thoughts :smiley:
```

---
## \#15 Posted by: pigeonic Posted at: 2018-01-30T05:47:58.792Z Reads: 37

```
Definitely did. Thanks!
```

---
