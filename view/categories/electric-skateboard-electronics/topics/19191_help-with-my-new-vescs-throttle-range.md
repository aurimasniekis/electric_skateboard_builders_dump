# Help with my new vescs-Throttle range

### Replies: 14 Views: 1082

## \#1 Posted by: krloz Posted at: 2017-03-16T22:05:58.359Z Reads: 97

```
i need some help with my newly arrived vescs.
firstly i have the problem that my throttle range is only one third of the remote range, im using a gt2b in a mad munkey enclosureand had absolutely no issue when using other esc before. i have tried everything i have found in this forum and cant get more than a range from about 1.5 to 1.65 pwm. and the remote ranges from 0.75 to 2.0 as read by the bldc tool.
the main issue however, is that putting exactly the same configuration on bothvescs, i get a good overall response from one of them (except from the range issue) and the other one, boots up with 3 red flashes and whenever i tried braking at anything above abolute minimum speed i get an over voltage error and it reboots. only on one of them.
i have both vescs 4.12 from scramboards (the yellow+heatsink design) to two sk3 236kv turnigys and powered out of a bench psu (i still didnt get connectors to wire apropiately to battery) set to 25v. but the psu gave me absolutely no issue with the other vesc
any ideas???
<img src="/uploads/db1493/original/3X/e/8/e8ce097f7a24cfe86cb8d04951bc1843ccbbb830.JPG" width="690" height="371"><img src="/uploads/db1493/original/3X/a/1/a1d338f5e2350b5ab2620d1ec8d591260d468174.JPG" width="690" height="371"><img src="/uploads/db1493/original/3X/e/d/eda39fd80b58c44e5bbe50b6ae4c67b60161a5eb.JPG" width="690" height="371"><img src="/uploads/db1493/original/3X/9/1/9121efa4b5603a3abf43f2d4c76720140ca491c8.JPG" width="690" height="371"><img src="/uploads/db1493/original/3X/8/a/8ac878781356472b0dae530b543a59d393d94c3d.JPG" width="690" height="371">
```

---
## \#2 Posted by: Blasto Posted at: 2017-03-16T22:17:13.051Z Reads: 82

```
Reduce your batt max to 25A and batt min -10A
```

---
## \#3 Posted by: krloz Posted at: 2017-03-16T22:37:15.605Z Reads: 81

```
tried. same issues:sweat:

I read that the three red b,inks is normal in bootup. no problem with that. but I still have one vesc with no braking abilty and a minimum throtle range. any other things i can try?
thank you very much
```

---
## \#4 Posted by: Namasaki Posted at: 2017-03-16T22:43:11.039Z Reads: 80

```
Are you connecting both Vescs to the receiver with a Y connector or are you connecting the Vescs together with a can bus cable?
```

---
## \#5 Posted by: krloz Posted at: 2017-03-16T22:45:42.535Z Reads: 73

```
just testing them for now one at a time. near future, can bus I hope.
I have a Y cable, schottky isolated power, though if needed.
```

---
## \#6 Posted by: Blasto Posted at: 2017-03-16T23:00:11.658Z Reads: 68

```
Diode huh.... can you draw up your setup (getho schematic), if you have a diode in series with the power you will have no regenerative braking since the diode will block the reverse current
```

---
## \#7 Posted by: krloz Posted at: 2017-03-16T23:13:53.761Z Reads: 69

```
no. my bad. didnt explain correctly.
absolutely no diode in the power conecrtions.
I meant i have a servo y wire with diodes to prevent 5v from both becs when connecting to receiver. but not using it at all.
My good vesc does brake with regenerative, and the psu eats ir up. but the bad one doesnt brake at all, gives the over voltage fault blinks red and goes on again after 3 seconds. the motor doesnt brake. it spins freely.
```

---
## \#8 Posted by: Blasto Posted at: 2017-03-16T23:16:15.748Z Reads: 63

```
Did you try with a battery setup? Usually power supplies do not like breaking/regen
```

---
## \#9 Posted by: Titoxd10001 Posted at: 2017-03-16T23:18:43.969Z Reads: 59

```
the issue could be the gt2b mod. You should try to limit brake travel (physically) so that minimum pulsewidth is 1. The mod allows to much travel compared to stock gt2b case.
```

---
## \#10 Posted by: krloz Posted at: 2017-03-16T23:19:27.125Z Reads: 57

```
not yet. im waiting for connectors. but i will try to hook it up somehow safe tomorrow (its sleeping time in this timezone) what worries me is that the same psu, same cables and same motor breaks perfectly with one vesc and nothing at all with the other one
```

---
## \#11 Posted by: krloz Posted at: 2017-03-16T23:55:45.435Z Reads: 52

```
will also try that tomorrow. thanks
```

---
## \#12 Posted by: krloz Posted at: 2017-03-18T21:42:22.552Z Reads: 37

```
Hooked to battery. Now i have power and regen braking on both vescs.
Absolutely no idea how on Earth the same psu, wires motor and rx/tx can have regen braking on only one of 2 idéntical vescs. But good enough
```

---
## \#13 Posted by: krloz Posted at: 2017-03-18T21:45:49.606Z Reads: 38

```
Tried limiting the path of braking. Now i have minimum at 1 máximum at 2 and deadband at 0.1. but still same issue with both vescs. All throttle range IS between 1.5 and 1.65 where It Gerardo Max speed
```

---
## \#14 Posted by: Titoxd10001 Posted at: 2017-03-19T02:01:27.080Z Reads: 33

```
With the range issue when you say throttle range is between 1.5 and 1.65 do you mean the motor spins to max speed or pulsewidth signal reaches 100%.
```

---
