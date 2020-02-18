# Programming/VESC/Kick Assist

### Replies: 19 Views: 1169

## \#1 Posted by: Jreamer Posted at: 2017-09-28T05:01:27.075Z Reads: 168

```
Can you program the VESC to kick assist like the mellow board with their endless ride mode?
Such a cool feature, would love to implement it on my boards in the future.
```

---
## \#2 Posted by: JdogAwesome Posted at: 2017-09-28T05:04:36.805Z Reads: 167

```
Technically there's no reason why you wouldn't be able to program such a feature into the VESC though it isn't an implemented in any current release of the VESC firmware and you'd have to code it yourself.
```

---
## \#3 Posted by: Jreamer Posted at: 2017-09-28T05:12:37.043Z Reads: 163

```
Would it be hard to do? I am not getting my raptor 2 till the second batch, so won't be able to work on it soon anyway, might as well learn now.
```

---
## \#4 Posted by: scepterr Posted at: 2017-09-28T05:14:43.263Z Reads: 162

```
If you have to ask, usually the answer is yes 😉
What languages are you familiar with?
```

---
## \#5 Posted by: Jreamer Posted at: 2017-09-28T05:23:35.446Z Reads: 157

```
English, and not that well :)
```

---
## \#6 Posted by: scepterr Posted at: 2017-09-28T05:24:04.801Z Reads: 151

```
LMAO, programming languages....
```

---
## \#7 Posted by: Jreamer Posted at: 2017-09-28T05:38:50.258Z Reads: 153

```
I know, just not a programmer. Is it something that could be done with the android app?
```

---
## \#8 Posted by: scepterr Posted at: 2017-09-28T05:40:31.847Z Reads: 160

```
No, you need to either modify the firmware or write an addition to it.
You would also need to write your own Android app if you wanna tweak your modification/addition on the go
```

---
## \#9 Posted by: Cobber Posted at: 2017-09-28T06:57:45.697Z Reads: 150

```
@lowGuido made a[ push assist board](http://www.electric-skateboard.builders/t/low-guidos-hack-board-for-science-now-with-hub-motors/870/42)

https://youtu.be/8-8bFOhcSck
```

---
## \#10 Posted by: Paulf Posted at: 2017-09-28T11:17:20.201Z Reads: 134

```
I do think that this feature is available in Ackmaniac's 2.54 firmware
```

---
## \#11 Posted by: GrecoMan Posted at: 2017-09-28T11:19:16.584Z Reads: 126

```
Yea what about @Ackmaniac’s PID No Acceleration?

I’ve tried to set it up before but with no success
```

---
## \#12 Posted by: Paulf Posted at: 2017-09-28T16:07:28.829Z Reads: 103

```
I've successfully set it up, it works juste as you'd expect for me, kick push and then it'll keep your speed as long as you push the throttle on your remote (but you could easily add some kind of pedal on your board to get rid of the remote)
```

---
## \#13 Posted by: Jreamer Posted at: 2017-09-28T18:52:34.311Z Reads: 95

```
That is sweet dude. So this is programmable with the vesc. Can you use the App for it?
```

---
## \#14 Posted by: Paulf Posted at: 2017-09-29T05:08:30.255Z Reads: 83

```
Yes, you can use the app in order to switch to the mode "pid no acceleration"
```

---
## \#15 Posted by: karma Posted at: 2017-09-30T10:02:00.794Z Reads: 67

```
Very interesting, that feature let's you ride the board without a remote, only a pressure sensitive spot on the board. 
You could use [this](https://www.adafruit.com/product/166) and a arduino nano to make a pressure sensitive "remote" under the grip tape.
```

---
## \#16 Posted by: Cobber Posted at: 2017-09-30T10:17:52.317Z Reads: 63

```
and if you made it 250w limited it would confine to the manky ebike laws... but no one wants this reality!
that said, I am surprised there is not a commercial board filling this space with a big Ad budget...
```

---
## \#17 Posted by: lowGuido Posted at: 2017-09-30T10:34:26.799Z Reads: 62

```
you don't even need to make it that complicated. just a simple button is all you need.
I have one so small you can hardly even notice it.
```

---
## \#18 Posted by: karma Posted at: 2017-09-30T10:41:06.983Z Reads: 60

```
right you don't need to sense the pressure, only on or off for it to work. You could use something close to [this](http://www.ebay.com/itm/10pcs-4-4-0-55mm-SMD-Tact-Slim-Thin-Films-Tactile-Push-Button-Momentary-Switch-/391434353205?hash=item5b234e3a35:g:zPMAAOSwiYFXEEbZ) and you are good.
```

---
## \#19 Posted by: lowGuido Posted at: 2017-09-30T10:48:47.399Z Reads: 56

```
yeah I use something very similar to that.
```

---
