# Dead BMS on Delivery, help please

### Replies: 29 Views: 931

## \#1 Posted by: flywithgriff Posted at: 2017-08-27T21:40:26.032Z Reads: 90

```
I have just wired in a brand new Bestech 80A BMS and I am getting no power through it. If I bypass the BMS everything works fine. I have wired these before so Im 99% sure everything is wired properly.

B- to Battery Neg
P- to Vesc Neg
C- to Charge Neg

The ends of the e-switch are twisted together to rule out a faulty switch. There are no warm spots on the BMS as well as no parts that look burned or not soldered correctly.
```

---
## \#2 Posted by: Namasaki Posted at: 2017-08-27T21:50:22.045Z Reads: 90

```
Are the balance wires all connected properly?
Are you certain that every cell has adequate charge and is not tripping the low voltage protection.
Are you certain that you have no shorts anywhere thats tripping the short protection.
Note: that if any of the protections are activated, you will have to use the Eswitch to reset the bms, so you have to untwist the wires and retwist them.

If all that checks out, trace the Eswitch wires back to the pcb and see if one of them broke loose from the pcb

Note: these bms's are prepared per order and tested before shipped so the likelihood of a DOA bms is very slim unless it suffered some physical damage by customs or the shipper.
```

---
## \#3 Posted by: flywithgriff Posted at: 2017-08-27T21:55:24.980Z Reads: 82

```
I am 100% wired correctly and have tried resetting the switch. Could I have blown the fuse in the BMS?
```

---
## \#4 Posted by: willpark16 Posted at: 2017-08-27T22:05:23.061Z Reads: 81

```
Static electricity perhaps @Namasaki made me get an antistatic band before opening mine and it's had zero issues
```

---
## \#5 Posted by: flywithgriff Posted at: 2017-08-27T22:07:38.218Z Reads: 76

```
I see there is a fuse on the side of the BMS. Is this something that I can change to possibly fix the issue?
```

---
## \#6 Posted by: capfirepants Posted at: 2017-08-27T22:13:01.455Z Reads: 72

```
you could try bridging it with some wire just to test if it works - just don't pull any high amounts of current
```

---
## \#7 Posted by: flywithgriff Posted at: 2017-08-27T22:20:06.093Z Reads: 70

```
Please elaborate!
```

---
## \#8 Posted by: capfirepants Posted at: 2017-08-27T22:21:25.074Z Reads: 69

```
If you're sure there is a fuse and you think it's blown, you can take some wire and "replace" the fuse with it. Just do not pull loads of current - if the fuse blew it did so for a reason
```

---
## \#9 Posted by: chuttney1 Posted at: 2017-08-27T22:22:21.943Z Reads: 66

```
Which did you connect first, the balance wires or the main wires?
```

---
## \#10 Posted by: flywithgriff Posted at: 2017-08-27T22:23:22.788Z Reads: 65

```
Balance wires
```

---
## \#11 Posted by: chuttney1 Posted at: 2017-08-27T22:25:07.849Z Reads: 65

```
Just to clarify, the first you connected to the BMS is the balance wires from the battery to the BMS and then the red and black main wires?
```

---
## \#12 Posted by: willpark16 Posted at: 2017-08-27T22:27:06.010Z Reads: 65

```
U connect ur balance wires last
```

---
## \#13 Posted by: chuttney1 Posted at: 2017-08-27T22:30:16.080Z Reads: 65

```
In any case. Get yourself a New BMS. Connecting the balance wires first is a fatal mistake.
```

---
## \#14 Posted by: Jinra Posted at: 2017-08-27T22:31:26.575Z Reads: 66

```
I've had multiple BMS's (some bestech, some not) without anything besides the balance leads attached. Never burned anything out.
```

---
## \#15 Posted by: flywithgriff Posted at: 2017-08-27T22:36:08.693Z Reads: 62

```
I have used several bms and never had one burn up from attaching balance wires first.
```

---
## \#16 Posted by: Namasaki Posted at: 2017-08-27T22:46:51.239Z Reads: 60

```
[quote="flywithgriff, post:5, topic:31597, full:true"]
I see there is a fuse on the side of the BMS. Is this something that I can change to possibly fix the issue?
[/quote]


That is a temperature sensor. The bms has over temp protection.
```

---
## \#17 Posted by: Namasaki Posted at: 2017-08-27T22:48:07.057Z Reads: 61

```
[quote="chuttney1, post:13, topic:31597, full:true"]
In any case. Get yourself a New BMS. Connecting the balance wires first is a fatal mistake.
[/quote]

That is not correct.
You should connect the balance wires first and then the B- wire.
That is how I set them up
```

---
## \#18 Posted by: flywithgriff Posted at: 2017-08-27T22:49:34.131Z Reads: 59

```
This is what I did!!
```

---
## \#19 Posted by: Namasaki Posted at: 2017-08-27T22:50:58.456Z Reads: 59

```
did you check your battery cells with a volt meter?
IF one of your cells is low it will trigger the over discharge protection and the bms will shut off within micro seconds after you turn it on
```

---
## \#20 Posted by: flywithgriff Posted at: 2017-08-27T22:55:00.361Z Reads: 56

```
I put the pack together last week and all cells were balanced.
```

---
## \#21 Posted by: Namasaki Posted at: 2017-08-27T22:56:09.970Z Reads: 55

```
Check them again and what are the voltages?
you could have a bad weld or solder joint.
You can check voltages at the bms balance connector.
```

---
## \#22 Posted by: flywithgriff Posted at: 2017-08-27T22:57:04.217Z Reads: 55

```
It will take a few hours to break everything down.

Edit: I have access to another BMS that I will check it with.
```

---
## \#23 Posted by: Namasaki Posted at: 2017-08-27T22:59:01.491Z Reads: 56

```
before you break the battery down, check voltages at the bms balance connector
```

---
## \#24 Posted by: flywithgriff Posted at: 2017-08-27T23:50:27.840Z Reads: 51

```
I just used a wire and jumped the solder connection points for the switch wire on the BMS. It came to life!! Apparently the switch wire has a short somewhere.
```

---
## \#25 Posted by: Namasaki Posted at: 2017-08-28T00:05:28.121Z Reads: 49

```
You might want to just replace those stiff wires with some small silicone wire.
```

---
## \#26 Posted by: flywithgriff Posted at: 2017-08-28T00:12:36.992Z Reads: 49

```
I was so disappointed when it would not power on. @scepterr was a huge help in figuring out the problem!
```

---
## \#27 Posted by: scepterr Posted at: 2017-08-28T00:14:59.263Z Reads: 47

```
Silly Chinese wires :dizzy_face:
```

---
## \#28 Posted by: mmaner Posted at: 2017-08-28T03:18:09.768Z Reads: 42

```
I have a. Bestech BMS that had the same issue, spent 2 hours diagnosing and then replaced the switch wires and all was good.
```

---
## \#29 Posted by: flywithgriff Posted at: 2017-08-30T00:27:55.892Z Reads: 25

```
I'm really glad I wasn't the only one with this issue. Also glad I figured it out!
```

---
