# Anti-spark switch fuse question

### Replies: 14 Views: 1128

## \#1 Posted by: Guacamoleface Posted at: 2017-01-26T22:55:26.632Z Reads: 194

```
Hey so I've been looking around abit on antispark switches, mostly from eu shops. Noticed that many are fused at 40A.

Wouldnt that be to low for a board wheres battery and motor can pull up to 80A max?
```

---
## \#2 Posted by: evoheyax Posted at: 2017-01-26T23:01:37.013Z Reads: 196

```
Yes, you can pull well over 40 amps. But you also need to determine this number based on you. Hills, weight, gearing, motor kv, and especially voltage, affect how many amps you'll pull from your battery. Some people never pull more than 40 amps. I know I pull around 120 amps at times running 12s. You have to determine the max amps you'll pull biased on your setup, and you have to figure out what you'll pull. It's different for everyone.
```

---
## \#4 Posted by: Guacamoleface Posted at: 2017-01-28T00:07:13.166Z Reads: 160

```
Alright, not really certain on how the antispark is wired but if the board pulls 50A(example), then 50A will go through the Vedder antispark switch and pop the fuse? Or am I thinking wrong?
```

---
## \#5 Posted by: marcoluz Posted at: 2017-03-18T16:14:22.673Z Reads: 128

```
i have the same question.
```

---
## \#6 Posted by: Guacamoleface Posted at: 2017-03-18T20:07:16.694Z Reads: 120

```
Im just gonna get a switch that is fused for my max amps my battery can pull. So in my case its 80Amps. So to be safe I'll get one with 80A or more.
```

---
## \#7 Posted by: devguy Posted at: 2018-11-17T04:20:15.196Z Reads: 53

```
You have to get a fuse that will protect your ESC from getting fried as well as your motor coils from melting. Determine the one with the lower amp rating and get a fuse for this level.

If you have to pick between a fuse that is under-rated vs over-rated with what you really need, go with the under-rated and see how it works out. Worst case you blow the fuse and everything lives for another day. If you need to go over then you're taking a risk of your ESC or Motor getting damaged.

Also for example, if you battery can only push 40A and your ECS or Motor can handle 80A or more, there is no point in using a fuse.
```

---
## \#8 Posted by: mmaner Posted at: 2018-11-17T04:26:14.590Z Reads: 46

```
Uhhhh, no.

Fuses blow, board stop, street face. That's why most people don't run then. 

Oh, and this topic is 2 years old 😀.
```

---
## \#9 Posted by: devguy Posted at: 2018-11-17T04:29:44.856Z Reads: 43

```
Exactly how would the motor come to a dead halt with no power? At worst the skate would coast and slow down. Also the topic is 2 years old for you, not everyone new to this ;-)
```

---
## \#10 Posted by: mmaner Posted at: 2018-11-17T04:39:02.258Z Reads: 41

```
At 30 mph, the loss of forward momentum might as well be a stop...your still gonna keep going while the board is behind you.
```

---
## \#11 Posted by: Skunk Posted at: 2018-11-17T04:44:37.653Z Reads: 43

```
Who's this @mmaner guy?   How would you even know dude?  Who are you to give advice?
```

---
## \#12 Posted by: Wraith Posted at: 2018-11-17T04:45:03.233Z Reads: 43

```
you probably wouldn't have the time to react to a sudden change in speed which is enough to cause a loss in balance
```

---
## \#13 Posted by: devguy Posted at: 2018-11-17T04:46:32.014Z Reads: 42

```
Well if you blow your motor or ECS you going to experience the same effects. imho I rather protect my investment, to each their own I guess.
```

---
## \#14 Posted by: Wraith Posted at: 2018-11-17T04:48:15.587Z Reads: 43

```
it would come down to personal safety during the ride or keeping the hardware intact during a blowout which I think is why other builders would prefer to lose the vesc than break some bones or lose some skin.

But yes to each their own. just wanted to give some insight as to what the trade offs would be in that kind of a situation
```

---
## \#15 Posted by: devguy Posted at: 2018-11-17T04:51:26.071Z Reads: 42

```
So if you blow your ECS how is that going to save you from breaking bones? now you have 2 problems. 

I guess don't pick a fuse that is too under-rated that it will easily blow, you want to pick a safe level to the blowing point of your system.
```

---
