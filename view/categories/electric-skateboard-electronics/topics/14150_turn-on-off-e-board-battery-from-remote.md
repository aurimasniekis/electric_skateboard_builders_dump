# Turn on/off e-Board battery from remote

### Replies: 4 Views: 764

## \#1 Posted by: Eboosted Posted at: 2016-12-04T02:46:08.183Z Reads: 113

```
What electronic component would I need to turn on/off the battery from the remote? Is this even possible? 

If so, would this consume a lot of battery overnight or when it's not on use?
```

---
## \#2 Posted by: NNGG Posted at: 2016-12-04T03:09:56.043Z Reads: 107

```
You would need a servo to disconnect the battery from the esc. This is doable but stupid.  loop key attached to a fishing line would be a good emergency brake.
```

---
## \#3 Posted by: JuniorPotato93 Posted at: 2016-12-04T03:20:06.192Z Reads: 103

```
You do not need a servo if you have an e switch. Youll have to run the receiver from a ubec so it constantly has power and a controller with 2 or more channels. Now I dont know much about electronic components but assuming you have power to the receiver at all times and you can use a secondary circuit that takes the signal from the 2nd channel and provides power to a transistor like on an e switch to control the power on/off to the e switch then I think you could do it.

So to recap, constant power to the receiver. Then you'll need to remove the factory toggle on/off switch and connect that to a transistor. That transistor is part of the secondary circuit which must also always have power and can be powered by the ubec as well. Then calibrate the secondary circuit to interpret a momentary pulse as an on/off signal. 

I actually think this is quite doable though I simply dont know enough about electronics to figure it out. But if someone DOES make this a reality then sign me up for one.
```

---
## \#4 Posted by: saul Posted at: 2016-12-04T18:16:28.554Z Reads: 47

```
it could be done with an arduino + nrf tx/rx pair. ubec/buck (always on). and a mosfet in place of a eswitch pushbutton.

with the rx in sleep mode and using the irq line to "wake" the rx and then power on the board it would only use a few ma (maybe na in sleep mode).

But it adds another thing that can fail. Is it really that hard to push 2 buttons? :sob:
```

---
