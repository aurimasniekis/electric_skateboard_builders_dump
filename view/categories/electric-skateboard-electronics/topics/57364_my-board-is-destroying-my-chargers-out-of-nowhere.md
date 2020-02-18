# My board is destroying my chargers out of nowhere

### Replies: 16 Views: 343

## \#1 Posted by: ElskerShadow Posted at: 2018-05-31T16:51:21.408Z Reads: 131

```
Hey guys so I wanted to charge my board like I always do and when plugging the charger BOOOOM. I open the case, inspect the charge port nothing. I try again with another charger and BOOM. Now I don't have any other 10s charger :confused:
What could it be?
![1527785442412|375x500](upload://jr3Q1lXPYIvT68BL9h6uyzeLnUX.jpg)

Charger is blinking red, if I plug something it kills it instantly. So I have two questions then how can I repair all the chargers I just broke ( change capacitors maybe??)
And what the heck is happening to my board?!
```

---
## \#2 Posted by: linsus Posted at: 2018-05-31T17:01:24.121Z Reads: 121

```
My bet is that the fuse in the chargers blew, depending on the charger obv. 
If you they do indeed have fuses. It means that something is short circuitinng your + and - on your board (unless power socket is funky).
Use a multimeter and see if you have connection between + and - in the charger port. That would be the first steps.

come back with results.
```

---
## \#3 Posted by: b264 Posted at: 2018-05-31T17:09:56.064Z Reads: 113

```
Measure the voltage on the charger jack BUT DON'T STICK MULTIMETER PROBES IN IT.  Plug a male 5.5mm x 2.1mm barrel plug into it and probe the back of the plug.

It should be at battery voltage.  If it's 0V, check continuity across it.
```

---
## \#4 Posted by: ElskerShadow Posted at: 2018-05-31T17:41:50.077Z Reads: 98

```
I am following your recommendations and will come back with the results thanks guys
```

---
## \#5 Posted by: deucesdown Posted at: 2018-05-31T17:49:08.435Z Reads: 87

```
Lab PSU or one of those DPS units is helpful here. You get a display for voltage, and you can limit current to like 100mA to test.

What voltage are you getting at the charge port of the pack?
```

---
## \#6 Posted by: ElskerShadow Posted at: 2018-05-31T17:56:28.839Z Reads: 78

```
Battery is at 34.4 volt
@b264 i don't really know what you mean by plug?
```

---
## \#7 Posted by: ElskerShadow Posted at: 2018-05-31T17:59:22.549Z Reads: 71

```
I tried to check the voltage at the plug and it exploded, litteraly I will have to change it and cheik again can I just check the two wires maybe?
```

---
## \#8 Posted by: b264 Posted at: 2018-05-31T18:01:26.549Z Reads: 74

```
[quote="ElskerShadow, post:7, topic:57364"]
I tried to check the voltage at the plug and it exploded
[/quote]

I don't usually write in all-caps but that's why I said don't stick multimeter probes in there in all caps and suggested using a plug.  Don't ask me how I know....
```

---
## \#9 Posted by: ElskerShadow Posted at: 2018-05-31T19:03:06.912Z Reads: 56

```
Haha I just learn by mistake I tried with a bullet connector but didn't worked
```

---
## \#10 Posted by: deucesdown Posted at: 2018-05-31T19:03:47.792Z Reads: 56

```
[quote="ElskerShadow, post:7, topic:57364"]
I tried to check the voltage at the plug and it exploded
[/quote]

For explosions, there must be large flow of current, right? I'm thinking, there are 3 ways for this to happen at the plug.

1. battery demands huge current and charger provides it. Can't really happen as charger has a current limiter.

2. charger demands large current from battery. Can't really happen as the voltage at the charger is higher than 34.4v (water can't flow uphill).

3. there's a short somewhere.
```

---
## \#11 Posted by: ElskerShadow Posted at: 2018-05-31T19:04:32.564Z Reads: 56

```
[Uploading...]()
Should I do like so?
```

---
## \#12 Posted by: ElskerShadow Posted at: 2018-05-31T19:04:59.509Z Reads: 56

```
![1527793478872|375x500](upload://hDAwQYpp7aAaEOVxiXenRj34z5j.jpg)
```

---
## \#13 Posted by: deucesdown Posted at: 2018-05-31T19:06:41.261Z Reads: 53

```
I think he's saying

https://www.pimfg.com/products-large/VB870-DC-N-72-1.jpg?v=2

probe the wire ends.
```

---
## \#14 Posted by: b264 Posted at: 2018-05-31T19:12:45.053Z Reads: 53

```
:arrow_up: yes, that

OR this

![20180512_200413|690x345](upload://h14iHjTbiGPj2B4N7DI0VYzlO2q.jpg)
```

---
## \#15 Posted by: ElskerShadow Posted at: 2018-05-31T19:19:23.951Z Reads: 51

```
Alright I get it I m just dumb then :slight_smile: I found a new DC port and I will try again where is negative and positive so I don't mess up? . There is 3 pins ![1527794313922|375x500](upload://8W4NpTVADelFQbF2CbyWACfOveE.jpg)
```

---
## \#16 Posted by: L3chef Posted at: 2018-05-31T19:27:28.545Z Reads: 46

```
Plug the charger in the connector and meassure it with a multimeter. You will either see like ~35v or -35v 
Then you know wich is negative and positive
```

---
