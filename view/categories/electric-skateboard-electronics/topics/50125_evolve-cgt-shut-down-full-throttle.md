# Evolve CGT Shut Down Full Throttle

### Replies: 19 Views: 1116

## \#1 Posted by: omgomeromg Posted at: 2018-03-25T23:08:50.628Z Reads: 211

```
Got a Problem with my Evolve CGT AT :frowning:   Goin Full Throttle in GT Mode the Board completely shuts down (no more light on power switch). It happens only in GT Mode so i guess the Error is due high current .  Already got a brand new Battery but it still happens. I doubt its Voltage Sag as 10S5P VTC6 should deliver enough Amps.  Any Idea how to found out if its a ESC or BMS Error? Already checked wireing. Is it possible to bypass the BMS for discharging on  Evolve Board?
```

---
## \#2 Posted by: Jebe Posted at: 2018-03-26T00:55:10.578Z Reads: 188

```
Do you have the old battery to try?
```

---
## \#3 Posted by: b264 Posted at: 2018-03-26T02:01:08.115Z Reads: 179

```
I had an issue with the power switch where when you turn it on, you need to push it in one fluid motion and very firmly.  It can be on, but not latched inside and bumps & vibrations cause the power switch to turn off the board.

Does it only turn off during lots of bumpiness?
```

---
## \#4 Posted by: omgomeromg Posted at: 2018-03-26T10:37:00.738Z Reads: 160

```
happens only durin high amp draw (full throttle in GT Mode) no problem with power switch
```

---
## \#5 Posted by: omgomeromg Posted at: 2018-03-26T10:38:07.218Z Reads: 149

```
old battery same error. thats why i got a new pack
```

---
## \#6 Posted by: Skitzor Posted at: 2018-03-26T10:54:24.100Z Reads: 142

```
Does Evolve use their BMS for discharging too? Then your problem will probably be there.
```

---
## \#7 Posted by: omgomeromg Posted at: 2018-03-26T10:58:35.331Z Reads: 141

```
yes Evolve BMS is used for discharging.  any idea how to found out if BMS makes the Board Shutdown?
```

---
## \#8 Posted by: DeathCookies Posted at: 2018-03-26T11:23:52.975Z Reads: 136

```
Try bypassing it :D it is a bit soldering but then u'll know

Edit: can it be bypassed though? is there communciation needed between their esc and bms?
```

---
## \#9 Posted by: omgomeromg Posted at: 2018-03-26T11:28:07.438Z Reads: 131

```
bms is connected to ESC (uart and an e switch) :( so i guess its not possible
```

---
## \#10 Posted by: omgomeromg Posted at: 2018-03-30T09:47:24.529Z Reads: 115

```
bypassing failed :( . . Board stays on after connecting Battery directly to the ESC (E switch on bms) . will  check and redo all the connections and solder jobs on bms again. will also check the cells in the hidden Battery Menu durin the ride. maybe a bad Cell sag and trigger low voltage cutoff on the bms. Good news.. Evolve France is willing to sell me BMS. but iam still not 100% sure that the BMS is really the Problem. can it be cold weather that makes the ESC shutdown? i heard sometimes RC Flyers have this problem.
```

---
## \#11 Posted by: Goonman Posted at: 2018-10-14T10:05:57.830Z Reads: 92

```
Was that the only problem with bypassing the BMS? I want to use a different battery and chemistry it will be a 12s lifepo. I'm happy enough using an anti spark key.
```

---
## \#12 Posted by: Lambjr088 Posted at: 2018-10-14T10:35:42.815Z Reads: 86

```
Do the bypass and add a loopkey to turn it on and off
```

---
## \#13 Posted by: Wesselbrussen Posted at: 2018-10-20T00:41:16.748Z Reads: 78

```
This is also happening to my GT bamboo, let me know if you figured out what the problem was. Can't seem to find any info.
```

---
## \#15 Posted by: walterafable Posted at: 2018-10-20T04:40:52.530Z Reads: 73

```
With the battery upgrade, did you flip the BMS onto the ESC? If so, did you reposition the temperature sensor wire? If you left it untouched, it might be reading high temps from the ESC and shutting down the board when you’re throttling in GT. Try moving it around, back onto the battery pack, if possible, or to a relatively empty space in the enclosure.
```

---
## \#16 Posted by: Goonman Posted at: 2018-10-20T11:12:43.474Z Reads: 62

```
Tried bypassing BMS. ESC won't stay on without balance leads connected to bms. I was wondering if I could just manually close a switch between the red and black batt wires going from BMS to ESC. I think the ESC uses UART to see the cell information. No information no worky.?
```

---
## \#17 Posted by: Wesselbrussen Posted at: 2018-10-29T01:03:00.144Z Reads: 54

```
Just ordered a new battery pack as well, don't think it'll change anything. Have you figured it out yet or still just cruising in fast mode like me?
```

---
## \#18 Posted by: Sn4pz Posted at: 2018-10-29T01:33:25.131Z Reads: 53

```
[quote="Wesselbrussen, post:17, topic:50125"]
don’t think it’ll change anything
[/quote]

with a new battery every evolve product will need a new remote, reciever and esc

EDIT: my bad i misread, carry on :laughing::sweat_smile:
```

---
## \#19 Posted by: Wizeartz Posted at: 2019-09-17T02:48:46.826Z Reads: 30

```
Did you ever resolve this? I'm getting the problem too. I'm guessing the black wires with a black blob on the end is the temp probe and needs relocating. I'm running 10S5P of 18650's Samsung 35E's

Cheers
```

---
## \#20 Posted by: wallscw8 Posted at: 2019-09-23T12:49:57.015Z Reads: 19

```
Hey FYI I cut off my temperature sensor and it still has this issue, bamboo gtx. Will try a custom BMS bypass while still enabling the voltage readouts. will lyk.
```

---
