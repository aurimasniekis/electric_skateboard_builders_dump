# Wanna hear a weird VESC problem? CLICK HERE

### Replies: 16 Views: 1037

## \#1 Posted by: Challlsss Posted at: 2017-08-03T05:48:12.284Z Reads: 197

```
So I just finished turning my 6S Lipo board into a 6S2P Lipo board and I was stoked to give it a shot! So I plugged that sucker into the computer, ran a motor detect and hopped on it for a quick test ride. After riding around I decided I wanted more glue on my enclosure.... (my enclosure looks a lil something like this...)
<img src="/uploads/db1493/original/3X/c/a/ca71a595e1f3b78933134fe01ca43db115a0fd28.png" width="300" height="200">
And so after painstakingly waiting the 48 hours for the glue to cure I hopped on the board. Stoked for another test ride. BUT IT WAS NOT GOING TO HAPPEN. My board was at full brake without touching the remote and the only way to get the motor to spin at all was at full throttle where the wheel was only going about 2 mph.  Something was _wrong_ . 

So I ran upstairs and plugged the sucker into the computer, ran a motor detection and thought... well everything seems in order. But when I used the arrow keys just so spin the motor (for shits and giggles) the motor just twitched... So I panicked and checked for faults, _zip, zilch, nada_ .

I went back and ran a motor test again, it worked perfectly. 

Tried the arrows, nothing. 

Check the lil' real time plot, nothing happening, no current and just a wee little negative erpm when I hit a button. 

So naturally, I get pissed and start pressing all the arrow keys a bunch and the motor is just twitching a lil' bit, like a paraplegic who just managed to wiggle their big toe, (it's moving but just barely) Then I hear/see what every esk8 member dread a quiet pop aaaaaand red flashing light. I thought I was hosed. I go to check what the error code is and before I can do it the motor starts spinning on its own.

WTF It rocked a little bit backward, then a little bit forward about 5 times. Then it went __FULL THROTTLE__ without me touching _anything_ I mean nothing. The wireless remote was off and both hands were off the keyboard of my computer and this motor is going fast as hell. So I unplug the power and the  motor stops. I plug it back in and run a motor detection, no issues. I press the arrows, slight twitch. I then replicated the failure by mashing the arrow for a few seconds and I hear the _pop_ and red light flash. Here is my error code and settings:
<img src="/uploads/db1493/original/3X/0/7/0759a704ccd3fcad76cb1eaef5af90a60de96909.png" width="690" height="311">
<img src="/uploads/db1493/original/3X/c/d/cdf891b44f70dbef238230ed2408b76e74ce134a.png" width="690" height="308"><img src="/uploads/db1493/original/3X/8/4/84471afcabed06cea26a09dc0244931c50812f63.png" width="690" height="305">
I would really love some input here as I am completely lost as to WTF is wrong with my setup: 
Why does motor detection work fine? 
Why does the motor work for a few seconds then full brake?
Why am I getting an over current fault?
Please send halp.
```

---
## \#2 Posted by: Martinsp Posted at: 2017-08-03T06:08:40.914Z Reads: 161

```
Hey, what firmware are you using? Can you take a screenshot of your advanced tab in the motor config?
Also sometimes if you do your motor detection and have set PPM instead of No app it can mess with the results but I dont think that is your problem.  Also do your motor detection without motor connected to the wheel.
What happens if you hold an arrow key and "help the motor spin" with your hand?  Does it spin up or not at all?
Check your solder joints on motor connectors and on the VESC itself where the 3 phase wires connect to it.
```

---
## \#3 Posted by: L3chef Posted at: 2017-08-03T09:43:16.914Z Reads: 140

```
Hmm, try lowering your motor max and see if it helps.
```

---
## \#4 Posted by: Challlsss Posted at: 2017-08-03T13:29:42.364Z Reads: 122

```
<img src="/uploads/db1493/original/3X/e/e/ee19bf5857d5fe27cb9d90729c1fb1e7b6e63f47.png" width="690" height="309">

here are my advanced settings
```

---
## \#5 Posted by: Martinsp Posted at: 2017-08-03T14:40:24.239Z Reads: 103

```
Is it what you have set in the VESC? because it is showing that it is not connected.. just to make sure :D 

Did you try to spin up the motor with hand as i said before?
```

---
## \#6 Posted by: Ackmaniac Posted at: 2017-08-03T14:55:38.701Z Reads: 97

```
Ok go to the "App configuration" Tab and then on the left in the General Tab select "No app" and write the configuration. Now try to use the arrow keys. When this works then you first have to check your remote, adjust the failsafe and chosse the right settings in the PPM Tab.
```

---
## \#7 Posted by: Challlsss Posted at: 2017-08-03T20:08:28.249Z Reads: 81

```
Ok. I'm still at work but I'll give these a try soon and update. As far as the not connected that's because I took the screenshot while the board was off.
```

---
## \#8 Posted by: trancejunkiexxl Posted at: 2017-08-03T20:32:24.019Z Reads: 75

```
so i had soemthing similar to this happen, somehow i lost my ppm settings.. did a remote calibration and now im back on.. it would go full throttle just like you said until i changed the min pulse-width.. with the default programming it thought i was already gunning it.. hope you get it fixed gl bro!
```

---
## \#9 Posted by: Challlsss Posted at: 2017-08-04T02:44:30.900Z Reads: 65

```
@Ackmaniac 's solution worked. But I am unsure how to adjust the fail safe and PPM settings. I will look in other threads, but if anyone sees this before I delete this comment and knows where a good link / what to do and how to share it would be much appreciated!

Thanks for all the help!

***UPDATE: So I'm pretty sure the problem lies in the receiver. It isn't connecting to the remote at all now. (Nano-X) anyway I am going camping tomorrow but will pick up a servo wire and do some testing. Will update on Saturday. This could be a much easier fix than I had hoped! Cheers
```

---
## \#10 Posted by: evoheyax Posted at: 2017-08-04T03:34:18.980Z Reads: 55

```
The error you got means your throwing a fault due to too high of a voltage, likely because your input voltage is above your vesc's max voltage. This would then lead the motor detection to work, but it would try to spin, and fail because the second it tries, it throws a warning and boom!

Could you post the main vesc settings again and post the voltage of your pack?
```

---
## \#11 Posted by: Challlsss Posted at: 2017-08-04T03:56:46.302Z Reads: 51

```
It's a 6S pack max voltage at default 57 volts

Oh and it's the VESC-X (I got it right before the rename)
```

---
## \#12 Posted by: evoheyax Posted at: 2017-08-04T05:06:33.819Z Reads: 47

```
So weird, that's what it means, but if it's at 57, then idk...
```

---
## \#13 Posted by: Challlsss Posted at: 2017-08-04T06:11:45.159Z Reads: 50

```
Sure it's not current? the first thing it says is that somehow it hit 150ish amps
```

---
## \#14 Posted by: Challlsss Posted at: 2017-08-06T21:58:43.748Z Reads: 38

```
Update* so I know that the problem likely lies in the receiver, as the light flashes once then does not keep flashing. Has anyone else ever had this problem/know a way to fix it besides replacing parts?
```

---
## \#15 Posted by: leroy Posted at: 2017-11-04T18:44:23.264Z Reads: 31

```
I had something similar and I want to say I was the connection from the vesc to the wires for the receiver, 
I replaced the wires and solved my problem.
```

---
## \#16 Posted by: telnoi Posted at: 2017-11-04T18:49:25.506Z Reads: 29

```
Measure your 5v out when the receiver is connected and ensure that it stays stable and does not drop.
```

---
