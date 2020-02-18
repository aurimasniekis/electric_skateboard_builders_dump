# Foc vesc beginner settings

### Replies: 37 Views: 3139

## \#1 Posted by: ekitesurfer Posted at: 2016-08-30T14:38:02.200Z Reads: 345

```
I would like to be able to set this board up so that I could hand it to someone and not worry as much. What settings would you guys focus on?
```

---
## \#2 Posted by: Blasto Posted at: 2016-08-30T14:43:11.695Z Reads: 347

```
Set it in BLDC not FOC. FOC is not that easy to setup and can permanently damage your vesc if not done right.
```

---
## \#3 Posted by: rpn314 Posted at: 2016-08-30T14:45:49.545Z Reads: 346

```
I would definitely second @Blasto. BLDC mode is much more simple to set up, and not mess up. To add to that, I would set the max amp from the battery and erpm settings pretty low....I'd worry about people crashing and being dumb in general, so I'd limit them pretty heavily. Basically create a "beginner" mode :slight_smile:
```

---
## \#4 Posted by: ekitesurfer Posted at: 2016-08-30T14:53:54.200Z Reads: 338

```
I have blown vescs, I know... I seem to have one that is working (knock on wood). I tried decreasing the brake setting  to -6 from -12 and it didn't really do much. I am scared to change settings in foc, and I am also scared to switch to bldc from foc, so this thing is staying foc....  are there any settings I can play with?
```

---
## \#5 Posted by: DeathCookies Posted at: 2016-08-30T15:07:18.175Z Reads: 319

```
Motor Max
Battery Max
erpm limit
maybe ramp

If you want to change to bldc just flash a new firmware on it and you are ready to go
```

---
## \#6 Posted by: ekitesurfer Posted at: 2016-08-30T15:14:10.621Z Reads: 303

```
Don't really want to switch to bldc on this vesc, that's why I got a 12s esc from diy, but I had to send it back because I couldn't get the brakes to lighten up.
```

---
## \#7 Posted by: rpn314 Posted at: 2016-08-30T15:20:09.794Z Reads: 295

```
As long as it's functioning in FOC right now, I wouldn't switch it either. If all you're doing is preparing it so someone who knows nothing can use it (which I honestly wouldn't do unless I was standing there with them), I would turn down the Batt Max in the current Limits and maybe turn town the max ERPM limit so they can't go as fast and then probably disable reverse if you have it. Give them braking, but not reverse :) I just have a large distrust of everyone who doesn't know what these boards can do.
```

---
## \#8 Posted by: ekitesurfer Posted at: 2016-08-30T15:20:19.714Z Reads: 288

```
I would really just like to lower acceleration and deceleration.
```

---
## \#9 Posted by: Jinra Posted at: 2016-08-30T15:27:48.971Z Reads: 278

```
there's two brake settings, battery Regen and motor min. try decreasing motor min for lighter brakes
```

---
## \#10 Posted by: ekitesurfer Posted at: 2016-08-30T15:29:26.828Z Reads: 271

```
I tried that, -6 now
```

---
## \#11 Posted by: Jinra Posted at: 2016-08-30T15:30:27.003Z Reads: 260

```
you're at -6 battery and motor Regen?
```

---
## \#12 Posted by: ekitesurfer Posted at: 2016-08-30T15:34:47.313Z Reads: 254

```
It is on whatever onloop recommended... my laptop is at work, can't play with settings at home currently
```

---
## \#13 Posted by: Jinra Posted at: 2016-08-30T15:36:36.809Z Reads: 253

```
-6 sounds like your battery Regen to me, especially if you changed it from -12a (max charge current of the space cell 3).

just double check your motor regen later. If they're both low you should have pretty weak brakes.
```

---
## \#14 Posted by: ekitesurfer Posted at: 2016-08-30T15:39:43.429Z Reads: 251

```
I believe it is at -60
```

---
## \#15 Posted by: Jinra Posted at: 2016-08-30T15:41:26.221Z Reads: 248

```
that would make sense. try using -40a if your brakes are too strong.
```

---
## \#16 Posted by: ekitesurfer Posted at: 2016-08-30T15:43:59.797Z Reads: 245

```
Should I put the other setting back to -12?
```

---
## \#17 Posted by: Jinra Posted at: 2016-08-30T15:45:17.070Z Reads: 236

```
if you want the maximum regen. i have mine at max. it does affect braking somewhat as well so you wouldn't want it to be at 0 but -6 should be fine.
```

---
## \#18 Posted by: ekitesurfer Posted at: 2016-08-30T15:48:57.256Z Reads: 236

```
How do I decelereate this thing now?
```

---
## \#19 Posted by: Jinra Posted at: 2016-08-30T15:50:01.062Z Reads: 235

```
I'm not sure what you mean
```

---
## \#20 Posted by: ekitesurfer Posted at: 2016-08-30T15:51:31.430Z Reads: 234

```
Make it accelerate slower
```

---
## \#21 Posted by: Jinra Posted at: 2016-08-30T15:54:13.929Z Reads: 218

```
decrease motor max. you may have to decrease battery max too depending on value
```

---
## \#22 Posted by: ekitesurfer Posted at: 2016-08-30T15:58:47.852Z Reads: 215

```
Motor is 80, batt is 30, what should I switch them to?
```

---
## \#23 Posted by: Jinra Posted at: 2016-08-30T15:59:24.380Z Reads: 213

```
try motor max 50 or 60
```

---
## \#24 Posted by: ekitesurfer Posted at: 2016-08-30T16:02:34.228Z Reads: 212

```
Leave batt at 30?
```

---
## \#25 Posted by: Jinra Posted at: 2016-08-30T16:06:15.888Z Reads: 209

```
yep that's fine
```

---
## \#26 Posted by: ekitesurfer Posted at: 2016-08-30T16:22:15.175Z Reads: 205

```
I will change settings when I have my pc tonight, I'll let you know what I think, but thanks:)
```

---
## \#27 Posted by: ekitesurfer Posted at: 2016-09-05T07:09:52.878Z Reads: 182

```
I put my

motor max 40a
motor min -20
Batt max  30 
batt min -6
absolute max 130

These settings calmed it down quite a bit. I like how I can hit full brake and ride the brake going downhill or slowing down.
Do these seem ok? should I change anything?
Thanks!
```

---
## \#28 Posted by: Jinra Posted at: 2016-09-05T07:25:59.833Z Reads: 173

```
Sounds good, just adjust as necessary. I'd raise the battery Regen myself.
```

---
## \#29 Posted by: ekitesurfer Posted at: 2016-09-05T07:26:50.417Z Reads: 174

```
Back to -12?
```

---
## \#30 Posted by: Jinra Posted at: 2016-09-05T07:27:46.375Z Reads: 169

```
yep, if you're running 3p
```

---
## \#31 Posted by: ekitesurfer Posted at: 2016-09-05T07:28:57.507Z Reads: 167

```
What if I am running 4p?
```

---
## \#32 Posted by: Jinra Posted at: 2016-09-05T07:31:06.625Z Reads: 169

```
What cells? I use -16 on my 4p pack.
```

---
## \#33 Posted by: ekitesurfer Posted at: 2016-09-05T07:31:55.195Z Reads: 172

```
I have space 3 and 4...
```

---
## \#34 Posted by: Jinra Posted at: 2016-09-05T07:32:46.401Z Reads: 173

```
yea -12 for the 3 and -16 for the 4
```

---
## \#35 Posted by: paulbriz Posted at: 2019-01-19T20:09:26.177Z Reads: 35

```
hey, im haveing trouble with my first build, 6374 192kv 12s2p and a 4.12 vesc it turns on okay but when i press throotle motor will jolt then vesc turns off please help
```

---
## \#36 Posted by: Andy87 Posted at: 2019-01-19T21:09:29.997Z Reads: 35

```
Do your motor detection and ppm adjustments and you should be good
```

---
## \#37 Posted by: paulbriz Posted at: 2019-01-19T21:15:21.209Z Reads: 35

```
Annoyingly I've actually done that , but I'll try again , is fix more dangerous then bldc on vesc tool
```

---
