# Police cameras causing interference?

### Replies: 27 Views: 486

## \#1 Posted by: Badgermilk Posted at: 2018-10-01T13:17:11.055Z Reads: 199

```
![Screenshot_20181001-081120|281x500](upload://yzMsVDjJidFI6iqKX1goh8rcVtX.jpeg) 

Has anyone else out there had weird board reactions around one of these cameras?  I'm pretty sure that one of these cameras caused my brakes to go from 0-100 in 0.1 seconds. You're never gonna believe what happened after that!
```

---
## \#2 Posted by: mmaner Posted at: 2018-10-01T13:21:57.163Z Reads: 192

```
if you think it's causing interference I would file an RF complaint with the FCC.
```

---
## \#3 Posted by: Jc06505n Posted at: 2018-10-01T13:22:48.026Z Reads: 192

```
What remote are you using?

https://www.electric-skateboard.builders/t/does-anyone-else-s-remote-have-spotty-connection-when-riding-by-traffic-lights-intersections/59131
```

---
## \#4 Posted by: Badgermilk Posted at: 2018-10-01T13:26:02.788Z Reads: 188

```
![Screenshot_20181001-082444|281x500](upload://vLo5YHNRCWB7pjoi8N6xhqfcV0V.jpeg) 
This nano remote from eBay.
```

---
## \#5 Posted by: Blitz Posted at: 2018-10-01T13:31:45.758Z Reads: 180

```
hehehehehehehehehe

10char
```

---
## \#6 Posted by: Badgermilk Posted at: 2018-10-01T13:33:36.283Z Reads: 179

```
2.4 GHz nano
```

---
## \#7 Posted by: Badgermilk Posted at: 2018-10-01T13:35:13.227Z Reads: 176

```
I know it probably looked funny flying of the board. Any insight beyond laughing would be greatly appreciated
```

---
## \#8 Posted by: Blitz Posted at: 2018-10-01T14:13:15.290Z Reads: 165

```
That remote say winning" on it?

because it has widely been reported that the signal on those are weak and cut out.
especially when there in metal or carbon-fiber enclosures.


And yes that camera may had interfered, but the remote is also to blame.
when the remote lose's signal for even a second it sends a signal that says 0 or something and that causes the brakes to lock up. 


Just look up winning remote issues. I regrettably bought one too, but luckily @longhairedboy told me not to use it.
```

---
## \#9 Posted by: kylem21 Posted at: 2018-10-01T14:25:04.791Z Reads: 153

```
If you have the timeout setting to 0 amps would that make it so if a cut out occurs the board just free rolls?
```

---
## \#10 Posted by: Badgermilk Posted at: 2018-10-01T14:27:02.020Z Reads: 150

```
Are you sure it would cause the brakes to lock up when signal cuts out?  I bench tested it and turned the remote off during throttle with motor running, and it just slowed gradually. I even disconnected the signal wire and same outcome.
```

---
## \#11 Posted by: Badgermilk Posted at: 2018-10-01T14:40:12.280Z Reads: 139

```
A free roll would work better for me. These stupid cameras are everywhere. ![IMG_20180930_181004074|375x500](upload://q8UrbGO4Z3xE3l9pNRyHcKtOQ4y.jpeg) 
This is what happens when the brakes lock up. It could have been way worse I guess.
```

---
## \#12 Posted by: Blitz Posted at: 2018-10-01T14:46:08.717Z Reads: 133

```
[quote="Badgermilk, post:10, topic:69737"]
Are you sure
[/quote]

Not sure. 
Like i said you can look up winning remote issues. 
you can use the forum search or google what ever floats your boat
```

---
## \#13 Posted by: JdogAwesome Posted at: 2018-10-01T14:52:53.400Z Reads: 127

```
If it's consistent around those cameras might be interesting to use an SDR, or some sort of spectrum analyzer, capable of 2.4ghz and check out the noise coming from the cameras to see if it's really generating interference. If so than yes might be worth filing a complaint with the FCC like @mmaner said. However could definitely just be that shitty remote cutting out lol.
```

---
## \#14 Posted by: mmaner Posted at: 2018-10-01T14:54:58.975Z Reads: 121

```
def could be the remote.  the only reason I mentioned this is because we had some wifi traffic cameras that showed up that were creating havon with anything wireless.  the PD claimed for months it wasn't an issue with the cameras until someone started measuring freq drift locally and proved it.  FYI, they got a ticket for stopping on the side of the road while getting the measurements :slight_smile:.
```

---
## \#15 Posted by: Badgermilk Posted at: 2018-10-01T15:01:06.133Z Reads: 116

```
Welcome to America. Land of the fleeced, home of the slave. JK. Crime fighting has been replaced by revenue generation. Anyways, I'll probably just buy a new remote. I can't afford the PTSD if this were to happen again.
```

---
## \#16 Posted by: Acido Posted at: 2018-10-01T16:54:16.416Z Reads: 99

```
Honestly i bought it from the enertion closing sale, the guy told me its like a second batch/version and I never had any problems, maybe my remote is special

but that may also be because i literally do not have any camera/ weird stop light that causes faceplanting

but my city got an new intersection with those cameras that should turn on green so you do not have to stop if the other lanes are free (that's probably a normal stop light for you :D) so I will go and check it out
```

---
## \#17 Posted by: Blitz Posted at: 2018-10-01T17:11:05.105Z Reads: 86

```
Maybe Enertion extended the the antenna, setup the fail-safe correctly so it doesn't brake on disconnection and just had better QC.

and maybe your fiberglass enclosure doesn't trap signal as much as his.
```

---
## \#18 Posted by: Badgermilk Posted at: 2018-10-01T18:00:57.787Z Reads: 77

```
My box is actually made of nylon plastic. I do have a question for the experts though. If I simulate the signal dropping by turning the controller off or pulling out the receiver wires while bench testing, the gradual slowdown of the motor which is occurring is what should happen on the street right?
```

---
## \#19 Posted by: Badgermilk Posted at: 2018-10-01T18:05:38.541Z Reads: 77

```
I mean I understand the receiver signal may drop out every now and again due to interference or weakness. My main concern is that it doesn't lock up the rear wheel when this occurs if that is what happened which I'm still not sure that is what happened. I did go into my vesc settings and adjusted brake Force to a place where it won't lock up the wheel if Max brake is applied all at once.
```

---
## \#20 Posted by: telnoi Posted at: 2018-10-01T18:14:29.366Z Reads: 75

```
A proper implementation of FHSS/AFHDS should prevent a connection from dropping completely, despite of multiple (strong) 2.4Ghz signals in the neighbourhood.

It's usually good marketing blabla (and stands for something). The fact that this is missing from all marketing material/specs I could find probably indicates that frequency hopping is missing/only performed at boot/performing poorly/insert limitation. Another possibility is that the binding process/protocol is piss poor in that the receiver accepts random signals coming in, which would explain behaviour other than what is expected during signal loss (failsafe).
```

---
## \#21 Posted by: Badgermilk Posted at: 2018-10-01T19:27:39.367Z Reads: 68

```
That all sounds good to me, but man I think it might be my vesc failing. I felt the motor lock up and stutter at low speed. Frustrated...smh
```

---
## \#22 Posted by: dareno Posted at: 2018-10-01T19:50:45.671Z Reads: 64

```
Strange one that.  When my remote disconnects (because I forget to charge it) the board just loses power and coasts.  Can be a bit surprising when it happens but no brake lock up as yet.  Touch wood.
I use the maytech sex toy as lhb has lovingly described it and the benchwheel.  Both great remotes.  
I personally hate the nano for its snatchy throttle but thats just my own preference. 

[quote="Badgermilk, post:21, topic:69737"]
I felt the motor lock up and stutter at low speed. Frustrated…smh
[/quote]
Is it sensored?
```

---
## \#23 Posted by: Badgermilk Posted at: 2018-10-01T20:39:47.281Z Reads: 55

```
No, but I always push start it without issues. Of course it will stutter from a stand still normally, but this is way different.
```

---
## \#24 Posted by: dareno Posted at: 2018-10-02T00:51:00.068Z Reads: 51

```
Thats a good thing.  I had a bad sensor blow a vesc.  The motor is good though yeah?  No smoke or funny smells?  Rotates fine with no binding?  No clicking noises?  Nothing rattling.
```

---
## \#25 Posted by: Badgermilk Posted at: 2018-10-02T14:02:44.121Z Reads: 34

```
I didn't realize how jacked up it was, because it was smooth when I bench tested it, but at heavy load, it will start stuttering, and lock up. Upon further inspection of the VESC, I noticed the positive capacitor lead was broken. I resoldered it and the mystery has been solved. Soooooooo.... As much as I would love to blame the intrusive police cameras, and I'm sure they cause a bit of interference, unfortunately I can't. This mini remote control hasn't been too bad either. The mystery has been solved. I'm not afraid of my board anymore. Thanks for all the responses, check your capacitor contacts if you ever get severe stuttering and wheel lock, and always wear a helmet. ✌️
```

---
## \#26 Posted by: dareno Posted at: 2018-10-02T17:24:32.395Z Reads: 28

```
Great news.  new one on me though never had that happen.
```

---
## \#27 Posted by: baxtred Posted at: 2018-10-10T08:13:43.737Z Reads: 20

```
I have the same remote!

![IMG_20180816_202508|375x500](upload://eAoUbXuXtemM5q1kBkS5jkc77Cl.jpeg)

(learned I had my failsafe set to full brake, fixed now... And that's the good looking hand)
```

---
