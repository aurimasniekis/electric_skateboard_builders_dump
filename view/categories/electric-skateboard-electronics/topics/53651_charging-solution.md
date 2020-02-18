# Charging Solution

### Replies: 11 Views: 684

## \#1 Posted by: fredrikinn Posted at: 2018-04-27T12:38:56.434Z Reads: 152

```
Can anyone tell me if this will work or not? Looked around and it looks like this or BMS is what most people do.

![setupf|690x388](upload://tPUEPsOzMMLpbHAagiHNtDtROxO.png)

if i was going to use a bms instead, Whould i need new batterys?
```

---
## \#2 Posted by: E1Allen Posted at: 2018-04-27T12:47:13.310Z Reads: 142

```
Your current wiring diagram has you wired in parallel.  3s won't make for a fast board.  You can run a BMS with lipos.  Do a little reading, lots of good info here.  Check out some build logs and the beginners guide.
```

---
## \#3 Posted by: MannyM0E Posted at: 2018-04-27T14:56:47.500Z Reads: 109

```
I've done something similar to this with (3) 3s lipo connected in series and it worked out perfectly fine without a BMS.
```

---
## \#4 Posted by: fredrikinn Posted at: 2018-04-27T15:33:42.061Z Reads: 91

```
Cool do you have a picture?
```

---
## \#5 Posted by: b264 Posted at: 2018-04-27T15:39:37.135Z Reads: 85

```
Three 3S in series would work even better with a small BMS.
```

---
## \#6 Posted by: JamesNothing Posted at: 2018-04-27T15:57:13.526Z Reads: 76

```
I have the exact same setup on my board. 
make a 6s from 2 3s: lipo1 red to vest black to red of lipo2, lipo2's black to vesc.
then you peel (before the xt90 or switch on the side of the battery) and solder two wires corresponding to red of lipo1 and black on lipo2 and put an xt60 or 90 on it for charging.
it's better to have a male connector as a charging port, since it's more unlikely to short out.
then you take a 2 3s to 6s adapter for the balancing cables and connect it to your 2 3s, being careful to connect lips 1(the one with red cable that goes to the switch) to the 3s connector with the red cable in it and the lipo2 (black-negative) to the other lead.
make sure to protect your charging ports from shorting out because if you but them before the switch they're always live.
sorry if my English is not perfect, I'll be more than happy to explain a little better if you can't understand something :slight_smile:
```

---
## \#7 Posted by: fredrikinn Posted at: 2018-04-27T16:45:34.167Z Reads: 63

```
Like this? Just with the balance charger pins aswell 

![image|230x500](upload://yu4YVbsvBU8kGLIJBl3060pSGKH.jpg)
```

---
## \#8 Posted by: JamesNothing Posted at: 2018-04-27T17:00:34.460Z Reads: 57

```
exactly like that.
take care of the order of the cells when connecting the balance leads.
I don't remember why it's important, but someone told me to do so.
lipo 1 is the one with the positive lead going to the vesc and is the one that has it's balance leads connected to the adapter where it has the red lead. if your adapter has two red leads you should cut off the middle red one (if I remember correctly, but I didn't have to do this as my adapter didn't have the second red lead).
there was a discussion on this already on the forums, but I can't find it.
```

---
## \#9 Posted by: fredrikinn Posted at: 2018-04-27T18:53:11.147Z Reads: 50

```
So like pic 1 and NOT like pic 2? Just so i dont **** up

Pic 1
![setup1|690x388](upload://59PCvASqV5SQJyRKBTfkMvaYsc4.png)

Pic 2
![setup2|690x388](upload://liF5DxhGk6NcY35cdsfWOz0be1L.png)
```

---
## \#10 Posted by: JamesNothing Posted at: 2018-04-27T19:25:46.002Z Reads: 39

```
![Schizzo|690x460](upload://eUQ3cdZSRoJJEytc8ZPqMtowYlB.png)

like this. You could have an adapter for balancing that has a red and a black leads on the same pin. cut the red one and connect the positive side battery (lipo1) on the side of the adapter that has the uncut red wire.
if it does not have the red/black on the same pin (the one in the middle) don't cut anything and connect the 3s lead of lipo1 to the red wired connector
```

---
## \#11 Posted by: MannyM0E Posted at: 2018-04-28T04:20:05.308Z Reads: 26

```
Here's a thread where I found out how to do this.
Continuing the discussion from [How do you charge your longboard?](https://www.electric-skateboard.builders/t/how-do-you-charge-your-longboard/21561/51):
 @yaca was the person that helped me out. 
@b264 you right, but why you think it's better ? Eventually I ended up with a cheap BMS for charging so I don't do this anymore ?
```

---
