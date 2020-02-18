# Focbox &ldquo;Modes&rdquo; i.e. slow/fast

### Replies: 16 Views: 1446

## \#1 Posted by: DavidBanner Posted at: 2017-11-10T11:59:24.511Z Reads: 213

```
Is there any way to create "modes" in the FOCBOX (i.e a VESC)?  i.e.slow/fast modes which can be switched via a button on the remote? 

I have someone who is being told this is 100% possible with any remote ( assuming it can more than 1 channel, etc etc).

The nano-x controller has this functionality but I had assumed it was by limiting the PPM values sent within the controller rather than the VESC...
```

---
## \#2 Posted by: i2oadsweepei2 Posted at: 2017-11-10T12:32:54.719Z Reads: 207

```
My gt2b won't do it. Nor would my mini remote. I use the nano-x and it seems to work fine for letting a friend try. I never let anyone else try my boards. I think the only other way is to use an app to switch modes. Perimetr app from metr.at and also ackmaniacs app can switch modes I think. There are a few other apps around too. I don't know much about the others though.
```

---
## \#3 Posted by: DavidBanner Posted at: 2017-11-10T12:35:16.416Z Reads: 201

```
thanks @i2oadsweepei2

My guy is being told that the Focbox can do this with any remote on standard firmware. Would love to know how this is done...
```

---
## \#4 Posted by: i2oadsweepei2 Posted at: 2017-11-10T12:40:22.105Z Reads: 190

```
I guess it's possible using a full sized fully programable remote. But ewwww. Maybe some kind of arduino remote?
```

---
## \#5 Posted by: tueboard Posted at: 2017-11-10T13:36:40.394Z Reads: 176

```
the benchwheel remote has 2 speed modes and doesn't need any special vesc settings, i found it useful if you want to let other people try your board.. but maybe the slow mode is too slow and i don't know if there is any way to change it...
```

---
## \#6 Posted by: DavidBanner Posted at: 2017-11-10T13:41:27.193Z Reads: 168

```
@tueboard exactly how I imagined the Nanox doing things, i.e. via PPM levels, not switching modes or settings in the FOCBOX
```

---
## \#7 Posted by: egzplicit Posted at: 2017-11-10T13:45:02.910Z Reads: 169

```
Can confirm nano x does this. In slow mode it ramps PPM to 70% ish when full throttle so everything is a lot slower. Good mode when you give the board to somebody for a first try until they get used to it.
```

---
## \#8 Posted by: Esk8HubsUS Posted at: 2017-11-10T14:02:13.592Z Reads: 163

```
Ackmaniac 3.10 firmware + Bluetooth Module + VESC Monitor app (for Android) =. you can set "modes" in which you can set different motor/battery min/max levels ,  eRPM level (top speed) , and other things on each ... here's a link:

https://www.electric-skateboard.builders/t/vesc-monitor-android-app/20888

If you need it to work via remote,  then the new Maytech remote has the ability to limit to 70% throttle (slow mode) ,  as people have mentioned above .
```

---
## \#9 Posted by: DavidBanner Posted at: 2017-11-10T14:06:20.152Z Reads: 150

```
Thanks @Esk8hubsUS :)

I did know about Ackmaniac's amazing firmware but I am really just trying to confirm my suspicion that it can't be done on standard FOCBOX firmware. Flashing the firmware will void the warranty which could be an issue for some folks.
```

---
## \#10 Posted by: Esk8HubsUS Posted at: 2017-11-10T14:09:43.516Z Reads: 150

```
Ahhh yes,  makes sense.   in that case you could definitely just find a remote that allows for different throttle limiting "modes" ,  like the new Maytech remote ... not a very granular option ,  but it's something
```

---
## \#11 Posted by: DavidBanner Posted at: 2017-11-10T14:10:36.616Z Reads: 145

```
personally I have no issue with flashing firmware,but for folks on a first build I really don't want to send them down that particular rabbit hole just yet :slight_smile:
```

---
## \#12 Posted by: tueboard Posted at: 2017-11-10T22:05:17.600Z Reads: 125

```
interesting, i didn't know that the new maytech remote has this feature
https://www.youtube.com/watch?v=RNMQNL7_oiM
```

---
## \#13 Posted by: nige Posted at: 2017-11-11T02:53:24.781Z Reads: 110

```
I would like modes like on the evolve board which I think limit the amps to the motors or something.You still get the same speeds just the way it gets there is less torquay.I hope this is possible even if it means changing on my phone through a blue tooth app this is still ok for me lol
```

---
## \#14 Posted by: Esk8HubsUS Posted at: 2017-11-11T04:23:50.064Z Reads: 103

```
https://www.electric-skateboard.builders/t/vesc-monitor-android-app/20888
```

---
## \#15 Posted by: Okami Posted at: 2017-11-11T09:28:29.950Z Reads: 98

```
Ive heard by modding remote with resistors in line with potentiometer, it is possible. Though havent done myself but in theory thats how its done.
```

---
## \#16 Posted by: Riako Posted at: 2017-11-11T10:20:02.875Z Reads: 98

```
Sorry for this cross-post but @tueboard : it work pretty well, and led for remote battery voltage + skateboard battery voltage info is so cool and simple to tcheck now with one led for itch ! And you get reverse mode (same with slow and fast mode). 
https://youtu.be/uS7HnNrTmts
```

---
