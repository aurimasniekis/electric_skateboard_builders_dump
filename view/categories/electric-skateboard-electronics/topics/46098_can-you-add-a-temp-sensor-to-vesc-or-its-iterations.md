# Can you add a temp sensor to vesc or its iterations?

### Replies: 16 Views: 786

## \#1 Posted by: Hummie Posted at: 2018-02-11T07:06:35.594Z Reads: 124

```
das it.  need I say more.

be nice to see what actually winding temps to see what is most efficient.  infrared sensors aren't so accurate.
```

---
## \#2 Posted by: b264 Posted at: 2018-02-11T07:18:07.225Z Reads: 123

```
Hall/Encoder pin 2 is a temperature sensor input on 4.12

Hall/Encoder pin 5 is a temperature sensor input on 6.4
```

---
## \#3 Posted by: Nordle Posted at: 2018-02-11T07:35:11.102Z Reads: 110

```
You don't want to add hall sensors or an encoder to your hubs but a single temp sensor? Thats kinda silly...
```

---
## \#4 Posted by: Hummie Posted at: 2018-02-11T18:12:57.208Z Reads: 90

```
why silly?  In my experience sensors aren't necessary to get great slow speed control without cogging and they don't help efficiency and they break.  a temp sensor that's really accurate would tell a lot about efficiency
```

---
## \#5 Posted by: Nordle Posted at: 2018-02-12T07:35:16.198Z Reads: 65

```
Just my opinion, because the wires are the biggest part of these sensors, if you add one you can add all. And the difference in performance is significant. Or did you ever start uphills from a standstill with your hubs? I don't think so.
```

---
## \#6 Posted by: Hummie Posted at: 2018-02-12T07:44:17.213Z Reads: 61

```
i can get pretty damn close to an uphill from a standstill.  show you soon.  to me its for the lazy who cant do the slightest push.  if it showed efficiency gains then I'd be interested but haven't seen that
```

---
## \#7 Posted by: Der6FingerJo Posted at: 2018-02-12T07:45:50.546Z Reads: 56

```
[quote="Hummie, post:4, topic:46098"]
In my experience sensors aren’t necessary to get great slow speed control without cogging and they don’t help efficiency and they break.
[/quote]

Have you done something special in your configuration or so for that performance? 
On none of my boards i get the smooth startup performance with sensors disabled, or is it a hub motor thing?

I get that you can do a push but it just feels so much nicer to just roll away uphill without cogging.
```

---
## \#8 Posted by: Hummie Posted at: 2018-02-12T07:46:29.298Z Reads: 53

```
120 or 100 motor amps @Der6FingerJo
```

---
## \#9 Posted by: Der6FingerJo Posted at: 2018-02-12T08:02:42.260Z Reads: 51

```
Hah alright didn't think of that :ROFL:
```

---
## \#10 Posted by: Nordle Posted at: 2018-02-12T10:14:52.485Z Reads: 48

```
Its good for sure to use 120amps where 30 would be enough. Well if my machines would waste that much energy in heat i also would think about a temp sensor. But i already have one anyways near my hall sensors, and i only have those because i'm lazy or maybe because i want the feel of a premium product.
```

---
## \#11 Posted by: Hummie Posted at: 2018-02-12T17:17:41.391Z Reads: 45

```
If I can get halls in easily I'll do it. So far seems a lot of work.  I have a 3d printer n maybe can make a board for them.  

I'd like to see a comparison of 120 motor amps vs sensors. Sometime will happen
```

---
## \#12 Posted by: b264 Posted at: 2018-02-12T18:34:10.059Z Reads: 41

```
Maybe you could have **optional** Hall sensors as an add-on board that sits where a pulley would sit on a longboard wheel

That would also give you a convenient place to plug in an internal temperature sensor from the stator
```

---
## \#13 Posted by: Hummie Posted at: 2018-02-12T18:38:55.265Z Reads: 41

```
external?  theres so little room in the motor already but sounds fragile

but i'm sure I'll be into all those fixins after I get these fucking cans opened rubber poured and rolling.  damn had to order a crazy wrench and here in a day or two

still looking for testing to see how sensored compares in efficiency to sensorless.
```

---
## \#14 Posted by: Nordle Posted at: 2018-02-12T18:55:38.564Z Reads: 39

```
They fit in between stator teeth
```

---
## \#15 Posted by: Hummie Posted at: 2018-02-12T18:57:43.469Z Reads: 37

```
ive seen them on a board to orient them.  I think luke set them up without a board and took him like 3 hours otherwise.  
but are they more efficient or just for dare I say the lazy?  giving the slightest little push...I save a bit of juice
```

---
## \#16 Posted by: Nordle Posted at: 2018-02-12T19:03:30.852Z Reads: 34

```
i'm no expert but if you say you need 120 amps to do that and sensored motors do it better with half of that i just can immagine thats more efficient.
sensored is less efficient at high speeds can say that for sure, but vesc has hybrid mode.
```

---
