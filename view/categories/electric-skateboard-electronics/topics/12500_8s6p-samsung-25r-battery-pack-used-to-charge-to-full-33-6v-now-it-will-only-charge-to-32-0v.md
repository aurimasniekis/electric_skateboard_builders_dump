# 8S6P Samsung 25R Battery Pack Used to Charge to Full 33.6V, Now it Will Only Charge to ~32.0V

### Replies: 15 Views: 1107

## \#1 Posted by: JuniorPotato93 Posted at: 2016-11-04T21:59:47.288Z Reads: 123

```
As the title says,  the battery pack I made used to charge to 33.6 +/-. 05 per cell via a onboard BMS.  Then I charged it it went up to 33.0 when I turned it on but didn't think too much of it,  I had left it for a day before riding it again.  I noticed it was lower than I expected and when I charged it last weekend which it charged up to 32.8 which caught my attention and not today I charged it again,  it only made it to 32 this time.  I've never taken the pack lower than  27.5 volts if thats useful information. 

I'm not certain where to start looking as to what's going on,  is this a BMS or cell issue?  The BMS I have is from battery support 8S lipo,  80amp continuous,  20 amp charging.  I'm at a student house so I don't have a multimeter or my tools to look into what's going on so I'm looking for a place to start once I go home for a weekend.
```

---
## \#2 Posted by: Pantologist Posted at: 2016-11-04T22:06:21.487Z Reads: 122

```
I would not try charging it again. Either one cell is disconnected or dead or you have an issue with your BMS...

I had a similar issue, and then it turns out there was a short between two balance connectors and I had been overcharging my batteries while one cell was dead.
```

---
## \#3 Posted by: chinzw Posted at: 2016-11-04T22:15:45.286Z Reads: 115

```
That's why you need to know the status of each cell all the time :slight_smile:
```

---
## \#4 Posted by: JuniorPotato93 Posted at: 2016-11-04T22:21:26.374Z Reads: 104

```
So I'll have to do an autopsy of the battery/BMS set up then.  How do I check each individual cell if they are now joined in packs of 6? if there a trick to that? As far as i can tell, it will have the same potential across all 6 cells in each pack, no?
```

---
## \#5 Posted by: Pantologist Posted at: 2016-11-04T22:28:39.538Z Reads: 100

```
That is why I am done with "dumb" BMSes. Moving on to expensive "smart" BMSes because batteries are effing expensive...
```

---
## \#6 Posted by: chinzw Posted at: 2016-11-04T22:30:44.681Z Reads: 95

```
If the cells are +-+-+-+-+-+- then just check the same way you check you balance leads.
So: (+-)(+-)(+-)(+-)(+-)(+-)
```

---
## \#7 Posted by: chinzw Posted at: 2016-11-04T22:32:59.257Z Reads: 90

```
Yeah, im waiting to see what happens to the two open source bms developments. For now battery supports bms + arduino monitor gives me enough data. If i run out of projects i might do an arduino bms (already saw it done) which should be pretty simple and flexible.
```

---
## \#8 Posted by: Pantologist Posted at: 2016-11-04T22:36:11.636Z Reads: 90

```
@raphaelchang's design is :fire:

I am waiting for his next version.
```

---
## \#9 Posted by: JuniorPotato93 Posted at: 2016-11-04T22:42:09.908Z Reads: 86

```
Yeah I get that but if i'm trying to narrow down which of the 48 cells is dead, checking the +/- of each pack of 6 will only really tell me which one pack(or more) of the 8 is damaged, then to fix it I guess either way I'd have to take the pack apart. to remove the dead ones. :/ I dont like this, I agree with @Pantologist, batteries are hella expensive. Someone in Canada go ahead and start making custom battery packs please.
```

---
## \#10 Posted by: chinzw Posted at: 2016-11-04T23:13:46.649Z Reads: 77

```
Well, depending on your configuration how you would go around testing it. If you have 6 bundles of 8 serials or 8 bundles of 6 parallels. But yes, you will first need to narrow it down to which bundle is screwed, then narrow it down to which cell in that bundle.

Also, might be good to check the charger, it might be faulty and not delivering the required voltage.
```

---
## \#11 Posted by: JuniorPotato93 Posted at: 2016-11-04T23:15:32.538Z Reads: 73

```
Thats a good point, I didnt think to check the charger. Still dont have a multimeter with me but I'll check that out as well when I go home.
```

---
## \#12 Posted by: Pantologist Posted at: 2016-11-05T00:03:41.325Z Reads: 71

```
The issue with eSk8 in general is that everyone wants more range. 

Big batteries need more advanced pack designs to make sure each cell is in good health. This gets really hard with large paralleled packs since most BMSes don't monitor individual cells in parallel. 

This is why I am pushing for modular packs. Boosted's battery is able to monitor each individual cell since the whole battery pack is only 12 cells in total. If a cell goes bad, it is very easy to diagnose the program instead of looking through lots of cells for an issue. 

Modular packs are great for when the battery has an issue and is also great for making boards lighter for when you don't really need the crazy range that some of our builds have.
```

---
## \#13 Posted by: chinzw Posted at: 2016-11-05T00:25:23.055Z Reads: 64

```
Yeah, i was thinking about this the other day because i was thinking of going 12S1P or 6S2P and tought about just adding another 6S pack with its own bms.
```

---
## \#14 Posted by: flatsp0t Posted at: 2016-11-05T23:16:46.541Z Reads: 51

```
[quote="Pantologist, post:12, topic:12500"]
Boosted's battery is able to monitor each individual cell since the whole battery pack is only 12 cells in total
[/quote]

And they still go on fire.

The Problem is, with none of the currently available Batteries it is possible to build a 1P pack capable of some serious power.
So the only thing that you can do for now is adding cell level fusing, like Ollinboards and Tesla does it.
```

---
## \#15 Posted by: Pantologist Posted at: 2016-11-06T01:37:22.646Z Reads: 48

```
They aren't catching on fire. The cells are undergoing thermal runaway. Pretty sure they would have been on fire without the fire retardant housing.

But yeah, you either use A123 or advanced pack assembly.
```

---
