# New VESC Tool Help

### Replies: 6 Views: 198

## \#1 Posted by: MustardTiger Posted at: 2019-03-29T23:59:56.354Z Reads: 53

```
Just downloaded the new version of vesc tool and updated the firmware on both focboxes to 3.53 and now one of my motors will only work in FOC. When I change to BLDC I just get a high pitched whine and no movement. I’m running 12s and it’s my understanding that 12s and FOC is risky and I like to push my board to the limit.

The default values for the new tool seem off as well. 99 battery amps seems crazy!

Any help would be greatly appreciated thanks.
```

---
## \#2 Posted by: dareno Posted at: 2019-03-30T10:51:38.319Z Reads: 43

```
The tool has no default values.  You set the values according to your set up. Ignore the factory settings from whatever vesc you attach.  
If you want help then you need to first outline;
Battery type and config
Motors
Set up
Basically more information is necessary.
```

---
## \#3 Posted by: MustardTiger Posted at: 2019-03-30T22:12:02.471Z Reads: 30

```
I was making a video to demonstrate my problem and it just started working lol thanks anyways
```

---
## \#4 Posted by: MustardTiger Posted at: 2019-03-30T22:13:50.384Z Reads: 29

```
Under the rpm tab the tool has erpm at 100,000 should I lower this to 60,0000 like I did before?
```

---
## \#5 Posted by: dareno Posted at: 2019-03-30T22:32:28.945Z Reads: 26

```
Focbox are rated above the 60000 and yes technically to be safe its a good idea to lower the default value.  Again its difficult to assess any potential issues unless we know the complete set up you are running.
```

---
## \#6 Posted by: MustardTiger Posted at: 2019-03-31T02:33:39.461Z Reads: 18

```
![image|507x500](upload://n205kzbueLQD1AH8sgOAeJBREg4.jpeg) 
12s4p torqueboards battery
Dual 6380 170kv torqueboards motors
107mm wheels
16/36 12mm pulleys 

Motor: 80/-60
Battery: 45/-12
```

---
