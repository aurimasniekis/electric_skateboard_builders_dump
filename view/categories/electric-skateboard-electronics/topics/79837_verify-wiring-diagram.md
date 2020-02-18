# Verify Wiring Diagram

### Replies: 20 Views: 311

## \#1 Posted by: Customesk8 Posted at: 2019-01-04T06:24:24.610Z Reads: 57

```
Can someone please confirm this is not completely wrong or any reason it would be less efficient? 

Feedback? Better way of doing it? 


![image|395x418](upload://ym1vN7JVPW4RrVMWktgt6bibBQe.png)
```

---
## \#2 Posted by: amazingdave Posted at: 2019-01-04T06:41:06.359Z Reads: 50

```
Your voltage meter will be always on... move the position of the positive connection to the vesc side of the loopkey or have a switch in line with the meter...
```

---
## \#3 Posted by: amazingdave Posted at: 2019-01-04T06:46:09.163Z Reads: 47

```
Also note that the loop key must be in to charge with this setup, meaning the vesc will be on for charging. Better to join the positive charge lead directly to the battery positive. Oh and definitely put a fuse in the positive charge lead. 

https://www.electric-skateboard.builders/t/that-was-a-close-call/79409
```

---
## \#4 Posted by: Customesk8 Posted at: 2019-01-04T06:46:25.017Z Reads: 41

```
thanks for the response, could i just solder all 3  together like this and put a 4mm bullet connector on it? 

![image|397x432](upload://kb7UwaKWP1kjdENlmTB5MAWWX6u.png)
```

---
## \#5 Posted by: Customesk8 Posted at: 2019-01-04T06:49:41.566Z Reads: 38

```
ah so something like this? 

![image|397x432](upload://9rM6gE2CDqnJdolw88Kn0Sc7oav.png) 

i am trying to figure out how to do this without cutting into the existing battery connections (they are 4mm bullet connectors - is there no other way without meaning it will be all live whilst charging as you said
```

---
## \#6 Posted by: amazingdave Posted at: 2019-01-04T06:50:55.201Z Reads: 34

```
You could add the charge lead to the battery side of the xt90 loop key connector?
```

---
## \#7 Posted by: Customesk8 Posted at: 2019-01-04T06:52:47.677Z Reads: 36

```
![image|397x432](upload://7RL0aLDTjcAsuO9feaQcsXyP0KR.png) 

Like this? I already soldered the XT-90 so was kinda avoiding that as well but that might be the best bet.
```

---
## \#8 Posted by: amazingdave Posted at: 2019-01-04T06:54:14.936Z Reads: 33

```
Nope. Charge lead to battery side of loop key.
```

---
## \#9 Posted by: Customesk8 Posted at: 2019-01-04T06:55:27.197Z Reads: 33

```
doesn't that present the same issue as the original idea? it'd have to be plugged in to complete the circuit and charge?

Edit: I think I just realized why that is not the case :smile:
```

---
## \#10 Posted by: Customesk8 Posted at: 2019-01-04T06:59:52.567Z Reads: 34

```
I was getting the voltage meter confused with the charging port so one last time is this the winning diagram? 

![image|397x432](upload://14oi5IXuG0JAbekq6NEm9yDERdl.png)
```

---
## \#11 Posted by: amazingdave Posted at: 2019-01-04T07:01:29.656Z Reads: 33

```
That’s it. Don’t forget the fuse! ![image|397x432](upload://d4H8txhNWsqpdYi6DyitFQwPadf.jpeg)
```

---
## \#12 Posted by: Customesk8 Posted at: 2019-01-04T07:03:44.255Z Reads: 31

```
Thanks heaps man!

Just quickly where I've circled blue it's fine to put a bullet connector to connect directly to the battery?

![image|560x437](upload://6Luqk7Mzbw1Lm7lMcBnZL0XkGgy.png)
```

---
## \#13 Posted by: amazingdave Posted at: 2019-01-04T07:05:55.106Z Reads: 30

```
Yes.  If you want to lay out all your parts and take a photo for reassurance before you solder then go for it.
```

---
## \#14 Posted by: Customesk8 Posted at: 2019-01-04T07:17:26.453Z Reads: 30

```
Unfortunately I don't have connectors yet so I cant solder yet but just making sure I know exactly what to do when I can. 

This might be hard to see 

![image|690x335](upload://xAZCje3ARhaQZX1HBRXQ3hOZsen.jpeg)
```

---
## \#15 Posted by: amazingdave Posted at: 2019-01-04T07:19:10.893Z Reads: 28

```
Yeah that is hard to see! Just take your time, and double check before connecting the batteries.
```

---
## \#16 Posted by: Customesk8 Posted at: 2019-01-04T07:20:02.171Z Reads: 28

```
yeah it's pretty chaotic because the wires are all long and i dont want to cut them yet, but with the diagram i think i've got it
```

---
## \#17 Posted by: Customesk8 Posted at: 2019-01-04T09:17:56.912Z Reads: 29

```
I've got too much time on my hands right now....

![image|397x432](upload://5fKDuOpXSmaFkeEZaSZoulVohR.png)
```

---
## \#18 Posted by: amazingdave Posted at: 2019-01-04T09:48:09.842Z Reads: 24

```
Looks good to me. How are you connecting the balance plugs from your lipos to your bms? Remember if you’re cutting them to solder that you are live working... lipo shorts get exiting very quickly!
```

---
## \#19 Posted by: Customesk8 Posted at: 2019-01-04T09:54:12.321Z Reads: 23

```
I'm currently drafting that up. The bms came with long wires it looks like i can just put JST connections on that and plug directly into battery ones.
```

---
## \#20 Posted by: Customesk8 Posted at: 2019-01-04T10:32:33.706Z Reads: 21

```
![image|431x500](upload://8fdZ92ObeAWNuzKCsOLM05nHnnt.png)         

Looks like chaos - i think i understand it though
```

---
