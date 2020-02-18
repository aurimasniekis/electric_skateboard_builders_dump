# What happens when

### Replies: 9 Views: 408

## \#1 Posted by: FabianOdermatt Posted at: 2018-05-23T19:11:51.520Z Reads: 156

```
…I shut the board off while driving?

Let's say there is a loose connection and mid driving the VESC gets no power anymore.
What happens? Will the board just ride out, or will it brake? And are there some options in the BLDC-Tool to adjust for such a scenario?

Thanks for your help. :slight_smile:
```

---
## \#2 Posted by: Deckoz Posted at: 2018-05-23T19:19:13.591Z Reads: 150

```
If your power wires are the loose connection you talk about. The BEMF voltage will keep the power running on the ESCs. But if you brake the current has no where to go and quickly over voltage and fry the ESC. 

So make sure your power connection doesn't break so you always have brakes...
```

---
## \#3 Posted by: FabianOdermatt Posted at: 2018-05-23T19:30:37.395Z Reads: 131

```
Yeah I meant the power connection.
And there isn't something like a parameter to change, that when the VESC gets no voltage it shuts off or just don't reacts to the remote anymore?

The problem is, I do not really trust my anti-spark switch and I don't want to fry the VESC because of this.
```

---
## \#4 Posted by: Deckoz Posted at: 2018-05-23T19:35:04.042Z Reads: 117

```
The only setting to help you is the max voltage(default 57v) but sometimes that isn't fast enough to cut the braking off and save the vesc.

You options area hard connection, Or something like a brake chopper/braking resistor... 

Most Antispark fail open meaning the boards are stuck on.. so if the Antispark fails you still have power.. you just won't be able to turn off your board.
```

---
## \#5 Posted by: ih8Darian Posted at: 2018-05-23T20:21:59.046Z Reads: 99

```
I have a low rider and when I was riding over a weird crack it hit my power button and turned my board off. It just kept on riding out so I wasn't in danger at all.
```

---
## \#6 Posted by: TehAtheist Posted at: 2018-05-23T21:02:26.116Z Reads: 83

```
To be honest I think the scenario where a motor wires comes loose or creates a bad connection is more dangerous/appears more frequent.

If such wire comes loose and starts to make a bad connection, the motor will lock up. Such a sudden lock up might throw you off.
```

---
## \#7 Posted by: RedEagle Posted at: 2018-05-23T21:15:47.212Z Reads: 75

```
Your vesc will go though a series of brownouts as a result of the BEMF voltage when no battery is connected. 
It's highly recommended you have a battery connected at all times when riding. 
You would burn your vesc if you don't. Or you could just disconnect all phase wires, but you won't have brakes.
```

---
## \#8 Posted by: Sn4pz Posted at: 2018-05-23T22:30:01.350Z Reads: 53

```
Im sorry for the probably idiotic question, but if my battery pack outputs 50A, and i were riding at about 20 mph and slammed the breaks to a stop, is it possible to have over 57v and fry it? How much power actually makes it back to the vesc?
```

---
## \#9 Posted by: Deckoz Posted at: 2018-05-23T22:38:09.700Z Reads: 45

```
[quote="Sn4pz, post:8, topic:56507"]
How much power actually makes it back to the vesc?
[/quote]

As long as your battery is connected, the vesc follows "batt min" setting. If you are having issues hitting 57v over voltage fault with your battery plugged in:

Either your BMS is limiting the Regen. Or a series connection is broken on your pack. 

Basically the only way you could fry the ESC if the battery is connected, it's not your BMS, and your battery is fine. Is if you were going down a hill faster then your no-load speed and try to brake.
```

---
