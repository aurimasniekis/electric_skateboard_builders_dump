# I’m Going from 10s5p to 12s5p. What VESC settings need changed

### Replies: 14 Views: 372

## \#1 Posted by: ualsteve94 Posted at: 2019-06-04T05:54:24.128Z Reads: 132

```
I’ve got a stock Lacroix with two Focboxes.   The Original battery was a 10s5p, Sanyo 20700B.  My new pack is a 12s5p , same Sanyo 20700B.  What VESC settings will I need to change for the 12s battery?    Thanks for any HELP.
```

---
## \#2 Posted by: YungDaff Posted at: 2019-06-04T12:11:10.154Z Reads: 111

```
You need to change the voltage limits, so that it works for a 12 cell battery. The discharge is the same as both batteries are in an a 5P config. 

Just put in the battery calculator in the vesc tool that you have a 12 cell lithium ion battery and it will calculate the volts for you, just dont forget to hit apply.
```

---
## \#3 Posted by: ualsteve94 Posted at: 2019-06-04T17:26:45.388Z Reads: 91

```
So just the cutoff start and cutoff end ??   I’ll be using the BLDC tool.   
Thanks for the help YungDaff
```

---
## \#4 Posted by: YungDaff Posted at: 2019-06-04T17:29:24.251Z Reads: 88

```
I do not have any experience in the BLDC tool, I use the vesc tool. But the setting should be the same. I would put 40.8 at cutoff start and 38.4 at cutoff end.
```

---
## \#5 Posted by: ualsteve94 Posted at: 2019-06-04T17:42:52.071Z Reads: 85

```
Thank you, I’ll do that
```

---
## \#6 Posted by: epss4 Posted at: 2019-06-04T18:19:08.634Z Reads: 78

```
38.4 cutoff end is very high for sanyo cell , i have 12s5p with sanyo and my cutoff end is 35V
```

---
## \#7 Posted by: YungDaff Posted at: 2019-06-04T18:30:19.889Z Reads: 73

```
Might be, I for some reason assumed he was using 30Q. You might want to try other values when using 20700 and 21700 cells.
```

---
## \#8 Posted by: ualsteve94 Posted at: 2019-06-04T23:01:53.629Z Reads: 61

```
Roger that gentlemen.   I Was gonna go with 2.9 (34.8) cutoff end and 3.1 (37.2) cutoff start.    Just wondering if there where any other values else where that needed changing.   

Thanks again fellas.
```

---
## \#9 Posted by: Saturn_Corp Posted at: 2019-06-04T23:21:25.021Z Reads: 55

```
hmmmm, I just realized all this time I had cutoff start at 50.4 volts thinking that's what it is supposed to be set at for full charge, and my cutoff end at where I wanted it to cutoff at. 

What changes between cutoff start and cutoff end voltages?
```

---
## \#10 Posted by: Sn4pz Posted at: 2019-06-04T23:32:21.374Z Reads: 56

```
Cut off start = limp mode / lessened powah

Cut off end = no power

I think that's what you're asking? 🤔
```

---
## \#11 Posted by: Saturn_Corp Posted at: 2019-06-04T23:35:00.301Z Reads: 55

```
Yah I guess. Would it be reducing my power at slightly below full charge? I don't really notice anything big but I do feel sag <75 percent on 30q's 12s4p.

Might have to change it and see if I notice anything.
```

---
## \#12 Posted by: Sn4pz Posted at: 2019-06-05T00:11:03.271Z Reads: 49

```
That's likely causing the sag you feel 

I wouldn't go to 35v for the hardcutoff, thats too low. For my 12s7p 30q  I think I'll set the soft cutoff to 39v and hard cutoff to 37v

It obviously depends on the cell chemistry and how you want to treat the pack though. I would say 35v is fine for 21700 cells due to their increased 'durability'
```

---
## \#13 Posted by: meesie Posted at: 2019-06-05T15:27:59.686Z Reads: 31

```
set your max ERPM to 60k. higher voltage means more RPM's from your motor.

also lower your motor max by the way. increased voltage and same amperage still means higher wattage. but that's just a personal preference. just to get used to it
```

---
## \#14 Posted by: ualsteve94 Posted at: 2019-06-05T21:29:23.285Z Reads: 29

```
So I just received the new 12s battery.   I’ll be getting it hooked up to the BLDC tool here in the next hour.   I see he sent me back a nano-X controller and now has the nano-x receiver installed in the build.   I actually asked for nano-v2 , not the-x, since I already have a couple v2  Remotes.  QUESTION,  will my nano-v2 remotes work with this receiver the same way that all nano-v2 remotes work on any nano-v2 receiver?   Or did he just tie me down to this nano-x?   

Thanks
```

---
