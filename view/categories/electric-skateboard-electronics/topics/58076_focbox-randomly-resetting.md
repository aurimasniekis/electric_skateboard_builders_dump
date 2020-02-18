# Focbox randomly resetting

### Replies: 32 Views: 696

## \#1 Posted by: 91stantheman Posted at: 2018-06-06T23:31:15.152Z Reads: 159

```
Goodness I hope someone here can help me... my setup is a gt2b rx and TX, 2 5s  8Ah  lipo's in series, with a 6364 turnegy sk3. While riding my focbox randomly resets on me, usually during acceleration or breaking (gets scary). Most of the time I can get it to come back by hitting the opposite of what I was doing when It cut out ((break it i was accelerating), (throttle if I was breaking)). I'm running Ackmaniac's app and whenever this happens it freezes and stops recording data. When it recovers it starts over as if I just fired up the board, that's why I'm assuming its resetting. If anyone can point me in the right direction for troubleshooting that would be amazing. I just want to trust the board...
```

---
## \#2 Posted by: Scoo_B_SK8 Posted at: 2018-06-07T00:28:01.576Z Reads: 150

```
post (screenshot) your settings, probably hitting a cutoff somewhere
```

---
## \#3 Posted by: 91stantheman Posted at: 2018-06-07T10:47:14.161Z Reads: 143

```
![Screenshot_20180607-054506_ESC%20Monitor|243x500](upload://lUbJC40daFWerRJVIEjZrhWGIQg.jpg)

Here are some of them, I'll post up my settings in the vesc tool this evening
```

---
## \#4 Posted by: TarzanHBK Posted at: 2018-06-07T10:52:16.147Z Reads: 124

```
after the cutout happens, check for faults and let us see the result.
```

---
## \#5 Posted by: 91stantheman Posted at: 2018-06-07T11:31:03.506Z Reads: 117

```
I have and I don't get anything for faults, I'm not sure it is because it has reset itself or if it just isn't spitting out any but there are none when I check.
```

---
## \#6 Posted by: 91stantheman Posted at: 2018-06-07T16:52:39.959Z Reads: 113

```
Truthfully I don't think it's an issue with my settings, because the problem seems to come in waves and sometimes be more frequent than others. At its worst it will cut out as soon as I start moving with barely any throttle.
```

---
## \#7 Posted by: Deckoz Posted at: 2018-06-07T16:54:16.237Z Reads: 111

```
sounds like you aren't calibrating your throttle on startup and focbox receiving out of ppm range signal

ensure you go full throttle and full brake when powering on the remote, then power on the board.
```

---
## \#8 Posted by: JohnnyMeduse Posted at: 2018-06-07T16:56:37.695Z Reads: 107

```
How did you program your focbox? did you run any motor detection?

 Can you screenshot your parameter from the PC not an app
```

---
## \#9 Posted by: 91stantheman Posted at: 2018-06-07T17:24:43.528Z Reads: 100

```
I didn't even know you were supposed to calibrate the gt2b when you start it up... I'll definitely try that.
```

---
## \#10 Posted by: 91stantheman Posted at: 2018-06-07T17:25:43.156Z Reads: 99

```
Yes I ran motor detection. I'll post up the parameters in a couple hours when i get off work.
```

---
## \#11 Posted by: TarzanHBK Posted at: 2018-06-08T08:17:15.531Z Reads: 92

```
Maybe just start from zero. Load standard values and set up your focboxes new from start. Most of the time you just set a wrong value or didnt run a detection properly.
Report back if that helped. If not post screenshots of your settings
```

---
## \#12 Posted by: 91stantheman Posted at: 2018-06-08T11:31:20.868Z Reads: 90

```
Yah that's not a bad idea,  I didn't get a chance  to post my settings last night but I'm still testing the controller calibration idea. Went for a mile ride and didn't have one cut out. Can't say that was it yet until I go for a longer ride.
```

---
## \#13 Posted by: 91stantheman Posted at: 2018-06-09T12:55:21.031Z Reads: 89

```
![Capture3|690x487](upload://jtOPJycTqdC33vj59B6F866Sou1.PNG)![Capture2|690x160](upload://cbpLC4MMY4Q7Tl07xgGITPcwDab.PNG)![Capture|690x397](upload://rLUMNN4ZL9ibUUu9uVeJe9AAsXh.PNG)


here are some of my settings, i uploaded new firmware and left everything alone except motor detection and ppm mapping. going for a long ride today to see what happens.
```

---
## \#14 Posted by: 91stantheman Posted at: 2018-06-09T16:58:41.774Z Reads: 78

```
Slight difference now but still doing the same thing. Now it mainly does it when I'm at low speed at full throttle up a hill for a second or two, and when I'm on the throttle or break and hit a big crack in the road. That sounds like a abs max issue but it's set where it should be so idk.

It still cuts out randomly every now and then which adds a bunch of confusion to it all.
```

---
## \#15 Posted by: JohnnyMeduse Posted at: 2018-06-09T17:26:30.954Z Reads: 78

```
can you post picture of your build? and what type of connector are you using to connect your battery?
```

---
## \#16 Posted by: Silverline Posted at: 2018-06-09T19:57:41.785Z Reads: 73

```
What is your two battery cutoff's on the vesc ?

Do you have the metr module, so you could log your ride, and se in the log what is happening that exact  moment, it could be voltage sag from a bad battery / Connection.  
Are you shure your two lipo's is in good condition, and still got all the cells in ballance ?

Also have your checked your connections on the three phase wires between motor and vesc.
```

---
## \#17 Posted by: Ackmaniac Posted at: 2018-06-10T01:09:22.142Z Reads: 69

```
I would say your remote has a problem. Check the antenna on the receiver and on the remote. If you have a modded remote it is very likely the antenna is damaged.
Which firmware do you run (exact version number please) and do you experience a immediate power dropout or a decrease in power?
Of course also check your Pulsewith settings to be sure you didn't mess them up.

You can also check to be sure that it is a signal loss by adjusting the timeout ms. Set it to 250ms and if get's worse after that then you can be sure that that is the problem.
![image|643x192](upload://7gHYZCR6ngWBQVHG4sE9ieUgIDd.png) 

And that it happens at hard acceleration, braking and cracks makes sense when the antenna is broken by too much bending.

And yes GT2B do fail when you treat the antenna badly. I saw 2 bad once already that had signal losses.
```

---
## \#18 Posted by: 91stantheman Posted at: 2018-06-10T17:31:19.486Z Reads: 64

```
Wow, some big names hopping in to help. Thank you guys for taking time to help me, I feel pretty honored, and thank you for all you have contributed to this community. 

Johnny, I can take pics when I take the board apart later, but I have the factory bullet connectors making the series connection and they are heat shrieked together. From there its xt90's with 10 gauge wire until the focbox where I made an adapter to a xt60 with 12 gauge wire.

Silvermine, my cutoffs are 3.6 and 3.4. I'm not sure what module your talking about, but ackmaniac's app doesn't even record the issue when it happens. The app just freezes up until the board starts working again. My lipo's are brand new and operate like normal. I'm still getting 10 or so miles of range, so it could be connectors, I'll check them really closely when I pull it back apart. The phase wired are using the spring cage connectors normally used on rc motors. But when I had a bad factory solder joint on the focbox causing high resistance on one phase I got a ABS_overcurrent fault, not the symptom I'm having now. Still doesn't mean it's not the issue tho.

Ackmaniac, you are not the first to say that. I have a fair amount of experience with RF and building antennas myself, so I was considering building one for it to rule that out. My question is tho, how would that cause the sec to reset? When I turn the remote off nothing changes. The app still works fine and everything is still tracking. That's what makes me thing the vesc is completely resetting, because I lose my miles traveled and everything on your app.
I just updated with your latest firmware yesterday with 3.102 and left everything alone except voltage and PPM  mapping. I experience a immediate power drop out, as if the plug was pulled.
It doesn't happen only on those 3 situations but it seems to favor them. Occasionally I will be coasting on smooth pavement and when I go to get on the breaks or throttle it's just gone. I believe it would be the gt2b, but I have checked the solder joint on the antenna and it looks good, no shorts or stray wires. And I shrink wrapped the whole thing except the actual tx wire after the can to make sure there are no shorts.
```

---
## \#19 Posted by: Scoo_B_SK8 Posted at: 2018-06-10T17:44:18.634Z Reads: 59

```
i would try and lower the...
"Motor Current Max"
&
"Motor Current Max Brake"

cut both in half

(-60 on the brakes is alot in my opinion, i ride mine at -20)

your also in good hands with JonnyMeduse & Ackmaniac
```

---
## \#20 Posted by: Ackmaniac Posted at: 2018-06-10T18:29:23.317Z Reads: 58

```
When the ridden distance in the app is reset as well then it is even worse. Then you don't only have a error. Your system does a complete reset. Which means the focbox looses power. Only issue can be loose wires or loose nickel strips on your battery.
Because after a fault the distance and consumed wh/ah would still be available. 
Maybe you can record a video with the app.
```

---
## \#21 Posted by: 91stantheman Posted at: 2018-06-12T22:53:04.551Z Reads: 53

```
I'll post a video in a few when I take it out for a ride. I just took it apart to look at all connections and they all look good. No burn marks, not indications of hot wires, nothing.
```

---
## \#22 Posted by: 91stantheman Posted at: 2018-06-13T01:02:37.327Z Reads: 50

```
So I actually caught a fault code on the video, got an abs overcurrent fault. Not sure if that could cause the reset but its something. Can anyone give me a clue in how to upload the videos? Can't figure it out.
```

---
## \#23 Posted by: mmaner Posted at: 2018-06-13T02:43:47.940Z Reads: 47

```
Upload to YouTube then post the YouTube link.
```

---
## \#24 Posted by: 91stantheman Posted at: 2018-06-13T12:56:21.421Z Reads: 46

```
https://youtu.be/X5f3t6Cclj4

Here is the reset, happens right away and a few times during the video. Idk what happened with the audio, maby ackmaniac knows.
```

---
## \#25 Posted by: 91stantheman Posted at: 2018-06-13T13:05:59.363Z Reads: 45

```
https://youtu.be/TRIr8I5gwbE

Here is the video of the fault code popping up. Hopefully this leads to something.
```

---
## \#26 Posted by: TarzanHBK Posted at: 2018-06-22T09:57:24.871Z Reads: 36

```
Looks like something is shorting.
Vesc is shutting down to protect itself.
```

---
## \#27 Posted by: 91stantheman Posted at: 2018-06-22T17:39:31.643Z Reads: 32

```
Yah but what? The motor or the focbox? I really don't want to fork out the cash for either...
```

---
## \#28 Posted by: Sender Posted at: 2018-06-22T20:06:07.687Z Reads: 31

```
Did you change the max regen (batt min)? That is really high. -40.... try -20 on regen?
```

---
## \#29 Posted by: 91stantheman Posted at: 2018-06-22T23:06:02.061Z Reads: 27

```
Yah I have played with it, hasn't really changed anything. I'll try again this weekend and let you know
```

---
## \#30 Posted by: 91stantheman Posted at: 2018-06-22T23:09:34.195Z Reads: 29

```
Good news tho, I messaged hobbyking and they are sending me a replacement motor.
```

---
## \#31 Posted by: maxbicyclemax Posted at: 2019-11-26T13:45:39.500Z Reads: 5

```
How did you go with this??
I just had the same thing. Except I crashed.
I thought my remote may have disconnected or switched off, I lost throttle, tried brakes nothing then full.
I first thought it could be any number of things but realized the distance and consumed power had reset to zero.
Now sure that could be a connection or battery problem (and maybe it is) but I really don't think it is as it was only momentarily and only happened once...
If you found anything I'd really appreciate to hear
```

---
## \#32 Posted by: maxbicyclemax Posted at: 2019-11-26T13:47:40.812Z Reads: 5

```
@91stantheman see above please
Thx
```

---
