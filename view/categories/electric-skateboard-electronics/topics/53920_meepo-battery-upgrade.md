# Meepo battery upgrade

### Replies: 13 Views: 1668

## \#1 Posted by: Sebike Posted at: 2018-04-30T13:13:54.923Z Reads: 173

```
So, I'm going to build a new battery for my brothers meepo, probably a 3p of 30Qs. 

Do you guys know what bms they use in the stock batteries or where to source one, if you don't want to re-use the old one? 

Maybe someone even knows the discharge rating? 😉 Thanks
```

---
## \#2 Posted by: gstpierre Posted at: 2018-04-30T13:23:38.521Z Reads: 169

```
What I did was just buy a generic 10s bms and charge through it, but wire the circuit to discharge around it. Let me know if you want me to draw it out for you, but I think you'll be able to see what I mean if you look at it. There are plenty of cheap bms' on ebay, and since you're discharging around it, the discharge rating isn't a huge deal.
```

---
## \#3 Posted by: accrobrandon Posted at: 2018-04-30T13:44:20.116Z Reads: 162

```
its just a basic bms... i killed my meepo bms from riding in all weather... eventually corrosion got to it...but the cells were fine...  
3p your gonna need a new case anyways so what ever bms should work... if u were going 2p and trying to put it back in the same case then id say get a small rectangle one like meepo had.

or...reuse the bms and extend the wires if/where needed.
```

---
## \#4 Posted by: Fatos Posted at: 2018-04-30T13:49:16.478Z Reads: 154

```
I would go for 10s2p with 30q. You would get 33% extra range. And you would get rid of voltage sag. While using the same enclosure, and not increasing the weight.
```

---
## \#5 Posted by: sk8l8r Posted at: 2018-04-30T14:01:30.860Z Reads: 146

```
I would go for a 10s5p from diyeboard and use a printed meepo size enc. so you can use the same mounting holes

http://www.diyeboard.com/10s5p-18650-lithium-battery-pack-36v-10ah-360wh-p-460.html

 
https://esk8mods.com/10s5p-3d-printable-battery-case-meepo-board/
```

---
## \#6 Posted by: Toleg Posted at: 2018-04-30T14:04:17.033Z Reads: 142

```
@okp did a battery upgrade on a meepo: http://www.e-sk8.fr/forum/viewtopic.php?f=21&t=3163
```

---
## \#7 Posted by: Sebike Posted at: 2018-04-30T16:41:44.024Z Reads: 130

```
Thanks guys! 

Yes, the okp one is what I was going for
```

---
## \#8 Posted by: Sebike Posted at: 2018-04-30T20:21:50.353Z Reads: 123

```
Btw, is the stock bms hooked up for both charge and discharge?
```

---
## \#9 Posted by: accrobrandon Posted at: 2018-04-30T20:26:50.195Z Reads: 119

```
i dont remember but there was an extra jst soldered on that went to the charge port...and xt60 to the esc
```

---
## \#10 Posted by: JUSTIN5623 Posted at: 2018-08-20T10:03:03.981Z Reads: 78

```
So what do you mean when you say "wire the circuit to discharge around it"
```

---
## \#11 Posted by: bartroosen12 Posted at: 2018-08-20T13:03:49.517Z Reads: 73

```
I think he means if you buy a cheap bms, just use it for charging and bypass it for discharging.
```

---
## \#12 Posted by: JUSTIN5623 Posted at: 2018-08-25T20:21:27.488Z Reads: 60

```
How do you bypass it for charging? Can someone show me?
```

---
## \#13 Posted by: bartroosen12 Posted at: 2018-08-25T20:37:55.934Z Reads: 57

```
Bypassing for only charging means that you use the + and - of your battery and they go straight to your ESC, so you use direct power from your battery. So no current is going through the bms, so you won't be able to break your bms by pulling to much current.

If you connect your bms for discharge, you will pull power through your bms which is connected to your battery. The thing is with a cheap ass bms, they can't handle the high current and will break.
```

---
