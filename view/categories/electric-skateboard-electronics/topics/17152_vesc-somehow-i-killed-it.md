# VESC, somehow I killed it

### Replies: 10 Views: 1399

## \#1 Posted by: mmaner Posted at: 2017-02-03T16:30:11.808Z Reads: 152

```
Sooooo I killed one of my MEB VESC's.  I do not know what I did or if it was just one of those things.  I am sending it back to @oriol360 at [Miami Electric Boards](https://miamielectricboards.com/) for him to look at, he a rock star so I'm sure he can tell me what happened. 

Now, I am using 1 MEB VESC and 1 DIY VESC.  I would appreciate it if you guys could take a look and make sure I haven't flubbed anything in the config, screen shots below.  I am really not sure about the MAX WATT (@Ackmaniac).  I am running x2 190KV 6355 motors from DIY on 6s. 

thanks

VESC #1 (MEB)
<img src="/uploads/db1493/original/3X/0/a/0af2f2b6cf7db4fcafd9547bf422185c13bfe872.JPG" width="690" height="389">
<img src="/uploads/db1493/original/3X/a/7/a714c7f2d35cf28220a1575306a021a42e48aae9.JPG" width="690" height="389">
<img src="/uploads/db1493/original/3X/0/4/042f18a87dd0ab60dbc8e4f3edc4dccc5f24d366.JPG" width="690" height="389">
<img src="/uploads/db1493/original/3X/6/2/6227ac7934ef4384246d883a6eb2c0274a7b35b7.JPG" width="690" height="389">

VESC #2 (DIY)
<img src="/uploads/db1493/original/3X/b/a/ba8b7daec2551117b22c726cf3daf67067e1da2c.JPG" width="690" height="389">
<img src="/uploads/db1493/original/3X/8/3/83638d7344e67a4b5b90c16fc73ab2512c9d95ed.JPG" width="690" height="389">
<img src="/uploads/db1493/original/3X/e/b/ebca517f7ae141b3a04d30feddffbaca82249f24.JPG" width="690" height="389">
<img src="/uploads/db1493/original/3X/1/9/19b968eec39fa8ee4bdb159873888bc20ae22f8d.JPG" width="690" height="389">
```

---
## \#2 Posted by: Ackmaniac Posted at: 2017-02-03T18:53:50.096Z Reads: 118

```
I can see already one mistake that you made.
After the motor detection you changed the Int Limit Min ERPM instead of the BEM Coupling. But i ma not sure if this was the cause for the failing VESC. But it could be. 
So to run the motor detection the correct way you have to press the "Start detection" Button and afterwards the "Apply" Button. By pressing the apply you will see that the Integrator Limit and the BEMF coupling will change automatically. In you case those values will be 105 and 800 if the detection result is the same. Strangely many people change these values manually.
Set the "Int Limit Min ERPM" to the default 1100 value and write the settings before the Motor detection.

<img src="/uploads/db1493/original/3X/d/b/db1cee3fbfa11cd412760c8026969a0cc573b8fd.jpg" width="690" height="377">

And you need to adjust your PPM settings. Just use the autowizard and follow the instructions. Then it will be fine.

Next is that you told both VESCs to be the Master. The one that has the receiver cable connected should be the Master:
ControllerId = 0
Send status over CAN = no
Multiple ESCs over CAN = yes
Enable traction control = yes
Controller = PPM or PPM and UART (if bluetooth module is connected)
Control mode = watt no reverse with brake

The other should be defined as Slave:
ControllerId = 1
Send status over CAN = yes
Multiple ESCs over CAN = no
Enable traction control = no
Controller = None or PPM (if you want to use the secondary channel of the remote for cruise control, in that case also the PPM pulsewidth needs to be adjusted and "Cruise Control via secondary Channel" should be selected)
```

---
## \#3 Posted by: mmaner Posted at: 2017-02-03T19:04:31.185Z Reads: 108

```
These aren't the actual setting I ran, just what I plugged in while trying to see what happened.  I actually noticed the BEMF COupling mistake a bout 2 minutes ago, Ill correct that before I actually run the VESC's.

I am confused about the statement "you told both VESCs to be the Master".  

---
On VESC #1 I have...
<img src="/uploads/db1493/original/3X/e/b/eb7423a510706d9e32c3abd4602a804e82054cdb.jpg" width="634" height="222">
---
On VESC #2 I have...
<img src="/uploads/db1493/original/3X/1/7/17dd7666704591774c321262cbdc980d8b45cae7.jpg" width="594" height="217">

---
In WATT Settings, what MAX Watt value should I use?
<img src="/uploads/db1493/original/3X/3/e/3e502f778d574539b5e59601e2ebb83093c21db7.jpg" width="690" height="61">
```

---
## \#4 Posted by: Ackmaniac Posted at: 2017-02-03T19:11:03.671Z Reads: 104

```
Just have a look here

http://www.lp-electronic.com/vesc/connect-two-vesc-via-can-bus/

or here

http://www.electric-skateboard.builders/t/vesc-faq-connect-two-vesc-via-canbus-for-dual-motors/142
```

---
## \#5 Posted by: mmaner Posted at: 2017-02-03T19:33:57.334Z Reads: 99

```
I see, I had the Multiple ESCs over CAN option ticked on both, makes sense now.  

How do I figure the MAX Watt value?  I understand that **Max Watt = Max Current * Battery Volts**, I don't understand Max Current, at least not fully.

As I understand it, to get Max Current (Max Discharge?) you use the following...
Max Current = C Rating x Capacity
With my x2 8000mah 30c Lipo packs I would have the following value?
30c * 8k mah = 240a * 2 Packs = 480a

Then if MAX Battery Current * Battery Volts = MAX Watt I would use the following values...
480a * 22.2v = 10,656 Watts

Does that look correct?
```

---
## \#6 Posted by: Ackmaniac Posted at: 2017-02-03T21:10:40.252Z Reads: 89

```
With 10656 at each motor i wish you a good flight.

To use the maximum potential of your motor settings you should calculate battery max * 3.6V * cells in series

So in your case it is 60A * 3.6V * 6S = 1296W

If you want to use more you also need to raise the battery max.

But on the other side you can also lower the max watts and leave the battery max. This way you can simply adjust the battery max to the maximum the battery can handle and adjust the maximum power simply with the max watt value.
But don't go crazy with the battery max. 60A is already relatively high.
```

---
## \#7 Posted by: mmaner Posted at: 2017-02-03T22:23:18.265Z Reads: 78

```
[quote="Ackmaniac, post:6, topic:17152"]
battery max * 3.6V * cells in series
[/quote]

That makes much more sense, I certainly dont wanna fly :).  Thanks for all the help, this is pretty confusing, but I am starting to get the hang of it.
```

---
## \#8 Posted by: Ackmaniac Posted at: 2017-02-03T22:40:16.464Z Reads: 73

```
in my latest version of the modded BLDC-Tool (2.53) you also get a lot of hints in the tooltips when you hover with the mouse over the parameters name.
```

---
## \#9 Posted by: Okami Posted at: 2017-02-03T22:42:21.681Z Reads: 73

```
As I said, I think this should be pointed out in the app itself, if possible! Im not sure does all of the people know about this ''function'' yet :D 

@mmaner Im sorry for your loss.. I hope Miami boards will get it sorted out, if it is repairable :)
```

---
## \#10 Posted by: mmaner Posted at: 2017-02-03T22:44:09.750Z Reads: 71

```
[quote="Okami, post:9, topic:17152"]
I hope Miami boards will get it sorted out, if it is repairable
[/quote]

Me too, but @oriol360 has always been great.
```

---
