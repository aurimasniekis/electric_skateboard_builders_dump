# Need sensor soldering help (5pin to 6pin JST)

### Replies: 12 Views: 131

## \#1 Posted by: whaddys Posted at: 2019-09-09T23:55:14.685Z Reads: 37

```
So I’d like to replace the male sensor pieces from my hub motors (5pinJST) to 6pinJST so that they fit into these FVT sleeping Lions. First off, is this even possible?
![IMG_5552|375x500](upload://ua9hPIxmFZBDqnrgcBcGceWvEXj.jpeg) 
![IMG_5550|375x500](upload://hRnRXE7OrxFBdWgtMwviWa0DShi.jpeg) 

The problem, as you can see, is that the 6pinJST I want to solder on is not color coded and I have no idea which phases would go where. From what I’ve read I would just not solder the temp wire (the extra wire out of the 6/5) but I have no idea which wire is temp here. They are all black…What do I do??
```

---
## \#2 Posted by: glyphiks Posted at: 2019-09-10T02:11:26.758Z Reads: 28

```
Can you power the motor and check the pins with a multimeter?
```

---
## \#3 Posted by: whaddys Posted at: 2019-09-10T02:14:41.424Z Reads: 27

```
sure I could do that - where do I place the leads of the multimeter?  One on the JST pin and the other one?
```

---
## \#4 Posted by: glyphiks Posted at: 2019-09-10T02:18:44.244Z Reads: 28

```
Neg of ESC should work?
```

---
## \#5 Posted by: whaddys Posted at: 2019-09-10T02:33:16.392Z Reads: 27

```
wait, sorry I'm confused.  
![IMG_5556|375x500](upload://iATykUxHzPHO4uy5EWTO5Oep4MR.jpeg)
```

---
## \#6 Posted by: glyphiks Posted at: 2019-09-10T02:55:27.953Z Reads: 24

```
The negative of wherever your power is coming from should work no?
```

---
## \#7 Posted by: whaddys Posted at: 2019-09-10T02:57:49.806Z Reads: 23

```
So just to map out the purpose of this experiment - how am I using the numbers I get in my readings for each of these 5 pins to figure out my soldering situation?
```

---
## \#8 Posted by: whaddys Posted at: 2019-09-10T03:00:49.219Z Reads: 22

```
Would I also take the 6pin JST, plug it into the VESC, and then get the readings of the 6 pins from there and then compare the readings across both JST's?
```

---
## \#9 Posted by: whaddys Posted at: 2019-09-10T03:07:26.040Z Reads: 22

```
Do I need to open my battery pack up to do this shit?  lol sorry I'm new to this level of measuring current...Or measuring current period...
```

---
## \#10 Posted by: glyphiks Posted at: 2019-09-10T05:13:06.371Z Reads: 19

```
Nah you just need to find anywhere negative on the same circuit, preferably close to where you are measuring. there's gotta be somewhere you can stick it 🤣 i would measure all of them and take note of them and try to figure out which is tthe temp sensor fron the readings.

I dont know what im talking about btw, just suggesting the course of action I would take 😬
```

---
## \#11 Posted by: glyphiks Posted at: 2019-09-10T05:14:38.493Z Reads: 20

```
You want the readings from the motor, not the ESC. You should have a schematic of the order to the ESC no?
```

---
## \#12 Posted by: whaddys Posted at: 2019-09-10T14:11:41.316Z Reads: 15

```
I'll have to search for a schematic on this ESC but I'm sure it exists
```

---
