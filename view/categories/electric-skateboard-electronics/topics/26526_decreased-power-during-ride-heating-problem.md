# Decreased power during ride.. heating problem?

### Replies: 13 Views: 764

## \#1 Posted by: flywithgriff Posted at: 2017-07-01T16:52:08.334Z Reads: 83

```
I have just finished a 10s build with a single vesc and 6374 on 90mm clones and 15/36 gearing. I just took it for a ride and after about a mile if 20-25mph riding I noticed the power seemed to be cut in half as well as braking strength decreased. I took about a minute break off of the board and everything was back to normal. Any ideas what could be causing the issue? I'm a heavy dude at 250lbs and the terrain is just slight elevations.
```

---
## \#2 Posted by: Jinra Posted at: 2017-07-01T17:04:12.107Z Reads: 79

```
Sounds like battery cutoff triggered due to voltage sag. What's your cutoff voltage at to. What battery do you have?
```

---
## \#3 Posted by: flywithgriff Posted at: 2017-07-01T17:06:25.029Z Reads: 76

```
10s1p Lipo (5x 2s 5ah 30c)
Cutoff starts at 33 shutdown at 30
```

---
## \#4 Posted by: Jinra Posted at: 2017-07-01T17:19:37.187Z Reads: 74

```
That should be adequate, it's probably overheating then. I'd reduce the size of the motor pulley for your weight. Probably 13T, or upgrade to dual motors of you want to keep 15T
```

---
## \#5 Posted by: flywithgriff Posted at: 2017-07-01T17:24:03.528Z Reads: 71

```
I certainly want to go dual and also pneumatics. But, that will have to wait. You think 13 on the motor would help?
```

---
## \#6 Posted by: Jinra Posted at: 2017-07-01T17:36:49.642Z Reads: 65

```
Yea you'll go from a 2.4:1 reduction to 2.76:1. If you can, try to go for a 3:1 reduction.
```

---
## \#7 Posted by: Alanhunt123 Posted at: 2017-07-01T18:37:31.233Z Reads: 66

```
I assume you are using a 4.xx VESC.

You could try cutting out the plastic casing and attaching some cheap aluminum heatsinks with some thermal paste.

@sl33py has an excellent DIY solution here as well 

 http://www.electric-skateboard.builders/t/how-to-heatsink-your-vesc/26129
```

---
## \#8 Posted by: flywithgriff Posted at: 2017-07-01T19:18:01.014Z Reads: 61

```
I am using an ollin vesc 4.12. Will any small aluminum heatsinks work?
```

---
## \#9 Posted by: sl33py Posted at: 2017-07-01T19:28:56.223Z Reads: 61

```
[quote="flywithgriff, post:8, topic:26526"]
Will any small aluminum heatsinks work?
[/quote]


@chaka's heatsink'd 4.12 VESCs are far superior to my hacked DIY heatsink...  Not sure how much improvement you'll get, but worth a shot.

Do you have decent airflow over the VESC now?  That's key for dissipating heat.  Then you just need more surface area - i'd add some inexpensive aluminum finned heatsink to help get it cooled down.

Also - where do you live?  Mojave Desert?  Ambient temp is a huge factor.

Edit - do you have the Ollin VESC with aluminum sandwich heatsink already?  I remember he has both versions and assumed you had the gorgeous CNC heatsink one, but you might've got it before he offered, or didn't spend the $ for that feature/upgrade?
```

---
## \#10 Posted by: flywithgriff Posted at: 2017-07-01T19:30:55.998Z Reads: 58

```
@sl33py I actually just pm'd you. I'm living just outside of NYC. The vesc I have is from ollin and only has about 60 miles in it. Can't afford to replace it as of now.

Edit: he didn't offer the Cnc case when I purchased my vesc
```

---
## \#11 Posted by: sl33py Posted at: 2017-07-01T19:58:27.640Z Reads: 55

```
gotcha.  Any interest in seeing if he can upgrade yours w/ CNC heatsink?  Far nicer than my DIY!  You likely need to send it back to him though...

Are you moderately handy?  My DIY heatsink is easy to make, but fiddly/time-consuming.
```

---
## \#12 Posted by: flywithgriff Posted at: 2017-07-01T19:59:35.219Z Reads: 56

```
I'm very handy! The problem is having just moved to an apartment outside of NYC and no tools or room.
```

---
## \#13 Posted by: chaka Posted at: 2017-07-01T23:48:01.951Z Reads: 41

```
A few things you can do. 

1 - you can vent your enclosure and get some fresh air circulating, "might" solve the overheating problem.

2 - PM me or send an email and we can talk about upgrading to our direct FET version with the aluminum heatsink enclosure.

3 - Lower your motor amps to reduce peak current during acceleration, 250lbs though... might want to hit me up for an upgrade.

I also have 14t, 15t, and 16t motor pulleys for 12mm belts if you need them.
```

---
