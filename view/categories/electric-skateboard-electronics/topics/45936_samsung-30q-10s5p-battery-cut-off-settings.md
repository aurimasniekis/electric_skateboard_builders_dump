# Samsung 30Q 10S5P Battery Cut Off settings

### Replies: 6 Views: 1226

## \#1 Posted by: goldrabe Posted at: 2018-02-09T05:35:00.155Z Reads: 179

```
I read that a safe value for cut off settings is start 3.4V end 3.2V multiplied by 10S means start 34V end 32V. That is also what the wizard sets in the Vesc Tool. However in a different post i read that you can safely go down to cut off start 30V end 28V to get the most out of your battery.
Can i set it to that?
Any advice will be appreciated.
```

---
## \#2 Posted by: E1Allen Posted at: 2018-02-09T05:45:36.398Z Reads: 179

```
I think most would set their cutoffs higher.  The discharge curve on a battery drops fast at the bottom.
```

---
## \#3 Posted by: MrHappy Posted at: 2018-02-09T05:46:03.519Z Reads: 172

```
This is all subjective to the person, but i do 33v start and a 30v end for my 30qs
```

---
## \#4 Posted by: bimmer Posted at: 2018-02-09T05:58:06.415Z Reads: 162

```
I tell people 32v end on the batteries I sell.
```

---
## \#5 Posted by: thisguyhere Posted at: 2018-02-09T05:58:26.895Z Reads: 155

```
keep per cell voltage above 2.8v and under 4.15v for longevity.

and give yourself plenty of space between soft and hard cutoff to avoid shutdowns.

on a 12s build i had the soft cutoff start at 36v (3v) and hard cutoff at 34v (2.83v).  at end of charge, took it up a hill under hard acceleration and the voltage sag caused total voltage to dip below hard cutoff and it shut down on me.  right in the middle of hard acceleration.  keeping a wider range will allow the vesc to throttle current draw and prevent shutdowns.
```

---
## \#6 Posted by: ZackoryCramer Posted at: 2018-02-09T06:26:34.815Z Reads: 144

```
I cut off my cells at 3.3v :ok_hand: Gets a bit annoying when you are going high speed on low capacity. :no_mouth:
```

---
