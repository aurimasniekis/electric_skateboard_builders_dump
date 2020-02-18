# Is my VESC dead? Riding fine until today

### Replies: 28 Views: 2074

## \#1 Posted by: c4Lvin Posted at: 2016-06-14T07:09:28.821Z Reads: 157

```
Guys, just started riding on a pretty new board I bought from a fellow here. Riding on the trails at 10-12mph and started feeling no throttle, then the brakes would lock up once every few seconds. Few more minutes, then absolutely no more response at all. Pedaled home and that's not a good feeling with 2+ miles on this thing. Never abused this board and treat her like a gem. I have no idea what happened. I still see a solid blue LED and then there's another solid smaller green LED. But the motor does not move. I've plugged another RC servo into my 2.4GHz receiver so it's not that as it responds normally (the RC servo). I got it to rev a few times but never again. I first thought it was just the receiver glitching or something but I even changed out the receiver to a standard RC 27MHz AM receiver and still the VESC is the same. I have yet to plug it up to my PC tonight but will try it tomorrow. I have NEVER actually plugged it up. Is this a common problem with these VESCs? If that's the case, these things are not ready for the mainstream market. I mean if the user did absolutely nothing wrong, it should not fail within 20-30 miles of light cruising. Getting really frustrated with these VESCs. If I can't fix this, there will be nomore that I will be purchasing. I'd rather have a cheapo RC ESC with limited easy tuning and sacrifice all the little tuning capabilities but prone to be damaged easily and drop more money into this already expensive hobby.
```

---
## \#2 Posted by: willpark16 Posted at: 2016-06-14T07:12:51.800Z Reads: 152

```
where did u get it from?
```

---
## \#3 Posted by: c4Lvin Posted at: 2016-06-14T07:15:40.836Z Reads: 148

```
I think the VESC is from Enertion. I can post pictures up in the morning after I clean it up and plug it into my PC. Anyone think it's fried? I doubt it because motor was barely warm, 65-70 degree outside in the evening. Nothing was really warm or even hot to the touch. I check it because I want to see how far I could ride from a full charge. I barely used up 20% from the Space Cell :(
```

---
## \#4 Posted by: willpark16 Posted at: 2016-06-14T07:17:50.293Z Reads: 140

```
well i do know that the red ones from enertion are prone to drv failures and such, so check ur DRV and if its not that just post a couple photos so i can see if anything is fried. Also sniff for burned electronics
```

---
## \#5 Posted by: c4Lvin Posted at: 2016-06-14T07:20:12.296Z Reads: 139

```
willpark16 i sniffed it and doesn't seem like anything was burnt. None of those 3 capacitors or whatever just hanging seems to have leaked or buldging. Give me a few minutes I'll take a few shots for everyone now.
```

---
## \#6 Posted by: willpark16 Posted at: 2016-06-14T07:21:13.224Z Reads: 135

```
Make sure to get a nice shot of your DRV
```

---
## \#7 Posted by: c4Lvin Posted at: 2016-06-14T07:28:32.611Z Reads: 135

```
OK here are a few shots. I don't even know what version they are. And earlier I was reading posts about people frying their DRV chips with new firmware or whatever...I never did any upgrades, just got it as is. Anyhow here are some pictures.<img src="/uploads/db1493/original/2X/5/5e52b04d95e506a1d87bf78f40a8290320f58174.jpg" width="666" height="500">
<img src="/uploads/db1493/original/2X/5/5335ff9a8ba325392bb31368a70f313d812c646a.jpg" width="666" height="500">
<img src="/uploads/db1493/original/2X/7/7412fe082f88dcbdc6ba82e49b78a839a96fff95.jpg" width="666" height="500">
<img src="/uploads/db1493/original/2X/d/d54003579c079dfdc84212c0a65e455f2487dbee.jpg" width="375" height="500">
```

---
## \#8 Posted by: trbt555 Posted at: 2016-06-14T07:29:48.194Z Reads: 129

```
Connect it to BLDC-tool while still on your board and connected to the batteries.
Activate live sampling
Pull the throttle trigger and watch what happens to the LEDS.
Take a screenshot of the live sampling window
Type "FAULTS" in the terminal pane, this should return a list of faults encountered since last power-up.
Report back with results.
```

---
## \#9 Posted by: c4Lvin Posted at: 2016-06-14T07:31:23.981Z Reads: 131

```
Thanks guys for the help. I'll try it in the morning as it's 1230AM here and got to work tomorrow. Hopefully I can revive it with all of your help. Probably can't sleep tonight!
```

---
## \#10 Posted by: elkick Posted at: 2016-06-14T07:51:58.272Z Reads: 129

```
Are you sure that this PPM cable you are using is ok? Everything you're describing here indicates a PPM issue somewhere. Vibrations can cause a lot of troubles.
```

---
## \#11 Posted by: trbt555 Posted at: 2016-06-14T08:16:00.650Z Reads: 126

```
While you have your vesc connected to BLDC tool, you can use the arrow keys to run the motor.
This can potentially give you a clue if the PWM cable or input aren't working correctly.
```

---
## \#12 Posted by: treenutter Posted at: 2016-06-14T13:23:52.356Z Reads: 118

```
@c4Lvin Check your connections from the VESC to the motor and make sure they are still fully connected and that there are no shorts. If any one of those cables is lose, vibration can knock them around so that they disconnect while you're riding. I highly recommend taping them.
```

---
## \#13 Posted by: FLATLINEcustoms Posted at: 2016-06-14T17:49:47.958Z Reads: 109

```
I see some carbon fiber in the background. Your VESC wasn't resting on that was it? Or possibly bumped into it?
```

---
## \#14 Posted by: c4Lvin Posted at: 2016-06-14T19:24:31.464Z Reads: 102

```
guys, i'm trying to bring an old laptop in the garage to try out the first time plugged into BLDC tool. Would it work with a Windows XP machine? That way I could just leave that old silly laptop there for tuning future e-board projects. @FLATLINEcustoms Yes it's carbon fiber but the VESC was carefully wrapped in some form of partial bicycle tire tubing and electrical tape with the bottom being double sided tape down so I don't think it would have shorted out in that way. Let me get this started. Thanks guys for all the input. Do appreciate it.
```

---
## \#15 Posted by: c4Lvin Posted at: 2016-06-14T19:59:28.048Z Reads: 91

```
I got it connected now. But it states that my firmware was too old and is limited? Firmware on now is 1.14. Supported Firmwares (for this version of BLDC tool) is 2.17 and 2.18. Where do I go from here guys? I don't want to proceed without anyone's advice. Thank you.

So I downloaded the correct BLDC tool for my 1.14FW and got it going. I guess I can worry about the FW later if that's the case. Anyways, when I go into "start detection" bad detection result received on the bottom right hand corner. No clue what to do now. Checked all motor settings, etc.
```

---
## \#16 Posted by: c4Lvin Posted at: 2016-06-14T21:02:13.463Z Reads: 90

```
here's the "faults" from terminal panel:
<img src="/uploads/db1493/original/2X/5/5ff43fdfefa54cf553b35967e4979073e9abc475.png" width="690" height="388">

and the realtime data:
<img src="/uploads/db1493/original/2X/0/0ea0bc68f92b267ac0a7b95b51cf910b5a310efa.png" width="690" height="388">
```

---
## \#17 Posted by: trbt555 Posted at: 2016-06-15T05:06:55.447Z Reads: 79

```
I'd say the DRV chip is fried. Not uncommon.
```

---
## \#18 Posted by: c4Lvin Posted at: 2016-06-15T05:08:47.238Z Reads: 80

```
thanks pal. I asked if anyone can help me replace just that chip to give it a shot. I'm afraid to setup the new one (exactly the same) at the moment. There goes all the hard savings :frowning:
```

---
## \#19 Posted by: lox897 Posted at: 2016-06-15T09:00:07.086Z Reads: 77

```
Did you configure your VESC at all or did you just use it out of the box? The VESC isn't plug and play. You have to configure it.
```

---
## \#20 Posted by: c4Lvin Posted at: 2016-06-15T09:01:57.505Z Reads: 73

```
I personally did not configure it. I believe that the original owner did in some way. I seriously cannot tell.
```

---
## \#21 Posted by: lox897 Posted at: 2016-06-15T09:05:26.623Z Reads: 72

```
You need to configure it to your exact setup. That is probably why your DRV fried.
```

---
## \#22 Posted by: c4Lvin Posted at: 2016-06-15T09:11:08.630Z Reads: 72

```
Is there something that looked particularly wrong in the settings that would damage the VESC?  It was doing perfectly fine for the first 3 or 4 rides totaling over 15-20 miles without any problems whatsoever.  If so what would be the correct parameters so I can setup my spare one myself without it being damaged one again.  Thanks.
```

---
## \#23 Posted by: lox897 Posted at: 2016-06-15T09:12:24.616Z Reads: 75

```
Can you send some pictures of your motor and battery configurations? You'll also need to provide some specs of your board (motor kv, esc, battery voltage, etc)
```

---
## \#24 Posted by: c4Lvin Posted at: 2016-06-15T09:15:06.485Z Reads: 73

```
Single Enertion rspec 6355 2.0 190kv, space cell 36V 10S3P, 83mm flywheel clones, etc . Can't think of anything else.  Oh 2.4ghz gt2 or gt3b.
```

---
## \#25 Posted by: lox897 Posted at: 2016-06-15T09:18:48.745Z Reads: 71

```
Screenshots please.
```

---
## \#26 Posted by: c4Lvin Posted at: 2016-06-15T09:26:24.084Z Reads: 71

```
I'll get some shots in the morning. It's almost 230am here.  Thank you guys
```

---
## \#27 Posted by: c4Lvin Posted at: 2016-06-17T01:21:21.576Z Reads: 60

```
I no longer have the screenshots but did record it under MS Word. I can't get the new screenshot as the VESC is being looked at. Can I send this MS Word file to you @lox897 ? Thanks
```

---
## \#28 Posted by: lox897 Posted at: 2016-06-17T11:16:27.399Z Reads: 56

```
I have never used a VESC but I know a little bit about them. It is probably best to send it to @chaka @barajabali @onloop @cmatson @longhairedboy or any other experienced VESC user. If you want you can send it to me as well but the other guys have more experience. I will PM you my email address.
```

---
