# LiPo cell dead?

### Replies: 9 Views: 677

## \#1 Posted by: florensvb Posted at: 2017-09-20T11:28:00.741Z Reads: 64

```
Hey guys,

as @notepad mentioned in [this thread](http://www.electric-skateboard.builders/t/battery-problems-help-needed/33491/2?u=florensvb), it seems that one of my lipo cells are dead. I am running 2 x 4S 8000mAh and just went to the store to get a multimeter and did some measuring:

1) **0.32V**
2) 4.14V
3) 4.18V
4) 4.17V

5) 4.15V
6) 4.15V
7) 4.16V
8) **4.09V** 

So obviously the 1st cell is bananas. But what about number 8, is it ok?

Is it dangerous to have a dead cell -- is there a fire hazard?! 

Also I need to know my options from here ... Whats the best solution? Get a new 4S pack? Take the dead cell out and make it 7S? ... other ideas? 

I have the [Skyrc e8 charger](http://www.skyrc.com/index.php?route=product/product&product_id=214) and am wondering how to wire the balance lead when one cell is missing .. just leave out the 8th balance plug?

Thanks a bunch guys
```

---
## \#2 Posted by: bartroosen12 Posted at: 2017-09-20T11:37:13.269Z Reads: 60

```
I should disconnect that dead cell and just cut the balance wire for that cell.
The cell number 8 is still pretty fine
```

---
## \#3 Posted by: florensvb Posted at: 2017-09-20T11:40:19.119Z Reads: 59

```
Ok few questions on that:

Disconnect? Id still have to open up the lipo pack to do that right? 

Also, since i do not have a balance board- how do i "convert" the 8S to 7S leads on my charger?

Thank you @bartroosen12
```

---
## \#4 Posted by: bartroosen12 Posted at: 2017-09-20T12:12:31.738Z Reads: 52

```
Yeah you have to open the battery but be carefull.
Unsolder the bad lipo and unsolder the balance lead which goed to that cell.
Just cut the wire from your balance wires and it will be no problem if you charge with a balance charger I think or you can just cut the connector to make it 3S <img src="/uploads/db1493/original/3X/c/d/cdbef04113307727647234bc268f4145926dd061.jpg" width="666" height="500">
```

---
## \#5 Posted by: Vieo Posted at: 2017-09-20T12:18:47.122Z Reads: 48

```
You could just buy a new 4S battery
```

---
## \#6 Posted by: wafflejock Posted at: 2017-09-20T13:20:07.780Z Reads: 41

```
@florensvb the one with the dead cell I would just toss.  If you can replace both it would be best to do that but the one with the .06V difference shouldn't be a major problem.  I would keep a close eye on it in terms of how it charges/discharges over the next week or two of charging to make sure it isn't drifting further off because you just don't want it to go over the cliff (basically if all the other cells are holding say 3.7V and it's down at 2.8V then it will end up like cell 1 in your first battery).  If it starts to recover or at least doesn't drift drastically far down you can probably safely keep using it.
```

---
## \#7 Posted by: florensvb Posted at: 2017-09-20T13:22:04.397Z Reads: 41

```
[quote="wafflejock, post:6, topic:33569"]
the one with the dead cell I would just toss
[/quote]

Hey there thanks for your answer. I think i am going to attempt removing the dead cell from the 1st pack because otherwise I need to spend another 50 euros on a new 4S pack and id have to wait for it to get here as well...
```

---
## \#8 Posted by: wafflejock Posted at: 2017-09-20T13:26:19.638Z Reads: 37

```
I did try remove 1 cell from a 6S to bring it down to a 5S with a pack I killed, but would advise disconnecting things and not trying to physically take the cell out of the pack (easy to mess up the foil around the cells trying to separate them from the adhesive/tape).  Regarding the JST you may need to shuffle some wires around to avoid moving too many connections on the battery tabs themselves... the battery tabs are aluminum (or at least can be soldered with aluminum solder/flux) regular solder won't work on them, you can desolder things or remelt the existing solder but if you need to add some you'll need to buy special solder for it to stick at all (basically do things plug side).  Unfortunately since it's the 1st cell ( I imagine you mean the one next to the ground part of the balance plug ) you'll have to shift things around since it expects to start with cell 1 from the black wire, and go from there.
```

---
## \#9 Posted by: florensvb Posted at: 2017-09-22T17:23:56.014Z Reads: 26

```
Did it! Have a working 7S now. Thanks for the help guys
```

---
