# Help with VESC, no motor detection

### Replies: 5 Views: 343

## \#1 Posted by: MaddMarkk Posted at: 2017-05-08T13:48:46.389Z Reads: 44

```
I guess I did a poor job of setting it up but it worked for 2 days, my VESC came with 5.5mm bullet connectors and the motor i have uses HXT, so I just soldered in a female HXT into the female 5.5mm bullet, it worked and it did heat shrink everything but one of the solder joints was bad and one came undone and I think this caused a short. My board died mid ride for what I thought was dead batteries until I saw the bad joint. Before that I was able to fully program the vesc and everything, but now I can connect to it with BLDC tool but the motor detection fails every time. The green and blue lights are also lit but the 3 flashes from the red light don't happen anymore, I only see the red flash when I power it off. Is there some sort of debugging tab, @torqueboards suggested I try and see if it's the DRV chip but I'm not seeing any where that states that. Any help is greatly appreciated!    

this is my set up
Two 5S 5000mAh lipos in series 
Turnigy 245KV 2700W
On/Off switch from http://
the VESC is also from diy
```

---
## \#2 Posted by: MaddMarkk Posted at: 2017-05-08T13:52:50.318Z Reads: 44

```
I forgot to add that I know the motor is functional, I tested it with a hobbyking ESC and it works.
```

---
## \#3 Posted by: Blasto Posted at: 2017-05-08T14:48:56.186Z Reads: 39

```
[quote="MaddMarkk, post:1, topic:22636"]
The green and blue lights are also lit but the 3 flashes from the red light don't happen anymore
[/quote]

the 3 red flashes happen only during power or if the vesc is throwing a fault code.

To see if you have a fault code, run a motor detection (detection fail?) go in the Terminal tab and type "faults"

 If you have 1 bad solder joint, chances are that they are all bad, post pics of your setup, use flux when soldering.
```

---
## \#4 Posted by: MaddMarkk Posted at: 2017-05-08T16:13:22.264Z Reads: 30

```
 [quote="Blasto, post:3, topic:22636, full:true"]
[quote="MaddMarkk, post:1, topic:22636"]
The green and blue lights are also lit but the 3 flashes from the red light don't happen anymore
[/quote]

the 3 red flashes happen only during power or if the vesc is throwing a fault code.

To see if you have a fault code, run a motor detection (detection fail?) go in the Terminal tab and type "faults"

 If you have 1 bad solder joint, chances are that they are all bad, post pics of your setup, use flux when soldering.
[/quote]
"No faults registered since startup":confused: 
Also during power up/ turning on the red light does not flash like it did before it stopped working
```

---
## \#5 Posted by: Gizmo Posted at: 2017-05-08T22:53:57.576Z Reads: 19

```
I have two DIY vescs that are doing (or not doing) the exact same thing. They worked, started acting weird, now they don't seem to register as working. Power is getting to the BT receiver but the red lights aren't blinking and the BLDC tool isn't seeing them.
```

---
