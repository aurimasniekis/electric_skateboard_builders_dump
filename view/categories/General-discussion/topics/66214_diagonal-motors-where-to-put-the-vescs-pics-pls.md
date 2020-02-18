# Diagonal motors&hellip; where to put the VESCs? (pics pls)

### Replies: 8 Views: 251

## \#1 Posted by: skelstar Posted at: 2018-08-27T07:01:51.769Z Reads: 122

```
I have a second motor to mount on my board and I _have to_ put it on the opposite corner from my first motor (i.e. on the front trucks). I have my current VESC on the back of the 3D printed battery enclosure.

I have my second VESC, but I wondering where to mount it:
- on the front of the battery enclosure (another 3D printed 'extension') and run a long CAN bus cable
- next first VESC at the back and run slightly long cables to the motor?

I would love to see pictures (or links) of anyone who has done this with the diagonally mounted motors.

Thanks!
```

---
## \#2 Posted by: Marsen Posted at: 2018-08-27T07:24:40.395Z Reads: 115

```
Any chance of pictures of you 3D printed enclosures. I have done one for the Bamboo GT to fit a bigger battery and always keen to look at other peoples designs.
```

---
## \#3 Posted by: skelstar Posted at: 2018-08-27T08:34:19.339Z Reads: 95

```
There are a few 3D printed enclosure threads around here. I don't have a pic of mine at the moment.
```

---
## \#4 Posted by: Andy87 Posted at: 2018-08-27T09:17:36.815Z Reads: 92

```
What deck you have?
How much space you have in your enclosure?
Which battery pack you use?

There different options fitting to different enclosure designs.

If you mount one VESC one every end of your enclosure, I wouldn´t use can (or as min only with shielded wires).
Not sure thou if it´s a problem, but I wouldn´t risk signal indifferences and in case of cut off CAN cable also to fry your VESCS.
You could just get a second receiver for your remote (one for every VESC) and bind them both to your remote.
```

---
## \#5 Posted by: skelstar Posted at: 2018-08-27T17:52:17.567Z Reads: 59

```
I have a Truncated Tesseract, custom 3D-printed enclosure (modular), so space inside the enclosure is immaterial.

I have created my own remote so getting another receiver is not trivial :). Not impossible, but...

Food for thought though. Cheers!
```

---
## \#6 Posted by: Andy87 Posted at: 2018-08-27T20:42:38.553Z Reads: 36

```
Can you split your battery and place your vescs in the middle?
No problem with can, no problem with long power cables from battery to the vesc.
Will be long Phase wires than but that shouldn’t be a problem
```

---
## \#7 Posted by: skelstar Posted at: 2018-08-27T20:46:29.554Z Reads: 41

```
The battery is one big 10S5P (too big) from dyeEboard.com.

Yeah I was worried about the long phase wires.

Will have to extend the length of my CAN cable and maybe put some shielding on it (some braid from maybe coaxial cable.. and twist the cable).
```

---
## \#8 Posted by: Andy87 Posted at: 2018-08-27T20:51:59.537Z Reads: 36

```
As far as I understand the problem only in the main power wires from battery to the vesc.
As there it’s dc current the induction can amplify voltage spikes which can fry your electronics.
The phase wires are ac so there shouldn’t be a too big problem if the longer.
```

---
