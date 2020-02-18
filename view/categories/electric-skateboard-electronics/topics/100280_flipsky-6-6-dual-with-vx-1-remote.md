# Flipsky 6.6 dual with VX 1 remote

### Replies: 17 Views: 398

## \#1 Posted by: eboardnewb Posted at: 2019-08-14T17:59:11.616Z Reads: 112

```
I am having difficulty connecting my Flipsky Dual FSESC 6.6 to the VX 1 remote. Each time I contact Flipsky I get a different answer.
 So far the total is 3![6%20w%20VX1|666x500](upload://bVpfKmnXXvjzjG8mun81g7uMfSZ.jpeg)
```

---
## \#2 Posted by: pundahh Posted at: 2019-08-14T18:46:30.749Z Reads: 99

```
All three options are correct. 
- Option 1 & 2 run the remote in ppm input, only difference is the voltage reader (blue wire) to use the board battery display on the remote.
- Option 3 runs through UART. 

I presume you've paired the remote to the receiver right?
```

---
## \#3 Posted by: eboardnewb Posted at: 2019-08-14T19:06:17.502Z Reads: 96

```
I've done nothing yet. I am awaiting batteries and want to be ready when they arrive.

Ok, when you say Board Battery you mean the status or level of the battery to display on the remote?

I do want that, so I should connect the blue wire to V on the receiver and the other end to main power on the board?
```

---
## \#4 Posted by: pundahh Posted at: 2019-08-14T19:16:48.552Z Reads: 87

```
Gotcha, I run PPM myself since I use a bluetooth module in the UART port. 

Board battery I mean the battery display on the remote (four dots). remember to set it up to your battery's voltage. 

Yep, connect blue to V on receiver and solder the other end to a positive wire somewhere in your circuit. Mine is on the positive coming out of my battery just before the xt splitter.
```

---
## \#5 Posted by: eboardnewb Posted at: 2019-08-14T19:34:49.206Z Reads: 81

```
Thank-you so very much!  Could you please explain the UART vs PPM?
```

---
## \#6 Posted by: pundahh Posted at: 2019-08-14T19:44:52.319Z Reads: 80

```
Just two types of vesc input. Most people (afaik) use PPM & since UART does telemetry stuff (i.e: davega, bluetooth module, remote with screens, etc). For the VX1 you'd miss out on the cruise control and reverse on the remote. All other features (ex. input, batt reading, speed modes) work fine. 
- reverse can also be implemented if you use ackmaniac firmware, so technically you'd only miss out on the cruise control.
```

---
## \#7 Posted by: eboardnewb Posted at: 2019-08-14T20:08:30.678Z Reads: 73

```
I certainly appreciate you sharing your knowledge. Because this is my  first build I am going to have questions that I need help with is it ok if I consult your expertise as things come close to completion?

I have questions like "Do I need to connect motor wires in any specific order?

I have  a 12s 2 p pack coming from Alien. It consists of 2x 6s 10,000mah packs and a 12s BMS.

When it gets here I would like your help in assembling it.Please!
```

---
## \#8 Posted by: pundahh Posted at: 2019-08-14T20:23:31.122Z Reads: 68

```
No prob! I'm happy to help with whatever I know (and so are others here & on the  form). Can't say I'll be much help with the battery though ._. Questions thread on the  forum is very helpful too :slight_smile: Good luck!
```

---
## \#9 Posted by: eboardnewb Posted at: 2019-08-14T21:08:51.715Z Reads: 57

```
Thank-you!
```

---
## \#10 Posted by: xsynatic Posted at: 2019-08-15T12:21:26.963Z Reads: 53

```
With the VX1 via PPM you still have Cruise control. Only Reverse is lost.

@eboardnewb
```

---
## \#11 Posted by: eboardnewb Posted at: 2019-08-15T15:35:37.379Z Reads: 46

```
I can do without reverse, cruise control is probably cool tho. Thank-you.
```

---
## \#12 Posted by: pundahh Posted at: 2019-08-15T15:51:22.218Z Reads: 44

```
Interesting! I’ll have to try it out then, never bothered & thought it was limited to uart. Thanks!
```

---
## \#13 Posted by: Blacksambo Posted at: 2019-08-16T01:32:41.723Z Reads: 26

```
Can you run the blue wire (Example 1) from the receiver to the red terminal on the VESC as is shown in Example 2 with the white wire?
```

---
## \#14 Posted by: pundahh Posted at: 2019-08-16T01:46:43.481Z Reads: 26

```
Yeah, you can run the voltage wire to any positive wire in your circuit. I wouldn't do it there exactly just because I'm shit at soldering & I'd like to avoid the esc as I can.
```

---
## \#15 Posted by: Randy_bobandy Posted at: 2019-08-16T07:53:45.028Z Reads: 25

```
So you only can run reverse in uart? If I have a bluetooth module in uart can I use my remote in the other uart slot on the other side of the duel vesc?
```

---
## \#16 Posted by: xsynatic Posted at: 2019-08-16T09:38:44.024Z Reads: 26

```
Correct. Reverse only in UART. You can use both yes. You just need to program it like that. I used to do that too. Remote via UART in the Master and Metr pro via UART in the slave.

Or use PPM if you don't care about reverse and plug the module in the master too.
```

---
## \#17 Posted by: Randy_bobandy Posted at: 2019-08-16T19:01:29.605Z Reads: 22

```
I have always used ppm, but I would like to try reverse out and see how I like it. Sometimes in narrow areas where turning is tight using reverse could be nice.
```

---
