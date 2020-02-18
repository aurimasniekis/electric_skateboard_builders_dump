# Question battery cut off

### Replies: 11 Views: 524

## \#1 Posted by: Devilmycry Posted at: 2018-03-02T21:59:05.269Z Reads: 83

```
I just want to know if my battery cut off is go 
My battery is 12s7p 30q cell my start cut off is 40.8v and end 39,60v 
It is ok
```

---
## \#2 Posted by: pat.speed Posted at: 2018-03-02T22:20:48.820Z Reads: 79

```
You can go much lower than that, 36v start and 33.6 end
```

---
## \#3 Posted by: Hummie Posted at: 2018-03-02T22:24:06.878Z Reads: 77

```
wow 7p.  maybe keep your cutoff high since you have so many watthours and will be very unlikely to run out of juice while ridding and then the cells will last way longer.  drop the full charge voltage too
```

---
## \#4 Posted by: myreala Posted at: 2018-03-02T22:24:56.128Z Reads: 73

```
I have mine at 35 start and 33 end. But I also have a discharge BMS.
```

---
## \#5 Posted by: Namasaki Posted at: 2018-03-02T22:49:14.751Z Reads: 63

```
Here is one of the advantages of Li-ion cells.
You can run them down to 2.8v no problem.
Yes, they theoretically can go down to 2.5v but being a little conservative is always good.

**NOTE**
I would not run them down to 2.8v unless discharging through a bms which is monitoring individual cell groups.
Just my opinion...
```

---
## \#6 Posted by: Devilmycry Posted at: 2018-03-02T23:05:14.082Z Reads: 54

```
This is my bms 
![image|319x500](upload://u4oPMtnhahoRMlOsksSWPWk9dMW.jpeg)![image|651x500](upload://dIlqZvuT2vRkpSqJ1gs3jZTXmaM.jpeg)
```

---
## \#7 Posted by: Devilmycry Posted at: 2018-03-02T23:06:17.370Z Reads: 51

```
What set up I should do?
Thank you
```

---
## \#8 Posted by: Namasaki Posted at: 2018-03-02T23:18:39.113Z Reads: 47

```
You’ll be fine with that bms. 
Just wire it according to the diagram and you will have protection during charge and discharge. 
The bms over discharge protection is 2.9v and you’ll want to set the Vesc start higher to avoid triggering the bms protection. The bms protection is your final fail safe and is important especially on a welded pack. 
I would set the Vesc low voltage start at 3.0v or 36v total. This will simply reduce power output when your battery drops to 36v. 
You could go lower if the bms went lower. 
It’s better if the bms protection doesn’t kick in because you’ll have to disconnect the battery to reset the bms. 
Unless you use a Bestech bms with built in E-switch. Then you just cycle the on/off switch to reset.
```

---
## \#9 Posted by: Devilmycry Posted at: 2018-03-02T23:21:52.394Z Reads: 47

```
What do you this I will make my battery cut off start at 37 and end at 36 
Is good
```

---
## \#10 Posted by: Namasaki Posted at: 2018-03-02T23:25:26.146Z Reads: 45

```
I wouldn’t start at 37v
36v start is good 
And 35v end
That way you won’t trip the bms protection unless something goes wrong with your battery like broken weld joints from bumps and vibration. This can be a problem with welded packs
If some of the cells break loose and disconnect within a cell group, it will cause that cell group to discharge faster than the rest of the pack
Since the bms monitors each cell group, it will shut the system down before the cells in that group are damaged.
```

---
## \#11 Posted by: Devilmycry Posted at: 2018-03-02T23:28:20.684Z Reads: 44

```
Ok thank you I will do like this
```

---
