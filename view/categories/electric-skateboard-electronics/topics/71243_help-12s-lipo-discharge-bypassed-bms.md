# HELP 12S lipo discharge bypassed BMS

### Replies: 11 Views: 727

## \#1 Posted by: TheFluffiest Posted at: 2018-10-14T22:08:01.601Z Reads: 113

```
Hey there, I am having a big problem wiring my 4x3s lipos to make a 12s setup. I have the wiring between batteries done, but the bms is giving me problems. I've attached a diagram of my wiring, but forgot an antispark key between the charging port and the volt meter.

I fully charged all 3s batteries to 12.6 (4.2v/cell) before wiring, and now they are at the voltages at the left in the diagram. They have never been discharged and haven't even been hooked up to anything that would discharge them. I am at a completely loss as to how that would happen, but here we are. 

Is my diagram correct? 

![15395548511042602249557806278347|281x500](upload://mOJuBUbzjw7zZuTE25oShPdPBD9.jpeg)
```

---
## \#2 Posted by: Andy87 Posted at: 2018-10-15T11:36:17.746Z Reads: 97

```
Which bms you have?
Did you check the over all voltage of your cells after putting them together? I mean without bms.

Sometimes it’s not necessary to connect the b- to the first pin. Only the main b- from the power lead. Like here
![image|507x500](upload://pnwj9q0y5SwKfWDcI63C0Gx3cWW.jpeg)
```

---
## \#3 Posted by: TheFluffiest Posted at: 2018-10-15T23:23:43.794Z Reads: 87

```
I did, and it was correctly. I checked them individually and together. I'm using this:

https://buildkitboards.com/collections/batteries/products/bestech-d140-charge-only-bms?variant=12511076909150

Hmm... That still wouldn't drain it like that would it? I will take off the negative pin and see what happens. The voltage is the same even without anything plugged in though
```

---
## \#4 Posted by: Andy87 Posted at: 2018-10-16T03:55:12.112Z Reads: 77

```
That shouldn’t be an issue, but for the d140 definitely the b- on the balance leads is free (is connected on the pcb with the main b-)
![image|230x500](upload://7KCZG5qRM6wXto2FMLW8QxJdOht.jpeg)
```

---
## \#5 Posted by: TheFluffiest Posted at: 2018-10-16T05:05:41.805Z Reads: 70

```
Oh hey! I probably should have looked up the actual wiring diagram for it. What are the odds this thing is blown at this point? I can guess the lipos are dead, but what about the bms?
```

---
## \#6 Posted by: b264 Posted at: 2018-10-16T05:37:55.367Z Reads: 71

```
Charger negative does not go on B-, it goes on C-, P-, or N- in that order if they are present
```

---
## \#7 Posted by: TheFluffiest Posted at: 2018-10-16T05:47:56.407Z Reads: 68

```
Got it. There a p-. I figured it would go that way since I'm bypassing discharge. I wouldn't imagine doing that would fry the bms would it? What do you think about all that?
```

---
## \#8 Posted by: b264 Posted at: 2018-10-16T05:55:08.488Z Reads: 68

```
Charging is the one thing you need the BMS for.

The ESC will take care of over-discharge shutdown, assuming you're using an ESC that does that, like VESC, and that it's been set up with the correct voltages in the setup.
```

---
## \#9 Posted by: TheFluffiest Posted at: 2018-10-16T15:23:53.600Z Reads: 60

```
Do you think the bms is fried after being wired the way it was?
```

---
## \#10 Posted by: tux-scooby Posted at: 2018-11-13T10:09:16.868Z Reads: 54

```
Hi, since this topic is already opened I also have similar question. Can this diagram also be used to bypass the discharge on BMS? (cannot find the origin/source of this picture but it is from here)

![Wiring%20V4%20(1)|690x388](upload://3fGurOAV1CHtNPOpwh4ZXLCTyOj.jpg)
```

---
## \#11 Posted by: Andy87 Posted at: 2018-11-13T10:46:49.598Z Reads: 50

```
yes this diagram is for a discharge bms
```

---
