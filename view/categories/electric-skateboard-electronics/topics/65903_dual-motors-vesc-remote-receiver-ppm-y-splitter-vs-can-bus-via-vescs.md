# Dual motors/VESC: Remote receiver PPM Y splitter vs CAN Bus Via VESCS?

### Replies: 6 Views: 731

## \#1 Posted by: Taliesin Posted at: 2018-08-24T01:31:44.437Z Reads: 185

```
I need some insight/clarification.

Currently I have a PPM Y splitter between my ESCapes, connecting to my remotes receiver, and no CAN bus.

From what I understand, this means I will need to set up each VESC individually one at a time with equal settings, then program the remote to an individual VESC and hope that it controls both?  Will this work?

On the other hand,

If I were to be using a CAN bus, then I would not need the ppm splitter? With a can bus you can program both vescs at once and then the remote can/will be programmed to both at the same time?

Is there any reason you would need the ppm splitter AND a can bus?

I don’t have the can bus wiring readily available so I’m hoping I can make this work with the ppm splitter.  

Does anyone know the pros and cons of both?
```

---
## \#2 Posted by: abenny Posted at: 2018-08-24T01:43:05.449Z Reads: 178

```
with the split ppm you set up each motor individually on each esc, and you set the remote on each esc individually as well.
as for differences between canbus and split ppm; can bus has a traction control option...but i cant comment on it because i use split ppm myself.

and no, you would never use both split ppm and can bus.
```

---
## \#3 Posted by: Taliesin Posted at: 2018-08-24T01:57:14.372Z Reads: 164

```
Ok thanks man that helps clear it up
```

---
## \#4 Posted by: dareno Posted at: 2018-08-24T03:05:43.734Z Reads: 156

```
Split ppm works well its just a bit more long winded to program but make sure that your cabling is not supplying too much voltage to the receiver.  One vesc should have all three wires connected and the other should have just the signal wire.
```

---
## \#5 Posted by: Andy87 Posted at: 2018-08-24T04:45:10.964Z Reads: 150

```
On top of what the other guys already said.
With split ppm you programm two master separated. 
With can bus you have a master and a slave.
With can bus you have traction control and you can get data from both your focboxes with only one Bluetooth module (in case you use). You can also change your settings on both focboxes on the go via any Esk8 app.
With ppm you will not fry your focbox by unfortunately disconnect the can plug while operating. Make sure please the with split ppm you cut one of the power wires on the y-split adapter
```

---
## \#6 Posted by: PartyPoison Posted at: 2018-08-24T11:31:09.458Z Reads: 138

```
This is a long thread! But if you want to learn you can read this!
https://www.electric-skateboard.builders/t/y-piece-or-canbus/26461?u=partypoison
```

---
