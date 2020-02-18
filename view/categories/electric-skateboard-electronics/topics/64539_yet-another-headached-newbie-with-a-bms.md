# Yet another headached newbie with a BMS

### Replies: 7 Views: 280

## \#1 Posted by: reiko Posted at: 2018-08-11T10:38:18.012Z Reads: 98

```
Hey everyone, thanks for taking the time to read the topic.

I am having a hard time wrapping my head around wiring the BMS to bypass discharging and to be used only for charging. I have read numerous topics and watched countless videos, but still I do not feel confident to start soldering things together. 

I am using a 6s Multistar 10000mAh battery. I used Paint to sketch up a little wiring diagram of how I think this should work, but in reality have no idea if this is how it is actually supposed to work.

Anyways, here is my wiring diagram:

![BMS%20DISCHARGE%20BYPASS|424x500](upload://fFMHBvBAgAoleGg23KBeMuJ5JDw.png)

I would love to hear your feedback on it. Is it ok? What should I change?

Thanks a lot!
```

---
## \#2 Posted by: pat.speed Posted at: 2018-08-11T11:40:11.564Z Reads: 80

```
That is almost correct, the charge port should be connected to C- unless there is not one on this specific bms. The hardest part is getting the balance cables in the correct order, which you seem to have done
```

---
## \#3 Posted by: reiko Posted at: 2018-08-11T12:02:36.858Z Reads: 74

```
There's only P- and B-. Thanks a lot for your feedback, I'll try not to mess up the balance cables.
```

---
## \#4 Posted by: pat.speed Posted at: 2018-08-11T12:26:30.865Z Reads: 70

```
In that case it’s correct, some bms modules use a common charge/discharge terminal
```

---
## \#5 Posted by: Jake2k17 Posted at: 2018-08-11T14:48:00.037Z Reads: 58

```
The balance cables can be tricky, they go in order by voltage, however your diagram is correct but the ground balance wire does not need to be connected anywhere
```

---
## \#6 Posted by: Wilsonliang777 Posted at: 2018-08-12T05:38:44.300Z Reads: 44

```
My newbie mistake with bms was that I got the balance wires confused (backward)  becarful.  Use a device to check the voltage of the balance wires b4 connecting it to the bms. The wire that read 4.2v is b1.
```

---
## \#7 Posted by: TowerCrisis Posted at: 2018-08-12T07:04:27.723Z Reads: 31

```
Some BMS's will have a + next to one side of the balance port. In my case of an 8S BMS, the port is labeled 1 2 3 4 5 6 7 8+ with 8 being what connects to your main battery terminal.

Just make sure you read the datasheet for the BMS you're using
```

---
