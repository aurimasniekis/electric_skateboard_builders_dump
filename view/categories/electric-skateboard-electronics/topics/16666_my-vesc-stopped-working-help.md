# My vesc stopped working HELP

### Replies: 19 Views: 985

## \#1 Posted by: Quinlanbrown Posted at: 2017-01-25T20:42:31.731Z Reads: 76

```
so i was useing my board and it hit a carb and fliped over and after it worked for a second but then stopped when i tryed to get back on it didint and when i pust on the gas the pink light flashes 3 times then 3 more not sure what to do
```

---
## \#2 Posted by: NickTheDude Posted at: 2017-01-25T20:45:33.309Z Reads: 76

```
Plug it in and type "faults" in the terminal in BLDC tool.
```

---
## \#3 Posted by: Blasto Posted at: 2017-01-25T20:49:10.790Z Reads: 74

```
Most probably some physical damage... post some pictures...
```

---
## \#4 Posted by: Quinlanbrown Posted at: 2017-01-25T20:57:09.928Z Reads: 71

```
<img src="/uploads/db1493/original/3X/4/f/4f035efbbdb87a0ffc5b85327b2b9bc477722157.png" width="690" height="388">
so i need a new drv chip?
```

---
## \#5 Posted by: JohnnyMeduse Posted at: 2017-01-25T21:01:37.696Z Reads: 64

```
Not necessarily, it may also be cause by physical damage....
```

---
## \#6 Posted by: Eboosted Posted at: 2017-01-25T21:37:05.450Z Reads: 60

```
Your motor cables might have been disconnected and shorted at the moment of the crash, that could have caused a burnt VESC. I'm still a little dissapointed by how fragile this things are
```

---
## \#7 Posted by: Quinlanbrown Posted at: 2017-01-25T21:43:28.849Z Reads: 58

```
i was ridding the other day and the motor wires where spaking up but i put some electrical take on them and it still worked after that, i mite order a vesc X in hopes that its more durable, then get both my broken vescs fixed for a future build
```

---
## \#8 Posted by: Blasto Posted at: 2017-01-25T21:45:50.818Z Reads: 58

```

[quote="Quinlanbrown, post:7, topic:16666"]
i was ridding the other day and the motor wires where spaking up but i put some electrical take on them and it still worked after tha
[/quote]

you got lucky it was still working... that's an instant blow.
```

---
## \#9 Posted by: Namasaki Posted at: 2017-01-25T21:49:49.957Z Reads: 57

```
I'm guessing that shorted phase wires will kill any Esc not just the Vesc.

I have used 120a hobby style Esc's in the past and in my opinion they where more fragile than
the Vesc's I am currently using.
```

---
## \#10 Posted by: Eboosted Posted at: 2017-01-26T00:08:28.947Z Reads: 49

```
[quote="Namasaki, post:9, topic:16666"]
used 120a hobby style Esc's in the past and in my opinion they where more fragile thanthe Vesc's I am currently using.
[/quote]

I guess you meant sparkling? how did you see the sparks if you were riding the board?
```

---
## \#11 Posted by: Quinlanbrown Posted at: 2017-01-26T03:10:18.460Z Reads: 42

```
i was rideing at night and the wires started sparking when it went and when i used the brakeing so i stoped and turned it off and caried it home
```

---
## \#12 Posted by: wmj259 Posted at: 2017-01-26T14:01:28.530Z Reads: 39

```
I couldn't find anything for this size,  but I have seen from my dad's repair shop that gasoline lines in cars have this  connector that keeps two gas lines  together,  maybe it can be used to keep the phase wires together. 
The clip that has the two hooks pointing back inwards. 
<img src="/uploads/db1493/original/3X/2/8/288585166d6829038fdc633ea32442ceacf79a87.jpg" width="450" height="338">
```

---
## \#13 Posted by: JohnnyMeduse Posted at: 2017-01-26T14:05:58.552Z Reads: 39

```
or you could just use MT60 connector.... <img src="/uploads/db1493/original/3X/8/1/8151ee3e6ddbf4586d392961eb7d8cf0452cc2e9.png" width="500" height="500">
```

---
## \#14 Posted by: zmoney Posted at: 2017-01-28T19:36:49.036Z Reads: 33

```
Iv'e been eyeing those. Only draw back is that they are 3mm.
```

---
## \#15 Posted by: mmaner Posted at: 2017-01-28T19:39:55.344Z Reads: 33

```
[quote="JohnnyMeduse, post:13, topic:16666"]
you could just use MT60 connector....
[/quote]

I've got some, in black, that I'm going to use with my dual setup.
```

---
## \#16 Posted by: Maxid Posted at: 2017-01-28T23:14:06.682Z Reads: 31

```
Keep in mind that with those you can't just switch two motor phases to change direction.
```

---
## \#17 Posted by: JohnnyMeduse Posted at: 2017-01-28T23:15:29.967Z Reads: 31

```
Once your set you shoun't have to switch your phase wire.
```

---
## \#18 Posted by: Maxid Posted at: 2017-01-28T23:18:30.229Z Reads: 30

```
What does that mean? With a VESC it is fine but with a Car ESC it can be troublesome to change it via programming. Before soldering the connectors there is no way to tell without first trying normal bullet connectors and taking notes.
```

---
## \#19 Posted by: JohnnyMeduse Posted at: 2017-01-28T23:34:39.891Z Reads: 28

```
Hummm. I din't say these where easy to use because you can't change the direction vesc without switching phase cable, so basically you have to test it and unsolder / resolder in the right order the phase cable if needed.... but these provide a much more solid connection than regular bullet and if the connector detach itself, cable won't ever short, like what happen in the present case... Also in the case above (if you had read the thread), we are talking about VESC and not car esc, witch have bullet connector solder directly on them without any wire and won't short together if ever disconnect during use.
```

---
