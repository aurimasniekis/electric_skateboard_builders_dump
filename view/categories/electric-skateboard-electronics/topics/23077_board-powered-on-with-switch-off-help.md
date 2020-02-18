# Board powered on, with switch off.. Help

### Replies: 22 Views: 1058

## \#1 Posted by: flywithgriff Posted at: 2017-05-15T01:23:56.082Z Reads: 104

```
I spent the day assembling the pack for my board and hooking everything up. Everything was perfect, programming went well, I charged the battery... literally everything was functioning perfectly. I let the board sit while I ate dinner and when I came back the board is powered on. The switch does not have an effect on the power, i even cut a wire to it to be sure it wasn't fried. Is it possible my BMS went bad? I am completely out of ideas.I have checked all the wires for a short, nothing anywhere.
```

---
## \#2 Posted by: JLabs Posted at: 2017-05-15T01:25:01.695Z Reads: 101

```
What switch are you using? Build into the BMS?
```

---
## \#3 Posted by: Smorto Posted at: 2017-05-15T01:25:20.212Z Reads: 99

```
Pics of the setup?
```

---
## \#4 Posted by: flywithgriff Posted at: 2017-05-15T01:27:38.836Z Reads: 97

```
The switch that came with the BMS. It's the BMS I spoke with you about from the group buy I bought from @mmaner.
```

---
## \#5 Posted by: flywithgriff Posted at: 2017-05-15T01:31:05.551Z Reads: 97

```
I noticed before this issue occurred that when the switch was on or off there was still a blue flashing led light near the balance port. Now it is off.


<img src="/uploads/db1493/original/3X/b/1/b1cd4e10df5b28336c16f6b7b192c01cf741f260.JPG" width="236" height="500">
```

---
## \#6 Posted by: flywithgriff Posted at: 2017-05-15T01:44:11.554Z Reads: 94

```
It has to be a bms issue. There is no way for power to backfeed from the vesc end of the circuit. Th positive wire goes straight to the vesc so that rules it out. The only thing left is a short in the BMS causing the negative current to jump through the bms bypassing the switch.
```

---
## \#7 Posted by: JLabs Posted at: 2017-05-15T01:46:51.461Z Reads: 91

```
Hmm, it worked when I sent it out to @mmaner

Are you sure everything is wired properly?
```

---
## \#8 Posted by: flywithgriff Posted at: 2017-05-15T01:48:30.499Z Reads: 88

```
It worked great today. I was literally ready to start test fitting the cover and this happened.
No pops, no smoke, no smell. I am completely lost.
```

---
## \#9 Posted by: JLabs Posted at: 2017-05-15T01:52:15.062Z Reads: 89

```
My assumption is a solder joint worked itself loose
```

---
## \#10 Posted by: flywithgriff Posted at: 2017-05-15T01:53:14.634Z Reads: 90

```
But wouldn't that cause a loss of power? I can't get the board to turn off. Am I wrong in thinking that the way this is wired there has to be power passing through the BMS in order to make the esc negative wife have power?


Here is both sides of the BMS.
<img src="/uploads/db1493/original/3X/6/d/6d24752d51b41e40d4356065c2ce27407d8e4881.JPG" width="375" height="500"><img src="/uploads/db1493/original/3X/d/e/de8e076e3307a4ce4c9b7c725684b9c703efabc3.JPG" width="666" height="500">
```

---
## \#11 Posted by: mmaner Posted at: 2017-05-15T02:56:15.183Z Reads: 74

```
Try putting a load in it, when bench testing the BMS will show transient voltage. After outting a load in it it should go away.  I would also suggest an in line volt.meter after the BMS, that way you know if it actually supplying power or it's transient.
```

---
## \#12 Posted by: flywithgriff Posted at: 2017-05-15T03:03:41.667Z Reads: 75

```
I have a voltmeter in place. That's how I know the system is powered on and it has been lit for over an hour now. I attempted to reconnect the vesc but got a pop when connecting the positive lead. I can hook it up again I was just worried about killing my vesc with an arc.
```

---
## \#13 Posted by: flywithgriff Posted at: 2017-05-15T03:30:11.310Z Reads: 69

```
I hooked everything back up and ran the motor for a total of about 3 minutes. The power is still on and the switch is still off.
```

---
## \#14 Posted by: Namasaki Posted at: 2017-05-15T03:38:55.754Z Reads: 67

```
Check where the switch wires are attached to the bms circuit board and make sure they are not shorted together and the solder holes are not shorted together.
```

---
## \#15 Posted by: mmaner Posted at: 2017-05-15T03:41:01.442Z Reads: 66

```
If you remove the switch from the circuit does it stay on?
```

---
## \#16 Posted by: flywithgriff Posted at: 2017-05-15T03:42:33.546Z Reads: 65

```
Unfortunately they aren't even close to being shorted.

@mmaner i removed one wire from the switch just in case it was a stuck switch and the board remained powered with only one wire on the switch.
```

---
## \#17 Posted by: Namasaki Posted at: 2017-05-15T03:45:25.797Z Reads: 65

```
What about on the circuit board where the wires are soldered? Could there be a bit of solder shorting the pads or holes where the wires are soldered?
```

---
## \#18 Posted by: flywithgriff Posted at: 2017-05-15T03:47:02.584Z Reads: 65

```
I don't see anything. The board worked just fine today for about two hours of being powered on without error. This happened all of a sudden while I wasn't even touching the board.

To rule out the switch i removed the switch leads from the bms, still powered on. i just took the B- wire off to kill the power.
```

---
## \#19 Posted by: mmaner Posted at: 2017-05-15T13:02:20.550Z Reads: 54

```
Thats strange brother, I dont know what it could be.  @JLabs you have any ideas?
```

---
## \#20 Posted by: flywithgriff Posted at: 2017-05-15T18:13:23.039Z Reads: 46

```
I just bought another BMS. I really don't see what else it could be.
```

---
## \#21 Posted by: SirDiff Posted at: 2017-05-15T22:24:54.121Z Reads: 33

```
Wait, so the bms was always on like it didn't have an eswitch? Couldn't you just use it with a loop key?
```

---
## \#22 Posted by: flywithgriff Posted at: 2017-05-15T23:20:29.015Z Reads: 29

```
The BMS stayed on constantly, correct. Yes I probably could keep using it with the use of a loop key. I've already ordered a replacement.
```

---
