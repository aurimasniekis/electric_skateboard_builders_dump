# Bluetooth BMS 10s 2p *Setup help*

### Replies: 8 Views: 345

## \#1 Posted by: Travo Posted at: 2018-10-22T22:46:33.415Z Reads: 81

```
I've connected the BMS wires on to the battery and was wondering if this looks correct. The wires go 1,3,5,7,9,11 and 2,4,6,8,10 
Side note, I got the battery welded but I definitely need more nickel on there or something. I don't have a spot welder and was wondering if I could just lay down some wire via solder? Thoughts?![15402483227976650597991563955305|375x500](upload://6N55b3Ne8700lLvlUthF285aHhV.jpeg)
```

---
## \#2 Posted by: rojitor Posted at: 2018-10-23T08:33:45.698Z Reads: 66

```
Solder copper braids between the cells. You Will not damage them. The balance wires look correct.
```

---
## \#3 Posted by: rojitor Posted at: 2018-10-23T09:10:47.934Z Reads: 59

```
i have a pc around now. 
![solder|375x500](upload://rlAX7VcbjCXjGGHLEYMNSuZA6xN.jpeg) 
solder like that. copper braids between cells for series and a small piece on main positive and negative. Then you solder on that small braid the bms wires.
That job is quite poor, very thin nickel and no gaskets. If you ride fast the heat will be a problem here:
![weak|375x500](upload://qltQyNQKsBEgKycxxP6GYJCmJCK.jpeg) 
Try to put pieces of paper under the nickel at those spots, it's not as good as fish paper rings but better than nothing. 
Also if you know someone close to you with a spot welder it's not too late to fix it.
```

---
## \#4 Posted by: Travo Posted at: 2018-10-23T13:34:36.987Z Reads: 46

```
Thanks for the response, I have some of the sticker things for the cell. I'll attach the small circle guys in between the nickel.  I think I'll get some fatter nickel and find someone to weld it on top of the existing welds. If you know a link to the wire that I could solder on that'd be great as I keep getting results for desolder copper braids. The reason I asked if the BMS was wired correctly is because I was getting that weird electronic burning smell. I unplugged it as to not burn anything but no smoke or burn marks where anywhere on the ports or the PCB board. Is the smell a result of the board being used for the first time? I felt heat at the connection so I must have done something wrong? Just lemme know
```

---
## \#5 Posted by: rojitor Posted at: 2018-10-23T13:58:50.849Z Reads: 42

```
Smell? No good. Did you check voltage? You must check all the pins. First should read 3.5v second 7v....and so on. Also did you plug It to the bms without -b soldered? You must not plug that wire in that case
```

---
## \#6 Posted by: Travo Posted at: 2018-10-23T14:38:09.055Z Reads: 42

```
Oh shoot that might be the problem. So this is what it should look like (the x just means there's no connection there)![sketch-1540305430802|281x500](upload://5VTH0WvSluGWBw3bG6BhILGShsz.jpeg)
```

---
## \#7 Posted by: rojitor Posted at: 2018-10-23T17:57:32.198Z Reads: 33

```
Unless manufacturer said otherwise -b must be connected before you plug balance. It's not mandatory but you should solder charge and discharge too. Never ever plug that wire without checking voltage first. Regardless the colors of the wires they do not mean the same depending on the model. Mostly first is main negative and last is main positive but that's not always like that. Some lack the negative wire or go backwards... Check diagram first.
Now you should take a look at the bms. Look if there's anything burnt or damaged.
```

---
## \#8 Posted by: dareno Posted at: 2018-10-24T04:21:16.752Z Reads: 26

```
There's a lot you could do to improve this pack tbh.  @mmaner can we move this to the rate my battery thread?
```

---
