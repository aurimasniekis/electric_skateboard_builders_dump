# Is my VESC fried?

### Replies: 41 Views: 1847

## \#1 Posted by: LAVAMAN Posted at: 2017-12-18T18:07:53.619Z Reads: 169

```
I need some advise form you VESC experts. I followed all the instructions and end up with no motor detection and flashing red LED's. I modified the battery settings before doing motor detection. I am using 2 XT90 anti-spark connectors in my harness. One at VESC connection and one in anti-spark loop switch. I thought that would make it safe for me to configure my VESC using fully charged 6S LIPO batteries (3 x 2S in series). I don't have any additional motors etc. to swap out to get the answer to my problem. I can purchase a meter and check resistance in motor lead wires to try to eliminate the motor as the problem. I have a couple RC cars that have ESC's but I don't think I can connect my large E skate motor to one of those setups to see if the motor would run. As you can tell, I am not an electronics expert. Are there any settings I can change in the BLDC tool and re-try? Is they a way with a cheap multi-meter for me to verify if my VESC is toast? If it is DOA I just want to move on and buy another one. If so I want more advise. Do I buy a FOC Box with warranty and try again or do I buy a Olins VESC and try again? Or maybe a VESC from Miami Electric Boards? I need to hear from people with experience. Thanks in advance.<img src="/uploads/db1493/original/3X/8/5/854441bc8424e5b65301b263d4444a14aafda455.jpg" width="690" height="419"><img src="/uploads/db1493/original/3X/f/8/f83d32dae9464e4d1ad4ed769ea559c678bf4ce2.jpg" width="690" height="415"><img src="/uploads/db1493/original/3X/9/e/9ec82d19031aca059e5609305fdeed20c91827f4.jpg" width="690" height="414"><img src="/uploads/db1493/original/3X/b/1/b13dab04ace555485f354791292bc1cfbf70e595.jpg" width="690" height="417"><img src="/uploads/db1493/original/3X/0/2/0212e9c1caa5a82369295213bf8cc6894fa1f76e.jpg" width="690" height="388"><img src="/uploads/db1493/original/3X/a/8/a8eb244f944bab000480fab01e5b282eaff3fd1c.jpg" width="690" height="388"><img src="/uploads/db1493/original/3X/7/1/711cbc5dee4266ff9b5ad8e78a90855482218eb3.jpg" width="690" height="388"><img src="/uploads/db1493/original/3X/b/2/b232b56d5519e09623a70159a51d5190ef47946f.jpg" width="281" height="500">
```

---
## \#2 Posted by: yelnats8j Posted at: 2017-12-18T18:09:30.590Z Reads: 140

```

Are you doing the detection with the wheel on.
If so that's your problem you can't test it with the wheel on.
```

---
## \#3 Posted by: LAVAMAN Posted at: 2017-12-18T18:10:18.913Z Reads: 137

```
Yes belt and wheel attached.
```

---
## \#4 Posted by: yelnats8j Posted at: 2017-12-18T18:10:52.602Z Reads: 136

```
That's your problem try it without the wheel and belt it should work then.
Good luck
```

---
## \#5 Posted by: LAVAMAN Posted at: 2017-12-18T18:12:38.424Z Reads: 132

```
Sweet! They don't mention that in the Vid's on VESC configuration!

Thanks!
```

---
## \#6 Posted by: yelnats8j Posted at: 2017-12-18T18:13:46.271Z Reads: 127

```
Yeah don't tell anyone but I made that mistake was rushing and wanted to get it done and forgot to do that. Also reset any changes you made to the setting well trying to figure it out don't want and wildly incorrect values. By the way did it work
```

---
## \#7 Posted by: onepunchboard Posted at: 2017-12-18T19:31:39.921Z Reads: 117

```
u can also increas ermp by 100s
```

---
## \#8 Posted by: ThermalM16 Posted at: 2017-12-18T19:54:12.726Z Reads: 115

```
Glad you sorted it out. If you run motor detection without any motor attached and type faults in the console window, it should tell you if the DRV is bad or overcurrrent and things like that. It might be helpful for any future troubleshooting.  Good luck with your build!
```

---
## \#9 Posted by: LAVAMAN Posted at: 2017-12-19T22:50:22.161Z Reads: 94

```
I just tried to run motor detection again with belt/pulley/wheel removed and still get "failed Motor Detection". When I connect the VESC to the BLDC tool it just flashes red but it does read configuration and I can change settings etc. Now I am back to square 1. I have to figure out if VESC is fried. If all I get are red flashing LED's, does that mean I might be doing something wrong or does it mean the VESC is toast?
```

---
## \#10 Posted by: LAVAMAN Posted at: 2017-12-19T22:52:36.933Z Reads: 93

```
removing belt/pulley/wheel did not work. Where is the console window? Is that the box that gives you the values after it detects your motor? I want to try to do a motor detect with no motor attached and see if I can get fault codes.
```

---
## \#11 Posted by: yelnats8j Posted at: 2017-12-19T22:55:25.131Z Reads: 89

```
I would recheck your values for anything you may have changed on accident or something you may have missed.
```

---
## \#12 Posted by: LAVAMAN Posted at: 2017-12-19T22:55:31.982Z Reads: 87

```
I still have not solved my VESC issues. Under sensorless I have "Min ERPM" and also "BR ERPM" and also "Phase advance at BR ERPM" Which setting are you referring to and how much should I change it to? Increase by 100?
```

---
## \#13 Posted by: LAVAMAN Posted at: 2017-12-19T23:10:47.936Z Reads: 83

```
ok I am driving blind but I managed to get some information. Please see screen shot and tell me what this means.<img src="/uploads/db1493/original/3X/4/6/4644beae27f491bce8fe89f6da38f824d5d02671.jpg" width="690" height="425">
```

---
## \#14 Posted by: deucesdown Posted at: 2017-12-19T23:13:33.762Z Reads: 79

```
Double check your series voltage, make sure it's in the 6S range (at the XT90 that connects to vesc), and well above the battery cutoff numbers.

Make sure your XT90S are fully seated.

Is the motor new (known to be good)?

Have you tried switching the phase wires around?

Does VESC smell burned?

Look at VESC closely with magnifying glass and see if you can spot any short circuits or burned/exploded parts.

When you do BLDC motor detection does the motor make crazy noises like it's going to explode? (that's normal)
```

---
## \#15 Posted by: yelnats8j Posted at: 2017-12-19T23:13:40.736Z Reads: 77

```
Your getting a OVER_TEMP_FET falt code take a look at this. The search tool is useful.
http://www.electric-skateboard.builders/t/vesc-over-temp-fet/9134/7
```

---
## \#16 Posted by: deucesdown Posted at: 2017-12-19T23:19:09.656Z Reads: 79

```
[quote="yelnats8j, post:15, topic:41354"]
Your getting a OVER_TEMP_FET falt code
[/quote]


Yow 108.30 Deg C it says.

Does vesc get hot? especially the 3 fat chips on both sides (the mosfets)? yeinats8j's link is probably the best resource.
```

---
## \#17 Posted by: onepunchboard Posted at: 2017-12-19T23:26:03.215Z Reads: 73

```
when you do detection, should see min erpm 600. up this 700 800 900 like that
```

---
## \#18 Posted by: Namasaki Posted at: 2017-12-19T23:27:35.427Z Reads: 75

```
Maybe firmware issue causing false over temp signal
what firmware are you using?
```

---
## \#19 Posted by: Namasaki Posted at: 2017-12-19T23:31:34.042Z Reads: 76

```
Maybe my old friend Dexter, @torqueboards can shed some light here.
He helped me more than you can imagine when I was a newbie.
```

---
## \#20 Posted by: LAVAMAN Posted at: 2017-12-19T23:35:41.201Z Reads: 74

```
motor is brand new Enertion Big boy. XT90's are seated. don't see or smell anything burn't. Motor detect does nothing, no noise, no movement, nothing.
```

---
## \#21 Posted by: LAVAMAN Posted at: 2017-12-19T23:36:31.523Z Reads: 73

```
2.18 is version that is on the VESC
```

---
## \#22 Posted by: onepunchboard Posted at: 2017-12-19T23:38:27.570Z Reads: 68

```
thats strange motor should at least make noise. i think it's faulty vesc
```

---
## \#23 Posted by: LAVAMAN Posted at: 2017-12-19T23:38:56.841Z Reads: 69

```
Let me try that, thx
```

---
## \#24 Posted by: LAVAMAN Posted at: 2017-12-19T23:41:30.036Z Reads: 71

```
700, 800, 900 did not work
```

---
## \#25 Posted by: LAVAMAN Posted at: 2017-12-19T23:43:43.911Z Reads: 69

```
That is worth a try. Do I re flash with same firmware (basically re-load the software on the chip)?
```

---
## \#26 Posted by: onepunchboard Posted at: 2017-12-19T23:44:30.366Z Reads: 67

```
srry to hear that. u can up the detection amp up to 10 but if the motor doesnt make any noise you should  contact vesc seller.
```

---
## \#27 Posted by: LAVAMAN Posted at: 2017-12-19T23:44:35.231Z Reads: 62

```
no heat this thing is a cold fish
```

---
## \#28 Posted by: LAVAMAN Posted at: 2017-12-19T23:45:39.622Z Reads: 64

```
The only thing remotely warm are the LED's flashing red
```

---
## \#29 Posted by: onepunchboard Posted at: 2017-12-19T23:46:14.093Z Reads: 64

```
usually the led is blue when on
```

---
## \#30 Posted by: LAVAMAN Posted at: 2017-12-19T23:47:00.179Z Reads: 64

```
I guess I have to pay my dues with this hobby. I was hoping to get this thing on the road. I need to talk to Dexter.
```

---
## \#31 Posted by: LAVAMAN Posted at: 2017-12-19T23:48:25.178Z Reads: 66

```
You are correct. Thx
```

---
## \#32 Posted by: LAVAMAN Posted at: 2017-12-20T00:20:17.592Z Reads: 67

```
How do I re flash firmware? Where can I download firmware? My VESC might need a re-boot.
```

---
## \#33 Posted by: Namasaki Posted at: 2017-12-20T00:22:34.080Z Reads: 66

```
The firmware file is very small. pm me your email address and I will email it to you
You have Vesc 4.12 correct? Yes you do, it's right on the package.
```

---
## \#34 Posted by: Namasaki Posted at: 2017-12-20T02:37:00.399Z Reads: 64

```
BTW, your absolute max is too low at 80a.
It should be set between 130-150a
I run mine at 140a.
The absolute max is a last resort over current protection in case the soft back off strategies fail.
You really don't want to activate the absolute max protection.

<img src="/uploads/db1493/original/3X/2/d/2d47ab135868b1cd364ec4ea38ab5fa6d6af899f.png" width="690" height="319">
```

---
## \#35 Posted by: ThermalM16 Posted at: 2017-12-20T04:43:43.585Z Reads: 60

```
I know I read some of DIYs VESCs had defective thermistors on them a while ago, so that's a possibility, I'll put a gif below of how to check faults in BLDC tool. You should be able to run a duty cycle or something from the menu on the left and it'll throw faults without a motor connected if it's a defect on the VESC itself. The red light should blink if a fault code is thrown and here's how to check them. 
I typed "faults" after misspelling it and hit enter
https://gyazo.com/1e8a9c2612fb7e3d92c2c936382b8c0e
```

---
## \#36 Posted by: torqueboards Posted at: 2017-12-20T06:43:41.202Z Reads: 54

```
@LAVAMAN when did you get your VESC? Order #? PM me.
```

---
## \#37 Posted by: LAVAMAN Posted at: 2017-12-20T17:32:31.580Z Reads: 50

```
Thanks for this information. That is a possibility. I will wait to hear back from TB. I sent him my order # so he can check if I got a bad one. If not I can follow your advise and see if I can get a fault code from the BDLC tool or maybe re flash the VESC. Maybe it got hung up because I tried to do a motor detect with wheel and belt attached.
```

---
## \#38 Posted by: LAVAMAN Posted at: 2017-12-20T17:35:53.014Z Reads: 50

```
Thanks again for your assistance. After I hear back from TB, I will plan my next attempt to fix before ordering another VESC. Fault codes and firmware are next on the list of things to try.
```

---
## \#39 Posted by: Namasaki Posted at: 2017-12-20T18:39:14.719Z Reads: 45

```
[quote="LAVAMAN, post:37, topic:41354"]
Maybe it got hung up because I tried to do a motor detect with wheel and belt attached.
[/quote]

Too much drag on the motor during detection would cause an over current fault, not an over temp fault. 
It would probably take more than having the wheel and belt on to cause that fault unless maybe if your using a 15mm belt and it’s too tight. 
Still, I think it’s best to detect the motor with the shaft spinning free.
```

---
## \#40 Posted by: LAVAMAN Posted at: 2017-12-24T19:30:11.918Z Reads: 38

```
I tried to do a motor detect again with the following results. When I first connected the VESC and powered it up there were no flashing red LED's. I double checked my settings and did a read configuration and then it started flashing red again. I went to terminal screen and typed in faults (as instructed and got the following). seems to be the same issue, I am just not sure why.<img src="/uploads/db1493/original/3X/4/7/47143a6ab750bb41efc35bdfd700c943ab08831f.jpg" width="690" height="421"><img src="/uploads/db1493/original/3X/d/0/d0db36a3daf91eedf1c1ae048a7377670bf1463d.jpg" width="690" height="428">
```

---
## \#41 Posted by: LAVAMAN Posted at: 2018-01-05T20:09:16.339Z Reads: 25

```
Hey Dexter,
I got "The Board Tech" (thermalM16) to fix my VESC. He told me it was the thermistor that was defective and he repaired it for me for $45.00. I think it was this way when I received it from you. My question is this. Can I get a discount on my next order from you to offset the cost of the VESC repair? I have another build in mind. I want to do a single "sensored" motor, so I would need your 218mm mechanical kit, 190kv motor with 90mm black wheels and 15mm belt option. Let me know what you can do.

Thanks,

Mark Garey
```

---
