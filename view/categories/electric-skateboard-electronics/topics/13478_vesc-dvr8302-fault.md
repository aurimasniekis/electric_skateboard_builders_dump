# VESC DVR8302 Fault

### Replies: 19 Views: 2274

## \#1 Posted by: tonys Posted at: 2016-11-22T16:55:05.267Z Reads: 179

```
I fear my VESC died. This my my 3rd VESC. I originally purchased 2 from . One worked perfect upon motor detection and the second never could be detected. After much conversation with Dexter he sent me a replacement at the cost of the warranty $60 + $10 for shipping. The replacement worked well for about 20 miles when the motor it controlled (I'm running dual motors/VESC's) would intermittently lock without warning then after a few seconds start running again. Wasn't bad at first but problem became more and more frequent until yesterday when it did some funky things, stop start stop start then died. It was a slow painful death. I did the walk of shame home with board in tow and proceeded to run the VESC on the BLDC tool. Blue lights then 3 red lights flashed. When I ran motor detection the red lights flashed and got the DVR8302 fault. Any ideas what happened? Is there a fix? If not should I take my chances with another VESC from DIY electric skateboard or go for one from @chaka Ollin. Some on here seem to like the quality of Ollin better. Thanks in advance for any help. You can see my build in previous posts.
```

---
## \#2 Posted by: Jinra Posted at: 2016-11-22T17:01:52.979Z Reads: 170

```
Can you post your VESC settings?
```

---
## \#3 Posted by: tonys Posted at: 2016-11-22T18:52:04.970Z Reads: 159

```
Sure. I'm running dual VESC and dual 192kv motors powered by (2) 5s LiPo batteries.<img src="/uploads/db1493/original/3X/f/f/ffc6f17aa7afb29a5d85b7dad5a6c4d23f990e84.jpg" width="690" height="363">
```

---
## \#4 Posted by: Jinra Posted at: 2016-11-22T19:09:45.627Z Reads: 146

```
thanks, Bldc and app config tabs as well would be helpful
```

---
## \#5 Posted by: tonys Posted at: 2016-11-22T19:19:17.972Z Reads: 143

```
<img src="/uploads/db1493/original/3X/6/f/6f132b4c3b01862bb83235df981d28142889d8d5.jpg" width="690" height="363"><img src="/uploads/db1493/original/3X/2/c/2cdad7673b1f2a62b777748cb74b276b84edb075.jpg" width="690" height="365">
```

---
## \#6 Posted by: Jinra Posted at: 2016-11-22T19:27:10.372Z Reads: 140

```
Is 62 the detection result you got initially for the integrator limit? Seems kind of low. Can you show your advanced tab as well?
```

---
## \#7 Posted by: tonys Posted at: 2016-11-22T19:46:37.161Z Reads: 146

```
Not sure when I got the 62 reading. Here's the Advanced Tab<img src="/uploads/db1493/original/3X/0/2/027eaa77f5a7e7ec1006bffeffb22d8760ced5d2.jpg" width="690" height="363">
```

---
## \#8 Posted by: Jinra Posted at: 2016-11-22T19:48:40.568Z Reads: 145

```
Ouch so you got the bugged firmware. You'll need to reflash it if you decide to repair this one. Notice your max current ramp step is at 50.00. Default is .04. It'll multiply itself by 10 every time you write config. Reflashing newest firmware will fix this. See here for details:

http://www.electric-skateboard.builders/t/psa-remember-to-reset-your-max-current-ramp-step-when-programming-your-vesc/6262

I'm guessing that's whats been causing your VESC to blow. Make sure you verify Int limit and BEMF coupling when you get your new VESC.
```

---
## \#9 Posted by: tonys Posted at: 2016-11-22T20:01:58.520Z Reads: 133

```
Thanks so much! Ahhhh I was totally unaware of that regarding Max current ramp step. What should the correct Int limit and BEMF readings show?
```

---
## \#10 Posted by: Jinra Posted at: 2016-11-22T20:05:20.575Z Reads: 130

```
You have to do motor detection to find out
```

---
## \#11 Posted by: tonys Posted at: 2016-11-22T20:21:59.202Z Reads: 130

```
Just wanted to clear something up. Appreciate your patience and help. When I run the motor detection do I input the Detection results into the above fields. In this case I would change the BEMF from 600 to 900.28 and the Int limit from 62 to 104.77 (rounded out) by clicking on apply correct? This is from my working VESC<img src="/uploads/db1493/original/3X/a/a/aaf3220c41e878758b646acafeb8f4c110b80be2.jpg" width="690" height="361">
```

---
## \#12 Posted by: Jinra Posted at: 2016-11-22T20:58:29.871Z Reads: 120

```
When you click apply it should round int limit down to nearest 5 and bemf coupling to nearest 50. But yes, that's pretty much correct.
```

---
## \#13 Posted by: rpn314 Posted at: 2016-11-22T22:08:42.607Z Reads: 117

```
Just be careful of the firmware download source. I thought I'd gotten the "newest" one and ended up with blowing a drv chip. Thankfully I'd ordered extras when I originally soldered them, and had the ability to repair it myself. I'm positive that's what blew mine (slowly, just like yours) cause every other setting was just fine.
```

---
## \#14 Posted by: Rollbrett Posted at: 2017-01-15T22:43:59.036Z Reads: 96

```
Is this confirmed, does the "Max Current Ramp Step" bug actually fry the DRV?
I followed the VESC config process from eSk8.de and thats the only reason I even touched the advance settings. Expensive hobby -_- 

I was using a VESC 4.12 with FW 2.18 from DIY-ES and downloaded the BLDC Tool from http://vesc.net.au/BLDC-TOOL/OS%20X/ (15-Aug-2016 01:37)

What exactly caused this problem?
The FW on the VESC or the BLDC Tool?

And how much is a reasonable price to get the DRV fixed?
```

---
## \#15 Posted by: rpn314 Posted at: 2017-01-16T18:24:21.736Z Reads: 87

```
It can, but it doesn't always.

It was an issue with the firmware on the VESC. Vedder resolved it long ago, but there are a few downloads floating around that have it. You can see if you have it in BLDC tool by reading and writing a few times. If your Max Current Ramp Step value increases by a factor of 10 each time you write and then read back, then you have the bug and you should re-flash the firmware with a new one from a different source.. Otherwise you're fine.

I don't actually know a good price for a fix. I'd probably charge like $15-20.
```

---
## \#16 Posted by: Idobartal Posted at: 2017-02-14T15:02:15.006Z Reads: 72

```
Im having a problem with my vesc
i have a Vedder 4.12 from diyelectricskateboard, after a couple of Nice rides i bumped into the pavement.. the skateboard Still works fine but every once in a while i dont get Any reaction from the motor when i press the remote. After connecting it to my mac and checking faults on bldc tool I found out that i have the drv8302 error, but the thing is that the eskaye still works fine.. the error isnt so common and it feels ok To ride it, i do feel some motor twitches and no throttle control but its not so frequent..
is that possible that a drv832 fault is coming and going ?... isn't it a 'fatal' vesc error???
**
My setup:

Turnigy Sk3 6374 168kv
6s (2* 3s 5000mah batteries connected in series)
Maybe some Vesc pics will bring up some ideas?
<img src="/uploads/db1493/original/3X/a/7/a7203944eb43b06a277f2d4ec2d8f95d7d3f6c35.JPG" width="375" height="500">
```

---
## \#17 Posted by: tonys Posted at: 2017-02-14T15:40:27.512Z Reads: 66

```
I had the exact same problem. The situation gets progressively worse until the VESC completely dies. I would replace it now as it could get dangerous if the motor locks up when you're cruising at a high speed (which mine did) I also purchased mine from diyelectricskateboard. Not saying they sell defective products but I had 2 from them that malfunctioned. I now use another vendor and so far working flawlessly. Also check your firmware. It may be the buggy one. If it is you need to update it asap: http://www.electric-skateboard.builders/t/psa-remember-to-reset-your-max-current-ramp-step-when-programming-your-vesc/6262
```

---
## \#18 Posted by: Idobartal Posted at: 2017-02-14T15:59:03.850Z Reads: 65

```
Thx so much man... although you had bad news for me and my vesc it's comforting to know you're not alone with your situation so thx again...
I have just ordered a new vesc two days ago from "faraday motion UG", if you know something about them or their product feel free to tell me.. 
one thing that concerns me is the 'capacitor' dilemma... i see alot of vescs out there on the internet, most of them has three capacitors on the top, as my diyelectricskateboard has...
The new one I ordered from 'faraday motion' has only one big capacitor.. i dont really know what it means and weather it should concern me...
Thx for any help
Ido
@tonys
```

---
## \#19 Posted by: tonys Posted at: 2017-02-14T16:32:25.716Z Reads: 63

```
Sure thing. Not familiar with Faraday but looking at their website they have some cool stuff. I used Ollin Electric Skateboard  to replace my defective VESC. It's expensive when u add the warranty from them  but even more expensive when you have to pay full price to replace a defective one. Maybe someone with more knowledge can comment on the Farady VESC.
```

---
