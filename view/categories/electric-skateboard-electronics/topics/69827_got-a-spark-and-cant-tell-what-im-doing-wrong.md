# Got a spark and can&rsquo;t tell what I&rsquo;m doing wrong

### Replies: 10 Views: 285

## \#1 Posted by: ShakeNBake7000 Posted at: 2018-10-02T10:07:01.037Z Reads: 69

```
Just tried to assemble my build after finishing soldering and when everything was connected and I turned the board on, I got a spark between the positive battery's balance cable and the series balance connector. I immediately disconnected it and made sure no part got fried, nothing was hot except for the BMS.

These are the electronics of the board:
![board|690x388](upload://uU8kX8DhKV66C9B4ZPCLcWUQ6uy.jpeg) 

I don't know much about electronics and what I do know is from building this board, one thing that seemed pretty weird is that the BMS gets warm (not very hot) whenever the balance cable is connected, not sure if that's normal or also some kind of problem.

Batteries are two 3s's in series to make a 6s, the BMS is a 6s BMS, so I don't see where the problem is.
Any help appreciated, I'm clueless.
Thanks
```

---
## \#2 Posted by: dareno Posted at: 2018-10-02T10:13:29.894Z Reads: 63

```
You have a balance wire crossed or shorted.  Check everything again.
```

---
## \#3 Posted by: ShakeNBake7000 Posted at: 2018-10-02T10:19:11.213Z Reads: 62

```
I can't remember how it was connected when it sparked but is this the right way to connect the balance and series connectors?
![50|690x388](upload://i6evbzGXvLIAR0FxjKi8JdgOfD8.jpeg)
```

---
## \#4 Posted by: Jumpman Posted at: 2018-10-02T10:27:57.848Z Reads: 61

```
While everything looks correct, it’s possible that the final balance connector into the bms is wired backwards.
```

---
## \#5 Posted by: ShakeNBake7000 Posted at: 2018-10-02T10:42:25.620Z Reads: 58

```
I think you're right, the cable can only go in on one side, and its the wrong side:
![52|281x500](upload://qLoRybylr979SAZ9nocRjTUksjZ.jpeg) 

When it's connected, the pins go into the port as they should but when I looked on the other side it seemed wrong:

![10|281x500](upload://ovllP3DA9Qjj62idCdd0xL4kZaZ.jpeg) 

For some reason, the negative on the BMS is on the side of the positive of the balance cable and when I checked the cable that came with the BMS it made sense:

![09|281x500](upload://gWfwfqa3qz8IRMvBacOUrFoPhiS.jpeg) 

The negative and the positive were swapped sides for some reason, and now I can't use the 3s to 6s balance adaptor.
The other side of the cable that came with the BMS is just open wires, I guess I can manually connect them one by one but that doesn't seem like a permanent solution, any ideas on what I should do?
Thanks for the help

Edit: Just got the idea of connecting the negative balance wire into the positive battery and connect the positive balance cable into the negative battery, my logic says it would work but I'm not sure.
Basically swapping these:
![58|690x372](upload://zdo5qV05twtd8bHl6mM9irpzVLw.jpeg)
```

---
## \#6 Posted by: Andy87 Posted at: 2018-10-02T11:22:11.553Z Reads: 49

```
take a needle to get the pins out of your 6s JST plug.
It´s a bit fiddly to get them out but should work.
Than swap the wires.
or cut the 3s to 6s adapter and solder them in the right order.
```

---
## \#7 Posted by: ShakeNBake7000 Posted at: 2018-10-02T11:29:23.168Z Reads: 44

```
Alright I'll try to take them out, Thanks for the help!
```

---
## \#8 Posted by: Newby Posted at: 2018-10-02T11:31:14.423Z Reads: 42

```
Tape the pins when you pull them out aswell so they don't knock together
```

---
## \#9 Posted by: ShakeNBake7000 Posted at: 2018-10-02T11:34:01.955Z Reads: 41

```
You mean tape them to make sure I keep them in the right order?
```

---
## \#10 Posted by: Andy87 Posted at: 2018-10-02T11:36:55.496Z Reads: 39

```
i think @Newby means that you don´t short anything,
but if you disconnect your 3s to 6s plug on both sides than it will
not happen.
```

---
