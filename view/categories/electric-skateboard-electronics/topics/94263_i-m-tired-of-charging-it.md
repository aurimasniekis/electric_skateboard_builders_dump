# I’m tired of charging it

### Replies: 13 Views: 488

## \#1 Posted by: Ginga Posted at: 2019-05-18T19:25:33.865Z Reads: 266

```

So, I have two batteries connected in parallel obviously. They are both 3s, 11.1 v, and 5,000mah. Now, each time I charge them it’s really annoying. I have to unplug the whole set up and check the voltage. Then plug it into a balance charger. I know there’s a faster way to charge them without taking it a part. It’s with a balance circuit or something. The question I pose is; is how would I attach it on. How it works and if you guys could link me some balance circuits or something.
```

---
## \#2 Posted by: J_Dizzle Posted at: 2019-05-18T19:31:37.521Z Reads: 258

```
[quote="Ginga, post:1, topic:94263"]
So, I have two batteries connected in parallel obviously. They are both 3s, 11.1 v, and 5,000mah.
[/quote]
I think you mean series? So you have a 6s lipo configuration.

Search up “6s bms” and see what you can find, there are lots of helpful topics on using bms with lipos. But to answer your question yes you need a bms for easy one plug charging
```

---
## \#3 Posted by: Hummie Posted at: 2019-05-18T19:35:58.805Z Reads: 236

```
Search Lipo discharge balancer and twenty four volt power supply.   U can charge and balance at rocket speed cheaply with two plugs.  One connection to the main leads and the lipo balancer on the balance plug.   Ur lipo should have a max charge rate similar to a c rating and charge within that and maybe just charge to four point one instead of four point two to be safe and batteries will last much longer.                                   Unless you’re charging slowly there will also be a settling of the voltage and off the power supply the voltage of the battery will drop by like point one within minutes.
```

---
## \#4 Posted by: b264 Posted at: 2019-05-18T19:41:00.467Z Reads: 197

```
@Hummie that still involves taking the enclosure apart or leaving balance wires sticking out, which means cannot be made water resistant

As @J_Dizzle said, the best solution involves using a BMS

And you need to figure out if they are in series or parallel.
```

---
## \#5 Posted by: Hummie Posted at: 2019-05-18T19:44:47.878Z Reads: 171

```
Yea.  But if u have a charge port and a single balance plug coming out of the enclosure they can be protected from water.    Everyone has a charge port probably anyway and it’s not much trouble to have a balance plug come out.   I’ve seen waterproof protection for charge ports but not balance plug covers.  Both of which are dooming with even half a drip contact possibly making a short.
```

---
## \#6 Posted by: b264 Posted at: 2019-05-18T19:46:39.758Z Reads: 152

```
[quote="Hummie, post:5, topic:94263"]
I’ve seen waterproof protection for charge ports but not balance plug covers.
[/quote]

I second this.
```

---
## \#7 Posted by: Hummie Posted at: 2019-05-18T19:49:23.583Z Reads: 137

```
I won’t say a cheap bms put in by a diy guy who doesn’t know much electronics is a safer bet.  It adds a lot of ways to possibly fail as apposed to kiss.   With waterproofing of both points and a real human eye on the cell voltages while charging I feel safer without the bms.   The bms has other safety features which people maybe want too
```

---
## \#8 Posted by: Wilsonliang777 Posted at: 2019-05-18T22:22:14.408Z Reads: 115

```
I used to have 2x 3s lipo  that I connected into 6s battery.   I hot glued the balance cable and xt90 plug flush to the  enclosure and used a stronge tape to seal it from water and dirt.     All I have to do when I want to charge the battery I take off the tape,  connect the xt90 plug and balance plug to the lipo charger.  No bms needed and I am sure my 6s lipo is balanced each time.
```

---
## \#9 Posted by: iamasalmon Posted at: 2019-05-18T22:35:01.469Z Reads: 114

```
voila

Waterproof balance charge port, 2x 5s charge. No onboard bms=more room for batteries. Was going to unveil in a build thread, but my ears were burning. @Hummie 
![IMG_2007|375x500](upload://3QL06cCMl40F2uziY3r3fM6ttL8.jpeg)
```

---
## \#10 Posted by: Hummie Posted at: 2019-05-18T23:38:55.645Z Reads: 100

```
looking forward to seeing it opened up and what materials you used.  much nicer than a balance plug or two hanging off the side.
```

---
## \#11 Posted by: Ginga Posted at: 2019-05-20T06:50:26.618Z Reads: 58

```
Yea, it’s series. My bad it has been a while.
```

---
## \#12 Posted by: Ginga Posted at: 2019-05-20T06:55:30.188Z Reads: 60

```
[quote="Hummie, post:3, topic:94263"]
point
[/quote]

Probably should have mention this, but I already have a Lipo discharge balancer.
```

---
## \#13 Posted by: bartroosen12 Posted at: 2019-05-20T07:41:33.415Z Reads: 54

```
Buy this:
Bms 6S Lithium
https://s.click.aliexpress.com/e/b3TMsip2

Connect it like the schema on the picture.

Use it for charging only so you have to bypass the bms (use the + and - directly from your battery)

You will also need a 25.2V charger:
https://s.click.aliexpress.com/e/bpsXfLDe
```

---
