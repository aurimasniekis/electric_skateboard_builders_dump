# Something is going on with my board and its made it really dangerous to ride. HELP

### Replies: 10 Views: 1223

## \#1 Posted by: nick.schweng Posted at: 2016-10-17T17:17:59.902Z Reads: 166

```
My board has been running great since I made it until now. I have: 
- Dual rear wheel Enertion motors
- Dual VESCs connected via canbus
- Dual 22.2 Volt, 10000 mAh batteries
- Torqueboards 2.4 ghz micro remote and receiver

This issue just started last night. For some reason, when my board is accelerating, it seems like the brakes on the board go on and the motors seize up. The batteries are charged above the battery cutoff start that I programmed on my VESCs. Could it maybe be the remote? I'd never had an issue with it, but it's still a possibility. 

I uploaded a couple clips of it not working to youtube here: 
https://www.youtube.com/watch?v=WhKDfwBzo30
https://www.youtube.com/watch?v=Qw_5ma51AFg&feature=youtu.be

As you can see, once I get going the brakes appear to go on, even though I'm not  touching the brake button on the remote. This is making it really dangerous to ride because I get thrown off the board. Any advice would be greatly appreciated!
```

---
## \#2 Posted by: JohnnyMeduse Posted at: 2016-10-17T18:13:22.039Z Reads: 145

```
Sound like your trim button as been touch and now you need to re-calibrate you remote.
```

---
## \#3 Posted by: JohnnyMeduse Posted at: 2016-10-17T18:16:54.905Z Reads: 143

```
http://www.electric-skateboard.builders/t/vesc-faq-setting-up-receiver-and-brakes/244
```

---
## \#4 Posted by: mishrasubhransu Posted at: 2016-10-17T18:30:18.226Z Reads: 136

```
What's up with clickbaity title?

BTW. New motors? or old one. There might be a short inside the motors. There is a fix for it.
```

---
## \#5 Posted by: nick.schweng Posted at: 2016-10-17T18:55:24.747Z Reads: 131

```
I've only had the motors for about two months. Do you have any links or advice on motor shorts that I could look at?
```

---
## \#6 Posted by: Hummie Posted at: 2016-10-17T21:23:53.596Z Reads: 109

```
someone said trim.  did you possibly adjust the knobs on the remote?

actually now having watched the video sounds shorted.  you can check on the vesc tool
```

---
## \#7 Posted by: GeorgeKing Posted at: 2016-10-18T11:26:44.661Z Reads: 74

```
I had the same problem just last week. I had just put in some nice polyurethane foam to cushion my VESC and this happened after the test ride. I quickly removed the foam, wrapped the VESC in insulation tape and hot glued everything down. Been working fine ever since. But, I have absolutely no idea why. I can't imagine that it would be the polyurethane foam causing the short so I figured perhaps it was the foam blocking the signal to the remote or possibly causing some wires to come loose.

Either way, once the foam was removed, all was working perfectly, i took the board on a massive 30km test run which included quite few hills and lots of dust and dirt and bumps and it worked flawlessly the whole time. No problems with losing signal or overheating. 

So confused right now.
```

---
## \#8 Posted by: Monte Posted at: 2016-10-18T17:21:51.926Z Reads: 45

```
I think i know why. Non-sensored motors should never start from 0 rpm with load. I had this once when a friend tested my board and not pushed. My board just went crazy and tried to kill him. :sweat_smile: You just need to push once in your beginning or driving. Everytime.
Thats why its shuttering so hard when you start to drive.
```

---
## \#9 Posted by: Monte Posted at: 2016-10-18T17:43:20.380Z Reads: 41

```
I personally believe it has to do something with the motor detection. Maybe the Vesc 'think' the motor is already spinning because it gets wrong information.
```

---
## \#10 Posted by: Hummie Posted at: 2016-10-18T17:57:52.146Z Reads: 39

```
@GeorgeKing
maybe you were squeezing the vesc and forcing a pin through a wire.  had that happen.
```

---
