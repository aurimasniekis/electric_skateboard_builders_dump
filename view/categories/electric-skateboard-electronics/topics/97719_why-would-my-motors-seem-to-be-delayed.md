# Why would my motors seem to be delayed

### Replies: 16 Views: 213

## \#1 Posted by: Jcammarata4 Posted at: 2019-07-02T16:09:16.585Z Reads: 69

```
I have been having issues lately ..thought it was vescs..bought new flipsKY dual 6.6.....installed it on new motors 6374 149kv. Sensorless. And the battery is 10s4p ..so new vesc on new motors....they go through setup and detection ok. They seem to be delayed meaning one spins then the other will join in after a minor delay....it's not running as it should...can this be due to the quality of the soldering.....they are soldered together ok... to my assesment but I'm no expert. If it's not the vesc or motors....and theyve gone through setup and I'm still getting these odd issues like they are delayed or one runs then the other won't I'll post a vid.  I'm no expert w this stuff and I am a quick learner. I've read and tried tons of stuff but get this feeling it's the connections or the wires themselves....does it make sense to anyone.....please help.
```

---
## \#2 Posted by: linsus Posted at: 2019-07-02T16:12:46.401Z Reads: 63

```
You're running them without load and expect them to spin exactly simultaniously? You're funny :D 

Make sure slave over CAN is enabled. If you want you can enable traction control, might help with some of the paranoia
```

---
## \#3 Posted by: Jcammarata4 Posted at: 2019-07-02T16:13:15.491Z Reads: 64

```
No it does this with load
```

---
## \#4 Posted by: Jcammarata4 Posted at: 2019-07-02T16:18:53.238Z Reads: 57

```
Trust me I'm not picky I just wanna ride without fear of death
```

---
## \#5 Posted by: Jcammarata4 Posted at: 2019-07-02T16:19:19.319Z Reads: 54

```
It doesn't need perfection just reliability
```

---
## \#6 Posted by: linsus Posted at: 2019-07-02T16:26:39.576Z Reads: 48

```
well, buying from x chinese vendor + fear of death kind of goes hand in hand. 

Thats a lie, If reliability was your biggest concern you'd get trampa one. 

Like I said, make sure you enabled CAN, try traction control. Make sure the belt tension or w/e drive train you're using are as similiar as posible. Thats the only thing i can think of. The quality of soldering has nothing to do with this. If they were faulty they wouldnt spin. Unless you have any faultcodes?
```

---
## \#7 Posted by: Jcammarata4 Posted at: 2019-07-02T16:28:00.624Z Reads: 47

```
No codes but thanks that does help in my checking off crap that may be an issue dept. Does anyone live around Boston area willing to help out ...I'm willing to compensate ,drive, feed,ECT....just want this thing up and running properly
```

---
## \#8 Posted by: Jcammarata4 Posted at: 2019-07-02T16:30:47.775Z Reads: 48

```
And yes those things are checked ..can bus...traction...still happens...I was thinking there was possibly some kinda kink in the the wires somewhere that may be an issue. The thing should be running great but I don't trust it like I have in the past even though I've upgraded motors and vesc.
```

---
## \#9 Posted by: Jcammarata4 Posted at: 2019-07-02T16:33:35.991Z Reads: 43

```
Question ...you don't trust flipsky parts? I did some reading and thought it was a decent product for the money .flipsky dual 6.6 200a? I know it's preference but seems well built and I thought definitly better than what came with it...2 50a maytec super escs right??
```

---
## \#10 Posted by: Jcammarata4 Posted at: 2019-07-02T17:00:35.418Z Reads: 41

```
Could you or anyone reading this post what they think my vesc settings ought to be at roughly...for 10s4p  dual 6374 149kv on flipsKY dual 6.6 vesc. I just want some opinions from people more knowledgeable than myself...which is most everyone...please and thanks.
```

---
## \#11 Posted by: linsus Posted at: 2019-07-02T18:16:10.559Z Reads: 36

```
Settings depends alot on your batttery. I'm not super familiar with either flipsky or maytech from personal use but have seen plenty of threads where they broke or were dead on arrival. Thats enough for me to not dig more into it. 

try  instead, if u want more help not alot of ppl respond here anymore.
```

---
## \#12 Posted by: Jcammarata4 Posted at: 2019-07-02T22:41:09.883Z Reads: 28

```
Aren't all motors ...ALLA motors made in China...I mean everyone just slaps their name on Chinese motors...I don't know any American motors ..but maybe I'm wrong but further even most vescs same thing...mass produced in China with their company name on them ...so it's tough to say Chinese crap when most everything is produced there regardless of who came up with the idea....?? Idk I got my board running anyhow it was a bad connection on one motor wire it may have snapped the solder during a ride and it's all shrink wrapped so unless u tear it apart after you just put it all together it's hard to say what's the issue but thank you anyhow for the help
```

---
## \#13 Posted by: linsus Posted at: 2019-07-02T23:04:33.338Z Reads: 27

```

There is one factory that makes most of the higher quality motors. (Sk3, sk8, trampa and more)  however, it does exist handwound marvels like the hummiemotor. Not sure if thats a pro or con tho, being handwound.


Read up on the vesc project and who s behind it, just cause something is made in china dsnt dictate what quality it will hold, this is especially applicable in electronics where so many factors can be deciding factor. One of the biggest is QC control, where 90% lack the proper routines. But no. Not all vescs are made i china.

One of the biggest misstake ppl dont realise is that there is a huge difference between the vendor beeing chinese (like flipsky or maytech) and just having some production in china. The former often more notorious for cutting corners and going for cheap.
```

---
## \#14 Posted by: mishrasubhransu Posted at: 2019-07-02T23:06:12.494Z Reads: 25

```
Nothing wrong with your setup. Enable traction control.
```

---
## \#15 Posted by: Jcammarata4 Posted at: 2019-07-02T23:47:55.116Z Reads: 24

```
Thanks bud for the type of responses that are appropriate here. Sometimes you get responses from people who should clearly "say nothing if you have nothing nice to say" that's what my mommie says anyhow. Saying there's nothing wrong when clearly I have had an issue enough so to take time to post it instead of just riding you know........so thank you for your time
```

---
## \#16 Posted by: AlanZhou Posted at: 2019-07-02T23:54:40.618Z Reads: 23

```
[quote="Jcammarata4, post:12, topic:97719"]
Aren’t all motors …ALLA motors made in China
[/quote]

there are exceptions, like @Hummie 

[quote="Jcammarata4, post:12, topic:97719"]
but maybe I’m wrong but further even most vescs same thing…mass produced in China with their company name on them
[/quote]

not true, a lot of vesc have custom PCB's and components that may function better than stock 4.12's, Like the Focbox/Focbox Unity (well maybe not the unity but.... :rofl:), @chaka direct fet vesc and so on.

[quote="Jcammarata4, post:12, topic:97719"]
so it’s tough to say Chinese crap when most everything is produced there regardless of who came up with the idea…??
[/quote]

its Chinese crap when the item is proven unreliable, it is however not Chinese crap when the community has thoroughly tested the item and has proven reliable.

[quote="Jcammarata4, post:12, topic:97719"]
I mean everyone just slaps their name on Chinese motors
[/quote]

also, that's exactly true
```

---
