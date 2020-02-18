# Eboard braking too hard then changes after loss of 3volts

### Replies: 8 Views: 298

## \#1 Posted by: Danny414 Posted at: 2018-04-24T17:10:53.237Z Reads: 78

```
Hello!

I have a diy eboard with 2 focboxs and a custom 10s5p and in the bldc settings I have it set to not brake to hard but I’m noticing that when it is fully charged at 42volts to about 40volts braking is harder then around 39volts it’s not as hard

Thanks!

![image|666x500](upload://fdrcNuWyCFsSufMycqPgRdaoRlT.jpeg)
```

---
## \#2 Posted by: RedEagle Posted at: 2018-04-24T17:22:52.933Z Reads: 69

```
This is normal. As your voltage drops you will also lose top speed. Braking at lower voltage is weaker simply because your battery is nearly empty. 
Less volts = less power.
```

---
## \#3 Posted by: Danny414 Posted at: 2018-04-24T18:06:32.909Z Reads: 61

```
Yeah but the settings I have in the vesc are for not so hard of braking. Shouldn’t the vesc listen to my settings and not brake so hard?
```

---
## \#4 Posted by: Danny414 Posted at: 2018-04-24T20:38:43.391Z Reads: 52

```
I actually figured out what happened.. im using enertions nano-x and it accidentally changed to r-spec mode and increased everything.. is there a way to decrease aspects mode braking?
```

---
## \#5 Posted by: RedEagle Posted at: 2018-04-24T21:18:33.817Z Reads: 44

```
I'm not familiar with the enertion nano-x. Did you try braking in r-spec mode at full charge?
```

---
## \#6 Posted by: Danny414 Posted at: 2018-04-24T23:22:59.352Z Reads: 34

```
nope, kinda afraid too lol but I think it has something to do with the different modes.. because I did feel a difference when switching them
```

---
## \#7 Posted by: RedEagle Posted at: 2018-04-25T00:19:57.868Z Reads: 32

```
I think I know what happened here. The remote limits the ppm output at modes lower than r-spec mode. 

For example: 
Beginner mode, ppm max value 80%, max speed 30km/h
R-spec mode, ppm max value 100%, max speed 37km/h

Which means you set the remote up in beginner mode. Make sure the remote is in r-spec mode first, then redo the app setup in bldc tool. 

Are you using @Ackmaniac 's custom firmware? 
If so I would update to the new version. There was a bug that he fixed that is related to this.
```

---
## \#8 Posted by: Danny414 Posted at: 2018-04-25T00:21:26.975Z Reads: 34

```
ahh that makes sense.. I don't think so.. I ordered the focboxs direct from enertions website
```

---
