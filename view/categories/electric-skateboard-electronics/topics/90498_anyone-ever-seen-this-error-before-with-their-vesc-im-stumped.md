# Anyone ever seen this error before with their VESC - I&rsquo;m stumped

### Replies: 3 Views: 263

## \#1 Posted by: Jansen Posted at: 2019-04-14T15:05:23.112Z Reads: 83

```
Ok, I have tried everything fellas. Here's the deal....

Build number 3.5, have learned a lot and gotten good at diagnosing my issues. I am using 2 focboxes that I have been using and just switched them over to a new build which is a 10s4p 30q, flipsky antispark, 2 focboxes, bms, TB 6355 on surfrodz with 6shooters (w/ quick66 mounts) on the new evo deck with other little things) so I go to plug in first VESC to run motor detection (running split PPM with nano-x mod) and it connects fine for a second then I get to motor detection and I get this error

"serial port error: the semaphore timeout period has expired"

I can't get VESC to reconnect at all. I'll shut everything down, restart comp, and every once in a while I will get them to reconnect but then after a few minutes sane thing.... I've tried....

- updated drivers
- different cables
- different computers (a surface and a dell desktop both on windows 10)
- having board on and plugged in when I open the VESC tool
- Not having board on when opening VESC tool
- I tried @CarlCollins from Enertions fix I found and that let it work at first, but still error'd iut after a few minutes into the set up
- Searched the forms up and down the last 24-48 hours and tried every potential fix I can find but nope.

HELP.

Oh and running @Ackmaniac 3.1 firmware and using the VESC tool (not the 2019 one) 

See PIC and hope someone can help so I can make my group ride later today. 

![58|666x499](upload://aPSxFtFgqHotUYHW1YTRSk8U8zd.png)
```

---
## \#2 Posted by: sayekim Posted at: 2019-04-16T14:44:51.027Z Reads: 42

```
Have you tried both motors/focboxes?

Never seen this error before.
```

---
## \#3 Posted by: queruvin05 Posted at: 2019-10-07T14:47:18.863Z Reads: 23

```
Alright i got the same problem and i found the solution for it  for some reason it seems that the vesc didn't know which usb port to connect to.

Just turn off windows bluetooth then got to Device manager  look for the ports (com & lpt) uninstall all of them after that remove all the connected usb from the pc restart the vesc tool re unplug the vesc connection then it should work then. Worked for me i'm not 100% sure if it will work for the others
```

---
