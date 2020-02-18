# Vesc was clunking

### Replies: 7 Views: 556

## \#1 Posted by: Charster10 Posted at: 2016-11-28T19:56:59.814Z Reads: 47

```
Ok so i fixed eveything that was an issue...but now everything is perfect but i went for a 5 mile ride just then and every so often it would just go full throttle by itself like without me even touching the remote...anything i can change in the Bldc tool ? Thanks again!
```

---
## \#2 Posted by: longhairedboy Posted at: 2016-11-28T20:02:18.623Z Reads: 47

```
did you check your receiver wires for shorts? If the power lead and the signal lead short... you may find yourself streeting your face. I've had a number of situation involving this very thing and symptoms can vary depending on how badly its shorting. everything from intermittant stutters to the board just going full tilt out of nowhere, and to exacerbate the issue, if the remote drops its pairing because of something related to the short, you won't be able to do shit about it until a curb, bush, or car stops your board,  and its more likely to just go full blast in that situation. 

replace your servo (receiver signal) wires first and see what happens.
```

---
## \#3 Posted by: saul Posted at: 2016-11-28T20:04:21.218Z Reads: 44

```
yupp sounds like loose servo wire.

if it is a pin version I would remove them and solder wires, then hot glue to prevent shorts like lhb said this are bad.
```

---
## \#4 Posted by: longhairedboy Posted at: 2016-11-28T20:08:45.256Z Reads: 39

```
That's exactly what i do now in some of my builds. Just watch out for those solder bridges. 

Also if you're running dual VESCs over the CAN bus be sure those connections are solid too. Weird shit can happen there as well.
```

---
## \#6 Posted by: Charster10 Posted at: 2016-11-28T20:16:37.141Z Reads: 32

```
Where abouts would the be loose? Cant be on the vesc as there soldered but do u mean going into my reciever?
```

---
## \#7 Posted by: Charster10 Posted at: 2016-11-28T20:20:53.816Z Reads: 31

```
Where abouts would the be loose? Cant be on the vesc as there soldered but do u mean going into my reciever? @longhairedboy
```

---
## \#8 Posted by: longhairedboy Posted at: 2016-11-28T20:23:14.248Z Reads: 30

```
if you soldered your servo/receiver leads to the VESC then triple check for solder bridges. They can be tiny. Also check the receiver end if you're using a connector there, sometimes the connectors can have tiny hairs of wires peeking out from the crimps, but that's rare. also a loose or broken crimp in the connector can make weird shit happen. 

Also make sure you adjusted your signal range in BLDC tool for your receiver specifically, weird shit can happen if that's not done as well.
```

---
