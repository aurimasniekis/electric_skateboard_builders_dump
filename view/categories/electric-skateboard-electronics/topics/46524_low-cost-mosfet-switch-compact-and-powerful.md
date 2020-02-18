# Low-cost Mosfet switch. Compact and powerful

### Replies: 11 Views: 789

## \#1 Posted by: getyorma Posted at: 2018-02-15T20:22:37.950Z Reads: 130

```
I recently realised, that instead of prefboard soldering i should make a nice looking compact PCB. The board with IRLS3034 (9s) can handle up to 120A (-edit >peak< ) and 80A continuous. 
There is also a 60v version (12s) that can do exactly the same, but the fets cost a tiny bit more.
![28125793_1998635826845526_1923225910_o|375x500](upload://lMgiKAF0G7xs93XPPZAND6xYLqX.jpg)

This is the testing of the first PCB-s. I quickly realized that the 2oz copper was not thick enough, so the next ones will have thick solder tracks all across the board.
Here is the "bench test" version with copper pads, i want to over-current test these and push them to their limits:
![28125819_1998636176845491_1663983617_o|375x500](upload://qATOFI7C7A3zRUsdZALmASo5LXu.jpg)

Also a smaller version(50A max):
![28081946_1998636610178781_7766900_o|666x500](upload://h1V3TNHDhRtzkr9QlU0o5miVe7s.jpg)
(edit - corrected picture)

What do you guys think? This could be done on a prefboard really well too! :smiley:
```

---
## \#2 Posted by: Jammeslu Posted at: 2018-02-15T20:27:18.676Z Reads: 112

```
Does it support a led switch?
```

---
## \#3 Posted by: Acido Posted at: 2018-02-15T20:28:11.947Z Reads: 114

```
People have done them much bigger and they failed hard on bigger batteries, these might work for some smaller ones

Its a cool project tho, good luck with them
```

---
## \#4 Posted by: getyorma Posted at: 2018-02-15T20:30:40.639Z Reads: 110

```
Yup - do note that these are not for sale, maybe in the future if there is enough interest. This is mainly done because i like to keep my boards looking clean :D I will probably redesign the whole thing before that happens.
```

---
## \#5 Posted by: getyorma Posted at: 2018-02-15T20:34:15.112Z Reads: 98

```
For my use - a 2WD mountainboard that pulls 50A peak per mosfet switch - it's perfect, maybe if i want to go full crasy on it, the switch shoulde be able to handle it fine. Only 4W of heat is produced in total across all mosfets together @120A - they might get warm if that is continious, but if it is cooled properly i do not see an issue :D I might even make a really compact 4 mosfet version of this that would be as good as a wire in terms of internal resistance.
```

---
## \#6 Posted by: SimosMCmuffin Posted at: 2018-02-15T20:43:39.048Z Reads: 88

```
[quote="getyorma, post:1, topic:46524"]
IRLS3034
[/quote]

IRLB3034, S-models are surface mount devices.

[quote="getyorma, post:5, topic:46524"]
Only 4W of heat is produced in total across all mosfets together @120A
[/quote]
I can't figure out how you got to those numbers. Care to share the math behind that?
```

---
## \#8 Posted by: getyorma Posted at: 2018-02-15T20:56:03.947Z Reads: 74

```
Sorry, i accidentally put in the wrong package name, will fix that. The Mosfets have an internal resistance typ 1.4mOhm, now 3 of these bad boys in parallel will give us 0.47 mOhms, that is  0.00047ohms. 
And i do apologize again, i kind of screwed up on the last part :lying_face: - the following was for the @80A when pushing the board to it's limits (Dual vesc pulls 60A on my board max). I will bench test the board this week and report back actual numbers of amperage and heat with proper graphs.
Silly me, cant even remember what i calculated it for and just put the numbers in.  - though i think it should handle 120A if the enclosure is cooled :3 - i have a build log coming up on that.
![image|690x343](upload://co6NM5x4A3t17EjU16eOCA8e8o7.png)
```

---
## \#9 Posted by: getyorma Posted at: 2018-02-15T21:01:32.516Z Reads: 67

```
This is not a sales thread in any way. This just a regular thread - i will update this when i make some progress. I make stuff like this for myself - as i said in a previous reply also.
```

---
## \#10 Posted by: SimosMCmuffin Posted at: 2018-02-15T21:03:28.495Z Reads: 68

```
Remember to account in the temperature co-efficiency of the Rds(on). AKA the resistance will increase with the junction temperature. Although calculating the loss is a bit tedious as the FETs heat up and cool down with changing load, but maybe using just the typical Rds(on) @ 25 C might not be quite realistic.
![image|447x421](upload://5snVKBZKbZGbP3UfEgwRimqkDZm.png)
https://www.infineon.com/dgdl/irlb3034pbf.pdf?fileId=5546d462533600a40153566027b22585
```

---
## \#11 Posted by: getyorma Posted at: 2018-02-15T21:16:13.404Z Reads: 58

```
Absolutely - a good remark. I will be testing the board next week and i will update the main thread with the aquired info. The fets are soldered on to the pcb just like an smd component. The board will help dissipate any excess heat. After all,  two of those are perfect for a dual vesc 4.12 build. Since the vesc pulls about 30A per board continious it should work fine. The main key of my project is to keep it low cost and robust.
```

---
## \#12 Posted by: SimosMCmuffin Posted at: 2018-02-15T21:29:55.662Z Reads: 49

```
Keeping it simple is often a good choice.
```

---
