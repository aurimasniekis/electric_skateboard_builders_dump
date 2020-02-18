# Clearly this isnt written correctly&hellip;. right?

### Replies: 9 Views: 366

## \#1 Posted by: Sn4pz Posted at: 2018-08-30T18:51:27.720Z Reads: 191

```
https://flipsky.net/collections/accessories/products/antispark-switch-pro-280a

280a?? :confused: :crazy_face:
```

---
## \#2 Posted by: Winfly Posted at: 2018-08-30T19:03:35.166Z Reads: 181

```
@BarbaraZ is it possible to see a test to show that it can actually handle 280A continuous and 800A burst?
```

---
## \#3 Posted by: Kug3lis Posted at: 2018-08-30T19:26:21.368Z Reads: 165

```
Haha those wires would melt first before even 200A :D
```

---
## \#4 Posted by: Sn4pz Posted at: 2018-08-30T23:34:20.966Z Reads: 124

```
thats what im saying
```

---
## \#5 Posted by: yelnats8j Posted at: 2018-08-31T02:06:19.977Z Reads: 99

```
280 A What The HELLLLL I call BS
```

---
## \#6 Posted by: TowerCrisis Posted at: 2018-08-31T02:19:07.950Z Reads: 97

```
It's probably the spec of some component or fet on the board. Definitely does not have the heat dissipation or actual current carrying capacity in the design.

EDIT: it DOES appear to have a heatsink on it.. but then it's wrapped in shrink tubing 😂 I'm really not sure what to think of this
```

---
## \#7 Posted by: TowerCrisis Posted at: 2018-08-31T02:59:05.868Z Reads: 89

```
Alright, I did some digging on these mosfets they're using.

First of all, their heatsink does nothing. These mosfets have large pads on their underside and are made to heatsink into the PCB. Adding a heatsink above the plastic casing will not help cooling in any meaningful way.

They're rated to dissipate 3.7 watts when only ambient air cools them, and 110 when properly heatsinked.

So ambiently cooled they can carry28A continuously each. So 224 total 🤔(still not 280) we're using this metric because the heatsink does nil and the shrinkwrap will end up trapping more hot air.

BUT AHA FINE PRINT! The 28A spec is for when a single fet has a 2.55cm by 2.55 cm copper pad on the PCB. That's VERY big compared to the actual size of the fet. The fet is 0.6cm in it's longest dimension.

SO in order to get actual CC of 224 (they advertise 280, which is ludicrous) all the fees would NEED to be ~2cm apart from each other to properly dissipate heat. Based on the pictures, they look to be... Well, close to 0.01 cm apart. Totally implausible for ambient cooling.

TLDR: The heatsink does very very little to cool this, the fets aren't even rated to what they say, and to even come close to their CC of 280A the fets would need to be 2cm apart from eachother, bringing the total board size to ~ 10x7 CENTIMETERS. 70cm^2 needed. The PCB is 12cm^2. It is **almost six times too small overall.**

Total load of bull. Completely false advertising. #Debunked
```

---
## \#8 Posted by: TowerCrisis Posted at: 2018-08-31T03:18:13.797Z Reads: 73

```
![Screenshot_20180830-230654|413x500](upload://f4eyrJdmodIab44eKeBfn8I1REX.png)

![Screenshot_20180830-230953|414x500](upload://sxpLszOykJCqcYSa6yx2WAvKfhW.png)

![Screenshot_20180830-231248|416x500](upload://yECB6a2x6SnLIwKhtSb5qg2qgkI.png)



As polite as their rep was, I don't buy it 🤷‍♂️ but I guess we'll see.
```

---
## \#9 Posted by: b264 Posted at: 2018-08-31T04:00:06.582Z Reads: 57

```
[quote="TowerCrisis, post:6, topic:66574"]
it DOES appear to have a heatsink on it… but then it’s wrapped in shrink tubing :joy: I’m really not sure what to think of this
[/quote]

They just want to make sure it is completely shrunk at all times
```

---
