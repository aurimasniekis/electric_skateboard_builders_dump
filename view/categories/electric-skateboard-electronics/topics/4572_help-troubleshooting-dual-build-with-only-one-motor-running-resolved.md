# Help! Troubleshooting Dual Build With Only One Motor Running (Resolved)

### Replies: 7 Views: 828

## \#1 Posted by: AbrownMN Posted at: 2016-06-11T21:10:25.566Z Reads: 81

```
Hey there, I could use some help from yall..finally setting up my board and I am having an issue at the very last step. I had both motors running fine the entire time on the bench and even kept testing as I put the enclosure to the board. Finally got everything situated and one of the cables pulled right out of the CAN BUS connection when I was wiggling some shit around

No big deal, stuck it back it, hot glued it, tested it, and it worked fine. Then, I got everything screwed on tight and now only one motor will run! The master motor runs fine, but no signal seems to be getting to the other motor for some reason. Rechecked the CANBUS cable to the best of my ability. Took it back out, re-situated it and still nothing seems to work. I plugged master VESC into the slave motor and that still runs fine. Is the only ( most likely) possibility the can bus connection? No idea why it isn't working still. Is there a better way to "rebuild " it like popping out the little metal connector completely and re wrapping the wire before I stick it back in? Is there any other work around, troubleshooting to do here? Really want to finally get this thing running right after months of waiting I am about to break something...

 Any ideas? Thanks!
```

---
## \#2 Posted by: AbrownMN Posted at: 2016-06-11T21:24:07.886Z Reads: 80

```
Great...Just ripped the other two ends out of the cable too, barely even pulled on them.. >_> 

Is there a better way to link them together?
```

---
## \#3 Posted by: cmatson Posted at: 2016-06-11T21:31:37.310Z Reads: 73

```
You can just link two VESCs by splitting the PPM wire to each individually.

You'd have to run each vesc as a single (so no master or slave) but it wouldn't affect the performance. This is the way you'd link all other escs before the vesc was avaliable.
```

---
## \#4 Posted by: AbrownMN Posted at: 2016-06-11T21:50:31.193Z Reads: 65

```
Got any pictures of this I can work with? Do I need to solder them? I had it running perfect...damn this shitty connection..

Edit: Ended up pulling off the connectors, slipping the wires over the pins and caking in the hot glue to keep them in place as a temporary/troubleshooting fix. Not the best route, but at least I know the issue was just with the CANBUS connectors..Time for her maiden voyage!
```

---
## \#5 Posted by: flatsp0t Posted at: 2016-06-12T20:15:35.416Z Reads: 37

```
Just solder the wires directly to the connectors, it will get berfect connection and there is no risk it gets loose due to vibration.
```

---
## \#6 Posted by: AbrownMN Posted at: 2016-06-12T21:44:58.949Z Reads: 30

```
Yeah, eventually that will be the plan. Makes them a bit tougher to service individually, but I prefer the stable connection.
```

---
## \#7 Posted by: flatsp0t Posted at: 2016-06-13T06:09:15.897Z Reads: 28

```
These two solder joints are desoldered in a minute. ^^
```

---
