# VESC Tool Current settings struggles

### Replies: 6 Views: 310

## \#1 Posted by: MuggaTheFirst Posted at: 2018-09-14T13:51:24.952Z Reads: 82

```
Hey guys, it might be a little stupid question, but I really didn't find the answer and I don't wanna burn my LiPos...

I'm using 2 Battery packs connected parallel. This parallel plug delivers the voltage for 2 VESCs.
I go to VESC Tool -> Motor Setting -> General -> Current -> Battery Current max and I set this to 25 Amps.
Does this mean, that each VESC can draw 25A so all together there will be a current of 50A? Or do both motors share this 25A so each motor just gets 12.5A

Same is with the battery current max regen: When I set this to 10 Amps, does each motor deliver 10 Amps so there will be 20 Amps all in all or do both motors together deliver this 10 Amps?
```

---
## \#2 Posted by: Andy87 Posted at: 2018-09-14T14:00:41.364Z Reads: 76

```
You set always just one vesc.
So all values single values.
For the overall current value you need to add them up.
```

---
## \#3 Posted by: ElectricCoast Posted at: 2018-09-15T09:41:38.608Z Reads: 61

```
I read that 4 times and the answer is confusing at least for me it is.  Can you elaborate?
```

---
## \#4 Posted by: Andy87 Posted at: 2018-09-15T09:44:28.287Z Reads: 59

```
Your vescs are in parallel connected to your battery.
Your battery can let’s say supply 80a
So as the vescs parallel you can set each vesc to max bat current 40a
Hope it’s more clear 😅 if no ask please
```

---
## \#5 Posted by: MuggaTheFirst Posted at: 2018-09-15T10:43:27.267Z Reads: 53

```
Thanks for your answer!

I were confused because of my following thoughts:
I have 2 vescs that communicate via CAN bus. I can set up a max motor current for each single motor, so I thought that "max bat current" would mean that both vescs commuicate via the CAN bus and therefore grant an overall current not bigger than the set value...

But well, now I know that I was wrong so thank you for that!
```

---
## \#6 Posted by: threebysix Posted at: 2018-09-16T00:19:51.201Z Reads: 39

```
Basically, motor min and max can be set for individual vescs (e.g. 60/-60 on each vescs), battery min and max will need to be divided by two because you have two vescs
```

---
