# Nano Remote Broken Throttle?

### Replies: 11 Views: 257

## \#1 Posted by: tarikalauddin Posted at: 2018-07-11T04:43:29.337Z Reads: 91

```
Hi everyone! About 2 days ago I finished my first build and everything was working flawlessly. However, when I went out yesterday, my remote was acting up. I have the Nano remote from DIY Electric btw. It will bind with the receiver just fine, but will not make the motor do anything. I tried going into VESC tool to maybe recalibrate the controller, but I couldn't get it to read anything from the remote. I also made sure my servo wires are correctly plugged in. Im super confused and frustrated, I just want to ride! Any ideas on how to fix this?
```

---
## \#2 Posted by: briman05 Posted at: 2018-07-11T04:56:41.752Z Reads: 83

```
Post a pic of your config on the vesc tool and your config into the vesc
```

---
## \#3 Posted by: tarikalauddin Posted at: 2018-07-11T05:09:55.652Z Reads: 74

```
![26%20PM|690x431](upload://6ecD87LsaTou86uih2tZfnw4pDl.jpg)![IMG_0513|375x500](upload://pItUdQ05Hx7cykbpZnfemo2yzb.JPG) (Lights are solid on receiver and remote)
```

---
## \#4 Posted by: PartyPoison Posted at: 2018-07-11T06:28:32.102Z Reads: 65

```
Your remote is AUTO BIND
Dont go to wizard for remote,
Just set your app.
Save/write.

Turn off board,
Turn on remote (push throttle up and down this for calibration)
Turn on board! Ready to go!
```

---
## \#5 Posted by: tarikalauddin Posted at: 2018-07-11T07:01:51.419Z Reads: 58

```
I went through the wizard the first time with the remote and it worked just fine. I tried what youre saying, configuring just in the app settings, under ppm, pressed "write app configuration", turned off the board, turned remote on (and did the throttle up and down), turned board on, and still nothing. Am I missing something either in the tool or physically?? Here are my settings...![26%20PM|690x431](upload://8cdFc3a9GJqHrsqm1P9eEtsklgr.jpg)![33%20PM|690x431](upload://rTHJGfTjVDGeU93VBakN0JFYgnZ.jpg)![39%20PM|690x431](upload://vMDNvHEiS0DSHmBalCarShmRett.jpg)
```

---
## \#6 Posted by: Andy87 Posted at: 2018-07-11T07:15:22.795Z Reads: 47

```
looks like you connected your receiver to the wrong channel.
![04%20PM|387x500](upload://u2D6wGgAY7iR6RkcOXdVotVK67s.png)

ch1 should be where your cables plugged in.
```

---
## \#7 Posted by: PartyPoison Posted at: 2018-07-11T11:59:49.246Z Reads: 39

```
Yeah! Wrong channel! Sorry didnt see that...
```

---
## \#8 Posted by: tarikalauddin Posted at: 2018-07-11T16:30:27.645Z Reads: 34

```
it still doesn’t work! i switched to channel 1 but does the same thing.... should i try reconfiguring the remote in the vesc tool while on channel 1?
```

---
## \#9 Posted by: PartyPoison Posted at: 2018-07-11T16:49:18.483Z Reads: 32

```
Setup

General
PPM 

Save and try again
Remote on push up and down
Board on
```

---
## \#10 Posted by: tarikalauddin Posted at: 2018-07-12T00:31:39.654Z Reads: 21

```
okay that seemed to do the trick. for some reason i have to flip the mode to low and then high before the motor will respond but that’s something i can live with as long as the remote works and i don’t have to spend another $60. thank you so much!
```

---
## \#11 Posted by: PartyPoison Posted at: 2018-07-12T03:16:24.776Z Reads: 17

```
Thats good to hear, same here, it takes some sec before the motor turn, well its ok, coz im testing the motor and connection before i ride, throttle and break!. Ride safe! Wear a helmet!
```

---
